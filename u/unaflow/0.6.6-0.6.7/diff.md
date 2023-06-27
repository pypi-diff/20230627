# Comparing `tmp/unaflow-0.6.6.tar.gz` & `tmp/unaflow-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unaflow-0.6.6.tar", last modified: Tue Jun 28 11:44:54 2022, max compression
+gzip compressed data, was "dist/unaflow-0.6.7.tar", last modified: Tue Jun 27 13:36:04 2023, max compression
```

## Comparing `unaflow-0.6.6.tar` & `unaflow-0.6.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-28 11:43:50.000000 unaflow-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-06-28 11:44:54.000000 unaflow-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-06-28 11:43:50.000000 unaflow-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-28 11:44:54.000000 unaflow-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-06-28 11:43:50.000000 unaflow-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/dags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/dags/trigger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/gcs_context_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/gcs_trigger_dag_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/trigger_dag_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/dags/trigger_dag/trigger_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/functions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/functions/opsgenie.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/functions/slack_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/operators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/operators/branch_dag_run_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/operators/check_dag_run_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/operators/clear_dag_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/operators/gcs_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-06-28 11:43:50.000000 unaflow-0.6.6/unaflow/sensors/external_dag_run_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-28 11:44:54.000000 unaflow-0.6.6/unaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-06-28 11:43:50.000000 unaflow-0.6.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:33:58.000000 unaflow-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 13:33:58.000000 unaflow-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-27 13:36:04.000000 unaflow-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 13:33:58.000000 unaflow-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 13:36:04.000000 unaflow-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 13:33:58.000000 unaflow-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/dags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/dags/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/gcs_context_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/gcs_trigger_dag_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/trigger_dag_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/dags/trigger_dag/trigger_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/functions/opsgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/functions/slack_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/operators/branch_dag_run_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/operators/check_dag_run_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/operators/clear_dag_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/operators/gcs_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 13:33:58.000000 unaflow-0.6.7/unaflow/sensors/external_dag_run_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 13:36:04.000000 unaflow-0.6.7/unaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-27 13:33:58.000000 unaflow-0.6.7/versioneer.py
```

### Comparing `unaflow-0.6.6/setup.py` & `unaflow-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/gcs_context_functions.py` & `unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/gcs_context_functions.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/dags/trigger_dag/providers/google/gcs_trigger_dag_configuration.py` & `unaflow-0.6.7/unaflow/dags/trigger_dag/providers/google/gcs_trigger_dag_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,39 +25,33 @@
         storage bucket.
     :type prefix: str
     :param single_file: If destination or destination_bucket is set, we move only one file
     :type single_file: bool
     :param google_cloud_conn_id: The connection ID to use when
         connecting to Google cloud storage.
     :type google_cloud_conn_id: str
-    :param delegate_to: The account to impersonate, if any.
-        For this to work, the service account making the request must have
-        domain-wide delegation enabled.
-    :type delegate_to: str
     :param destination_bucket:
     :param destination:
     """
 
     def __init__(self,
                  bucket: str = None,
                  prefix: str = None,
                  destination_bucket=None,
                  destination=None,
                  gcp_conn_id=None,
-                 delegate_to=None,
                  single_file=True,
                  *args, **kwargs
                  ) -> None:
         super(GcsMovefilesTriggerDagConfiguration, self).__init__(*args, **kwargs)
         self.bucket: str = bucket
         self.prefix: str = prefix
         self.destination_bucket = destination_bucket or bucket
         self.destination = destination
         self.gcp_conn_id = gcp_conn_id
-        self.delegate_to = delegate_to
         self.configuration = {**self.configuration, 'bucket': self.destination_bucket}
         self.single_file = single_file
         if self.single_file:
             self._source_objects = [XCOM_TOP_FILE]
             self.configuration = {**self.configuration,
                                   'filename': "{{ ti.xcom_pull(task_ids='move_files')[0] }}"}
         else:
@@ -66,30 +60,28 @@
                                   'filenames': "{{ ti.xcom_pull(task_ids='move_files') }}"}
 
     def create_sensor(self) -> BaseSensorOperator:
         return GCSObjectsWithPrefixExistenceSensor(
             task_id=SENSOR_TASK_ID,
             bucket=self.bucket,
             prefix=self.prefix,
-            delegate_to=self.delegate_to,
             google_cloud_conn_id=self.gcp_conn_id,
             poke_interval=self.poke_interval,
             mode=self.mode
         )
 
     def create_downstream_sensor(self) -> Union[TaskMixin, Sequence[TaskMixin]]:
         return GoogleCloudStorageCopyOperator(
             task_id="move_files",
             source_bucket=self.bucket,
             source_objects=self._source_objects,
             destination_bucket=self.destination_bucket,
             destination_object=self.destination,
             move_object=True,
             gcp_conn_id=self.gcp_conn_id,
-            delegate_to=self.delegate_to
         )
 
     def default_doc_md(self):
         return f"""# Triggering DAG for {self.trigger_dag_id}
 
 This DAG listens for files arriving in `{self.bucket}` with the prefix `{self.prefix}`.
```

### Comparing `unaflow-0.6.6/unaflow/dags/trigger_dag/trigger_dag_configuration.py` & `unaflow-0.6.7/unaflow/dags/trigger_dag/trigger_dag_configuration.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/dags/trigger_dag/trigger_dag_factory.py` & `unaflow-0.6.7/unaflow/dags/trigger_dag/trigger_dag_factory.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/functions/opsgenie.py` & `unaflow-0.6.7/unaflow/functions/opsgenie.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/functions/slack_functions.py` & `unaflow-0.6.7/unaflow/functions/slack_functions.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/operators/branch_dag_run_operator.py` & `unaflow-0.6.7/unaflow/operators/branch_dag_run_operator.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/operators/check_dag_run_operator.py` & `unaflow-0.6.7/unaflow/operators/check_dag_run_operator.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/operators/clear_dag_operator.py` & `unaflow-0.6.7/unaflow/operators/clear_dag_operator.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/operators/gcs_copy.py` & `unaflow-0.6.7/unaflow/operators/gcs_copy.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow/sensors/external_dag_run_sensor.py` & `unaflow-0.6.7/unaflow/sensors/external_dag_run_sensor.py`

 * *Files identical despite different names*

### Comparing `unaflow-0.6.6/unaflow.egg-info/SOURCES.txt` & `unaflow-0.6.7/unaflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 unaflow/__init__.py
 unaflow/_version.py
```

### Comparing `unaflow-0.6.6/versioneer.py` & `unaflow-0.6.7/versioneer.py`

 * *Files identical despite different names*

