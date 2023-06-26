# Comparing `tmp/datahtml-0.4.0rc4.tar.gz` & `tmp/datahtml-0.4.0rc5.tar.gz`

## Comparing `datahtml-0.4.0rc4.tar` & `datahtml-0.4.0rc5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/_utils.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/base.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/crawler.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/defaults.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/google.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/google_trends.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/news.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/parsers.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/sitemap.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/types.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/web.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/apis/__init__.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/datahtml/apis/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/api_reference.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/conf.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/make.bat
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/api/crawler.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/api/sitemap.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/api/types.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/docs/api/web.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/google_search.html
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/google_trends_rss.xml
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/test_apis_youtube.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/test_google.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/test_google_trends.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_search.html
--rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_search_response.json
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_video.json
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_video_multiple_ids.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/tests/youtube_video_response.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/pyproject.toml
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/_utils.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/base.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/crawler.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/defaults.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/google.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/google_trends.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/news.py
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/parsers.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/rss.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/sitemap.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/types.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/web.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/google_search.html
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/google_trends_rss.xml
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/test_google.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/test_google_trends.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 datahtml-0.4.0rc5/PKG-INFO
```

### Comparing `datahtml-0.4.0rc4/.pylintrc` & `datahtml-0.4.0rc5/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/crawler.py` & `datahtml-0.4.0rc5/datahtml/crawler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 import os
 from typing import Any, Dict, Optional
 
 import httpx
 
-from datahtml import errors
+from datahtml import errors, types
 from datahtml.base import CrawlerSpec, CrawlResponse
+from datahtml.parsers import proxyconf2url
 
 # import traceback
 
 
 class LocalCrawler(CrawlerSpec):
     def get(
-        self, url, headers: Optional[Dict[str, Any]] = {}, timeout_secs: int = 60
+        self,
+        url,
+        headers: Optional[Dict[str, Any]] = None,
+        timeout_secs: int = 60,
+        proxy: Optional[types.ProxyConf] = None,
     ) -> CrawlResponse:
 
+        client = httpx.Client(
+            headers=headers, timeout=timeout_secs, follow_redirects=True
+        )
+        if proxy:
+            proxy_url = proxyconf2url(proxy)
+            client = httpx.Client(
+                headers=headers,
+                timeout=timeout_secs,
+                follow_redirects=True,
+                proxies={"all://": proxy_url},
+            )
+
         try:
-            r = httpx.get(
+            r = client.get(
                 url, headers=headers, timeout=timeout_secs, follow_redirects=True
             )
             rsp = CrawlResponse(
-                url=url, headers=r.headers, status_code=r.status_code, content=r.content
+                url=url,
+                headers=dict(r.headers),
+                status_code=r.status_code,
+                content=r.content,
             )
             return rsp
         except httpx.HTTPError as e:
             # err = traceback.format_exc()
             raise errors.CrawlHTTPError(str(e))
 
 
@@ -37,15 +57,19 @@
         :param token: token to be used for the crawler
         """
         self._url = url or os.getenv("AXIOS_URL")
         self._token = token or os.getenv("AXIOS_TOKEN")
         self._headers = {"Authorization": f"Bearer {self._token}"}
 
     def get(
-        self, url, headers: Optional[Dict[str, Any]] = {}, timeout_secs: int = 60
+        self,
+        url,
+        headers: Optional[Dict[str, Any]] = None,
+        timeout_secs: int = 60,
+        proxy: Optional[types.ProxyConf] = None,
     ) -> CrawlResponse:
         # TODO: fix if something fail on the crawler service
 
         try:
             r = httpx.post(
                 self._url,
                 data={"url": url, "headers": headers},
```

### Comparing `datahtml-0.4.0rc4/datahtml/defaults.py` & `datahtml-0.4.0rc5/datahtml/defaults.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/errors.py` & `datahtml-0.4.0rc5/datahtml/errors.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/google.py` & `datahtml-0.4.0rc5/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/google_trends.py` & `datahtml-0.4.0rc5/datahtml/google_trends.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/news.py` & `datahtml-0.4.0rc5/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/parsers.py` & `datahtml-0.4.0rc5/datahtml/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,7 +220,15 @@
     keywords = ""
     for d in data:
         if d.get("property"):
             if d["property"] == "keywords":
                 keywords = d["content"]
                 break
     return keywords
+
+def proxyconf2url(p: types.ProxyConf) -> str:
+    url = p.server
+    if p.username:
+        parsed = urlparse(p.server)
+        url = f"{parsed.scheme}://{p.username}:{p.password}@{parsed.netloc}"
+    return url
+
```

### Comparing `datahtml-0.4.0rc4/datahtml/rss.py` & `datahtml-0.4.0rc5/datahtml/rss.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/sitemap.py` & `datahtml-0.4.0rc5/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/web.py` & `datahtml-0.4.0rc5/datahtml/web.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/youtube.py` & `datahtml-0.4.0rc5/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/datahtml/apis/youtube.py` & `datahtml-0.4.0rc5/datahtml/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/docs/Makefile` & `datahtml-0.4.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/docs/conf.py` & `datahtml-0.4.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/docs/index.rst` & `datahtml-0.4.0rc5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/docs/make.bat` & `datahtml-0.4.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/google_search.html` & `datahtml-0.4.0rc5/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/google_trends_rss.xml` & `datahtml-0.4.0rc5/tests/google_trends_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/lanacion_article.html` & `datahtml-0.4.0rc5/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc5/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/test_apis_youtube.py` & `datahtml-0.4.0rc5/tests/test_apis_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/test_youtube.py` & `datahtml-0.4.0rc5/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_channel.html` & `datahtml-0.4.0rc5/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc5/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_search.html` & `datahtml-0.4.0rc5/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_search_response.json` & `datahtml-0.4.0rc5/tests/youtube_search_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_video.html` & `datahtml-0.4.0rc5/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_video.json` & `datahtml-0.4.0rc5/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_video_multiple_ids.json` & `datahtml-0.4.0rc5/tests/youtube_video_multiple_ids.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/tests/youtube_video_response.json` & `datahtml-0.4.0rc5/tests/youtube_video_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/.gitignore` & `datahtml-0.4.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/LICENSE` & `datahtml-0.4.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/README.md` & `datahtml-0.4.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc4/pyproject.toml` & `datahtml-0.4.0rc5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 	"lxml~=4.6.3",
 	"ujson~=4.2.0",
 	"extruct~=0.13.0",
 	"feedparser~=6.0.8",
 	# "reppy~=0.4.14",
 	"newspaper3k~=0.2.8",
 	"httpx~=0.23.0",
-    "pydantic~=1.10.7"
+    	"pydantic~=1.10.7",
+	"attrs~=23.1.0",
         
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/algorinfo/datahtml#readme"
 Issues = "https://github.com/algorinfo/datahtml/issues"
```

### Comparing `datahtml-0.4.0rc4/PKG-INFO` & `datahtml-0.4.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.4.0rc4
+Version: 0.4.0rc5
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: attrs~=23.1.0
 Requires-Dist: beautifulsoup4~=4.10.0
 Requires-Dist: extruct~=0.13.0
 Requires-Dist: feedparser~=6.0.8
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: lxml~=4.6.3
 Requires-Dist: newspaper3k~=0.2.8
 Requires-Dist: pydantic~=1.10.7
```

