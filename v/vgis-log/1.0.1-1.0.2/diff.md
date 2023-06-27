# Comparing `tmp/vgis_log-1.0.1.tar.gz` & `tmp/vgis_log-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_log-1.0.1.tar", last modified: Tue Jun 27 09:20:41 2023, max compression
+gzip compressed data, was "dist\vgis_log-1.0.2.tar", last modified: Tue Jun 27 09:33:01 2023, max compression
```

## Comparing `vgis_log-1.0.1.tar` & `vgis_log-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:20:41.913342 vgis_log-1.0.1/
--rw-rw-rw-   0        0        0     1022 2023-06-27 09:20:41.912341 vgis_log-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-06-27 09:06:27.000000 vgis_log-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:20:41.913342 vgis_log-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2145 2023-06-27 09:11:10.000000 vgis_log-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:20:41.902343 vgis_log-1.0.1/vgis_log/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_log-1.0.1/vgis_log/__init__.py
--rw-rw-rw-   0        0        0     5023 2023-06-27 09:18:16.000000 vgis_log-1.0.1/vgis_log/logTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:20:41.910341 vgis_log-1.0.1/vgis_log.egg-info/
--rw-rw-rw-   0        0        0     1022 2023-06-27 09:20:41.000000 vgis_log-1.0.1/vgis_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-06-27 09:20:41.000000 vgis_log-1.0.1/vgis_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:20:41.000000 vgis_log-1.0.1/vgis_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 09:20:41.000000 vgis_log-1.0.1/vgis_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 09:20:41.000000 vgis_log-1.0.1/vgis_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 09:33:01.847913 vgis_log-1.0.2/
+-rw-rw-rw-   0        0        0     1022 2023-06-27 09:33:01.847913 vgis_log-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-06-27 09:06:27.000000 vgis_log-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:33:01.847913 vgis_log-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2145 2023-06-27 09:32:55.000000 vgis_log-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:33:01.837924 vgis_log-1.0.2/vgis_log/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_log-1.0.2/vgis_log/__init__.py
+-rw-rw-rw-   0        0        0     5051 2023-06-27 09:32:45.000000 vgis_log-1.0.2/vgis_log/logTools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:33:01.845915 vgis_log-1.0.2/vgis_log.egg-info/
+-rw-rw-rw-   0        0        0     1022 2023-06-27 09:33:01.000000 vgis_log-1.0.2/vgis_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-06-27 09:33:01.000000 vgis_log-1.0.2/vgis_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:33:01.000000 vgis_log-1.0.2/vgis_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 09:33:01.000000 vgis_log-1.0.2/vgis_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 09:33:01.000000 vgis_log-1.0.2/vgis_log.egg-info/top_level.txt
```

### Comparing `vgis_log-1.0.1/PKG-INFO` & `vgis_log-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_log
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for log operator
 Home-page: https://github.com/gisfanmachel/vgisLog
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis log lib
```

### Comparing `vgis_log-1.0.1/setup.py` & `vgis_log-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_log",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
+    version="1.0.2",  # Required 发布版本号
     description="A libary for log operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisLog",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_log-1.0.1/vgis_log/logTools.py` & `vgis_log-1.0.2/vgis_log/logTools.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,26 +74,26 @@
     @staticmethod
     def set_start_log_info(logger):
         start = time.perf_counter()
         logger.info("开始时间：" + datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
         return start
 
     @staticmethod
-    def set_end_log_info(logger, start, api_path, user, request, function_title):
+    def set_end_log_info(SysLog,logger, start, api_path, user, request, function_title):
         logger.info("结束时间：" + datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
         end = time.perf_counter()
         t = end - start
         logger.info("总共用时{}秒".format(t))
-        LoggerHelper.insert_log_info(user, function_title + "成功",
+        LoggerHelper.insert_log_info(SysLog,user, function_title + "成功",
                                      api_path,
                                      HttpHelper.get_params_request(request),
                                      t, HttpHelper.get_ip_request(request), None)
 
     @staticmethod
-    def set_end_log_info_in_exception(logger, start, api_path, user, request, function_title, error_info, exp):
+    def set_end_log_info_in_exception(SysLog,logger, start, api_path, user, request, function_title, error_info, exp):
         if exp is not None:
             logger.error("{}失败：{}".format(function_title, str(exp)))
             logger.error(exp)
             logger.error(exp.__traceback__.tb_frame.f_globals["__file__"])  # 发生异常所在的文件
             logger.error(exp.__traceback__.tb_lineno)  # 发生异常所在的行数
             error_info = str(exp) + "\n代码：" + str(exp.__traceback__.tb_frame.f_globals["__file__"]) + "\n行数：" + str(
                 exp.__traceback__.tb_lineno)
@@ -108,15 +108,15 @@
                 "info": error_info
             }
         logger.info("结束时间：" + datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
         end = time.perf_counter()
         t = end - start
         logger.info("总共用时{}秒".format(t))
         # 日志入库
-        LoggerHelper.insert_log_info(user, function_title + "失败",
+        LoggerHelper.insert_log_info(SysLog,user, function_title + "失败",
                                      api_path,
                                      HttpHelper.get_params_request(request),
                                      t, HttpHelper.get_ip_request(request), error_info)
         return res
 
 
 # 主入口,进行测试
```

### Comparing `vgis_log-1.0.1/vgis_log.egg-info/PKG-INFO` & `vgis_log-1.0.2/vgis_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-log
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for log operator
 Home-page: https://github.com/gisfanmachel/vgisLog
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis log lib
```

