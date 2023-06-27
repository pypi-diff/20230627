# Comparing `tmp/mara-cron-0.9.5.tar.gz` & `tmp/mara-cron-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mara-cron-0.9.5.tar", last modified: Fri Jun 24 14:56:51 2022, max compression
+gzip compressed data, was "mara-cron-0.9.6.tar", last modified: Fri Sep 30 13:39:42 2022, max compression
```

## Comparing `mara-cron-0.9.5.tar` & `mara-cron-0.9.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-06-24 14:56:51.240059 mara-cron-0.9.5/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1079 2022-06-22 08:16:58.000000 mara-cron-0.9.5/LICENSE
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2885 2022-06-24 14:56:51.240059 mara-cron-0.9.5/PKG-INFO
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2597 2022-06-22 08:41:59.000000 mara-cron-0.9.5/README.md
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-06-24 14:56:51.230059 mara-cron-0.9.5/mara_cron/
--rw-r--r--   0 lschick   (1000) lschick   (1000)      683 2022-06-24 14:55:07.000000 mara-cron-0.9.5/mara_cron/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2031 2022-02-08 13:38:22.000000 mara-cron-0.9.5/mara_cron/cli.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2338 2022-06-22 08:16:58.000000 mara-cron-0.9.5/mara_cron/config.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3181 2022-06-22 08:16:58.000000 mara-cron-0.9.5/mara_cron/crontab.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4794 2022-06-24 14:53:58.000000 mara-cron-0.9.5/mara_cron/job.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-06-24 14:56:51.240059 mara-cron-0.9.5/mara_cron/ui/
--rw-r--r--   0 lschick   (1000) lschick   (1000)       26 2022-06-22 08:16:58.000000 mara-cron-0.9.5/mara_cron/ui/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)      951 2022-06-22 08:16:58.000000 mara-cron-0.9.5/mara_cron/ui/schedule_run.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     6779 2022-06-22 08:16:58.000000 mara-cron-0.9.5/mara_cron/views.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-06-24 14:56:51.230059 mara-cron-0.9.5/mara_cron.egg-info/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2885 2022-06-24 14:56:50.000000 mara-cron-0.9.5/mara_cron.egg-info/PKG-INFO
--rw-r--r--   0 lschick   (1000) lschick   (1000)      385 2022-06-24 14:56:51.000000 mara-cron-0.9.5/mara_cron.egg-info/SOURCES.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2022-06-24 14:56:50.000000 mara-cron-0.9.5/mara_cron.egg-info/dependency_links.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)       83 2022-06-24 14:56:50.000000 mara-cron-0.9.5/mara_cron.egg-info/requires.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)       10 2022-06-24 14:56:51.000000 mara-cron-0.9.5/mara_cron.egg-info/top_level.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)      100 2022-06-22 08:16:58.000000 mara-cron-0.9.5/pyproject.toml
--rw-r--r--   0 lschick   (1000) lschick   (1000)      551 2022-06-24 14:56:51.240059 mara-cron-0.9.5/setup.cfg
--rw-r--r--   0 lschick   (1000) lschick   (1000)       38 2022-06-22 08:16:58.000000 mara-cron-0.9.5/setup.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-30 13:39:42.755473 mara-cron-0.9.6/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1079 2022-06-22 08:16:58.000000 mara-cron-0.9.6/LICENSE
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2901 2022-09-30 13:39:42.755473 mara-cron-0.9.6/PKG-INFO
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2613 2022-09-30 13:38:14.000000 mara-cron-0.9.6/README.md
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-30 13:39:42.755473 mara-cron-0.9.6/mara_cron/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      683 2022-09-30 13:36:55.000000 mara-cron-0.9.6/mara_cron/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2031 2022-02-08 13:38:22.000000 mara-cron-0.9.6/mara_cron/cli.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2338 2022-06-22 08:16:58.000000 mara-cron-0.9.6/mara_cron/config.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3181 2022-06-22 08:16:58.000000 mara-cron-0.9.6/mara_cron/crontab.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4789 2022-06-24 15:18:15.000000 mara-cron-0.9.6/mara_cron/job.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-30 13:39:42.755473 mara-cron-0.9.6/mara_cron/ui/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       26 2022-06-22 08:16:58.000000 mara-cron-0.9.6/mara_cron/ui/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      951 2022-06-22 08:16:58.000000 mara-cron-0.9.6/mara_cron/ui/schedule_run.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     6746 2022-09-30 13:34:27.000000 mara-cron-0.9.6/mara_cron/views.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2022-09-30 13:39:42.755473 mara-cron-0.9.6/mara_cron.egg-info/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2901 2022-09-30 13:39:42.000000 mara-cron-0.9.6/mara_cron.egg-info/PKG-INFO
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      385 2022-09-30 13:39:42.000000 mara-cron-0.9.6/mara_cron.egg-info/SOURCES.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2022-09-30 13:39:42.000000 mara-cron-0.9.6/mara_cron.egg-info/dependency_links.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       83 2022-09-30 13:39:42.000000 mara-cron-0.9.6/mara_cron.egg-info/requires.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       10 2022-09-30 13:39:42.000000 mara-cron-0.9.6/mara_cron.egg-info/top_level.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      100 2022-06-22 08:16:58.000000 mara-cron-0.9.6/pyproject.toml
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      551 2022-09-30 13:39:42.755473 mara-cron-0.9.6/setup.cfg
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       38 2022-06-22 08:16:58.000000 mara-cron-0.9.6/setup.py
```

### Comparing `mara-cron-0.9.5/LICENSE` & `mara-cron-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mara-cron-0.9.5/PKG-INFO` & `mara-cron-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mara-cron
-Version: 0.9.5
+Version: 0.9.6
 Summary: Lets you manage cron jobs via mara
 Home-page: https://github.com/mara/mara-cron
 Author: Mara contributors
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -39,20 +39,20 @@
 
 ```python
 def MARA_CRON_JOBS():
     from mara_cron.job import CronJob, MaraJob
     return [
         CronJob(id='cleanup_data_folder',
                 description='Clean up the data folder',
-                time_pattern='0 0 * * *',
+                default_time_pattern='0 0 * * *',
                 command='rm -rf /data/*',
                 enabled=False),
         MaraJob(id='nightly',
                 description="Nightly run of the BI system",
-                time_pattern='0 1 * * *',
+                default_time_pattern='0 1 * * *',
                 command='mara_pipelines.ui.run'),
     ]
 ```
 
 ## Local config
 
 Sample local config to activate crontab management in your mara app:
```

### Comparing `mara-cron-0.9.5/README.md` & `mara-cron-0.9.6/mara_cron.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: mara-cron
+Version: 0.9.6
+Summary: Lets you manage cron jobs via mara
+Home-page: https://github.com/mara/mara-cron
+Author: Mara contributors
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # Mara Cron
 
 Mini package for managing cron jobs via mara.
 
 &nbsp;
 
 ## Installation
@@ -27,20 +39,20 @@
 
 ```python
 def MARA_CRON_JOBS():
     from mara_cron.job import CronJob, MaraJob
     return [
         CronJob(id='cleanup_data_folder',
                 description='Clean up the data folder',
-                time_pattern='0 0 * * *',
+                default_time_pattern='0 0 * * *',
                 command='rm -rf /data/*',
                 enabled=False),
         MaraJob(id='nightly',
                 description="Nightly run of the BI system",
-                time_pattern='0 1 * * *',
+                default_time_pattern='0 1 * * *',
                 command='mara_pipelines.ui.run'),
     ]
 ```
 
 ## Local config
 
 Sample local config to activate crontab management in your mara app:
```

### Comparing `mara-cron-0.9.5/mara_cron/__init__.py` & `mara-cron-0.9.6/mara_cron/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Make the functionalities of this package auto-discoverable by mara-app"""
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 
 
 def MARA_CONFIG_MODULES():
     from . import config
     return [config]
```

### Comparing `mara-cron-0.9.5/mara_cron/cli.py` & `mara-cron-0.9.6/mara_cron/cli.py`

 * *Files identical despite different names*

### Comparing `mara-cron-0.9.5/mara_cron/config.py` & `mara-cron-0.9.6/mara_cron/config.py`

 * *Files identical despite different names*

### Comparing `mara-cron-0.9.5/mara_cron/crontab.py` & `mara-cron-0.9.6/mara_cron/crontab.py`

 * *Files identical despite different names*

### Comparing `mara-cron-0.9.5/mara_cron/job.py` & `mara-cron-0.9.6/mara_cron/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 log_command = f'{{ echo "MARA CRON JOB {self.id} START $(date)"; {self.command}; echo "MARA CRON JOB {self.id} END $(date)" ; }}'
 
                 if '$' not in log_full_path:
                     log_full_path = shlex.quote(log_full_path)
 
                 return f'{log_command} >> {log_full_path} 2>&1'
 
-        if self.max_retries:
+        if max_retries:
             return f"for i in {' '.join([str(2**(i+3)) for i in range(max_retries+1)])} 0; do ({self.command}) && break || sleep $i; done"
 
         return self.command
 
 
 class MaraJob(CronJob):
     """ A configuration for a mara job"""
```

### Comparing `mara-cron-0.9.5/mara_cron/ui/schedule_run.py` & `mara-cron-0.9.6/mara_cron/ui/schedule_run.py`

 * *Files identical despite different names*

### Comparing `mara-cron-0.9.5/mara_cron/views.py` & `mara-cron-0.9.6/mara_cron/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                                                  else acl.inline_permission_denied_message()
                                              ],
                                              _.td[
                                                  _.span[
                                                     bootstrap.button(url=flask.url_for('mara_cron.do_schedule_run', job_id=cronjob_id),
                                                                     label='Schedule run', icon='play',
                                                                     title='Schedule this task to run in less then 1 minute')
-                                                        if cronjob.get('enabled',False) and config.allow_run_from_web_ui() else '',
+                                                        if config.allow_run_from_web_ui() else '',
                                                  ] if current_user_has_permission
                                                  else acl.inline_permission_denied_message()
                                              ]] for cronjob_id, cronjob in module['cronjobs'].items()])
                                     ]) if module['cronjobs'] else '')
               for module_name, module in sorted(_cronjob_modules().items())],
         title='Mara Crontab')
```

### Comparing `mara-cron-0.9.5/mara_cron.egg-info/PKG-INFO` & `mara-cron-0.9.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: mara-cron
-Version: 0.9.5
-Summary: Lets you manage cron jobs via mara
-Home-page: https://github.com/mara/mara-cron
-Author: Mara contributors
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # Mara Cron
 
 Mini package for managing cron jobs via mara.
 
 &nbsp;
 
 ## Installation
@@ -39,20 +27,20 @@
 
 ```python
 def MARA_CRON_JOBS():
     from mara_cron.job import CronJob, MaraJob
     return [
         CronJob(id='cleanup_data_folder',
                 description='Clean up the data folder',
-                time_pattern='0 0 * * *',
+                default_time_pattern='0 0 * * *',
                 command='rm -rf /data/*',
                 enabled=False),
         MaraJob(id='nightly',
                 description="Nightly run of the BI system",
-                time_pattern='0 1 * * *',
+                default_time_pattern='0 1 * * *',
                 command='mara_pipelines.ui.run'),
     ]
 ```
 
 ## Local config
 
 Sample local config to activate crontab management in your mara app:
```

### Comparing `mara-cron-0.9.5/setup.cfg` & `mara-cron-0.9.6/setup.cfg`

 * *Files identical despite different names*

