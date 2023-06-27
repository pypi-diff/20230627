# Comparing `tmp/nonebot_plugin_setu_now-0.6.1.tar.gz` & `tmp/nonebot_plugin_setu_now-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_setu_now-0.6.1.tar", last modified: Mon Jun 26 06:30:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_setu_now-0.6.2.tar", last modified: Tue Jun 27 09:17:54 2023, max compression
```

## Comparing `nonebot_plugin_setu_now-0.6.1.tar` & `nonebot_plugin_setu_now-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/LICENSE
--rw-r--r--   0        0        0     3403 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/README.md
--rwxr-xr-x   0        0        0     7467 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/__init__.py
--rw-r--r--   0        0        0      305 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/__init__.py
--rw-r--r--   0        0        0     3922 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/_main.py
--rw-r--r--   0        0        0     1030 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/config.py
--rw-r--r--   0        0        0     2340 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/data_source.py
--rw-r--r--   0        0        0     1047 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/database.py
--rw-r--r--   0        0        0     4262 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/img_utils.py
--rw-r--r--   0        0        0      959 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/models.py
--rw-r--r--   0        0        0      613 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/perf_timer.py
--rw-r--r--   0        0        0     1640 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/r18_whitelist.py
--rw-r--r--   0        0        0     2964 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/utils.py
--rw-r--r--   0        0        0      799 2023-06-26 06:30:51.727846 nonebot_plugin_setu_now-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-27 09:17:42.000607 nonebot_plugin_setu_now-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3403 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/README.md
+-rwxr-xr-x   0        0        0     7534 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/__init__.py
+-rw-r--r--   0        0        0     3922 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/_main.py
+-rw-r--r--   0        0        0     1030 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/config.py
+-rw-r--r--   0        0        0     2340 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/data_source.py
+-rw-r--r--   0        0        0     1047 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/database.py
+-rw-r--r--   0        0        0     4262 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/img_utils.py
+-rw-r--r--   0        0        0      959 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/models.py
+-rw-r--r--   0        0        0      613 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/perf_timer.py
+-rw-r--r--   0        0        0     1640 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/r18_whitelist.py
+-rw-r--r--   0        0        0     2964 2023-06-27 09:17:42.004608 nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/utils.py
+-rw-r--r--   0        0        0      797 2023-06-27 09:17:54.784708 nonebot_plugin_setu_now-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.2/PKG-INFO
```

### Comparing `nonebot_plugin_setu_now-0.6.1/LICENSE` & `nonebot_plugin_setu_now-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/README.md` & `nonebot_plugin_setu_now-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/__init__.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 usage_msg = """TL;DR: 色图 或 看文档"""
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-setu-now",
     description="另一个色图插件",
     usage=usage_msg,
     type="application",
+    homepage="https://github.com/kexue-z/nonebot-plugin-setu-now",
     config=Config,
     extra={},
 )
 
 
 add_model("nonebot_plugin_setu_now.database")
```

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/_main.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/aioutils/_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/config.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/data_source.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/database.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/database.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/img_utils.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/img_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/models.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/perf_timer.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/perf_timer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/r18_whitelist.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/r18_whitelist.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/utils.py` & `nonebot_plugin_setu_now-0.6.2/nonebot_plugin_setu_now/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.1/pyproject.toml` & `nonebot_plugin_setu_now-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "nonebot-plugin-setu-now"
-version = "0.6.1"
+version = "0.6.2"
 description = "另一个色图插件"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.0.0",
     "pydantic>=1.5.0",
     "pillow>=8.0.0",
-    "nonebot-plugin-tortoise-orm>=0.0.1a3",
+    "nonebot-plugin-tortoise-orm>=0.1.0",
     "nonebot-plugin-localstore>=0.5.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_setu_now-0.6.1/PKG-INFO` & `nonebot_plugin_setu_now-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-setu-now
-Version: 0.6.1
+Version: 0.6.2
 Summary: 另一个色图插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-setu-now
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-setu-now
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx<1.0.0,>=0.18.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.0.0
 Requires-Dist: pydantic>=1.5.0
 Requires-Dist: pillow>=8.0.0
-Requires-Dist: nonebot-plugin-tortoise-orm>=0.0.1a3
+Requires-Dist: nonebot-plugin-tortoise-orm>=0.1.0
 Requires-Dist: nonebot-plugin-localstore>=0.5.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://user-images.githubusercontent.com/44545625/209862575-acdc9feb-3c76-471d-ad89-cc78927e5875.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.2 Summary:
 å¦ä¸ä¸ªè²å¾æä»¶ Home-page: https://github.com/kexue-z/nonebot-plugin-
 setu-now Author-Email: kexue
 foxmail.com> License: MIT Project-URL: Homepage, https://github.com/kexue-z/
 nonebot-plugin-setu-now Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx<1.0.0,>=0.18.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0 Requires-Dist: pydantic>=1.5.0 Requires-Dist:
-pillow>=8.0.0 Requires-Dist: nonebot-plugin-tortoise-orm>=0.0.1a3 Requires-
-Dist: nonebot-plugin-localstore>=0.5.0 Description-Content-Type: text/markdown
+pillow>=8.0.0 Requires-Dist: nonebot-plugin-tortoise-orm>=0.1.0 Requires-Dist:
+nonebot-plugin-localstore>=0.5.0 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
            # nonebot-plugin-setu-now _â¨ NoneBot2 æ¶©å¾æä»¶ â¨_
                            [license] [pypi] [python]
 ## ç®ä» å¯éè¿ç¾¤èæç§èè·å Pixiv æ¶©å¾ç NoneBot2 æä»¶ ##
 ç¹è² - **æé«çæ¶©å¾åéæåçï¼ä»é0.5.0ä»¥ä¸æ°çæ¬ï¼** -
 éè¿åå¤è·åå¾çä¿¡æ¯ - èªå¨æ¤åæ¶©å¾ - R18ç½ååç¾¤ç» -
 èªå¨æ¤åæ¶©å¾ - ç¬ç«çä¸è½½åéä»»å¡ç»æï¼éåº¦æ´å¿« ## å®è£
```

