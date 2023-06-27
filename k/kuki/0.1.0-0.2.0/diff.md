# Comparing `tmp/kuki-0.1.0.tar.gz` & `tmp/kuki-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.1.0.tar", last modified: Sun May  7 13:59:20 2023, max compression
+gzip compressed data, was "kuki-0.2.0.tar", last modified: Tue Jun 27 13:17:13 2023, max compression
```

## Comparing `kuki-0.1.0.tar` & `kuki-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,38 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:59:20.276850 kuki-0.1.0/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.1.0/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12697 2023-05-07 13:59:20.276850 kuki-0.1.0/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1116 2023-05-07 13:57:13.000000 kuki-0.1.0/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:59:20.275849 kuki-0.1.0/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.1.0/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      864 2023-05-07 13:15:07.000000 kuki-0.1.0/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       21 2023-05-07 13:14:38.000000 kuki-0.1.0/kuki/krun.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3373 2023-05-07 13:15:07.000000 kuki-0.1.0/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3268 2023-05-07 13:15:07.000000 kuki-0.1.0/kuki/package_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13352 2023-05-07 13:15:07.000000 kuki-0.1.0/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-05-07 13:57:34.000000 kuki-0.1.0/kuki/version.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:59:20.275849 kuki-0.1.0/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12697 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      373 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       62 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        5 2023-05-07 13:59:20.000000 kuki-0.1.0/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      451 2023-05-07 13:59:20.276850 kuki-0.1.0/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      280 2023-05-07 13:14:38.000000 kuki-0.1.0/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:59:20.275849 kuki-0.1.0/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14229 2023-05-07 13:15:07.000000 kuki-0.1.0/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/
+-rw-r--r--   0 jshinonome  (1000) users      (100)    11357 2023-06-15 05:01:08.000000 kuki-0.2.0/LICENSE
+-rw-r--r--   0 jshinonome  (1000) users      (100)    12993 2023-06-27 13:17:13.765620 kuki-0.2.0/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) users      (100)     1412 2023-06-27 13:15:32.000000 kuki-0.2.0/README.md
+drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki/
+-rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     1176 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     4844 2023-06-27 08:58:19.000000 kuki-0.2.0/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     3088 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/krun.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     3371 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     3313 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/package_util.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)      279 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/profile_util.py
+drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 12:26:24.000000 kuki-0.2.0/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     3262 2023-06-27 13:09:13.000000 kuki-0.2.0/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)     6359 2023-06-27 11:09:55.000000 kuki-0.2.0/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/q/krun.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)     1958 2023-06-27 10:44:52.000000 kuki-0.2.0/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)     2177 2023-06-20 14:00:10.000000 kuki-0.2.0/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)      878 2023-06-27 09:49:09.000000 kuki-0.2.0/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) users      (100)    13261 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     2141 2023-06-27 11:04:34.000000 kuki-0.2.0/kuki/util.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)       22 2023-06-27 13:10:22.000000 kuki-0.2.0/kuki/version.py
+drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) users      (100)    12993 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) users      (100)      573 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) users      (100)        1 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) users      (100)       84 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) users      (100)        1 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) users      (100)       17 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) users      (100)       10 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) users      (100)      486 2023-06-27 13:17:13.765620 kuki-0.2.0/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) users      (100)      315 2023-06-15 11:42:17.000000 kuki-0.2.0/setup.py
+drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/test/
+-rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)     1605 2023-06-15 12:34:54.000000 kuki-0.2.0/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) users      (100)    14435 2023-06-15 05:01:08.000000 kuki-0.2.0/test/test_kuki.py
```

### Comparing `kuki-0.1.0/LICENSE` & `kuki-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.1.0/PKG-INFO` & `kuki-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.1.0
+Version: 0.2.0
 Summary: kdb+/q package manager
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: kdb,q
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Kdb Ultimate pacKage Installer
+## K Ultimate pacKage Installer
 
 - use the same registry site as the npm
 - use file `$HOME/.kukirc.json` to configure local registry site and token
 - default local repo: `$HOME/kuki`, use environment variable `KUKIPATH` to overwrite local repo
 - `kuki.json` to maintain package dependencies
 - `kuki_index.json` to maintain indices of all required packages. For a version conflict:
   - it will use dependency version if it is a dependency
   - latest version if it is not a dependency
 
 ### Command: kuki
 
+K Ultimate pacKage Installer
+
 #### config
 
 use format 'field=value'
 
 ```bash
 kuki --config registry=https://localhost token=some_token
 ```
@@ -67,14 +69,36 @@
 
 uninstall a package from current working package
 
 ```bash
 kuki --uninstall dummy
 ```
 
+### Command: kest
+
+K tEST CLI
+
+#### Define Test
+
+- `.kest.Test`
+
+#### Setup and Teardown
+
+- `.kest.BeforeAll`
+- `.kest.AfterAll`
+- `.kest.BeforeEach`
+- `.kest.AfterEach`
+
+#### Using Matchers
+
+- `.kest.ToThrow`
+- `.kest.Match`
+- `.kest.MatchTable`
+- `.kest.MatchDict`
+
 ### Command: krun
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.1.0/README.md` & `kuki-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-## Kdb Ultimate pacKage Installer
+## K Ultimate pacKage Installer
 
 - use the same registry site as the npm
 - use file `$HOME/.kukirc.json` to configure local registry site and token
 - default local repo: `$HOME/kuki`, use environment variable `KUKIPATH` to overwrite local repo
 - `kuki.json` to maintain package dependencies
 - `kuki_index.json` to maintain indices of all required packages. For a version conflict:
   - it will use dependency version if it is a dependency
   - latest version if it is not a dependency
 
 ### Command: kuki
 
+K Ultimate pacKage Installer
+
 #### config
 
 use format 'field=value'
 
 ```bash
 kuki --config registry=https://localhost token=some_token
 ```
@@ -56,8 +58,30 @@
 
 uninstall a package from current working package
 
 ```bash
 kuki --uninstall dummy
 ```
 
+### Command: kest
+
+K tEST CLI
+
+#### Define Test
+
+- `.kest.Test`
+
+#### Setup and Teardown
+
+- `.kest.BeforeAll`
+- `.kest.AfterAll`
+- `.kest.BeforeEach`
+- `.kest.AfterEach`
+
+#### Using Matchers
+
+- `.kest.ToThrow`
+- `.kest.Match`
+- `.kest.MatchTable`
+- `.kest.MatchDict`
+
 ### Command: krun
```

### Comparing `kuki-0.1.0/kuki/kuki.py` & `kuki-0.2.0/kuki/kuki.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 FORMAT = "%(asctime)s %(levelname)s: %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 logging.basicConfig(level=logging.INFO, format=FORMAT, datefmt=DATE_FORMAT)
 
 logger = logging.getLogger()
 
-parser = argparse.ArgumentParser(description="Kdb Ultimate pacKage Installer CLI")
+parser = argparse.ArgumentParser(description="K Ultimate pacKage Installer CLI")
 
 group = parser.add_mutually_exclusive_group()
 
 group.add_argument(
     "-a",
     "--adduser",
     action="store_true",
```

### Comparing `kuki-0.1.0/kuki/package_util.py` & `kuki-0.2.0/kuki/package_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 logger = logging.getLogger()
 config_file = "kuki.json"
 index_file = "kuki_index.json"
 readme_file = "README.md"
 
 package_path = Path.cwd()
 readme_path = Path(readme_file)
-kuki_config_path = Path(config_file)
-kuki_include_path = Path(".kukiinclude")
-kuki_index_path = Path(index_file)
+package_config_path = Path(config_file)
+package_include_path = Path(".kukiinclude")
+package_index_path = Path(index_file)
 
 
 class Kuki(TypedDict):
     name: str
     version: str
     description: str
     author: str
     git: str
     dependencies: Dict[str, str]
 
 
 def generate_json(name: str, description="", author="", git=""):
-    if kuki_config_path.exists():
+    if package_config_path.exists():
         overwrite = input("kuki.json already exists, overwrite: (yes/No) ").strip()
         if not overwrite or not overwrite.lower() in ["yes"]:
             return
     kuki: Kuki = {
         "name": name,
         "version": "0.0.1",
         "description": description,
         "author": author,
         "git": git,
         "dependencies": {},
     }
     kuki_json = json.dumps(kuki, indent=2)
-    logger.info("About to write to {}".format(kuki_config_path))
+    logger.info("About to write to {}".format(package_config_path))
     logger.info("\n" + kuki_json)
     proceed = input("Is this OK? (YES/no) ").strip()
     if not proceed or proceed.lower() == "yes":
         dump_kuki(kuki)
         readme_path.touch()
 
 
@@ -56,24 +56,24 @@
     author = input("author: ").strip()
     git = input("git repository: ").strip()
 
     generate_json(package, description, author, git)
 
 
 def dump_kuki(kuki: Kuki):
-    with open(kuki_config_path, "w") as file:
+    with open(package_config_path, "w") as file:
         file.write(json.dumps(kuki, indent=2))
 
 
 def exits():
-    return kuki_config_path.exists()
+    return package_config_path.exists()
 
 
 def roll_up_version(type: str):
-    kuki: Kuki = json.loads(kuki_config_path.read_text())
+    kuki: Kuki = json.loads(package_config_path.read_text())
     logger.info("roll up version")
     logger.info("from - " + kuki["version"])
     [major, minor, patch] = list(map(int, kuki["version"].split(".")))
     if type == "patch":
         patch += 1
     elif type == "minor":
         minor += 1
@@ -85,39 +85,39 @@
     version = "{}.{}.{}".format(major, minor, patch)
     kuki["version"] = version
     logger.info("to   - " + version)
     dump_kuki(kuki)
 
 
 def load_kuki() -> Kuki:
-    if kuki_config_path.exists():
-        return json.loads(kuki_config_path.read_text())
+    if package_config_path.exists():
+        return json.loads(package_config_path.read_text())
     else:
         return {}
 
 
 def load_include() -> List[str]:
     includes = set(["src/*", "lib/*", config_file, readme_file])
-    if kuki_include_path.exists():
-        with open(kuki_include_path, "r") as file:
+    if package_include_path.exists():
+        with open(package_include_path, "r") as file:
             while line := file.readline():
                 if line.strip() != "":
                     includes.add(line.strip())
     return includes
 
 
 def load_readme() -> str:
     with open(readme_path, "r") as file:
         return file.read()
 
 
 def load_pkg_index() -> Dict[str, Kuki]:
-    if kuki_index_path.exists():
-        with open(kuki_index_path, "r") as file:
+    if package_index_path.exists():
+        with open(package_index_path, "r") as file:
             return json.load(file)
     else:
         return {}
 
 
 def dump_pkg_index(kuki_index: Dict[str, Kuki]):
-    with open(kuki_index_path, "w") as file:
+    with open(package_index_path, "w") as file:
         json.dump(kuki_index, file, indent=2)
```

### Comparing `kuki-0.1.0/kuki/registry_util.py` & `kuki-0.2.0/kuki/registry_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,23 @@
 from . import config_util, package_util
 
 logger = logging.getLogger()
 config = config_util.load_config()
 registry = config.get("registry", "http://0.0.0.0:4873/")
 token = config.get("token", "")
 
-global_repo_path = (
-    Path(os.getenv("KUKIPATH")) if os.getenv("KUKIPATH") else Path.joinpath(Path.home(), "kuki")
-)
-
-global_cache_path = Path.joinpath(global_repo_path, ".cache")
-global_index_path = Path.joinpath(global_repo_path, ".index")
+global_cache_dir = Path.joinpath(config_util.global_kuki_root, "_cache")
+global_index_path = Path.joinpath(config_util.global_kuki_root, ".index")
 
 kuki_json = package_util.load_kuki()
 
-if global_cache_path.exists() and not global_cache_path.is_dir():
-    os.remove(str(global_cache_path))
+if global_cache_dir.exists() and not global_cache_dir.is_dir():
+    os.remove(str(global_cache_dir))
 
-global_cache_path.mkdir(parents=True, exist_ok=True)
+global_cache_dir.mkdir(parents=True, exist_ok=True)
 
 user_url = registry + "-/user/org.couchdb.user:"
 search_url = registry + "-/v1/search?text={}"
 
 package_index = package_util.load_pkg_index()
 
 
@@ -202,15 +198,15 @@
 
 
 def get_tar_name(name: str, version: str):
     return "{}-v{}.tgz".format(name, version)
 
 
 def get_pkg_path(name: str, version: str):
-    return Path.joinpath(global_repo_path, name, version)
+    return Path.joinpath(config_util.global_kuki_root, name, version)
 
 
 def get_pkg_id(metadata: Metadata):
     return "{}@{}".format(metadata["name"], metadata["version"])
 
 
 def get_metadata(name: str) -> Metadata:
@@ -238,15 +234,15 @@
     if os.path.isfile(filepath) and os.path.getsize(filepath) > 0:
         return True
     else:
         return False
 
 
 def get_cached_filepath(tar_name) -> str:
-    return str(Path.joinpath(global_cache_path, tar_name))
+    return str(Path.joinpath(global_cache_dir, tar_name))
 
 
 def download_entry(name: str):
     try:
         metadata = get_metadata(name)
         pkg_filepath = download_package(metadata)
         shutil.copy(pkg_filepath, os.path.basename(pkg_filepath))
```

### Comparing `kuki-0.1.0/kuki.egg-info/PKG-INFO` & `kuki-0.2.0/kuki.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.1.0
+Version: 0.2.0
 Summary: kdb+/q package manager
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: kdb,q
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Kdb Ultimate pacKage Installer
+## K Ultimate pacKage Installer
 
 - use the same registry site as the npm
 - use file `$HOME/.kukirc.json` to configure local registry site and token
 - default local repo: `$HOME/kuki`, use environment variable `KUKIPATH` to overwrite local repo
 - `kuki.json` to maintain package dependencies
 - `kuki_index.json` to maintain indices of all required packages. For a version conflict:
   - it will use dependency version if it is a dependency
   - latest version if it is not a dependency
 
 ### Command: kuki
 
+K Ultimate pacKage Installer
+
 #### config
 
 use format 'field=value'
 
 ```bash
 kuki --config registry=https://localhost token=some_token
 ```
@@ -67,14 +69,36 @@
 
 uninstall a package from current working package
 
 ```bash
 kuki --uninstall dummy
 ```
 
+### Command: kest
+
+K tEST CLI
+
+#### Define Test
+
+- `.kest.Test`
+
+#### Setup and Teardown
+
+- `.kest.BeforeAll`
+- `.kest.AfterAll`
+- `.kest.BeforeEach`
+- `.kest.AfterEach`
+
+#### Using Matchers
+
+- `.kest.ToThrow`
+- `.kest.Match`
+- `.kest.MatchTable`
+- `.kest.MatchDict`
+
 ### Command: krun
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.1.0/test/test_kuki.py` & `kuki-0.2.0/test/test_kuki.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,37 @@
 def tmp_dir(tmp_path_factory: pytest.TempPathFactory, monkeypatch: pytest.MonkeyPatch):
     # generate new dir every run
     dir = tmp_path_factory.mktemp("kuki")
 
     home = Path.joinpath(dir, "home")
     home.mkdir(parents=True, exist_ok=True)
 
-    config_util.config_path = Path.joinpath(home, config_util.config_file)
-    global_repo_path = Path.joinpath(home, "kuki")
-    global_repo_path.mkdir(parents=True, exist_ok=True)
-    registry_util.global_repo_path = global_repo_path
+    global_kuki_root = Path.joinpath(home, "kuki")
+    global_kuki_root.mkdir(parents=True, exist_ok=True)
+    config_util.global_kuki_root = global_kuki_root
 
-    global_cache_path = Path.joinpath(global_repo_path, ".cache")
+    config_util.global_config_dir = Path.joinpath(config_util.global_kuki_root, "config")
+
+    config_util.global_config_dir.mkdir(parents=True, exist_ok=True)
+    config_util.global_config_path = Path.joinpath(
+        config_util.global_config_dir, config_util.config_file
+    )
+
+    global_cache_path = Path.joinpath(global_kuki_root, ".cache")
     global_cache_path.mkdir(parents=True, exist_ok=True)
-    registry_util.global_cache_path = global_cache_path
+    registry_util.global_cache_dir = global_cache_path
 
-    global_index_path = Path.joinpath(global_repo_path, ".index")
+    global_index_path = Path.joinpath(global_kuki_root, ".index")
     registry_util.global_index_path = global_index_path
 
     dummy_package = Path.joinpath(dir, "dummy")
     dummy_package.mkdir(parents=True, exist_ok=True)
 
     package_util.package_path = dummy_package
-    package_util.kuki_config_path = Path.joinpath(dummy_package, package_util.config_file)
+    package_util.package_config_path = Path.joinpath(dummy_package, package_util.config_file)
     monkeypatch.chdir(dummy_package)
 
     registry_util.package_index = package_util.load_pkg_index()
     registry_util.global_index = registry_util.load_global_index()
     return dir
 
 
@@ -291,15 +297,15 @@
     sorted_tar_files = sorted(tar_files)
     for i, file in enumerate(sorted_tar_files):
         assert file == sorted_source_files[i]
 
     tar.close()
 
     # test includes
-    with open(package_util.kuki_include_path, "w") as file:
+    with open(package_util.package_include_path, "w") as file:
         file.writelines(["conf*", ""])
 
     run_kuki("--publish")
 
     assert tar_path.exists()
 
     tar = tarfile.open(str(tar_path), "r:gz")
@@ -385,15 +391,15 @@
     run_kuki(command_params)
     global_index = registry_util.load_global_index()
     assert len(global_index) == len(expected_index)
 
     for pkg_id in expected_index:
         assert pkg_id in global_index
         name, version = pkg_id.split("@")
-        pkg_dir = Path.joinpath(registry_util.global_repo_path, name, version)
+        pkg_dir = Path.joinpath(config_util.global_kuki_root, name, version)
         assert Path.joinpath(pkg_dir, package_util.config_file).exists()
 
     pkg_index = package_util.load_pkg_index()
     assert len(pkg_index) == len(expected_pkg_index)
     for pkg in expected_pkg_index:
         assert pkg in pkg_index
 
@@ -446,15 +452,15 @@
     run_kuki(command_params)
     global_index = registry_util.load_global_index()
     assert len(global_index) == len(expected_index)
 
     for pkg_id in expected_index:
         assert pkg_id in global_index
         name, version = pkg_id.split("@")
-        pkg_dir = Path.joinpath(registry_util.global_repo_path, name, version)
+        pkg_dir = Path.joinpath(config_util.global_kuki_root, name, version)
         assert Path.joinpath(pkg_dir, package_util.config_file).exists()
 
     pkg_index = package_util.load_pkg_index()
     assert len(pkg_index) == len(expected_pkg_index)
     for pkg in expected_pkg_index:
         assert pkg in pkg_index
```

