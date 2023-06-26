# Comparing `tmp/uw_saml-1.2.3.tar.gz` & `tmp/uw_saml-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw_saml-1.2.3.tar", max compression
+gzip compressed data, was "uw_saml-1.2.4.tar", max compression
```

## Comparing `uw_saml-1.2.3.tar` & `uw_saml-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      564 2023-06-08 22:58:14.080633 uw_saml-1.2.3/LICENSE
--rw-r--r--   0        0        0      606 2023-06-08 22:58:14.080633 uw_saml-1.2.3/pyproject.toml
--rw-r--r--   0        0        0       53 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/VERSION
--rw-r--r--   0        0        0       70 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/__init__.py
--rw-r--r--   0        0        0     3221 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/auth.py
--rw-r--r--   0        0        0      389 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/__init__.py
--rw-r--r--   0        0        0     1619 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/attribute.py
--rw-r--r--   0        0        0    12055 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/federated.py
--rw-r--r--   0        0        0     2589 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/idp/uw.py
--rw-r--r--   0        0        0     1538 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/mock.py
--rw-r--r--   0        0        0      279 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/python3_saml.py
--rw-r--r--   0        0        0     2302 2023-06-08 22:58:14.080633 uw_saml-1.2.3/uw_saml2/sp.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      564 2023-06-26 23:28:18.178825 uw_saml-1.2.4/LICENSE
+-rw-r--r--   0        0        0      606 2023-06-26 23:28:18.178825 uw_saml-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-06-26 23:28:18.178825 uw_saml-1.2.4/uw_saml2/VERSION
+-rw-r--r--   0        0        0       70 2023-06-26 23:28:18.178825 uw_saml-1.2.4/uw_saml2/__init__.py
+-rw-r--r--   0        0        0     3221 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/auth.py
+-rw-r--r--   0        0        0      389 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/idp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/idp/attribute.py
+-rw-r--r--   0        0        0    12055 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/idp/federated.py
+-rw-r--r--   0        0        0     2589 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/idp/uw.py
+-rw-r--r--   0        0        0     1538 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/mock.py
+-rw-r--r--   0        0        0      279 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/python3_saml.py
+-rw-r--r--   0        0        0     2302 2023-06-26 23:28:18.182825 uw_saml-1.2.4/uw_saml2/sp.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 uw_saml-1.2.4/PKG-INFO
```

### Comparing `uw_saml-1.2.3/LICENSE` & `uw_saml-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/pyproject.toml` & `uw_saml-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uw-saml"
-version = "1.2.3"
+version = "1.2.4"
 description = "A UW-specific adapter to the python3-saml package."
 authors = []
 license = "Apache 2.0"
 packages = [
     { include = 'uw_saml2' }
 ]
```

### Comparing `uw_saml-1.2.3/uw_saml2/auth.py` & `uw_saml-1.2.4/uw_saml2/auth.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/uw_saml2/idp/attribute.py` & `uw_saml-1.2.4/uw_saml2/idp/attribute.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/uw_saml2/idp/federated.py` & `uw_saml-1.2.4/uw_saml2/idp/federated.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,30 +120,30 @@
     attribute_map = {
         f"{_attribute_prefix}/name": "saml_unique_name",
         f"{_attribute_prefix2}/objectidentifier": "saml_oid",
         f"{_attribute_prefix2}/displayname": "saml_displayname",
         f"{_attribute_prefix2}/authnmethodsreferences": "saml_authncontextclassref",
     }
     x509_cert = """
-        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
+        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
-        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
+        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
-        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"""
+        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"""
 
 
 class SccaIdp(IdpConfig):
     x509_cert = """
         MIIGFzCCBP+gAwIBAgITHQAAAV+l62jdEnLx3AAAAAABXzANBgkqhkiG9w0BAQsF
         ADCB9TELMAkGA1UEBhMCVVMxEzARBgNVBAgTCkNhbGlmb3JuaWExDzANBgNVBAcT
         BklydmluZTEfMB0GA1UEChMWU2VjdXJlQXV0aCBDb3Jwb3JhdGlvbjFCMEAGA1UE
```

### Comparing `uw_saml-1.2.3/uw_saml2/idp/uw.py` & `uw_saml-1.2.4/uw_saml2/idp/uw.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/uw_saml2/mock.py` & `uw_saml-1.2.4/uw_saml2/mock.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/uw_saml2/sp.py` & `uw_saml-1.2.4/uw_saml2/sp.py`

 * *Files identical despite different names*

### Comparing `uw_saml-1.2.3/PKG-INFO` & `uw_saml-1.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uw-saml
-Version: 1.2.3
+Version: 1.2.4
 Summary: A UW-specific adapter to the python3-saml package.
 License: Apache 2.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

