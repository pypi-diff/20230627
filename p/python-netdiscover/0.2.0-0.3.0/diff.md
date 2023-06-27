# Comparing `tmp/python-netdiscover-0.2.0.tar.gz` & `tmp/python-netdiscover-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-netdiscover-0.2.0.tar", last modified: Wed May 15 10:03:22 2019, max compression
+gzip compressed data, was "python-netdiscover-0.3.0.tar", last modified: Tue Jun 27 08:05:58 2023, max compression
```

## Comparing `python-netdiscover-0.2.0.tar` & `python-netdiscover-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,35 @@
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/netdiscover/
--rw-r--r--   0 cirne     (1000) cirne     (1000)      187 2019-05-15 09:38:40.000000 python-netdiscover-0.2.0/netdiscover/__init__.py
--rw-r--r--   0 cirne     (1000) cirne     (1000)     4663 2019-05-15 10:02:41.000000 python-netdiscover-0.2.0/netdiscover/netdiscover.py
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/
--rw-r--r--   0 cirne     (1000) cirne     (1000)        1 2019-05-14 15:16:56.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/not-zip-safe
--rw-r--r--   0 cirne     (1000) cirne     (1000)     3562 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/PKG-INFO
--rw-r--r--   0 cirne     (1000) cirne     (1000)     1013 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/SOURCES.txt
--rw-r--r--   0 cirne     (1000) cirne     (1000)       12 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/top_level.txt
--rw-r--r--   0 cirne     (1000) cirne     (1000)        1 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/python_netdiscover.egg-info/dependency_links.txt
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/tests/
--rw-r--r--   0 cirne     (1000) cirne     (1000)       66 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/tests/__init__.py
--rw-r--r--   0 cirne     (1000) cirne     (1000)      431 2019-05-14 08:57:06.000000 python-netdiscover-0.2.0/tests/test_netdiscover.py
--rw-r--r--   0 cirne     (1000) cirne     (1000)      394 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/setup.cfg
--rw-r--r--   0 cirne     (1000) cirne     (1000)      290 2019-05-15 09:36:25.000000 python-netdiscover-0.2.0/HISTORY.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)     1892 2019-05-14 15:43:24.000000 python-netdiscover-0.2.0/README.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)     3562 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/PKG-INFO
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/docs/
--rw-r--r--   0 cirne     (1000) cirne     (1000)      315 2019-05-14 15:08:22.000000 python-netdiscover-0.2.0/docs/index.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      773 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/docs/make.bat
--rw-r--r--   0 cirne     (1000) cirne     (1000)     1230 2019-05-14 11:27:41.000000 python-netdiscover-0.2.0/docs/installation.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      850 2019-05-14 11:38:48.000000 python-netdiscover-0.2.0/docs/readme.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      344 2019-05-15 09:31:23.000000 python-netdiscover-0.2.0/docs/netdiscover.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)       70 2019-05-14 15:05:29.000000 python-netdiscover-0.2.0/docs/modules.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)       28 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/docs/authors.rst
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/docs/_build/
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/docs/_build/html/
-drwxr-xr-x   0 cirne     (1000) cirne     (1000)        0 2019-05-15 10:03:22.000000 python-netdiscover-0.2.0/docs/_build/html/_static/
--rw-r--r--   0 cirne     (1000) cirne     (1000)      202 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/down.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      829 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      214 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      222 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      673 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 cirne     (1000) cirne     (1000)       90 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      756 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)       90 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      286 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/file.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      203 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/up.png
--rw-r--r--   0 cirne     (1000) cirne     (1000)      641 2019-05-14 11:35:26.000000 python-netdiscover-0.2.0/docs/_build/html/_static/comment.png
--rwxr-xr-x   0 cirne     (1000) cirne     (1000)     4889 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/docs/conf.py
--rw-r--r--   0 cirne     (1000) cirne     (1000)      242 2019-05-14 11:44:59.000000 python-netdiscover-0.2.0/docs/usage.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      619 2019-05-14 11:25:57.000000 python-netdiscover-0.2.0/docs/Makefile
--rw-r--r--   0 cirne     (1000) cirne     (1000)       33 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/docs/contributing.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)       28 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/docs/history.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)     1693 2019-05-15 09:38:40.000000 python-netdiscover-0.2.0/setup.py
--rw-r--r--   0 cirne     (1000) cirne     (1000)     3614 2019-05-14 11:36:50.000000 python-netdiscover-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      155 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/AUTHORS.rst
--rw-r--r--   0 cirne     (1000) cirne     (1000)      262 2019-05-14 08:35:49.000000 python-netdiscover-0.2.0/MANIFEST.in
--rw-r--r--   0 cirne     (1000) cirne     (1000)    35149 2019-05-14 08:52:30.000000 python-netdiscover-0.2.0/LICENSE
+drwxr-xr-x   0 acirne    (1000) acirne    (1000)        0 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      155 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/AUTHORS.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     3614 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      273 2023-06-27 08:00:49.000000 python-netdiscover-0.3.0/HISTORY.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)    35149 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/LICENSE
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      262 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/MANIFEST.in
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     3338 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/PKG-INFO
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     2171 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/README.rst
+drwxr-xr-x   0 acirne    (1000) acirne    (1000)        0 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/docs/
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      619 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/Makefile
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       28 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 acirne    (1000) acirne    (1000)     4889 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/conf.py
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       33 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/contributing.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       28 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/history.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      315 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/index.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     1230 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/installation.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      773 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/make.bat
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       70 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/modules.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      344 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/netdiscover.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      850 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/readme.rst
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      242 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/docs/usage.rst
+drwxr-xr-x   0 acirne    (1000) acirne    (1000)        0 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/netdiscover/
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      187 2023-06-27 08:00:55.000000 python-netdiscover-0.3.0/netdiscover/__init__.py
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     5335 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/netdiscover/netdiscover.py
+drwxr-xr-x   0 acirne    (1000) acirne    (1000)        0 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/python_netdiscover.egg-info/
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     3338 2023-06-27 08:05:58.000000 python-netdiscover-0.3.0/python_netdiscover.egg-info/PKG-INFO
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      597 2023-06-27 08:05:58.000000 python-netdiscover-0.3.0/python_netdiscover.egg-info/SOURCES.txt
+-rw-r--r--   0 acirne    (1000) acirne    (1000)        1 2023-06-27 08:05:58.000000 python-netdiscover-0.3.0/python_netdiscover.egg-info/dependency_links.txt
+-rw-r--r--   0 acirne    (1000) acirne    (1000)        1 2023-06-27 08:05:58.000000 python-netdiscover-0.3.0/python_netdiscover.egg-info/not-zip-safe
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       12 2023-06-27 08:05:58.000000 python-netdiscover-0.3.0/python_netdiscover.egg-info/top_level.txt
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      394 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/setup.cfg
+-rw-r--r--   0 acirne    (1000) acirne    (1000)     1693 2023-06-27 08:01:03.000000 python-netdiscover-0.3.0/setup.py
+drwxr-xr-x   0 acirne    (1000) acirne    (1000)        0 2023-06-27 08:05:58.799775 python-netdiscover-0.3.0/tests/
+-rw-r--r--   0 acirne    (1000) acirne    (1000)       66 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/tests/__init__.py
+-rw-r--r--   0 acirne    (1000) acirne    (1000)      431 2023-06-27 07:58:52.000000 python-netdiscover-0.3.0/tests/test_netdiscover.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-netdiscover-0.2.0/netdiscover/netdiscover.py` & `python-netdiscover-0.3.0/netdiscover/netdiscover.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import sys
 import shlex
-
+import re
 
 class Discover:
 
     def __init__(self, netdiscover_path=None, root_verify=True):
         """
         :param netdiscover_path: Path where is the netdiscover binary. If not defined it will search on defaults netdiscover locations
         :param root_verify: Verify if the user is root
@@ -54,27 +54,28 @@
     def get_command(self):
         """
         :return: Commad used to scan the network
         """
         return self.command
 
     def scan(self, interface=None, ip_range=None, file=None, passive=False, filter_p=None, sleep=None, node=None,
-             count=None, fast=None, sleep_supression=None):
+             count=None, fast=None, sleep_supression=None, output=["ip","mac"]):
         """
         :param interface: Your network device
         :param ip_range: Scan a given range instead of auto scan. 192.168.6.0/24,/16,/8
         :param file: Scan the list of ranges contained into the given file
         :param passive:  Do not send anything, only sniff
         :param macs: File with the list of known MACs and host names
         :param filter_p: Customize pcap filter expression (default: "arp")
         :param sleep: Time to sleep between each arp request (miliseconds)
         :param node: Last ip octet used for scanning (from 2 to 253)
         :param count: Number of times to send each arp reques (for nets with packet loss)
         :param fast: Enable fastmode scan, saves a lot of time, recommended for auto
         :param sleep_supression:  Enable sleep time supression betwen each request (hardcore mode)
+        :param output: List of elements that should be part of the output, by default thats ip and mac.
 
         :return: List with the result of the scan
         """
         self.command = 'netdiscover -P -N'
 
         if interface:
             self.command += " -i %s" % interface
@@ -106,32 +107,41 @@
         if fast:
             self.command += ' -f'
 
         if sleep_supression:
             self.command += ' -S'
 
         self._raw_result = subprocess.check_output(shlex.split(self.command))
-        self._scan_result = self.parse_output(self._raw_result)
+        self._scan_result = self.parse_output(self._raw_result, output)
 
         return self._scan_result
 
     @staticmethod
-    def parse_output(out):
+    def parse_output(data, output):
         """
 
-        :param out: Raw output to parse
-        :return: List with the results from the scan. Each result is represented by a dictionary with two keys, 'ip' and 'mac'.
+        :param data: Raw output to parse
+        :param output: List of elements that should be part of the output.
+        :return: List with the results from the scan. Each result is represented by a dictionary.
         """
-        content = out.split(b"\n")
-        content = content[:-3]
+
+        # decode and split raw output
+        content = data.decode("UTF-8").split("\n")
+
+        # sanitize user coices for output
+        output = [key for key in output if key in ("ip","mac","count","len","vendor")]
 
         results = []
 
         if len(content) != 0:
-            for i in content:
-                pars = i.split()
-                results.append({
-                    'ip': pars[0],
-                    'mac': pars[1]
-                })
+            for chunk in content:
+                pars = re.search(r"\s?(?P<ip>\d+\.\d+\.\d+\.\d+)"
+                                 r"\s+(?P<mac>[a-fA-F0-9:]{17})"
+                                 r"\s+(?P<count>\d+)"
+                                 r"\s+(?P<len>\d+)"
+                                 r"\s+(?P<vendor>.*)",
+                                 chunk)
+                if pars:
+                    pars = pars.groupdict()
+                    results.append({key: pars[key] for key in output})
 
         return results
```

### Comparing `python-netdiscover-0.2.0/python_netdiscover.egg-info/PKG-INFO` & `python-netdiscover-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-netdiscover
-Version: 0.2.0
+Version: 0.3.0
 Summary: python-netdiscover is a simple wrapper for the netdiscover reconnaissance tool
 Home-page: https://github.com/MrSuicideParrot/python-netdiscover
 Author: André Cirne
 Author-email: ancirne@gmail.com
 License: GNU General Public License v3
-Description: ==================
-        python-netdiscover
-        ==================
-        
-        .. image:: https://img.shields.io/pypi/v/python-netdiscover.svg
-                :target: https://pypi.python.org/pypi/python-netdiscover
-        
-        .. image:: https://img.shields.io/pypi/pyversions/python-netdiscover.svg
-                :target: https://pypi.python.org/pypi/python-netdiscover
-        
-        The  python-netdiscover is a simple wrapper for the `netdiscover reconnaissance tool <https://sourceforge.net/projects/netdiscover/>`_.
-        
-        This library offers a simple way to create scans from a python script and analyse the results.
-        
-        
-        * Documentation: https://python-netdiscover.readthedocs.io
-        * GitHub: https://github.com/MrSuicideParrot/python-netdiscover
-        * PyPI: https://pypi.org/project/python-netdiscover/
-        
-        Installation
-        ============
-        From the shell, uncompress python-netdiscover.tar.gz and then run make :
-        
-        .. code-block:: bash
-        
-            $ tar xvzf python-netdiscover.tar.gz
-            $ cd python-netdiscover
-            $ python setup.py install
-        
-        or using Pip
-        
-        .. code-block:: bash
-        
-            $ pip install python-netdiscover
-        
-        
-        Usage
-        =====
-        From python/ipython:
-        --------------------
-        
-        .. code-block:: python
-        
-            >>> from netdiscover import *
-            >>> disc = Discover()
-            >>> disc.scan(ip_range="192.168.1.0/24")
-            [{'mac': b'73:8b:10:0e:bd:23', 'ip': b'192.168.1.1'}, {'mac': b'f4:3c:4a:73:47:07', 'ip': b'192.168.1.2'}]
-        
-        
-        Notes
-        =====
-        This tool needs to be run as root. It is necessary to be presented on the system the *netdiscover* tool. The library will look for the *netdiscovery* binary in the following paths:
-        
-        *  netdiscover
-        * /usr/bin/netdiscover
-        * /usr/sbin/netdiscover
-        * /usr/local/bin/netdiscover
-        * /sw/bin/netdiscover
-        * /opt/local/bin/netdiscover
-        
-        If *netdiscovery* is not present in any of the paths above, you can specifie path with the argument *netdiscover_path* on Discover class.
-        
-        .. code-block:: python
-        
-            disc = Discover(netdiscover_path="path_of_netdiscover")
-        
 Keywords: network,netdiscover,arpscanner,sysadmin
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -85,7 +18,77 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==================
+python-netdiscover
+==================
+
+.. image:: https://img.shields.io/pypi/v/python-netdiscover.svg
+        :target: https://pypi.python.org/pypi/python-netdiscover
+
+.. image:: https://img.shields.io/pypi/pyversions/python-netdiscover.svg
+        :target: https://pypi.python.org/pypi/python-netdiscover
+
+The  python-netdiscover is a simple wrapper for the `netdiscover reconnaissance tool <https://sourceforge.net/projects/netdiscover/>`_.
+
+This library offers a simple way to create scans from a python script and analyse the results.
+
+
+* Documentation: https://python-netdiscover.readthedocs.io
+* GitHub: https://github.com/MrSuicideParrot/python-netdiscover
+* PyPI: https://pypi.org/project/python-netdiscover/
+
+Installation
+============
+First, you will need to install the `netdiscover binary <https://sourceforge.net/projects/netdiscover/>`_ on your system, this may depend on your operating system. Many distributions have this tool available in `their main repository <https://pkgs.org/download/netdiscover>`_. 
+
+From the shell, uncompress python-netdiscover.tar.gz and then run make :
+
+.. code-block:: bash
+
+    $ tar xvzf python-netdiscover.tar.gz
+    $ cd python-netdiscover
+    $ python setup.py install
+
+or using Pip
+
+.. code-block:: bash
+
+    $ pip install python-netdiscover
+
+
+Usage
+=====
+From python/ipython:
+--------------------
+
+.. code-block:: python
+
+    >>> from netdiscover import *
+    >>> disc = Discover()
+    >>> disc.scan(ip_range="192.168.1.0/24")
+    [{'mac': b'73:8b:10:0e:bd:23', 'ip': b'192.168.1.1'}, {'mac': b'f4:3c:4a:73:47:07', 'ip': b'192.168.1.2'}]
+
+
+Notes
+=====
+This tool needs to be run as root. It is necessary to be presented on the system the *netdiscover* tool. The library will look for the *netdiscovery* binary in the following paths:
+
+*  netdiscover
+* /usr/bin/netdiscover
+* /usr/sbin/netdiscover
+* /usr/local/bin/netdiscover
+* /sw/bin/netdiscover
+* /opt/local/bin/netdiscover
+
+If *netdiscovery* is not present in any of the paths above, you can specifie path with the argument *netdiscover_path* on Discover class.
+
+.. code-block:: python
+
+    disc = Discover(netdiscover_path="path_of_netdiscover")
```

### Comparing `python-netdiscover-0.2.0/README.rst` & `python-netdiscover-0.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 * Documentation: https://python-netdiscover.readthedocs.io
 * GitHub: https://github.com/MrSuicideParrot/python-netdiscover
 * PyPI: https://pypi.org/project/python-netdiscover/
 
 Installation
 ============
+First, you will need to install the `netdiscover binary <https://sourceforge.net/projects/netdiscover/>`_ on your system, this may depend on your operating system. Many distributions have this tool available in `their main repository <https://pkgs.org/download/netdiscover>`_. 
+
 From the shell, uncompress python-netdiscover.tar.gz and then run make :
 
 .. code-block:: bash
 
     $ tar xvzf python-netdiscover.tar.gz
     $ cd python-netdiscover
     $ python setup.py install
```

### Comparing `python-netdiscover-0.2.0/PKG-INFO` & `python-netdiscover-0.3.0/python_netdiscover.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: python-netdiscover
-Version: 0.2.0
+Version: 0.3.0
 Summary: python-netdiscover is a simple wrapper for the netdiscover reconnaissance tool
 Home-page: https://github.com/MrSuicideParrot/python-netdiscover
 Author: André Cirne
 Author-email: ancirne@gmail.com
 License: GNU General Public License v3
-Description: ==================
-        python-netdiscover
-        ==================
-        
-        .. image:: https://img.shields.io/pypi/v/python-netdiscover.svg
-                :target: https://pypi.python.org/pypi/python-netdiscover
-        
-        .. image:: https://img.shields.io/pypi/pyversions/python-netdiscover.svg
-                :target: https://pypi.python.org/pypi/python-netdiscover
-        
-        The  python-netdiscover is a simple wrapper for the `netdiscover reconnaissance tool <https://sourceforge.net/projects/netdiscover/>`_.
-        
-        This library offers a simple way to create scans from a python script and analyse the results.
-        
-        
-        * Documentation: https://python-netdiscover.readthedocs.io
-        * GitHub: https://github.com/MrSuicideParrot/python-netdiscover
-        * PyPI: https://pypi.org/project/python-netdiscover/
-        
-        Installation
-        ============
-        From the shell, uncompress python-netdiscover.tar.gz and then run make :
-        
-        .. code-block:: bash
-        
-            $ tar xvzf python-netdiscover.tar.gz
-            $ cd python-netdiscover
-            $ python setup.py install
-        
-        or using Pip
-        
-        .. code-block:: bash
-        
-            $ pip install python-netdiscover
-        
-        
-        Usage
-        =====
-        From python/ipython:
-        --------------------
-        
-        .. code-block:: python
-        
-            >>> from netdiscover import *
-            >>> disc = Discover()
-            >>> disc.scan(ip_range="192.168.1.0/24")
-            [{'mac': b'73:8b:10:0e:bd:23', 'ip': b'192.168.1.1'}, {'mac': b'f4:3c:4a:73:47:07', 'ip': b'192.168.1.2'}]
-        
-        
-        Notes
-        =====
-        This tool needs to be run as root. It is necessary to be presented on the system the *netdiscover* tool. The library will look for the *netdiscovery* binary in the following paths:
-        
-        *  netdiscover
-        * /usr/bin/netdiscover
-        * /usr/sbin/netdiscover
-        * /usr/local/bin/netdiscover
-        * /sw/bin/netdiscover
-        * /opt/local/bin/netdiscover
-        
-        If *netdiscovery* is not present in any of the paths above, you can specifie path with the argument *netdiscover_path* on Discover class.
-        
-        .. code-block:: python
-        
-            disc = Discover(netdiscover_path="path_of_netdiscover")
-        
 Keywords: network,netdiscover,arpscanner,sysadmin
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -85,7 +18,77 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==================
+python-netdiscover
+==================
+
+.. image:: https://img.shields.io/pypi/v/python-netdiscover.svg
+        :target: https://pypi.python.org/pypi/python-netdiscover
+
+.. image:: https://img.shields.io/pypi/pyversions/python-netdiscover.svg
+        :target: https://pypi.python.org/pypi/python-netdiscover
+
+The  python-netdiscover is a simple wrapper for the `netdiscover reconnaissance tool <https://sourceforge.net/projects/netdiscover/>`_.
+
+This library offers a simple way to create scans from a python script and analyse the results.
+
+
+* Documentation: https://python-netdiscover.readthedocs.io
+* GitHub: https://github.com/MrSuicideParrot/python-netdiscover
+* PyPI: https://pypi.org/project/python-netdiscover/
+
+Installation
+============
+First, you will need to install the `netdiscover binary <https://sourceforge.net/projects/netdiscover/>`_ on your system, this may depend on your operating system. Many distributions have this tool available in `their main repository <https://pkgs.org/download/netdiscover>`_. 
+
+From the shell, uncompress python-netdiscover.tar.gz and then run make :
+
+.. code-block:: bash
+
+    $ tar xvzf python-netdiscover.tar.gz
+    $ cd python-netdiscover
+    $ python setup.py install
+
+or using Pip
+
+.. code-block:: bash
+
+    $ pip install python-netdiscover
+
+
+Usage
+=====
+From python/ipython:
+--------------------
+
+.. code-block:: python
+
+    >>> from netdiscover import *
+    >>> disc = Discover()
+    >>> disc.scan(ip_range="192.168.1.0/24")
+    [{'mac': b'73:8b:10:0e:bd:23', 'ip': b'192.168.1.1'}, {'mac': b'f4:3c:4a:73:47:07', 'ip': b'192.168.1.2'}]
+
+
+Notes
+=====
+This tool needs to be run as root. It is necessary to be presented on the system the *netdiscover* tool. The library will look for the *netdiscovery* binary in the following paths:
+
+*  netdiscover
+* /usr/bin/netdiscover
+* /usr/sbin/netdiscover
+* /usr/local/bin/netdiscover
+* /sw/bin/netdiscover
+* /opt/local/bin/netdiscover
+
+If *netdiscovery* is not present in any of the paths above, you can specifie path with the argument *netdiscover_path* on Discover class.
+
+.. code-block:: python
+
+    disc = Discover(netdiscover_path="path_of_netdiscover")
```

### Comparing `python-netdiscover-0.2.0/docs/make.bat` & `python-netdiscover-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/docs/installation.rst` & `python-netdiscover-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/docs/readme.rst` & `python-netdiscover-0.3.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/docs/conf.py` & `python-netdiscover-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/docs/Makefile` & `python-netdiscover-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/setup.py` & `python-netdiscover-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords='network, netdiscover, arpscanner, sysadmin',
     name='python-netdiscover',
     packages=find_packages(include=['netdiscover']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MrSuicideParrot/python-netdiscover',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `python-netdiscover-0.2.0/CONTRIBUTING.rst` & `python-netdiscover-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-netdiscover-0.2.0/LICENSE` & `python-netdiscover-0.3.0/LICENSE`

 * *Files identical despite different names*

