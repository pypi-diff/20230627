# Comparing `tmp/wikisource-0.0.8.tar.gz` & `tmp/wikisource-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikisource-0.0.8.tar", last modified: Tue Jun 27 12:00:35 2023, max compression
+gzip compressed data, was "wikisource-0.0.9.tar", last modified: Tue Jun 27 13:07:06 2023, max compression
```

## Comparing `wikisource-0.0.8.tar` & `wikisource-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.160277 wikisource-0.0.8/
--rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.8/LICENSE
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 12:00:35.160323 wikisource-0.0.8/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.8/README.md
--rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 12:00:26.000000 wikisource-0.0.8/pyproject.toml
--rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 12:00:35.160503 wikisource-0.0.8/setup.cfg
--rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.8/setup.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.158257 wikisource-0.0.8/tests/
--rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.8/tests/test_chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.8/tests/test_collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.8/tests/test_wikisource.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.159324 wikisource-0.0.8/wikisource/
--rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.8/wikisource/__init__.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2565 2023-06-27 11:57:45.000000 wikisource-0.0.8/wikisource/chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.8/wikisource/cli.py
--rw-r--r--   0 mathieu    (501) staff       (20)     1923 2023-06-27 11:47:08.000000 wikisource-0.0.8/wikisource/collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)      607 2023-06-27 11:47:37.000000 wikisource-0.0.8/wikisource/paragraph.py
--rw-r--r--   0 mathieu    (501) staff       (20)     4261 2023-06-27 12:00:09.000000 wikisource-0.0.8/wikisource/source.py
--rw-r--r--   0 mathieu    (501) staff       (20)      454 2023-06-27 11:50:30.000000 wikisource-0.0.8/wikisource/webpage.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 12:00:35.160190 wikisource-0.0.8/wikisource.egg-info/
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/SOURCES.txt
--rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/dependency_links.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/entry_points.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/requires.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 12:00:35.000000 wikisource-0.0.8/wikisource.egg-info/top_level.txt
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 13:07:06.633781 wikisource-0.0.9/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.9/LICENSE
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 13:07:06.633824 wikisource-0.0.9/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.9/README.md
+-rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 13:06:39.000000 wikisource-0.0.9/pyproject.toml
+-rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 13:07:06.633996 wikisource-0.0.9/setup.cfg
+-rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.9/setup.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 13:07:06.631978 wikisource-0.0.9/tests/
+-rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.9/tests/test_chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     1426 2023-06-27 12:10:01.000000 wikisource-0.0.9/tests/test_collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     3042 2023-06-27 13:02:34.000000 wikisource-0.0.9/tests/test_wikisource.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 13:07:06.633022 wikisource-0.0.9/wikisource/
+-rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.9/wikisource/__init__.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2565 2023-06-27 11:57:45.000000 wikisource-0.0.9/wikisource/chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.9/wikisource/cli.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     1923 2023-06-27 11:47:08.000000 wikisource-0.0.9/wikisource/collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      607 2023-06-27 11:47:37.000000 wikisource-0.0.9/wikisource/paragraph.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     4630 2023-06-27 13:06:11.000000 wikisource-0.0.9/wikisource/source.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      454 2023-06-27 11:50:30.000000 wikisource-0.0.9/wikisource/webpage.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 13:07:06.633672 wikisource-0.0.9/wikisource.egg-info/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/entry_points.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/requires.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 13:07:06.000000 wikisource-0.0.9/wikisource.egg-info/top_level.txt
```

### Comparing `wikisource-0.0.8/LICENSE` & `wikisource-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/PKG-INFO` & `wikisource-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wikisource-0.0.8/README.md` & `wikisource-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/tests/test_chapter.py` & `wikisource-0.0.9/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/tests/test_wikisource.py` & `wikisource-0.0.9/tests/test_wikisource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import unittest, os
 from wikisource.source import WikiSource
 
 sources = dict(
-    rousseau = dict(url="https://fr.wikisource.org/wiki/Les_Confessions_(Rousseau)",
-                    title="Les Confessions"),
-    nietzsche = dict(url="https://fr.wikisource.org/wiki/L%E2%80%99Origine_de_la_Trag%C3%A9die",
-                     title="L'Origine de la Tragédie"),
-    locke = dict(url="https://fr.wikisource.org/wiki/Trait%C3%A9_du_gouvernement_civil_(trad._Mazel)",
-                 title="Traité du gouvernement civil"),
-    spinoza = dict(url="https://fr.wikisource.org/wiki/Trait%C3%A9_th%C3%A9ologico-politique",
-                   title="Traité théologico-politique"),
-    descartes = dict(url="https://fr.wikisource.org/wiki/Discours_de_la_m%C3%A9thode_(%C3%A9d._Cousin)",
-                     title="Discours de la méthode"))
+    rousseau = "https://fr.wikisource.org/wiki/Les_Confessions_(Rousseau)",
+    nietzsche = "https://fr.wikisource.org/wiki/L%E2%80%99Origine_de_la_Trag%C3%A9die",
+    locke = "https://fr.wikisource.org/wiki/Trait%C3%A9_du_gouvernement_civil_(trad._Mazel)",
+    spinoza = "https://fr.wikisource.org/wiki/Trait%C3%A9_th%C3%A9ologico-politique",
+    descartes = "https://fr.wikisource.org/wiki/Discours_de_la_m%C3%A9thode_(%C3%A9d._Cousin)",
+    spinoza_2 = "https://fr.wikisource.org/wiki/Court_Traité",
+    thucydides = "https://fr.wikisource.org/wiki/Biblioth%C3%A8que_historique_et_militaire/Guerre_du_P%C3%A9loponn%C3%A8se"
+)
+
 
 class WhenUsingWikiSourceToListChapters(unittest.TestCase):
     def test_it_should_have_a_book_url(self):
-        wiki_source = WikiSource(sources["rousseau"]["url"])
-        self.assertEqual(wiki_source.url, sources["rousseau"]["url"])
+        wiki_source = WikiSource(sources["rousseau"])
+        self.assertEqual(wiki_source.url, sources["rousseau"])
 
     def test_it_should_list_all_chapters(self):
-        wiki_source = WikiSource(sources["rousseau"]["url"])
+        wiki_source = WikiSource(sources["rousseau"])
         wiki_source.read()
         self.assertEqual(len(wiki_source.chapter_links), 13)
 
     def test_it_should_have_a_title_and_an_author(self): 
-        wiki_source = WikiSource(sources["rousseau"]["url"])
+        wiki_source = WikiSource(sources["rousseau"])
         wiki_source.read()
         self.assertEqual(wiki_source.author, "Jean-Jacques Rousseau")
         self.assertEqual(wiki_source.title, "Les Confessions")
 
     def test_it_should_list_all_chapters_for_nietzsche(self):
-        wiki_source = WikiSource(sources["nietzsche"]["url"])
+        wiki_source = WikiSource(sources["nietzsche"])
         wiki_source.read()
         self.assertEqual(len(wiki_source.chapter_links), 29)
 
     def test_it_should_list_all_chapters_for_locke(self):
-        wiki_source = WikiSource(sources["locke"]["url"])
+        wiki_source = WikiSource(sources["locke"])
         wiki_source.read()
         self.assertEqual(len(wiki_source.chapter_links), 23)
 
     def test_it_should_list_all_chapters_for_spinoza(self):
-        wiki_source = WikiSource(sources["spinoza"]["url"])
+        wiki_source = WikiSource(sources["spinoza"])
         wiki_source.read()
         self.assertEqual(len(wiki_source.chapter_links), 22)
 
     def test_it_should_list_all_chapters_for_descartes(self):
-        wiki_source = WikiSource(sources["descartes"]["url"])
+        wiki_source = WikiSource(sources["descartes"])
         wiki_source.read()
         self.assertEqual(len(wiki_source.chapter_links), 6)
 
+    def test_it_should_list_all_chapters_for_spinoza_2(self):
+        wiki_source = WikiSource(sources["spinoza_2"])
+        wiki_source.read()
+        self.assertGreater(len(wiki_source.chapter_links), 0)
+
+    def test_it_should_list_all_chapters_for_thucydides(self):
+        wiki_source = WikiSource(sources["thucydides"])
+        wiki_source.read()
+        self.assertEqual(len(wiki_source.chapter_links), 10)
 
 
 class WhenUsingWikiSourceToSearch(unittest.TestCase):
     def test_it_should_return_matching_paragraphs(self):
-        wiki_source = WikiSource(sources["rousseau"]["url"])
+        wiki_source = WikiSource(sources["rousseau"])
         wiki_source.read()
         results = wiki_source.search("désir")
         self.assertEqual(len(results), 133)
         
         results = wiki_source.search("désir", num_max_sentences_per_chapter=1)
         self.assertEqual(len(results), 13)
```

### Comparing `wikisource-0.0.8/wikisource/chapter.py` & `wikisource-0.0.9/wikisource/chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/wikisource/cli.py` & `wikisource-0.0.9/wikisource/cli.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/wikisource/collection.py` & `wikisource-0.0.9/wikisource/collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/wikisource/paragraph.py` & `wikisource-0.0.9/wikisource/paragraph.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.8/wikisource/source.py` & `wikisource-0.0.9/wikisource/source.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 from bs4 import BeautifulSoup
 from .chapter import Chapter
 from .webpage import WebPage
 import json
 from dataclasses import dataclass
 from typing import Optional
+from urllib.parse import unquote
 
 @dataclass
 class ChapterLink:
     title: str
     url: str
 
 
@@ -25,17 +26,18 @@
         :param url: The url of the book.
         :type url: str
         :param download_folder: (optional) The folder where the book will be downloaded.
         :type download_folder: str
         """
 
         super().__init__(url)
-        self.book_id = url.split('/')[-1]
+        route = self.url.split('//')[1]
+        self.book_id = "/".join(route.split('/')[2:])
         self.download_folder = download_folder
-        self.download_path = f"{self.download_folder}/{self.book_id}__info.txt"
+        self.download_path = f"{self.download_folder}/{self.book_id.replace('/', '_')}_info_____.txt"
         self.chapters = list()
 
     def read(self): 
         """Reads the book online or from the downloaded files."""
 
         self.read_info()
         self.read_chapters()
@@ -84,15 +86,18 @@
         if subheader:
             subheader.decompose()
         self.chapter_links = list()
         for content_div in self.soup.find_all('div', class_='prp-pages-output'):
             a_tags = content_div.find_all('a')
             for a_tag in a_tags:
                 href = a_tag.get('href')
-                if href and href.startswith(f"/wiki/{self.book_id}") and not(re.match(r".*\.(djvu|svg).*", href)):
+                print(href and unquote(href), unquote(f"/wiki/{self.book_id}"), href and unquote(href).startswith(unquote(f"/wiki/{self.book_id}")))
+                if href and unquote(href).startswith(unquote(f"/wiki/{self.book_id}")) and \
+                        not(re.match(r".*\.(djvu|svg).*", href)) and \
+                        not unquote(href) == unquote(self.url):
                     self.chapter_links.append(ChapterLink(url=f"https://fr.wikisource.org{href}", title=a_tag.text))
 
 
     def search(self, 
                query, 
                num_max_results:Optional[int]=None, 
                num_max_sentences_per_chapter:Optional[int]=None):
```

### Comparing `wikisource-0.0.8/wikisource.egg-info/PKG-INFO` & `wikisource-0.0.9/wikisource.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

