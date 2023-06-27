# Comparing `tmp/mentord-1.0.7.tar.gz` & `tmp/mentord-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.0.7.tar", last modified: Tue Jun 27 11:08:55 2023, max compression
+gzip compressed data, was "mentord-1.0.8.tar", last modified: Tue Jun 27 11:10:35 2023, max compression
```

## Comparing `mentord-1.0.7.tar` & `mentord-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:08:55.405469 mentord-1.0.7/
--rw-rw-rw-   0        0        0      149 2023-06-27 11:08:55.406469 mentord-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 11:08:55.400677 mentord-1.0.7/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.7/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.7/mentord/channel.py
--rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.7/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.7/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.7/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.7/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.7/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.7/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.7/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.7/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:08:55.404194 mentord-1.0.7/mentord.egg-info/
--rw-rw-rw-   0        0        0      149 2023-06-27 11:08:55.000000 mentord-1.0.7/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 11:08:55.000000 mentord-1.0.7/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:08:55.000000 mentord-1.0.7/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 11:08:55.000000 mentord-1.0.7/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 11:08:55.406469 mentord-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      250 2023-06-27 11:08:48.000000 mentord-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:10:35.283119 mentord-1.0.8/
+-rw-rw-rw-   0        0        0      381 2023-06-27 11:10:35.283119 mentord-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 11:10:35.278121 mentord-1.0.8/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.8/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.8/mentord/channel.py
+-rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.8/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.8/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.8/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.8/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.8/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.8/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.8/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.8/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:10:35.282120 mentord-1.0.8/mentord.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-06-27 11:10:35.000000 mentord-1.0.8/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 11:10:35.000000 mentord-1.0.8/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:10:35.000000 mentord-1.0.8/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 11:10:35.000000 mentord-1.0.8/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:10:35.284527 mentord-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      295 2023-06-27 11:10:31.000000 mentord-1.0.8/setup.py
```

### Comparing `mentord-1.0.7/mentord/channel.py` & `mentord-1.0.8/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/client.py` & `mentord-1.0.8/mentord/client.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/embed.py` & `mentord-1.0.8/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/eother.py` & `mentord-1.0.8/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/guild.py` & `mentord-1.0.8/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/http_.py` & `mentord-1.0.8/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/member.py` & `mentord-1.0.8/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/message.py` & `mentord-1.0.8/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.7/mentord/user.py` & `mentord-1.0.8/mentord/user.py`

 * *Files identical despite different names*

