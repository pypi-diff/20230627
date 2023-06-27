# Comparing `tmp/lacam_v0-0.1.3.tar.gz` & `tmp/lacam_v0-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacam_v0-0.1.3.tar", last modified: Tue Jun 27 20:02:22 2023, max compression
+gzip compressed data, was "lacam_v0-0.1.4.tar", last modified: Tue Jun 27 20:04:55 2023, max compression
```

## Comparing `lacam_v0-0.1.3.tar` & `lacam_v0-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 20:02:22.910412 lacam_v0-0.1.3/
--rw-rw-rw-   0        0        0      264 2023-06-27 20:02:22.907420 lacam_v0-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 20:02:22.910412 lacam_v0-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-27 20:00:38.000000 lacam_v0-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 20:02:22.848581 lacam_v0-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 20:02:22.855559 lacam_v0-0.1.3/src/lacam_v0/
--rw-rw-rw-   0        0        0       35 2023-06-27 19:56:41.000000 lacam_v0-0.1.3/src/lacam_v0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 20:02:22.903442 lacam_v0-0.1.3/src/lacam_v0/data/
--rw-rw-rw-   0        0        0      315 2023-06-27 18:45:36.000000 lacam_v0-0.1.3/src/lacam_v0/data/dict_dados_disp.txt
--rw-rw-rw-   0        0        0     1204 2023-06-27 19:57:04.000000 lacam_v0-0.1.3/src/lacam_v0/datasets.py
-drwxrwxrwx   0        0        0        0 2023-06-27 20:02:22.897447 lacam_v0-0.1.3/src/lacam_v0.egg-info/
--rw-rw-rw-   0        0        0      264 2023-06-27 20:02:22.000000 lacam_v0-0.1.3/src/lacam_v0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-27 20:02:22.000000 lacam_v0-0.1.3/src/lacam_v0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 20:02:22.000000 lacam_v0-0.1.3/src/lacam_v0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 20:02:22.000000 lacam_v0-0.1.3/src/lacam_v0.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 20:04:55.714736 lacam_v0-0.1.4/
+-rw-rw-rw-   0        0        0      264 2023-06-27 20:04:55.712741 lacam_v0-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 20:04:55.715733 lacam_v0-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-27 20:04:51.000000 lacam_v0-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:04:55.664531 lacam_v0-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 20:04:55.682485 lacam_v0-0.1.4/src/lacam_v0/
+-rw-rw-rw-   0        0        0       35 2023-06-27 19:56:41.000000 lacam_v0-0.1.4/src/lacam_v0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:04:55.709753 lacam_v0-0.1.4/src/lacam_v0/data/
+-rw-rw-rw-   0        0        0      315 2023-06-27 18:45:36.000000 lacam_v0-0.1.4/src/lacam_v0/data/dict_dados_disp.txt
+-rw-rw-rw-   0        0        0     1214 2023-06-27 20:04:39.000000 lacam_v0-0.1.4/src/lacam_v0/datasets.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:04:55.707757 lacam_v0-0.1.4/src/lacam_v0.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-06-27 20:04:55.000000 lacam_v0-0.1.4/src/lacam_v0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-27 20:04:55.000000 lacam_v0-0.1.4/src/lacam_v0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 20:04:55.000000 lacam_v0-0.1.4/src/lacam_v0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 20:04:55.000000 lacam_v0-0.1.4/src/lacam_v0.egg-info/top_level.txt
```

### Comparing `lacam_v0-0.1.3/src/lacam_v0/datasets.py` & `lacam_v0-0.1.4/src/lacam_v0/datasets.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
     
     def __init__(self, name: list):
         self.arquivos_disponiveis = self._criarDict()
         
         for i in range(name):
             self._baixarDados(name[i])
 
-    def _criarDict():
+    def _criarDict(self):
         try:
             dicio = {}
             path = "data/dict_dados_disp.txt"
             with open(path, "r") as file:
                 for line in file:
                     key, value = line.split(";")
                     dicio[key] = value       
             return dicio
         except Exception as e:
             print(f"Error: {str(e)}")
 
-    def _baixarDados(name: str):
+    def _baixarDados(self, name: str):
 
         if name in self.arquivos_disponiveis.keys():
 
             filename = self.arquivos_disponiveis.get(name)
             url = self.arquivos_disponiveis[filename]
             filename = filename + '.csv'
```

