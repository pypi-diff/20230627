# Comparing `tmp/analysis-runner-2.41.1.tar.gz` & `tmp/analysis-runner-2.41.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-runner-2.41.1.tar", last modified: Mon Jun 26 05:02:16 2023, max compression
+gzip compressed data, was "analysis-runner-2.41.2.tar", last modified: Tue Jun 27 04:12:34 2023, max compression
```

## Comparing `analysis-runner-2.41.1.tar` & `analysis-runner-2.41.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:16.329905 analysis-runner-2.41.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-26 05:02:16.329905 analysis-runner-2.41.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:16.321905 analysis-runner-2.41.1/analysis_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cli_analysisrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cli_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/analysis_runner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:16.321905 analysis-runner-2.41.1/analysis_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 05:02:16.000000 analysis-runner-2.41.1/analysis_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:02:16.329905 analysis-runner-2.41.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:16.321905 analysis-runner-2.41.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-26 05:02:12.000000 analysis-runner-2.41.1/test/test_analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:12:34.133034 analysis-runner-2.41.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-27 04:12:34.133034 analysis-runner-2.41.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:12:34.129034 analysis-runner-2.41.2/analysis_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cli_analysisrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cli_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24822 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/analysis_runner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:12:34.133034 analysis-runner-2.41.2/analysis_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 04:12:34.000000 analysis-runner-2.41.2/analysis_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 04:12:34.133034 analysis-runner-2.41.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:12:34.133034 analysis-runner-2.41.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-27 04:12:31.000000 analysis-runner-2.41.2/test/test_analysis_runner.py
```

### Comparing `analysis-runner-2.41.1/LICENSE` & `analysis-runner-2.41.2/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/PKG-INFO` & `analysis-runner-2.41.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.41.1
+Version: 2.41.2
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.41.1/README.md` & `analysis-runner-2.41.2/README.md`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/cli.py` & `analysis-runner-2.41.2/analysis_runner/cli.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/cli_analysisrunner.py` & `analysis-runner-2.41.2/analysis_runner/cli_analysisrunner.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/cli_config.py` & `analysis-runner-2.41.2/analysis_runner/cli_config.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/cli_cromwell.py` & `analysis-runner-2.41.2/analysis_runner/cli_cromwell.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/constants.py` & `analysis-runner-2.41.2/analysis_runner/constants.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/cromwell.py` & `analysis-runner-2.41.2/analysis_runner/cromwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,15 @@
     watch_job.env('PYTHONUNBUFFERED', '1')  # makes the logs go quicker
     watch_job.image(driver_image)  # need an image with python3 + requests
 
     watch_job.command(
         query_command(
             watch_workflow,
             watch_workflow.__name__,
-            workflow_id_file,
+            str(workflow_id_file),
             max_sequential_exception_count,
             max_poll_interval,
             exponential_decrease_seconds,
             str(watch_job.output_json_path),
             setup_gcp=True,
             setup_hail=False,
         )
```

### Comparing `analysis-runner-2.41.1/analysis_runner/cromwell_model.py` & `analysis-runner-2.41.2/analysis_runner/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/dataproc.py` & `analysis-runner-2.41.2/analysis_runner/dataproc.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/git.py` & `analysis-runner-2.41.2/analysis_runner/git.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner/util.py` & `analysis-runner-2.41.2/analysis_runner/util.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/analysis_runner.egg-info/PKG-INFO` & `analysis-runner-2.41.2/analysis_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.41.1
+Version: 2.41.2
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.41.1/analysis_runner.egg-info/SOURCES.txt` & `analysis-runner-2.41.2/analysis_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.41.1/setup.py` & `analysis-runner-2.41.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='2.41.1',
+    version='2.41.2',
     description='Analysis runner to help make analysis results reproducible',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/{PKG}',
     license='MIT',
     packages=['analysis_runner'],
     include_package_data=True,
```

### Comparing `analysis-runner-2.41.1/test/test_analysis_runner.py` & `analysis-runner-2.41.2/test/test_analysis_runner.py`

 * *Files identical despite different names*

