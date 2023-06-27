# Comparing `tmp/liteclashproman-0.1.4.tar.gz` & `tmp/liteclashproman-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.1.4.tar", last modified: Sat Jun 10 05:08:44 2023, max compression
+gzip compressed data, was "liteclashproman-0.2.0.tar", last modified: Tue Jun 27 13:01:39 2023, max compression
```

## Comparing `liteclashproman-0.1.4.tar` & `liteclashproman-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LICENSE
--rw-r--r--   0        0        0     1177 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3565 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1782 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/log.py
--rw-r--r--   0        0        0     1936 2023-06-10 05:08:32.655111 liteclashproman-0.1.4/LiteClashProMan/main.py
--rw-r--r--   0        0        0     2008 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      379 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     3637 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     2226 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      774 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1530 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1789 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-06-10 05:08:32.659111 liteclashproman-0.1.4/README.md
--rw-r--r--   0        0        0      595 2023-06-10 05:08:44.387228 liteclashproman-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 liteclashproman-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1177 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     3595 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1782 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     2175 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     2008 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      379 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     3827 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3508 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2607 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     2226 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      774 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1530 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1789 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-06-27 13:01:24.126191 liteclashproman-0.2.0/README.md
+-rw-r--r--   0        0        0      675 2023-06-27 13:01:39.870248 liteclashproman-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 liteclashproman-0.2.0/PKG-INFO
```

### Comparing `liteclashproman-0.1.4/LICENSE` & `liteclashproman-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/__init__.py` & `liteclashproman-0.2.0/LiteClashProMan/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/config.py` & `liteclashproman-0.2.0/LiteClashProMan/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     subs: List[str] = []
 
 
 class Config(BaseModel, extra=Extra.ignore):
     log_level: Literal[
         "TRACE", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
     ] = "INFO"
+    sentry_dsn: Optional[str]
 
     download_thread: int = 4
     download_retry: int = 3
     download_proxy: Optional[str] = None
 
     update_cron: str = "35 6 * * *"
     update_tz: str = "Asia/Shanghai"
```

### Comparing `liteclashproman-0.1.4/LiteClashProMan/log.py` & `liteclashproman-0.2.0/LiteClashProMan/log.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/main.py` & `liteclashproman-0.2.0/LiteClashProMan/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from loguru import logger
 from starlette.responses import FileResponse
 
 from .config import config
 from .log import LOGGING_CONFIG
 from .subscribe import counter, update
 
+if config.sentry_dsn:
+    import sentry_sdk
+
+    sentry_sdk.init(
+        dsn=config.sentry_dsn,
+        traces_sample_rate=1.0,
+    )
+
+
 app = FastAPI()
 
 # provider download
 app.mount(f"/{config.urlprefix}/provider", StaticFiles(directory="data/provider"))
 
 
 # profile download
@@ -37,14 +46,18 @@
 # manual update trigger
 @app.get(f"/{config.urlprefix}/update")
 async def _():
     logger.info("Update is triggered manually")
     error = await update()
     return str(error) or "update complete"
 
+# test sentry debug
+@app.get("/sentry-debug")
+async def trigger_error():
+    division_by_zero = 1 / 0
 
 @app.on_event("startup")
 async def startup_event():
     error = await update()
     if error:
         raise error
     logger.info(
```

### Comparing `liteclashproman-0.1.4/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.2.0/LiteClashProMan/model/clash/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.2.0/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.2.0/LiteClashProMan/static/config.exp.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # ============================== 日志相关设置 ==============================
 ## 终端输出的日志等级，取值范围如下，排名越靠后其等级越高、详细程度越低、内容越少
 ## TRACE / DEBUG / INFO / WARNING / ERROR / CRITICAL       推荐取 INFO 即可
 log_level: INFO
+## 使用 sentry.io 进行异常捕获，并提示账号所有者
+## 需要额外的依赖 sentry-sdk[fastapi]，或LiteClashProMan[extra]
+# sentry_dsn: https://xxxx.ingest.sentry.io/xxxxxx
 
 # ============================== 下载相关设置 ==============================
 ## 下载的最大携程数，服务器网络质量越好可以设置的值越高
 download_thread: 3
 ## 下载失败的重试次数，若服务器网络质量较差，建议设置较高数值
 download_retry: 3
 ## 下载使用的代理地址
```

### Comparing `liteclashproman-0.1.4/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.2.0/LiteClashProMan/static/template/blacklist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.2.0/LiteClashProMan/static/template/whitelist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.2.0/LiteClashProMan/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.2.0/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.2.0/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.2.0/LiteClashProMan/subscribe/jms.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/LiteClashProMan/utils.py` & `liteclashproman-0.2.0/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/README.md` & `liteclashproman-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.1.4/pyproject.toml` & `liteclashproman-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.1.4"
+version = "0.2.0"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
@@ -14,14 +14,19 @@
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "APGL-3.0"
 
+[project.optional-dependencies]
+extra = [
+    "sentry-sdk[fastapi]>=1.26.0",
+]
+
 [project.scripts]
 lcpm = "LiteClashProMan.__init__:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `liteclashproman-0.1.4/PKG-INFO` & `liteclashproman-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: liteclashproman
-Version: 0.1.4
+Name: LiteClashProMan
+Version: 0.2.0
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: APScheduler>=3.10.1
 Requires-Dist: loguru>=0.7.0
+Requires-Dist: sentry-sdk[fastapi]>=1.26.0; extra == "extra"
+Provides-Extra: extra
 Description-Content-Type: text/markdown
 
 # LiteClashProMan
 
 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 
 ## 说明
```

