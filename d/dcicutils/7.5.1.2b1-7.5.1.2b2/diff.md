# Comparing `tmp/dcicutils-7.5.1.2b1.tar.gz` & `tmp/dcicutils-7.5.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.5.1.2b1.tar", max compression
+gzip compressed data, was "dcicutils-7.5.1.2b2.tar", max compression
```

## Comparing `dcicutils-7.5.1.2b1.tar` & `dcicutils-7.5.1.2b2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2023-06-23 18:53:48.240759 dcicutils-7.5.1.2b1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-06-23 18:53:48.240759 dcicutils-7.5.1.2b1/README.rst
--rw-r--r--   0        0        0        0 2023-06-23 18:53:48.240759 dcicutils-7.5.1.2b1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-06-23 18:53:48.240759 dcicutils-7.5.1.2b1/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-06-23 18:53:48.240759 dcicutils-7.5.1.2b1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    16577 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-06-23 18:53:48.244759 dcicutils-7.5.1.2b1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3972 2023-06-23 18:53:48.248759 dcicutils-7.5.1.2b1/pyproject.toml
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.5.1.2b1/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.5.1.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/README.rst
+-rw-r--r--   0        0        0        0 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-06-24 20:00:08.568741 dcicutils-7.5.1.2b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    16705 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-06-24 20:00:08.572741 dcicutils-7.5.1.2b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3972 2023-06-24 20:00:08.576741 dcicutils-7.5.1.2b2/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.5.1.2b2/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.5.1.2b2/PKG-INFO
```

### Comparing `dcicutils-7.5.1.2b1/LICENSE.txt` & `dcicutils-7.5.1.2b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/README.rst` & `dcicutils-7.5.1.2b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/base.py` & `dcicutils-7.5.1.2b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/beanstalk_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/cloudformation_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/codebuild_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/command_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/common.py` & `dcicutils-7.5.1.2b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/creds_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/data_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/deployment_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/diff_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/docker_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ecr_scripts.py` & `dcicutils-7.5.1.2b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ecr_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ecs_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/env_base.py` & `dcicutils-7.5.1.2b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/env_manager.py` & `dcicutils-7.5.1.2b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/env_scripts.py` & `dcicutils-7.5.1.2b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/env_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/env_utils_legacy.py` & `dcicutils-7.5.1.2b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/es_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/exceptions.py` & `dcicutils-7.5.1.2b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ff_mocks.py` & `dcicutils-7.5.1.2b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ff_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/function_cache_decorator.py` & `dcicutils-7.5.1.2b2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/glacier_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/jh_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/kibana/dashboards.json` & `dcicutils-7.5.1.2b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/kibana/readme.md` & `dcicutils-7.5.1.2b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/lang_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/license_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/license_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 try:
     import piplicenses
-except ImportError:
+except ImportError:  # pragma: no cover - not worth unit testing this case
     raise Exception("The dcicutils.license_utils module is intended for use at development time, not runtime."
                     " It does not export a requirement for the pip-licenses library,"
                     " but to use this in your unit tests, you are expected to assure a dev dependency on that library"
                     " as part of the [tool.poetry.dependencies] section of your pyproject.toml file."
                     " If you are trying to manually evaluate the utility of this library, you can"
                     " do 'pip install pip-licenses' and then retry importing this library.")
 # or you can comment out the above raise of Exception and instead execute:
@@ -187,16 +187,16 @@
 class UnacceptableLicenseFailure(Exception):
 
     def __init__(self, message=None, unacceptable_licenses=None):
         self.unacceptable_licenses = unacceptable_licenses
         if not message:
             if unacceptable_licenses:
                 message = there_are(unacceptable_licenses, kind='unacceptable license')
-            else:
-                message = "One or more licenses are unacceptable."
+            else:  # any null value, even things like [] or {}, which is odd, but not likely to happen
+                message = "Licenses are unacceptable."
         super().__init__(message)
 
 
 class C4InfrastructureLicenseChecker(LicenseChecker):
     """
     This set of values is useful to us in Park Lab where these tools were developed.
     If you're at some other organization, we recommend you make a class that has values
```

### Comparing `dcicutils-7.5.1.2b1/dcicutils/log_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/misc_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/obfuscation_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/opensearch_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/project_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/qa_checkers.py` & `dcicutils-7.5.1.2b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/qa_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/redis_tools.py` & `dcicutils-7.5.1.2b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/redis_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/s3_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.5.1.2b2/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/secrets_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/snapshot_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/task_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/dcicutils/trace_utils.py` & `dcicutils-7.5.1.2b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.1.2b1/pyproject.toml` & `dcicutils-7.5.1.2b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.5.1.2b1"
+version = "7.5.1.2b2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.5.1.2b1/setup.py` & `dcicutils-7.5.1.2b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.5.1.2b1',
+    'version': '7.5.1.2b2',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.5.1.2b1/PKG-INFO` & `dcicutils-7.5.1.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.5.1.2b1
+Version: 7.5.1.2b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

