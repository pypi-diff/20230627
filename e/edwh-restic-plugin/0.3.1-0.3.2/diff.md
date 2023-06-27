# Comparing `tmp/edwh_restic_plugin-0.3.1.tar.gz` & `tmp/edwh_restic_plugin-0.3.2.tar.gz`

## Comparing `edwh_restic_plugin-0.3.1.tar` & `edwh_restic_plugin-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    30323 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/README.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30451 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.2/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.3.1/CHANGELOG.md` & `edwh_restic_plugin-0.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.2 (2023-06-27)
+### Fix
+* Added expanduser() to check_env to make `~/` work ([`7d5fcd5`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/7d5fcd5eae40943f0d4e2143e89ea761373fec4a))
+
 ## v0.3.1 (2023-06-20)
 ### Fix
 * Fixed color coding in restic plugin. now doesn't only print in white but in set color of the cmd ([`80ad277`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/80ad27717a89c9843b62d002e214493ad428c39c))
 
 ## v0.3.0 (2023-06-09)
 ### Feature
 * Edwh-restic-plugin now exist with the highest status code one of the given shell scripts gave it ([`281f600`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/281f600082cba3853b1bc35efda93ea50ea8f3b5))
```

### Comparing `edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.3.2/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.3.2/src/edwh_restic_plugin/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -675,14 +675,16 @@
     if key in env:
         return env[key]
     with path.open(mode="r+") as env_file:
         # get response value from prompt/input
         response = input(f"Enter value for {key} ({comment})\n default=`{default}`: ")
         # if response_value is none make value default else value is response_value
         value = response.strip() or default
+        if value.startswith("~/") and Path(value).expanduser().exists():
+            value = Path(value).expanduser().__str__()
         if prefix:
             value = prefix + value
         if postfix:
             value += postfix
         env_file.seek(0, 2)
         # write key and value to .env file
         env_file.write(f"\n{key.upper()}={value}\n")
```

### Comparing `edwh_restic_plugin-0.3.1/LICENSE.txt` & `edwh_restic_plugin-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.1/README.md` & `edwh_restic_plugin-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.1/pyproject.toml` & `edwh_restic_plugin-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.1/PKG-INFO` & `edwh_restic_plugin-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.3.1
+Version: 0.3.2
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

