# Comparing `tmp/aws-ssm-tunnel-agent-1.5.1.tar.gz` & `tmp/aws-ssm-tunnel-agent-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws-ssm-tunnel-agent-1.5.1.tar", last modified: Tue Feb 21 04:59:10 2023, max compression
+gzip compressed data, was "dist/aws-ssm-tunnel-agent-1.6.0.tar", last modified: Tue Jun 27 02:20:12 2023, max compression
```

## Comparing `aws-ssm-tunnel-agent-1.5.1.tar` & `aws-ssm-tunnel-agent-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2055 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-02-21 04:59:09.000000 aws-ssm-tunnel-agent-1.5.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      978 2023-02-21 04:59:09.000000 aws-ssm-tunnel-agent-1.5.1/setup-agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2023-02-21 04:59:09.000000 aws-ssm-tunnel-agent-1.5.1/setup.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4420 2023-02-21 04:59:09.000000 aws-ssm-tunnel-agent-1.5.1/ssm-tunnel-agent
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2055 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-21 04:59:10.000000 aws-ssm-tunnel-agent-1.5.1/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2055 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-06-27 02:20:10.000000 aws-ssm-tunnel-agent-1.6.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      978 2023-06-27 02:20:10.000000 aws-ssm-tunnel-agent-1.6.0/setup-agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2023-06-27 02:20:10.000000 aws-ssm-tunnel-agent-1.6.0/setup.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4420 2023-06-27 02:20:10.000000 aws-ssm-tunnel-agent-1.6.0/ssm-tunnel-agent
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2055 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 02:20:12.000000 aws-ssm-tunnel-agent-1.6.0/setup.cfg
```

### Comparing `aws-ssm-tunnel-agent-1.5.1/aws_ssm_tunnel_agent.egg-info/PKG-INFO` & `aws-ssm-tunnel-agent-1.6.0/aws_ssm_tunnel_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tunnel-agent
-Version: 1.5.1
+Version: 1.6.0
 Summary: ssm-tunnel-agent for ssm-tunnel script from aws-ssm-tools package
 Home-page: https://github.com/mludvig/aws-ssm-tools
 Author: Michael Ludvig
 Author-email: mludvig@logix.net.nz
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mludvig/aws-ssm-tools/issues
 Project-URL: Documentation, https://github.com/mludvig/aws-ssm-tools/blob/master/README.md
```

### Comparing `aws-ssm-tunnel-agent-1.5.1/README.md` & `aws-ssm-tunnel-agent-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ssm-tunnel-agent-1.5.1/setup-agent.py` & `aws-ssm-tunnel-agent-1.6.0/setup-agent.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tunnel-agent-1.5.1/setup.py` & `aws-ssm-tunnel-agent-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tunnel-agent-1.5.1/ssm-tunnel-agent` & `aws-ssm-tunnel-agent-1.6.0/ssm-tunnel-agent`

 * *Files identical despite different names*

### Comparing `aws-ssm-tunnel-agent-1.5.1/PKG-INFO` & `aws-ssm-tunnel-agent-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tunnel-agent
-Version: 1.5.1
+Version: 1.6.0
 Summary: ssm-tunnel-agent for ssm-tunnel script from aws-ssm-tools package
 Home-page: https://github.com/mludvig/aws-ssm-tools
 Author: Michael Ludvig
 Author-email: mludvig@logix.net.nz
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mludvig/aws-ssm-tools/issues
 Project-URL: Documentation, https://github.com/mludvig/aws-ssm-tools/blob/master/README.md
```

