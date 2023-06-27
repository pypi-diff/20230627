# Comparing `tmp/gull_api-0.0.13.tar.gz` & `tmp/gull_api-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gull_api-0.0.13.tar", max compression
+gzip compressed data, was "gull_api-0.0.14.tar", max compression
```

## Comparing `gull_api-0.0.13.tar` & `gull_api-0.0.14.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     2223 2023-06-26 02:33:05.689565 gull_api-0.0.13/LICENSE
--rw-r--r--   0        0        0     2821 2023-06-26 02:33:05.689565 gull_api-0.0.13/README.md
--rw-r--r--   0        0        0      423 2023-06-26 02:33:05.689565 gull_api-0.0.13/gull_api/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-26 02:33:05.689565 gull_api-0.0.13/gull_api/db.py
--rw-r--r--   0        0        0     5637 2023-06-26 02:33:05.689565 gull_api-0.0.13/gull_api/main.py
--rw-r--r--   0        0        0     1601 2023-06-26 02:33:05.785566 gull_api-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 gull_api-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     2223 2023-06-27 11:49:32.274845 gull_api-0.0.14/LICENSE
+-rw-r--r--   0        0        0     3260 2023-06-27 11:49:32.274845 gull_api-0.0.14/README.md
+-rw-r--r--   0        0        0      271 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/__init__.py
+-rw-r--r--   0        0        0      469 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/config.py
+-rw-r--r--   0        0        0     1688 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/db.py
+-rw-r--r--   0        0        0     5388 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/main.py
+-rw-r--r--   0        0        0     1469 2023-06-27 11:49:32.274845 gull_api-0.0.14/gull_api/run_gull_api.py
+-rw-r--r--   0        0        0     1688 2023-06-27 11:49:32.382846 gull_api-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 gull_api-0.0.14/PKG-INFO
```

### Comparing `gull_api-0.0.13/LICENSE` & `gull_api-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.13/README.md` & `gull_api-0.0.14/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,27 @@
 3. Install the dependencies:
 
    ```
    pip install poetry
    poetry install
    ```
 
-4. Run the application:
+4. Configure Environment Variables (Optional):
+
+   `GULL-API` can be configured using environment variables. To do this, create a file named `.env` in the root of the project directory, and set the environment variables there. For example:
+
+   ```
+   DB_URI=sqlite:///mydatabase.db
+   CLI_JSON_PATH=/path/to/cli.json
+   ```
+
+   `GULL-API` uses the `python-dotenv` package to load these environment variables when the application starts.
+
+
+5. Run the application:
 
    ```
    uvicorn gull_api.main:app --host 0.0.0.0 --port 8000
    ```
 
 The API will be available at `http://localhost:8000`.
```

### Comparing `gull_api-0.0.13/gull_api/db.py` & `gull_api-0.0.14/gull_api/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 import json
 import sqlalchemy
 from sqlalchemy import create_engine, Column, Integer, String, Boolean
 import sqlalchemy.orm
 from sqlalchemy.exc import SQLAlchemyError
+from gull_api import config
 
 Base = sqlalchemy.orm.declarative_base()
 
 class APIRequestLog(Base):
     __tablename__ = "api_request_log"
 
     id = Column(Integer, primary_key=True)
     request = Column(String)
     response = Column(String)
     error_occurred = Column(Boolean)
     error_details = Column(String)
 
-def load_db_config(filename="db_config.json"):
-    try:
-        with open(filename) as f:
-            return json.load(f)
-    except FileNotFoundError:
-        return {"db_uri": "sqlite:////app/data/database.db"}
-
 def get_engine():
-    db_config = load_db_config()
-    return create_engine(db_config.get("db_uri", "sqlite:///:memory:"))
+    return create_engine(config.DB_URI)
 
 def get_session_maker(engine=None):
     if engine is None:
         engine = get_engine()
     Base.metadata.create_all(bind=engine)
     return sqlalchemy.orm.sessionmaker(bind=engine)
```

### Comparing `gull_api-0.0.13/gull_api/main.py` & `gull_api-0.0.14/gull_api/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 from fastapi import FastAPI, Depends, HTTPException
 from pydantic import BaseModel, Field, create_model
 from typing import Dict, Any
 import json
 import subprocess
 import asyncio
 from gull_api.db import APIRequestLog, SessionManager
+from gull_api import config
 
 app = FastAPI()
 
 def get_single_key(dictionary: Dict[str, Any]) -> str:
     return list(dictionary.keys())[0]
 
 def load_cli_json():
-    with open("cli.json", "r") as f:
+    with open(config.CLI_JSON_PATH, "r") as f:
         return json.load(f)
 
 def create_llm_request_model(cli_json: Dict[str, Any]) -> BaseModel:
     fields = {}
     for param in cli_json[get_single_key(cli_json)]:
         param_name = param["name"]
-        if param_name == "Executable":  # skip Executable since it's not used by the api
-            continue
         field_kwargs = {"description": param["description"]}
         if "default" in param:
             field_kwargs["default"] = param["default"]
         else:
             if param.get('required', True) is False:
                 field_kwargs["default"] = None
         if "min" in param and "max" in param:
             field_kwargs["gt"] = param["min"]
             field_kwargs["lt"] = param["max"]
         fields[param["name"]] = (param["type"], Field(**field_kwargs))
     return create_model("LLMRequest", **fields)
 
 def convert_request_to_cli_command(request: BaseModel, cli_json: Dict[str, Any]) -> str:
     cli_args = []
-    command = ["./main"]  # default executable
+    command = [config.EXECUTABLE]  # use executable from config
     for param in cli_json[get_single_key(cli_json)]:
         param_name = param["name"]
-        if param_name == "Executable":  # if parameter is the executable
-            command = [param.get("default", "./main")]  # use default value or fallback to "./main"
-            continue
         if param_name in request.dict():
             value = request.dict()[param_name]
             flag = param["flag"]
             if param["type"] == "bool":
                 if value:
                     cli_args.append(flag)
             else:
```

### Comparing `gull_api-0.0.13/pyproject.toml` & `gull_api-0.0.14/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "gull-api"
-version = "0.0.13"
+version = "0.0.14"
 description = "A REST API for running Large Language Models"
 authors = ["Michael Becker <mdbecker@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/mdbecker/gull_api"
 repository = "https://github.com/mdbecker/gull_api"
 documentation = "https://github.com/mdbecker/gull_api/blob/main/README.md"
 readme = "README.md"
@@ -37,12 +37,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 SQLAlchemy = "^2.0.16"
 fastapi = "^0.97.0"
 pydantic = "^1.10.9"
 uvicorn = "^0.22.0"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
+
+[tool.poetry.scripts]
+gull-api = 'gull_api.run_gull_api:main'
```

### Comparing `gull_api-0.0.13/PKG-INFO` & `gull_api-0.0.14/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gull-api
-Version: 0.0.13
+Version: 0.0.14
 Summary: A REST API for running Large Language Models
 Home-page: https://github.com/mdbecker/gull_api
 License: MIT
 Keywords: api,artificial-intelligence,automation,bot,deep-learning,fastapi,GPT,language-models,large-language-models,machine-learning,microservices,natural-language-processing,NLP,openai,REST,text,text-generation,web-api
 Author: Michael Becker
 Author-email: mdbecker@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Requires-Dist: SQLAlchemy (>=2.0.16,<3.0.0)
 Requires-Dist: fastapi (>=0.97.0,<0.98.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Project-URL: Documentation, https://github.com/mdbecker/gull_api/blob/main/README.md
 Project-URL: Repository, https://github.com/mdbecker/gull_api
 Description-Content-Type: text/markdown
 
 # GULL-API
 
@@ -93,15 +94,27 @@
 3. Install the dependencies:
 
    ```
    pip install poetry
    poetry install
    ```
 
-4. Run the application:
+4. Configure Environment Variables (Optional):
+
+   `GULL-API` can be configured using environment variables. To do this, create a file named `.env` in the root of the project directory, and set the environment variables there. For example:
+
+   ```
+   DB_URI=sqlite:///mydatabase.db
+   CLI_JSON_PATH=/path/to/cli.json
+   ```
+
+   `GULL-API` uses the `python-dotenv` package to load these environment variables when the application starts.
+
+
+5. Run the application:
 
    ```
    uvicorn gull_api.main:app --host 0.0.0.0 --port 8000
    ```
 
 The API will be available at `http://localhost:8000`.
```

