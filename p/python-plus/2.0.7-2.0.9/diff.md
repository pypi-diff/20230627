# Comparing `tmp/python_plus-2.0.7.tar.gz` & `tmp/python_plus-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python_plus-2.0.7.tar", last modified: Tue May  9 17:40:32 2023, max compression
+gzip compressed data, was "dist/python_plus-2.0.9.tar", last modified: Tue Jun 27 19:02:06 2023, max compression
```

## Comparing `python_plus-2.0.7.tar` & `python_plus-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7608 2023-05-09 11:58:50.000000 python_plus-2.0.7/python_plus/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/scripts/vem.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    54303 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/list_requirements.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    68223 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/vem.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/vem.man
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.7/python_plus.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       26 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:40:32.000000 python_plus-2.0.7/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7608 2023-05-09 15:53:59.000000 python_plus-2.0.7/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-05-09 17:40:32.000000 python_plus-2.0.7/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15133 2023-05-09 17:40:32.000000 python_plus-2.0.7/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:02:06.000000 python_plus-2.0.9/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-06-27 18:57:06.000000 python_plus-2.0.9/python_plus/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7608 2023-06-24 06:17:11.000000 python_plus-2.0.9/python_plus/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-06-27 18:57:06.000000 python_plus-2.0.9/python_plus/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.9/python_plus/scripts/vem.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    51482 2023-06-27 18:57:06.000000 python_plus-2.0.9/python_plus/scripts/list_requirements.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    69747 2023-06-27 18:57:06.000000 python_plus-2.0.9/python_plus/scripts/vem.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.9/python_plus/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-06-27 18:57:06.000000 python_plus-2.0.9/python_plus/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.9/python_plus/vem.man
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.9/python_plus.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       26 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-06-27 19:02:06.000000 python_plus-2.0.9/python_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-06-27 19:02:06.000000 python_plus-2.0.9/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7632 2023-06-27 18:57:06.000000 python_plus-2.0.9/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-06-27 19:02:06.000000 python_plus-2.0.9/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5881 2023-06-24 06:17:11.000000 python_plus-2.0.9/README.rst
```

### Comparing `python_plus-2.0.7/python_plus/__main__.py` & `python_plus-2.0.9/python_plus/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os
 import subprocess
 import sys
 
 from zerobug import Z0BUG
 
-__version__ = "2.0.7"
+__version__ = "2.0.9"
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 if __name__ == "__main__":
     action = False
     if len(sys.argv) > 1:
         action = sys.argv[1]
```

### Comparing `python_plus-2.0.7/python_plus/scripts/setup.info` & `python_plus-2.0.9/python_plus/scripts/setup.info`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='python_plus',
-    version='2.0.6',
+    version='2.0.7',
     description='python useful function',
     long_description="""
 Python supplemental features
 ----------------------------
 
 python-plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
```

### Comparing `python_plus-2.0.7/python_plus/scripts/main.py` & `python_plus-2.0.9/python_plus/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.9"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `python_plus-2.0.7/python_plus/scripts/vem.py` & `python_plus-2.0.9/python_plus/scripts/vem.py`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.7/python_plus/scripts/list_requirements.py` & `python_plus-2.0.9/python_plus/scripts/list_requirements.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     import python_plus
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.9"
 python_version = "%s.%s" % (sys.version_info[0], sys.version_info[1])
 
 #
 # known incompatibilities:
 # - requests: oca-maintainers-tools -> '==2.3.0',
 #             codecov -> '>=2.7.9'
 # Here we assume: Odoo 11.0 use python 3.6, Odoo 12.0 -> 3.7, Odoo 16.0 -> 3.8
@@ -49,15 +49,15 @@
         "14.0": "==2.3.1",
         "15.0": "2.4.2"
     },
     "codicefiscale": {"6.1": "==0.9"},
     "coverage": {"2.7": "<5.6.0", "3.5": ">=5.0.0"},
     "cryptography": {"2.7": ">=2.2.2,<3.4", "3.7": ">=38.0,<39.0"},
     "decorator": {"6.1": "==3.4.0", "10.0": "==4.0.10"},
-    "docutils": {"6.1": "==0.12", "0": "==0.14", "3.7": "==0.16"},       # By test pkgs
+    "docutils": {"0": "==0.14", "6.1": "==0.12", "3.7": "==0.16"},       # By test pkgs
     "ebaysdk": {"6.1": "==2.1.4"},
     "email_validator": {"10.0": "<1.3.0", "12.0": ">=1.3"},
     "ERPpeek": {"0": "==1.6.1"},
     "feedparser": {"6.1": "==5.1.3", "10.0": "==5.2.1"},
     "flake8": {
         "6.1": "==3.4.1"     # Tested 3.5.0; 3.6.0 does not work
     },
@@ -187,15 +187,18 @@
     "validate_email": {"6.1": ">=1.3"},
     "vatnumber": {"6.1": "==1.2"},
     "vobject": {"6.1": "==0.6.6", "7.0": "==0.9.3"},  # Tested 0.9.5
     "Werkzeug": {
         "6.1": "==0.9.6",
         "10.0": "==0.11.11",
         "11.0": "==0.11.15",
-        "3.7": "==0.14.1",
+        "12.0": "==0.14.1",
+        "14.0": "==0.16.1",
+        "3.9": "==2.0.2",
+
     },
     "wkhtmltopdf": {"6.1": "==0.12.1", "10.0": "==0.12.4", "12.0": "==0.12.5"},
     "wok_code": {"6.1": "<2.0.6", "10.0": ">=2.0.0"},
     "wsgiref": {"6.1": "==0.1.2"},
     "XlsxWriter": {"6.1": "==0.9.3"},  # Tested 1.0.2
     "xlrd": {"6.1": "==1.0.0"},
     "xlwt": {"6.1": "==0.7.5", "10.0": "==1.1.2", "12.0": "==1.3"},
@@ -262,15 +265,15 @@
     "libssl-dev": "",
     "libxml2-dev": "libxml2-devel",
     "libxslt-dev": "libxslt-devel",
     "zlib1g": "epel-release --enablerepo=extras",
     "zlib1g-dev": "zlib-devel",
 }
 FORCE_ALIAS2 = {
-    "docutils==0.12": "docutils==0.14",
+    # "docutils==0.12": "docutils==0.14",
     "pytz==2014.4": "pytz>=2014.4",
     "pytz==2014.10": "pytz>=2014.10",
     "pytz==2016.7": "pytz>=2016.7",
     "zeep==4.0.0": "zeep==2.4.0",
     "python-ldap": "python-ldap==3.1.0",
     "Mako==1.0.4": "Mako>=1.0.4",
     "rich": "rich<=12.0.0",
@@ -535,146 +538,24 @@
 DEPS3 = {
     "lxml": {
         "bin": ("PY3_DEV", "python3-lxml", "libxml2-dev", "libxslt1-dev", "zlib1g-dev")
     },
     "python-psycopg2": {"bin": ("PY3_DEV", "libpq-dev")},
     "python3-ldap": {"bin": ("libsasl2-dev", "libldap2-dev", "libssl-dev")},
 }
-# DEPS9 = [
-#     "astroid==1.6.5",
-#     "astroid==2.2.0",
-#     "astroid==2.4.2",
-#     "docutils==0.12",
-#     "docutils==0.14",
-#     "docutils==0.16",
-#     "Pillow==3.4.1",
-#     "Pygments==2.0.2",
-#     "six==1.15.0",
-# ]
-
-# PYCODESET = 'utf-8'
-# if PY3:
-#     text_type = unicode = str
-#     bytestr_type = bytes
-# elif PY2:
-#     # unicode exist only for python2
-#     text_type = unicode
-#     bytestr_type = str
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def get_naked_pkgname(pkg):
     return re.split('[!<=>@#;]', python_plus.qsplit(pkg)[0])[0].strip()
 
 
-# def _b(s):
-#     if isinstance(s, text_type):
-#         return s.encode(PYCODESET)
-#     return s
-#
-#
-# def _u(s):
-#     if isinstance(s, bytestr_type):
-#         if PY3:
-#             return s.decode(PYCODESET)
-#         return unicode(s, PYCODESET)
-#     return s
-#
-#
-# def bstrings(src):
-#     if isinstance(src, dict):
-#         src2 = src.copy()
-#         for x in src2.keys():
-#             if isinstance(x, text_type):
-#                 del src[x]
-#             src[_b(x)] = _b(src2[x])
-#     elif isinstance(src, (list, tuple)):
-#         for i, x in enumerate(src):
-#             src[i] = _b(x)
-#     return src
-#
-#
-# def unicodes(src):
-#     if isinstance(src, dict):
-#         src2 = src.copy()
-#         for x in src2.keys():
-#             if isinstance(x, bytestr_type):
-#                 del src[x]
-#             src[_u(x)] = _u(src2[x])
-#     elif isinstance(src, (list, tuple)):
-#         for i, x in enumerate(src):
-#             src[i] = _u(x)
-#     return src
-#
-#
-# def qsplit(*args, **kwargs):
-#     src = args[0]
-#     if len(args) > 1 and args[1]:
-#         sep = args[1]
-#         if isinstance(sep, (tuple, list)):
-#             sep = unicodes(sep)
-#         elif isinstance(sep, basestring):
-#             sep = _u(sep)
-#     else:
-#         sep = [' ', '\t', '\n', '\r']
-#     if len(args) > 2 and args[2]:
-#         maxsplit = args[2]
-#     else:
-#         maxsplit = -1
-#     quotes = kwargs.get('quotes', ["'", '"'])
-#     escape = kwargs.get('escape', False)
-#     enquote = kwargs.get('enquote', False)
-#     strip = kwargs.get('strip', False)
-#     source = _u(src)
-#     sts = False
-#     result = []
-#     item = ''
-#     esc_sts = False
-#     ctr = 0
-#     for ch in source:
-#         if maxsplit >= 0 and ctr >= maxsplit:
-#             item += ch
-#         elif esc_sts:
-#             esc_sts = False
-#             item += ch
-#         elif ch == escape:
-#             esc_sts = True
-#         elif ch == sts:
-#             sts = False
-#             if enquote:
-#                 item += ch
-#         elif sts:
-#             item += ch
-#         elif ch in quotes:
-#             sts = ch
-#             if enquote:
-#                 item += ch
-#         elif (isinstance(sep, (tuple, list)) and ch in sep) or (
-#             isinstance(sep, basestring) and ch == sep
-#         ):
-#             if strip:
-#                 result.append(item.strip())
-#             else:
-#                 result.append(item)
-#             item = ''
-#             ctr += 1
-#         else:
-#             item += ch
-#     if strip:
-#         result.append(item.strip())
-#     else:
-#         result.append(item)
-#     if isinstance(src, bytestr_type):
-#         return bstrings(result)
-#     return result
-
-
 def eval_requirement_cond(line, pyver=None, odoo_ver=None):
     pyver = pyver or '3.7'
     items = line.split('#')[0].split(";")
     if len(items) == 1:
         return get_naked_pkgname(line)
     testenv = {"sys_platform": sys.platform,
                "python_version": pyver,
@@ -747,14 +628,17 @@
                         reqlist.append(re.split('[#;]', line)[0].strip())
     except BaseException as e:
         print("File %s: error %s" % (reqfile, e))
     return reqlist
 
 
 def name_n_version(full_item, with_version=None, odoo_ver=None, pyver=None):
+    def comp_ver(version):
+        return [int(x) for x in version.split(".")]
+
     item = os.path.basename(get_naked_pkgname(re.split("[!=<>]", full_item)[0]))
     if item.endswith(".git"):
         item = item[:-4]
     if not filter(lambda x: item.startswith(x), PIP_WITH_DOT):
         if '.' in item:
             full_item = full_item.replace('.' + item.split(".")[1], '')
             item = item.split(".")[0].lower()
@@ -763,48 +647,46 @@
         full_item = full_item.replace(item, ALIAS[item_l])
         item = ALIAS[item_l]
     if odoo_ver and int(odoo_ver.split('.')[0]) > 10:
         if "openupgradelib" not in item and item in ALIAS3:
             full_item = full_item.replace(item, ALIAS3[item])
             item = ALIAS3[item]
     # if odoo_ver and with_version and not item_ver:
-    if odoo_ver and with_version:
+    if (odoo_ver or pyver) and with_version:
         if item in REQVERSION:
             min_v = False
-            valid_ver = False
-            if pyver in REQVERSION[item]:
-                min_v = pyver
-            elif pyver and pyver.startswith("3"):
-                for v in ("3.9", "3.8", "3.7", "3.6", "3.5"):
-                    if v in REQVERSION[item]:
-                        min_v = v
-                        break
-            if not min_v:
+            if odoo_ver:
                 for v in (
-                    "0",
                     "6.1",
                     "7.0",
                     "8.0",
                     "9.0",
                     "10.0",
                     "11.0",
                     "12.0",
                     "13.0",
                     "14.0",
                     "15.0",
                     "16.0",
                 ):
-                    if v in REQVERSION[item]:
+                    if v in REQVERSION[item] and comp_ver(v) <= comp_ver(odoo_ver):
                         min_v = v
-                        if v == odoo_ver or valid_ver or (not odoo_ver and v == "0"):
-                            break
-                    elif v == odoo_ver:
-                        valid_ver = True
-                        if min_v:
-                            break
+                    if comp_ver(v) >= comp_ver(odoo_ver):
+                        break
+            if pyver and (not min_v or comp_ver(min_v) <= comp_ver("10.0")
+                          and pyver.startswith("3")):
+                for v in ("2.7", "3.5", "3.6", "3.7", "3.8", "3.9"):
+                    if v == "2.7" and odoo_ver and min_v:
+                        continue
+                    if v in REQVERSION[item] and comp_ver(v) <= comp_ver(pyver):
+                        min_v = v
+                    if comp_ver(v) >= comp_ver(pyver):
+                        break
+            if not min_v and "0" in REQVERSION[item]:
+                min_v = "0"
             if min_v:
                 full_item = merge_item_version(
                     full_item,
                     "%s%s" % (item, REQVERSION[item][min_v]),
                     ignore_error=True)
     item = python_plus.qsplit(item)[0].strip()
     full_item = python_plus.qsplit(full_item)[0].strip()
@@ -1117,24 +999,24 @@
     return manifests, reqfiles, setups
 
 
 def swap(deps, itm1, itm2):
     itm1_id = -1
     itm2_id = -1
     for item in deps:
-        if item.startswith(itm1):
+        x = re.search(r"[a-zA-Z0-9_-]+", item)
+        itm0 = item[x.start(): x.end()] if x else item
+        if itm0 == itm1:
             itm1_id = deps.index(item)
-        elif item.startswith(itm2):
+        elif itm0 == itm2:
             itm2_id = deps.index(item)
         if itm1_id >= 0 and itm2_id >= 0:
             break
     if itm1_id < itm2_id:
-        item = deps[itm2_id]
-        del deps[itm2_id]
-        deps.insert(itm1_id, item)
+        deps[itm2_id], deps[itm1_id] = deps[itm2_id], deps[itm1_id]
 
 
 def walk_dir(cdir, manifests, reqfiles, setups, read_from_manifest, recurse):
 
     def parse_manifest(manifests, reqfiles, setups, root, files, no_deep):
         if "/setup/" in root and "setup.py" in files:
             fn = os.path.join(root, "setup.py")
@@ -1387,15 +1269,15 @@
         "--exclude-devel",
         help="Exclude base,rpc,secure and test packages from output list",
         action="store_true",
         dest="exclude_devel",
     )
     parser.add_argument("-V")
     parser.add_argument("-v")
-    parser.add_argument("-y", "--python-version", action="store", dest="pyver")
+    parser.add_argument("-y", "--python", action="store", dest="pyver")
     ctx = parser.parseoptargs(sys.argv[1:], apply_conf=False)
     if ctx["pyver"]:
         global PY3_DEV
         PY3_DEV = "python%s-dev" % ctx["pyver"]
     if ctx["odoo_ver"] and not ctx["pyver"]:
         ctx = get_pyver(ctx)
     if ctx["out_file"]:
@@ -1640,37 +1522,37 @@
                 del deps_list["bin"][ii]
     for ii, dep_pkg in enumerate(deps_list["python"]):
         if ">" in dep_pkg or "<" in dep_pkg or " " in dep_pkg:
             deps_list["python"][ii] = "'%s'" % dep_pkg
     for ii, dep_pkg in enumerate(deps_list["bin"]):
         if ">" in dep_pkg or "<" in dep_pkg or " " in dep_pkg:
             deps_list["bin"][ii] = "'%s'" % dep_pkg
-    for item in DEPS:
-        if "python" in DEPS[item]:
-            if isinstance(DEPS[item]["python"], (tuple, list)):
-                for itm in DEPS[item]["python"]:
-                    swap(deps_list["python"], item, itm)
-            else:
-                swap(deps_list["python"], item, DEPS[item]["python"])
-    if ctx["pyver"] and ctx["pyver"].split(".")[0] == "2":
-        for item in DEPS2:
-            if "python" in DEPS2[item]:
-                if isinstance(DEPS2[item]["python"], (tuple, list)):
-                    for itm in DEPS2[item]["python"]:
-                        swap(deps_list["python"], item, itm)
-                else:
-                    swap(deps_list["python"], item, DEPS2[item]["python"])
-    if ctx["pyver"] and ctx["pyver"].split(".")[0] == "3":
-        for item in DEPS3:
-            if "python" in DEPS3[item]:
-                if isinstance(DEPS3[item]["python"], (tuple, list)):
-                    for itm in DEPS3[item]["python"]:
-                        swap(deps_list["python"], item, itm)
-                else:
-                    swap(deps_list["python"], item, DEPS3[item]["python"])
+    # for item in DEPS:
+    #     if "python" in DEPS[item]:
+    #         if isinstance(DEPS[item]["python"], (tuple, list)):
+    #             for itm in DEPS[item]["python"]:
+    #                 swap(deps_list["python"], item, itm)
+    #         else:
+    #             swap(deps_list["python"], item, DEPS[item]["python"])
+    # if ctx["pyver"] and ctx["pyver"].split(".")[0] == "2":
+    #     for item in DEPS2:
+    #         if "python" in DEPS2[item]:
+    #             if isinstance(DEPS2[item]["python"], (tuple, list)):
+    #                 for itm in DEPS2[item]["python"]:
+    #                     swap(deps_list["python"], item, itm)
+    #             else:
+    #                 swap(deps_list["python"], item, DEPS2[item]["python"])
+    # if ctx["pyver"] and ctx["pyver"].split(".")[0] == "3":
+    #     for item in DEPS3:
+    #         if "python" in DEPS3[item]:
+    #             if isinstance(DEPS3[item]["python"], (tuple, list)):
+    #                 for itm in DEPS3[item]["python"]:
+    #                     swap(deps_list["python"], item, itm)
+    #             else:
+    #                 swap(deps_list["python"], item, DEPS3[item]["python"])
     if ctx["out_file"]:
         req_pkgs = []
         try:
             with open(ctx["opt_fn"], "r") as fd:
                 for pkg in fd.read().split("\n"):
                     if get_naked_pkgname(pkg):
                         req_pkgs.append(pkg)
```

### Comparing `python_plus-2.0.7/python_plus/scripts/vem.sh` & `python_plus-2.0.9/python_plus/scripts/vem.sh`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.9
 
 declare -A PY3_PKGS
 NEEDING_PKGS="configparser future python_plus z0lib"
 # DEVEL_PKGS="click flake8 pycodestyle pylint"
 # SUP_PKGS="future python-plus"
 EI_PKGS="(distribute)"
 BZR_PKGS="(aeroolib)"
@@ -60,14 +60,18 @@
 GIT_PKGS="(openupgradelib|prestapyt)"
 PYBIN_PKGS="(dateutil|ldap|openid)"
 BIN_PKGS="(wkhtmltopdf|lessc)"
 FLT_PKGS="(jwt|FOO)"
 UNISOLATED_PKGS="(.?-|lxml)"
 ERROR_PKGS=""
 LOCAL_PKGS="(clodoo|odoo_score|os0|python_plus|z0bug_odoo|z0lib|zerobug)"
+[[ -d $HOME_DEVEL/../tools ]] && LOCAL_PKGS=$(find $HOME_DEVEL/../tools -maxdepth 1 -type d|grep -Ev "(/|.git|.idea|docs|egg-info|license_text|templates|tools|tests|z0tester)$"|sort|cut -d/ -f7|tr "\n" " ")
+[[ -d $HOME_DEVEL/pypi ]] && LOCAL_PKGS=$(find $HOME_DEVEL/pypi -maxdepth 1 -type d|grep -Ev "(/|.git|.idea|docs|egg-info|license_text|templates|tools|tests|z0tester)$"|sort|cut -d/ -f6|tr "\n" " ")
+LOCAL_PKGS=$(echo $LOCAL_PKGS)
+LOCAL_PKGS=(${LOCAL_PKGS// /|})
 XPKGS_RE=""
 PY3_PKGS[jsonlib]="jsonlib-python3"
 RED="\e[31m"
 CLR="\e[0m"
 
 push_venv() {
     # push_venv(VENV)
@@ -220,39 +224,41 @@
     [[ -n $fn ]] && cmd="$cmd -m $fn"
     [[ $wh =~ debug ]] && echo $cmd -qs "" || $cmd -qs" "
 }
 
 bin_install() {
   # bin_install(pkg)
   [[ $opt_verbose -gt 2 ]] && echo ">>> bin_install($*)"
-  local NPM reqver size x FH DISTO
+  local NPM reqver size x FH DISTO sts=126
   [[ -n $opt_FH ]] && FH=$opt_FH || FH=$(xuname -f)
   local MACHARCH=$(xuname -m)
   [[ -n $opt_distro ]] && DISTO=${opt_distro,,} || DISTO=$(xuname -d)
   [[ -z $opt_distro ]] && DISTO=${DISTO,,}$(xuname -v | grep --color=never -Eo "[0-9]*" | head -n1)
   local pkg=$1
   if [[ -z "$XPKGS_RE" || ! $pkg =~ ($XPKGS_RE) ]]; then
     if [[ $pkg =~ lessc ]]; then
       x=$(which lessc 2>/dev/null)
       if [[ -z $x ]]; then
         x=$(which npm 2>/dev/null)
         if [[ -z "$x" ]]; then
+          sts=125
           echo "Package $pkg require npm software but this software is not installed on your system"
           echo "You should install npm ..."
           [[ $DISTO =~ ^fedora ]] && echo "dnf install npm"
           [[ ! $DISTO =~ ^fedora && $FH == "RHEL" ]] && echo "yum install npm"
           [[ $DISTO =~ ^debian ]] && echo "apt install npm"
           ERROR_PKGS="$ERROR_PKGS   '$pkg'"
         else
           [[ $opt_gbl -ne 0 ]] && NPM="npm -g" || NPM="npm"
           [[ $NPM == "npm" && ! -f package-lock.json ]] && run_traced "$NPM init -y"
           [[ $pkg == "lessc" ]] && pkg="less@3.0.4"
           pkg=${pkg/==/@}
           pkg=$(echo $pkg | tr -d "'")
           run_traced "$NPM install \"$pkg\""
+          sts=$?
           run_traced "$NPM install less-plugin-clean-css"
           x=$(find $($NPM bin) -name lessc 2>/dev/null | head -n1)
         fi
         [[ -n "$x" ]] && run_traced "ln -s $x $VENV/bin" || ERROR_PKGS="$ERROR_PKGS   '$pkg'"
       fi
     elif [[ $pkg =~ wkhtmltopdf ]]; then
       mkdir wkhtmltox.rpm_files
@@ -263,77 +269,87 @@
       [[ $opt_verbose -gt 0 ]] && echo "Download ${wkhtmltopdf_wget}"
       wget -q --timeout=240 ${wkhtmltopdf_wget} -O wkhtmltox${pkgext}
       size=$(stat -c %s wkhtmltox${pkgext})
       if [ $size -eq 0 ]; then
         echo "File wkhtmltox${pkgext} not found!"
       elif [ "$pkgext" == ".rpm" ]; then
         run_traced "rpm2cpio wkhtmltox${pkgext} | cpio -idm"
+        sts=$?
         run_traced "cp ./usr/local/bin/wkhtmltopdf ${VENV}/bin/wkhtmltopdf"
       elif [ "$pkgext" == ".deb" ]; then
         run_traced "dpkg --extract wkhtmltox${pkgext} wkhtmltox.deb_files"
+        sts=$?
         run_traced "cp wkhtmltox.deb_files/usr/local/bin/wkhtmltopdf ${VENV}/bin/wkhtmltopdf"
         run_traced "rm -r wkhtmltox.deb*"
       else
         run_traced "tar -xf wkhtmltox${pkgext}"
+        sts=$?
         run_traced "cp ./wkhtmltox/bin/wkhtmltopdf ${VENV}/bin/wkhtmltopdf"
         run_traced "rm -fr ./wkhtmltox"
       fi
       popd >/dev/null
       rm -fR wkhtmltox.rpm_files
     fi
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
+  return $sts
 }
 
 bin_install_1() {
   # bin_install_1()
   echo -en "\e[?25l"
   [[ $opt_verbose -gt 2 ]] && echo ">>> bin_install_1($*)"
-  local pkg
+  local pkg sts=126
   local binreq bin_re
   [[ -n "$opt_bins" ]] && binreq="${opt_bins//,/ }"
   if [[ -n "$opt_bins" ]]; then
     [[ $opt_verbose -gt 0 ]] && echo -e "(1) Analyzing \e[36m$opt_bins\e[0m"
     for pkg in $binreq; do
       bin_install $pkg
+      ((sts=sts+$?))
     done
   fi
   echo -en "\e[?25h"
+  return $sts
 }
 
 pip_install_wget() {
 # pip_install_wget(fn)
-    local d="" pfn="$1" x
+    local d="" pfn="$1" x sts=126
     pfn="$1"
     [[ $pfn == "python-chart" ]] && d="https://files.pythonhosted.org/packages/22/bf/f37ecd52d9f6ce81d4372956dc52c792de527abfadbf8393dd25deb5c90b/Python-Chart-1.39.tar.gz"
     [[ -z "$d" ]] && echo "Unknown URL for $pfn" && return
     x=$(basename $d)
     run_traced "mkdir -p $VIRTUAL_ENV/tmp"
     run_traced "cd $VIRTUAL_ENV/tmp"
     [[ -f $x ]] && run_traced "rm -f $x"
     run_traced "wget $d"
     run_traced "$PIP install $popts $x"
-    [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+    sts=$?
+    [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+    return $sts
 }
 
 pip_install_git() {
 # pip_install_git(fn)
-    local d="" pfn="$1" x
+    local d="" pfn="$1" x sts=126
     [[ $pfn =~ "future" ]] && d="git+https://github.com/PythonCharmers/python-future.git"
     [[ $pfn =~ "openupgradelib" ]] && d="git+https://github.com/OCA/openupgradelib.git"
     [[ $pfn =~ "prestapyt" ]] && d="git+https://github.com/prestapyt/prestapyt.git@master"
     [[ -z "$d" ]] && echo "Unknown URL for $pfn" && return
     run_traced "$PIP install $d"
-    [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+    sts=$?
+    [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+    return $sts
 }
 
 pip_install() {
   #pip_install(pkg opts)
-  local d pfn pkg popts pypath srcdir tmpdir v vpkg x DISTO FH
+  local d pfn pkg popts pypath srcdir tmpdir v vpkg x DISTO FH sts=126
   [[ $1 =~ ^[\'\"] ]] && pkg="${1:1: -1}" || pkg="$1"
   [[ $opt_verbose -gt 1 ]] && echo -e "  \e[32mpip install \"$1\" $2\e[0m"
   [[ -n $opt_FH ]] && FH=$opt_FH || FH=$(xuname -f)
   [[ -n $opt_distro ]] && DISTO=${opt_distro,,} || DISTO=$(xuname -d)
   pypath=$(find $VIRTUAL_ENV/lib -type d -name "python$opt_pyver")
   [[ -n "$pypath" && -d $pypath/site-packages ]] && pypath=$pypath/site-packages || pypath=$(find $(readlink -f $(dirname $(which $PYTHON 2>/dev/null))/../lib) -type d -name site-packages)
   tmpdir=$VIRTUAL_ENV/tmp
@@ -366,72 +382,80 @@
         [[ -d $opt_oepath/odoo && -f $opt_oepath/odoo/__init__.py ]] && srcdir=$opt_oepath/odoo
       fi
       [[ -z $srcdir && $opt_debug -ge 2 && $pfn =~ $LOCAL_PKGS ]] && echo "Invalid or not found source path $srcdir!" && exit 1
       [[ -z $srcdir && $pfn =~ ^(odoo|openerp)$ ]] && echo "Odoo source not found!" && exit 1
     fi
     if [[ $pfn =~ $BIN_PKGS ]]; then
       bin_install "$pkg"
+      sts=$?
     elif [[ -n "$srcdir" ]]; then
       [[ -d $pypath/$pfn && ! -L $pypath/$pfn ]] && run_traced "rm -fR $pypath/$pfn"
       [[ -L $pypath/$pfn ]] && run_traced "rm -f $pypath/$pfn"
       if [[ $opt_debug -eq 2 ]]; then
         [[ ! -d $tmpdir ]] && run_traced "mkdir $tmpdir"
         run_traced "mkdir -p $tmpdir/$pfn"
         run_traced "cp -r $srcdir $tmpdir/$pfn/"
         run_traced "mv $tmpdir/$pfn/$pfn/setup.py $tmpdir/$pfn/setup.py"
+        [[ -f tmpdir/$pfn/$pfn/README.rst ]] && run_traced "mv tmpdir/$pfn/$pfn/README.rst $tmpdir/$pfn/README.rst"
         x=$(grep -A3 -E "^ *package_data" $tmpdir/$pfn/setup.py|grep --color=never -Eo "\./README.rst")
         # [[ $x == "\./README.rst" ]] && run_traced "mv $tmpdir/$pfn/$pfn/README.rst $tmpdir/$pfn/README.rst"
         run_traced "$PIP install $tmpdir/$pfn $popts"
-        [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+        sts=$?
+        [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
         run_traced "rm -fR $tmpdir/$pfn"
       elif [[ $opt_debug -eq 3 ]]; then
         run_traced "$PIP install \"$srcdir\" $popts"
-        [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+        sts=$?
+        [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
       else
         pushd $srcdir/.. >/dev/null
         [[ $pfn =~ ^(odoo|openerp)$ ]] && x="$opt_oever" || x=$(get_local_version $pfn)
         v=$([[ $(echo $x|grep "mismatch") ]] && echo $x|awk -F/ '{print $2}' || echo $x)
         popd >/dev/null
         x=$(ls -d $pypath/${pfn}-*dist-info 2>/dev/null|grep -E "${pfn}-[0-9.]*dist-info")
         [[ -n $x && $x != $pypath/${pfn}-${v}.dist-info ]] && run_traced "mv $x $pypath/${pfn}-${v}.dist-info"
         if [[ ! -d $pypath/${pfn}-${v}.dist-info ]]; then
           run_traced "mkdir $pypath/${pfn}-${v}.dist-info"
           for d in INSTALLER METADATA RECORD REQUESTED top_level.txt WHEEL; do
             run_traced "touch $pypath/${pfn}-${v}.dist-info/$d"
           done
         fi
         run_traced "ln -s $srcdir $pypath/$pfn"
-        [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+        sts=$?
+        [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
       fi
       # TODO> ?
       # set_hashbang "$pypath/${pfn}"
       [[ -x $VIRTUAL_ENV/bin/${pfn}-info && $opt_verbose -ne 0 ]] && run_traced "$VIRTUAL_ENV/bin/${pfn}-info -v --copy-pkg-data"
       [[ -x $VIRTUAL_ENV/bin/${pfn}-info && $opt_verbose -eq 0 ]] && run_traced "$VIRTUAL_ENV/bin/${pfn}-info --copy-pkg-data"
     elif [[ $pfn =~ $EI_PKGS ]]; then
       run_traced "easy_install install \"$pkg\""
       run_traced "$PIP install $popts --upgrade \"$pkg\""
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     elif [[ $pfn =~ $WGET_PKGS ]]; then
       d=""
       [[ $pfn == "python-chart" ]] && d="https://files.pythonhosted.org/packages/22/bf/f37ecd52d9f6ce81d4372956dc52c792de527abfadbf8393dd25deb5c90b/Python-Chart-1.39.tar.gz"
       [[ -z "$d" ]] && echo "Unknown URL for $pfn" && return
       x=$(basename $d)
       run_traced "mkdir -p $VIRTUAL_ENV/tmp"
       run_traced "cd $VIRTUAL_ENV/tmp"
       [[ -f $x ]] && run_traced "rm -f $x"
       run_traced "wget $d"
       run_traced "$PIP install $popts $x"
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     elif [[ $pfn =~ $GIT_PKGS ]]; then
       d=""
       [[ $pfn =~ "openupgradelib" ]] && d="git+https://github.com/OCA/openupgradelib.git"
       [[ $pfn =~ "prestapyt" ]] && d="git+https://github.com/prestapyt/prestapyt.git@master"
       [[ -z "$d" ]] && echo "Unknown URL for $pfn" && return
       run_traced "$PIP install $d"
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     elif [[ $pfn =~ $BZR_PKGS ]]; then
       x=$(which bzr 2>/dev/null)
       if [[ -z "$x" ]]; then
         echo "Package $pfn require bazar software but this software is not installed on your system"
         echo "You should install bazar ..."
         [[ $DISTO =~ ^fedora ]] && echo "dnf install bzr"
         [[ ! $DISTO =~ ^fedora && $FH == "RHEL" ]] && echo "yum install bzr"
@@ -444,98 +468,110 @@
         run_traced "cd $HOME/bazar"
         run_traced "bzr branch lp:$pkg"
         d=$(find $pfn -name setup.py | head -n1)
         [[ -n "$d" ]] && d=$(dirname $d) || d=""
         if [[ -n "$d" && -d "$d" ]]; then
           run_traced "cd $d"
           run_traced "python ./setup.py install"
-          [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+          sts=$?
+          [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
         else
           echo "Invalid bazar package: file setup.py not found!"
           ERROR_PKGS="$ERROR_PKGS   '$pfn'"
         fi
       fi
     elif [[ $opt_debug -eq 1 ]]; then
       [[ -L $pypath/$pfn ]] && rm -f $pypath/$pfn
       [[ $opt_verbose -lt 2 ]] && x=-1 || x=""
       run_traced "$PIP install $popts --extra-index-url https://testpypi.python.org/pypi \"$vpkg\" $2" "$x"
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     else
       [[ -L $pypath/$pfn ]] && rm -f $pypath/$pfn
       [[ $opt_verbose -lt 2 ]] && x=-1 || x=""
       run_traced "$PIP install $popts \"$vpkg\" $2" "$x"
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     fi
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
+  return $sts
 }
 
 pip_install_1() {
   # pip_install_1(popts)
   echo -en "\e[?25l"
-  local pkg popts ll
+  local pkg popts ll sts=0
   [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
   [[ $opt_verbose -gt 0 ]] && echo -e "(2) Analyzing \e[36m$SECURE_PKGS\e[0m"
   for pkg in $SECURE_PKGS; do
     pip_install "$pkg" "$popts"
+    ((sts=sts+$?))
   done
   if [[ -n $DEVEL_PKGS ]]; then
     [[ $opt_verbose -gt 0 ]] && echo -e "(3) Analyzing \e[36m$DEVEL_PKGS\e[0m"
     for pkg in $DEVEL_PKGS; do
       pip_install "$pkg" "$popts"
+      ((sts=sts+$?))
     done
   elif [[ $opt_verbose -gt 0 ]]; then
     echo -e "\e[1m(3) No DEVEL packages\e[0m"
   fi
   ll=$(get_req_list "" "python" "base")
   if [[ -n $ll ]]; then
     [[ $opt_verbose -gt 0 ]] && echo -e "(4) Analyzing \e[36m$ll\e[0m"
     for pkg in $ll; do
       pip_install "$pkg" "$popts"
+      ((sts=sts+$?))
     done
   elif [[ $opt_verbose -gt 0 ]]; then
     echo -e "\e[1m(4) No BASE packages\e[0m"
   fi
   echo -en "\e[?25h"
+  return $sts
 }
 
 pip_install_2() {
-  # pip_install_2(popts)
+  # pip_install_2()
   echo -en "\e[?25l"
-  local pkg popts
+  local pkg popts sts=0
   [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
   [[ $opt_verbose -gt 0 ]] && echo -e "(5) Analyzing \e[36m$OEPKGS\e[0m"
   for pkg in $OEPKGS; do
     pip_install "$pkg" "$popts"
+    ((sts=sts+$?))
   done
   echo -en "\e[?25h"
+  return $sts
 }
 
 pip_install_req() {
-  # pip_install_req(popts)
+  # pip_install_req()
   echo -en "\e[?25l"
-  local f pfn pkg flist cmd popts
+  local f pfn pkg flist cmd popts sts=0
   [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
   for f in ${opt_rfile//,/ }; do
     pfn=$(readlink -f $f)
     [[ -z "$pfn" ]] && echo "File $f not found!" && continue
     [[ $opt_verbose -gt 0 ]] && echo -e "(6) Analyzing file \e[36m$pfn\e[0m"
     flist=$(get_req_list "$pfn")
     [[ $opt_verbose -gt 2 ]] && echo "<<<$flist>>>$(get_req_list '$pfn' '' 'debug')"
     for pkg in $flist; do
       pip_install "$pkg" "$popts"
+      ((sts=sts+$?))
     done
   done
   echo -en "\e[?25h"
+  return $sts
 }
 
 pip_uninstall() {
   #pip_uninstall(pkg opts)
-  local pkg d x srcdir pfn popts v
+  local pkg d x srcdir pfn popts v sts=0
   local pypath=$VIRTUAL_ENV/lib/python$opt_pyver/site-packages
   pkg=$(get_pkg_wo_version $(get_actual_pkg $1))
   [[ $opt_verbose -eq 0 ]] && popts="$popts -q"
   [[ $opt_yes -ne 0 ]] && popts="$popts -y"
   if [[ -z "$XPKGS_RE" || ! $pkg =~ ($XPKGS_RE) ]]; then
     srcdir=""
     [[ $pkg =~ (python-plus|z0bug-odoo) ]] && pfn=${pkg//-/_} || pfn=$pkg
@@ -549,23 +585,26 @@
       pushd $srcdir/.. >/dev/null
       [[ $pkg =~ ^(odoo|openerp)$ ]] || x=$(get_local_version $pfn)
       v=$([[ $(echo $x|grep "mismatch") ]] && echo $x|awk -F/ '{print $2}' || echo $x)
       popd >/dev/null
       x=$(ls -d $pypath/${pfn}-*dist-info 2>/dev/null|grep -E "${pfn}-[0-9.]*dist-info")
       [[ -n $x && $x != $pypath/${pfn}-${v}.dist-info ]] && run_traced "rm $x"
       run_traced "rm -fR $pypath/${pfn}-${v}.dist-info"
+      sts=$?
       run_traced "rm -f $srcdir"
     else
       [[ -L $pypath/$pkg ]] && rm -f $pypath/$pkg
       run_traced "$PIP uninstall $popts $pkg $2"
-      [[ $? -ne 0 && ! $ERROR_PKGS =~ $pkg ]] && ERROR_PKGS="$ERROR_PKGS   '$pkg'"
+      sts=$?
+      [[ $sts -ne 0 && ! $ERROR_PKGS =~ $pkg ]] && ERROR_PKGS="$ERROR_PKGS   '$pkg'"
     fi
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
+  return $sts
 }
 
 check_bin_package() {
   # check_bin_package(pkg, [show])
   local op reqver xreqver sts curver vpkg x
   local vpkg=$1 mode=$2
 
@@ -955,15 +994,15 @@
     [[ -n "$x" && ! $x =~ ^$VENV ]] && echo "Warning: file $x is outside of virtual env"
   done
 }
 
 do_venv_mgr() {
   # do_venv_mgr {amend|check|cp|mv|merge|test} VENV NEW_VENV
   [[ $opt_verbose -gt 2 ]] && echo ">>> do_venv_mgr($*)"
-  local d f mime VENV V sitecustom x
+  local d f mime VENV V sitecustom x sts=126
   local cmd=$1
   VENV="$2"
   [[ -n "$3" ]] && VENV_TGT=$(readlink -m $3)
   [[ $cmd =~ (amend|check|test|inspect) ]] && VENV_TGT=$VENV
   if [[ -z "$VENV" || -z "$VENV_TGT" ]]; then
     echo "Missed parameters!"
     echo "use: venv_mgr ${CMDS// /|} VENV NEW_VENV"
@@ -997,28 +1036,30 @@
         echo "use: venv_mgr cp -f VENV NEW_VENV"
         exit 1
       fi
       run_traced "rm -fR $VENV_TGT"
     fi
     [[ -d $(dirname $VENV_TGT) ]] || run_traced "mkdir -p $(dirname $VENV_TGT)"
     run_traced "cp -r $VENV $VENV_TGT"
+    sts=$?
     [[ $opt_dry_run -eq 0 ]] && custom_env $VENV_TGT $opt_pyver
     V=$VENV_TGT
     do_activate "$V" "-q"
     find_cur_py
   elif [[ "$cmd" == "merge" ]]; then
     do_deactivate "-q"
     if [[ ! -d $VENV_TGT || ! -d $VENV_TGT/bin || ! -f $VENV_TGT/bin/activate ]]; then
       echo "Invalid destination virtual env $VENV_TGT!"
       exit 1
     fi
     for d in bin include lib lib64 .local; do
       if [ -d "$VENV/$d" ]; then
         [[ $opt_verbose -gt 1 ]] && run_traced "rsync -a $VENV/$d/ $VENV_TGT/$d/"
         [[ $opt_verbose -eq 0 ]] && run_traced "rsync -aq $VENV/$d/ $VENV_TGT/$d/"
+        sts=$?
       fi
     done
     V=$VENV_TGT
     do_activate "$V" "-q"
   else
     if [[ -d $VENV_TGT ]]; then
       echo "Destination virtual env $VENV_TGT already exists!"
@@ -1081,14 +1122,15 @@
           [[ ! :$PATH: =~ :$x: ]] && export PATH=$x:$PATH
         fi
       fi
     fi
     if [[ "$cmd" == "mv" ]]; then
       do_deactivate
       run_traced "mv $VENV $VENV_TGT"
+      sts=$?
       do_activate "$VENV_TGT" "-q"
     fi
   elif [[ $cmd == "inspect" ]]; then
     do_activate "$V"
     set_pybin "" "opt_pyver"
     cmd="vem create $V"
     echo "Virtual Environment name: $V"
@@ -1118,26 +1160,28 @@
       fi
     fi
     echo "Internal sys.path: $PATH"
     echo -e "Environment created with command: \e[1m$cmd\e[0m"
     do_deactivate
   fi
   do_venv_mgr_test $V
+  return $sts
 }
 
 do_venv_create() {
   # do_venv_create VENV
   [[ $opt_verbose -gt 2 ]] && echo ">>> do_venv_create($*)"
-  local f p pkg v VENV xpkgs SAVED_PATH x
+  local f p pkg v VENV xpkgs SAVED_PATH x sts=126
   local venvexe pyexe pypath
   VENV="$1"
   [[ $VENV =~ /$ ]] && VENV="${VENV:0: -1}"
   if [[ -d $VENV ]]; then
     if [[ $opt_force -eq 0 ]]; then
       echo "Warning: virtual environment $VENV already exists!!"
+      sts=125
     else
       for f in bin include lib node_modules share; do
          [[ -d $VENV/$f ]] && run_traced "rm -fR $VENV/$f"
       done
       for f in odoo package-lock.json pyvenv.cfg "=2.0.0"; do
          [[ -f $VENV/$f ]] && run_traced "rm -f $VENV/$f"
       done
@@ -1190,15 +1234,15 @@
     venvexe="$pyexe -m venv"
     [[ $opt_spkg -ne 0 ]] && p="--system-site-packages"
     [[ -d $VENV ]] && p="$p --clear"
     [[ $opt_alone -ne 0 ]] && p="$p --copies"
   fi
   run_traced "$venvexe $p $VENV"
   sts=$?
-  [[ $sts -ne 0 ]] && return
+  [[ $sts -ne 0 ]] && return $sts
   if [[ -d ${VENV}~ ]]; then
       empty=1
       if [[ -z $(find ${VENV}~ -maxdepth 0 -empty) ]]; then
           for f in ${VENV}~/*; do
               b=$(basename $f)
               [[ ! -e $VENV/$b ]] && run_traced "mv $f $VENV/"
               empty=0
@@ -1224,26 +1268,29 @@
     bin_install_1 $VENV
     pip_install_2
   fi
   [[ -n "$opt_rfile" ]] && pip_install_req
   [[ -n "$opt_oepath" && -d $opt_oepath/openerp ]] && pip_install openerp
   [[ -n "$opt_oepath" && -d $opt_oepath/odoo ]] && pip_install odoo
   do_venv_mgr_test $VENV
+  return $sts
 }
 
 do_venv_exec() {
   # do_venv_exec VENV cmd
-  local d f mime VENV V sitecustom
+  local d f mime VENV V sitecustom sts
   VENV="$1"
   run_traced "$2 $3 $4 $5 $6 $7 $8 $9"
+  sts=$?
+  return $sts
 }
 
 do_venv_pip() {
   # do_venv_pip VENV action pkg
-  local d f VENV V popts x
+  local d f VENV V popts x sts=126
   local SAVED_PATH=$PATH
   local cmd="$2"
   VENV="$1"
   pkg=$(get_actual_pkg $3)
   [[ $pkg =~ "-e " ]] && pkg=${pkg//-e /--editable=}
   if [[ $opt_alone -ne 0 && ! $pkg =~ $UNISOLATED_PKGS ]]; then
     V=""
@@ -1251,37 +1298,46 @@
       [[ $d =~ ^$HOME/ || $d =~ ^/(usr/bin) ]] && V="$V:$d"
     done
     PATH=${V:1}
     [[ $opt_verbose -ne 0 ]] && echo "$ PATH=$PATH"
   fi
   if [[ $cmd == "uninstall" ]]; then
     pip_uninstall "$pkg"
+    sts=$?
   else
     [[ $opt_alone -ne 0 && ! $pkg =~ $UNISOLATED_PKGS ]] && popts="--isolated --disable-pip-version-check --no-python-version-warning --no-cache-dir" || popts="--disable-pip-version-check --no-python-version-warning"
     [[ $PIPVER -gt 18 && ! no-warn-conflicts =~ $popts ]] && popts="$popts --no-warn-conflicts"
     [[ $PIPVER -eq 19 && ! 2020-resolver =~ $popts ]] && popts="$popts --use-feature=2020-resolver"
     [[ $PIPVER -eq 21  && ! in-tree-build =~ $popts  ]] && popts="$popts --use-feature=in-tree-build $popts"
     [[ $opt_pyver =~ ^2 && $(uname -r) =~ ^3 ]] && popts="$popts --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org"
     [[ $opt_verbose -lt 2 ]] && popts="$popts -q"
     if [[ $cmd =~ (info|show) ]]; then
       pkg=$(get_pkg_wo_version $pkg)
       if [[ $pkg =~ $BIN_PKGS ]]; then
         check_bin_package "$pkg" "show"
+        sts=$?
       else
         run_traced "$PIP show $pkg"
+        sts=$?
         x=$($PIP show $pkg  2>/dev/null| grep -E ^Location | awk -F: '{print $2}' | sed -e "s| ||")
         [[ -n $x ]] && x=$x/$pkg
         [[ -L $x ]] && echo "Actual location is $(readlink -e $x)"
       fi
     fi
-    [[ $cmd == "install" ]] && pip_install "$pkg"
-    [[ $cmd == "update" ]] && pip_install "$pkg" "--upgrade"
+    if [[ $cmd == "install" ]]; then
+      pip_install "$pkg"
+      sts=$?
+    elif [[ $cmd == "update" ]]; then
+      pip_install "$pkg" "--upgrade"
+      sts=$?
+    fi
   fi
   do_deactivate
   export PATH=$SAVED_PATH
+  return $sts
 }
 
 validate_py_oe_vers() {
   local odoo_majver
   if [[ -n $opt_oever && -z $opt_pyver ]]; then
     odoo_majver=$(echo $opt_oever|cut -d. -f1)
     [[ $odoo_majver -le 10 ]] && opt_pyver=2 || opt_pyver=3
@@ -1425,53 +1481,63 @@
 FLAG=">"
 [[ $opt_dry_run -eq 0 ]] && FLAG="\$"
 [[ -f $TDIR/list_requirements.py ]] && LIST_REQ="$TDIR/list_requirements.py" || LIST_REQ=""
 [[ -z $LIST_REQ ]] && echo "Command list_requirements.py not found!" && exit 1
 chmod -c +x $LIST_REQ
 # LIST_REQ="python $LIST_REQ"    #debug
 
+sts=126
 if [[ $action == "rm" ]]; then
   [[ $PWD == $(readlink -f $p2) ]] && cd
   rm -fR $p2
   [[ -n "${BASH-}" || -n "${ZSH_VERSION-}" ]] && hash -r 2>/dev/null
   unset PYTHON PIP
   exit 0
 elif [[ $action == "create" ]]; then
   [[ -n $opt_oepath ]] && opt_oepath=$(readlink -f $opt_oepath) && venv_mgr_check_oever
+  sts=$?
 elif [[ $action != "help" ]]; then
   do_activate "$p2" "-q"
   venv_mgr_check_src_path "$p2"
   [[ -z $opt_oepath ]] && find_odoo_path "$p2"
   [[ -z $opt_oever ]] && venv_mgr_check_oever
   check_installed_pkgs
   validate_py_oe_vers
   pypi_requrements "$opt_force"
 fi
 
+sts=126
 if [[ "$action" == "help" ]]; then
   man $(dirname $0)/man/man8/$(basename $0).8.gz
+  sts=0
 elif [[ "$action" == "exec" ]]; then
   do_venv_exec "$p2" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
+  sts=$?
   do_deactivate "-q"
 elif [[ "$action" == "python" ]]; then
   do_venv_exec "$p2" "python" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
+  sts=$?
   do_deactivate "-q"
 elif [[ "$action" == "shell" ]]; then
   do_venv_exec "$p2" "$SHELL -i" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
+  sts=$?
   do_deactivate "-q"
 elif [[ $action =~ (info|install|show|uninstall|update) ]]; then
   [[ $opt_cc -ne 0 && -d $HOME/.cache/pip ]] && run_traced "rm -fR $HOME/.cache/pip"
   do_venv_pip "$p2" "$action" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
+  sts=$?
   do_deactivate "-q"
 elif [[ "$action" == "create" ]]; then
   [[ $opt_cc -ne 0 && -d $HOME/.cache/pip ]] && run_traced "rm -fR $HOME/.cache/pip"
   do_venv_create "$p2" "$p3" "$p4" "$p5" "$p6"
+  sts=$?
   do_deactivate "-q"
 else
   do_venv_mgr "$action" "$p2" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
+  sts=$?
 fi
 PYTHONPATH=$SAVED_PYTHONPATH
 [[ $opt_verbose -gt 3 ]] && set +x
 if [[ -n "$ERROR_PKGS" ]]; then
   echo "************************************************************"
   echo -e "\e[1mWarning! Following packages with wrong version or uninstalled\e[0m"
   echo "$ERROR_PKGS"
@@ -1519,8 +1585,8 @@
   if [[ $ERROR_PKGS =~ psycopg2 ]]; then
     PKGLIST=""
     [[ $FH == "RHEL" ]] && PKGLIST="$PKGLIST postgresql-devel" || PKGLIST="$PKGLIST libpq-dev"
     echo "$XTAL install $PKGLIST    # psycopg2-binary / psycopg2"
   fi
 fi
 unset PYTHON PIP
-exit 0
+exit $sts
```

### Comparing `python_plus-2.0.7/python_plus/__init__.py` & `python_plus-2.0.9/python_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __author__ = 'Antonio Maria Vigliotti'
 __license__ = 'L-GPL'
 __copyright__ = 'Copyright 2018-2023 SHS-AV srl'
 __ver_major__ = 0
 __ver_minor__ = 1
 __ver_patch__ = 3
 __ver_sub__ = '6'
-__version__ = '2.0.7'
+__version__ = '2.0.9'
 
 PYCODESET = 'utf-8'
 if PY3:
     text_type = unicode = str
     bytestr_type = bytes
 elif PY2:
     # unicode exist only for python2
```

### Comparing `python_plus-2.0.7/python_plus/vem.man` & `python_plus-2.0.9/python_plus/vem.man`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.7/python_plus.egg-info/SOURCES.txt` & `python_plus-2.0.9/python_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.7/python_plus.egg-info/PKG-INFO` & `python_plus-2.0.9/python_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-plus
-Version: 2.0.7
+Version: 2.0.9
 Summary: python useful function
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `python_plus-2.0.7/setup.py` & `python_plus-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 setup(
     name='python_plus',
-    version='2.0.7',
+    version='2.0.9',
     description='python useful function',
     long_description="""
 Python supplemental features
 ----------------------------
 
 python-plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
```

### Comparing `python_plus-2.0.7/PKG-INFO` & `python_plus-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python_plus
-Version: 2.0.7
+Version: 2.0.9
 Summary: python useful function
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

