# Comparing `tmp/gull_api-0.0.14.tar.gz` & `tmp/gull_api-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gull_api-0.0.14.tar", max compression
+gzip compressed data, was "gull_api-0.0.15.tar", max compression
```

## Comparing `gull_api-0.0.14.tar` & `gull_api-0.0.15.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2223 2023-06-27 11:49:32.274845 gull_api-0.0.14/LICENSE
--rw-r--r--   0        0        0     3260 2023-06-27 11:49:32.274845 gull_api-0.0.14/README.md
--rw-r--r--   0        0        0      271 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/__init__.py
--rw-r--r--   0        0        0      469 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/config.py
--rw-r--r--   0        0        0     1688 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/db.py
--rw-r--r--   0        0        0     5388 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/main.py
--rw-r--r--   0        0        0     1469 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/run_gull_api.py
--rw-r--r--   0        0        0     1688 2023-06-27 11:49:32.382846 gull_api-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 gull_api-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0     2223 2023-06-27 12:19:56.710617 gull_api-0.0.15/LICENSE
+-rw-r--r--   0        0        0     3260 2023-06-27 12:19:56.710617 gull_api-0.0.15/README.md
+-rw-r--r--   0        0        0      271 2023-06-27 12:19:56.710617 gull_api-0.0.15/gull_api/__init__.py
+-rw-r--r--   0        0        0      469 2023-06-27 12:19:56.710617 gull_api-0.0.15/gull_api/config.py
+-rw-r--r--   0        0        0     1688 2023-06-27 12:19:56.710617 gull_api-0.0.15/gull_api/db.py
+-rw-r--r--   0        0        0     5394 2023-06-27 12:19:56.710617 gull_api-0.0.15/gull_api/main.py
+-rw-r--r--   0        0        0     1469 2023-06-27 12:19:56.710617 gull_api-0.0.15/gull_api/run_gull_api.py
+-rw-r--r--   0        0        0     1688 2023-06-27 12:19:56.810618 gull_api-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 gull_api-0.0.15/PKG-INFO
```

### Comparing `gull_api-0.0.14/LICENSE` & `gull_api-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.14/README.md` & `gull_api-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.14/gull_api/db.py` & `gull_api-0.0.15/gull_api/db.py`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.14/gull_api/main.py` & `gull_api-0.0.15/gull_api/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,31 +101,33 @@
         detail (str): Detailed error message.
         stderr (str, optional): Standard error stream. Defaults to "".
         returncode (int, optional): Return code of the process. Defaults to 1.
     """
     log = await create_and_log(request, stderr=stderr, returncode=returncode)
     raise HTTPException(status_code=status_code, detail=detail)
 
-# Updated post_llm function
 @app.post("/llm")
 async def post_llm(request: Dict[str, Any], cli_json=Depends(load_cli_json)):
     LLMRequest = create_llm_request_model(cli_json)
     validated_request = LLMRequest(**request)
     command = convert_request_to_cli_command(validated_request, cli_json)
     
+    return_code = None
+    
     try:
         process = await asyncio.create_subprocess_exec(*command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         stdout_bytes, stderr_bytes = await asyncio.wait_for(process.communicate(), timeout=60)
         stdout = stdout_bytes.decode("utf-8")
         stderr = stderr_bytes.decode("utf-8")
+        return_code = process.returncode
     except asyncio.TimeoutError:
-        await handle_error(request, status_code=504, detail="Server processing timed out.", returncode=process.returncode)
+        await handle_error(request, status_code=504, detail="Server processing timed out.", returncode=return_code)
     except Exception as e:
-        await handle_error(request, status_code=500, detail="Internal Server Error", stderr=str(e), returncode=process.returncode)
+        await handle_error(request, status_code=500, detail="Internal Server Error", stderr=str(e), returncode=return_code)
     else:
-        if process.returncode != 0:
-            await handle_error(request, status_code=422, detail=stderr, stderr=stderr, returncode=process.returncode)
+        if return_code != 0:
+            await handle_error(request, status_code=422, detail=stderr, stderr=stderr, returncode=return_code)
     
     # Logging successful response
-    await create_and_log(request, stdout=stdout, returncode=process.returncode)
+    await create_and_log(request, stdout=stdout, returncode=return_code)
     
     return {'response': stdout}
```

### Comparing `gull_api-0.0.14/gull_api/run_gull_api.py` & `gull_api-0.0.15/gull_api/run_gull_api.py`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.14/pyproject.toml` & `gull_api-0.0.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "gull-api"
-version = "0.0.14"
+version = "0.0.15"
 description = "A REST API for running Large Language Models"
 authors = ["Michael Becker <mdbecker@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/mdbecker/gull_api"
 repository = "https://github.com/mdbecker/gull_api"
 documentation = "https://github.com/mdbecker/gull_api/blob/main/README.md"
 readme = "README.md"
```

### Comparing `gull_api-0.0.14/PKG-INFO` & `gull_api-0.0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gull-api
-Version: 0.0.14
+Version: 0.0.15
 Summary: A REST API for running Large Language Models
 Home-page: https://github.com/mdbecker/gull_api
 License: MIT
 Keywords: api,artificial-intelligence,automation,bot,deep-learning,fastapi,GPT,language-models,large-language-models,machine-learning,microservices,natural-language-processing,NLP,openai,REST,text,text-generation,web-api
 Author: Michael Becker
 Author-email: mdbecker@gmail.com
 Requires-Python: >=3.10,<4.0
```

