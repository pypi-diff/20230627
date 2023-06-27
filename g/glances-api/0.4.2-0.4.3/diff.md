# Comparing `tmp/glances_api-0.4.2.tar.gz` & `tmp/glances_api-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances_api-0.4.2.tar", max compression
+gzip compressed data, was "glances_api-0.4.3.tar", max compression
```

## Comparing `glances_api-0.4.2.tar` & `glances_api-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1110 2023-05-21 11:03:42.721345 glances_api-0.4.2/LICENSE
--rw-r--r--   0        0        0      956 2023-05-21 11:03:42.721345 glances_api-0.4.2/README.rst
--rw-r--r--   0        0        0     5820 2023-05-21 11:03:42.721345 glances_api-0.4.2/glances_api/__init__.py
--rw-r--r--   0        0        0      459 2023-05-21 11:03:42.721345 glances_api-0.4.2/glances_api/exceptions.py
--rw-r--r--   0        0        0     1388 2023-05-21 11:08:13.471569 glances_api-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 glances_api-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-21 11:03:42.721345 glances_api-0.4.3/LICENSE
+-rw-r--r--   0        0        0      956 2023-05-21 11:03:42.721345 glances_api-0.4.3/README.rst
+-rw-r--r--   0        0        0     6349 2023-06-27 21:00:09.751357 glances_api-0.4.3/glances_api/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-21 11:03:42.721345 glances_api-0.4.3/glances_api/exceptions.py
+-rw-r--r--   0        0        0     1388 2023-06-27 21:04:27.968570 glances_api-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 glances_api-0.4.3/PKG-INFO
```

### Comparing `glances_api-0.4.2/LICENSE` & `glances_api-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glances_api-0.4.2/README.rst` & `glances_api-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `glances_api-0.4.2/glances_api/__init__.py` & `glances_api-0.4.3/glances_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,23 @@
                 "process_running": data["running"],
                 "process_total": data["total"],
                 "process_thread": data["thread"],
                 "process_sleeping": data["sleeping"],
             }
         if data := self.data.get("quicklook"):
             sensor_data["cpu"] = {"cpu_use_percent": data["cpu"]}
+        if networks := self.data.get("network"):
+            sensor_data["network"] = {}
+            for network in networks:
+                sensor_data["network"][network["interface_name"]] = {
+                    "is_up": network["is_up"],
+                    "rx": round(network["rx"] / 1024, 1),
+                    "tx": round(network["tx"] / 1024, 1),
+                    "speed": round(network["speed"] / 1024**3, 1),
+                }
         if "docker" in self.data and (data := self.data["docker"].get("containers")):
             active_containers = [
                 container for container in data if container["Status"] == "running"
             ]
             sensor_data["docker"] = {"docker_active": len(active_containers)}
             cpu_use = 0.0
             for container in active_containers:
@@ -146,8 +155,10 @@
             sensor_data["docker"]["docker_cpu_use"] = round(cpu_use, 1)
             mem_use = 0.0
             for container in active_containers:
                 mem_use += container["memory"].get("usage", 0)
             sensor_data["docker"]["docker_memory_use"] = round(mem_use / 1024**2, 1)
         if data := self.data.get("raid"):
             sensor_data["raid"] = data
+        if data := self.data.get("uptime"):
+            sensor_data["uptime"] = data
         return sensor_data
```

### Comparing `glances_api-0.4.2/pyproject.toml` & `glances_api-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glances_api"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python API for interacting with Glances"
 authors = ["Fabian Affolter <fabian@affolter-engineering.ch>"]
 homepage = "https://github.com/home-assistant-ecosystem/python-glances-api"
 repository = "https://github.com/home-assistant-ecosystem/python-glances-api/releases"
 readme = "README.rst"
 license = "MIT"
 classifiers = [
@@ -19,15 +19,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = ">=0.23,<1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3"
-pytest = "^7.1.2"
+pytest = "^7.3.0"
 pytest-httpx = ">0.15,<1"
 pytest-asyncio = "^0.16.0"
 isort = "^5.10.0"
 mypy = "^0.971"
 
 [tool.mypy]
 check_untyped_defs = true
```

### Comparing `glances_api-0.4.2/PKG-INFO` & `glances_api-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glances-api
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python API for interacting with Glances
 Home-page: https://github.com/home-assistant-ecosystem/python-glances-api
 License: MIT
 Author: Fabian Affolter
 Author-email: fabian@affolter-engineering.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

