# Comparing `tmp/mentord-1.0.2.tar.gz` & `tmp/mentord-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.0.2.tar", last modified: Tue Jun 27 10:06:54 2023, max compression
+gzip compressed data, was "mentord-1.0.3.tar", last modified: Tue Jun 27 10:46:33 2023, max compression
```

## Comparing `mentord-1.0.2.tar` & `mentord-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.026118 mentord-1.0.2/
--rw-rw-rw-   0        0        0       95 2023-06-27 10:06:54.027115 mentord-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.022118 mentord-1.0.2/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.2/mentord/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.2/mentord/channel.py
--rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.2/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.2/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.2/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.2/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.2/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.2/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.2/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.2/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:06:54.026118 mentord-1.0.2/mentord.egg-info/
--rw-rw-rw-   0        0        0       95 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 10:06:53.000000 mentord-1.0.2/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 10:06:54.027115 mentord-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      159 2023-06-27 10:06:15.000000 mentord-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:46:33.442469 mentord-1.0.3/
+-rw-rw-rw-   0        0        0      355 2023-06-27 10:46:33.442469 mentord-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 10:46:33.437471 mentord-1.0.3/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-27 09:45:09.000000 mentord-1.0.3/mentord/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 09:58:00.000000 mentord-1.0.3/mentord/channel.py
+-rw-rw-rw-   0        0        0     2840 2023-06-27 10:06:38.000000 mentord-1.0.3/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.0.3/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.0.3/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.0.3/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.0.3/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.0.3/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.0.3/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.0.3/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:46:33.441470 mentord-1.0.3/mentord.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-06-27 10:46:33.000000 mentord-1.0.3/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-27 10:46:33.000000 mentord-1.0.3/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:46:33.000000 mentord-1.0.3/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 10:46:33.000000 mentord-1.0.3/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:46:33.443470 mentord-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      386 2023-06-27 10:46:01.000000 mentord-1.0.3/setup.py
```

### Comparing `mentord-1.0.2/mentord/channel.py` & `mentord-1.0.3/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/client.py` & `mentord-1.0.3/mentord/client.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/embed.py` & `mentord-1.0.3/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/eother.py` & `mentord-1.0.3/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/guild.py` & `mentord-1.0.3/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/http_.py` & `mentord-1.0.3/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/member.py` & `mentord-1.0.3/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/message.py` & `mentord-1.0.3/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.0.2/mentord/user.py` & `mentord-1.0.3/mentord/user.py`

 * *Files identical despite different names*

