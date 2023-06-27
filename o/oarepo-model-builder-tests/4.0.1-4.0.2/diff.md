# Comparing `tmp/oarepo-model-builder-tests-4.0.1.tar.gz` & `tmp/oarepo-model-builder-tests-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-tests-4.0.1.tar", last modified: Thu May 25 06:30:29 2023, max compression
+gzip compressed data, was "oarepo-model-builder-tests-4.0.2.tar", last modified: Tue Jun 27 08:19:53 2023, max compression
```

## Comparing `oarepo-model-builder-tests-4.0.1.tar` & `oarepo-model-builder-tests-4.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/conftest_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/datatypes/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/utils.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/test_resource_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/test_service_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/utils_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:30:29.970601 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 06:30:29.000000 oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-25 06:30:29.974601 oarepo-model-builder-tests-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 06:26:11.000000 oarepo-model-builder-tests-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:19:53.946694 oarepo-model-builder-tests-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-27 08:19:53.946694 oarepo-model-builder-tests-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:19:53.942695 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/conftest_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:19:53.946694 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/datatypes/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:19:53.946694 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/test_resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/test_service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/utils.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/test_resource_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/test_service_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/utils_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:19:53.942695 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 08:19:53.000000 oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-27 08:19:53.946694 oarepo-model-builder-tests-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 08:16:15.000000 oarepo-model-builder-tests-4.0.2/setup.py
```

### Comparing `oarepo-model-builder-tests-4.0.1/LICENSE` & `oarepo-model-builder-tests-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.1/PKG-INFO` & `oarepo-model-builder-tests-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 4.0.1
+Version: 4.0.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-4.0.1/README.md` & `oarepo-model-builder-tests-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/conftest.py.jinja2` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/conftest.py.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from invenio_app.factory import create_api
 from invenio_records_resources.services.uow import UnitOfWork, RecordCommitOp
 import os
 
 from {{ vars.proxy.module }} import {{ vars.service.proxy }}
 {{ vars.record.class|generate_import }}
 
+@pytest.fixture
+def record_service():
+    return current_service
 
 @pytest.fixture(scope="function")
 def sample_metadata_list():
     data_path = f"{Path(__file__).parent.parent}/{{ vars.sample.file }}"
     docs = list(yaml.load_all(open(data_path), Loader=yaml.SafeLoader))
     return docs
```

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/test_resource.py.jinja2` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/test_resource.py.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         ret_paths.append(f"{cur_path}")
     return ret_paths
 
 
 def get_paths(prefix, data):
     return _get_paths(prefix, data)
 
-BASE_URL = f"http://localhost{{ "{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}"
+BASE_URL = {{ vars.resource_config.class|base_name }}.url_prefix
 """
 def check_allowed(action_name):
     permission_cls = {{ vars.service.proxy }}.config.permission_policy_cls
     permission = permission_cls(action_name)
     identity = g.identity
     auth = permission.allows(identity)
     return auth
@@ -55,24 +55,57 @@
     if action_allowed and response.status_code == authorized_response_code:
         return True
     elif not action_allowed and response.status_code == 403:
         return True
     return False
 
 
-def test_get_item({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, search_clear):
+def test_read(client_with_credentials, {{ fixtures.sample_record }}, search_clear):
     non_existing = client_with_credentials.get(f"{BASE_URL}yjuykyukyuk")
     assert non_existing.status_code == 404
 
-    get_response = client_with_credentials.get(f"{BASE_URL}{sample_record['id']}")
+    get_response = client_with_credentials.get(f"{BASE_URL}{{ "{" }}{{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.read_url }}")
     assert response_code_ok("read", True, get_response, 200)
     if is_action_allowed("read", True):
-        assert get_response.json["metadata"] == sample_record["metadata"]
+        assert get_response.json["metadata"] == {{ fixtures.sample_record }}["metadata"]
 
+def test_create(
+    client_with_credentials, client, sample_metadata_list, app, search_clear
+):
+    created_responses = []
+    for sample_metadata_point in sample_metadata_list:
+        created_responses.append(
+            client_with_credentials.post(f"{BASE_URL}", json=sample_metadata_point)
+        )
+        with app.test_client() as unauth_client:
+            unauth_response = unauth_client.post(
+                f"{BASE_URL}", json=sample_metadata_point
+            )
+            assert response_code_ok("create", False, unauth_response, 201)
+    assert all(
+        [
+            response_code_ok("create", True, new_response, 201)
+            for new_response in created_responses
+        ]
+    )
 
+    if is_action_allowed("create", True):
+        for sample_metadata_point, created_response in zip(
+            sample_metadata_list, created_responses
+        ):
+            created_response_reread = client_with_credentials.get(
+                f"{BASE_URL}{created_response.json['id']}{{ test_constants.read_url }}"
+            )
+            assert response_code_ok("read", True, created_response_reread, 200)
+            assert (
+                created_response_reread.json["metadata"]
+                == sample_metadata_point["metadata"]
+            )
+
+"""
 def test_create(
     {{ vars.tests.extra_fixtures|generate_list(end=true) }}client_with_credentials, client, sample_metadata_list, app, search_clear
 ):
     created_responses = []
     for sample_metadata_point in sample_metadata_list:
         created_responses.append(
             client_with_credentials.post(f"{BASE_URL}", json=sample_metadata_point)
@@ -92,46 +125,48 @@
                 f"{BASE_URL}{created_response.json['id']}"
             )
             assert response_code_ok("read", True, created_response_reread, 200)
             assert (
                 created_response_reread.json["metadata"]
                 == sample_metadata_point["metadata"]
             )
+"""
 
-
+"""
 def test_listing({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_records, search_clear):
     listing_response = client_with_credentials.get(BASE_URL)
     hits = listing_response.json["hits"]["hits"]
     assert len(hits) == 10
+"""
 
 
 def test_update(
-    {{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, sample_metadata_list, search_clear
+    client_with_credentials, {{ fixtures.sample_record }}, sample_metadata_list, search_clear
 ):
     non_existing = client_with_credentials.put(
-        f"{BASE_URL}yjuykyukyuk", json=sample_metadata_list[5]
+        f"{BASE_URL}yjuykyukyuk{{ test_constants.read_url }}", json=sample_metadata_list[5]
     )
 
     old_record_read_response_json = client_with_credentials.get(
-        f"{BASE_URL}{sample_record['id']}"
+        f"{BASE_URL}{{ "{" }} {{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.read_url }}"
     ).json
 
     update_response = client_with_credentials.put(
-        f"{BASE_URL}{sample_record['id']}", json=sample_metadata_list[2]
+        f"{BASE_URL}{{ "{" }} {{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.update_url }}", json=sample_metadata_list[2]
     )
 
     updated_record_read_response = client_with_credentials.get(
-        f"{BASE_URL}{sample_record['id']}"
+        f"{BASE_URL}{{ "{" }} {{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.read_url }}"
     )
 
     assert response_code_ok("read", True, updated_record_read_response, 200)
     assert response_code_ok("update", True, non_existing, 404)
     assert response_code_ok("update", True, update_response, 200)
     if is_action_allowed("update", True):
-        assert old_record_read_response_json["metadata"] == sample_record.metadata
+        assert old_record_read_response_json["metadata"] == {{ fixtures.sample_record }}.metadata
         assert (
             update_response.json["metadata"]
             == sample_metadata_list[2]["metadata"]
             != old_record_read_response_json["metadata"]
         )
         assert (
             updated_record_read_response.json["metadata"]
@@ -146,38 +181,37 @@
     # to make it work change create_url_rules in resource and allow jsonpatch in request_body_parsers in resource config
     # patch_response = client_with_credentials.patch(f"{BASE_URL}{sample_record['id']}",
     #                                                              json={"path": "/metadata/title",
     #                                                              "op": "replace",
     #                                                              "value": "UPDATED!"})
 
 
-def test_delete({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, app, search_clear):
+def test_delete(client_with_credentials, {{ fixtures.sample_record }}, app, search_clear):
     non_existing = client_with_credentials.delete(f"{BASE_URL}yjuykyukyuk")
     assert response_code_ok("delete", True, non_existing, 404)
 
-    read_response = client_with_credentials.get(f"{BASE_URL}{sample_record['id']}")
-    assert response_code_ok("read", True, read_response, 200)
-
-    delete_response = client_with_credentials.delete(f"{BASE_URL}{sample_record['id']}")
+    delete_response = client_with_credentials.delete(f"{BASE_URL}{{ "{" }} {{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.delete_url }}")
     assert response_code_ok("delete", True, delete_response, 204)
 
     if is_action_allowed("delete", True):
         deleted_get_response = client_with_credentials.delete(
-            f"{BASE_URL}{sample_record['id']}"
+            f"{BASE_URL}{{ "{" }} {{ fixtures.sample_record }}['id']{{ "}" }}{{ test_constants.delete_url }}"
         )
-        assert deleted_get_response.status_code == 410
+        assert deleted_get_response.status_code == {{ test_constants.deleted_http_code }}
 
+"""
 def test_delete_unauth(sample_record, search_clear, app):
     with app.test_client() as unauth_client:
         unauth_delete_response = unauth_client.delete(
             f"{BASE_URL}{sample_record['id']}"
         )
         assert response_code_ok("delete", False, unauth_delete_response, 204)
+"""
 
-
+{% if not test_constants.skip_search_test %}
 def test_search({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_records, sample_metadata_list, search_clear):
     if is_action_allowed("search", True):
         paths = get_paths("metadata", sample_metadata_list[0]["metadata"])
 
         for record in sample_records:
             for path in paths:
                 field_value = dict_lookup(record, path)
@@ -212,8 +246,9 @@
         res_created_fail = client_with_credentials.get(f"{BASE_URL}?q=2022-10-16")
         record_created = sample_records[0].created.isoformat() + "Z"
         res_facets = client_with_credentials.get(f"{BASE_URL}?created={record_created}")
 
         assert len(res_fail.json["hits"]["hits"]) == 0
         assert len(res_created.json["hits"]["hits"]) == 10
         assert len(res_created_fail.json["hits"]["hits"]) == 0
-        assert len(res_facets.json["hits"]["hits"]) == 1
+        assert len(res_facets.json["hits"]["hits"]) == 1
+{% endif %}
```

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests/templates/utils.py.jinja2` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests/templates/utils.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/PKG-INFO` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 4.0.1
+Version: 4.0.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/SOURCES.txt` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-4.0.1/oarepo_model_builder_tests.egg-info/entry_points.txt` & `oarepo-model-builder-tests-4.0.2/oarepo_model_builder_tests.egg-info/entry_points.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [oarepo_model_builder.builders.record]
 2010-oarepo_model_builder_setup_cfg = oarepo_model_builder_tests.oarepo_model_builder_setup_cfg:OarepoModelBuilderSetupCfgBuilder
 5020-conftest = oarepo_model_builder_tests.conftest_builder:ConftestBuilder
-5020-test_utils = oarepo_model_builder_tests.utils_builder:TestUtilsBuilder
 5021-test_resource = oarepo_model_builder_tests.test_resource_builder:TestResourceBuilder
 5022-test_service = oarepo_model_builder_tests.test_service_builder:TestServiceBuilder
 
 [oarepo_model_builder.datatypes.components]
 0200-tests = oarepo_model_builder_tests.datatypes.components:components
 
 [oarepo_model_builder.templates]
```

### Comparing `oarepo-model-builder-tests-4.0.1/setup.cfg` & `oarepo-model-builder-tests-4.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-tests
-version = 4.0.1
+version = 4.0.2
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -21,15 +21,14 @@
 
 [options.entry_points]
 oarepo_model_builder.datatypes.components = 
 	0200-tests = oarepo_model_builder_tests.datatypes.components:components
 oarepo_model_builder.builders.record = 
 	2010-oarepo_model_builder_setup_cfg = oarepo_model_builder_tests.oarepo_model_builder_setup_cfg:OarepoModelBuilderSetupCfgBuilder
 	5020-conftest  = oarepo_model_builder_tests.conftest_builder:ConftestBuilder
-	5020-test_utils = oarepo_model_builder_tests.utils_builder:TestUtilsBuilder
 	5021-test_resource  = oarepo_model_builder_tests.test_resource_builder:TestResourceBuilder
 	5022-test_service  = oarepo_model_builder_tests.test_service_builder:TestServiceBuilder
 oarepo_model_builder.templates = 
 	99-tests_templates  = oarepo_model_builder_tests
 
 [egg_info]
 tag_build =
```

