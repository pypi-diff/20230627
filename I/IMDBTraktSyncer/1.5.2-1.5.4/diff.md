# Comparing `tmp/IMDBTraktSyncer-1.5.2.tar.gz` & `tmp/IMDBTraktSyncer-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.5.2.tar", last modified: Sun Jun 25 00:18:13 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.5.4.tar", last modified: Tue Jun 27 08:05:19 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.5.2.tar` & `IMDBTraktSyncer-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.452952 IMDBTraktSyncer-1.5.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.419464 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    35244 2023-06-24 23:28:03.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6941 2023-06-24 23:42:02.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10647 2023-06-25 00:08:47.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.449956 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.2/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-06-25 00:18:13.451940 IMDBTraktSyncer-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-06-25 00:16:59.000000 IMDBTraktSyncer-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 00:18:13.452952 IMDBTraktSyncer-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-25 00:17:18.000000 IMDBTraktSyncer-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.970382 IMDBTraktSyncer-1.5.4/
+drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.946384 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    35244 2023-06-27 07:18:11.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10647 2023-06-25 00:08:47.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.967384 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-06-27 08:05:19.969383 IMDBTraktSyncer-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-06-27 08:02:25.000000 IMDBTraktSyncer-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:05:19.970382 IMDBTraktSyncer-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-27 08:04:31.000000 IMDBTraktSyncer-1.5.4/setup.py
```

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 
                 # Count the total number of items
                 num_items = len(trakt_watchlist_to_set)
                 item_count = 0
 
                 for item in trakt_watchlist_to_set:
                     item_count += 1
+                    print(f" - Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     imdb_id = item['IMDB_ID']
                     media_type = item['Type']  # 'movie', 'show', or 'episode'
 
                     url = f"https://api.trakt.tv/sync/watchlist"
 
                     data = {
                         "movies": [],
@@ -196,17 +197,16 @@
                         data['episodes'].append({
                             "ids": {
                                 "imdb": imdb_id
                             }
                         })
 
                     response = EH.make_trakt_request(url, payload=data)
-                    if response:
-                        print(f" - Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
-                    else:
+                    
+                    if response is None:
                         error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist"
                         print(f"   - {error_message}")
                         EL.logger.error(error_message)
 
                 print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
@@ -387,14 +387,15 @@
 
                     # Count the total number of items
                     num_items = len(trakt_reviews_to_set)
                     item_count = 0
 
                     for review in trakt_reviews_to_set:
                         item_count += 1
+                        print(f" - Submitting comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                         imdb_id = review['IMDB_ID']
                         comment = review['Comment']
                         media_type = review['Type']  # 'movie', 'show', or 'episode'
 
                         url = f"https://api.trakt.tv/comments"
 
                         data = {
@@ -417,17 +418,16 @@
                             data['episode'] = {
                                 "ids": {
                                     "imdb": episode_id
                                 }
                             }
                         
                         response = EH.make_trakt_request(url, payload=data)
-                        if response:
-                            print(f" - Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
-                        else:
+                        
+                        if response is None:
                             error_message = f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt"
                             print(f"   - {error_message}")
                             EL.logger.error(error_message)
 
                     print('Trakt Reviews Set Successfully')
                 else:
                     print('No Trakt Reviews To Set')
@@ -534,15 +534,15 @@
                         }
                         print(f" - Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
 
                     # Make the API call to remove the item from the watchlist
                     response = EH.make_trakt_request(remove_url, payload=data)
 
                     if response is None:
-                        error_message = f"Error removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
+                        error_message = f"Failed removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
                         print(f"   - {error_message}")
                         EL.logger.error(error_message)
 
                 print('Removing Watched Items From Trakt Watchlist Complete')
             else:
                 print('No Watched Items To Remove From Trakt Watchlist')
```

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorHandling.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,27 +116,24 @@
     max_retries = num_retries
     status_code = None
 
     for retry in range(max_retries):
         try:
             driver.get(url)
             
-            # Wait until the page has finished loading
-            wait.until(EC.presence_of_element_located((By.TAG_NAME, 'body')))
+            # Wait until the status code becomes available
+            wait.until(lambda driver: driver.execute_script(
+                "return window.performance.getEntries().length > 0 && window.performance.getEntries()[0].responseStatus !== undefined"
+            ))
             
             # Get the HTTP status code of the page using JavaScript
             status_code = driver.execute_script(
-                """
-                var xhr = new XMLHttpRequest();
-                xhr.open('GET', window.location.href, false);
-                xhr.send(null);
-                return xhr.status;
-                """
+                "return window.performance.getEntries()[0].responseStatus;"
             )
-
+            
             # Check for any error codes
             if status_code is None:
                 return True, status_code, url  # Unable to determine page loaded status
             elif status_code >= 400:
                 raise PageLoadException(f'Failed to load page. Status code: {status_code}. URL: {url}')
             else:
                 return True, status_code, url  # Page loaded successfully
```

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.2
+Version: 1.5.4
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/LICENSE` & `IMDBTraktSyncer-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/PKG-INFO` & `IMDBTraktSyncer-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.2
+Version: 1.5.4
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.2/README.md` & `IMDBTraktSyncer-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.2/setup.py` & `IMDBTraktSyncer-1.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.2'
+VERSION = '1.5.4'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

