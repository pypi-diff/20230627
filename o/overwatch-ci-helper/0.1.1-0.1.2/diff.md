# Comparing `tmp/overwatch_ci_helper-0.1.1.tar.gz` & `tmp/overwatch_ci_helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overwatch_ci_helper-0.1.1.tar", max compression
+gzip compressed data, was "overwatch_ci_helper-0.1.2.tar", max compression
```

## Comparing `overwatch_ci_helper-0.1.1.tar` & `overwatch_ci_helper-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1037 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/README.md
--rw-r--r--   0        0        0     7126 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/overwatch_ci_helper/needs.py
--rw-r--r--   0        0        0     2297 2023-06-19 20:15:21.224854 overwatch_ci_helper-0.1.1/overwatch_ci_helper/template.config.yaml
--rw-r--r--   0        0        0      519 2023-06-19 20:15:21.228854 overwatch_ci_helper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 overwatch_ci_helper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-06-27 14:57:02.723881 overwatch_ci_helper-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 14:57:03.487907 overwatch_ci_helper-0.1.2/overwatch_ci_helper/__init__.py
+-rw-r--r--   0        0        0     8726 2023-06-27 14:57:02.723881 overwatch_ci_helper-0.1.2/overwatch_ci_helper/needs.py
+-rw-r--r--   0        0        0     2297 2023-06-27 14:57:02.727881 overwatch_ci_helper-0.1.2/overwatch_ci_helper/template.config.yaml
+-rw-r--r--   0        0        0      519 2023-06-27 14:57:02.727881 overwatch_ci_helper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 overwatch_ci_helper-0.1.2/PKG-INFO
```

### Comparing `overwatch_ci_helper-0.1.1/README.md` & `overwatch_ci_helper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `overwatch_ci_helper-0.1.1/overwatch_ci_helper/needs.py` & `overwatch_ci_helper-0.1.2/overwatch_ci_helper/needs.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,29 +21,34 @@
         else:
             d[k] = v
     return d
 
 
 
 def prep_directory(dependencies):
+    # create a filepath that does not already exist
     root_directory = os.path.join( tempfile.gettempdir(),f"ow-ci-helper-{str(uuid.uuid4())}" )
     while os.path.exists(root_directory):
+        # check if rootdir exists, and if so, try again
         root_directory = os.path.join( tempfile.gettempdir(),  str(uuid.uuid4()) )
+
+    # make a directory at the filepath
     os.mkdir(root_directory)
 
+    # volume mounts maps from dependancy to the directory corresponding to that dependancy
     volume_mounts = {}
     for dependency in dependencies:
+        # creates a directory at a file path off of root_directory, named after the dependancy
         dependency_dir = os.path.join( root_directory, dependency )
         os.mkdir(dependency_dir)
         if dependency in 'model-registry':
-            os.mkdir(os.path.join(dependency_dir, 'data-dir'))
-            os.mkdir(os.path.join(dependency_dir, 'data-dir', 'models'))
+            # if the dependancy is a model-registry, add a sub-directory for models
+            os.makedirs( os.path.join(dependency_dir, 'data-dir', 'models'), exist_ok=True)
         elif dependency in 'input-server':
-            os.mkdir(os.path.join(dependency_dir, 'data-dir'))
-            os.mkdir(os.path.join(dependency_dir, 'data-dir', 'inputs'))
+            os.makedirs( os.path.join(dependency_dir, 'data-dir', 'inputs'), exist_ok=True)
             
         volume_mounts[dependency] = dependency_dir
 
     return root_directory, volume_mounts
 
 def pull_image( client, image ):
     repo_name, tag = image.split(":")
@@ -58,31 +63,40 @@
     volume_path = os.path.join( root_volume_directory, dependency, 'config.yaml' )
     with open(volume_path, 'w') as f:
         f.write( yaml.dump(config, Dumper=Dumper) )
 
     mount_path = '/app/config.yaml'
 
     if dependency in ['input-server', 'overwatch-server' ]:
+        # the directory on the host machine which will be mapped to a directory in the docker container
+        host_dir = None
+
+        if 'INPUT_SERVER_DATA_DIR' in os.environ:
+            # if a bash variable has been set, use it for the data dir
+            host_dir = os.environ['INPUT_SERVER_DATA_DIR']
+        else:
+            # if no data dir is set, use the temp dir
+            host_dir = os.path.join( root_volume_directory, 'input-server', 'data-dir' )
+
         mounts.append(
             docker.types.Mount(
                 '/data-dir',
-                os.path.join( root_volume_directory, 'input-server', 'data-dir' ),
+                host_dir,
                 type = 'bind'
             )
         )
     else:
         mounts.append(
             docker.types.Mount(
                 '/data-dir',
                 os.path.join( root_volume_directory, dependency, 'data-dir' ),
                 type = 'bind'
             )
         )
 
-
     mounts.append(
         docker.types.Mount(mount_path, volume_path, read_only=True, type='bind')
     )
 
     return mounts
 
 def cleanup(client, dependencies, config):
@@ -96,53 +110,65 @@
             container = all_containers[dependency]
             container.stop()
             container.wait()
             mounts = container.attrs['Mounts']
             for mount in mounts:
                 if mount['Destination'] == '/root/.dcp':
                     continue
+                if mount['Source'] == os.environ.get('INPUT_SERVER_DATA_DIR'):
+                    # if the mount directory on the host machine is specified by CLI variable, do not delete it
+                    continue
                 if os.path.exists(mount['Source']) and os.path.isdir(mount['Source']):
                     shutil.rmtree(mount['Source'])
                 elif os.path.exists(mount['Source']):
                     os.remove(mount['Source'])
             container.remove()
             print(f"Done cleaning up {dependency}")
     print("Finished cleaning up all dependencies")
     return
 
 
 def satisfy_needs(client, dependencies, config, keystores):
     
+    # check if the keystore exists
     assert os.path.exists(keystores), f"Given keystore path does not exist: {keystores}"
 
+    # gets the running containers
     all_containers = {}
     for container in client.containers.list(all=True):
         all_containers[container.name] = container
 
+    # creates temp directories for the containers to mount volumes on
+    # root_volume_directory is the temp-dir that each of the dopendacy's volumes are contained within
+    # volume_mounts is an object mapping from dependancy names to the dir within root_volume_directory for that specific dependancy
     root_volume_directory, volume_mounts = prep_directory(dependencies)
 
     for dependency in dependencies:
+        # stops any running containers that are dependancies
         if dependency in list(all_containers.keys()):
             print(f"Stopping {dependency}")
             container = all_containers[dependency]
             container.stop()
             container.wait()
             container.remove()
             print(f"Stopped and removed {dependency}")
 
+        # checks that the dependancy has a config
         assert dependency in config.keys(), f"No config entry for {dependency}"
-
+        # gets the dependancy's config
         dependency_config = config[dependency]
         
-        mounts = make_mount_list( 
+
+        mounts = make_mount_list(
             dependency, 
             dependency_config, 
             root_volume_directory,
         )
 
+        # if the dependancy is overwatchserver, mount a directory for the keystore
         if dependency in 'overwatch-server':
             mounts.append(
                 docker.types.Mount(
                     '/root/.dcp',
                     keystores,
                     type='bind',
                     read_only=True,
@@ -158,15 +184,15 @@
         )
         container.rename(dependency)
         container.start()
     print(f"Finished deploying dependencies: {dependencies}")
 
 
 
-
+# creates and caches a docker client
 def setup_client():
     if hasattr(setup_client, "client"):
         return setup_client.client
     client = docker.from_env()
     pretty_client_info = json.dumps( client.version(), sort_keys=True, indent=2 )
     print(f"Connected to docker: \n{pretty_client_info}")
     setup_client.client = client
```

### Comparing `overwatch_ci_helper-0.1.1/overwatch_ci_helper/template.config.yaml` & `overwatch_ci_helper-0.1.2/overwatch_ci_helper/template.config.yaml`

 * *Files identical despite different names*

### Comparing `overwatch_ci_helper-0.1.1/pyproject.toml` & `overwatch_ci_helper-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overwatch-ci-helper"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [{include = "overwatch_ci_helper"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `overwatch_ci_helper-0.1.1/PKG-INFO` & `overwatch_ci_helper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overwatch-ci-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Hamada Gasmallah
 Author-email: hamada@distributive.network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

