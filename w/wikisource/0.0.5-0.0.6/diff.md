# Comparing `tmp/wikisource-0.0.5.tar.gz` & `tmp/wikisource-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikisource-0.0.5.tar", last modified: Tue Jun 27 11:28:24 2023, max compression
+gzip compressed data, was "wikisource-0.0.6.tar", last modified: Tue Jun 27 11:51:49 2023, max compression
```

## Comparing `wikisource-0.0.5.tar` & `wikisource-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:28:24.801707 wikisource-0.0.5/
--rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.5/LICENSE
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:28:24.801747 wikisource-0.0.5/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.5/README.md
--rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 11:27:25.000000 wikisource-0.0.5/pyproject.toml
--rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 11:28:24.801922 wikisource-0.0.5/setup.cfg
--rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.5/setup.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:28:24.800036 wikisource-0.0.5/tests/
--rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.5/tests/test_chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.5/tests/test_collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.5/tests/test_wikisource.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:28:24.800836 wikisource-0.0.5/wikisource/
--rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.5/wikisource/__init__.py
--rw-r--r--   0 mathieu    (501) staff       (20)     1888 2023-06-26 22:49:59.000000 wikisource-0.0.5/wikisource/chapter.py
--rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.5/wikisource/cli.py
--rw-r--r--   0 mathieu    (501) staff       (20)      962 2023-06-26 23:04:54.000000 wikisource-0.0.5/wikisource/collection.py
--rw-r--r--   0 mathieu    (501) staff       (20)      355 2023-06-26 23:08:19.000000 wikisource-0.0.5/wikisource/paragraph.py
--rw-r--r--   0 mathieu    (501) staff       (20)     3225 2023-06-26 23:04:30.000000 wikisource-0.0.5/wikisource/source.py
--rw-r--r--   0 mathieu    (501) staff       (20)      238 2023-06-26 22:08:48.000000 wikisource-0.0.5/wikisource/webpage.py
-drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:28:24.801602 wikisource-0.0.5/wikisource.egg-info/
--rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/PKG-INFO
--rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/SOURCES.txt
--rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/dependency_links.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/entry_points.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/requires.txt
--rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 11:28:24.000000 wikisource-0.0.5/wikisource.egg-info/top_level.txt
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:51:49.244471 wikisource-0.0.6/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1074 2023-06-27 09:07:24.000000 wikisource-0.0.6/LICENSE
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:51:49.244519 wikisource-0.0.6/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)     1014 2023-06-27 09:19:30.000000 wikisource-0.0.6/README.md
+-rw-r--r--   0 mathieu    (501) staff       (20)      421 2023-06-27 11:51:22.000000 wikisource-0.0.6/pyproject.toml
+-rw-r--r--   0 mathieu    (501) staff       (20)      108 2023-06-27 11:51:49.244683 wikisource-0.0.6/setup.cfg
+-rw-r--r--   0 mathieu    (501) staff       (20)       38 2023-06-27 11:27:10.000000 wikisource-0.0.6/setup.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:51:49.242726 wikisource-0.0.6/tests/
+-rw-r--r--   0 mathieu    (501) staff       (20)      765 2023-06-27 09:02:51.000000 wikisource-0.0.6/tests/test_chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2214 2023-06-27 09:02:55.000000 wikisource-0.0.6/tests/test_collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2819 2023-06-27 09:02:57.000000 wikisource-0.0.6/tests/test_wikisource.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:51:49.243602 wikisource-0.0.6/wikisource/
+-rw-r--r--   0 mathieu    (501) staff       (20)        0 2023-06-26 17:07:46.000000 wikisource-0.0.6/wikisource/__init__.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     2565 2023-06-27 11:45:51.000000 wikisource-0.0.6/wikisource/chapter.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      878 2023-06-27 10:18:02.000000 wikisource-0.0.6/wikisource/cli.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     1923 2023-06-27 11:47:08.000000 wikisource-0.0.6/wikisource/collection.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      607 2023-06-27 11:47:37.000000 wikisource-0.0.6/wikisource/paragraph.py
+-rw-r--r--   0 mathieu    (501) staff       (20)     4149 2023-06-27 11:50:05.000000 wikisource-0.0.6/wikisource/source.py
+-rw-r--r--   0 mathieu    (501) staff       (20)      454 2023-06-27 11:50:30.000000 wikisource-0.0.6/wikisource/webpage.py
+drwxr-xr-x   0 mathieu    (501) staff       (20)        0 2023-06-27 11:51:49.244353 wikisource-0.0.6/wikisource.egg-info/
+-rw-r--r--   0 mathieu    (501) staff       (20)     1404 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu    (501) staff       (20)      484 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)        1 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       44 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/entry_points.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       13 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/requires.txt
+-rw-r--r--   0 mathieu    (501) staff       (20)       11 2023-06-27 11:51:49.000000 wikisource-0.0.6/wikisource.egg-info/top_level.txt
```

### Comparing `wikisource-0.0.5/LICENSE` & `wikisource-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/PKG-INFO` & `wikisource-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wikisource-0.0.5/README.md` & `wikisource-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/tests/test_chapter.py` & `wikisource-0.0.6/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/tests/test_collection.py` & `wikisource-0.0.6/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/tests/test_wikisource.py` & `wikisource-0.0.6/tests/test_wikisource.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/wikisource/cli.py` & `wikisource-0.0.6/wikisource/cli.py`

 * *Files identical despite different names*

### Comparing `wikisource-0.0.5/wikisource/source.py` & `wikisource-0.0.6/wikisource/source.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,23 +7,39 @@
 from dataclasses import dataclass
 
 @dataclass
 class ChapterLink:
     title: str
     url: str
 
+
 class WikiSource(WebPage):
+    """A wikisource book.
+
+    It is matching a wikisource web page which contains the table of contents of a book.
+    """
+
     def __init__(self, url, download_folder="/tmp"):
+        """Initializes a wikisource book object.
+
+        :param url: The url of the book.
+        :type url: str
+        :param download_folder: (optional) The folder where the book will be downloaded.
+        :type download_folder: str
+        """
+
         super().__init__(url)
         self.book_id = url.split('/')[-1]
         self.download_folder = download_folder
         self.download_path = f"{self.download_folder}/{self.book_id}__info.txt"
         self.chapters = list()
 
     def read(self): 
+        """Reads the book online or from the downloaded files."""
+
         self.read_info()
         self.read_chapters()
 
     def read_info(self):
         if os.path.exists(self.download_path):
             self.read_info_from_file()
         else:
@@ -72,14 +88,26 @@
             for a_tag in a_tags:
                 href = a_tag.get('href')
                 if href and href.startswith(f"/wiki/{self.book_id}") and not(re.match(r".*\.(djvu|svg).*", href)):
                     self.chapter_links.append(ChapterLink(url=f"https://fr.wikisource.org{href}", title=a_tag.text))
 
 
     def search(self, query, num_max_results=None, num_max_sentences_per_chapter=None):
+        """Search for a query in the book.
+
+        :param query: The query to search for.
+        :type query: str
+        :param num_max_results: (optional) The maximum number of results to return.
+        :type num_max_results: int
+        :param num_max_sentences_per_chapter: (optional) The maximum number of sentences to return per chapter.
+        :type num_max_sentences_per_chapter: int
+        :return: A list of results.
+        :rtype: List[SearchResult]
+        """
+
         results = list()
         for i_chap, chapter in enumerate(self.chapters):
             chapter_results = chapter.search(query)
             for i_sent, sentence in enumerate(chapter_results):
                 if ((num_max_sentences_per_chapter is None) or i_sent <= num_max_sentences_per_chapter - 1) and \
                         ((num_max_results is None) or len(results) < num_max_results):
                     chapter_link = self.chapter_links[i_chap]
```

### Comparing `wikisource-0.0.5/wikisource.egg-info/PKG-INFO` & `wikisource-0.0.6/wikisource.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikisource
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to search in books available on wikisource.org
 Author-email: "Mathieu G." <mathieu6700417@gmail.com>
 Project-URL: Homepage, https://github.com/mathieu6700417/wikisource
 Project-URL: Bug Tracker, https://github.com/mathieu6700417/wikisource/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

