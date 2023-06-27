# Comparing `tmp/mentord-1.0.4.tar.gz` & `tmp/mentord-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.0.4.tar", last modified: Tue Jun 27 10:53:31 2023, max compression
+gzip compressed data, was "mentord-1.0.5.tar", last modified: Tue Jun 27 10:54:16 2023, max compression
```

## Comparing `mentord-1.0.4.tar` & `mentord-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:53:31.745160 mentord-1.0.4/
--rw-rw-rw-   0        0        0      396 2023-06-27 10:53:31.745160 mentord-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 10:53:31.740158 mentord-1.0.4/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.4/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.4/mentord/channel.py
--rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.4/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.4/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.4/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.4/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.4/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.4/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.4/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.4/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:53:31.744158 mentord-1.0.4/mentord.egg-info/
--rw-rw-rw-   0        0        0      396 2023-06-27 10:53:31.000000 mentord-1.0.4/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 10:53:31.000000 mentord-1.0.4/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:53:31.000000 mentord-1.0.4/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 10:53:31.000000 mentord-1.0.4/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 10:53:31.746209 mentord-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      386 2023-06-27 10:53:13.000000 mentord-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:54:16.826618 mentord-1.0.5/
+-rw-rw-rw-   0        0        0      381 2023-06-27 10:54:16.826618 mentord-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 10:54:16.821598 mentord-1.0.5/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.5/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.5/mentord/channel.py
+-rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.5/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.5/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.5/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.5/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.5/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.5/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.5/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.5/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:54:16.825595 mentord-1.0.5/mentord.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-06-27 10:54:16.000000 mentord-1.0.5/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 10:54:16.000000 mentord-1.0.5/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:54:16.000000 mentord-1.0.5/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 10:54:16.000000 mentord-1.0.5/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:54:16.827616 mentord-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      386 2023-06-27 10:54:09.000000 mentord-1.0.5/setup.py
```

### Comparing `mentord-1.0.4/mentord/channel.py` & `mentord-1.0.5/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/client.py` & `mentord-1.0.5/mentord/client.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/embed.py` & `mentord-1.0.5/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/eother.py` & `mentord-1.0.5/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/guild.py` & `mentord-1.0.5/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/http_.py` & `mentord-1.0.5/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/member.py` & `mentord-1.0.5/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/message.py` & `mentord-1.0.5/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.4/mentord/user.py` & `mentord-1.0.5/mentord/user.py`

 * *Files identical despite different names*

