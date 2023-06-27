# Comparing `tmp/python-netbox-0.0.8.tar.gz` & `tmp/python-netbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-netbox-0.0.8.tar", last modified: Tue Jan 23 08:14:18 2018, max compression
+gzip compressed data, was "dist/python-netbox-0.0.9.tar", last modified: Fri Feb 23 07:51:24 2018, max compression
```

## Comparing `python-netbox-0.0.8.tar` & `python-netbox-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-01-23 08:14:18.000000 python-netbox-0.0.8/
-drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     2275 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1001) thomas    (1001)        1 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1001) thomas    (1001)       19 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1001) thomas    (1001)        7 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1001) thomas    (1001)      348 2018-01-23 08:14:18.000000 python-netbox-0.0.8/python_netbox.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     1242 2018-01-11 05:58:25.000000 python-netbox-0.0.8/README.rst
--rw-rw-r--   0 thomas    (1001) thomas    (1001)        0 2017-09-22 08:54:58.000000 python-netbox-0.0.8/MANIFEST.in
-drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-01-23 08:14:18.000000 python-netbox-0.0.8/netbox/
--rw-rw-r--   0 thomas    (1001) thomas    (1001)    16550 2018-01-23 08:12:26.000000 python-netbox-0.0.8/netbox/dcim.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)       26 2017-09-22 08:54:58.000000 python-netbox-0.0.8/netbox/__init__.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     1503 2017-11-08 10:39:21.000000 python-netbox-0.0.8/netbox/exceptions.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)    13050 2017-12-18 06:26:55.000000 python-netbox-0.0.8/netbox/ipam.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     6674 2017-11-08 10:39:21.000000 python-netbox-0.0.8/netbox/virtualization.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)      526 2018-01-22 13:07:21.000000 python-netbox-0.0.8/netbox/netbox.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     4681 2017-12-14 10:52:06.000000 python-netbox-0.0.8/netbox/connection.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)      941 2018-01-23 08:12:59.000000 python-netbox-0.0.8/setup.py
--rw-rw-r--   0 thomas    (1001) thomas    (1001)     2275 2018-01-23 08:14:18.000000 python-netbox-0.0.8/PKG-INFO
--rw-rw-r--   0 thomas    (1001) thomas    (1001)       38 2018-01-23 08:14:18.000000 python-netbox-0.0.8/setup.cfg
+drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-02-23 07:51:24.000000 python-netbox-0.0.9/
+drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-02-23 07:51:24.000000 python-netbox-0.0.9/python_netbox.egg-info/
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     2275 2018-02-23 07:51:23.000000 python-netbox-0.0.9/python_netbox.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)        1 2018-02-23 07:51:23.000000 python-netbox-0.0.9/python_netbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)       19 2018-02-23 07:51:23.000000 python-netbox-0.0.9/python_netbox.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)        7 2018-02-23 07:51:23.000000 python-netbox-0.0.9/python_netbox.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)      366 2018-02-23 07:51:24.000000 python-netbox-0.0.9/python_netbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     1242 2018-01-11 05:58:25.000000 python-netbox-0.0.9/README.rst
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)        0 2017-09-22 08:54:58.000000 python-netbox-0.0.9/MANIFEST.in
+drwxrwxr-x   0 thomas    (1001) thomas    (1001)        0 2018-02-23 07:51:24.000000 python-netbox-0.0.9/netbox/
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)    16540 2018-02-23 07:29:09.000000 python-netbox-0.0.9/netbox/dcim.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)       26 2017-09-22 08:54:58.000000 python-netbox-0.0.9/netbox/__init__.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     1503 2017-11-08 10:39:21.000000 python-netbox-0.0.9/netbox/exceptions.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)    13321 2018-02-13 10:22:20.000000 python-netbox-0.0.9/netbox/ipam.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     6674 2017-11-08 10:39:21.000000 python-netbox-0.0.9/netbox/virtualization.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)      615 2018-02-23 07:23:59.000000 python-netbox-0.0.9/netbox/netbox.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     4681 2017-12-14 10:52:06.000000 python-netbox-0.0.9/netbox/connection.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     3381 2018-02-23 07:34:54.000000 python-netbox-0.0.9/netbox/tenancy.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)      941 2018-02-23 07:48:41.000000 python-netbox-0.0.9/setup.py
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)     2275 2018-02-23 07:51:24.000000 python-netbox-0.0.9/PKG-INFO
+-rw-rw-r--   0 thomas    (1001) thomas    (1001)       38 2018-02-23 07:51:24.000000 python-netbox-0.0.9/setup.cfg
```

### Comparing `python-netbox-0.0.8/python_netbox.egg-info/PKG-INFO` & `python-netbox-0.0.9/python_netbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: python-netbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python NetBox Client
 Home-page: https://github.com/jagter/python-netbox
 Author: Thomas van der Jagt
 Author-email: thomas@tjrb.nl
 License: UNKNOWN
-Download-URL: https://github.com/jagter/python-netbox/releases/tag/0.0.4.tar.gz
+Download-URL: https://github.com/jagter/python-netbox/releases/tag/0.0.9.tar.gz
 Description: ============================
         Python Netbox Client
         ============================
         
         python-netbox is a client for the Netbox (https://github.com/digitalocean/netbox) API.
         It's based on the APIv2 which is released since version 2.0.0.
```

### Comparing `python-netbox-0.0.8/README.rst` & `python-netbox-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `python-netbox-0.0.8/netbox/dcim.py` & `python-netbox-0.0.9/netbox/dcim.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.netbox_con = netbox_con
 
     def get_sites(self, **kwargs):
         """Returns the available sites"""
         return self.netbox_con.get('/dcim/sites/', **kwargs)
 
     def create_site(self, name, slug, **kwargs):
-        """Create new site
+        """Create a new site
 
         :param name: Site name
         :param slug: slug name
         :param kwargs: optional fields
         :return: bool True if successful otherwise exception raised
         """
         required_fields = {"name": name, "slug": slug}
@@ -32,15 +32,15 @@
         except IndexError:
             raise exceptions.NotFoundException('site: {}'.format(site_name)) from None
         return self.netbox_con.delete('/dcim/sites/', site_id)
 
     def update_site(self, site_name, **kwargs):
         """
 
-        :param site_name: device-type name to update
+        :param site_name: Site to update
         :param kwargs: requests body dict
         :return: bool True if successful otherwise raise UpdateException
         """
         try:
             site_id = self.get_sites(name=site_name)[0]['id']
         except IndexError:
             raise exceptions.NotFoundException('site: {}'.format(site_name)) from None
```

### Comparing `python-netbox-0.0.8/netbox/exceptions.py` & `python-netbox-0.0.9/netbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-netbox-0.0.8/netbox/ipam.py` & `python-netbox-0.0.9/netbox/ipam.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,22 @@
         """
         try:
             ip_id = self.get_ip_addresses(q=ip_address)[0]['id']
         except IndexError:
             raise exceptions.NotFoundException('ip: {}'.format(ip_address)) from None
         return self.netbox_con.delete('/ipam/ip-addresses/', ip_id)
 
+    def delete_ip_by_id(self, ip_id):
+        """Delete IP address
+
+        :param ip_id: ID of ip address to delete
+        :return: bool True if successful otherwise raise DeleteException
+        """
+        return self.netbox_con.delete('/ipam/ip-addresses/', ip_id)
+
     def get_ip_prefixes(self, **kwargs):
         """Return all ip prefixes"""
         return self.netbox_con.get('/ipam/prefixes/', **kwargs)
 
     def create_ip_prefix(self, prefix, **kwargs):
         """Create a new ip prefix
```

### Comparing `python-netbox-0.0.8/netbox/virtualization.py` & `python-netbox-0.0.9/netbox/virtualization.py`

 * *Files identical despite different names*

### Comparing `python-netbox-0.0.8/netbox/netbox.py` & `python-netbox-0.0.9/netbox/netbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import netbox.connection as connection
 import netbox.dcim as dcim
 import netbox.ipam as ipam
 import netbox.virtualization as virtualization
 import netbox.exceptions as exceptions
+import netbox.tenancy as tenancy
 
 
 class NetBox(object):
     def __init__(self, host, **kwargs):
         self.connection = connection.NetboxConnection(host=host, **kwargs)
         self.ipam = ipam.Ipam(self.connection)
         self.dcim = dcim.Dcim(self.connection)
         self.virtualization = virtualization.Virtualization(self.connection)
+        self.tenancy = tenancy.Tenancy(self.connection)
         self.exceptions = exceptions
```

### Comparing `python-netbox-0.0.8/netbox/connection.py` & `python-netbox-0.0.9/netbox/connection.py`

 * *Files identical despite different names*

### Comparing `python-netbox-0.0.8/setup.py` & `python-netbox-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(name='python-netbox',
-      version='0.0.8',
+      version='0.0.9',
       description='Python NetBox Client',
       long_description=readme(),
       python_requires='>=3',
       author='Thomas van der Jagt',
       author_email='thomas@tjrb.nl',
       url='https://github.com/jagter/python-netbox',
-      download_url='https://github.com/jagter/python-netbox/releases/tag/0.0.4.tar.gz',
+      download_url='https://github.com/jagter/python-netbox/releases/tag/0.0.9.tar.gz',
       packages=find_packages(),
       install_requires=['ipaddress', 'requests'],
       classifiers = [
         "Programming Language :: Python :: 3",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.6",
```

### Comparing `python-netbox-0.0.8/PKG-INFO` & `python-netbox-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: python-netbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python NetBox Client
 Home-page: https://github.com/jagter/python-netbox
 Author: Thomas van der Jagt
 Author-email: thomas@tjrb.nl
 License: UNKNOWN
-Download-URL: https://github.com/jagter/python-netbox/releases/tag/0.0.4.tar.gz
+Download-URL: https://github.com/jagter/python-netbox/releases/tag/0.0.9.tar.gz
 Description: ============================
         Python Netbox Client
         ============================
         
         python-netbox is a client for the Netbox (https://github.com/digitalocean/netbox) API.
         It's based on the APIv2 which is released since version 2.0.0.
```

