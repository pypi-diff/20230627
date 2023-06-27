# Comparing `tmp/cldf_ldd-0.0.4.tar.gz` & `tmp/cldf_ldd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cldf_ldd-0.0.4.tar", last modified: Wed Mar  1 22:20:27 2023, max compression
+gzip compressed data, was "dist/cldf_ldd-0.0.6.tar", last modified: Tue Jun 27 20:56:19 2023, max compression
```

## Comparing `cldf_ldd-0.0.4.tar` & `cldf_ldd-0.0.6.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      395 2023-03-01 22:20:23.000000 cldf_ldd-0.0.4/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1074 2022-12-03 06:33:53.000000 cldf_ldd-0.0.4/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       64 2023-02-20 05:18:09.000000 cldf_ldd-0.0.4/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1765 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/PKG-INFO
--rw-r--r--   0 florianm  (1000) florianm  (1000)      886 2023-02-27 23:28:29.000000 cldf_ldd-0.0.4/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      507 2022-12-03 06:33:53.000000 cldf_ldd-0.0.4/pyproject.toml
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1666 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-12-03 06:33:53.000000 cldf_ldd-0.0.4/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1714 2023-03-01 22:20:17.000000 cldf_ldd-0.0.4/src/cldf_ldd/__init__.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      487 2023-02-20 02:10:58.000000 cldf_ldd-0.0.4/src/cldf_ldd/cldf.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2393 2023-02-27 21:01:46.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/__init__.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      741 2023-02-25 03:48:58.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/columns.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1192 2023-02-27 21:00:15.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/DerivProcTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1200 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      217 2023-01-31 07:56:56.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2008 2023-02-28 20:09:34.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/DerivationTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1401 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      236 2023-02-27 23:33:40.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1476 2023-02-25 03:40:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/ExampleParts-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      882 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      122 2023-02-10 08:39:32.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1231 2023-02-27 22:27:18.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/FormParts-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      737 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      145 2023-02-27 22:52:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1254 2023-02-27 22:26:52.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/FormStems-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      631 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       16 2023-02-27 22:51:39.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      898 2023-02-25 03:40:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/GlossTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1068 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      376 2023-01-31 08:35:02.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1275 2023-02-27 22:44:23.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/InflCatTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      987 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      146 2023-02-27 23:01:46.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1175 2023-02-27 22:26:06.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/InflValTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      901 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      136 2023-02-27 22:43:05.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1487 2023-02-28 00:18:44.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/InflectionTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1425 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      544 2023-02-27 22:42:30.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/description.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1760 2023-02-27 21:01:45.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/keys.yaml
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2733 2023-02-28 20:10:38.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/LexemeTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1875 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       89 2023-02-27 22:59:59.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2168 2023-02-27 22:35:20.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/MorphemeTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1614 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2023-02-27 22:35:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2802 2023-02-27 22:33:44.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/MorphTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2664 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      248 2023-02-27 22:10:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1899 2023-02-25 03:40:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/POSTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1355 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       17 2023-02-02 09:20:15.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      606 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      648 2023-02-25 03:40:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/SpeakerTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       79 2023-01-17 17:01:57.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      770 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1505 2023-02-27 22:25:38.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/StemParts-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       12 2023-01-30 20:05:59.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stems/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2089 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stems/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2773 2023-02-27 22:25:30.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stems/StemTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      342 2023-02-27 23:00:19.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/stems/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/texts/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2089 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/texts/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1815 2023-03-01 22:19:11.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/texts/TextTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      847 2023-01-17 15:57:18.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/texts/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1296 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1528 2023-02-27 22:25:21.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/WordformParts-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2023-02-27 22:40:16.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2295 2023-03-01 22:19:50.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/README.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2947 2023-02-28 20:08:18.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/WordformTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      514 2023-02-28 20:06:00.000000 cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/description.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1765 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3455 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      238 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        9 2023-03-01 22:20:27.000000 cldf_ldd-0.0.4/src/cldf_ldd.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      395 2023-06-27 20:56:09.000000 cldf_ldd-0.0.6/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1074 2022-12-03 06:33:53.000000 cldf_ldd-0.0.6/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       64 2023-02-20 05:18:09.000000 cldf_ldd-0.0.6/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1765 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/PKG-INFO
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      886 2023-02-27 23:28:29.000000 cldf_ldd-0.0.6/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      507 2022-12-03 06:33:53.000000 cldf_ldd-0.0.6/pyproject.toml
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1666 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-12-03 06:33:53.000000 cldf_ldd-0.0.6/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1522 2023-06-27 20:56:00.000000 cldf_ldd-0.0.6/src/cldf_ldd/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      488 2023-06-17 19:30:10.000000 cldf_ldd-0.0.6/src/cldf_ldd/cldf.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2627 2023-06-20 17:07:58.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/__init__.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      930 2023-03-07 07:13:22.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/columns.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1192 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/DerivProcTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1200 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      217 2023-01-31 07:56:56.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2009 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/DerivationTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1401 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      236 2023-02-27 23:33:40.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1476 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/ExampleParts-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      882 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      122 2023-02-10 08:39:32.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1231 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/FormParts-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      766 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      145 2023-02-27 22:52:27.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1242 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/FormStems-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      712 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       16 2023-02-27 22:51:39.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      898 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/GlossTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1068 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      376 2023-01-31 08:35:02.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1275 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/InflCatTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      987 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      146 2023-02-27 23:01:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1176 2023-06-26 16:56:36.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/InflValTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      901 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      136 2023-02-27 22:43:05.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1487 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/InflectionTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1425 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      544 2023-02-27 22:42:30.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/description.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2200 2023-06-20 17:08:14.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/keys.yaml
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2726 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/LexemeTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1821 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       89 2023-02-27 22:59:59.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2434 2023-06-17 00:54:17.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/MorphemeTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1753 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2023-02-27 22:35:50.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3063 2023-06-17 00:54:13.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/MorphTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2798 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      248 2023-02-27 22:10:57.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1899 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/POSTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1355 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       17 2023-02-02 09:20:15.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/phonemes/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1898 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/phonemes/PhonemeTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1352 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/phonemes/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       11 2023-03-02 02:47:00.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/phonemes/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      598 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      640 2023-03-07 07:10:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/SpeakerTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       79 2023-01-17 17:01:57.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      770 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1505 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/StemParts-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       12 2023-01-30 20:05:59.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stems/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2890 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stems/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3041 2023-06-17 00:54:48.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stems/StemTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      342 2023-02-27 23:00:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/stems/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/texts/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2089 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/texts/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1815 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/texts/TextTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      847 2023-01-17 15:57:18.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/texts/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1296 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1528 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/WordformParts-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2023-02-27 22:40:16.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3182 2023-06-27 20:51:46.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/README.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3423 2023-03-04 23:53:09.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/WordformTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      514 2023-02-28 20:06:00.000000 cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/description.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1765 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3606 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      238 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        9 2023-06-27 20:56:19.000000 cldf_ldd-0.0.6/src/cldf_ldd.egg-info/top_level.txt
```

### Comparing `cldf_ldd-0.0.4/LICENSE` & `cldf_ldd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/PKG-INFO` & `cldf_ldd-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldf_ldd
-Version: 0.0.4
+Version: 0.0.6
 Summary: CLDF schemata for language description and documentation.
 Home-page: https://github.com/fmatter/cldf-ldd
 Author: Florian Matter
 Author-email: fmatter@mailbox.org
 Project-URL: Bug Tracker, https://github.com/fmatter/cldf-ldd/issues
 Keywords: cldf,descriptive linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cldf_ldd-0.0.4/README.md` & `cldf_ldd-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/setup.cfg` & `cldf_ldd-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	descriptive linguistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = cldf_ldd
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/cldf-ldd/issues
 url = https://github.com/fmatter/cldf-ldd
-version = 0.0.4
+version = 0.0.6
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/__init__.py` & `cldf_ldd-0.0.6/src/cldf_ldd/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 """Top-level package for cldf-ldd."""
 import functools
 import logging
 import colorlog
-from cldf_ldd.cldf import columns, keys
+from cldf_ldd.cldf import columns
+from cldf_ldd.cldf import keys
 from cldf_ldd.components import *
 
+
 try:
     from importlib.resources import files  # pragma: no cover
 except ImportError:  # pragma: no cover
     from importlib_resources import files  # pragma: no cover
 
 
-handler = colorlog.StreamHandler(None)
-handler.setFormatter(
-    colorlog.ColoredFormatter("%(log_color)s%(levelname)-7s%(reset)s %(message)s")
-)
 log = logging.getLogger(__name__)
-log.setLevel(logging.INFO)
-log.propagate = True
-log.addHandler(handler)
 
 
 __author__ = "Florian Matter"
 __email__ = "fmatter@mailbox.org"
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 
 def valid_parts(name, dataset, table, column, row):
     value = row[column.name]
     if value and None in value:
         raise ValueError(f"None in {value} in column {column}")
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/__init__.py` & `cldf_ldd-0.0.6/src/cldf_ldd/components/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     "FormParts",
     "FormStems",
     "StemParts",
     "GlossTable",
     "POSTable",
     "TextTable",
     "ExampleParts",
+    "PhonemeTable",
+    "SpeakerTable",
 ]
 
 cldf_path = files("cldf_ldd") / "components"
 WordformTable = jsonlib.load(cldf_path / "wordforms/WordformTable-metadata.json")
 StemTable = jsonlib.load(cldf_path / "stems/StemTable-metadata.json")
 MorphTable = jsonlib.load(cldf_path / "morphs/MorphTable-metadata.json")
 InflectionTable = jsonlib.load(cldf_path / "inflections/InflectionTable-metadata.json")
@@ -45,14 +47,16 @@
 FormParts = jsonlib.load(cldf_path / "formparts/FormParts-metadata.json")
 FormStems = jsonlib.load(cldf_path / "formstems/FormStems-metadata.json")
 StemParts = jsonlib.load(cldf_path / "stemparts/StemParts-metadata.json")
 GlossTable = jsonlib.load(cldf_path / "glosses/GlossTable-metadata.json")
 POSTable = jsonlib.load(cldf_path / "partsofspeech/POSTable-metadata.json")
 TextTable = jsonlib.load(cldf_path / "texts/TextTable-metadata.json")
 ExampleParts = jsonlib.load(cldf_path / "exampleparts/ExampleParts-metadata.json")
+PhonemeTable = jsonlib.load(cldf_path / "phonemes/PhonemeTable-metadata.json")
+SpeakerTable = jsonlib.load(cldf_path / "speakers/SpeakerTable-metadata.json")
 
 tables = [
     WordformTable,
     StemTable,
     MorphTable,
     InflectionTable,
     InflValTable,
@@ -65,8 +69,10 @@
     FormParts,
     FormStems,
     StemParts,
     GlossTable,
     POSTable,
     TextTable,
     ExampleParts,
+    PhonemeTable,
+    SpeakerTable,
 ]
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/columns.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/columns.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'ExampleTable'": "{insert: [(2, OrderedDict([('name', 'Speaker_ID'), ('required', False), "*

 * *                   "('dc:description', 'The speaker who uttered this record.'), ('datatype', "*

 * *                   "'string')]))]}"}*

```diff
@@ -7,14 +7,20 @@
             "required": false
         },
         {
             "datatype": "integer",
             "dc:description": "The positions of this record in the text.",
             "name": "Record_Number",
             "required": false
+        },
+        {
+            "datatype": "string",
+            "dc:description": "The speaker who uttered this record.",
+            "name": "Speaker_ID",
+            "required": false
         }
     ],
     "FormTable": [
         {
             "datatype": "string",
             "dc:description": "The form, segmented into morphological segments.",
             "dc:extent": "multivalued",
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/DerivProcTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/DerivProcTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/derivationalprocesses/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/derivationalprocesses/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/DerivationTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/DerivationTable-metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'tableSchema'": "{'columns': {5: {'required': False}}}"}*

```diff
@@ -39,15 +39,15 @@
                 "required": false
             },
             {
                 "datatype": "string",
                 "dc:description": "Specifies one or multiple morphs in the stem marking the derivation.",
                 "dc:extent": "multivalued",
                 "name": "Stempart_IDs",
-                "required": true,
+                "required": false,
                 "separator": ","
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/derivations/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/derivations/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/ExampleParts-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/ExampleParts-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/exampleparts/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/exampleparts/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/FormParts-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/FormParts-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/formparts/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/formparts/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 
 ## FormParts: `formparts.csv`
 
 Name/Property | Datatype | Cardinality | Description
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
 `Form_ID` | `string` | singlevalued | The associated form.
-`Wordform_ID` | `string` | singlevalued | The associated wordform.
+`Wordform_ID` | `string` | singlevalued | The associated wordform.<br>References wordforms.csv.
 `Index` | `string` | singlevalued | Specifies the position of a morph in a wordform.
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/FormStems-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/WordformParts-metadata.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.71%*

 * *Differences: {"'tableSchema'": "{'columns': {1: {'dc:description': 'The involved wordform.'}, 2: {'name': "*

 * *                  "'Morph_ID', 'required': False, 'dc:description': 'The involved morph.'}, 3: "*

 * *                  "{'required': False, 'dc:description': 'Specifies the position of a morph in a "*

 * *                  "wordform.'}, insert: [(4, OrderedDict([('name', 'Gloss_ID'), ('required', "*

 * *                  "False), ('dc:extent', 'multivalued'), ('separator', ','), ('dc:description', "*

 * *                  "'The glos […]*

```diff
@@ -8,33 +8,41 @@
                 },
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The associated wordform.",
+                "dc:description": "The involved wordform.",
                 "dc:extent": "singlevalued",
                 "name": "Wordform_ID",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The stem of the associated wordform.",
+                "dc:description": "The involved morph.",
                 "dc:extent": "singlevalued",
-                "name": "Stem_ID",
-                "required": true
+                "name": "Morph_ID",
+                "required": false
             },
             {
                 "datatype": {
                     "base": "string",
                     "format": "\\d+(:\\d+)?"
                 },
-                "dc:description": "Specifies the position(s) of an stem in a wordform.",
+                "dc:description": "Specifies the position of a morph in a wordform.",
                 "dc:extent": "singlevalued",
                 "name": "Index",
-                "required": true
+                "required": false
+            },
+            {
+                "datatype": "string",
+                "dc:description": "The gloss the morph has in the wordform.",
+                "dc:extent": "multivalued",
+                "name": "Gloss_ID",
+                "required": false,
+                "separator": ","
             }
         ]
     },
-    "url": "wordformstems.csv"
+    "url": "wordformparts.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/formstems/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 
 
 ## FormStems: `wordformstems.csv`
 
 Name/Property | Datatype | Cardinality | Description
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
-`Wordform_ID` | `string` | singlevalued | The associated wordform.
-`Stem_ID` | `string` | singlevalued | The stem of the associated wordform.
-`Index` | `string` | singlevalued | Specifies the position(s) of an stem in a wordform.
+`Wordform_ID` | `string` | singlevalued | The associated wordform.<br>References wordforms.csv.
+`Stem_ID` | `string` | singlevalued | The stem of the associated wordform.<br>References stems.csv.
+`Index` | list of `integer` (separated by `,`) | multivalued | Specifies the position(s) of an stem in a wordform.
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/GlossTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/GlossTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/glosses/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/glosses/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/InflCatTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/InflCatTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalcategories/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalcategories/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/InflValTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/InflValTable-metadata.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'tableSchema'": "{'columns': {3: {'required': False}}}"}*

```diff
@@ -25,13 +25,13 @@
                 "required": true
             },
             {
                 "datatype": "string",
                 "dc:description": "The gloss for the inflectional value.",
                 "dc:extent": "singlevalued",
                 "name": "Gloss_ID",
-                "required": true
+                "required": false
             }
         ]
     },
     "url": "inflectionalvalues.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflectionalvalues/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflectionalvalues/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/InflectionTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/InflectionTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/inflections/description.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/inflections/description.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/keys.yaml` & `cldf_ldd-0.0.6/src/cldf_ldd/components/keys.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -14,107 +14,135 @@
   - Stempart_IDs
   - stemparts.csv
   - ID
 - - derivations.csv
   - Target_ID
   - stems.csv
   - ID
+- - exampleparts.csv
+  - Example_ID
+  - ExampleTable
+  - ID
+- - exampleparts.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
+- - exampleparts.csv
+  - Wordform_ID
+  - wordforms.csv
+  - ID
+- - examples.csv
+  - Text_ID
+  - texts.csv
+  - ID
+- - ExampleTable
+  - Speaker_ID
+  - speakers.csv
+  - ID
+- - formparts.csv
+  - Wordform_ID
+  - wordforms.csv
+  - ID
 - - inflectionalvalues.csv
   - Category_ID
   - inflectionalcategories.csv
   - ID
 - - inflectionalvalues.csv
   - Gloss_ID
   - glosses.csv
   - ID
 - - inflections.csv
+  - Form_ID
+  - forms.csv
+  - ID
+- - inflections.csv
   - Stem_ID
   - stems.csv
   - ID
 - - inflections.csv
   - Value_ID
   - inflectionalvalues.csv
   - ID
 - - inflections.csv
-  - Form_ID
-  - forms.csv
-  - ID
-- - inflections.csv
   - Wordformpart_ID
   - wordformparts.csv
   - ID
+- - lexemes.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
+- - morphemes.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
 - - morphs.csv
   - Morpheme_ID
   - morphemes.csv
   - ID
+- - morphs.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
 - - stemparts.csv
   - Gloss_ID
   - glosses.csv
   - ID
 - - stemparts.csv
   - Morph_ID
   - morphs.csv
   - ID
 - - stemparts.csv
   - Stem_ID
   - stems.csv
   - ID
+- - stems.csv
+  - Lexeme_ID
+  - lexemes.csv
+  - ID
+- - stems.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
 - - wordformparts.csv
   - Gloss_ID
   - glosses.csv
   - ID
 - - wordformparts.csv
   - Morph_ID
   - morphs.csv
   - ID
 - - wordformparts.csv
   - Wordform_ID
   - wordforms.csv
   - ID
 - - wordforms.csv
+  - Parameter_ID
+  - ParameterTable
+  - ID
+- - wordforms.csv
   - Stem_ID
   - stems.csv
   - ID
-- - exampleparts.csv
-  - Wordform_ID
-  - wordforms.csv
+- - wordforms.csv
+  - Part_Of_Speech
+  - partsofspeech.csv
   - ID
-- - exampleparts.csv
-  - Example_ID
-  - ExampleTable
+- - wordformstems.csv
+  - Stem_ID
+  - stems.csv
   - ID
-- - exampleparts.csv
-  - Parameter_ID
-  - ParameterTable
+- - wordformstems.csv
+  - Wordform_ID
+  - wordforms.csv
   - ID
 - - morphs.csv
-  - Parameter_ID
-  - ParameterTable
+  - Part_Of_Speech
+  - partsofspeech.csv
   - ID
 - - morphemes.csv
-  - Parameter_ID
-  - ParameterTable
-  - ID
-- - lexemes.csv
-  - Parameter_ID
-  - ParameterTable
-  - ID
-- - wordforms.csv
-  - Parameter_ID
-  - ParameterTable
+  - Part_Of_Speech
+  - partsofspeech.csv
   - ID
 - - stems.csv
-  - Parameter_ID
-  - ParameterTable
-  - ID
-- - stems.csv
-  - Gloss_ID
-  - glosses.csv
-  - ID
-- - examples.csv
-  - Text_ID
-  - texts.csv
-  - ID
-- - stems.csv
-  - Lexeme_ID
-  - lexemes.csv
+  - Part_Of_Speech
+  - partsofspeech.csv
   - ID
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/LexemeTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/LexemeTable-metadata.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'tableSchema'": "{'columns': {5: {'dc:description': 'A reference to the meaning denoted by the "*

 * *                  "lexeme.', 'dc:extent': 'multivalued', 'separator': '; ', delete: "*

 * *                  "['propertyUrl']}}}"}*

```diff
@@ -38,18 +38,19 @@
                 "dc:extent": "singlevalued",
                 "name": "Part_Of_Speech",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech",
                 "required": false
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to the meaning denoted by the form",
+                "dc:description": "A reference to the meaning denoted by the lexeme.",
+                "dc:extent": "multivalued",
                 "name": "Parameter_ID",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#parameterReference",
-                "required": false
+                "required": false,
+                "separator": "; "
             },
             {
                 "datatype": "string",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
                 "required": false
             },
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/lexemes/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/lexemes/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 Name/Property | Datatype | Cardinality | Description
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
 [Language_ID](http://cldf.clld.org/v1.0/terms.rdf#languageReference) | `string` | singlevalued | A reference to a language (or variety) the lexeme belongs to<br>References LanguageTable
 [Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | singlevalued | <div> <p>A title, name or label for an entity.</p> </div> 
 [Description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | singlevalued | A human-readable description
 [Part_Of_Speech](http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech) | `string` | singlevalued | <div> <p> The part-of-speech of dictionary entry. </p> </div> 
-[Parameter_ID](http://cldf.clld.org/v1.0/terms.rdf#parameterReference) | `string` | unspecified | A reference to the meaning denoted by the form<br>References ParameterTable
+`Parameter_ID` | list of `string` (separated by `; `) | multivalued | A reference to the meaning denoted by the lexeme.
 [Comment](http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | unspecified | <div> <p> A human-readable comment on a resource, providing additional context. </p> </div> 
 `Paradigm_View` | `json` | singlevalued | A dict with 'x' and 'y' keys containing lists of derivational category IDs.
 [Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `;`) | multivalued | <div> <p>List of source specifications, of the form &lt;source_ID&gt;[], e.g. http://glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where meier2015 is a citation key in the accompanying BibTeX file.</p> </div>
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/MorphemeTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/MorphemeTable-metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'tableSchema'": "{'columns': {4: {'dc:description': 'A reference to the meaning denoted by the "*

 * *                  "morpheme.', 'dc:extent': 'multivalued', 'separator': '; ', delete: "*

 * *                  "['propertyUrl']}, insert: [(7, OrderedDict([('name', 'Part_Of_Speech'), "*

 * *                  "('required', False), ('propertyUrl', "*

 * *                  "'http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech'), ('datatype', 'string'), "*

 * *                  "('dc:extent', 'singlevalued')]))]}}"}*

```diff
@@ -31,30 +31,38 @@
                 "dc:extent": "singlevalued",
                 "name": "Description",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#description",
                 "required": false
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to the meaning denoted by the form",
+                "dc:description": "A reference to the meaning denoted by the morpheme.",
+                "dc:extent": "multivalued",
                 "name": "Parameter_ID",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#parameterReference",
-                "required": false
+                "required": false,
+                "separator": "; "
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
                 "required": false
             },
             {
                 "datatype": "string",
                 "name": "Source",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#source",
                 "required": false,
                 "separator": "; "
+            },
+            {
+                "datatype": "string",
+                "dc:extent": "singlevalued",
+                "name": "Part_Of_Speech",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech",
+                "required": false
             }
         ]
     },
     "url": "morphemes.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/morphemes/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/morphemes/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 
 Name/Property | Datatype | Cardinality | Description
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
 [Language_ID](http://cldf.clld.org/v1.0/terms.rdf#languageReference) | `string` | singlevalued | A reference to a language (or variety) the morpheme belongs to.<br>References LanguageTable
 [Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | singlevalued | <div> <p>A title, name or label for an entity.</p> </div> 
 [Description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | singlevalued | A human-readable description.
-[Parameter_ID](http://cldf.clld.org/v1.0/terms.rdf#parameterReference) | `string` | unspecified | A reference to the meaning denoted by the form<br>References ParameterTable
+`Parameter_ID` | list of `string` (separated by `; `) | multivalued | A reference to the meaning denoted by the morpheme.
 [Comment](http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | singlevalued | <div> <p> A human-readable comment on a resource, providing additional context. </p> </div> 
-[Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `; `) | multivalued | <div> <p>List of source specifications, of the form &lt;source_ID&gt;[], e.g. http://glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where meier2015 is a citation key in the accompanying BibTeX file.</p> </div> 
+[Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `; `) | multivalued | <div> <p>List of source specifications, of the form &lt;source_ID&gt;[], e.g. http://glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where meier2015 is a citation key in the accompanying BibTeX file.</p> </div> 
+[Part_Of_Speech](http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech) | `string` | singlevalued | <div> <p> The part-of-speech of dictionary entry. </p> </div> <br>References partsofspeech.csv.
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/MorphTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/stems/StemTable-metadata.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7136904761904762%*

 * *Differences: {"'tableSchema'": "{'columns': {1: {'dc:description': 'A reference to a language (or variety) the "*

 * *                  "stem belongs to'}, 3: {'name': 'Lexeme_ID', 'dc:description': 'The lexeme this "*

 * *                  "stem belongs to.', delete: ['propertyUrl']}, 4: {'name': 'Parameter_ID', "*

 * *                  "'required': True, 'separator': '; ', 'dc:description': 'A reference to the "*

 * *                  "meaning denoted by the stem.', delete: ['propertyUrl']}, 5: {'name': "*

 * *                  "'Morpho_Segme […]*

```diff
@@ -9,56 +9,57 @@
                 "dc:extent": "singlevalued",
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to a language (or variety) the form belongs to",
+                "dc:description": "A reference to a language (or variety) the stem belongs to",
                 "dc:extent": "singlevalued",
                 "name": "Language_ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#languageReference",
                 "required": true
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Name",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#name",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "A human-readable description.",
+                "dc:description": "The lexeme this stem belongs to.",
                 "dc:extent": "singlevalued",
-                "name": "Description",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#description",
+                "name": "Lexeme_ID",
                 "required": false
             },
             {
                 "datatype": "string",
+                "dc:description": "A reference to the meaning denoted by the stem.",
                 "dc:extent": "multivalued",
-                "name": "Segments",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#segments",
-                "required": false,
-                "separator": " "
+                "name": "Parameter_ID",
+                "required": true,
+                "separator": "; "
             },
             {
                 "datatype": "string",
-                "dc:description": "The morpheme this form belongs to.",
-                "dc:extent": "singlevalued",
-                "name": "Morpheme_ID",
-                "required": false
+                "dc:description": "A representation of the morphologically segmented stem.",
+                "dc:extent": "multivalued",
+                "name": "Morpho_Segments",
+                "required": false,
+                "separator": " "
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to the meaning denoted by the morph.",
-                "name": "Parameter_ID",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#parameterReference",
-                "required": false
+                "dc:extent": "multivalued",
+                "name": "Segments",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#segments",
+                "required": false,
+                "separator": " "
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
                 "required": false
@@ -66,12 +67,19 @@
             {
                 "datatype": "string",
                 "dc:extent": "multivalued",
                 "name": "Source",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#source",
                 "required": false,
                 "separator": "; "
+            },
+            {
+                "datatype": "string",
+                "dc:extent": "singlevalued",
+                "name": "Part_Of_Speech",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech",
+                "required": false
             }
         ]
     },
-    "url": "morphs.csv"
+    "url": "stems.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/morphs/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,10 +10,11 @@
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
 [Language_ID](http://cldf.clld.org/v1.0/terms.rdf#languageReference) | `string` | singlevalued | A reference to a language (or variety) the form belongs to<br>References LanguageTable
 [Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | singlevalued | <div> <p>A title, name or label for an entity.</p> </div> 
 [Description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | singlevalued | A human-readable description.
 [Segments](http://cldf.clld.org/v1.0/terms.rdf#segments) | list of `string` (separated by ` `) | multivalued | <div> <p> A list of segments (aka a sound sequence) is understood as the strict segmental representation of a <a href="http://linguistics-ontology.org/gold/2010/FormUnit">form unit</a> of a language, which is usually given in phonetic transcription. <a href="http://linguistics-ontology.org/gold/2010/Suprasegmental">Suprasegmental elements</a>, like tone or accent, of sound sequences are usually represented in a sequential form, although they are usually co-articulated along with the segmental elements of a sound sequence. Alternatively, suprasegmental aspects could also be represented as part of the <a href="#prosodicStructure">prosodic structure</a> of a word form. </p> </div> 
 `Morpheme_ID` | `string` | singlevalued | The morpheme this form belongs to.<br>References morphemes.csv.
-[Parameter_ID](http://cldf.clld.org/v1.0/terms.rdf#parameterReference) | `string` | unspecified | A reference to the meaning denoted by the morph.<br>References ParameterTable
+`Parameter_ID` | list of `string` (separated by `; `) | multivalued | A reference to the meaning denoted by the morph.
 [Comment](http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | singlevalued | <div> <p> A human-readable comment on a resource, providing additional context. </p> </div> 
-[Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `; `) | multivalued | <div> <p>List of source specifications, of the form &lt;source_ID&gt;[], e.g. http://glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where meier2015 is a citation key in the accompanying BibTeX file.</p> </div> 
+[Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `; `) | multivalued | <div> <p>List of source specifications, of the form &lt;source_ID&gt;[], e.g. http://glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where meier2015 is a citation key in the accompanying BibTeX file.</p> </div> 
+[Part_Of_Speech](http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech) | `string` | singlevalued | <div> <p> The part-of-speech of dictionary entry. </p> </div> <br>References partsofspeech.csv.
```

#### html2text {}

```diff
@@ -19,18 +19,21 @@
 representation of a form_unit of a language, which is usually given in phonetic
 transcription. Suprasegmental_elements, like tone or accent, of sound sequences
 are usually represented in a sequential form, although they are usually co-
 articulated along with the segmental elements of a sound sequence.
 Alternatively, suprasegmental aspects could also be represented as part of the
 prosodic_structure of a word form.
 `Morpheme_ID` | `string` | singlevalued | The morpheme this form belongs to.
-References morphemes.csv. [Parameter_ID](http://cldf.clld.org/v1.0/
-terms.rdf#parameterReference) | `string` | unspecified | A reference to the
-meaning denoted by the morph.
-References ParameterTable [Comment](http://cldf.clld.org/v1.0/
-terms.rdf#comment) | `string` | singlevalued |
+References morphemes.csv. `Parameter_ID` | list of `string` (separated by `; `)
+| multivalued | A reference to the meaning denoted by the morph. [Comment]
+(http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | singlevalued |
 A human-readable comment on a resource, providing additional context.
 [Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string`
 (separated by `; `) | multivalued |
 List of source specifications, of the form <source_ID>[], e.g. http://
 glottolog.org/resource/reference/id/318814[34], or meier2015[3-12] where
 meier2015 is a citation key in the accompanying BibTeX file.
+[Part_Of_Speech](http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech) | `string` |
+singlevalued |
+The part-of-speech of dictionary entry.
+
+References partsofspeech.csv.
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/POSTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/POSTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/partsofspeech/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/partsofspeech/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 Speakers should be able to be connected to text records (examples).
 
 ## SpeakerTable: `speakers.csv`
 
 Name/Property | Datatype | Cardinality | Description
  --- | --- | --- | --- 
 [ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | singlevalued | <div> <p>A unique identifier for a row in a table.</p> <p> To allow usage of identifiers as path components of URLs IDs must only contain alphanumeric characters, underscore and hyphen. </p> </div> 
-[Abbreviation](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | singlevalued | <div> <p>A title, name or label for an entity.</p> </div> 
+[Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | singlevalued | <div> <p>A title, name or label for an entity.</p> </div>
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/speakers/SpeakerTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/speakers/SpeakerTable-metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'tableSchema'": "{'columns': {1: {'name': 'Name'}}}"}*

```diff
@@ -9,15 +9,15 @@
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
-                "name": "Abbreviation",
+                "name": "Name",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#name",
                 "required": true
             }
         ]
     },
     "url": "speakers.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/stemparts/StemParts-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/stemparts/StemParts-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/stems/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/stems/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -65,67 +65,117 @@
 00000400: 7479 2e3c 2f70 3e20 3c2f 6469 763e 200a  ty.</p> </div> .
 00000410: 604c 6578 656d 655f 4944 6020 7c20 6073  `Lexeme_ID` | `s
 00000420: 7472 696e 6760 207c 2073 696e 676c 6576  tring` | singlev
 00000430: 616c 7565 6420 7c20 5468 6520 6c65 7865  alued | The lexe
 00000440: 6d65 2074 6869 7320 7374 656d 2062 656c  me this stem bel
 00000450: 6f6e 6773 2074 6f2e 3c62 723e 5265 6665  ongs to.<br>Refe
 00000460: 7265 6e63 6573 206c 6578 656d 6573 2e63  rences lexemes.c
-00000470: 7376 2e0a 5b50 6172 616d 6574 6572 5f49  sv..[Parameter_I
-00000480: 445d 2868 7474 703a 2f2f 636c 6466 2e63  D](http://cldf.c
-00000490: 6c6c 642e 6f72 672f 7631 2e30 2f74 6572  lld.org/v1.0/ter
-000004a0: 6d73 2e72 6466 2370 6172 616d 6574 6572  ms.rdf#parameter
-000004b0: 5265 6665 7265 6e63 6529 207c 2060 7374  Reference) | `st
-000004c0: 7269 6e67 6020 7c20 756e 7370 6563 6966  ring` | unspecif
-000004d0: 6965 6420 7c20 4120 7265 6665 7265 6e63  ied | A referenc
-000004e0: 6520 746f 2074 6865 206d 6561 6e69 6e67  e to the meaning
-000004f0: 2064 656e 6f74 6564 2062 7920 7468 6520   denoted by the 
-00000500: 7374 656d 3c62 723e 5265 6665 7265 6e63  stem<br>Referenc
-00000510: 6573 2050 6172 616d 6574 6572 5461 626c  es ParameterTabl
-00000520: 650a 604d 6f72 7068 6f5f 5365 676d 656e  e.`Morpho_Segmen
-00000530: 7473 6020 7c20 6c69 7374 206f 6620 6073  ts` | list of `s
-00000540: 7472 696e 6760 2028 7365 7061 7261 7465  tring` (separate
-00000550: 6420 6279 2060 2060 2920 7c20 6d75 6c74  d by ` `) | mult
-00000560: 6976 616c 7565 6420 7c20 4120 7265 7072  ivalued | A repr
-00000570: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00000580: 6520 6d6f 7270 686f 6c6f 6769 6361 6c6c  e morphologicall
-00000590: 7920 7365 676d 656e 7465 6420 7374 656d  y segmented stem
-000005a0: 2e0a 6047 6c6f 7373 5f49 4460 207c 206c  ..`Gloss_ID` | l
-000005b0: 6973 7420 6f66 2060 7374 7269 6e67 6020  ist of `string` 
-000005c0: 2873 6570 6172 6174 6564 2062 7920 602c  (separated by `,
-000005d0: 6029 207c 206d 756c 7469 7661 6c75 6564  `) | multivalued
-000005e0: 207c 2054 6865 2067 6c6f 7373 2074 6865   | The gloss the
-000005f0: 206d 6f72 7068 2068 6173 2069 6e20 7468   morph has in th
-00000600: 6520 776f 7264 666f 726d 2e3c 6272 3e52  e wordform.<br>R
-00000610: 6566 6572 656e 6365 7320 676c 6f73 7365  eferences glosse
-00000620: 732e 6373 762e 0a5b 436f 6d6d 656e 745d  s.csv..[Comment]
-00000630: 2868 7474 703a 2f2f 636c 6466 2e63 6c6c  (http://cldf.cll
-00000640: 642e 6f72 672f 7631 2e30 2f74 6572 6d73  d.org/v1.0/terms
-00000650: 2e72 6466 2363 6f6d 6d65 6e74 2920 7c20  .rdf#comment) | 
-00000660: 6073 7472 696e 6760 207c 2073 696e 676c  `string` | singl
-00000670: 6576 616c 7565 6420 7c20 3c64 6976 3e20  evalued | <div> 
-00000680: 3c70 3e20 4120 6875 6d61 6e2d 7265 6164  <p> A human-read
-00000690: 6162 6c65 2063 6f6d 6d65 6e74 206f 6e20  able comment on 
-000006a0: 6120 7265 736f 7572 6365 2c20 7072 6f76  a resource, prov
-000006b0: 6964 696e 6720 6164 6469 7469 6f6e 616c  iding additional
-000006c0: 2063 6f6e 7465 7874 2e20 3c2f 703e 203c   context. </p> <
-000006d0: 2f64 6976 3e20 0a5b 536f 7572 6365 5d28  /div> .[Source](
-000006e0: 6874 7470 3a2f 2f63 6c64 662e 636c 6c64  http://cldf.clld
-000006f0: 2e6f 7267 2f76 312e 302f 7465 726d 732e  .org/v1.0/terms.
-00000700: 7264 6623 736f 7572 6365 2920 7c20 6c69  rdf#source) | li
-00000710: 7374 206f 6620 6073 7472 696e 6760 2028  st of `string` (
-00000720: 7365 7061 7261 7465 6420 6279 2060 3b20  separated by `; 
-00000730: 6029 207c 206d 756c 7469 7661 6c75 6564  `) | multivalued
-00000740: 207c 203c 6469 763e 203c 703e 4c69 7374   | <div> <p>List
-00000750: 206f 6620 736f 7572 6365 2073 7065 6369   of source speci
-00000760: 6669 6361 7469 6f6e 732c 206f 6620 7468  fications, of th
-00000770: 6520 666f 726d 2026 6c74 3b73 6f75 7263  e form &lt;sourc
-00000780: 655f 4944 2667 743b 5b5d 2c20 652e 672e  e_ID&gt;[], e.g.
-00000790: 2068 7474 703a 2f2f 676c 6f74 746f 6c6f   http://glottolo
-000007a0: 672e 6f72 672f 7265 736f 7572 6365 2f72  g.org/resource/r
-000007b0: 6566 6572 656e 6365 2f69 642f 3331 3838  eference/id/3188
-000007c0: 3134 5b33 345d 2c20 6f72 206d 6569 6572  14[34], or meier
-000007d0: 3230 3135 5b33 2d31 325d 2077 6865 7265  2015[3-12] where
-000007e0: 206d 6569 6572 3230 3135 2069 7320 6120   meier2015 is a 
-000007f0: 6369 7461 7469 6f6e 206b 6579 2069 6e20  citation key in 
-00000800: 7468 6520 6163 636f 6d70 616e 7969 6e67  the accompanying
-00000810: 2042 6962 5465 5820 6669 6c65 2e3c 2f70   BibTeX file.</p
-00000820: 3e20 3c2f 6469 763e 20                   > </div> 
+00000470: 7376 2e0a 6050 6172 616d 6574 6572 5f49  sv..`Parameter_I
+00000480: 4460 207c 206c 6973 7420 6f66 2060 7374  D` | list of `st
+00000490: 7269 6e67 6020 2873 6570 6172 6174 6564  ring` (separated
+000004a0: 2062 7920 603b 2060 2920 7c20 6d75 6c74   by `; `) | mult
+000004b0: 6976 616c 7565 6420 7c20 4120 7265 6665  ivalued | A refe
+000004c0: 7265 6e63 6520 746f 2074 6865 206d 6561  rence to the mea
+000004d0: 6e69 6e67 2064 656e 6f74 6564 2062 7920  ning denoted by 
+000004e0: 7468 6520 7374 656d 2e0a 604d 6f72 7068  the stem..`Morph
+000004f0: 6f5f 5365 676d 656e 7473 6020 7c20 6c69  o_Segments` | li
+00000500: 7374 206f 6620 6073 7472 696e 6760 2028  st of `string` (
+00000510: 7365 7061 7261 7465 6420 6279 2060 2060  separated by ` `
+00000520: 2920 7c20 6d75 6c74 6976 616c 7565 6420  ) | multivalued 
+00000530: 7c20 4120 7265 7072 6573 656e 7461 7469  | A representati
+00000540: 6f6e 206f 6620 7468 6520 6d6f 7270 686f  on of the morpho
+00000550: 6c6f 6769 6361 6c6c 7920 7365 676d 656e  logically segmen
+00000560: 7465 6420 7374 656d 2e0a 5b53 6567 6d65  ted stem..[Segme
+00000570: 6e74 735d 2868 7474 703a 2f2f 636c 6466  nts](http://cldf
+00000580: 2e63 6c6c 642e 6f72 672f 7631 2e30 2f74  .clld.org/v1.0/t
+00000590: 6572 6d73 2e72 6466 2373 6567 6d65 6e74  erms.rdf#segment
+000005a0: 7329 207c 206c 6973 7420 6f66 2060 7374  s) | list of `st
+000005b0: 7269 6e67 6020 2873 6570 6172 6174 6564  ring` (separated
+000005c0: 2062 7920 6020 6029 207c 206d 756c 7469   by ` `) | multi
+000005d0: 7661 6c75 6564 207c 203c 6469 763e 203c  valued | <div> <
+000005e0: 703e 2041 206c 6973 7420 6f66 2073 6567  p> A list of seg
+000005f0: 6d65 6e74 7320 2861 6b61 2061 2073 6f75  ments (aka a sou
+00000600: 6e64 2073 6571 7565 6e63 6529 2069 7320  nd sequence) is 
+00000610: 756e 6465 7273 746f 6f64 2061 7320 7468  understood as th
+00000620: 6520 7374 7269 6374 2073 6567 6d65 6e74  e strict segment
+00000630: 616c 2072 6570 7265 7365 6e74 6174 696f  al representatio
+00000640: 6e20 6f66 2061 203c 6120 6872 6566 3d22  n of a <a href="
+00000650: 6874 7470 3a2f 2f6c 696e 6775 6973 7469  http://linguisti
+00000660: 6373 2d6f 6e74 6f6c 6f67 792e 6f72 672f  cs-ontology.org/
+00000670: 676f 6c64 2f32 3031 302f 466f 726d 556e  gold/2010/FormUn
+00000680: 6974 223e 666f 726d 2075 6e69 743c 2f61  it">form unit</a
+00000690: 3e20 6f66 2061 206c 616e 6775 6167 652c  > of a language,
+000006a0: 2077 6869 6368 2069 7320 7573 7561 6c6c   which is usuall
+000006b0: 7920 6769 7665 6e20 696e 2070 686f 6e65  y given in phone
+000006c0: 7469 6320 7472 616e 7363 7269 7074 696f  tic transcriptio
+000006d0: 6e2e 203c 6120 6872 6566 3d22 6874 7470  n. <a href="http
+000006e0: 3a2f 2f6c 696e 6775 6973 7469 6373 2d6f  ://linguistics-o
+000006f0: 6e74 6f6c 6f67 792e 6f72 672f 676f 6c64  ntology.org/gold
+00000700: 2f32 3031 302f 5375 7072 6173 6567 6d65  /2010/Suprasegme
+00000710: 6e74 616c 223e 5375 7072 6173 6567 6d65  ntal">Suprasegme
+00000720: 6e74 616c 2065 6c65 6d65 6e74 733c 2f61  ntal elements</a
+00000730: 3e2c 206c 696b 6520 746f 6e65 206f 7220  >, like tone or 
+00000740: 6163 6365 6e74 2c20 6f66 2073 6f75 6e64  accent, of sound
+00000750: 2073 6571 7565 6e63 6573 2061 7265 2075   sequences are u
+00000760: 7375 616c 6c79 2072 6570 7265 7365 6e74  sually represent
+00000770: 6564 2069 6e20 6120 7365 7175 656e 7469  ed in a sequenti
+00000780: 616c 2066 6f72 6d2c 2061 6c74 686f 7567  al form, althoug
+00000790: 6820 7468 6579 2061 7265 2075 7375 616c  h they are usual
+000007a0: 6c79 2063 6f2d 6172 7469 6375 6c61 7465  ly co-articulate
+000007b0: 6420 616c 6f6e 6720 7769 7468 2074 6865  d along with the
+000007c0: 2073 6567 6d65 6e74 616c 2065 6c65 6d65   segmental eleme
+000007d0: 6e74 7320 6f66 2061 2073 6f75 6e64 2073  nts of a sound s
+000007e0: 6571 7565 6e63 652e 2041 6c74 6572 6e61  equence. Alterna
+000007f0: 7469 7665 6c79 2c20 7375 7072 6173 6567  tively, supraseg
+00000800: 6d65 6e74 616c 2061 7370 6563 7473 2063  mental aspects c
+00000810: 6f75 6c64 2061 6c73 6f20 6265 2072 6570  ould also be rep
+00000820: 7265 7365 6e74 6564 2061 7320 7061 7274  resented as part
+00000830: 206f 6620 7468 6520 3c61 2068 7265 663d   of the <a href=
+00000840: 2223 7072 6f73 6f64 6963 5374 7275 6374  "#prosodicStruct
+00000850: 7572 6522 3e70 726f 736f 6469 6320 7374  ure">prosodic st
+00000860: 7275 6374 7572 653c 2f61 3e20 6f66 2061  ructure</a> of a
+00000870: 2077 6f72 6420 666f 726d 2e20 3c2f 703e   word form. </p>
+00000880: 203c 2f64 6976 3e20 0a5b 436f 6d6d 656e   </div> .[Commen
+00000890: 745d 2868 7474 703a 2f2f 636c 6466 2e63  t](http://cldf.c
+000008a0: 6c6c 642e 6f72 672f 7631 2e30 2f74 6572  lld.org/v1.0/ter
+000008b0: 6d73 2e72 6466 2363 6f6d 6d65 6e74 2920  ms.rdf#comment) 
+000008c0: 7c20 6073 7472 696e 6760 207c 2073 696e  | `string` | sin
+000008d0: 676c 6576 616c 7565 6420 7c20 3c64 6976  glevalued | <div
+000008e0: 3e20 3c70 3e20 4120 6875 6d61 6e2d 7265  > <p> A human-re
+000008f0: 6164 6162 6c65 2063 6f6d 6d65 6e74 206f  adable comment o
+00000900: 6e20 6120 7265 736f 7572 6365 2c20 7072  n a resource, pr
+00000910: 6f76 6964 696e 6720 6164 6469 7469 6f6e  oviding addition
+00000920: 616c 2063 6f6e 7465 7874 2e20 3c2f 703e  al context. </p>
+00000930: 203c 2f64 6976 3e20 0a5b 536f 7572 6365   </div> .[Source
+00000940: 5d28 6874 7470 3a2f 2f63 6c64 662e 636c  ](http://cldf.cl
+00000950: 6c64 2e6f 7267 2f76 312e 302f 7465 726d  ld.org/v1.0/term
+00000960: 732e 7264 6623 736f 7572 6365 2920 7c20  s.rdf#source) | 
+00000970: 6c69 7374 206f 6620 6073 7472 696e 6760  list of `string`
+00000980: 2028 7365 7061 7261 7465 6420 6279 2060   (separated by `
+00000990: 3b20 6029 207c 206d 756c 7469 7661 6c75  ; `) | multivalu
+000009a0: 6564 207c 203c 6469 763e 203c 703e 4c69  ed | <div> <p>Li
+000009b0: 7374 206f 6620 736f 7572 6365 2073 7065  st of source spe
+000009c0: 6369 6669 6361 7469 6f6e 732c 206f 6620  cifications, of 
+000009d0: 7468 6520 666f 726d 2026 6c74 3b73 6f75  the form &lt;sou
+000009e0: 7263 655f 4944 2667 743b 5b5d 2c20 652e  rce_ID&gt;[], e.
+000009f0: 672e 2068 7474 703a 2f2f 676c 6f74 746f  g. http://glotto
+00000a00: 6c6f 672e 6f72 672f 7265 736f 7572 6365  log.org/resource
+00000a10: 2f72 6566 6572 656e 6365 2f69 642f 3331  /reference/id/31
+00000a20: 3838 3134 5b33 345d 2c20 6f72 206d 6569  8814[34], or mei
+00000a30: 6572 3230 3135 5b33 2d31 325d 2077 6865  er2015[3-12] whe
+00000a40: 7265 206d 6569 6572 3230 3135 2069 7320  re meier2015 is 
+00000a50: 6120 6369 7461 7469 6f6e 206b 6579 2069  a citation key i
+00000a60: 6e20 7468 6520 6163 636f 6d70 616e 7969  n the accompanyi
+00000a70: 6e67 2042 6962 5465 5820 6669 6c65 2e3c  ng BibTeX file.<
+00000a80: 2f70 3e20 3c2f 6469 763e 200a 5b50 6172  /p> </div> .[Par
+00000a90: 745f 4f66 5f53 7065 6563 685d 2868 7474  t_Of_Speech](htt
+00000aa0: 703a 2f2f 636c 6466 2e63 6c6c 642e 6f72  p://cldf.clld.or
+00000ab0: 672f 7631 2e30 2f74 6572 6d73 2e72 6466  g/v1.0/terms.rdf
+00000ac0: 2370 6172 744f 6653 7065 6563 6829 207c  #partOfSpeech) |
+00000ad0: 2060 7374 7269 6e67 6020 7c20 7369 6e67   `string` | sing
+00000ae0: 6c65 7661 6c75 6564 207c 203c 6469 763e  levalued | <div>
+00000af0: 203c 703e 2054 6865 2070 6172 742d 6f66   <p> The part-of
+00000b00: 2d73 7065 6563 6820 6f66 2064 6963 7469  -speech of dicti
+00000b10: 6f6e 6172 7920 656e 7472 792e 203c 2f70  onary entry. </p
+00000b20: 3e20 3c2f 6469 763e 203c 6272 3e52 6566  > </div> <br>Ref
+00000b30: 6572 656e 6365 7320 7061 7274 736f 6673  erences partsofs
+00000b40: 7065 6563 682e 6373 762e                 peech.csv.
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/stems/StemTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/WordformTable-metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7003787878787879%*

 * *Differences: {"'tableSchema'": "{'columns': {0: {delete: ['dc:extent']}, 1: {'dc:description': 'A reference to "*

 * *                  "a language (or variety) the form belongs to'}, 2: {'name': 'Form', "*

 * *                  "'propertyUrl': 'http://cldf.clld.org/v1.0/terms.rdf#form', 'dc:description': "*

 * *                  "'The written expression of the form.'}, 3: {'name': 'Description', "*

 * *                  "'dc:description': 'A human-readable description', 'propertyUrl': "*

 * *                  "'http://cldf.clld.org/v1.0/terms. […]*

```diff
@@ -2,76 +2,93 @@
     "tableSchema": {
         "columns": [
             {
                 "datatype": {
                     "base": "string",
                     "format": "[a-zA-Z0-9_\\-]+"
                 },
-                "dc:extent": "singlevalued",
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to a language (or variety) the stem belongs to",
+                "dc:description": "A reference to a language (or variety) the form belongs to",
                 "dc:extent": "singlevalued",
                 "name": "Language_ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#languageReference",
                 "required": true
             },
             {
                 "datatype": "string",
+                "dc:description": "The written expression of the form.",
                 "dc:extent": "singlevalued",
-                "name": "Name",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#name",
+                "name": "Form",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#form",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The lexeme this stem belongs to.",
+                "dc:description": "A human-readable description",
+                "dc:extent": "singlevalued",
+                "name": "Description",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#description",
+                "required": false
+            },
+            {
+                "datatype": "string",
                 "dc:extent": "singlevalued",
-                "name": "Lexeme_ID",
+                "name": "Part_Of_Speech",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech",
                 "required": false
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to the meaning denoted by the stem",
+                "dc:description": "A reference to the meaning denoted by the form",
+                "dc:extent": "multivalued",
                 "name": "Parameter_ID",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#parameterReference",
-                "required": true
+                "required": true,
+                "separator": "; "
             },
             {
                 "datatype": "string",
-                "dc:description": "A representation of the morphologically segmented stem.",
+                "dc:description": "A representation of the morphologically segmented form.",
                 "dc:extent": "multivalued",
                 "name": "Morpho_Segments",
                 "required": false,
                 "separator": " "
             },
             {
                 "datatype": "string",
-                "dc:description": "The gloss the morph has in the wordform.",
+                "dc:description": "The stem of which this wordform is an inflected form.",
+                "dc:extent": "singlevalued",
+                "name": "Stem_ID",
+                "required": false
+            },
+            {
+                "datatype": "string",
                 "dc:extent": "multivalued",
-                "name": "Gloss_ID",
-                "required": true,
-                "separator": ","
+                "name": "Segments",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#segments",
+                "required": false,
+                "separator": " "
             },
             {
                 "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
                 "required": false
             },
             {
-                "datatype": "string",
-                "dc:extent": "multivalued",
+                "datatype": {
+                    "base": "string"
+                },
                 "name": "Source",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#source",
                 "required": false,
-                "separator": "; "
+                "separator": ";"
             }
         ]
     },
-    "url": "stems.csv"
+    "url": "wordforms.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/texts/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/texts/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/texts/TextTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/texts/TextTable-metadata.json`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/texts/description.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/texts/description.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/wordformparts/README.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/wordformparts/WordformParts-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/formstems/FormStems-metadata.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7066666666666667%*

 * *Differences: {"'tableSchema'": "{'columns': {1: {'dc:description': 'The associated wordform.'}, 2: {'name': "*

 * *                  "'Stem_ID', 'required': True, 'dc:description': 'The stem of the associated "*

 * *                  "wordform.'}, 3: {'name': 'Index', 'required': True, 'dc:description': "*

 * *                  "'Specifies the position(s) of an stem in a wordform.', 'datatype': {replace: "*

 * *                  "OrderedDict([('base', 'integer')])}}, delete: [3]}}",*

 * * "'url'": "'wordformstems.csv'"}*

```diff
@@ -8,41 +8,33 @@
                 },
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The involved wordform.",
+                "dc:description": "The associated wordform.",
                 "dc:extent": "singlevalued",
                 "name": "Wordform_ID",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The involved morph.",
+                "dc:description": "The stem of the associated wordform.",
                 "dc:extent": "singlevalued",
-                "name": "Morph_ID",
-                "required": false
+                "name": "Stem_ID",
+                "required": true
             },
             {
                 "datatype": {
-                    "base": "string",
-                    "format": "\\d+(:\\d+)?"
+                    "base": "integer"
                 },
-                "dc:description": "Specifies the position of a morph in a wordform.",
-                "dc:extent": "singlevalued",
-                "name": "Index",
-                "required": false
-            },
-            {
-                "datatype": "string",
-                "dc:description": "The gloss the morph has in the wordform.",
+                "dc:description": "Specifies the position(s) of an stem in a wordform.",
                 "dc:extent": "multivalued",
-                "name": "Gloss_ID",
-                "required": false,
+                "name": "Index",
+                "required": true,
                 "separator": ","
             }
         ]
     },
-    "url": "wordformparts.csv"
+    "url": "wordformstems.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/README.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -76,69 +76,124 @@
 000004b0: 7363 7269 7074 696f 6e5d 2868 7474 703a  scription](http:
 000004c0: 2f2f 636c 6466 2e63 6c6c 642e 6f72 672f  //cldf.clld.org/
 000004d0: 7631 2e30 2f74 6572 6d73 2e72 6466 2364  v1.0/terms.rdf#d
 000004e0: 6573 6372 6970 7469 6f6e 2920 7c20 6073  escription) | `s
 000004f0: 7472 696e 6760 207c 2073 696e 676c 6576  tring` | singlev
 00000500: 616c 7565 6420 7c20 4120 6875 6d61 6e2d  alued | A human-
 00000510: 7265 6164 6162 6c65 2064 6573 6372 6970  readable descrip
-00000520: 7469 6f6e 0a5b 5061 7261 6d65 7465 725f  tion.[Parameter_
-00000530: 4944 5d28 6874 7470 3a2f 2f63 6c64 662e  ID](http://cldf.
-00000540: 636c 6c64 2e6f 7267 2f76 312e 302f 7465  clld.org/v1.0/te
-00000550: 726d 732e 7264 6623 7061 7261 6d65 7465  rms.rdf#paramete
-00000560: 7252 6566 6572 656e 6365 2920 7c20 6073  rReference) | `s
-00000570: 7472 696e 6760 207c 2075 6e73 7065 6369  tring` | unspeci
-00000580: 6669 6564 207c 2041 2072 6566 6572 656e  fied | A referen
-00000590: 6365 2074 6f20 7468 6520 6d65 616e 696e  ce to the meanin
-000005a0: 6720 6465 6e6f 7465 6420 6279 2074 6865  g denoted by the
-000005b0: 2066 6f72 6d3c 6272 3e52 6566 6572 656e   form<br>Referen
-000005c0: 6365 7320 5061 7261 6d65 7465 7254 6162  ces ParameterTab
-000005d0: 6c65 0a5b 4d6f 7270 686f 5f53 6567 6d65  le.[Morpho_Segme
-000005e0: 6e74 735d 2868 7474 703a 2f2f 636c 6466  nts](http://cldf
-000005f0: 2e63 6c6c 642e 6f72 672f 7631 2e30 2f74  .clld.org/v1.0/t
-00000600: 6572 6d73 2e72 6466 2373 6567 6d65 6e74  erms.rdf#segment
-00000610: 7329 207c 206c 6973 7420 6f66 2060 7374  s) | list of `st
-00000620: 7269 6e67 6020 2873 6570 6172 6174 6564  ring` (separated
-00000630: 2062 7920 6020 6029 207c 206d 756c 7469   by ` `) | multi
-00000640: 7661 6c75 6564 207c 2041 2072 6570 7265  valued | A repre
-00000650: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
-00000660: 206d 6f72 7068 6f6c 6f67 6963 616c 6c79   morphologically
-00000670: 2073 6567 6d65 6e74 6564 2066 6f72 6d2e   segmented form.
-00000680: 0a60 5374 656d 5f49 4460 207c 2060 7374  .`Stem_ID` | `st
-00000690: 7269 6e67 6020 7c20 7369 6e67 6c65 7661  ring` | singleva
-000006a0: 6c75 6564 207c 2054 6865 2073 7465 6d20  lued | The stem 
-000006b0: 6f66 2077 6869 6368 2074 6869 7320 776f  of which this wo
-000006c0: 7264 666f 726d 2069 7320 616e 2069 6e66  rdform is an inf
-000006d0: 6c65 6374 6564 2066 6f72 6d2e 3c62 723e  lected form.<br>
-000006e0: 5265 6665 7265 6e63 6573 2073 7465 6d73  References stems
-000006f0: 2e63 7376 2e0a 5b43 6f6d 6d65 6e74 5d28  .csv..[Comment](
-00000700: 6874 7470 3a2f 2f63 6c64 662e 636c 6c64  http://cldf.clld
-00000710: 2e6f 7267 2f76 312e 302f 7465 726d 732e  .org/v1.0/terms.
-00000720: 7264 6623 636f 6d6d 656e 7429 207c 2060  rdf#comment) | `
-00000730: 7374 7269 6e67 6020 7c20 7369 6e67 6c65  string` | single
-00000740: 7661 6c75 6564 207c 203c 6469 763e 203c  valued | <div> <
-00000750: 703e 2041 2068 756d 616e 2d72 6561 6461  p> A human-reada
-00000760: 626c 6520 636f 6d6d 656e 7420 6f6e 2061  ble comment on a
-00000770: 2072 6573 6f75 7263 652c 2070 726f 7669   resource, provi
-00000780: 6469 6e67 2061 6464 6974 696f 6e61 6c20  ding additional 
-00000790: 636f 6e74 6578 742e 203c 2f70 3e20 3c2f  context. </p> </
-000007a0: 6469 763e 200a 5b53 6f75 7263 655d 2868  div> .[Source](h
-000007b0: 7474 703a 2f2f 636c 6466 2e63 6c6c 642e  ttp://cldf.clld.
-000007c0: 6f72 672f 7631 2e30 2f74 6572 6d73 2e72  org/v1.0/terms.r
-000007d0: 6466 2373 6f75 7263 6529 207c 206c 6973  df#source) | lis
-000007e0: 7420 6f66 2060 7374 7269 6e67 6020 2873  t of `string` (s
-000007f0: 6570 6172 6174 6564 2062 7920 603b 6029  eparated by `;`)
-00000800: 207c 206d 756c 7469 7661 6c75 6564 207c   | multivalued |
-00000810: 203c 6469 763e 203c 703e 4c69 7374 206f   <div> <p>List o
-00000820: 6620 736f 7572 6365 2073 7065 6369 6669  f source specifi
-00000830: 6361 7469 6f6e 732c 206f 6620 7468 6520  cations, of the 
-00000840: 666f 726d 2026 6c74 3b73 6f75 7263 655f  form &lt;source_
-00000850: 4944 2667 743b 5b5d 2c20 652e 672e 2068  ID&gt;[], e.g. h
-00000860: 7474 703a 2f2f 676c 6f74 746f 6c6f 672e  ttp://glottolog.
-00000870: 6f72 672f 7265 736f 7572 6365 2f72 6566  org/resource/ref
-00000880: 6572 656e 6365 2f69 642f 3331 3838 3134  erence/id/318814
-00000890: 5b33 345d 2c20 6f72 206d 6569 6572 3230  [34], or meier20
-000008a0: 3135 5b33 2d31 325d 2077 6865 7265 206d  15[3-12] where m
-000008b0: 6569 6572 3230 3135 2069 7320 6120 6369  eier2015 is a ci
-000008c0: 7461 7469 6f6e 206b 6579 2069 6e20 7468  tation key in th
-000008d0: 6520 6163 636f 6d70 616e 7969 6e67 2042  e accompanying B
-000008e0: 6962 5465 5820 6669 6c65 2e3c 2f70 3e20  ibTeX file.</p> 
-000008f0: 3c2f 6469 763e 20                        </div> 
+00000520: 7469 6f6e 0a5b 5061 7274 5f4f 665f 5370  tion.[Part_Of_Sp
+00000530: 6565 6368 5d28 6874 7470 3a2f 2f63 6c64  eech](http://cld
+00000540: 662e 636c 6c64 2e6f 7267 2f76 312e 302f  f.clld.org/v1.0/
+00000550: 7465 726d 732e 7264 6623 7061 7274 4f66  terms.rdf#partOf
+00000560: 5370 6565 6368 2920 7c20 6073 7472 696e  Speech) | `strin
+00000570: 6760 207c 2073 696e 676c 6576 616c 7565  g` | singlevalue
+00000580: 6420 7c20 3c64 6976 3e20 3c70 3e20 5468  d | <div> <p> Th
+00000590: 6520 7061 7274 2d6f 662d 7370 6565 6368  e part-of-speech
+000005a0: 206f 6620 6469 6374 696f 6e61 7279 2065   of dictionary e
+000005b0: 6e74 7279 2e20 3c2f 703e 203c 2f64 6976  ntry. </p> </div
+000005c0: 3e20 3c62 723e 5265 6665 7265 6e63 6573  > <br>References
+000005d0: 2070 6172 7473 6f66 7370 6565 6368 2e63   partsofspeech.c
+000005e0: 7376 2e0a 6050 6172 616d 6574 6572 5f49  sv..`Parameter_I
+000005f0: 4460 207c 206c 6973 7420 6f66 2060 7374  D` | list of `st
+00000600: 7269 6e67 6020 2873 6570 6172 6174 6564  ring` (separated
+00000610: 2062 7920 603b 2060 2920 7c20 6d75 6c74   by `; `) | mult
+00000620: 6976 616c 7565 6420 7c20 4120 7265 6665  ivalued | A refe
+00000630: 7265 6e63 6520 746f 2074 6865 206d 6561  rence to the mea
+00000640: 6e69 6e67 2064 656e 6f74 6564 2062 7920  ning denoted by 
+00000650: 7468 6520 666f 726d 0a60 4d6f 7270 686f  the form.`Morpho
+00000660: 5f53 6567 6d65 6e74 7360 207c 206c 6973  _Segments` | lis
+00000670: 7420 6f66 2060 7374 7269 6e67 6020 2873  t of `string` (s
+00000680: 6570 6172 6174 6564 2062 7920 6020 6029  eparated by ` `)
+00000690: 207c 206d 756c 7469 7661 6c75 6564 207c   | multivalued |
+000006a0: 2041 2072 6570 7265 7365 6e74 6174 696f   A representatio
+000006b0: 6e20 6f66 2074 6865 206d 6f72 7068 6f6c  n of the morphol
+000006c0: 6f67 6963 616c 6c79 2073 6567 6d65 6e74  ogically segment
+000006d0: 6564 2066 6f72 6d2e 0a60 5374 656d 5f49  ed form..`Stem_I
+000006e0: 4460 207c 2060 7374 7269 6e67 6020 7c20  D` | `string` | 
+000006f0: 7369 6e67 6c65 7661 6c75 6564 207c 2054  singlevalued | T
+00000700: 6865 2073 7465 6d20 6f66 2077 6869 6368  he stem of which
+00000710: 2074 6869 7320 776f 7264 666f 726d 2069   this wordform i
+00000720: 7320 616e 2069 6e66 6c65 6374 6564 2066  s an inflected f
+00000730: 6f72 6d2e 3c62 723e 5265 6665 7265 6e63  orm.<br>Referenc
+00000740: 6573 2073 7465 6d73 2e63 7376 2e0a 5b53  es stems.csv..[S
+00000750: 6567 6d65 6e74 735d 2868 7474 703a 2f2f  egments](http://
+00000760: 636c 6466 2e63 6c6c 642e 6f72 672f 7631  cldf.clld.org/v1
+00000770: 2e30 2f74 6572 6d73 2e72 6466 2373 6567  .0/terms.rdf#seg
+00000780: 6d65 6e74 7329 207c 206c 6973 7420 6f66  ments) | list of
+00000790: 2060 7374 7269 6e67 6020 2873 6570 6172   `string` (separ
+000007a0: 6174 6564 2062 7920 6020 6029 207c 206d  ated by ` `) | m
+000007b0: 756c 7469 7661 6c75 6564 207c 203c 6469  ultivalued | <di
+000007c0: 763e 203c 703e 2041 206c 6973 7420 6f66  v> <p> A list of
+000007d0: 2073 6567 6d65 6e74 7320 2861 6b61 2061   segments (aka a
+000007e0: 2073 6f75 6e64 2073 6571 7565 6e63 6529   sound sequence)
+000007f0: 2069 7320 756e 6465 7273 746f 6f64 2061   is understood a
+00000800: 7320 7468 6520 7374 7269 6374 2073 6567  s the strict seg
+00000810: 6d65 6e74 616c 2072 6570 7265 7365 6e74  mental represent
+00000820: 6174 696f 6e20 6f66 2061 203c 6120 6872  ation of a <a hr
+00000830: 6566 3d22 6874 7470 3a2f 2f6c 696e 6775  ef="http://lingu
+00000840: 6973 7469 6373 2d6f 6e74 6f6c 6f67 792e  istics-ontology.
+00000850: 6f72 672f 676f 6c64 2f32 3031 302f 466f  org/gold/2010/Fo
+00000860: 726d 556e 6974 223e 666f 726d 2075 6e69  rmUnit">form uni
+00000870: 743c 2f61 3e20 6f66 2061 206c 616e 6775  t</a> of a langu
+00000880: 6167 652c 2077 6869 6368 2069 7320 7573  age, which is us
+00000890: 7561 6c6c 7920 6769 7665 6e20 696e 2070  ually given in p
+000008a0: 686f 6e65 7469 6320 7472 616e 7363 7269  honetic transcri
+000008b0: 7074 696f 6e2e 203c 6120 6872 6566 3d22  ption. <a href="
+000008c0: 6874 7470 3a2f 2f6c 696e 6775 6973 7469  http://linguisti
+000008d0: 6373 2d6f 6e74 6f6c 6f67 792e 6f72 672f  cs-ontology.org/
+000008e0: 676f 6c64 2f32 3031 302f 5375 7072 6173  gold/2010/Supras
+000008f0: 6567 6d65 6e74 616c 223e 5375 7072 6173  egmental">Supras
+00000900: 6567 6d65 6e74 616c 2065 6c65 6d65 6e74  egmental element
+00000910: 733c 2f61 3e2c 206c 696b 6520 746f 6e65  s</a>, like tone
+00000920: 206f 7220 6163 6365 6e74 2c20 6f66 2073   or accent, of s
+00000930: 6f75 6e64 2073 6571 7565 6e63 6573 2061  ound sequences a
+00000940: 7265 2075 7375 616c 6c79 2072 6570 7265  re usually repre
+00000950: 7365 6e74 6564 2069 6e20 6120 7365 7175  sented in a sequ
+00000960: 656e 7469 616c 2066 6f72 6d2c 2061 6c74  ential form, alt
+00000970: 686f 7567 6820 7468 6579 2061 7265 2075  hough they are u
+00000980: 7375 616c 6c79 2063 6f2d 6172 7469 6375  sually co-articu
+00000990: 6c61 7465 6420 616c 6f6e 6720 7769 7468  lated along with
+000009a0: 2074 6865 2073 6567 6d65 6e74 616c 2065   the segmental e
+000009b0: 6c65 6d65 6e74 7320 6f66 2061 2073 6f75  lements of a sou
+000009c0: 6e64 2073 6571 7565 6e63 652e 2041 6c74  nd sequence. Alt
+000009d0: 6572 6e61 7469 7665 6c79 2c20 7375 7072  ernatively, supr
+000009e0: 6173 6567 6d65 6e74 616c 2061 7370 6563  asegmental aspec
+000009f0: 7473 2063 6f75 6c64 2061 6c73 6f20 6265  ts could also be
+00000a00: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+00000a10: 7061 7274 206f 6620 7468 6520 3c61 2068  part of the <a h
+00000a20: 7265 663d 2223 7072 6f73 6f64 6963 5374  ref="#prosodicSt
+00000a30: 7275 6374 7572 6522 3e70 726f 736f 6469  ructure">prosodi
+00000a40: 6320 7374 7275 6374 7572 653c 2f61 3e20  c structure</a> 
+00000a50: 6f66 2061 2077 6f72 6420 666f 726d 2e20  of a word form. 
+00000a60: 3c2f 703e 203c 2f64 6976 3e20 0a5b 436f  </p> </div> .[Co
+00000a70: 6d6d 656e 745d 2868 7474 703a 2f2f 636c  mment](http://cl
+00000a80: 6466 2e63 6c6c 642e 6f72 672f 7631 2e30  df.clld.org/v1.0
+00000a90: 2f74 6572 6d73 2e72 6466 2363 6f6d 6d65  /terms.rdf#comme
+00000aa0: 6e74 2920 7c20 6073 7472 696e 6760 207c  nt) | `string` |
+00000ab0: 2073 696e 676c 6576 616c 7565 6420 7c20   singlevalued | 
+00000ac0: 3c64 6976 3e20 3c70 3e20 4120 6875 6d61  <div> <p> A huma
+00000ad0: 6e2d 7265 6164 6162 6c65 2063 6f6d 6d65  n-readable comme
+00000ae0: 6e74 206f 6e20 6120 7265 736f 7572 6365  nt on a resource
+00000af0: 2c20 7072 6f76 6964 696e 6720 6164 6469  , providing addi
+00000b00: 7469 6f6e 616c 2063 6f6e 7465 7874 2e20  tional context. 
+00000b10: 3c2f 703e 203c 2f64 6976 3e20 0a5b 536f  </p> </div> .[So
+00000b20: 7572 6365 5d28 6874 7470 3a2f 2f63 6c64  urce](http://cld
+00000b30: 662e 636c 6c64 2e6f 7267 2f76 312e 302f  f.clld.org/v1.0/
+00000b40: 7465 726d 732e 7264 6623 736f 7572 6365  terms.rdf#source
+00000b50: 2920 7c20 6c69 7374 206f 6620 6073 7472  ) | list of `str
+00000b60: 696e 6760 2028 7365 7061 7261 7465 6420  ing` (separated 
+00000b70: 6279 2060 3b60 2920 7c20 6d75 6c74 6976  by `;`) | multiv
+00000b80: 616c 7565 6420 7c20 3c64 6976 3e20 3c70  alued | <div> <p
+00000b90: 3e4c 6973 7420 6f66 2073 6f75 7263 6520  >List of source 
+00000ba0: 7370 6563 6966 6963 6174 696f 6e73 2c20  specifications, 
+00000bb0: 6f66 2074 6865 2066 6f72 6d20 266c 743b  of the form &lt;
+00000bc0: 736f 7572 6365 5f49 4426 6774 3b5b 5d2c  source_ID&gt;[],
+00000bd0: 2065 2e67 2e20 6874 7470 3a2f 2f67 6c6f   e.g. http://glo
+00000be0: 7474 6f6c 6f67 2e6f 7267 2f72 6573 6f75  ttolog.org/resou
+00000bf0: 7263 652f 7265 6665 7265 6e63 652f 6964  rce/reference/id
+00000c00: 2f33 3138 3831 345b 3334 5d2c 206f 7220  /318814[34], or 
+00000c10: 6d65 6965 7232 3031 355b 332d 3132 5d20  meier2015[3-12] 
+00000c20: 7768 6572 6520 6d65 6965 7232 3031 3520  where meier2015 
+00000c30: 6973 2061 2063 6974 6174 696f 6e20 6b65  is a citation ke
+00000c40: 7920 696e 2074 6865 2061 6363 6f6d 7061  y in the accompa
+00000c50: 6e79 696e 6720 4269 6254 6558 2066 696c  nying BibTeX fil
+00000c60: 652e 3c2f 703e 203c 2f64 6976 3e20       e.</p> </div>
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/WordformTable-metadata.json` & `cldf_ldd-0.0.6/src/cldf_ldd/components/morphs/MorphTable-metadata.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7004058441558442%*

 * *Differences: {"'tableSchema'": "{'columns': {0: {'dc:extent': 'singlevalued'}, 2: {'name': 'Name', "*

 * *                  "'propertyUrl': 'http://cldf.clld.org/v1.0/terms.rdf#name', delete: "*

 * *                  "['dc:description']}, 3: {'dc:description': 'A human-readable description.'}, 4: "*

 * *                  "{'name': 'Segments', delete: ['dc:description']}, 5: {'name': 'Morpheme_ID', "*

 * *                  "'dc:description': 'The morpheme this form belongs to.'}, 8: {'datatype': "*

 * *                  "'string', 'separator': ' […]*

```diff
@@ -2,78 +2,84 @@
     "tableSchema": {
         "columns": [
             {
                 "datatype": {
                     "base": "string",
                     "format": "[a-zA-Z0-9_\\-]+"
                 },
+                "dc:extent": "singlevalued",
                 "name": "ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#id",
                 "required": true
             },
             {
                 "datatype": "string",
                 "dc:description": "A reference to a language (or variety) the form belongs to",
                 "dc:extent": "singlevalued",
                 "name": "Language_ID",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#languageReference",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "The written expression of the form.",
                 "dc:extent": "singlevalued",
-                "name": "Form",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#form",
+                "name": "Name",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#name",
                 "required": true
             },
             {
                 "datatype": "string",
-                "dc:description": "A human-readable description",
+                "dc:description": "A human-readable description.",
                 "dc:extent": "singlevalued",
                 "name": "Description",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#description",
                 "required": false
             },
             {
                 "datatype": "string",
-                "dc:description": "A reference to the meaning denoted by the form",
-                "name": "Parameter_ID",
-                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#parameterReference",
-                "required": true
-            },
-            {
-                "datatype": "string",
-                "dc:description": "A representation of the morphologically segmented form.",
                 "dc:extent": "multivalued",
-                "name": "Morpho_Segments",
+                "name": "Segments",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#segments",
                 "required": false,
                 "separator": " "
             },
             {
                 "datatype": "string",
-                "dc:description": "The stem of which this wordform is an inflected form.",
+                "dc:description": "The morpheme this form belongs to.",
                 "dc:extent": "singlevalued",
-                "name": "Stem_ID",
+                "name": "Morpheme_ID",
                 "required": false
             },
             {
                 "datatype": "string",
+                "dc:description": "A reference to the meaning denoted by the morph.",
+                "dc:extent": "multivalued",
+                "name": "Parameter_ID",
+                "required": false,
+                "separator": "; "
+            },
+            {
+                "datatype": "string",
                 "dc:extent": "singlevalued",
                 "name": "Comment",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#comment",
                 "required": false
             },
             {
-                "datatype": {
-                    "base": "string"
-                },
+                "datatype": "string",
+                "dc:extent": "multivalued",
                 "name": "Source",
                 "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#source",
                 "required": false,
-                "separator": ";"
+                "separator": "; "
+            },
+            {
+                "datatype": "string",
+                "dc:extent": "singlevalued",
+                "name": "Part_Of_Speech",
+                "propertyUrl": "http://cldf.clld.org/v1.0/terms.rdf#partOfSpeech",
+                "required": false
             }
         ]
     },
-    "url": "wordforms.csv"
+    "url": "morphs.csv"
 }
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd/components/wordforms/description.md` & `cldf_ldd-0.0.6/src/cldf_ldd/components/wordforms/description.md`

 * *Files identical despite different names*

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd.egg-info/PKG-INFO` & `cldf_ldd-0.0.6/src/cldf_ldd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cldf-ldd
-Version: 0.0.4
+Version: 0.0.6
 Summary: CLDF schemata for language description and documentation.
 Home-page: https://github.com/fmatter/cldf-ldd
 Author: Florian Matter
 Author-email: fmatter@mailbox.org
 Project-URL: Bug Tracker, https://github.com/fmatter/cldf-ldd/issues
 Keywords: cldf,descriptive linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cldf_ldd-0.0.4/src/cldf_ldd.egg-info/SOURCES.txt` & `cldf_ldd-0.0.6/src/cldf_ldd.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 src/cldf_ldd/components/morphemes/description.md
 src/cldf_ldd/components/morphs/MorphTable-metadata.json
 src/cldf_ldd/components/morphs/README.md
 src/cldf_ldd/components/morphs/description.md
 src/cldf_ldd/components/partsofspeech/POSTable-metadata.json
 src/cldf_ldd/components/partsofspeech/README.md
 src/cldf_ldd/components/partsofspeech/description.md
+src/cldf_ldd/components/phonemes/PhonemeTable-metadata.json
+src/cldf_ldd/components/phonemes/README.md
+src/cldf_ldd/components/phonemes/description.md
 src/cldf_ldd/components/speakers/README.md
 src/cldf_ldd/components/speakers/SpeakerTable-metadata.json
 src/cldf_ldd/components/speakers/description.md
 src/cldf_ldd/components/stemparts/README.md
 src/cldf_ldd/components/stemparts/StemParts-metadata.json
 src/cldf_ldd/components/stemparts/description.md
 src/cldf_ldd/components/stems/README.md
```

