# Comparing `tmp/acore_db_ssh_tunnel-0.1.2.tar.gz` & `tmp/acore_db_ssh_tunnel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_db_ssh_tunnel-0.1.2.tar", last modified: Fri Jun 16 15:41:39 2023, max compression
+gzip compressed data, was "acore_db_ssh_tunnel-0.1.3.tar", last modified: Tue Jun 27 04:25:06 2023, max compression
```

## Comparing `acore_db_ssh_tunnel-0.1.2.tar` & `acore_db_ssh_tunnel-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.387557 acore_db_ssh_tunnel-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 15:41:39.387421 acore_db_ssh_tunnel-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4527 2023-06-16 04:35:58.000000 acore_db_ssh_tunnel-0.1.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.385612 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/
--rw-r--r--   0 sanhehu    (501) staff       (20)      436 2023-06-16 04:36:53.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 15:39:32.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1938 2023-06-16 04:24:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/acore_ssh_tunnel.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-16 04:25:38.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386424 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      354 2023-06-16 03:06:37.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/mysql_engine.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7930 2023-06-16 15:39:03.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/ssh_tunnel.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386716 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386986 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386269 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      844 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1113 2023-06-16 15:40:46.000000 acore_db_ssh_tunnel-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       77 2023-06-16 04:31:11.000000 acore_db_ssh_tunnel-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 15:41:39.387592 acore_db_ssh_tunnel-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.387128 acore_db_ssh_tunnel-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      414 2023-06-16 04:26:05.000000 acore_db_ssh_tunnel-0.1.2/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.756992 acore_db_ssh_tunnel-0.1.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-27 04:25:06.756851 acore_db_ssh_tunnel-0.1.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4527 2023-06-16 04:35:58.000000 acore_db_ssh_tunnel-0.1.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.754430 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      436 2023-06-16 04:36:53.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-27 04:21:44.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1938 2023-06-16 04:24:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/acore_ssh_tunnel.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      320 2023-06-27 04:20:57.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.755806 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      354 2023-06-16 03:06:37.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/mysql_engine.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7927 2023-06-27 04:21:37.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/ssh_tunnel.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.756205 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.756518 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.755692 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-27 04:25:06.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      844 2023-06-27 04:25:06.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-27 04:25:06.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-06-27 04:25:06.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-27 04:25:06.000000 acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-27 04:23:06.000000 acore_db_ssh_tunnel-0.1.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       77 2023-06-16 04:31:11.000000 acore_db_ssh_tunnel-0.1.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-27 04:25:06.757038 acore_db_ssh_tunnel-0.1.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 04:25:06.756671 acore_db_ssh_tunnel-0.1.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      440 2023-06-27 04:24:33.000000 acore_db_ssh_tunnel-0.1.3/tests/test_api.py
```

### Comparing `acore_db_ssh_tunnel-0.1.2/AUTHORS.rst` & `acore_db_ssh_tunnel-0.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/LICENSE.txt` & `acore_db_ssh_tunnel-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/PKG-INFO` & `acore_db_ssh_tunnel-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_db_ssh_tunnel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create Database SSH Tunnel for Azerothcore World of Warcraft MySQL Database
 Home-page: https://github.com/MacHu-GWU/acore_db_ssh_tunnel-project
-Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_db_ssh_tunnel-0.1.2/README.rst` & `acore_db_ssh_tunnel-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/acore_ssh_tunnel.py` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/acore_ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/paths.py` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/paths.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/ssh_tunnel.py` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/ssh_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,17 @@
             "Enter the following command in terminal to create SSH tunnel: "
         )
         print_func(f"  {ssh_cmd}")
     else:
         print_func("Failed to create SSH Tunnel.")
 
 
-def list_ssh_tunnel_pid(path_pem_file) -> T.List[str]:
+def list_ssh_tunnel_pid(
+    path_pem_file,
+) -> T.List[str]:
     """
     List the PID of SSH Tunnel processes.
 
     找出在本地机器上已有的 SSH Tunnel 的 PID (process id, 即进程 ID). 其原理是用
     `ps aux <https://www.linode.com/docs/guides/use-the-ps-aux-command-in-linux/>`_
     命令以 BSD 的格式列出所有进程, 而这个进程一定是包含 ``ssh`` 的. 然后再用 python 捕获
     这些进程列表, 这些进程里包含 pem 文件路径的就一定是我们要找的 SSH Tunnel 进程.
@@ -114,15 +116,15 @@
             words = [word.strip() for word in line.split(" ") if word.strip()]
             pid = words[1]
             pid_list.append(pid)
     return pid_list
 
 
 def list_ssh_tunnel(
-    path_pem_file: str,
+    path_pem_file,
     print_func: T.Callable = print,
 ):
     """
     List the SSH Tunnel processes.
 
     列出在本地机器上用特定 pem 秘钥创建的 SSH Tunnel. 其原理请参考 :func:`list_ssh_tunnel_pid`.
 
@@ -143,15 +145,15 @@
         for line in lines:
             print_func(line)
     else:
         print_func("There's NO existing SSH tunnel.")
 
 
 def kill_ssh_tunnel(
-    path_pem_file: str,
+    path_pem_file,
     verbose: bool = True,
     print_func: T.Callable = print,
 ):
     """
     Kill the SSH Tunnel processes.
 
     关闭所有在本地机器上用特定 pem 秘钥创建的 SSH Tunnel. 其原理是用
```

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/PKG-INFO` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-db-ssh-tunnel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create Database SSH Tunnel for Azerothcore World of Warcraft MySQL Database
 Home-page: https://github.com/MacHu-GWU/acore_db_ssh_tunnel-project
-Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/SOURCES.txt` & `acore_db_ssh_tunnel-0.1.3/acore_db_ssh_tunnel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/release-history.rst` & `acore_db_ssh_tunnel-0.1.3/release-history.rst`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.3 (2023-06-27)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- add ``acore_db_ssh_tunnel.api.create_engine`` to public API.
+
+**Minor Improvements**
+
+- fix type hint in ``list_ssh_tunnel`` and ``kill_ssh_tunnel``.
+
+
 0.1.2 (2023-06-16)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - Fix a bug that the ``create_ssh_tunnel`` cannot be run in Python IDE, but has to run in a terminal at the first time. Because you have to manually enter pass phrase and enter 'yes' to trust the host.
```

### Comparing `acore_db_ssh_tunnel-0.1.2/requirements-doc.txt` & `acore_db_ssh_tunnel-0.1.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.2/setup.py` & `acore_db_ssh_tunnel-0.1.3/setup.py`

 * *Files identical despite different names*

