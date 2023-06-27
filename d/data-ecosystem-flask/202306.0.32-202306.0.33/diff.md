# Comparing `tmp/data_ecosystem_flask-202306.0.32.tar.gz` & `tmp/data_ecosystem_flask-202306.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202306.0.32.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202306.0.33.tar", max compression
```

## Comparing `data_ecosystem_flask-202306.0.32.tar` & `data_ecosystem_flask-202306.0.33.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10359 2023-06-27 14:04:40.284817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile
--rw-r--r--   0        0        0      863 2023-06-27 14:04:40.284817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0    59837 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    12147 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0   145583 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
--rw-r--r--   0        0        0   145583 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
--rw-r--r--   0        0        0   325863 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
--rw-r--r--   0        0        0   325863 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
--rw-r--r--   0        0        0   145835 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
--rw-r--r--   0        0        0     1692 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_posit_manifests/manifest.json
--rw-r--r--   0        0        0    12165 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
--rw-r--r--   0        0        0    28571 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0     2082 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0     5462 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5240 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      374 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0    17091 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0    14015 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/schema/manifest.schema.json
--rw-r--r--   0        0        0     2401 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0    11357 2023-06-27 14:04:40.288817 data_ecosystem_flask-202306.0.32/license.md
--rw-r--r--   0        0        0     2463 2023-06-27 14:12:59.964224 data_ecosystem_flask-202306.0.32/pyproject.toml
--rw-r--r--   0        0        0    15006 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/readme.md
--rw-r--r--   0        0        0      126 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-27 14:04:40.292817 data_ecosystem_flask-202306.0.32/setup.py
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.32/PKG-INFO
+-rw-r--r--   0        0        0    10359 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/Makefile
+-rw-r--r--   0        0        0      863 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0    59818 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    12102 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0   145583 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json
+-rw-r--r--   0        0        0   145583 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json
+-rw-r--r--   0        0        0   325863 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json
+-rw-r--r--   0        0        0   325863 2023-06-27 19:06:36.475874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json
+-rw-r--r--   0        0        0   145835 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json
+-rw-r--r--   0        0        0     1692 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_posit_manifests/manifest.json
+-rw-r--r--   0        0        0    12165 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json
+-rw-r--r--   0        0        0    28571 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0     5285 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json
+-rw-r--r--   0        0        0     5240 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json
+-rw-r--r--   0        0        0      374 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/ocio/ocio_pade_dev/config/manifest.json
+-rw-r--r--   0        0        0    17091 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0    14015 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/schema/manifest.schema.json
+-rw-r--r--   0        0        0     2401 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0    11357 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/license.md
+-rw-r--r--   0        0        0     2463 2023-06-27 19:15:35.177705 data_ecosystem_flask-202306.0.33/pyproject.toml
+-rw-r--r--   0        0        0    15006 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/readme.md
+-rw-r--r--   0        0        0      126 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-27 19:06:36.479874 data_ecosystem_flask-202306.0.33/setup.py
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 data_ecosystem_flask-202306.0.33/PKG-INFO
```

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/Makefile`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,57 @@
                            type=FileStorage, required=True)
 
 # Define the blueprint
 cdc_admin_bp = Blueprint('logs', __name__,
                          url_prefix='/logs')
 
 
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
+        # Sort the log entries by date
+        log_entries.sort(key=lambda entry: datetime.strptime(
+            entry[0], "%Y-%m-%d %I:%M:%S %p"))
+
+        return render_template('log_file.html', entries=log_entries)
+
+
 app.register_blueprint(cdc_admin_bp)
 
 
 def get_posit_api_key():
 
     with tracer.start_as_current_span(f"/get_posit_api_key"):
 
@@ -189,101 +232,14 @@
         alation_user_id = config.get("edc_alation_user_id")
         api_access_token = token_endpoint.get_api_access_token(
             edc_alation_base_url, alation_user_id, alation_refresh_token)
         logger.info(f"api_access_token:{api_access_token}")
         return api_access_token
 
 
-@cdc_admin_bp.route('/get_log_file_tail/<int:number_of_lines>')
-def get_log_file_tail(number_of_lines):
-
-    with tracer.start_as_current_span(f"get_log_file_tail"):
-
-        try:
-            log_data = logger_singleton.get_log_file_tail(number_of_lines)
-        except AttributeError:
-            return "Error: Logger not correctly configured", 500
-
-        log_entries = [line.replace('\\', ':').split(None, 3)
-                       for line in log_data.strip().split('\n')]
-
-        for entry in log_entries:
-
-            try:
-                time_string = entry[1].split(":data_ecosystem_services:", 1)[0]
-                if time_string.count(':') >= 2:
-                    datetime_object = datetime.strptime(
-                        f"{entry[0]} {time_string}", "%Y-%m-%d %H:%M:%S")
-                    entry[0] = datetime_object.strftime("%Y-%m-%d %I:%M:%S %p")
-                else:
-                    raise ValueError("Invalid date and time format")
-            except ValueError:
-                return f"Error: Unable to parse date and time from {entry[0]} {time_string}", 500
-            except IndexError:
-                return f"Error: Unable to split string {entry[1]}", 500
-
-            try:
-                module, line_number = entry[1].split(
-                    ":data_ecosystem_services:", 1)[1].split(':', 1)
-                entry[1] = module
-                entry.insert(2, line_number)
-            except ValueError:
-                return f"Error: Unable to split string {entry[1]}", 500
-
-        return render_template('log_file.html', entries=log_entries)
-
-
-@app.route('/')
-def home():
-    API_DESCRIPTION = (
-        "The Program Agnostic Data Ecosystem (PADE) provides shared resources, "
-        "practices and guardrails for analysts to discover, access, link, and use "
-        "agency data in a consistent way. PADE improvements in standardized and "
-        "streamlined workflows reduce the effort required to find, access, and "
-        f"trust data. Logs can be found at [this link]({request.url_root}/logs/get_log_file_tail/1000)."
-    )
-
-    api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_cdc_security = create_api(
-        app, API_DESCRIPTION)
-
-    ns_welcome.add_resource(WelcomeSwagger, '/')
-    ns_welcome.add_resource(WelcomeSwagger, "/api/swagger")
-    ns_jira.add_resource(Task, '/tasks/<string:project>')
-    ns_alation.add_resource(MetadataExcelFileUploadRequest,
-                            "/metadata_excel_file_upload_request/<int:schema_id>")
-    ns_alation.add_resource(MetadataJsonFileUploadRequest,
-                            "/metadata_json_file_upload_request/<int:schema_id>")
-    ns_alation.add_resource(MetadataJsonFileDownload,
-                            "/metadata_json_file_download/<int:schema_id>")
-    ns_alation.add_resource(MetadataExcelFileDownload,
-                            "/metadata_excel_file_download/<int:schema_id>")
-    ns_alation.add_resource(MetadataExcelFileUpload,
-                            "/metadata_excel_file_upload")
-
-    ns_alation.add_resource(MetadataJsonFileUpload,
-                            "/metadata_json_file_upload")
-
-    ns_posit.add_resource(ConnectApiKeyVerification,
-                          "/connect_api_key_verification")
-    ns_posit.add_resource(PythonInformation, "/python_information")
-    ns_posit.add_resource(GeneratedManifest, "/generate_manifest")
-    ns_posit.add_resource(PublishManifest, "/publish_manifest")
-    ns_posit.add_resource(ContentList, "/list_content")
-    ns_posit.add_resource(
-        DeploymentBundle, "/build_deployment_bundle/<string:content_id>/<string:bundle_id>")
-    ns_posit.add_resource(DeploymentBundleList,
-                          "/list_deployment_bundles/<string:content_id>")
-    ns_posit.add_resource(TaskStatus, "/get_task_status/<string:task_id>")
-
-    ns_cdc_security.add_resource(
-        AzSubscriptionClientSecretVerification, "/verify_az_sub_client_secret")
-
-    return {"message": "Welcome to our API"}
-
-
 class WelcomeSwagger(Resource):
     def get(self):
         """
         Returns the Swagger API documentation.
 
         Returns:
             dict: The Swagger API documentation schema.
@@ -567,15 +523,15 @@
         """
 
         with tracer.start_as_current_span(f"/metadata_json_file_download/{schema_id}"):
             try:
                 config = app.cdc_config
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 api_access_token = get_api_access_token(config)
-
+                environment = config.get("environment")
                 if len(api_access_token.strip()) == 0:
                     msg = "Alation API Access Token is not set"
                     logger.error(msg)
                     return {"error": f"An unexpected error occurred: {msg}"}
 
                 logger.info("###### GET SCHEMA #######")
                 headers = {
@@ -583,14 +539,16 @@
                     "Content-Type": "application/json",
                 }
                 api_url = f"/integration/v1/schema/{schema_id}/"
                 schema_url = edc_alation_base_url + api_url
                 schema = pade_schema.Schema()
                 logger.info(f"schema_url: {schema_url}")
                 logger.info(f"headers: {headers}")
+                logger.info(f"environment: {environment}")
+
                 schema_results = schema.get_schema(
                     headers, edc_alation_base_url, schema_id
                 )
                 logger.info(f"schema_results: {str(schema_results)}")
                 response_schema_text = "not_set"
                 datasource_id = -1
                 # Check the response status code to determine if successful
@@ -598,17 +556,18 @@
                     # Extract the API token from the response
                     schema_name = schema_results.get("name")
                     datasource_id = schema_results.get("ds_id")
                 else:
                     response_schema_text = schema_results.get("reason")
                     error_msg = "Failed to get schema:" + \
                         str(response_schema_text)
-                    error_msg = error_msg + " for schema_id: " + str(schema_id)
+                    error_msg = error_msg + f" for environment: {environment}"
                     error_msg = error_msg + \
-                        " and schema_name: " + str(schema_name)
+                        " for schema_url: " + str(schema_url)
+                    error_msg = error_msg + " for schema_id: " + str(schema_id)
                     error_msg = error_msg + \
                         " and datasource_id: " + str(datasource_id)
                     error_msg = error_msg + \
                         " and schema_results: " + str(schema_results)
                     logger.error(error_msg)
                     return {"error": error_msg}
 
@@ -633,15 +592,15 @@
 
                 schema_location = config.get("edc_schema_location")
                 logger.info(
                     "Loading manifest schema from {0}".format(schema_location))
                 manifest = pade_manifest.Manifest(schema_location)
                 obj_file = pade_env_file.EnvironmentFile()
                 app_dir = os.path.dirname(os.path.abspath(__file__))
-                environment = config.get("environment")
+
                 yyyy = config.get("yyyy")
                 mm = config.get("mm")
                 dd = config.get("dd")
                 manifest_path = (
                     app_dir + "/" + environment + "_manifests/"
                 )
                 manifest_file = (
@@ -1517,10 +1476,53 @@
 FlaskInstrumentor().instrument_app(app)
 # When running in Posit Workbench, apply ProxyFix middleware
 # See: https://flask.palletsprojects.com/en/2.2.x/deploying/proxy_fix/
 if "RS_SERVER_URL" in os.environ and os.environ["RS_SERVER_URL"]:
     from werkzeug.middleware.proxy_fix import ProxyFix
     app.wsgi_app = ProxyFix(app.wsgi_app, x_prefix=1)
 
+API_DESCRIPTION = (
+    "The Program Agnostic Data Ecosystem (PADE) provides shared resources, "
+    "practices and guardrails for analysts to discover, access, link, and use "
+    "agency data in a consistent way. PADE improvements in standardized and "
+    "streamlined workflows reduce the effort required to find, access, and "
+    f"trust data."
+)
+
+api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_cdc_security = create_api(
+    app, API_DESCRIPTION)
+
+ns_welcome.add_resource(WelcomeSwagger, '/')
+ns_welcome.add_resource(WelcomeSwagger, "/api/swagger")
+ns_jira.add_resource(Task, '/tasks/<string:project>')
+ns_alation.add_resource(MetadataExcelFileUploadRequest,
+                        "/metadata_excel_file_upload_request/<int:schema_id>")
+ns_alation.add_resource(MetadataJsonFileUploadRequest,
+                        "/metadata_json_file_upload_request/<int:schema_id>")
+ns_alation.add_resource(MetadataJsonFileDownload,
+                        "/metadata_json_file_download/<int:schema_id>")
+ns_alation.add_resource(MetadataExcelFileDownload,
+                        "/metadata_excel_file_download/<int:schema_id>")
+ns_alation.add_resource(MetadataExcelFileUpload,
+                        "/metadata_excel_file_upload")
+
+ns_alation.add_resource(MetadataJsonFileUpload,
+                        "/metadata_json_file_upload")
+
+ns_posit.add_resource(ConnectApiKeyVerification,
+                      "/connect_api_key_verification")
+ns_posit.add_resource(PythonInformation, "/python_information")
+ns_posit.add_resource(GeneratedManifest, "/generate_manifest")
+ns_posit.add_resource(PublishManifest, "/publish_manifest")
+ns_posit.add_resource(ContentList, "/list_content")
+ns_posit.add_resource(
+    DeploymentBundle, "/build_deployment_bundle/<string:content_id>/<string:bundle_id>")
+ns_posit.add_resource(DeploymentBundleList,
+                      "/list_deployment_bundles/<string:content_id>")
+ns_posit.add_resource(TaskStatus, "/get_task_status/<string:task_id>")
+
+ns_cdc_security.add_resource(
+    AzSubscriptionClientSecretVerification, "/verify_az_sub_client_secret")
+
 
 if __name__ == "__main__":
     app.run(debug=True)
```

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/app_startup.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,14 @@
     tracer = tracer_singleton.get_tracer()
 
     try:
         with tracer.start_as_current_span("create_app"):
 
             logger.info("ran create_app")
 
-            current_directory = os.getcwd()
-
             obj_env_metadata = pade_env_metadata.EnvironmentMetaData()
             environment = get_environment_name()
             yyyy = str(datetime.now().year)
             dd = str(datetime.now().day).zfill(2)
             mm = str(datetime.now().month).zfill(2)
             running_local = True
             change_to_flask_directory()
```

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_09.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_10.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_12.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_14.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_manifests/ocio_pade_dev_databricks_ocio_pade_dev_metadata_2023_06_15.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_posit_manifests/manifest.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_posit_manifests/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/dev_swagger_manifests/swagger_2023_06_22.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8707865168539326%*

 * *Differences: {"'az_kv_az_sub_client_secret_key'": "'OCIO-PADE-PROD-AZ-CLIENT-SECRET'",*

 * * "'az_kv_edc_client_secret_key'": "'OCIO-PADE-PROD-EDC-CLIENT-SECRET'",*

 * * "'az_kv_edc_refresh_secret_key'": "'OCIO-PADE-PROD-EDC-SECRET'",*

 * * "'az_kv_edc_secret_key'": "'OCIO-PADE-PROD-EDC-SECRET'",*

 * * "'az_kv_posit_connect_secret_key'": "'OCIO-PADE-PROD-POSIT-CONNECT-SECRET'",*

 * * "'az_sub_subscription_name'": "'OCIO-TSBPROD-C1'",*

 * * "'config_folder'": "'abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/config/'",*

 * *  […]*

```diff
@@ -1,68 +1,66 @@
 {
     "adf_data_factory_name": "na",
     "adf_devops_account_name": "null",
     "adf_devops_project_name": "null",
     "adf_devops_repository_type": "null",
     "az_apin_ingestion_endpoint": "https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=h$",
     "az_apin_instrumentation_key": "69b08e65-3b37-4d98-821e-bc8cc07cbefd",
-    "az_kv_az_sub_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
-    "az_kv_edc_client_secret_key": "OCIO-PADE-DEV-EDC-CLIENT-SECRET",
-    "az_kv_edc_refresh_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
+    "az_kv_az_sub_client_secret_key": "OCIO-PADE-PROD-AZ-CLIENT-SECRET",
+    "az_kv_edc_client_secret_key": "OCIO-PADE-PROD-EDC-CLIENT-SECRET",
+    "az_kv_edc_refresh_secret_key": "OCIO-PADE-PROD-EDC-SECRET",
     "az_kv_edc_secret_expiration_date": "2023-12-03",
-    "az_kv_edc_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
-    "az_kv_gh_client_secret_key": "OCIO-PADE-DEV-GITHUB-ACCESS-TOKEN",
+    "az_kv_edc_secret_key": "OCIO-PADE-PROD-EDC-SECRET",
     "az_kv_key_vault_name": "edav-dev-od-edo-dm-pade",
-    "az_kv_posit_connect_secret_key": "OCIO-PADE-DEV-POSIT-CONNECT-SECRET",
+    "az_kv_posit_connect_secret_key": "OCIO-PADE-PROD-POSIT-CONNECT-SECRET",
     "az_sub_client_id": "140ec12a-3b3d-4138-8294-57d6c0e82dd6",
     "az_sub_oauth_token_endpoint": "https://login.microsoftonline.com/",
     "az_sub_subscription_id": "b6085d96-6bb5-4e70-890c-e026d0cb1d1a",
-    "az_sub_subscription_name": "OCIO-TSBDEV-C1",
+    "az_sub_subscription_name": "OCIO-TSBPROD-C1",
     "az_sub_tenant_id": "9ce70869-60db-44fd-abe8-d2767077fc8f",
     "cdc_environment": "dev",
-    "config_folder": "abfss://od-edo-dm@davsynapseanalytics.dfs.core.windows.net/PADE/ocio/pade/dev/config/",
+    "config_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/config/",
     "database_name": "ocio_pade_prod",
     "databricks_repository_id": "null",
     "dav_python_app_insights_secret_key_expiration_date": "null",
     "davt_arcgis_client_id": "null",
     "davt_arcgis_secret_expiration_date": "null",
     "davt_arcgis_secret_key": "null",
     "davt_azure_resource_group_location": "eastus",
-    "davt_azure_resource_group_name": "OCIO-DAV-DEV",
+    "davt_azure_resource_group_name": "OCIO-DAV-PROD",
     "davt_azure_storage_account": "edavsynapsedatalake",
     "davt_checkpoint_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/delta/checkpoint/",
     "davt_container_database": "od-edo-dm",
     "davt_container_project": "od-edo-dm",
-    "davt_database_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_dev/",
-    "davt_database_name": "ocio_pade_dev",
+    "davt_database_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_prod/",
+    "davt_database_name": "ocio_pade_prod",
     "davt_databricks_cluster": "    0309-172114-8ez3bm99",
     "davt_databricks_devops_account_name": "NA-Uses-GitHub",
     "davt_databricks_devops_project_description": "null",
     "davt_databricks_devops_project_name": "null",
     "davt_databricks_devops_repository_name": "NA-Uses-GitHub",
     "davt_databricks_devops_repository_type": "null",
     "davt_databricks_endpoint_path_data_science": "sql/protocolv1/o/8219004871211840/0309-172114-8ez3bm99",
     "davt_databricks_endpoint_path_sql": "null",
     "davt_databricks_ghe_repository_name": "NA-Uses-GitHub",
     "davt_databricks_instance_id": "adb-8219004871211837.17.azuredatabricks.net",
-    "davt_databricks_kv_client_secret_key": " DAVT-PADE-OCIO-DEV-AZURE-CLIENT-SECRET",
     "davt_databricks_kv_scope": "edav-dev-od-edo-dm-pade",
     "davt_databricks_org": 8219004871211840,
     "davt_databricks_owner_group": "gp-u-EDAV-OD-EDO-DM-PADE-DBR-ADMIN",
-    "davt_databricks_pat_secret_key": "OCIO_PADE_DEV_DATABRICKS_CLIENT_SECRET",
+    "davt_databricks_pat_secret_key": "OCIO_PADE_PROD_DATABRICKS_CLIENT_SECRET",
     "davt_databricks_pat_secret_scope": "not_used",
     "davt_databricks_repository_id": "null",
     "davt_dcipher_client_id": "null",
     "davt_dcipher_secret_expiration_date": "null",
     "davt_dcipher_secret_key": "null",
     "davt_dependencies_pypi_secret_expiration_date": "null",
-    "davt_dependencies_pypi_secret_key": "DAVT_DEPENDENCIES_PYTHON_DEV_PYPI_CLIENT_SECRET",
-    "davt_ghe_pat_secret_key": "DAVT-PADE-OCIO-DEV-GITHUB-CLIENT-SECRET",
+    "davt_dependencies_pypi_secret_key": "DAVT_DEPENDENCIES_PYTHON_PROD_PYPI_CLIENT_SECRET",
+    "davt_ghe_pat_secret_key": "DAVT-PADE-OCIO-PROD-GITHUB-CLIENT-SECRET",
     "davt_oauth_databricks_resource_id": "2ff814a6-3304-4ab8-85cb-cd0e6f879c1d",
-    "davt_oauth_sp_kv_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
+    "davt_oauth_sp_kv_client_secret_key": "OCIO-PADE-PROD-AZ-CLIENT-SECRET",
     "davt_oauth_sp_kv_endpoint_key": "OBSOLETE_TO_REMOVE_COLUMN",
     "davt_oauth_sp_redirect_url": "http://localhost",
     "davt_project_id": "ocio_pade",
     "davt_project_id_individual": "pade",
     "davt_project_id_root": "ocio",
     "davt_project_id_templates": "davt",
     "davt_pypi_repository_url": "https://test.pypi.org/",
@@ -70,22 +68,21 @@
     "davt_root_project_url": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/",
     "davt_services_python_version": "null",
     "davt_tag_center": "ocio",
     "davt_tag_cost_center": "null",
     "davt_tag_poc": "zfi4",
     "davt_tag_program": "null",
     "delta_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_dev/",
-    "edc_alation_base_url": "https://alation.edav.cdc.gov",
+    "edc_alation_base_url": "https://edc.cdc.gov",
     "edc_alation_client_id": "PADE@cdc.gov",
     "edc_alation_user_id": 174,
     "edc_schema_location": "schema/manifest.schema.json",
     "excel_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
-    "gh_az_sub_client_secret_key": "OCIO_PADE_DEV_AZ_CLIENT_SECRET",
     "ingress_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/ingress/",
     "jira_base_url": "https://jiradc.cdc.gov",
-    "jira_client_secret_key": "OCIO_PADE_DEV_JIRA_TOKEN_SECRET",
-    "jira_user_password_key": "OCIO_PADE_DEV_JIRA_USER_PASSWORD",
+    "jira_client_secret_key": "OCIO_PADE_PROD_JIRA_TOKEN_SECRET",
+    "jira_user_password_key": "OCIO_PADE_PROD_JIRA_USER_PASSWORD",
     "json_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
     "managed_identity": "edav-dev-mid-ociopade",
     "managed_identity_type": "user_assigned",
     "posit_connect_base_url": "https://rconnect.edav.cdc.gov:8080/"
 }
```

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.prod.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/ocio/ocio_pade_dev/config/config.dev.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8707865168539326%*

 * *Differences: {"'az_kv_az_sub_client_secret_key'": "'OCIO-PADE-DEV-AZ-CLIENT-SECRET'",*

 * * "'az_kv_edc_client_secret_key'": "'OCIO-PADE-DEV-EDC-CLIENT-SECRET'",*

 * * "'az_kv_edc_refresh_secret_key'": "'OCIO-PADE-DEV-EDC-SECRET'",*

 * * "'az_kv_edc_secret_key'": "'OCIO-PADE-DEV-EDC-SECRET'",*

 * * "'az_kv_gh_client_secret_key'": "'OCIO-PADE-DEV-GITHUB-ACCESS-TOKEN'",*

 * * "'az_kv_posit_connect_secret_key'": "'OCIO-PADE-DEV-POSIT-CONNECT-SECRET'",*

 * * "'az_sub_subscription_name'": "'OCIO-TSBDEV-C1'",*

 * * "'config_folder'": "'abfss://od-edo-dm@davsyn […]*

```diff
@@ -1,66 +1,68 @@
 {
     "adf_data_factory_name": "na",
     "adf_devops_account_name": "null",
     "adf_devops_project_name": "null",
     "adf_devops_repository_type": "null",
     "az_apin_ingestion_endpoint": "https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=h$",
     "az_apin_instrumentation_key": "69b08e65-3b37-4d98-821e-bc8cc07cbefd",
-    "az_kv_az_sub_client_secret_key": "OCIO-PADE-PROD-AZ-CLIENT-SECRET",
-    "az_kv_edc_client_secret_key": "OCIO-PADE-PROD-EDC-CLIENT-SECRET",
-    "az_kv_edc_refresh_secret_key": "OCIO-PADE-PROD-EDC-SECRET",
+    "az_kv_az_sub_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
+    "az_kv_edc_client_secret_key": "OCIO-PADE-DEV-EDC-CLIENT-SECRET",
+    "az_kv_edc_refresh_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
     "az_kv_edc_secret_expiration_date": "2023-12-03",
-    "az_kv_edc_secret_key": "OCIO-PADE-PROD-EDC-SECRET",
+    "az_kv_edc_secret_key": "OCIO-PADE-DEV-EDC-SECRET",
+    "az_kv_gh_client_secret_key": "OCIO-PADE-DEV-GITHUB-ACCESS-TOKEN",
     "az_kv_key_vault_name": "edav-dev-od-edo-dm-pade",
-    "az_kv_posit_connect_secret_key": "OCIO-PADE-PROD-POSIT-CONNECT-SECRET",
+    "az_kv_posit_connect_secret_key": "OCIO-PADE-DEV-POSIT-CONNECT-SECRET",
     "az_sub_client_id": "140ec12a-3b3d-4138-8294-57d6c0e82dd6",
     "az_sub_oauth_token_endpoint": "https://login.microsoftonline.com/",
     "az_sub_subscription_id": "b6085d96-6bb5-4e70-890c-e026d0cb1d1a",
-    "az_sub_subscription_name": "OCIO-TSBPROD-C1",
+    "az_sub_subscription_name": "OCIO-TSBDEV-C1",
     "az_sub_tenant_id": "9ce70869-60db-44fd-abe8-d2767077fc8f",
     "cdc_environment": "dev",
-    "config_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/config/",
+    "config_folder": "abfss://od-edo-dm@davsynapseanalytics.dfs.core.windows.net/PADE/ocio/pade/dev/config/",
     "database_name": "ocio_pade_prod",
     "databricks_repository_id": "null",
     "dav_python_app_insights_secret_key_expiration_date": "null",
     "davt_arcgis_client_id": "null",
     "davt_arcgis_secret_expiration_date": "null",
     "davt_arcgis_secret_key": "null",
     "davt_azure_resource_group_location": "eastus",
-    "davt_azure_resource_group_name": "OCIO-DAV-PROD",
+    "davt_azure_resource_group_name": "OCIO-DAV-DEV",
     "davt_azure_storage_account": "edavsynapsedatalake",
     "davt_checkpoint_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/delta/checkpoint/",
     "davt_container_database": "od-edo-dm",
     "davt_container_project": "od-edo-dm",
-    "davt_database_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_prod/",
-    "davt_database_name": "ocio_pade_prod",
+    "davt_database_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_dev/",
+    "davt_database_name": "ocio_pade_dev",
     "davt_databricks_cluster": "    0309-172114-8ez3bm99",
     "davt_databricks_devops_account_name": "NA-Uses-GitHub",
     "davt_databricks_devops_project_description": "null",
     "davt_databricks_devops_project_name": "null",
     "davt_databricks_devops_repository_name": "NA-Uses-GitHub",
     "davt_databricks_devops_repository_type": "null",
     "davt_databricks_endpoint_path_data_science": "sql/protocolv1/o/8219004871211840/0309-172114-8ez3bm99",
     "davt_databricks_endpoint_path_sql": "null",
     "davt_databricks_ghe_repository_name": "NA-Uses-GitHub",
     "davt_databricks_instance_id": "adb-8219004871211837.17.azuredatabricks.net",
+    "davt_databricks_kv_client_secret_key": " DAVT-PADE-OCIO-DEV-AZURE-CLIENT-SECRET",
     "davt_databricks_kv_scope": "edav-dev-od-edo-dm-pade",
     "davt_databricks_org": 8219004871211840,
     "davt_databricks_owner_group": "gp-u-EDAV-OD-EDO-DM-PADE-DBR-ADMIN",
-    "davt_databricks_pat_secret_key": "OCIO_PADE_PROD_DATABRICKS_CLIENT_SECRET",
+    "davt_databricks_pat_secret_key": "OCIO_PADE_DEV_DATABRICKS_CLIENT_SECRET",
     "davt_databricks_pat_secret_scope": "not_used",
     "davt_databricks_repository_id": "null",
     "davt_dcipher_client_id": "null",
     "davt_dcipher_secret_expiration_date": "null",
     "davt_dcipher_secret_key": "null",
     "davt_dependencies_pypi_secret_expiration_date": "null",
-    "davt_dependencies_pypi_secret_key": "DAVT_DEPENDENCIES_PYTHON_PROD_PYPI_CLIENT_SECRET",
-    "davt_ghe_pat_secret_key": "DAVT-PADE-OCIO-PROD-GITHUB-CLIENT-SECRET",
+    "davt_dependencies_pypi_secret_key": "DAVT_DEPENDENCIES_PYTHON_DEV_PYPI_CLIENT_SECRET",
+    "davt_ghe_pat_secret_key": "DAVT-PADE-OCIO-DEV-GITHUB-CLIENT-SECRET",
     "davt_oauth_databricks_resource_id": "2ff814a6-3304-4ab8-85cb-cd0e6f879c1d",
-    "davt_oauth_sp_kv_client_secret_key": "OCIO-PADE-PROD-AZ-CLIENT-SECRET",
+    "davt_oauth_sp_kv_client_secret_key": "OCIO-PADE-DEV-AZ-CLIENT-SECRET",
     "davt_oauth_sp_kv_endpoint_key": "OBSOLETE_TO_REMOVE_COLUMN",
     "davt_oauth_sp_redirect_url": "http://localhost",
     "davt_project_id": "ocio_pade",
     "davt_project_id_individual": "pade",
     "davt_project_id_root": "ocio",
     "davt_project_id_templates": "davt",
     "davt_pypi_repository_url": "https://test.pypi.org/",
@@ -68,21 +70,22 @@
     "davt_root_project_url": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/",
     "davt_services_python_version": "null",
     "davt_tag_center": "ocio",
     "davt_tag_cost_center": "null",
     "davt_tag_poc": "zfi4",
     "davt_tag_program": "null",
     "delta_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/Database/PADE/ocio/ocio_pade_dev/",
-    "edc_alation_base_url": "https://edc.cdc.gov",
+    "edc_alation_base_url": "https://dev.alation.edav.cdc.gov",
     "edc_alation_client_id": "PADE@cdc.gov",
     "edc_alation_user_id": 174,
     "edc_schema_location": "schema/manifest.schema.json",
     "excel_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
+    "gh_az_sub_client_secret_key": "OCIO_PADE_DEV_AZ_CLIENT_SECRET",
     "ingress_folder": "abfss://od-edo-dm@edavsynapsedatalake.dfs.core.windows.net/PADE/ocio/pade/dev/ingress/",
     "jira_base_url": "https://jiradc.cdc.gov",
-    "jira_client_secret_key": "OCIO_PADE_PROD_JIRA_TOKEN_SECRET",
-    "jira_user_password_key": "OCIO_PADE_PROD_JIRA_USER_PASSWORD",
+    "jira_client_secret_key": "OCIO_PADE_DEV_JIRA_TOKEN_SECRET",
+    "jira_user_password_key": "OCIO_PADE_DEV_JIRA_USER_PASSWORD",
     "json_metadata_az_storage_queue_name": "OCIO_PADE_JSON_METADATA_STORAGE_QUEUE",
     "managed_identity": "edav-dev-mid-ociopade",
     "managed_identity_type": "user_assigned",
     "posit_connect_base_url": "https://rconnect.edav.cdc.gov:8080/"
 }
```

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/schema/manifest.schema.json` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/schema/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202306.0.33/data_ecosystem_flask/templates/log_file.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/license.md` & `data_ecosystem_flask-202306.0.33/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/pyproject.toml` & `data_ecosystem_flask-202306.0.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202306.0.32"
+version="202306.0.33"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `data_ecosystem_flask-202306.0.32/readme.md` & `data_ecosystem_flask-202306.0.33/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202306.0.32/PKG-INFO` & `data_ecosystem_flask-202306.0.33/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202306.0.32
+Version: 202306.0.33
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

