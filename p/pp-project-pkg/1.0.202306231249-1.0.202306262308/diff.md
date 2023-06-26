# Comparing `tmp/pp_project_pkg-1.0.202306231249-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306262308-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 10665 bytes, number of entries: 13
+Zip file size: 10366 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-23 12:39 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-23 12:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-23 12:49 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-26 23:08 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306231249.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306231249.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-23 12:49 pp_project_pkg-1.0.202306231249.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 12:49 pp_project_pkg-1.0.202306231249.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-23 12:49 pp_project_pkg-1.0.202306231249.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-23 12:49 pp_project_pkg-1.0.202306231249.dist-info/RECORD
-13 files, 27614 bytes uncompressed, 8643 bytes compressed:  68.7%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-26 23:09 pp_project_pkg-1.0.202306262308.dist-info/RECORD
+12 files, 27436 bytes uncompressed, 8536 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -15,26 +15,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306231249.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306231249.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306262308.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306231249.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306262308.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306231249.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306262308.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306231249.dist-info/top_level.txt
-Comment: 
-
-Filename: pp_project_pkg-1.0.202306231249.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306262308.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
-VERSION_DAY = int('23')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('49')
+VERSION_DAY = int('26')
+VERSION_HOUR = int('23')
+VERSION_MINUTE = int('08')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306231249
-version_date = '2023/06/23 12:49'
+PATCH_VERSION = 202306262308
+version_date = '2023/06/26 23:08'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306231249.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306231249.dist-info/RECORD` & `pp_project_pkg-1.0.202306262308.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
 pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=BG-GcL2RWURz6u6eBY3jQevUck205t9HgE6Xftpp7hQ,396
+pp_project_pkg/version.py,sha256=tAmroGakhkmEHycpy5xpt-3WDi_m7HryVAvPxUNgiJ0,396
 pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306231249.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306231249.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306231249.dist-info/METADATA,sha256=7h_y7ISzBSu5WT2OjQ7iYD56GhmdlnZskp-FIDC-GRw,191
-pp_project_pkg-1.0.202306231249.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306231249.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306231249.dist-info/RECORD,,
+pp_project_pkg-1.0.202306262308.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306262308.dist-info/METADATA,sha256=KfGCOrf2IvSNyatMe9WYimvoPBEhIhYooNF8Qg223KM,191
+pp_project_pkg-1.0.202306262308.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306262308.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306262308.dist-info/RECORD,,
```

