# Comparing `tmp/py-chinese-holidays-1.1.tar.gz` & `tmp/py-chinese-holidays-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-chinese-holidays-1.1.tar", last modified: Tue Jun 27 07:32:53 2023, max compression
+gzip compressed data, was "py-chinese-holidays-1.1.1.tar", last modified: Tue Jun 27 09:26:21 2023, max compression
```

## Comparing `py-chinese-holidays-1.1.tar` & `py-chinese-holidays-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:32:53.648834 py-chinese-holidays-1.1/
--rw-rw-rw-   0        0        0      374 2023-06-27 07:32:53.647830 py-chinese-holidays-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4629 2023-06-27 05:41:09.000000 py-chinese-holidays-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:32:53.640850 py-chinese-holidays-1.1/chinese_holidays/
--rw-rw-rw-   0        0        0       64 2023-06-27 07:25:27.000000 py-chinese-holidays-1.1/chinese_holidays/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-06-27 02:35:46.000000 py-chinese-holidays-1.1/chinese_holidays/cal_chinese_holidays.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:32:53.645834 py-chinese-holidays-1.1/py_chinese_holidays.egg-info/
--rw-rw-rw-   0        0        0      374 2023-06-27 07:32:52.000000 py-chinese-holidays-1.1/py_chinese_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-06-27 07:32:53.000000 py-chinese-holidays-1.1/py_chinese_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:32:52.000000 py-chinese-holidays-1.1/py_chinese_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 07:32:53.000000 py-chinese-holidays-1.1/py_chinese_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 07:32:53.648834 py-chinese-holidays-1.1/setup.cfg
--rw-rw-rw-   0        0        0      546 2023-06-27 07:30:56.000000 py-chinese-holidays-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:26:21.838232 py-chinese-holidays-1.1.1/
+-rw-rw-rw-   0        0        0      376 2023-06-27 09:26:21.837232 py-chinese-holidays-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4629 2023-06-27 05:41:09.000000 py-chinese-holidays-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 09:26:21.826260 py-chinese-holidays-1.1.1/chinese_holidays/
+-rw-rw-rw-   0        0        0       64 2023-06-27 07:25:27.000000 py-chinese-holidays-1.1.1/chinese_holidays/__init__.py
+-rw-rw-rw-   0        0        0     5027 2023-06-27 09:15:32.000000 py-chinese-holidays-1.1.1/chinese_holidays/cal_chinese_holidays.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:26:21.836235 py-chinese-holidays-1.1.1/py_chinese_holidays.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-27 09:26:21.000000 py-chinese-holidays-1.1.1/py_chinese_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-06-27 09:26:21.000000 py-chinese-holidays-1.1.1/py_chinese_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:26:21.000000 py-chinese-holidays-1.1.1/py_chinese_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 09:26:21.000000 py-chinese-holidays-1.1.1/py_chinese_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:26:21.839230 py-chinese-holidays-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-27 09:26:10.000000 py-chinese-holidays-1.1.1/setup.py
```

### Comparing `py-chinese-holidays-1.1/README.md` & `py-chinese-holidays-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py-chinese-holidays-1.1/chinese_holidays/cal_chinese_holidays.py` & `py-chinese-holidays-1.1.1/chinese_holidays/cal_chinese_holidays.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         day_info['gzYear'] = ele['gzYear']
         day_info['lunarDay'] = ele['lunarDate']
         day_info['lunarMonth'] = ele['lunarMonth']
         day_info['lunarYear'] = ele['lunarYear']
         day_info['lunarDate'] = ele['lunarYear'] + '-' + ele['lunarMonth'] + '-' + ele['lunarDate']
         day_info['lDay'] = ele['lDate']
         day_info['lMonth'] = ele['lMonth']
+        day_info['status'] = ele.get('status', None)
         day_info['generalFestival'] = ele.get('festivalList', None)
         day_info['traditionalFestival'] = None
         day_info['nationalHoliday'] = None
         day_info['isRestDay'] = False
         if 'festivalList' in ele and 'type' in ele:
             if ele['type'] == 't':  # 中国传统节日
                 if 'term' in ele and len(ele['term']) > 0:
```

### Comparing `py-chinese-holidays-1.1/setup.py` & `py-chinese-holidays-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='py-chinese-holidays',
-    version='v1.1',
+    version='v1.1.1',
     description='Calculate Chinese holidays, traditional festivals, and rest days for a specified year.',  # 简要描述
     # py_modules=['chinese_holidays'],
     author='JWDuan',
     author_email='494056012@qq.com',
     url='https://github.com/ymzx/chinese-holidays',
     packages=find_packages(),
     include_package_data=True,
```

