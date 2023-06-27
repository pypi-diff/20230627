# Comparing `tmp/clld_document_plugin-0.0.4.tar.gz` & `tmp/clld_document_plugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clld_document_plugin-0.0.4.tar", last modified: Mon Nov 28 00:42:33 2022, max compression
+gzip compressed data, was "dist/clld_document_plugin-0.0.5.tar", last modified: Tue Jun 27 21:08:55 2023, max compression
```

## Comparing `clld_document_plugin-0.0.4.tar` & `clld_document_plugin-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      405 2022-11-28 00:42:08.000000 clld_document_plugin-0.0.4/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-06-02 21:28:29.000000 clld_document_plugin-0.0.4/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2022-11-07 15:38:09.000000 clld_document_plugin-0.0.4/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1051 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)      147 2022-06-03 21:34:22.000000 clld_document_plugin-0.0.4/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      519 2022-06-02 21:28:29.000000 clld_document_plugin-0.0.4/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1744 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-06-02 21:28:29.000000 clld_document_plugin-0.0.4/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5294 2022-11-28 00:41:52.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/__init__.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)      186 2022-06-03 02:11:56.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/datatables.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)      122 2022-11-22 19:55:46.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/interfaces.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1041 2022-11-22 19:55:46.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/models.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1123 2022-11-01 17:34:55.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-chapter.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      202 2022-08-25 09:05:00.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-document.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5186 2022-11-06 17:28:47.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-document.js
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     8087 2022-09-17 16:19:30.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-slides.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      795 2022-09-17 16:19:30.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-slides.js
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1189 2022-11-03 00:49:18.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/chapter.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      415 2022-11-06 17:34:57.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/detail_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      249 2022-06-02 19:04:41.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/index_html.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1379 2022-09-17 16:19:30.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/slides.mako
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1180 2022-11-22 19:55:46.000000 clld_document_plugin-0.0.4/src/clld_document_plugin/util.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1051 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1022 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      230 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       21 2022-11-28 00:42:33.000000 clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      405 2023-06-27 21:08:26.000000 clld_document_plugin-0.0.5/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2023-06-27 18:56:36.000000 clld_document_plugin-0.0.5/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2023-06-27 18:56:37.000000 clld_document_plugin-0.0.5/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1051 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/PKG-INFO
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      147 2023-06-27 18:56:36.000000 clld_document_plugin-0.0.5/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      519 2023-06-27 18:56:36.000000 clld_document_plugin-0.0.5/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1744 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2023-06-27 18:56:36.000000 clld_document_plugin-0.0.5/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6669 2023-06-27 21:08:15.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      378 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/datatables.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      204 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/interfaces.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1546 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/models.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1168 2023-06-27 21:07:27.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-chapter.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      202 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-document.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5753 2023-06-27 21:07:27.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-document.js
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     8087 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-slides.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      795 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-slides.js
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1185 2023-06-27 21:07:27.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/chapter.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      415 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      249 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/index_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1362 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/slides.mako
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/topic/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      829 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/topic/detail_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      243 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/templates/topic/index_html.mako
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1180 2023-06-27 18:58:07.000000 clld_document_plugin-0.0.5/src/clld_document_plugin/util.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1051 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1137 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      230 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       21 2023-06-27 21:08:55.000000 clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/top_level.txt
```

### Comparing `clld_document_plugin-0.0.4/LICENSE` & `clld_document_plugin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clld_document_plugin-0.0.4/PKG-INFO` & `clld_document_plugin-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld_document_plugin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Document model and rendering in CLLD apps.
 Home-page: https://github.com/fmatter/clld-document-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-document-plugin/issues
 Keywords: clld,linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_document_plugin-0.0.4/pyproject.toml` & `clld_document_plugin-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clld_document_plugin-0.0.4/setup.cfg` & `clld_document_plugin-0.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	linguistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = clld_document_plugin
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/clld-document-plugin/issues
 url = https://github.com/fmatter/clld-document-plugin
-version = 0.0.4
+version = 0.0.5
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/__init__.py` & `clld_document_plugin-0.0.5/src/clld_document_plugin/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Top-level package for clld-document-plugin."""
 import re
 from clld.db.models import Sentence
+from clld.db.models import common
 from clld.web.util.htmllib import HTML
+from clld.web.util.helpers import link
 from clld_corpus_plugin.util import rendered_sentence
 from markdown.extensions.toc import TocExtension
 from clld_document_plugin import datatables
 from clld_document_plugin import interfaces
 from clld_document_plugin import models
+from clld_markdown_plugin import link_entity
 
 
 __author__ = "Florian Matter"
 __email__ = "florianmatter@gmail.com"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 glossing_delimiters = [
     "-",
     "–",
     ".",
     "=",
     ";",
@@ -94,14 +97,26 @@
                             output += decoration(gloss.lower())
                 else:
                     output += part
         words_list[i] = output[1:]
     gloss_text_upcased = " ".join(words_list)
     return gloss_text_upcased
 
+def render_sources(req, objid, table, session, ids=None, **kwargs):
+    if "full" in kwargs:
+        source = session.query(common.Source).filter(common.Source.id == objid)[0]
+        return link(req, source, label=source.bibtex().text())
+    return link_entity(
+                        req,
+                        objid,
+                        "source",
+                        common.Source,
+                        session,
+                    )
+
 
 def render_ex(
     req, objid, table, session, ids=None, subexample=False, **kwargs
 ):  # pylint: disable=too-many-arguments
     if "subexample" in kwargs.get("format", []):
         subexample = True
     example_id = kwargs.get("example_id", [None])[0]
@@ -140,14 +155,20 @@
             counter_class="example",
             title=title,
         ),
         class_="example",
     )
 
 
+def render_abbrev_list(req, objid, table, session, ids=None, **kwargs):
+    abbrev_items = []
+    for abbrev in session.query(common.GlossAbbreviation).all():
+        abbrev_items.append(HTML.tr(HTML.td(abbrev.id), HTML.td(abbrev.name)))
+    return HTML.table(HTML.tbody(*abbrev_items), **{"class": "table table-nonfluid"})
+
 def includeme(config):
 
     config.registry.settings["mako.directories"].insert(
         1, "clld_document_plugin:templates"
     )
     config.registry.settings["clld_markdown_plugin"]["extensions"].extend(
         [
@@ -157,16 +178,26 @@
             "markdown.extensions.footnotes",
             "pymdownx.tilde",
         ]
     )
     config.registry.settings["clld_markdown_plugin"]["renderer_map"][
         "ExampleTable"
     ] = render_ex
-    config.registry.settings["clld_markdown_plugin"]["model_map"]["ChapterTable"] = {"route": "document", "model": models.Document}
+    config.registry.settings["clld_markdown_plugin"]["model_map"]["ChapterTable"] = {
+        "route": "document",
+        "model": models.Document,
+    }
+
+    config.registry.settings["clld_markdown_plugin"]["renderer_map"]["abbreviations.csv"] = render_abbrev_list
+
+    config.registry.settings["clld_markdown_plugin"]["renderer_map"]["sources.bib"] = render_sources
+    config.registry.settings["clld_markdown_plugin"]["renderer_map"]["Source"] = render_sources
 
     config.add_static_view("clld-document-plugin-static", "clld_document_plugin:static")
 
     config.register_resource(
         "document", models.Document, interfaces.IDocument, with_index=True
     )
+    config.register_resource("topic", models.Topic, interfaces.ITopic, with_index=True)
 
+    config.register_datatable("topics", datatables.Topics)
     config.register_datatable("documents", datatables.Documents)
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-chapter.css` & `clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-chapter.css`

 * *Files 9% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 
 article tbody {
     border-bottom: 2px solid black;
 }
 
 article table {
   border-collapse: collapse;*/
-display: inline;
-border-spacing: 0px 0px;
-margin: 0 auto;
+  display: inline;
+  border-spacing: 0px 0px;
+  margin: 0 auto;
 }
 
 article td {
     vertical-align: top;
 }
 
 article th, td {
-    padding: 0.4em;
+    padding: 0.1em;
+    padding-inline: 0.3em;
 }
+
 ol table {
   border-collapse: collapse;*/
   border-spacing: 0px 0px;
-display: inline;
-margin:4px;
-margin: 0 auto;
+  display: inline;
+  margin:4px;
+  margin: 0 auto;
 }
 
 ol thead {
     border-bottom: 0px;
     border-top: 0px;
 }
 
@@ -38,18 +40,18 @@
     font-weight: normal;
 }
 
 ol tbody {
     border-bottom: 0px;
 }
 
-
 html {
     scroll-padding-top: 40px;
 }
+
 article {
     width: 50em;
     /*margin: 0 auto;*/
     margin-left: 10em;
     max-width: 100%;
     line-height: 1.5;
     text-align: justify;
@@ -62,25 +64,26 @@
     /*width: 40em;*/
     /*font-size: 90%;*/
     top: 3.5em;
     right: 1em;
 }
 
 
-
 article h1 {
   font-size: 1.5em;
 }
+
 article h2 {
   font-size: 1.17em !important;
 }
+
 article h3 {
   font-size: 1em;
 }
 
 div.caption {
     display: table;
     margin: auto;
-text-align: center;
+    text-align: center;
 }
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-document.js` & `clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-document.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-function number_examples() {
+function numberExamples() {
     var examples = document.querySelectorAll("li.example"); // select all examples
     for (var exc = 0; exc < examples.length; exc++) {
         ex = examples[exc]
         ex.setAttribute("value", exc + 1) // number each example
         var subexamplesol = ex.querySelector("ol.subexample");
         if (subexamplesol) { // if there are subexamples, number them example-internally
             subexamples = subexamplesol.children
@@ -12,53 +12,55 @@
         }
     }
 
     var exrefs = document.querySelectorAll("a.exref"); // get all links that are references to examples
     exrefs.forEach(function(x, i) {
         example_id = x.getAttribute("example_id")
         x.setAttribute("href", "#" + example_id) // point the link to the example
-        x.textContent = "(" + get_example_label(example_id) // get_example_label returns labels like 1 or 2b
+        x.textContent = getExampleLabel(example_id) // getExampleLabel returns labels like 1 or 2b
         if (x.hasAttribute("end")) { // for exrefs of the form (10-12)
             end = x.getAttribute("end")
-            x.textContent += "-" + get_example_label(end)
+            x.textContent += "-" + getExampleLabel(end)
         }
         if (x.hasAttribute("suffix")) { // for exrefs of the form (10a-b)
             x.textContent += x.getAttribute("suffix")
         }
-        x.textContent += ")" // wrap it up
+        if (!x.hasAttribute("bare")) {
+            x.textContent = "(" + x.textContent + ")" // wrap it up in parentheses (or not!)
+        }
     });
 }
 
 
-function get_example_label(example_id) {
+function getExampleLabel(example_id) {
     ex = document.getElementById(example_id)
     if (ex == null) {
         console.log("Could not find example with ID " + example_id);
         return "undefined"
     }
     parent = ex.parentElement
     if (parent.getAttribute("class") == "subexample") {
         return parent.parentElement.value + String.fromCharCode(96 + ex.value) // convert to alphabetical labels
     }
     return ex.value
 }
 
 // returns strings like 3. or 4.3.2
-function get_number_label(counters, level) {
+function getNumberLabel(counters, level) {
     output = []
     for (var i = 2; i <= level; i++) {
         output.push(counters["h" + i])
     }
     return output.join(".")
 }
 
 //used for storing both section labels and float counters
 var stored = {}
 
-function number_sections() {
+function numberSections() {
     var toc = document.getElementById("toc") // get the table of contents
     var counters = {}; // initialize counters for every heading level except h1 (below)
     var levels = ["h2", "h3", "h4", "h5", "h6"];
     levels.forEach(function(x, i) {
         counters[x] = 0
     })
 
@@ -77,15 +79,15 @@
     toc.appendChild(toctitle)
 
     // iterate all headings
     var headings = document.querySelectorAll("h2, h3, h4, h5, h6");
     headings.forEach(function(heading, i) {
         var level = heading.tagName.toLowerCase();
         counters[level] += 1
-        number = get_number_label(counters, level.charAt(level.length - 1)) // the formatted X.Y.Z counter
+        number = getNumberLabel(counters, level.charAt(level.length - 1)) // the formatted X.Y.Z counter
         heading.textContent = prefix + number + ". " + heading.textContent
 
         toclink = document.createElement('a') // insert links into the TOC
         toclink.textContent = '\xa0\xa0'.repeat(level.charAt(level.length - 1) - 2) + heading.textContent
         toclink.href = "#" + heading.id
         tocdiv = document.createElement('div')
         tocdiv.appendChild(toclink);
@@ -107,35 +109,44 @@
 }
 
 
 function capitalizeFirstLetter(string) {
     return string.charAt(0).toUpperCase() + string.slice(1);
 }
 
-function number_captions() {
+function numberCaptions() {
     var captions = document.querySelectorAll("div.caption"); // get all captions
+    var figcaptions = document.querySelectorAll("figcaption"); // get all captions
     var kinds = ["table", "figure"] // only these two types for now
     var counters = {
         "table": 0,
         "figure": 0
     }
     captions.forEach(function(caption, i) {
         kinds.forEach(function(kind, j) {
             if (caption.classList.contains(kind)) {
                 counters[kind] += 1
                 ref_counter = capitalizeFirstLetter(kind) + " " + counters[kind];
                 caption.textContent = ref_counter + ": " + caption.textContent
-                stored[caption.id] = ref_counter // store the value for resolve_crossrefs below
+                stored[caption.id] = ref_counter // store the value for resolveCrossrefs below
             }
         });
     });
+    figcaptions.forEach(function(caption, i) {
+        counters["figure"] += 1
+        ref_counter = capitalizeFirstLetter("figure") + " " + counters["figure"];
+        if (!caption.textContent.startsWith(ref_counter + ": ")) {
+            caption.textContent = ref_counter + ": " + caption.textContent
+        }
+        stored[caption.id] = ref_counter // store the value for resolveCrossrefs below
+    })
 }
 
 // iterate all a.crossref and insert the calculated values; for floats and sections
-function resolve_crossrefs() {
+function resolveCrossrefs() {
     var refs = document.querySelectorAll("a.crossref");
     refs.forEach(function(ref, i) {
         ref.textContent = stored[ref.name]
         if (ref.hasAttribute("end")) { // for ranges
             end = ref.getAttribute("end")
             ref.textContent += "–" + stored[end]
         }
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-slides.css` & `clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-slides.css`

 * *Files identical despite different names*

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/static/clld-slides.js` & `clld_document_plugin-0.0.5/src/clld_document_plugin/static/clld-slides.js`

 * *Files identical despite different names*

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/chapter.mako` & `clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/chapter.mako`

 * *Files 13% similar despite different names*

```diff
@@ -45,12 +45,12 @@
     </div>
 </div>
 
 
 <script src="${req.static_url('clld_document_plugin:static/clld-document.js')}">
 </script>
 <script>
-    number_sections()
-    number_examples()
-    number_captions()
-    resolve_crossrefs()
+    numberSections()
+    numberExamples()
+    numberCaptions()
+    resolveCrossrefs()
 </script>
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/templates/document/slides.mako` & `clld_document_plugin-0.0.5/src/clld_document_plugin/templates/document/slides.mako`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     <% tag = re.findall("{#(.*?)}", title) %>
     <% title = title.split("{#")[0].strip() %>
     % if len(tag) == 0:
         <% tag = f"slide-{i}" %>
     % else:
         <% tag = tag[0] %>
     % endif
-    <div id="${tag}" class="slide"><div class="slide-title"><h2>${title}</h2></div><div class="slide-content">${markdown(request, content, permalink=False)|n}</div></div>
+    <div id="${tag}" class="slide"><div class="slide-title"><h2>${title}</h2></div><div class="slide-content">${markdown(request, content)|n}</div></div>
 
 
 % endfor
 
 </div>
 
 <script src="${req.static_url('clld_document_plugin:static/clld-slides.js')}"></script>
```

#### html2text {}

```diff
@@ -9,10 +9,10 @@
     * % endfor
 %endif
 % for (i, part) in enumerate(parts): <% title, content = part.split("\n", 1) %>
 <% tag = re.findall("{#(.*?)}", title) %> <% title = title.split("{#")[0].strip
 () %> % if len(tag) == 0: <% tag = f"slide-{i}" %> % else: <% tag = tag[0] %> %
 endif
 ***** ${title} *****
-${markdown(request, content, permalink=False)|n}
+${markdown(request, content)|n}
 % endfor
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin/util.py` & `clld_document_plugin-0.0.5/src/clld_document_plugin/util.py`

 * *Files identical despite different names*

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/PKG-INFO` & `clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld-document-plugin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Document model and rendering in CLLD apps.
 Home-page: https://github.com/fmatter/clld-document-plugin
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 Project-URL: Bug Tracker, https://github.com/fmatter/clld-document-plugin/issues
 Keywords: clld,linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `clld_document_plugin-0.0.4/src/clld_document_plugin.egg-info/SOURCES.txt` & `clld_document_plugin-0.0.5/src/clld_document_plugin.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 src/clld_document_plugin/static/clld-document.css
 src/clld_document_plugin/static/clld-document.js
 src/clld_document_plugin/static/clld-slides.css
 src/clld_document_plugin/static/clld-slides.js
 src/clld_document_plugin/templates/document/chapter.mako
 src/clld_document_plugin/templates/document/detail_html.mako
 src/clld_document_plugin/templates/document/index_html.mako
-src/clld_document_plugin/templates/document/slides.mako
+src/clld_document_plugin/templates/document/slides.mako
+src/clld_document_plugin/templates/topic/detail_html.mako
+src/clld_document_plugin/templates/topic/index_html.mako
```

