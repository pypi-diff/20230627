# Comparing `tmp/data_ecosystem_flask-202306.0.29.tar.gz` & `tmp/data_ecosystem_flask-202306.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202306.0.29.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202306.0.32.tar", max compression
```

## Comparing `data_ecosystem_flask-202306.0.29.tar` & `data_ecosystem_flask-202306.0.32.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     9758 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/Makefile
--rw-r--r--   0        0        0    55368 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    10937 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0   145583 2023-06-25 21:21:57.445355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
--rw-r--r--   0        0        0   145583 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
--rw-r--r--   0        0        0   325863 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
--rw-r--r--   0        0        0   325863 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
--rw-r--r--   0        0        0   145835 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
--rw-r--r--   0        0        0     1692 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_posit_manifests/manifest.json
--rw-r--r--   0        0        0    12165 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
--rw-r--r--   0        0        0     2082 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0     5321 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5240 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      374 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0    17169 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0    14015 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/data_ecosystem_flask/schema/manifest.schema.json
--rw-r--r--   0        0        0    11357 2023-06-25 21:21:57.449355 data_ecosystem_flask-202306.0.29/license.md
--rw-r--r--   0        0        0     2442 2023-06-25 21:33:08.081480 data_ecosystem_flask-202306.0.29/pyproject.toml
--rw-r--r--   0        0        0    14911 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/readme.md
--rw-r--r--   0        0        0      126 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-25 21:21:57.453355 data_ecosystem_flask-202306.0.29/setup.py
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.29/PKG-INFO
+-rw-r--r--   0        0        0    10359 2023-06-27 14:04:40.284817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile
+-rw-r--r--   0        0        0      863 2023-06-27 14:04:40.284817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0    59837 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    12147 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0   145583 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
+-rw-r--r--   0        0        0   145583 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
+-rw-r--r--   0        0        0   325863 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
+-rw-r--r--   0        0        0   325863 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
+-rw-r--r--   0        0        0   145835 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
+-rw-r--r--   0        0        0     1692 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_posit_manifests/manifest.json
+-rw-r--r--   0        0        0    12165 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
+-rw-r--r--   0        0        0    28571 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0     5462 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
+-rw-r--r--   0        0        0     5240 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
+-rw-r--r--   0        0        0      374 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
+-rw-r--r--   0        0        0    17091 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0    14015 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/schema/manifest.schema.json
+-rw-r--r--   0        0        0     2401 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0    11357 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/license.md
+-rw-r--r--   0        0        0     2463 2023-06-27 14:12:59.964224 data_ecosystem_flask-202306.0.32/pyproject.toml
+-rw-r--r--   0        0        0    15006 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/readme.md
+-rw-r--r--   0        0        0      126 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/setup.py
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.32/PKG-INFO
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/Makefile` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -56,17 +56,15 @@
 	export FLASK_ENV=development && \
 	export FLASK_DEBUG=1 && \
 	flask run  --debug   
 
 flask-run-posit-prod:
 	poetry update && \
 	poetry install	 && \
-	export POSIT_ENV_NAME=prod && \
 	export FLASK_APP=app.py  && \
-	export FLASK_ENV=production && \
 	export FLASK_DEBUG=1 && \
 	flask run --debug  
 
 chrome-libva-install:
 	# Logout of ZScaler first
 	cd ~   && \
 	sudo apt update  && \
@@ -78,14 +76,17 @@
 
 chrome-libva-reboot:
 	sudo reboot 
 
 chrome-libva-test:
 	vainfo
 
+github-setup-secrets:
+	npm install -g gh
+	
 github-config:
 	git config --global user.name "John Bowyer"
 	git config --global user.email "jcbowyer@hotmail.com"
 
 node-create:
 	pip3 uninstall nodeenv
 	pip3 install --user nodeenv
@@ -171,21 +172,31 @@
 	done < .env; \
 	new_args=`echo $$args | sed 's/,$$//'`; \
 	echo "$$new_args";  \
 	rsconnect deploy api --name data-ecosystem-flask --title "Data Ecosystem Flask" --new  --force-generate  --verbose  --environment $$new_args .
 
 python-create-posit:
 	cd ~  && \
-	INSTALL_DIR="$(HOME)/.local"  && \
+	INSTALL_DIR="$$HOME/.local"  && \
+	wget https://www.sqlite.org/2023/sqlite-autoconf-3420000.tar.gz && \
+	tar -xf sqlite-autoconf-3420000.tar.gz && \
+	cd sqlite-autoconf-3420000 && \
+	gcc  -c -fPIC sqlite3.c -o sqlite3.o  && \
+	ar rcs libsqlite3.a sqlite3.o && \
+	gcc -shared -o libsqlite3.so sqlite3.o && \
+	mkdir -p $$HOME/.local/bin/sqlite-autoconf-3420000 && \
+	mv ~/sqlite-autoconf-3420000/libsqlite3.so $$HOME/.local/bin/sqlite-autoconf-3420000/libsqlite3.so && \
+	mv ~/sqlite-autoconf-3420000/sqlite3.o $$HOME/.local/bin/sqlite-autoconf-3420000/sqlite3.o && \
+	export LD_LIBRARY_PATH=$$HOME/.local/bin/sqlite-autoconf-3420000:$$LD_LIBRARY_PATH   && \
 	wget https://www.python.org/ftp/python/3.9.9/Python-3.9.9.tar.xz  && \
 	tar -xvf Python-3.9.9.tar.xz  && \
 	cd Python-3.9.9 && \
 	./configure --prefix=$$INSTALL_DIR && \
 	make  && \
-	make install  && \
+	make altinstall  && \
 	echo "export PATH=\"$$INSTALL_DIR/bin:\$$PATH\"" >> ~/.bashrc  && \
 	source ~/.bashrc  && \
 	python3.9 --version
 
 python-create-wsl:
 	sudo apt update
 	sudo apt install python3.9
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,32 @@
     This Flask app provides endpoints to interact with
     JIRA and Alation services through a Swagger UI.
 
 Returns:
     None
 """
 
-from flask import Flask, send_file, request
+from flask import Flask, send_file, request, render_template, Blueprint, g
 from opentelemetry import trace
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
 from pathlib import Path
 from datetime import datetime
 from io import BytesIO
 from pandas import ExcelWriter
 from requests.exceptions import HTTPError
 from openpyxl.utils.exceptions import InvalidFileException
-from flask_restx import Api, Resource, fields, Namespace
+from flask_restx import Api, Resource, fields, Namespace, reqparse
 from json import JSONDecodeError
 from bs4 import BeautifulSoup
 from app_startup import create_api, create_app
 import rsconnect
+from datetime import datetime
+from werkzeug.datastructures import FileStorage
+import re
 
 # Ensure .bashrc where zfi4 is your username
 # export PYTHONPATH=/home/zfi4/data-ecosystem-services/pade_python:$PYTHONPATH
 from data_ecosystem_services.alation_service import (
     schema as pade_schema,
     datasource as pade_datasource,
     tokenendpoint as pade_tokenendpoint,
@@ -69,31 +72,42 @@
 
 
 TIMEOUT_5_SEC = 5
 TIMEOUT_ONE_MIN = 60
 
 CURRENT_USER_NAME = "zfi4"
 API_PATH = "/data-ecosystem-services/pade_python"
- 
+
 sys.path.append(os.getcwd())
 app_dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(app_dir)
 
 # app.config["PYTHONPATH"] = "../../../pade_python/"
 
+
 app = create_app()
-api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_security = create_api(app)
 
 
+@app.before_request
+def before_request():
+    g.base_url = request.url_root
+    g.log_url = g.base_url + "/logs/get_log_file_tail/1000"
+
+
+upload_parser = reqparse.RequestParser()
+upload_parser.add_argument('file', location='files',
+                           type=FileStorage, required=True)
+
+# Define the blueprint
+cdc_admin_bp = Blueprint('logs', __name__,
+                         url_prefix='/logs')
+
+
+app.register_blueprint(cdc_admin_bp)
 
-def expect_upload_parser(f):
-    @api.expect(upload_parser)
-    def decorated(*args, **kwargs):
-        return f(*args, **kwargs)
-    return decorated
 
 def get_posit_api_key():
 
     with tracer.start_as_current_span(f"/get_posit_api_key"):
 
         config = app.cdc_config
 
@@ -120,27 +134,14 @@
 
         az_kv_posit_connect_secret = az_key_vault.get_secret(
             az_kv_posit_connect_secret_key)
 
         return az_kv_posit_connect_secret
 
 
-class WelcomeSwagger(Resource):
-    def get(self):
-        """
-        Returns the Swagger API documentation.
-
-        Returns:
-            dict: The Swagger API documentation schema.
-        """
-        with tracer.start_as_current_span("/api/swagger"):
-
-            return api.__schema__
-
-
 def get_api_access_token(config):
     """Retrieves the API access token from a configuration dictionary.
 
     The function fetches various configuration values from the input dictionary,
     including Azure subscription details and Key Vault secrets, to create an Azure
     Key Vault client and fetch the Alation refresh token. The API access token is then
     generated using the TokenEndpoint and the relevant Alation details.
@@ -149,46 +150,150 @@
         config (dict): A dictionary containing necessary configuration values,
         such as Azure subscription details, Key Vault name, Key Vault secret keys,
         and Alation base URL.
 
     Returns:
         str: The API access token.
     """
-    az_sub_tenant_id = config.get("az_sub_tenant_id")
-    az_sub_client_id = config.get("az_sub_client_id")
-    az_kv_key_vault_name = config.get("az_kv_key_vault_name")
-    az_kv_az_sub_client_secret_key = config.get(
-        "az_kv_az_sub_client_secret_key")
-    az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
-        "-", "_")
-    client_secret = os.getenv(az_kv_az_sub_client_secret_key)
-    print(f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
-    print(f"az_sub_client_id:{az_sub_client_id}")
-    # Initialize running_interactive as False
-    running_interactive = False
-
-    # Trim leading and trailing whitespace from client_secret
-    client_secret = client_secret.strip()
-
-    # Check if the client_secret is None or a zero-length string
-    if not client_secret:
-        running_interactive = True
-
-    # This will print True if client_secret is None or a zero-length string
-    print(running_interactive)
-
-    az_key_vault = pade_az_key_vault.AzKeyVault(
-        az_sub_tenant_id, az_sub_client_id, client_secret, az_kv_key_vault_name, running_interactive)
-    az_kv_edc_refresh_secret_key = config.get("az_kv_edc_refresh_secret_key")
-    alation_refresh_token = az_key_vault.get_secret(
-        az_kv_edc_refresh_secret_key)
-    edc_alation_base_url = config.get("edc_alation_base_url")
-    api_access_token = get_api_access_token(config)
-    logger.info(f"api_access_token:{api_access_token}")
-    return api_access_token
+
+    with tracer.start_as_current_span(f"get_api_access_token"):
+
+        az_sub_tenant_id = config.get("az_sub_tenant_id")
+        az_sub_client_id = config.get("az_sub_client_id")
+        az_kv_key_vault_name = config.get("az_kv_key_vault_name")
+        az_kv_az_sub_client_secret_key = config.get(
+            "az_kv_az_sub_client_secret_key")
+        az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
+            "-", "_")
+        client_secret = os.getenv(az_kv_az_sub_client_secret_key)
+        print(
+            f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
+        print(f"az_sub_client_id:{az_sub_client_id}")
+        # Initialize running_interactive as False
+        running_interactive = False
+
+        # Trim leading and trailing whitespace from client_secret
+        client_secret = client_secret.strip()
+
+        # Check if the client_secret is None or a zero-length string
+        if not client_secret:
+            running_interactive = True
+
+        az_key_vault = pade_az_key_vault.AzKeyVault(
+            az_sub_tenant_id, az_sub_client_id, client_secret, az_kv_key_vault_name, running_interactive)
+        az_kv_edc_refresh_secret_key = config.get(
+            "az_kv_edc_refresh_secret_key")
+        alation_refresh_token = az_key_vault.get_secret(
+            az_kv_edc_refresh_secret_key)
+        edc_alation_base_url = config.get("edc_alation_base_url")
+        token_endpoint = pade_tokenendpoint.TokenEndpoint(edc_alation_base_url)
+        alation_user_id = config.get("edc_alation_user_id")
+        api_access_token = token_endpoint.get_api_access_token(
+            edc_alation_base_url, alation_user_id, alation_refresh_token)
+        logger.info(f"api_access_token:{api_access_token}")
+        return api_access_token
+
+
+@cdc_admin_bp.route('/get_log_file_tail/<int:number_of_lines>')
+def get_log_file_tail(number_of_lines):
+
+    with tracer.start_as_current_span(f"get_log_file_tail"):
+
+        try:
+            log_data = logger_singleton.get_log_file_tail(number_of_lines)
+        except AttributeError:
+            return "Error: Logger not correctly configured", 500
+
+        log_entries = [line.replace('\\', ':').split(None, 3)
+                       for line in log_data.strip().split('\n')]
+
+        for entry in log_entries:
+
+            try:
+                time_string = entry[1].split(":data_ecosystem_services:", 1)[0]
+                if time_string.count(':') >= 2:
+                    datetime_object = datetime.strptime(
+                        f"{entry[0]} {time_string}", "%Y-%m-%d %H:%M:%S")
+                    entry[0] = datetime_object.strftime("%Y-%m-%d %I:%M:%S %p")
+                else:
+                    raise ValueError("Invalid date and time format")
+            except ValueError:
+                return f"Error: Unable to parse date and time from {entry[0]} {time_string}", 500
+            except IndexError:
+                return f"Error: Unable to split string {entry[1]}", 500
+
+            try:
+                module, line_number = entry[1].split(
+                    ":data_ecosystem_services:", 1)[1].split(':', 1)
+                entry[1] = module
+                entry.insert(2, line_number)
+            except ValueError:
+                return f"Error: Unable to split string {entry[1]}", 500
+
+        return render_template('log_file.html', entries=log_entries)
+
+
+@app.route('/')
+def home():
+    API_DESCRIPTION = (
+        "The Program Agnostic Data Ecosystem (PADE) provides shared resources, "
+        "practices and guardrails for analysts to discover, access, link, and use "
+        "agency data in a consistent way. PADE improvements in standardized and "
+        "streamlined workflows reduce the effort required to find, access, and "
+        f"trust data. Logs can be found at [this link]({request.url_root}/logs/get_log_file_tail/1000)."
+    )
+
+    api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_cdc_security = create_api(
+        app, API_DESCRIPTION)
+
+    ns_welcome.add_resource(WelcomeSwagger, '/')
+    ns_welcome.add_resource(WelcomeSwagger, "/api/swagger")
+    ns_jira.add_resource(Task, '/tasks/<string:project>')
+    ns_alation.add_resource(MetadataExcelFileUploadRequest,
+                            "/metadata_excel_file_upload_request/<int:schema_id>")
+    ns_alation.add_resource(MetadataJsonFileUploadRequest,
+                            "/metadata_json_file_upload_request/<int:schema_id>")
+    ns_alation.add_resource(MetadataJsonFileDownload,
+                            "/metadata_json_file_download/<int:schema_id>")
+    ns_alation.add_resource(MetadataExcelFileDownload,
+                            "/metadata_excel_file_download/<int:schema_id>")
+    ns_alation.add_resource(MetadataExcelFileUpload,
+                            "/metadata_excel_file_upload")
+
+    ns_alation.add_resource(MetadataJsonFileUpload,
+                            "/metadata_json_file_upload")
+
+    ns_posit.add_resource(ConnectApiKeyVerification,
+                          "/connect_api_key_verification")
+    ns_posit.add_resource(PythonInformation, "/python_information")
+    ns_posit.add_resource(GeneratedManifest, "/generate_manifest")
+    ns_posit.add_resource(PublishManifest, "/publish_manifest")
+    ns_posit.add_resource(ContentList, "/list_content")
+    ns_posit.add_resource(
+        DeploymentBundle, "/build_deployment_bundle/<string:content_id>/<string:bundle_id>")
+    ns_posit.add_resource(DeploymentBundleList,
+                          "/list_deployment_bundles/<string:content_id>")
+    ns_posit.add_resource(TaskStatus, "/get_task_status/<string:task_id>")
+
+    ns_cdc_security.add_resource(
+        AzSubscriptionClientSecretVerification, "/verify_az_sub_client_secret")
+
+    return {"message": "Welcome to our API"}
+
+
+class WelcomeSwagger(Resource):
+    def get(self):
+        """
+        Returns the Swagger API documentation.
+
+        Returns:
+            dict: The Swagger API documentation schema.
+        """
+        with tracer.start_as_current_span("/api/swagger"):
+            return api.__schema__
 
 
 class Task(Resource):
     """
     Represents the endpoint for retrieving tasks related to a specific project.
 
     This class is used as a Flask-RESTful resource to handle requests related
@@ -338,17 +443,19 @@
             This method uploads the Excel metadata file from SharePoint to
             Alation.
 
         Example:
             Use schema_id 106788 to test OCIO_PADE_DEV (DataBricks).
         """
 
-        return {
-            "message": f"Tasks: GET method called for project: {schema_id}"
-        }
+        with tracer.start_as_current_span(f"/metadata_excel_file_upload_request/schema_id"):
+
+            return {
+                "message": f"Tasks: GET method called for project: {schema_id}"
+            }
 
 
 class MetadataJsonFileUploadRequest(Resource):
     """
     Represents the endpoint for uploading a metadata JSON file.
 
     This class is used as a Flask resource to handle requests related to
@@ -374,14 +481,19 @@
         Returns:
             dict: A dictionary containing the response data.
 
         Example:
             Use schema_id 106788 to test OCIO_PADE_DEV (DataBricks).
         """
 
+        logger_singleton = pade_env_logging.LoggerSingleton.instance()
+        logger = logger_singleton.get_logger()
+        tracer_singleton = pade_env_tracing.TracerSingleton.instance()
+        tracer = tracer_singleton.get_tracer()
+
         with tracer.start_as_current_span(f"/metadata_json_file_upload_request/{schema_id}"):
 
             try:
                 config = app.cdc_config
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 logger.info(f"edc_alation_base_url:{edc_alation_base_url}")
                 api_access_token = get_api_access_token(config)
@@ -401,24 +513,28 @@
                 if response_datasource.status_code in (200, 201):
                     # Extract the API token from the response
                     datasource = json.loads(response_datasource.text)
                     datasource_title = datasource.get("title")
                     logger.info(f"datasource: {str(datasource_title)}")
                 else:
                     response_datasource_text = response_datasource.reason
+                    logger.error(
+                        f"Failed to get Datasource : {response_datasource_text}")
+                    logger_singleton.force_flush()
                     return "Failed to get Datasource :" + str(response_datasource_text)
 
                 msg = "Metadata_Json_File: Upload Processed for "
                 msg = msg + f"schema_id: {schema_id}"
+                logger.info(msg)
+                logger_singleton.force_flush()
+
                 return {
                     "message": msg
                 }
 
-                logger_singleton.force_flush()
-
             except Exception as e:
                 logger.error(f"An unexpected error occurred: {str(e)}")
                 logger_singleton.force_flush()
                 return {"error": f"An unexpected error occurred: {str(e)}"}
 
 
 class MetadataJsonFileDownload(Resource):
@@ -452,14 +568,19 @@
 
         with tracer.start_as_current_span(f"/metadata_json_file_download/{schema_id}"):
             try:
                 config = app.cdc_config
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 api_access_token = get_api_access_token(config)
 
+                if len(api_access_token.strip()) == 0:
+                    msg = "Alation API Access Token is not set"
+                    logger.error(msg)
+                    return {"error": f"An unexpected error occurred: {msg}"}
+
                 logger.info("###### GET SCHEMA #######")
                 headers = {
                     "Token": api_access_token,
                     "Content-Type": "application/json",
                 }
                 api_url = f"/integration/v1/schema/{schema_id}/"
                 schema_url = edc_alation_base_url + api_url
@@ -475,15 +596,25 @@
                 # Check the response status code to determine if successful
                 if "title" in schema_results:
                     # Extract the API token from the response
                     schema_name = schema_results.get("name")
                     datasource_id = schema_results.get("ds_id")
                 else:
                     response_schema_text = schema_results.get("reason")
-                    return "Failed to get schema :" + str(response_schema_text)
+                    error_msg = "Failed to get schema:" + \
+                        str(response_schema_text)
+                    error_msg = error_msg + " for schema_id: " + str(schema_id)
+                    error_msg = error_msg + \
+                        " and schema_name: " + str(schema_name)
+                    error_msg = error_msg + \
+                        " and datasource_id: " + str(datasource_id)
+                    error_msg = error_msg + \
+                        " and schema_results: " + str(schema_results)
+                    logger.error(error_msg)
+                    return {"error": error_msg}
 
                 logger.info("###### GET DATASOURCE #######")
                 api_url = f"/integration/v1/datasource/{datasource_id}/"
                 datasource_url = edc_alation_base_url + api_url
                 logger.info(f"datasource_url: {datasource_url}")
                 logger.info(f"headers: {headers}")
                 response_datasource = requests.get(datasource_url,
@@ -502,14 +633,18 @@
 
                 schema_location = config.get("edc_schema_location")
                 logger.info(
                     "Loading manifest schema from {0}".format(schema_location))
                 manifest = pade_manifest.Manifest(schema_location)
                 obj_file = pade_env_file.EnvironmentFile()
                 app_dir = os.path.dirname(os.path.abspath(__file__))
+                environment = config.get("environment")
+                yyyy = config.get("yyyy")
+                mm = config.get("mm")
+                dd = config.get("dd")
                 manifest_path = (
                     app_dir + "/" + environment + "_manifests/"
                 )
                 manifest_file = (
                     obj_file.scrub_file_name(datasource_title)
                     + "_"
                     + obj_file.scrub_file_name(schema_name)
@@ -748,16 +883,14 @@
 
     Returns:
         Response: The response of the HTTP request after processing the
         uploaded file. The specific content and status code of the response
         will depend on the implementation.
     """
 
-    method_decorators = [expect_upload_parser]  # Apply decorator here
-
     def post(self):
         """
         Uploads the Excel metadata file to Alation via direct upload based on
         the schema_id.
 
         Args:
             schema_id (int): The ID of the schema associated with the metadata
@@ -766,19 +899,19 @@
         Returns:
             dict: A dictionary containing the response data.
 
         Example:
             Use schema_id 106788 to test OCIO_PADE_DEV (DataBricks).
         """
 
-        method_decorators = [expect_upload_parser]  # Apply decorator here
+        args = upload_parser.parse_args()
 
-        file = request.files["file"]
+        file = args["file"]
         logger.info(f"file: {file}")
-        msg = "Metadata_Excel_File_Upload: POST method called successfully."
+        msg = "Metadata_Json_File_Upload: POST method called successfully."
         return {
             "message": msg
         }
 
 
 class MetadataJsonFileUpload(Resource):
     """
@@ -796,23 +929,24 @@
     Returns:
         Response: The response of the HTTP request after processing the
         uploaded file.
         The specific content and status code of the response will depend on
         the implementation.
     """
 
-    method_decorators = [expect_upload_parser]  # Apply decorator here
-
     def post(self):
         """Uploads JSON metadata file via direct upload to Alation
         based on schema_id.
         Use 106788 to test OCIO_PADE_DEV (DataBricks)"""
+        args = upload_parser.parse_args()
 
         with tracer.start_as_current_span(f"/metadata_json_file_upload"):
-            file = request.files["file"]
+
+            # Get the uploaded file
+            file = args["file"]
 
             # Read the contents of the file as JSON
             file_contents = file.read()
             json_data = json.loads(file_contents)
 
             # Extract the alationSchemaID
             schema_id = json_data["alationSchemaID"]
@@ -863,18 +997,23 @@
                 else:
                     response_datasource_text = response_datasource.reason
                     return "Failed to get Datasource :" + str(
                         response_datasource_text
                     )
 
                 schema_location = config.get("edc_schema_location")
-                logger.info(f"Loading manifest schema from {schema_location}")
+                logger.info(
+                    f"Loading manifest schema from {schema_location}")
                 manifest = pade_manifest.Manifest(schema_location)
                 obj_file = pade_env_file.EnvironmentFile()
                 app_dir = os.path.dirname(os.path.abspath(__file__))
+                environment = config.get("environment")
+                yyyy = config.get("yyyy")
+                mm = config.get("mm")
+                dd = config.get("dd")
                 manifest_path = (
                     app_dir + "/" + environment + "_manifests/"
                 )
                 manifest_file = (
                     obj_file.scrub_file_name(datasource_title)
                     + "_"
                     + obj_file.scrub_file_name(schema_name)
@@ -886,14 +1025,35 @@
                     + dd
                     + ".json"
                 )
                 manifest_file = manifest_path + manifest_file
                 logger.info(f"manifest_file: {manifest_file}")
                 logger.info(f"datasource_id: {datasource_id}")
 
+                az_sub_tenant_id = config.get("az_sub_tenant_id")
+                az_sub_client_id = config.get("az_sub_client_id")
+                az_kv_key_vault_name = config.get("az_kv_key_vault_name")
+
+                # Initialize running_interactive as False
+                running_interactive = False
+
+                # Trim leading and trailing whitespace from client_secret
+                client_secret = client_secret.strip()
+
+                # Check if the client_secret is None or a zero-length string
+                if not client_secret:
+                    running_interactive = True
+
+                az_key_vault = pade_az_key_vault.AzKeyVault(
+                    az_sub_tenant_id, az_sub_client_id, client_secret, az_kv_key_vault_name, running_interactive)
+                az_kv_edc_refresh_secret_key = config.get(
+                    "az_kv_edc_refresh_secret_key")
+                alation_refresh_token = az_key_vault.get_secret(
+                    az_kv_edc_refresh_secret_key)
+
                 # Save the JSON data to a file
                 with open(manifest_file, "w") as file:
                     json.dump(json_data, file)
                 schema.upload_schema_manifest(
                     schema_id,
                     headers,
                     edc_alation_base_url,
@@ -930,25 +1090,22 @@
             az_kv_az_sub_client_secret_key = config.get(
                 "az_kv_az_sub_client_secret_key")
             az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
                 "-", "_")
             client_secret = os.getenv(az_kv_az_sub_client_secret_key)
             tenant_id = config.get("tenant_id")
             client_id = config.get("client_id")
-                 
+
             security_core = pade_security_core.SecurityCore()
-            status_code, response_content, = pade_security_core.verify_az_sub_client_secret(
+            status_code, response_content = security_core.verify_az_sub_client_secret(
                 tenant_id, client_id, client_secret)
 
             # Handle the verification logic
             return {
                 'status_code': status_code,
-                'posit_connect_base_url': posit_connect_base_url,
-                'api_url': api_url,
-                "connect_api_key": connect_api_key,
                 'response_content': response_content
             }, 200
 
 
 class ConnectApiKeyVerification(Resource):
     """
     A Flask-RESTful resource for handling the verification of API keys.
@@ -1018,14 +1175,15 @@
             # Handle the verification logic
             return {
                 'posit_connect_base_url': posit_connect_base_url,
                 'api_url': api_url,
                 'response_content': response_content
             }, 200
 
+
 class PythonInformation(Resource):
     """
     A Flask-RESTful resource for handling POSIT Python Information.
 
     """
 
     def get(self):
@@ -1055,32 +1213,14 @@
             return {
                 'posit_connect_base_url': posit_connect_base_url,
                 'api_url': api_url,
                 "az_kv_posit_connect_secret_key": az_kv_posit_connect_secret_key,
                 'response_content': response_content
             }, 200
 
-class MessageHTML(Resource):
-    """
-    A Flask-RESTful resource for displaying HTML
-
-    """
-
-    def get(self):
-        """
-        Display HTML content provided as a 'html' query parameter in the request URL.
-
-        Returns:
-            str: Rendered HTML content as a HTTP response. 
-            If no 'html' parameter is provided, an empty string is returned.
-        """
-        html_content = request.args.get('html', '')  # Default to empty string if no 'html' parameter
-        return render_template_string(html_content)
-
- 
 
 class GeneratedManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Generation
 
     """
 
@@ -1112,48 +1252,48 @@
             obj_file = pade_env_file.EnvironmentFile()
 
             app_dir = os.path.dirname(os.path.abspath(__file__))
 
             manifest_path = (
                 app_dir + "/" + environment + "_posit_manifests/"
             )
-            
+
             swagger_path = (
                 app_dir + "/" + environment + "_swagger_manifests/"
             )
 
             yyyy = str(datetime.now().year)
             dd = str(datetime.now().day).zfill(2)
             mm = str(datetime.now().month).zfill(2)
-          
+
             json_extension = (
                 "_"
                 + yyyy
                 + "_"
                 + mm
                 + "_"
                 + dd
                 + ".json"
             )
             manifest_file = manifest_path + "manifest" + json_extension
             # swagger_file = swagger_path + "swagger" + json_extension
-            # use cached json file for now 
+            # use cached json file for now
             # having issues downloading
             swagger_file = swagger_path + "swagger_2023_06_22.json"
             connect_api_key = get_posit_api_key()
             requirements_file = app_dir + "/requirements.txt"
 
             # headers = {
             #     "Authorization": f"Bearer {connect_api_key}",
             # }
             swagger_url = f"{base_url}/swagger.json"
             # response = requests.get(swagger_url, headers=headers)
 
             # response_data = None
-            # error_message = None 
+            # error_message = None
             # if response.status_code == 200:  # HTTP status code 200 means "OK"
             #     try:
             #         response_data =  response.json()
             #         response.raise_for_status()  # This will raise an HTTPError if the HTTP request returned an unsuccessful status code
             #   except requests.HTTPError as http_err:
             #        error_message = f"HTTP error occurred: {http_err}"
             #        soup = BeautifulSoup(response.text, 'html.parser')
@@ -1185,22 +1325,23 @@
             posit_connect = pade_posit_connect.PositConnect()
 
             manifest_json = posit_connect.generate_manifest(
                 swagger_file, requirements_file)
 
             with open(manifest_file, 'w') as f:
                 f.write(manifest_json)
-                    
+
             # Handle the verification logic
             return {
-                'swagger_url' :  swagger_url,
+                'swagger_url': swagger_url,
                 'manifest_json': manifest_json,
                 'status_message': 'success'
             }, 200
 
+
 class PublishManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Publication
 
     """
 
     def get(self):
@@ -1227,35 +1368,34 @@
             # Join the parts back together
             url_without_filename = '/'.join(url_parts)
             base_url = url_without_filename
             environment = config.get("environment")
             obj_file = pade_env_file.EnvironmentFile()
 
             app_dir = os.path.dirname(os.path.abspath(__file__))
-            
+
             manifest_path = (
                 app_dir + "/" + environment + "_posit_manifests/"
             )
 
-            
             manifest_file = obj_file.get_latest_file(manifest_path)
 
             logger.info(f"manfiest_file:{manifest_file}")
             az_kv_posit_connect_secret_key = config.get(
                 "az_kv_posit_connect_secret_key")
             connect_api_key = get_posit_api_key()
 
             posit_connect = pade_posit_connect.PositConnect()
 
             status_code, response_content, api_url = posit_connect.publish_manifest(
                 connect_api_key, posit_connect_base_url, manifest_file)
-                    
+
             # Handle the verification logic
             return {
-                'status_code' :  status_code,
+                'status_code': status_code,
                 'response_content': response_content,
                 'api_url': api_url
             }, 200
 
 
 class ContentList(Resource):
     """
@@ -1281,22 +1421,23 @@
                 "az_kv_posit_connect_secret_key")
             connect_api_key = get_posit_api_key()
 
             posit_connect = pade_posit_connect.PositConnect()
 
             status_code, response_content, api_url = posit_connect.list_content(
                 connect_api_key, posit_connect_base_url)
-                    
+
             # Handle the verification logic
             return {
-                'status_code' :  status_code,
+                'status_code': status_code,
                 'response_content': response_content,
                 'api_url': api_url
             }, 200
 
+
 class DeploymentBundleList(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
     def get(self, content_id):
@@ -1317,22 +1458,23 @@
                 "az_kv_posit_connect_secret_key")
             connect_api_key = get_posit_api_key()
 
             posit_connect = pade_posit_connect.PositConnect()
 
             status_code, response_content, api_url = posit_connect.list_deployment_bundles(
                 connect_api_key, posit_connect_base_url, content_id)
-                    
+
             # Handle the verification logic
             return {
-                'status_code' :  status_code,
+                'status_code': status_code,
                 'response_content': response_content,
                 'api_url': api_url
             }, 200
 
+
 class TaskStatus(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
     def get(self, task_id):
@@ -1353,18 +1495,18 @@
                 "az_kv_posit_connect_secret_key")
             connect_api_key = get_posit_api_key()
 
             posit_connect = pade_posit_connect.PositConnect()
 
             status_code, response_content, api_url = posit_connect.get_task_details(
                 connect_api_key, posit_connect_base_url, task_id)
-                    
+
             # Handle the verification logic
             return {
-                'status_code' :  status_code,
+                'status_code': status_code,
                 'response_content': response_content,
                 'api_url': api_url
             }, 200
 
 
 metric_exporter = AzureMonitorMetricExporter()
 
@@ -1376,42 +1518,9 @@
 # When running in Posit Workbench, apply ProxyFix middleware
 # See: https://flask.palletsprojects.com/en/2.2.x/deploying/proxy_fix/
 if "RS_SERVER_URL" in os.environ and os.environ["RS_SERVER_URL"]:
     from werkzeug.middleware.proxy_fix import ProxyFix
     app.wsgi_app = ProxyFix(app.wsgi_app, x_prefix=1)
 
 
-upload_parser = api.parser()
-upload_parser.add_argument(
-    "file", location="files", type="FileStorage", required=True
-)
-
-ns_welcome.add_resource(WelcomeSwagger, '/')
-ns_welcome.add_resource(WelcomeSwagger, "/api/swagger")
-ns_jira.add_resource(Task, '/tasks/<string:project>')
-ns_alation.add_resource(MetadataExcelFileUploadRequest,
-                        "/metadata_excel_file_upload_request/<int:schema_id>")
-ns_alation.add_resource(MetadataJsonFileUploadRequest,
-                        "/metadata_json_file_upload_request/<int:schema_id>")
-ns_alation.add_resource(MetadataJsonFileDownload,
-                        "/metadata_json_file_download/<int:schema_id>")
-ns_alation.add_resource(MetadataExcelFileDownload,
-                        "/metadata_excel_file_download/<int:schema_id>")
-ns_alation.add_resource(MetadataExcelFileUpload, "/metadata_excel_file_upload")
-MetadataExcelFileUpload.method_decorators.append(api.expect(upload_parser))
-ns_alation.add_resource(MetadataJsonFileUpload, "/metadata_json_file_upload")
-MetadataJsonFileUpload.method_decorators.append(api.expect(upload_parser))
-
-ns_posit.add_resource(ConnectApiKeyVerification, "/connect_api_key_verification")
-ns_posit.add_resource(PythonInformation, "/python_information")
-ns_posit.add_resource(GeneratedManifest, "/generate_manifest")
-ns_posit.add_resource(PublishManifest, "/publish_manifest")
-ns_posit.add_resource(ContentList, "/list_content")
-ns_posit.add_resource(DeploymentBundle, "/build_deployment_bundle/<string:content_id>/<string:bundle_id>")
-ns_posit.add_resource(DeploymentBundleList, "/list_deployment_bundles/<string:content_id>")
-ns_posit.add_resource(TaskStatus, "/get_task_status/<string:task_id>")
-
-ns_cdc_admin.add_resource(MessageHTML, "/display_html/<string:html>")
-ns_cdc_security.add_resource(AzSubscriptionClientSecretVerification, "/verify_az_sub_client_secret" )
-
 if __name__ == "__main__":
     app.run(debug=True)
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app_startup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from flask import Flask
 from flask_restx import Api, Resource, fields, Namespace
 from datetime import datetime
 from pathlib import Path
 import shutil
 from dotenv import load_dotenv, set_key, dotenv_values
 import os
+from flask import request
 
 # Importing necessary modules from data_ecosystem_services package
 # These modules seem to be related to environment metadata, tracing and logging.
 from data_ecosystem_services.cdc_self_service import (
     environment_metadata as pade_env_metadata
 )
 from data_ecosystem_services.cdc_admin_service import (
@@ -24,14 +25,31 @@
 import sys
 import importlib
 
 # Constant indicating if the application is running inside Windows Subsystem for Linux (WSL)
 RUNNING_IN_WSL = False
 
 
+def change_to_flask_directory():
+    current_directory = os.getcwd()  # get current directory
+    base_directory = os.path.basename(
+        current_directory)  # get the base directory
+
+    if base_directory != 'data_ecosystem_flask':
+        # path to the directory you want to change to
+        new_directory = os.path.join(
+            current_directory, 'pade-flask/data_ecosystem_flask')
+
+        # change to new directory
+        os.chdir(new_directory)
+        print(f"Directory changed to {os.getcwd()}")
+    else:
+        print("Current directory is already 'data_ecosystem_flask'")
+
+
 def get_environment_name():
     """
     Retrieves the value of the 'POSIT_ENV_NAME' environment variable.
 
     Raises:
         ValueError: If the 'POSIT_ENV_NAME' environment variable is not set.
 
@@ -39,24 +57,24 @@
         str: The value of the 'POSIT_ENV_NAME' environment variable.
     """
 
     environment_name = os.environ.get("POSIT_ENV_NAME")
     if environment_name is None:
         environment_name = os.environ.get("FLASK_ENV")
         if environment_name is None:
-            raise ValueError("The POSIT_ENV_NAME environment variable is not set.")
+            raise ValueError(
+                "The POSIT_ENV_NAME environment variable is not set.")
     if environment_name == "development":
         environment_name = "dev"
     if environment_name == "production":
         environment_name = "prod"
     return environment_name
- 
 
 
-def create_api(app):
+def create_api(app, api_description):
     """ 
     Creates and initializes an API and its namespaces for a given app.
 
         Args:
             app (Flask): The Flask application instance for which the API will be created.
 
         Returns:
@@ -68,27 +86,19 @@
 
             ns_jira (flask_restplus.Namespace): A namespace for handling Jira-related routes.
 
             ns_posit (flask_restplus.Namespace): A namespace for handling Posit-related routes.
 
     """
 
-    API_DESCRIPTION = (
-        "The Program Agnostic Data Ecosystem (PADE) provides shared resources, "
-        "practices and guardrails for analysts to discover, access, link, and use "
-        "agency data in a consistent way. PADE improvements in standardized and "
-        "streamlined workflows reduce the effort required to find, access, and "
-        "trust data."
-    )
-
     api = Api(
         app,
         version="1.0",
         title="Data Ecosystem Flask API",
-        description=API_DESCRIPTION,
+        description=api_description,
         doc="/",
         url="/",
     )
 
     ns_welcome = api.namespace(
         "welcome", description="Welcome to the CDC Data Ecosystem API")
 
@@ -101,24 +111,24 @@
     )
 
     ns_tech_environment = api.namespace(
         "tech_environment",
         description=TECH_ENVIRONMENT_DESCRIPTION,
     )
 
-    SECURITY_DESCRIPTION = (
+    CDC_SECURITY_DESCRIPTION = (
         "The security service manages security of the data products and associated "
         "services. The package contains datasets that provide critical information "
         "for ensuring the confidentiality, integrity, and availability of the data "
         "products and associated services."
     )
 
-    ns_security = api.namespace(
-        "security",
-        description=SECURITY_DESCRIPTION,
+    ns_cdc_security = api.namespace(
+        "cdc_security",
+        description=CDC_SECURITY_DESCRIPTION,
     )
 
     BUSINESS_DESCRIPTION = (
         "The business service manages the business context and meaning of the data "
         "products and associated services. This package contains datasets that "
         "provide critical information for understanding the business context, "
         "meaning, and usage of the data products and associated services."
@@ -162,27 +172,24 @@
     )
 
     ns_posit = api.namespace(
         "posit",
         description=POSIT_DESCRIPTION,
     )
 
-
- 
-    
     api.add_namespace(ns_welcome)
     api.add_namespace(ns_tech_environment)
-    api.add_namespace(ns_security)
+    api.add_namespace(ns_cdc_security)
     api.add_namespace(ns_business)
     api.add_namespace(ns_cdc_admin)
     api.add_namespace(ns_jira)
     api.add_namespace(ns_alation)
     api.add_namespace(ns_posit)
 
-    return api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_security
+    return api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_cdc_security
 
 
 def create_app():
     """
     This function is used to create and configure a Flask application instance. 
 
     Returns:
@@ -198,131 +205,141 @@
     # Add your Flask app creation and configuration logic here
 
     # Get the path to the .env file
     dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
 
     # Load the .env file
     load_dotenv(dotenv_path)
-
-    set_key(dotenv_path, "APPLICATIONINSIGHTS_CONNECTION_STRING", "InstrumentationKey=d091b27b-14e0-437f-ae3c-90f3f04ef3dc;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/")
-    set_key(dotenv_path, "APPINSIGHTS_INSTRUMENTATIONKEY", "d091b27b-14e0-437f-ae3c-90f3f04ef3dc")
-
+    instrumentation_key = "d091b27b-14e0-437f-ae3c-90f3f04ef3dc"
+    set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE",
+            "1")
+    set_key(dotenv_path, "APPLICATIONINSIGHTS_CONNECTION_STRING",
+            f"InstrumentationKey={instrumentation_key};IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/")
+    set_key(dotenv_path, "APPINSIGHTS_INSTRUMENTATIONKEY",
+            instrumentation_key)
     # Reload the updated .env file
     load_dotenv(dotenv_path)
 
-    current_directory = os.getcwd()
-
     logger_singleton = pade_env_logging.LoggerSingleton.instance()
     logger = logger_singleton.get_logger()
-
-    obj_env_metadata = pade_env_metadata.EnvironmentMetaData()
-    environment = get_environment_name()
-    yyyy = str(datetime.now().year)
-    dd = str(datetime.now().day).zfill(2)
-    mm = str(datetime.now().month).zfill(2)
-    path = Path(os.getcwd())
-    running_local = True
-    repository_path_default = str(path.parent)
-    logger.info(
-        f"repository_path_default:{repository_path_default}")
-    parameters = {
-        "project_id": "ocio_pade_dev",
-        "project_id_root": "ocio",
-        "project_id_individual": "PADE",
-        "environment": environment,
-        "yyyy": yyyy,
-        "dd": dd,
-        "mm": mm,
-        "azure_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
-        "repository_path": repository_path_default,
-        "running_local": running_local,
-    }
-    config = obj_env_metadata.get_configuration_common(
-        parameters, None)
-
-    logger.info(f"config:{config}")
-
-    app = Flask(__name__)
-    app.env = 'development'
-    app.debug = True  # Enable debug mode
-
-    app.cdc_config = config
-    env_file_path = config.get("env_file_path")
-
-    shutil.copy(env_file_path, app.root_path)
-    load_dotenv(env_file_path)
-
-
-    az_kv_az_sub_client_secret_key = config.get(
-        "az_kv_az_sub_client_secret_key")
-    az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
-        "-", "_")
-    client_secret = os.getenv(az_kv_az_sub_client_secret_key)
-    logger.info(
-        f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
-    logger.info(f"client_secret:{client_secret}")
-
-    # Set the new value
-    set_key(dotenv_path, "FLASK_DEBUG", "1")
-    set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE","1")
-    tenant_id = config.get("tenant_id")
-    client_id = config.get("client_id")
-    az_kv_key_vault_name = config.get("az_kv_key_vault_name")
-    
-    # Reload the updated .env file
-    load_dotenv(dotenv_path)
-    
-    # Trim leading and trailing whitespace from client_secret
-    if client_secret is None:
-        logger.error(f"client_secret is None")
-    else:
-        client_secret = client_secret.strip()
-
-    running_interactive = False
-
-    # Check if the client_secret is None or a zero-length string
-    if not client_secret:
-        running_interactive = True
-
-    # This will print True if client_secret is None or a zero-length string
-    print(running_interactive)
-
-    az_key_vault = pade_az_key_vault.AzKeyVault(
-        tenant_id, client_id, client_secret, az_kv_key_vault_name, running_interactive)
-    connect_api_key = az_key_vault.get_secret(
-        "OCIO-PADE-DEV-POSIT-CONNECT-SECRET")
-    # set_key(dotenv_path, az_kv_az_sub_client_secret_key, client_secret)
-    # set_key(dotenv_path, "CONNECT_API_KEY", connect_api_key)
-
-    logger.info(f"env_file_path:{env_file_path}")
-    pade_env_tracing.TracerSingleton.log_to_console = False
     tracer_singleton = pade_env_tracing.TracerSingleton.instance()
     tracer = tracer_singleton.get_tracer()
 
-    with tracer.start_as_current_span("data_ecosystem_flask main"):
-        logger.info("ran data_ecosystem_flask main")
-
     try:
-        importlib.import_module("data_ecosystem_services")
-        logger.info("data_ecosystem_services is module in pythonpath")
-    except ImportError:
-        logger.info("data_ecosystem_services is not a module in pythonpath")
-
-    if RUNNING_IN_WSL is True:
-        sys.path.append(f"/home/{CURRENT_USER_NAME}{API_PATH}")
-        logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
-        logger.info(f"/home/{CURRENT_USER_NAME}{API_PATH}")
-    else:
-        sys.path.append(os.path.abspath(
-            __file__ + "/../../../pade_python/"
-        ))
-        logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
-        logger.info(
-            os.path.abspath(
-                __file__ + "/../../../pade_python/"
-            )
-        )
+        with tracer.start_as_current_span("create_app"):
+
+            logger.info("ran create_app")
 
-    app.tracer = tracer
-    app.logger = logger
+            current_directory = os.getcwd()
 
-    return app
+            obj_env_metadata = pade_env_metadata.EnvironmentMetaData()
+            environment = get_environment_name()
+            yyyy = str(datetime.now().year)
+            dd = str(datetime.now().day).zfill(2)
+            mm = str(datetime.now().month).zfill(2)
+            running_local = True
+            change_to_flask_directory()
+            path = Path(os.getcwd())
+            repository_path_default = str(path)
+
+            logger.info(
+                f"repository_path_default:{repository_path_default}")
+
+            parameters = {
+                "project_id": "ocio_pade_dev",
+                "project_id_root": "ocio",
+                "project_id_individual": "PADE",
+                "environment": environment,
+                "yyyy": yyyy,
+                "dd": dd,
+                "mm": mm,
+                "azure_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
+                "repository_path": repository_path_default,
+                "running_local": running_local,
+            }
+            config = obj_env_metadata.get_configuration_common(
+                parameters, None)
+
+            logger.info(f"config:{config}")
+
+            app = Flask(__name__)
+            app.env = 'development'
+            app.debug = True  # Enable debug mode
+
+            app.cdc_config = config
+            env_file_path = config.get("env_file_path")
+
+            shutil.copy(env_file_path, app.root_path)
+            load_dotenv(env_file_path)
+
+            az_kv_az_sub_client_secret_key = config.get(
+                "az_kv_az_sub_client_secret_key")
+            az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
+                "-", "_")
+            client_secret = os.getenv(az_kv_az_sub_client_secret_key)
+            logger.info(
+                f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
+            logger.info(f"client_secret:{client_secret}")
+
+            # Set the new value
+            set_key(dotenv_path, "FLASK_DEBUG", "1")
+            set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE", "1")
+            tenant_id = config.get("tenant_id")
+            client_id = config.get("client_id")
+            az_kv_key_vault_name = config.get("az_kv_key_vault_name")
+
+            # Reload the updated .env file
+            load_dotenv(dotenv_path)
+
+            # Trim leading and trailing whitespace from client_secret
+            if client_secret is None:
+                logger.error(f"client_secret is None")
+            else:
+                client_secret = client_secret.strip()
+
+            running_interactive = False
+
+            # Check if the client_secret is None or a zero-length string
+            if not client_secret:
+                running_interactive = True
+
+            az_key_vault = pade_az_key_vault.AzKeyVault(
+                tenant_id, client_id, client_secret, az_kv_key_vault_name, running_interactive)
+            connect_api_key = az_key_vault.get_secret(
+                "OCIO-PADE-DEV-POSIT-CONNECT-SECRET")
+            # set_key(dotenv_path, az_kv_az_sub_client_secret_key, client_secret)
+            # set_key(dotenv_path, "CONNECT_API_KEY", connect_api_key)
+
+            logger.info(f"env_file_path:{env_file_path}")
+            pade_env_tracing.TracerSingleton.log_to_console = False
+
+            try:
+                importlib.import_module("data_ecosystem_services")
+                logger.info("data_ecosystem_services is module in pythonpath")
+            except ImportError:
+                logger.error(
+                    "data_ecosystem_services is not a module in pythonpath")
+
+            if RUNNING_IN_WSL is True:
+                sys.path.append(f"/home/{CURRENT_USER_NAME}{API_PATH}")
+                logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
+                logger.info(f"/home/{CURRENT_USER_NAME}{API_PATH}")
+            else:
+                sys.path.append(os.path.abspath(
+                    __file__ + "/../../../pade_python/"
+                ))
+                logger.info(f"RUNNING_IN_WSL: {RUNNING_IN_WSL}")
+                logger.info(
+                    os.path.abspath(
+                        __file__ + "/../../../pade_python/"
+                    )
+                )
+
+            app.tracer = tracer
+            app.logger = logger
+
+            return app
+    except Exception as e:
+        app.tracer = tracer
+        app.logger = logger
+        logger.error(f"An error occurred in create_app: {str(e)}")
+        raise e
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_posit_manifests/manifest.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_posit_manifests/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9775280898876404%*

 * *Differences: {"'az_kv_gh_client_secret_key'": "'OCIO-PADE-DEV-GITHUB-ACCESS-TOKEN'",*

 * * "'gh_az_sub_client_secret_key'": "'OCIO_PADE_DEV_AZ_CLIENT_SECRET'"}*

```diff
@@ -6,14 +6,15 @@
     "az_apin_ingestion_endpoint": "https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=h$",
     "az_apin_instrumentation_key": "69b08e65-3b37-4d98-821e-bc8cc07cbefd",
     "az_kv_az_sub_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
     "az_kv_edc_client_secret_key": "OCIO-PADE-DEV-EDC-CLIENT-SECRET",
     "az_kv_edc_refresh_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
     "az_kv_edc_secret_expiration_date": "2023-12-03",
     "az_kv_edc_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
+    "az_kv_gh_client_secret_key": "OCIO-PADE-DEV-GITHUB-ACCESS-TOKEN",
     "az_kv_key_vault_name": "edav-dev-od-edo-dm-pade",
     "az_kv_posit_connect_secret_key": "OCIO-PADE-DEV-POSIT-CONNECT-SECRET",
     "az_sub_client_id": "140ec12a-3b3d-4138-8294-57d6c0e82dd6",
     "az_sub_oauth_token_endpoint": "https://login.microsoftonline.com/",
     "az_sub_subscription_id": "b6085d96-6bb5-4e70-890c-e026d0cb1d1a",
     "az_sub_subscription_name": "OCIO-TSBDEV-C1",
     "az_sub_tenant_id": "9ce70869-60db-44fd-abe8-d2767077fc8f",
@@ -74,14 +75,15 @@
     "davt_tag_program": "null",
     "delta_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_dev/",
     "edc_alation_base_url": "https://alation.edav.cdc.gov",
     "edc_alation_client_id": "PADE@cdc.gov",
     "edc_alation_user_id": 174,
     "edc_schema_location": "schema/manifest.schema.json",
     "excel_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
+    "gh_az_sub_client_secret_key": "OCIO_PADE_DEV_AZ_CLIENT_SECRET",
     "ingress_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/ingress/",
     "jira_base_url": "https://jiradc.cdc.gov",
     "jira_client_secret_key": "OCIO_PADE_DEV_JIRA_TOKEN_SECRET",
     "jira_user_password_key": "OCIO_PADE_DEV_JIRA_USER_PASSWORD",
     "json_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
     "managed_identity": "edav-dev-mid-ociopade",
     "managed_identity_type": "user_assigned",
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,41 +30,39 @@
 backcall==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 beautifulsoup4==4.12.2 ; python_version >= "3.9" and python_version < "4.0"
 bleach==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
 blinker==1.6.2 ; python_version >= "3.9" and python_version < "4.0"
 boto3==1.21.18 ; python_version >= "3.9" and python_version < "4.0"
 botocore==1.24.18 ; python_version >= "3.9" and python_version < "4.0"
 cachetools==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
-certifi==2022.12.7 ; python_version >= "3.9" and python_version < "4.0"
+certifi==2023.5.7 ; python_version >= "3.9" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0"
 chardet==5.1.0 ; python_version >= "3.9" and python_version < "4.0"
 charset-normalizer==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.9" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and (platform_system == "Windows" or sys_platform == "win32")
 comm==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
 coverage[toml]==7.2.7 ; python_version >= "3.9" and python_version < "4.0"
 cryptography==41.0.1 ; python_version >= "3.9" and python_version < "4.0"
-data-ecosystem-services==202306.0.20 ; python_version >= "3.9" and python_version < "4.0"
+data-ecosystem-services==202306.0.26 ; python_version >= "3.9" and python_version < "4.0"
 ddlparse==1.10.0 ; python_version >= "3.9" and python_version < "4.0"
 debugpy==1.6.7 ; python_version >= "3.9" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.9" and python_version < "4.0"
 defusedxml==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
-delta-spark==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 deprecated==1.2.14 ; python_version >= "3.9" and python_version < "4.0"
 docutils==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 entrypoints==0.4 ; python_version >= "3.9" and python_version < "4.0"
 et-xmlfile==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
 exceptiongroup==1.1.1 ; python_version >= "3.9" and python_version < "3.11"
 executing==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
 fastjsonschema==2.17.1 ; python_version >= "3.9" and python_version < "4.0"
 fixedint==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
 flake8==4.0.1 ; python_version >= "3.9" and python_version < "4.0"
 flask-restful==0.3.10 ; python_version >= "3.9" and python_version < "4.0"
 flask-restx==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
-flask-sslify==0.1.5 ; python_version >= "3.9" and python_version < "4.0"
 flask==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 fqdn==1.5.1 ; python_version >= "3.9" and python_version < "4"
 fsspec==2023.6.0 ; python_version >= "3.9" and python_version < "4.0"
 google-api-core==2.11.1 ; python_version >= "3.9" and python_version < "4.0"
 google-auth==2.20.0 ; python_version >= "3.9" and python_version < "4.0"
 googleapis-common-protos==1.59.1 ; python_version >= "3.9" and python_version < "4.0"
 html2text==2020.1.16 ; python_version >= "3.9" and python_version < "4.0"
@@ -144,43 +142,42 @@
 portalocker==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 prometheus-client==0.17.0 ; python_version >= "3.9" and python_version < "4.0"
 prompt-toolkit==3.0.38 ; python_version >= "3.9" and python_version < "4.0"
 protobuf==4.23.3 ; python_version >= "3.9" and python_version < "4.0"
 psutil==5.9.5 ; python_version >= "3.9" and python_version < "4.0"
 ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform != "win32" or os_name != "nt")
 pure-eval==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
-py4j==0.10.9.7 ; python_version >= "3.9" and python_version < "4.0"
 pyarrow==10.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pyasn1-modules==0.3.0 ; python_version >= "3.9" and python_version < "4.0"
 pyasn1==0.5.0 ; python_version >= "3.9" and python_version < "4.0"
 pycodestyle==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0"
 pydash==7.0.4 ; python_version >= "3.9" and python_version < "4.0"
 pyflakes==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 pygments==2.15.1 ; python_version >= "3.9" and python_version < "4.0"
 pyjwt==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 pyjwt[crypto]==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 pyparsing==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
 pyreadstat==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
 pyrsistent==0.19.3 ; python_version >= "3.9" and python_version < "4.0"
-pyspark==3.4.1 ; python_version >= "3.9" and python_version < "4.0"
 pytest-cov==4.1.0 ; python_version >= "3.9" and python_version < "4.0"
 pytest==7.4.0 ; python_version >= "3.9" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 python-json-logger==2.0.7 ; python_version >= "3.9" and python_version < "4.0"
 pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0"
 pywin32==306 ; python_version >= "3.9" and (sys_platform == "win32" or platform_system == "Windows") and python_version < "4.0" and (platform_python_implementation != "PyPy" or platform_system == "Windows")
 pywinpty==2.0.10 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
 pyyaml==6.0 ; python_version >= "3.9" and python_version < "4.0"
 pyzmq==25.1.0 ; python_version >= "3.9" and python_version < "4.0"
 requests-oauthlib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0"
 rfc3339-validator==0.1.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3986-validator==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
+rich==13.4.2 ; python_version >= "3.9" and python_version < "4.0"
 rsa==4.9 ; python_version >= "3.9" and python_version < "4"
 rsconnect-jupyter==1.8.0 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect-python==1.17.1 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
 s3transfer==0.5.2 ; python_version >= "3.9" and python_version < "4.0"
 semver==2.13.0 ; python_version >= "3.9" and python_version < "4.0"
 send2trash==1.8.2 ; python_version >= "3.9" and python_version < "4.0"
@@ -206,17 +203,19 @@
 sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.9" and python_version < "4.0"
 stack-data==0.6.2 ; python_version >= "3.9" and python_version < "4.0"
 style==1.1.6 ; python_version >= "3.9" and python_version < "4.0"
 terminado==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 testresources==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tinycss2==1.2.1 ; python_version >= "3.9" and python_version < "4.0"
+toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tornado==6.3.2 ; python_version >= "3.9" and python_version < "4.0"
 traitlets==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
+tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 typing-extensions==4.6.3 ; python_version >= "3.9" and python_version < "4.0"
 tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0"
 unify==0.5 ; python_version >= "3.9" and python_version < "4.0"
 untokenize==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 uri-template==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 urllib3==1.26.16 ; python_version >= "3.9" and python_version < "4.0"
 wcwidth==0.2.6 ; python_version >= "3.9" and python_version < "4.0"
```

### Comparing `data_ecosystem_flask-202306.0.29/data_ecosystem_flask/schema/manifest.schema.json` & `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/schema/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/license.md` & `data_ecosystem_flask-202306.0.32/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.29/pyproject.toml` & `data_ecosystem_flask-202306.0.32/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "data_ecosystem_flask"
 authors = [{name="John Bowyer", email="zfi4@cdc.gov" }]
 description = "Data Ecosystem Flask (PADE)  - Python "
 readme = "readme.md"
 requires-python = ">=3.9,<4.0"
-version = "202306.0.20"
+version = "202306.0.26"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9"
 ]
 
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202306.0.29"
+version="202306.0.32"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
@@ -59,15 +59,16 @@
 alation = "^0.1.14"
 opentelemetry-sdk = "^1.17.0"
 azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
 opentelemetry-instrumentation-flask = "^0.39b0"
 python-dotenv = "^1.0.0"
 rsconnect = "^0.1.3"
 flask-restful = "^0.3.10"
-data-ecosystem-services = "^202306.0.20"
+data-ecosystem-services = "^202306.0.26"
+certifi = "2023.5.7"
  
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 flaskapp = "app:app"
```

### Comparing `data_ecosystem_flask-202306.0.29/readme.md` & `data_ecosystem_flask-202306.0.32/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,24 +59,24 @@
 /r-share/home/zfi4/.virtualenvs/OCIO_PADE_DEV/share/.pade_python_services_errors.log
 
 #### SetUp Deployment Env
 
 ``` sh
 /opt/python/3.9.9/bin/python3 -m venv .venv-3.9.9
 source .venv-3.9.9/bin/activate
-cd ~/data-ecosystem-services/pade-flask
+cd ~/data-ecosystem-services/pade-flask/data_ecosystem_flask
 poetry lock
 poetry install
-pip freeze > requirements.txt
+poetry export -f requirements.txt --output requirements.txt --without-hashes 
 ```
 
 #### Deploy the Flask App on POSIT (Primary)
 
 ``` sh
-cd pade-flask/data_ecosystem_flask
+cd ~/data-ecosystem-services/pade-flask/data_ecosystem_flask
 workon OCIO_PADE_DEV
 make posit-deploy
 ```
 
 #### Run your Flask App Locally on Ubuntu or WSL
 
 Steps to test web site
```

### Comparing `data_ecosystem_flask-202306.0.29/PKG-INFO` & `data_ecosystem_flask-202306.0.32/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202306.0.29
+Version: 202306.0.32
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alation (>=0.1.14,<0.2.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
-Requires-Dist: data-ecosystem-services (>=202306.0.20,<202307.0.0)
+Requires-Dist: certifi (==2023.5.7)
+Requires-Dist: data-ecosystem-services (>=202306.0.26,<202307.0.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: flask (>=2.0.0,<3.0.0)
 Requires-Dist: flask-restful (>=0.3.10,<0.4.0)
 Requires-Dist: flask-restx (>=1.1.0,<2.0.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: opentelemetry-instrumentation-flask (>=0.39b0,<0.40)
```

