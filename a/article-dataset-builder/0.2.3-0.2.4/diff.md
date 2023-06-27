# Comparing `tmp/article_dataset_builder-0.2.3.tar.gz` & `tmp/article_dataset_builder-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_dataset_builder-0.2.3.tar", last modified: Tue Mar  7 15:09:17 2023, max compression
+gzip compressed data, was "article_dataset_builder-0.2.4.tar", last modified: Tue Jun 27 18:31:43 2023, max compression
```

## Comparing `article_dataset_builder-0.2.3.tar` & `article_dataset_builder-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 15:09:17.850374 article_dataset_builder-0.2.3/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.3/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.3/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25864 2023-03-07 15:09:17.850374 article_dataset_builder-0.2.3/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25305 2023-03-05 14:50:16.000000 article_dataset_builder-0.2.3/Readme.md
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 15:09:17.850374 article_dataset_builder-0.2.3/article_dataset_builder/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.3/article_dataset_builder/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.3/article_dataset_builder/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.3/article_dataset_builder/check_cord19_coverage.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    84523 2023-03-07 15:08:49.000000 article_dataset_builder-0.2.3/article_dataset_builder/harvest.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6700 2023-03-07 15:08:08.000000 article_dataset_builder-0.2.3/article_dataset_builder/nlm2tei.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 15:09:17.850374 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25864 2023-03-07 15:09:17.000000 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-03-07 15:09:17.000000 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-03-07 15:09:17.000000 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-03-07 15:09:17.000000 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-03-07 15:09:17.000000 article_dataset_builder-0.2.3/article_dataset_builder.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-05 17:44:54.000000 article_dataset_builder-0.2.3/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-03-05 14:33:42.000000 article_dataset_builder-0.2.3/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-03-07 15:09:17.850374 article_dataset_builder-0.2.3/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      978 2023-03-07 15:08:55.000000 article_dataset_builder-0.2.3/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.4/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.4/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25390 2023-06-27 18:24:00.000000 article_dataset_builder-0.2.4/Readme.md
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/article_dataset_builder/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.4/article_dataset_builder/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.4/article_dataset_builder/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.4/article_dataset_builder/check_cord19_coverage.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    85040 2023-06-27 18:28:07.000000 article_dataset_builder-0.2.4/article_dataset_builder/harvest.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6700 2023-03-07 15:08:08.000000 article_dataset_builder-0.2.4/article_dataset_builder/nlm2tei.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-07 16:15:48.000000 article_dataset_builder-0.2.4/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-03-05 14:33:42.000000 article_dataset_builder-0.2.4/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      978 2023-06-27 16:39:57.000000 article_dataset_builder-0.2.4/setup.py
```

### Comparing `article_dataset_builder-0.2.3/LICENSE` & `article_dataset_builder-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.3/PKG-INFO` & `article_dataset_builder-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article_dataset_builder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -97,18 +97,18 @@
 
 ```sh
 python3 -m pip  install -e .
 ```
 
 #### Using PyPI package
 
-PyPI packages are available for stable versions. Latest stable version is `0.2.1`:
+PyPI packages are available for stable versions. Latest stable version is normally `0.2.4`, but double check [here](https://pypi.org/project/article-dataset-builder/):
 
 ```
-python3 -m pip install article-dataset-builder==0.2.1
+python3 -m pip install article-dataset-builder==0.2.4
 ```
 
 ### Third party web services
 
 Depending on the process you are interested to apply to the articles as they are harvested, the following tools need to be installed/accessed and running, with access information specified in the configuration file (`config.json`):
 
 - [biblio-glutton](https://github.com/kermitt2/biblio-glutton), for metadata retrieval and aggregation
```

### Comparing `article_dataset_builder-0.2.3/Readme.md` & `article_dataset_builder-0.2.4/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,18 +81,18 @@
 
 ```sh
 python3 -m pip  install -e .
 ```
 
 #### Using PyPI package
 
-PyPI packages are available for stable versions. Latest stable version is `0.2.1`:
+PyPI packages are available for stable versions. Latest stable version is normally `0.2.4`, but double check [here](https://pypi.org/project/article-dataset-builder/):
 
 ```
-python3 -m pip install article-dataset-builder==0.2.1
+python3 -m pip install article-dataset-builder==0.2.4
 ```
 
 ### Third party web services
 
 Depending on the process you are interested to apply to the articles as they are harvested, the following tools need to be installed/accessed and running, with access information specified in the configuration file (`config.json`):
 
 - [biblio-glutton](https://github.com/kermitt2/biblio-glutton), for metadata retrieval and aggregation
```

### Comparing `article_dataset_builder-0.2.3/article_dataset_builder/S3.py` & `article_dataset_builder-0.2.4/article_dataset_builder/S3.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.3/article_dataset_builder/check_cord19_coverage.py` & `article_dataset_builder-0.2.4/article_dataset_builder/check_cord19_coverage.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.3/article_dataset_builder/harvest.py` & `article_dataset_builder-0.2.4/article_dataset_builder/harvest.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from tqdm import tqdm
 import logging
 import logging.handlers
 import cloudscraper
 from bs4 import BeautifulSoup
 from random import randint, choices
 
-
 map_size = 100 * 1024 * 1024 * 1024 
 logging.basicConfig(filename='harvester.log', filemode='w', level=logging.INFO)
 
 urllib3.disable_warnings()
 
 scraper = cloudscraper.create_scraper(interpreter='nodejs')
 
@@ -1131,16 +1130,18 @@
         except IOError as e:
             logging.error("temporary file cleaning failed: " + str(e))    
 
     def getUUIDByStrongIdentifier(self, strong_identifier):
         """
         Strong identifiers depend on the data to be processed but typically includes DOI, sha, PMID, PMCID
         """
-        txn = self.env_uuid.begin()
-        return txn.get(strong_identifier.encode(encoding='UTF-8'))
+        uuid = None
+        with self.env_uuid.begin() as txn:
+            uuid = txn.get(strong_identifier.encode(encoding='UTF-8'))
+        return uuid
 
     def diagnostic(self, full=False, metadata_csv_file=None, cord19=False):
         """
         Print a report on failures stored during the harvesting process
         """
         nb_total = 0
         nb_invalid_oa_url = 0
@@ -1415,14 +1416,15 @@
     is harvested - but in our case we are harvesting a large variety of different Open Access servers
     '''
     user_agents = ["Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:81.0) Gecko/20100101 Firefox/81.0",
                    "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.81 Safari/537.36",
                    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36"]
     weights = [0.2, 0.3, 0.5]
     user_agent = choices(user_agents, weights=weights, k=1)
+    return user_agent[0]
 
 def _is_valid_file(file, mime_type):
     target_mime = []
     if mime_type == 'xml':
         target_mime.append("application/xml")
         target_mime.append("text/xml")
     elif mime_type == 'png':
@@ -1460,26 +1462,37 @@
     the_url = 'http://'+grobid_base
     if grobid_port is not None and len(grobid_port)>0:
         the_url += ":"+grobid_port
     the_url += "/api/"
     return the_url
 
 def _download(url, filename):
-    #result = _download_wget(url, filename)
-    try:
-        result = _download_cloudscraper(url, filename)
-    except:
-        logging.debug("_download_cloudscraper failed for " + url)
-    if result != "success":
-        if str(url).startswith("ftp"):
+    result = "fail"
+    if str(url).startswith("ftp"):  
+        result = _download_wget(url, filename)
+        if result != "success":
+            # this appears to be not reliable at all with lot of decompression errors
+            # but as last options why not
             result = _download_ftp(url, filename)
-            # if result != "success":
-            #     result = _download_wget(url, filename)
-        else:
-            result = _download_requests(url, filename)
+
+    if result != "success":
+        # note: cloudscraper does not support ftp
+        # to be checked for compressed file
+        try:
+            result = _download_cloudscraper(url, filename)
+        except:
+            logging.debug("_download_cloudscraper failed for " + url)
+    
+    # the following supports decompression well, but it is not very reliable
+    if result != "success":
+        result = _download_requests(url, filename)
+
+    if result != "success" and not str(url).startswith("ftp"):
+        result = _download_wget(url, filename)
+    
     return result
 
 def _download_cloudscraper(url, filename: str, n=0, timeout_in_seconds=30):
     """
     Use a cloudscraper session for downloading Cloudflare protected file. 
     Header agant generation is managed by cloudscraper.
     Websites not using Cloudflare will be treated like normal requests call. 
@@ -1512,27 +1525,28 @@
         logging.debug("Download failed for {0} with cloudscraper".format(url))
     except InvalidSchema:
         logging.debug("Download failed (invalid schema) for {0} with cloudscraper".format(url))
     return result
 
 def _download_wget(url, filename):
     """ 
-    First try with Python requests (which handle well compression), then move to a more robust download approach
+    This is the most reliable download solution I found, but it does not handle well decompression (depending how the 
+    local wget was compiled)
     """
     result = "fail"
     # This is the most robust and reliable way to download files I found with Python... to rely on system wget :)
     #cmd = "wget -c --quiet" + " -O " + filename + ' --connect-timeout=10 --waitretry=10 ' + \
 
     cmd = "wget -c --quiet" + " -O " + filename + ' --timeout=15 --waitretry=0 --tries=5 --retry-connrefused ' + \
-        '--header="User-Agent: ' + _get_random_user_agent()+ '" ' + \
+        '--header="User-Agent: ' + _get_random_user_agent() + '" ' + \
         '--header="Accept: application/pdf, text/html;q=0.9,*/*;q=0.8" --header="Accept-Encoding: gzip, deflate" ' + \
         '--no-check-certificate ' + \
         '"' + url + '"'
 
-    logging.debug(cmd)
+    #logging.debug(cmd)
     try:
         result = subprocess.check_call(cmd, shell=True)
         
         # if the used version of wget does not decompress automatically, the following ensures it is done
         result_compression = _check_compression(filename)
         if not result_compression:
             # decompression failed, or file is invalid
```

### Comparing `article_dataset_builder-0.2.3/article_dataset_builder/nlm2tei.py` & `article_dataset_builder-0.2.4/article_dataset_builder/nlm2tei.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.3/article_dataset_builder.egg-info/PKG-INFO` & `article_dataset_builder-0.2.4/article_dataset_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-dataset-builder
-Version: 0.2.3
+Version: 0.2.4
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -97,18 +97,18 @@
 
 ```sh
 python3 -m pip  install -e .
 ```
 
 #### Using PyPI package
 
-PyPI packages are available for stable versions. Latest stable version is `0.2.1`:
+PyPI packages are available for stable versions. Latest stable version is normally `0.2.4`, but double check [here](https://pypi.org/project/article-dataset-builder/):
 
 ```
-python3 -m pip install article-dataset-builder==0.2.1
+python3 -m pip install article-dataset-builder==0.2.4
 ```
 
 ### Third party web services
 
 Depending on the process you are interested to apply to the articles as they are harvested, the following tools need to be installed/accessed and running, with access information specified in the configuration file (`config.json`):
 
 - [biblio-glutton](https://github.com/kermitt2/biblio-glutton), for metadata retrieval and aggregation
```

### Comparing `article_dataset_builder-0.2.3/config.json` & `article_dataset_builder-0.2.4/config.json`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.3/setup.py` & `article_dataset_builder-0.2.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="article_dataset_builder",
-    version="0.2.3",
+    version="0.2.4",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="Open Access scholar PDF harvester, metadata aggregator and full-text ingester",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/kermitt2/article_dataset_builder",
     packages=find_packages(exclude=['test', '*.test', '*.test.*']),
```

