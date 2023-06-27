# Comparing `tmp/PyIpify-0.0.3.tar.gz` & `tmp/pyipify-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIpify-0.0.3.tar", last modified: Tue May 30 10:20:11 2023, max compression
+gzip compressed data, was "pyipify-0.0.3.1.tar", last modified: Tue Jun 27 15:12:43 2023, max compression
```

## Comparing `PyIpify-0.0.3.tar` & `pyipify-0.0.3.1.tar`

### file list

```diff
@@ -1,39 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.449116 PyIpify-0.0.3/
--rw-rw-rw-   0        0        0     3207 2023-05-30 10:20:11.449116 PyIpify-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.305926 PyIpify-0.0.3/PyIpify/
--rw-rw-rw-   0        0        0       38 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-05-30 10:03:50.000000 PyIpify-0.0.3/PyIpify/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.384818 PyIpify-0.0.3/PyIpify/asyncronous/
--rw-rw-rw-   0        0        0      106 2023-05-30 10:10:28.000000 PyIpify-0.0.3/PyIpify/asyncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.415011 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/
--rw-rw-rw-   0        0        0      201 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      247 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      522 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0     1294 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      523 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0     1295 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      542 2023-05-30 09:54:05.000000 PyIpify-0.0.3/PyIpify/asyncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      569 2023-05-30 09:54:51.000000 PyIpify-0.0.3/PyIpify/asyncronous/find_ipv6.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.416530 PyIpify-0.0.3/PyIpify/syncronous/
--rw-rw-rw-   0        0        0      104 2023-05-30 10:10:24.000000 PyIpify-0.0.3/PyIpify/syncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.447807 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/
--rw-rw-rw-   0        0        0      200 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      246 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      373 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0      516 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      374 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0      517 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      404 2023-05-30 09:55:37.000000 PyIpify-0.0.3/PyIpify/syncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      400 2023-05-30 09:56:00.000000 PyIpify-0.0.3/PyIpify/syncronous/find_ipv6.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.369198 PyIpify-0.0.3/PyIpify.egg-info/
--rw-rw-rw-   0        0        0     3207 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2144 2023-05-30 09:51:34.000000 PyIpify-0.0.3/README.md
--rw-rw-rw-   0        0        0    11549 2023-05-30 09:50:44.000000 PyIpify-0.0.3/license.md
--rw-rw-rw-   0        0        0      232 2023-05-30 09:53:00.000000 PyIpify-0.0.3/main.py
--rw-rw-rw-   0        0        0       28 2023-05-30 09:50:44.000000 PyIpify-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 10:20:11.449116 PyIpify-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1772 2023-05-30 10:19:41.000000 PyIpify-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:12:43.828850 pyipify-0.0.3.1/
+-rw-rw-rw-   0        0        0       96 2023-06-22 16:09:11.000000 pyipify-0.0.3.1/.deepsource.toml
+-rw-rw-rw-   0        0        0     5356 2023-06-22 16:09:11.000000 pyipify-0.0.3.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     3596 2023-06-22 16:09:11.000000 pyipify-0.0.3.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     3216 2023-06-27 15:12:43.816367 pyipify-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2149 2023-06-22 16:25:29.000000 pyipify-0.0.3.1/README.md
+-rw-rw-rw-   0        0        0    11549 2023-06-22 16:09:11.000000 pyipify-0.0.3.1/license.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:12:43.753675 pyipify-0.0.3.1/pyipify/
+-rw-rw-rw-   0        0        0       73 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:12:43.800644 pyipify-0.0.3.1/pyipify/asynchronous/
+-rw-rw-rw-   0        0        0      122 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/asynchronous/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/asynchronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      636 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/asynchronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:12:43.816367 pyipify-0.0.3.1/pyipify/synchronous/
+-rw-rw-rw-   0        0        0      135 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/synchronous/__init__.py
+-rw-rw-rw-   0        0        0      475 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/synchronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      486 2023-06-27 15:11:04.000000 pyipify-0.0.3.1/pyipify/synchronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:12:43.784947 pyipify-0.0.3.1/pyipify.egg-info/
+-rw-rw-rw-   0        0        0     3216 2023-06-27 15:12:43.000000 pyipify-0.0.3.1/pyipify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-27 15:12:43.000000 pyipify-0.0.3.1/pyipify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:12:43.000000 pyipify-0.0.3.1/pyipify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-27 15:12:43.000000 pyipify-0.0.3.1/pyipify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 15:12:43.000000 pyipify-0.0.3.1/pyipify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       28 2023-06-22 16:09:11.000000 pyipify-0.0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:12:43.828850 pyipify-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2052 2023-06-27 15:02:39.000000 pyipify-0.0.3.1/setup.py
```

### Comparing `PyIpify-0.0.3/PKG-INFO` & `pyipify-0.0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: PyIpify
-Version: 0.0.3
+Name: pyipify
+Version: 0.0.3.1
 Summary: A simple python library to find the public ip address of the system.
 Home-page: https://github.com/SigireddyBalasai/ipify
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
 Author: SigireddyBalasai
 Author-email: sigireddybalasai@gmail.com
 License: MIT
-Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asyncronous,ipify syncronous
+Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asynchronous,ipify synchronous
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -53,37 +53,37 @@
 pip install Pyipify
 ```
 
 
     
 ## Examples
 
-get ip address syncronous
+get ip address synchronous
 
 ```py
-from Pyipify.syncronous import find_ipv4,find_ipv6
+from Pyipify.synchronous import find_ipv4,find_ipv6
 ipv4_address = find_ipv4()
 ipv6_address = find_ipv6()
 print(ipv4_address,ipv6_address)
 ```
 
-get ip address asyncronously
+get ip address asynchronously
 ```py
-from Pyipify.asyncronous import find_ipv4,find_ipv6
+from Pyipify.asynchronous import find_ipv4,find_ipv6
 import asyncio
 async def main():
     ipv4_address = await find_ipv4()
     ipv6_address = await find_ipv6()
     return ipv4_address,ipv6_address
 asyncio.run(main())
 ```
 
 use cli to get ip address
 ``` python -m ipify -h```
-to get strted
+to get started
 
 
 
 
 ## Contributing
 
 Contributions are always welcome!
```

### Comparing `PyIpify-0.0.3/PyIpify/asyncronous/find_ipv6.py` & `pyipify-0.0.3.1/pyipify/asynchronous/find_ipv4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+"""this module contains the asynchronous function for finding the IPv4 address of the client."""
 import aiohttp
 
-async def find_ipv6():
-    """Return the public IPv6 address of the system.
-    This function is asyncronous.
-    
+
+async def find_ipv4():
+    """Returns the IPv4 address of the client.
+    This function is asynchronous.
+
     Returns:
-        str: The IPv6 address of the client.
-        
-        Example:
-            >>> import asyncio
-            >>> from PyIpify.asyncronous import find_ipv6
-            >>> asyncio.run(find_ipv6())
-            
+        str: The IPv4 address of the client.
+
+    Example:
+        >>> import asyncio
+        >>> from pyipify.asynchronous import find_ipv4
+        >>> asyncio.run(find_ipv4())
     """
     async with aiohttp.ClientSession() as session:
-        async with session.get('https://api64.ipify.org?format=json') as response:
+        async with session.get('https://api.ipify.org?format=json') as response:
             return (await response.json())['ip']
-
```

### Comparing `PyIpify-0.0.3/PyIpify.egg-info/PKG-INFO` & `pyipify-0.0.3.1/pyipify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: PyIpify
-Version: 0.0.3
+Name: pyipify
+Version: 0.0.3.1
 Summary: A simple python library to find the public ip address of the system.
 Home-page: https://github.com/SigireddyBalasai/ipify
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
 Author: SigireddyBalasai
 Author-email: sigireddybalasai@gmail.com
 License: MIT
-Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asyncronous,ipify syncronous
+Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asynchronous,ipify synchronous
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -53,37 +53,37 @@
 pip install Pyipify
 ```
 
 
     
 ## Examples
 
-get ip address syncronous
+get ip address synchronous
 
 ```py
-from Pyipify.syncronous import find_ipv4,find_ipv6
+from Pyipify.synchronous import find_ipv4,find_ipv6
 ipv4_address = find_ipv4()
 ipv6_address = find_ipv6()
 print(ipv4_address,ipv6_address)
 ```
 
-get ip address asyncronously
+get ip address asynchronously
 ```py
-from Pyipify.asyncronous import find_ipv4,find_ipv6
+from Pyipify.asynchronous import find_ipv4,find_ipv6
 import asyncio
 async def main():
     ipv4_address = await find_ipv4()
     ipv6_address = await find_ipv6()
     return ipv4_address,ipv6_address
 asyncio.run(main())
 ```
 
 use cli to get ip address
 ``` python -m ipify -h```
-to get strted
+to get started
 
 
 
 
 ## Contributing
 
 Contributions are always welcome!
```

### Comparing `PyIpify-0.0.3/README.md` & `pyipify-0.0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,60 +75,61 @@
 000004a0: 7374 616c 6c61 7469 6f6e 0d0a 0d0a 496e  stallation....In
 000004b0: 7374 616c 6c20 6d79 2d70 726f 6a65 6374  stall my-project
 000004c0: 2077 6974 6820 6e70 6d0d 0a0d 0a60 6060   with npm....```
 000004d0: 7079 0d0a 7069 7020 696e 7374 616c 6c20  py..pip install 
 000004e0: 5079 6970 6966 790d 0a60 6060 0d0a 0d0a  Pyipify..```....
 000004f0: 0d0a 2020 2020 0d0a 2323 2045 7861 6d70  ..    ..## Examp
 00000500: 6c65 730d 0a0d 0a67 6574 2069 7020 6164  les....get ip ad
-00000510: 6472 6573 7320 7379 6e63 726f 6e6f 7573  dress syncronous
-00000520: 0d0a 0d0a 6060 6070 790d 0a66 726f 6d20  ....```py..from 
-00000530: 5079 6970 6966 792e 7379 6e63 726f 6e6f  Pyipify.syncrono
-00000540: 7573 2069 6d70 6f72 7420 6669 6e64 5f69  us import find_i
-00000550: 7076 342c 6669 6e64 5f69 7076 360d 0a69  pv4,find_ipv6..i
-00000560: 7076 345f 6164 6472 6573 7320 3d20 6669  pv4_address = fi
-00000570: 6e64 5f69 7076 3428 290d 0a69 7076 365f  nd_ipv4()..ipv6_
-00000580: 6164 6472 6573 7320 3d20 6669 6e64 5f69  address = find_i
-00000590: 7076 3628 290d 0a70 7269 6e74 2869 7076  pv6()..print(ipv
-000005a0: 345f 6164 6472 6573 732c 6970 7636 5f61  4_address,ipv6_a
-000005b0: 6464 7265 7373 290d 0a60 6060 0d0a 0d0a  ddress)..```....
-000005c0: 6765 7420 6970 2061 6464 7265 7373 2061  get ip address a
-000005d0: 7379 6e63 726f 6e6f 7573 6c79 0d0a 6060  syncronously..``
-000005e0: 6070 790d 0a66 726f 6d20 5079 6970 6966  `py..from Pyipif
-000005f0: 792e 6173 796e 6372 6f6e 6f75 7320 696d  y.asyncronous im
-00000600: 706f 7274 2066 696e 645f 6970 7634 2c66  port find_ipv4,f
-00000610: 696e 645f 6970 7636 0d0a 696d 706f 7274  ind_ipv6..import
-00000620: 2061 7379 6e63 696f 0d0a 6173 796e 6320   asyncio..async 
-00000630: 6465 6620 6d61 696e 2829 3a0d 0a20 2020  def main():..   
-00000640: 2069 7076 345f 6164 6472 6573 7320 3d20   ipv4_address = 
-00000650: 6177 6169 7420 6669 6e64 5f69 7076 3428  await find_ipv4(
-00000660: 290d 0a20 2020 2069 7076 365f 6164 6472  )..    ipv6_addr
-00000670: 6573 7320 3d20 6177 6169 7420 6669 6e64  ess = await find
-00000680: 5f69 7076 3628 290d 0a20 2020 2072 6574  _ipv6()..    ret
-00000690: 7572 6e20 6970 7634 5f61 6464 7265 7373  urn ipv4_address
-000006a0: 2c69 7076 365f 6164 6472 6573 730d 0a61  ,ipv6_address..a
-000006b0: 7379 6e63 696f 2e72 756e 286d 6169 6e28  syncio.run(main(
-000006c0: 2929 0d0a 6060 600d 0a0d 0a75 7365 2063  ))..```....use c
-000006d0: 6c69 2074 6f20 6765 7420 6970 2061 6464  li to get ip add
-000006e0: 7265 7373 0d0a 6060 6020 7079 7468 6f6e  ress..``` python
-000006f0: 202d 6d20 6970 6966 7920 2d68 6060 600d   -m ipify -h```.
-00000700: 0a74 6f20 6765 7420 7374 7274 6564 0d0a  .to get strted..
-00000710: 0d0a 0d0a 0d0a 0d0a 2323 2043 6f6e 7472  ........## Contr
-00000720: 6962 7574 696e 670d 0a0d 0a43 6f6e 7472  ibuting....Contr
-00000730: 6962 7574 696f 6e73 2061 7265 2061 6c77  ibutions are alw
-00000740: 6179 7320 7765 6c63 6f6d 6521 0d0a 0d0a  ays welcome!....
-00000750: 5365 6520 6063 6f6e 7472 6962 7574 696e  See `contributin
-00000760: 672e 6d64 6020 666f 7220 7761 7973 2074  g.md` for ways t
-00000770: 6f20 6765 7420 7374 6172 7465 642e 0d0a  o get started...
-00000780: 0d0a 506c 6561 7365 2061 6468 6572 6520  ..Please adhere 
-00000790: 746f 2074 6869 7320 7072 6f6a 6563 7427  to this project'
-000007a0: 7320 6063 6f64 6520 6f66 2063 6f6e 6475  s `code of condu
-000007b0: 6374 602e 0d0a 0d0a 0d0a 2323 204c 6963  ct`.......## Lic
-000007c0: 656e 7365 0d0a 0d0a 5b41 7061 6368 6520  ense....[Apache 
-000007d0: 322e 305d 2868 7474 7073 3a2f 2f63 686f  2.0](https://cho
-000007e0: 6f73 6561 6c69 6365 6e73 652e 636f 6d2f  osealicense.com/
-000007f0: 6c69 6365 6e73 6573 2f61 7061 6368 652d  licenses/apache-
-00000800: 322e 302f 290d 0a0d 0a0d 0a23 2320 5375  2.0/)......## Su
-00000810: 7070 6f72 740d 0a0d 0a46 6f72 2073 7570  pport....For sup
-00000820: 706f 7274 2c20 656d 6169 6c20 7369 6769  port, email sigi
-00000830: 7265 6464 7962 616c 6173 6169 4067 6d61  reddybalasai@gma
-00000840: 696c 2e63 6f6d 206f 7220 6f70 656e 2061  il.com or open a
-00000850: 6e20 6973 7375 6520 6865 7265 0d0a 0d0a  n issue here....
+00000510: 6472 6573 7320 7379 6e63 6872 6f6e 6f75  dress synchronou
+00000520: 730d 0a0d 0a60 6060 7079 0d0a 6672 6f6d  s....```py..from
+00000530: 2050 7969 7069 6679 2e73 796e 6368 726f   Pyipify.synchro
+00000540: 6e6f 7573 2069 6d70 6f72 7420 6669 6e64  nous import find
+00000550: 5f69 7076 342c 6669 6e64 5f69 7076 360d  _ipv4,find_ipv6.
+00000560: 0a69 7076 345f 6164 6472 6573 7320 3d20  .ipv4_address = 
+00000570: 6669 6e64 5f69 7076 3428 290d 0a69 7076  find_ipv4()..ipv
+00000580: 365f 6164 6472 6573 7320 3d20 6669 6e64  6_address = find
+00000590: 5f69 7076 3628 290d 0a70 7269 6e74 2869  _ipv6()..print(i
+000005a0: 7076 345f 6164 6472 6573 732c 6970 7636  pv4_address,ipv6
+000005b0: 5f61 6464 7265 7373 290d 0a60 6060 0d0a  _address)..```..
+000005c0: 0d0a 6765 7420 6970 2061 6464 7265 7373  ..get ip address
+000005d0: 2061 7379 6e63 6872 6f6e 6f75 736c 790d   asynchronously.
+000005e0: 0a60 6060 7079 0d0a 6672 6f6d 2050 7969  .```py..from Pyi
+000005f0: 7069 6679 2e61 7379 6e63 6872 6f6e 6f75  pify.asynchronou
+00000600: 7320 696d 706f 7274 2066 696e 645f 6970  s import find_ip
+00000610: 7634 2c66 696e 645f 6970 7636 0d0a 696d  v4,find_ipv6..im
+00000620: 706f 7274 2061 7379 6e63 696f 0d0a 6173  port asyncio..as
+00000630: 796e 6320 6465 6620 6d61 696e 2829 3a0d  ync def main():.
+00000640: 0a20 2020 2069 7076 345f 6164 6472 6573  .    ipv4_addres
+00000650: 7320 3d20 6177 6169 7420 6669 6e64 5f69  s = await find_i
+00000660: 7076 3428 290d 0a20 2020 2069 7076 365f  pv4()..    ipv6_
+00000670: 6164 6472 6573 7320 3d20 6177 6169 7420  address = await 
+00000680: 6669 6e64 5f69 7076 3628 290d 0a20 2020  find_ipv6()..   
+00000690: 2072 6574 7572 6e20 6970 7634 5f61 6464   return ipv4_add
+000006a0: 7265 7373 2c69 7076 365f 6164 6472 6573  ress,ipv6_addres
+000006b0: 730d 0a61 7379 6e63 696f 2e72 756e 286d  s..asyncio.run(m
+000006c0: 6169 6e28 2929 0d0a 6060 600d 0a0d 0a75  ain())..```....u
+000006d0: 7365 2063 6c69 2074 6f20 6765 7420 6970  se cli to get ip
+000006e0: 2061 6464 7265 7373 0d0a 6060 6020 7079   address..``` py
+000006f0: 7468 6f6e 202d 6d20 6970 6966 7920 2d68  thon -m ipify -h
+00000700: 6060 600d 0a74 6f20 6765 7420 7374 6172  ```..to get star
+00000710: 7465 640d 0a0d 0a0d 0a0d 0a0d 0a23 2320  ted..........## 
+00000720: 436f 6e74 7269 6275 7469 6e67 0d0a 0d0a  Contributing....
+00000730: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00000740: 6520 616c 7761 7973 2077 656c 636f 6d65  e always welcome
+00000750: 210d 0a0d 0a53 6565 2060 636f 6e74 7269  !....See `contri
+00000760: 6275 7469 6e67 2e6d 6460 2066 6f72 2077  buting.md` for w
+00000770: 6179 7320 746f 2067 6574 2073 7461 7274  ays to get start
+00000780: 6564 2e0d 0a0d 0a50 6c65 6173 6520 6164  ed.....Please ad
+00000790: 6865 7265 2074 6f20 7468 6973 2070 726f  here to this pro
+000007a0: 6a65 6374 2773 2060 636f 6465 206f 6620  ject's `code of 
+000007b0: 636f 6e64 7563 7460 2e0d 0a0d 0a0d 0a23  conduct`.......#
+000007c0: 2320 4c69 6365 6e73 650d 0a0d 0a5b 4170  # License....[Ap
+000007d0: 6163 6865 2032 2e30 5d28 6874 7470 733a  ache 2.0](https:
+000007e0: 2f2f 6368 6f6f 7365 616c 6963 656e 7365  //choosealicense
+000007f0: 2e63 6f6d 2f6c 6963 656e 7365 732f 6170  .com/licenses/ap
+00000800: 6163 6865 2d32 2e30 2f29 0d0a 0d0a 0d0a  ache-2.0/)......
+00000810: 2323 2053 7570 706f 7274 0d0a 0d0a 466f  ## Support....Fo
+00000820: 7220 7375 7070 6f72 742c 2065 6d61 696c  r support, email
+00000830: 2073 6967 6972 6564 6479 6261 6c61 7361   sigireddybalasa
+00000840: 6940 676d 6169 6c2e 636f 6d20 6f72 206f  i@gmail.com or o
+00000850: 7065 6e20 616e 2069 7373 7565 2068 6572  pen an issue her
+00000860: 650d 0a0d 0a                             e....
```

### Comparing `PyIpify-0.0.3/license.md` & `pyipify-0.0.3.1/license.md`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.3/setup.py` & `pyipify-0.0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-from setuptools import setup
-import pathlib
+"""
+Setup file for the pyipify package.
+"""
 import os
+import pathlib
+from setuptools import setup
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def readme() -> str:
-    with open(r"README.md") as f:
-        README = f.read()
-    return README
+    """This will read the readme file"""
+    with open(str(pathlib.Path(dir_path) / "README.md"), encoding='utf-8') as file:
+        readme_data = file.read()
+    return readme_data
 
 
 def reqs():
+    """THis will read the requirements file"""
     print(dir_path)
-    with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r") as f:
-        requirements = [line.strip() for line in f]
+    with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r", encoding='utf-8') as file:
+        requirements = [line.strip() for line in file]
         return requirements
 
 
 setup(
-    name="PyIpify",
-    packages=['Pyipify', 'PyIpify.syncronous', 'PyIpify.asyncronous'],
-    version="0.0.3",
+    name="pyipify",
+    packages=['pyipify', 'pyipify.synchronous', 'pyipify.asynchronous'],
+    version="0.0.3.1",
     setup_requires=['setuptools_scm'],
     license="MIT",
     description="A simple python library to find the public ip address of the system.",
     author="SigireddyBalasai",
     author_email="sigireddybalasai@gmail.com",
     url="https://github.com/SigireddyBalasai/ipify",
     download_url="https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz",
-    keywords=["ipify", "ip", "ip address", "ipify.org", "ipify api", "ipify python", "ipify python library", "ipify python api", "ipify python library", "ipify python api", "ipify python package", "ipify","ipify cli","ipify asyncronous",'ipify syncronous'],
+    keywords=["ipify", "ip", "ip address", "ipify.org", "ipify api", "ipify python",
+              "ipify python library", "ipify python api", "ipify python library",
+              "ipify python api", "ipify python package",
+              "ipify", "ipify cli", "ipify asynchronous", 'ipify synchronous'],
     install_requires=reqs(),
     include_package_data=True,
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-)
+)
```

