# Comparing `tmp/jax-tools-1.0.47.tar.gz` & `tmp/jax-tools-1.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.47.tar", last modified: Tue Jun  6 03:59:01 2023, max compression
+gzip compressed data, was "jax-tools-1.0.61.tar", last modified: Tue Jun 27 07:13:39 2023, max compression
```

## Comparing `jax-tools-1.0.47.tar` & `jax-tools-1.0.61.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.905187 jax-tools-1.0.47/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-06 03:59:01.904931 jax-tools-1.0.47/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.47/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.872582 jax-tools-1.0.47/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.47/jax_tools/__init__.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.884536 jax-tools-1.0.47/jax_tools/cmd/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.47/jax_tools/cmd/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.47/jax_tools/cmd/jax.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.47/jax_tools/cmd/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.47/jax_tools/cmd/jax_fix.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.47/jax_tools/cmd/jax_nd.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1724 2023-06-06 03:38:17.000000 jax-tools-1.0.47/jax_tools/cmd/jax_pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.47/jax_tools/cmd/nd.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.902804 jax-tools-1.0.47/jax_tools/cmd_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.47/jax_tools/cmd_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4526 2023-06-06 03:38:17.000000 jax-tools-1.0.47/jax_tools/cmd_tools/pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6223 2023-06-06 03:32:23.000000 jax-tools-1.0.47/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.47/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.47/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.47/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.47/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2772 2023-06-06 03:34:47.000000 jax-tools-1.0.47/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.904528 jax-tools-1.0.47/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.47/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.47/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.877754 jax-tools-1.0.47/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      657 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      224 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       83 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-06 03:59:01.905273 jax-tools-1.0.47/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1963 2023-06-06 03:59:01.000000 jax-tools-1.0.47/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.747789 jax-tools-1.0.61/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-27 07:13:39.747499 jax-tools-1.0.61/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.61/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.711933 jax-tools-1.0.61/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.61/jax_tools/__init__.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.725444 jax-tools-1.0.61/jax_tools/cmd/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.61/jax_tools/cmd/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.61/jax_tools/cmd/jax.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.61/jax_tools/cmd/jax_encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.61/jax_tools/cmd/jax_fix.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.61/jax_tools/cmd/jax_nd.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1737 2023-06-21 02:57:30.000000 jax-tools-1.0.61/jax_tools/cmd/jax_pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.61/jax_tools/cmd/nd.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.727907 jax-tools-1.0.61/jax_tools/cmd_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.61/jax_tools/cmd_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     8063 2023-06-25 00:48:51.000000 jax-tools-1.0.61/jax_tools/cmd_tools/pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     6271 2023-06-27 02:06:15.000000 jax-tools-1.0.61/jax_tools/colorful_font.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.61/jax_tools/encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.61/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.61/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.61/jax_tools/proxies.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2772 2023-06-06 03:34:47.000000 jax-tools-1.0.61/jax_tools/ssh.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.746594 jax-tools-1.0.61/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.61/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.61/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-27 07:13:39.716149 jax-tools-1.0.61/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      657 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      224 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       83 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-27 07:13:39.000000 jax-tools-1.0.61/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-27 07:13:39.747896 jax-tools-1.0.61/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1963 2023-06-27 07:13:39.000000 jax-tools-1.0.61/setup.py
```

### Comparing `jax-tools-1.0.47/PKG-INFO` & `jax-tools-1.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.47
+Version: 1.0.61
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.47/README.md` & `jax-tools-1.0.61/README.md`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/cmd/jax_encrypt.py` & `jax-tools-1.0.61/jax_tools/cmd/jax_encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/cmd/jax_fix.py` & `jax-tools-1.0.61/jax_tools/cmd/jax_fix.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/cmd/jax_pam.py` & `jax-tools-1.0.61/jax_tools/cmd/jax_pam.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,20 +41,20 @@
         elif arg_1 in add_sign_list:
             name = input(u'请输入您的要新建的账号名称(如:jenkins web root account)：')
             username = input(u'请输入你的登录用户名: ')
             password = getpass.getpass(u'请输入你的登录密码或验证token: ')
             pm.add_account(name, username, password)
         elif arg_1 in delete_sign_list:
             if len(sys.argv) > 2:
-                name = sys.argv[2]
+                name = '' .join(sys.argv[2:])
                 pm.delete_account(name)
             else:
                 name = input(u'请输入您想要删除的账号名称：')
                 pm.delete_account(name)
         else:
-            pm.get_password(sys.argv[1])
+            pm().get_password(sys.argv[1])
     except IndexError:
         print_help()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `jax-tools-1.0.47/jax_tools/colorful_font.py` & `jax-tools-1.0.61/jax_tools/colorful_font.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Colorful Log Process
 """
 import time
 
 
-class ColorFont(object):
+class ColorfulFont(object):
     """
     Colored Font
     """
     STYLE_NORMAL = 0
     STYLE_BOLD = 1
     STYLE_UNDERLINE = 4
     STYLE_INVERSE = 7
@@ -109,54 +109,54 @@
 
         Returns:
             str: Colorful text.
         """
         return '\033[{0};33;{1}m{2}\033[0m'.format(style, color, msg)
 
 
-class Cyanic(ColorFont):
+class Cyanic(ColorfulFont):
     """
     Cyanic colored font
     """
-    color_num = ColorFont.COLOR_CYANIC
+    color_num = ColorfulFont.COLOR_CYANIC
 
 
-class Red(ColorFont):
+class Red(ColorfulFont):
     """
     Red colored font
     """
-    color_num = ColorFont.COLOR_RED
+    color_num = ColorfulFont.COLOR_RED
 
 
-class Green(ColorFont):
+class Green(ColorfulFont):
     """
     Green colored font
     """
-    color_num = ColorFont.COLOR_GREEN
+    color_num = ColorfulFont.COLOR_GREEN
 
 
-class Yellow(ColorFont):
+class Yellow(ColorfulFont):
     """
     Yellow Colored font
     """
-    color_num = ColorFont.COLOR_YELLOW
+    color_num = ColorfulFont.COLOR_YELLOW
 
 
-class Fuchsia(ColorFont):
+class Fuchsia(ColorfulFont):
     """
     Fuchsia Colored Font
     """
-    color_num = ColorFont.COLOR_FUCHSIA
+    color_num = ColorfulFont.COLOR_FUCHSIA
 
 
-class Normal(ColorFont):
+class Normal(ColorfulFont):
     """
     Normal Colored Font
     """
-    color_num = ColorFont.COLOR_NORMAL
+    color_num = ColorfulFont.COLOR_NORMAL
 
 
 def bold_msg(color, msg):
     """
     Return a bold colorful message.
 
     Args:
@@ -166,15 +166,15 @@
     Returns:
         str: The formatted message with bold and color.
 
     """
     return '\033[1;36;{0}m{1}\033[0m'.format(color, msg)
 
 
-class GetColor(ColorFont):
+class GetColor(ColorfulFont):
     """
     Get Font Color
     """
 
     @classmethod
     def score(cls, s):
         """
@@ -228,15 +228,15 @@
         return response
 
 
 if __name__ == '__main__':
     print(Red.underline('Cyanic'))
     print(Yellow.bold('Red'))
     print(GetColor.score(9.5))
-    print(ColorFont.colorful_text(ColorFont.STYLE_NORMAL, GetColor.score(6.5), '6.5 score'))
+    print(ColorfulFont.colorful_text(ColorfulFont.STYLE_NORMAL, GetColor.score(6.5), '6.5 score'))
     print(bold_msg(GetColor.score(2.5), '2.5 score'))
     print(bold_msg(GetColor.date('2020-01-01'), '2020-01-01'))
     print(bold_msg(GetColor.date('2023-01-01'), '2023-01-01'))
     print(bold_msg(GetColor.date('2019-01-01'), '2019-01-01'))
     print(Yellow('hello'))
     print(Yellow.text('hello'))
     print(Red.bold('hello'))
```

### Comparing `jax-tools-1.0.47/jax_tools/encrypt.py` & `jax-tools-1.0.61/jax_tools/encrypt.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/logger.py` & `jax-tools-1.0.61/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/network_test.py` & `jax-tools-1.0.61/jax_tools/network_test.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/proxies.py` & `jax-tools-1.0.61/jax_tools/proxies.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools/ssh.py` & `jax-tools-1.0.61/jax_tools/ssh.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/jax_tools.egg-info/PKG-INFO` & `jax-tools-1.0.61/jax_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.47
+Version: 1.0.61
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.47/jax_tools.egg-info/SOURCES.txt` & `jax-tools-1.0.61/jax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.47/setup.py` & `jax-tools-1.0.61/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.47",
+    version="1.0.61",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
     description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
     long_description=read_file('README.md'),
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
```

