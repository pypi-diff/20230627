# Comparing `tmp/wiliot-api-4.2.0.tar.gz` & `tmp/wiliot-api-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.2.0.tar", last modified: Wed Jun 21 08:03:46 2023, max compression
+gzip compressed data, was "wiliot-api-4.3.0.tar", last modified: Mon Jun 26 23:48:12 2023, max compression
```

## Comparing `wiliot-api-4.2.0.tar` & `wiliot-api-4.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3825 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3319 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8440 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.906452 wiliot-api-4.2.0/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11109 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15211 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14099 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35610 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3825 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7512 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11151 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15211 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14099 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35975 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.479524 wiliot-api-4.3.0/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2023-06-26 23:47:55.000000 wiliot-api-4.3.0/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 23:48:12.475524 wiliot-api-4.3.0/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-26 23:48:12.000000 wiliot-api-4.3.0/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.2.0/LICENSE` & `wiliot-api-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/PKG-INFO` & `wiliot-api-4.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-api
-Version: 4.2.0
-Summary: A library for interacting with Wiliot's private Cloud API
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud services from Python
 
 ## Public Library
 
 ### MAC Installation
@@ -57,14 +40,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+
+Version 4.3.0:
+-----------------
+* Change code to match the changes in asset label API endpoint
+* All 2xx status code returned by the API are considered a success
+
 Version 4.2.0:
 -----------------
 * Changed API URLs to support new cloud environment
 * Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
 * Added a function to update multiple bridges' configuration in one call
 * Removed GATEWAY as an association type for location - not supported by the platform
 * Requiring at least one pixel to be provided when creating an asset
@@ -102,9 +91,7 @@
 for more information please read 'wiliot' package's release notes
   
   
    
 
 
 
-
-
```

### Comparing `wiliot-api-4.2.0/README.md` & `wiliot-api-4.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-api
+Version: 4.3.0
+Summary: A library for interacting with Wiliot's private Cloud API
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud services from Python
 
 ## Public Library
 
 ### MAC Installation
@@ -40,14 +57,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+
+Version 4.3.0:
+-----------------
+* Change code to match the changes in asset label API endpoint
+* All 2xx status code returned by the API are considered a success
+
 Version 4.2.0:
 -----------------
 * Changed API URLs to support new cloud environment
 * Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
 * Added a function to update multiple bridges' configuration in one call
 * Removed GATEWAY as an association type for location - not supported by the platform
 * Requiring at least one pixel to be provided when creating an asset
@@ -85,7 +108,9 @@
 for more information please read 'wiliot' package's release notes
   
   
    
 
 
 
+
+
```

### Comparing `wiliot-api-4.2.0/bitbucket-pipelines.yml` & `wiliot-api-4.3.0/bitbucket-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -65,31 +65,14 @@
             #print current version:
             - python3 wiliot_api/utils/get_version.py
             #Update patch version by git tag:
             - version="`python3 wiliot_api/utils/get_version.py next_patch`" && echo $version && git tag -a -m "[skip ci] build number $BITBUCKET_BUILD_NUMBER set the library patch version to $version." $version  && git push origin $version
             #print new version
             - python3 wiliot_api/utils/get_version.py
 
-    publish-full-version-into-codearfact:
-      - step:
-          name: Build and publish full version py-wilot into codeartifact
-          <<: *wiliot-ci-image
-          script:
-            - pip3 install setuptools_scm
-            - pip3 install gitpython
-            # get updated version number:
-            - version="`python3 wiliot_api/utils/get_version.py`"
-            # update minor version:
-            - python3 setup.py sdist bdist_wheel
-            #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
-            - echo "__version__ = '$version'" > wiliot_api/version.py
-            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_api/version.py
-            - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
-            - twine upload --repository codeartifact dist/*
-
     publish-full-version-into-new-codearfact:
       - step:
           name: Build and publish full version py-wilot into codeartifact
           image:
             name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
             aws:
               access-key: $CLOUD_AWS_ACCESS_KEY_ID
@@ -102,15 +85,15 @@
             # update minor version:
             - python3 setup.py sdist bdist_wheel
             #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_api/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_api/version.py
             - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
             - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
-            - twine upload --repository codeartifact dist/*
+            - twine upload --verbose --repository codeartifact dist/*
 
 
     publish-slim-version-into-pypi:
       - step:
           name: Build and publish slim version py-wilot into pypi
           <<: *wiliot-ci-image
           script:
```

### Comparing `wiliot-api-4.2.0/setup.py` & `wiliot-api-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/__init__.py` & `wiliot-api-4.3.0/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/api_client.py` & `wiliot-api-4.3.0/wiliot_api/api_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,29 +121,29 @@
         try:
             message = response.json()
         except:
             message = response.text
         if isinstance(message, str):
             message = {"data": message}
         message.update({'status_code': response.status_code})
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(message)
         return message
     
     def _get_file(self, path, out_file, params=None, override_client_path=None, override_api_version=None):
         """
         A version of _get which expects to get back a text/csv and requires the user to provide a file
         pointer to write the content to
         """
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
         response = requests.get(base_path_to_use + path, headers=self.headers, params=params)
         out_file.write(response.text)
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(response.text)
         return response.ok
     
     def _put(self, path, payload, override_client_path=None, override_api_version=None):
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
@@ -152,15 +152,15 @@
         try:
             message = response.json()
         except:
             message = response.text
         if isinstance(message, str):
             message = {"data": message}
         message.update({'status_code': response.status_code})
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(message)
         return message
     
     def _post(self, path, payload, params=None, files=None, override_client_path=None, override_api_version=None):
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
@@ -170,15 +170,15 @@
         try:
             message = response.json()
         except:
             message = response.text
         if isinstance(message, str):
             message = {"data": message}
         message.update({'status_code': response.status_code})
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(message)
         return message
     
     def _post_with_files(self, path, files, payload=None, params=None, override_client_path=None, override_api_version=None):
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
@@ -193,24 +193,24 @@
         try:
             message = response.json()
         except:
             message = response.text
         if isinstance(message, str):
             message = {"data": message}
         message.update({'status_code': response.status_code})
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(message)
         return message
     
     def _delete(self, path, payload=None, override_client_path=None, override_api_version=None):
         self._renew_token()
         base_path_to_use = self._get_base_url(override_client_path=override_client_path,
                                               override_api_version=override_api_version)
         response = requests.delete(base_path_to_use + urllib.parse.quote(path), headers=self.headers,
                                    data=json.dumps(payload) if payload is not None else None)
-        if response.status_code != 200:
+        if int(response.status_code/100) != 2:
             raise WiliotCloudError(response.text)
         try:
             message = response.json()
         except:
             message = response.text
         return message
```

### Comparing `wiliot-api-4.2.0/wiliot_api/edge/edge.py` & `wiliot-api-4.3.0/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.3.0/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.3.0/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.3.0/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.3.0/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/platform/platform.py` & `wiliot-api-4.3.0/wiliot_api/platform/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,68 +312,72 @@
         :return: True if disassociation was successful.
         """
         path = f"asset/{asset_id}/tag/{pixel_id}"
         try:
             res = self._delete(path, payload={})
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
-            print("Failed to associate pixel to asset")
+            print("Failed to disassociate pixel from asset")
             raise e
 
     # Asset Label calls
 
     def get_asset_labels(self, asset_id, project_id='Default'):
         """
         Get all labels for an asset by its ID
-        :param project_id:
         :param asset_id:
+        :param project_id: String - optional - unused and kept for backward compatability. Will be removed
         :return: list of labels
         """
-        path = "/project/{}/asset/{}/label".format(project_id, asset_id)
+        path = "/asset/{}/label".format(asset_id)
         res = self._get(path)
-        return res.get("data", [])
+        return [a['label'] for a in res.get("data", [])]
 
     def create_asset_label(self, asset_id, label, project_id='Default'):
         """
         Create a label for an asset
-        :param project_id: String - required
         :param asset_id: String - required - the asset to create the label for
         :param label: String - the label to create
+        :param project_id: String - optional - unused and kept for backward compatability. Will be removed
         :return: True if label created
         """
-        path = "/project/{}/asset/{}/label".format(project_id, asset_id)
+        path = "/asset/{}/label".format(asset_id)
         payload = {"label": label}
         res = self._post(path, payload)
-        return res
+        return res.get("data")
 
     def delete_asset_labels(self, asset_id, project_id='Default'):
         """
         Create all labels for an asset identified by an ID
-        :param project_id: String - required
         :param asset_id: String - required - The ID of the asset for which labels should be deleted
+        :param project_id: String - optional - unused and kept for backward compatability. Will be removed
         :return: True if successful
         """
-        path = "/project/{}/asset/{}/label".format(project_id, asset_id)
+        path = "/asset/{}/label".format(asset_id)
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete POI label")
             raise e
 
     def delete_asset_label(self, asset_id, label, project_id='Default'):
         """
         Create all labels for an asset identified by an ID
-        :param project_id: String - required
         :param asset_id: String - required - The ID of the asset for which labels should be deleted
+        :param label: String - required - the label to delete
+        :param project_id: String - optional - unused and kept for backward compatability. Will be removed
         :return: True if successful
         """
-        path = "/project/{}/asset/{}/label/{}".format(project_id, asset_id, label)
+        path = "/asset/{}/delete/label".format(asset_id, label)
         try:
-            res = self._delete(path)
+            payload = {
+                "label": label
+            }
+            res = self._delete(path, payload=payload)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete POI label")
             raise e
 
     # Category calls
```

### Comparing `wiliot-api-4.2.0/wiliot_api/platform/platform_models.py` & `wiliot-api-4.3.0/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api/security/security.py` & `wiliot-api-4.3.0/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.2.0/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.3.0/wiliot_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.2.0
+Version: 4.3.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+
+Version 4.3.0:
+-----------------
+* Change code to match the changes in asset label API endpoint
+* All 2xx status code returned by the API are considered a success
+
 Version 4.2.0:
 -----------------
 * Changed API URLs to support new cloud environment
 * Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
 * Added a function to update multiple bridges' configuration in one call
 * Removed GATEWAY as an association type for location - not supported by the platform
 * Requiring at least one pixel to be provided when creating an asset
```

### Comparing `wiliot-api-4.2.0/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.3.0/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

