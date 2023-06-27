# Comparing `tmp/BibSane-0.1.2.tar.gz` & `tmp/BibSane-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BibSane-0.1.2.tar", last modified: Wed Apr 12 08:16:56 2023, max compression
+gzip compressed data, was "BibSane-0.1.3.tar", last modified: Tue Jun 27 07:56:11 2023, max compression
```

## Comparing `BibSane-0.1.2.tar` & `BibSane-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:16:56.152399 BibSane-0.1.2/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-12 08:16:56.152399 BibSane-0.1.2/BibSane.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43635 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      231 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       41 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        8 2023-04-12 08:16:56.000000 BibSane-0.1.2/BibSane.egg-info/top_level.txt
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2023-03-21 10:14:38.000000 BibSane-0.1.2/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43635 2023-04-12 08:16:56.152399 BibSane-0.1.2/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     2110 2023-03-24 18:08:11.000000 BibSane-0.1.2/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)    20484 2023-04-12 08:15:05.000000 BibSane-0.1.2/bibsane.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1152 2023-04-12 01:32:16.000000 BibSane-0.1.2/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-12 08:16:56.152399 BibSane-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:56:11.003987 BibSane-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 07:55:54.000000 BibSane-0.1.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:56:10.999987 BibSane-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 07:55:54.000000 BibSane-0.1.3/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:56:10.999987 BibSane-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 07:55:54.000000 BibSane-0.1.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 07:55:54.000000 BibSane-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-27 07:55:54.000000 BibSane-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 07:55:54.000000 BibSane-0.1.3/.pre-commit-hooks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:56:10.999987 BibSane-0.1.3/BibSane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43636 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:56:10.000000 BibSane-0.1.3/BibSane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 07:55:54.000000 BibSane-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 07:55:54.000000 BibSane-0.1.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 07:55:54.000000 BibSane-0.1.3/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-27 07:55:54.000000 BibSane-0.1.3/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43636 2023-06-27 07:56:10.999987 BibSane-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-27 07:55:54.000000 BibSane-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-27 07:55:54.000000 BibSane-0.1.3/bibsane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 07:55:54.000000 BibSane-0.1.3/exampleconfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-27 07:55:54.000000 BibSane-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:56:11.003987 BibSane-0.1.3/setup.cfg
```

### Comparing `BibSane-0.1.2/BibSane.egg-info/PKG-INFO` & `BibSane-0.1.3/BibSane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BibSane
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sanitize BibTeX files without going insane
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # BibSane
 
 Sanitize BibTeX files without going insane.
```

### Comparing `BibSane-0.1.2/COPYING` & `BibSane-0.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `BibSane-0.1.2/PKG-INFO` & `BibSane-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BibSane
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sanitize BibTeX files without going insane
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # BibSane
 
 Sanitize BibTeX files without going insane.
```

### Comparing `BibSane-0.1.2/README.md` & `BibSane-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BibSane-0.1.2/bibsane.py` & `BibSane-0.1.3/bibsane.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,23 @@
         return config
 
 
 RETURN_CODE_UNCHANGED = 0
 RETURN_CODE_CHANGED = 1
 RETURN_CODE_BROKEN = 2
 
+# List of citations to ignore, which are added by some LaTeX templates,
+# but which are not correctly parsed by python-bibtexparser.
+# Related issue: https://github.com/sciunto-org/python-bibtexparser/issues/384
+IGNORED_CITATIONS = set(
+    [
+        "REVTEX41Control",
+    ]
+)
+
 
 def main() -> int:
     """Bibsane main program."""
     fns_aux, verbose, config = parse_args()
     if len(fns_aux) == 0:
         # Only select aux files for which corresponding tex files exist.
         fns_aux = [
@@ -259,14 +268,16 @@
             parse_aux_line("citation", line, citations)
             parse_aux_line("bibdata", line, bibdata)
     fns_bib = []
     for fn_bib in bibdata:
         if not fn_bib.endswith(".bib"):
             fn_bib += ".bib"
         fns_bib.append(os.path.join(root, fn_bib))
+    # Filter out bogus citations
+    citations = [citation for citation in citations if citation not in IGNORED_CITATIONS]
     return citations, fns_bib
 
 
 def parse_aux_line(prefix: str, line: str, words: list[str]):
     """Parse a (simple) line from a LaTeX aux file."""
     if line.startswith(rf"\{prefix}{{"):
         assert line.endswith("}\n")
@@ -306,33 +317,33 @@
     return entries, valid
 
 
 def drop_check_citations(
     entries: list[dict[str, str]], citations: Collection[str], drop
 ) -> tuple[list[dict[str, str]], bool]:
     """Drop unused citations and complain about missing ones."""
-    # Drop unused entries
+    # Check for undefined references
+    defined = {entry["ID"] for entry in entries}
+    valid = True
+    for citation in citations:
+        if citation not in defined:
+            print("   💀 Missing reference:", citation)
+            valid = False
+
+    # Drop unused and irrelevant entries
     result = []
     for entry in entries:
         if entry["ID"] not in citations:
             print("     Dropping unused id:", entry["ID"])
             continue
         if entry["ENTRYTYPE"] in drop:
             print("     Dropping irrelevant entry type:", entry["ENTRYTYPE"])
             continue
         result.append(entry)
 
-    # Check for undefined references
-    defined = {entry["ID"] for entry in entries}
-    valid = True
-    for citation in citations:
-        if citation not in defined:
-            print("   💀 Missing reference:", citation)
-            valid = False
-
     return result, valid
 
 
 def clean_entries(
     entries: list[dict[str, str]], citation_policies: dict[str, dict[str, FieldPolicy]]
 ) -> tuple[list[dict[str, str]], bool]:
     """Clean the irrelevant fields in each entry and complain about missing ones."""
@@ -372,16 +383,16 @@
     """Fix unwarranted use of braces."""
     result = []
     for old_record in entries:
         # Strip all braces
         new_record = {
             key: value.replace("{", "").replace("}", "") for (key, value) in old_record.items()
         }
-        # Except from the author, editor or title
-        for field in "author", "editor", "title":
+        # Except from the author, editor, note or title
+        for field in "author", "editor", "note", "title":
             if field in old_record:
                 new_record[field] = old_record[field]
         result.append(new_record)
     return result
 
 
 def potential_mistakes(entries: list[dict[str, str]]) -> bool:
```

