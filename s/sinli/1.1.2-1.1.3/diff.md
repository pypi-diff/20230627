# Comparing `tmp/sinli-1.1.2.tar.gz` & `tmp/sinli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.2.tar", last modified: Mon May 22 21:37:53 2023, max compression
+gzip compressed data, was "sinli-1.1.3.tar", last modified: Tue Jun 27 10:59:01 2023, max compression
```

## Comparing `sinli-1.1.2.tar` & `sinli-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.510726 sinli-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2023-05-22 21:37:43.000000 sinli-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44158 2023-05-22 21:37:53.506726 sinli-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3934 2023-05-22 21:37:43.000000 sinli-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-22 21:37:43.000000 sinli-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 21:37:53.510726 sinli-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4967 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7220 2023-05-22 21:37:43.000000 sinli-1.1.2/src/sinli/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44158 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 21:37:53.000000 sinli-1.1.2/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 21:37:53.506726 sinli-1.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-22 21:37:43.000000 sinli-1.1.2/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2023-06-27 10:41:00.000000 sinli-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45669 2023-06-27 10:59:01.585718 sinli-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5445 2023-06-27 10:58:52.000000 sinli-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-27 10:58:52.000000 sinli-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 10:59:01.585718 sinli-1.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-27 10:41:00.000000 sinli-1.1.3/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     7392 2023-06-27 10:58:52.000000 sinli-1.1.3/src/sinli/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.581718 sinli-1.1.3/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45669 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 10:59:01.000000 sinli-1.1.3/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:59:01.585718 sinli-1.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-27 10:41:00.000000 sinli-1.1.3/tests/test_document.py
```

### Comparing `sinli-1.1.2/LICENSE` & `sinli-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/PKG-INFO` & `sinli-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.2
+Version: 1.1.3
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,14 +708,76 @@
 SINLI documents or messages are text-based, one file each, and line-based. There is no special syntax, instead, each line is to be processed separately,
 and the different fields in each line are split by their byte position in the line. Therefore, each field has a fixed lenght. In fields where the data has variable lenght, the data is padded with spaces in case of text, and ascii 0 characters in case of numerical fields.
 
 ### SINLI versions
 
 There are no standard-wide versions in SINLI. Instead, each message type has its own version number. New versions are meant to be backwards compatible to older clients. The standaring committee tries to only add fields at the end of the line, not modifying the lengths or meanings of the existing ones. However, they do not commit to it and call for "get what you can" and for a human check before importing to a system. We support implementing different versions of a document type and parsing them accordingly, but will only implement older versions in a case by case basis. SINLI editors do not like developers implementing old versions because in their opinion, it makes users lazier to update. Because of this and other reasons, older versions specifications are not publicly available.
 
+## Example code
+
+Read a document from a SINLI file
+```python
+from sinli import Document
+
+d = Document.from_filename("/path/to/document.sinli")
+```
+
+Generate a SINLI document
+```python
+from sinli import *
+from stdnum import isbn
+
+# Create a catalog document
+catalog = libros.v9.LibrosDoc()
+catalog.long_id_line.FROM = "LIB12345"
+catalog.long_id_line.TO = "LIB98765"
+catalog.short_id_line.FROM = "sinli@provider.example.org"
+catalog.short_id_line.TO = "sinli@library.example.org"
+
+# Create the header line of the doc
+header = libros.v9.LibrosDoc.Header()
+header.TYPE = "C"
+header.PROVIDER = "Traficantes de Sueños"
+header.CURRENCY = "E"
+
+catalog.doc_lines.append(header)
+                                                                               
+# Create one book for the catalog document                                     
+book = libros.v9.LibrosDoc.Book()
+
+book.EAN = "9788494597879"
+book.ISBN_INVOICE = isbn.format(book.EAN)
+book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
+book.TITLE_FULL = "Horizontes comunitario-populares"
+book.PRICE_PV = 12.00
+book.TAX_IVA = 4.00
+book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
+book.PRICE_TYPE = "F"
+
+catalog.doc_lines.append(book)
+
+# Final details
+catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
+```
+
+Export a SINLI document object to string
+```python
+import sinli
+
+catalog: libros.v9.LibrosDoc
+
+# ...
+
+# SINLI message string
+print(str(catalog))
+
+# Debugging string
+print(repr(catalog))
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.2/README.md` & `sinli-1.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -35,14 +35,76 @@
 SINLI documents or messages are text-based, one file each, and line-based. There is no special syntax, instead, each line is to be processed separately,
 and the different fields in each line are split by their byte position in the line. Therefore, each field has a fixed lenght. In fields where the data has variable lenght, the data is padded with spaces in case of text, and ascii 0 characters in case of numerical fields.
 
 ### SINLI versions
 
 There are no standard-wide versions in SINLI. Instead, each message type has its own version number. New versions are meant to be backwards compatible to older clients. The standaring committee tries to only add fields at the end of the line, not modifying the lengths or meanings of the existing ones. However, they do not commit to it and call for "get what you can" and for a human check before importing to a system. We support implementing different versions of a document type and parsing them accordingly, but will only implement older versions in a case by case basis. SINLI editors do not like developers implementing old versions because in their opinion, it makes users lazier to update. Because of this and other reasons, older versions specifications are not publicly available.
 
+## Example code
+
+Read a document from a SINLI file
+```python
+from sinli import Document
+
+d = Document.from_filename("/path/to/document.sinli")
+```
+
+Generate a SINLI document
+```python
+from sinli import *
+from stdnum import isbn
+
+# Create a catalog document
+catalog = libros.v9.LibrosDoc()
+catalog.long_id_line.FROM = "LIB12345"
+catalog.long_id_line.TO = "LIB98765"
+catalog.short_id_line.FROM = "sinli@provider.example.org"
+catalog.short_id_line.TO = "sinli@library.example.org"
+
+# Create the header line of the doc
+header = libros.v9.LibrosDoc.Header()
+header.TYPE = "C"
+header.PROVIDER = "Traficantes de Sueños"
+header.CURRENCY = "E"
+
+catalog.doc_lines.append(header)
+                                                                               
+# Create one book for the catalog document                                     
+book = libros.v9.LibrosDoc.Book()
+
+book.EAN = "9788494597879"
+book.ISBN_INVOICE = isbn.format(book.EAN)
+book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
+book.TITLE_FULL = "Horizontes comunitario-populares"
+book.PRICE_PV = 12.00
+book.TAX_IVA = 4.00
+book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
+book.PRICE_TYPE = "F"
+
+catalog.doc_lines.append(book)
+
+# Final details
+catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
+```
+
+Export a SINLI document object to string
+```python
+import sinli
+
+catalog: libros.v9.LibrosDoc
+
+# ...
+
+# SINLI message string
+print(str(catalog))
+
+# Debugging string
+print(repr(catalog))
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.2/pyproject.toml` & `sinli-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.1.2"
+version = "1.1.3"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.1.2/src/sinli/common/encoded_values.py` & `sinli-1.1.3/src/sinli/common/encoded_values.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/doctype/__init__.py` & `sinli-1.1.3/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/doctype/envio/v8.py` & `sinli-1.1.3/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/doctype/factul/v1.py` & `sinli-1.1.3/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/doctype/libros/v8.py` & `sinli-1.1.3/src/sinli/doctype/libros/v8.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from ...document import Document
 from ...line import Line
 from ...common import SinliCode as c
 from ...common import BasicType as t
 from enum import Enum
 from dataclasses import dataclass, field
 
-@dataclass
 class LibrosDoc(Document):
     class Header(Line):
         class Field(Enum):
             TYPE = (0, 1, t.STR, "Tipo de Registro")
             PROVIDER = (1, 40, t.STR, "Nombre del proveedor")
             CURRENCY = (41, 1, t.CURRENCY1, "Moneda")
 
@@ -34,17 +33,17 @@
             PAGE_NUM = (474, 4, t.INT, "Número de páginas")
             WIDTH_MM = (478, 4, t.INT, "Ancho en mm.")
             HEIGH_MM = (482, 4, t.INT, "Alto en mm.")
             TOPICS = (486, 20, t.STR, "Temas separados por ';' en códigos CDU o ISBN")
             KEYWORDS = (506, 80, t.STR, "Palabras clave o descriptores, separadas por '/'")
             STATUS = (586, 1, c.STATUS, "Código de situación en catálogo", )
             PRODUCT_TYPE = (587, 2, c.PRODUCT_TYPE, "Código de tipo de producto")
-            PRICE_PVP = (589, 10, t.INT, "PVP sin IVA en EUR (sin puntuación)")
-            PRICE_PV = (599, 10, t.INT, "PV con IVA en EUR (sin puntuación)")
-            TAX_IVA = (609, 5, t.INT, "Porcentaje de IVA (ej: 4, 16, 21, ...)")
+            PRICE_PVP = (589, 10, t.FLOAT, "PVP sin IVA en EUR (sin puntuación)")
+            PRICE_PV = (599, 10, t.FLOAT, "PV con IVA en EUR (sin puntuación)")
+            TAX_IVA = (609, 5, t.FLOAT, "Porcentaje de IVA (ej: 4, 16, 21, ...)")
             PRICE_TYPE = (614, 1, t.STR, "Tipo de precio. F = Fijo, L = Libre. Si es L, el precio sin IVA será el precio de cesión, y el precio con IVA, el precio de sesión más el IVA correspondiente")
             COLLECTION = (615, 40, t.STR, "Nombre de la colección")
             COL_NUM = (655, 10, t.STR, "Número de colección")
             VOL_NUM = (665, 4, t.STR, "Número de volumen")
             COVER_IMAGE = (669, 1, t.STR, "Fuente de la imagen de portada y/u otras. N = No; A = Anexada, debe ser en jpg, pesar menos de 500 KB, y el nombre del fichero adjunto con la/las imágenes será el código EAN13; U = URL")
             COVER_ILLUSTRATOR = (670, 150, t.STR, "Lista de ilustradores de la cubierta en formato 'Apellidos, Nombre' y separados por '/'")
             INNER_ILLUSTRATOR = (820, 150, t.STR, "Lista de ilustradores del interior en formato 'Apellidos, Nombre' y separados por '/'")
```

### Comparing `sinli-1.1.2/src/sinli/doctype/libros/v9.py` & `sinli-1.1.3/src/sinli/doctype/libros/v9.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
             PAGE_NUM = (474, 4, t.INT, "Número de páginas")
             WIDTH_MM = (478, 4, t.INT, "Ancho en mm.")
             HEIGH_MM = (482, 4, t.INT, "Alto en mm.")
             TOPICS = (486, 20, t.STR, "Temas separados por ';' en códigos CDU o ISBN")
             KEYWORDS = (506, 80, t.STR, "Palabras clave o descriptores, separadas por '/'")
             STATUS = (586, 1, c.STATUS, "Código de situación en catálogo", )
             PRODUCT_TYPE = (587, 2, c.PRODUCT_TYPE, "Código de tipo de producto")
-            PRICE_PVP = (589, 10, t.INT, "PVP sin IVA en EUR (sin puntuación)")
-            PRICE_PV = (599, 10, t.INT, "PV con IVA en EUR (sin puntuación)")
-            TAX_IVA = (609, 5, t.INT, "Porcentaje de IVA (ej: 4, 16, 21, ...)")
+            PRICE_PVP = (589, 10, t.FLOAT, "PVP sin IVA en EUR (sin puntuación)")
+            PRICE_PV = (599, 10, t.FLOAT, "PV con IVA en EUR (sin puntuación)")
+            TAX_IVA = (609, 5, t.FLOAT, "Porcentaje de IVA (ej: 4, 16, 21, ...)")
             PRICE_TYPE = (614, 1, t.STR, "Tipo de precio. F = Fijo, L = Libre. Si es L, el precio sin IVA será el precio de cesión, y el precio con IVA, el precio de sesión más el IVA correspondiente")
             COLLECTION = (615, 40, t.STR, "Nombre de la colección")
             COL_NUM = (655, 10, t.STR, "Número de colección")
             VOL_NUM = (665, 4, t.STR, "Número de volumen")
             COVER_IMAGE = (669, 1, t.STR, "Fuente de la imagen de portada y/u otras. N = No; A = Anexada, debe ser en jpg, pesar menos de 500 KB, y el nombre del fichero adjunto con la/las imágenes será el código EAN13; U = URL")
             COVER_ILLUSTRATOR = (670, 150, t.STR, "Lista de ilustradores de la cubierta en formato 'Apellidos, Nombre' y separados por '/'")
             INNER_ILLUSTRATOR = (820, 150, t.STR, "Lista de ilustradores del interior en formato 'Apellidos, Nombre' y separados por '/'")
```

### Comparing `sinli-1.1.2/src/sinli/doctype/mensaj/v1.py` & `sinli-1.1.3/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/doctype/pedido/v7.py` & `sinli-1.1.3/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.2/src/sinli/document.py` & `sinli-1.1.3/src/sinli/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,45 @@
 from dataclasses import dataclass, field
 
 # module
 from .line import LongIdentificationLine, ShortIdentificationLine, Line
 
 @dataclass
 class Document:
-    long_id_line: LongIdentificationLine = field(default=LongIdentificationLine())
-    short_id_line: ShortIdentificationLine = field(default=ShortIdentificationLine())
+    long_id_line: LongIdentificationLine = field(default_factory=LongIdentificationLine)
+    short_id_line: ShortIdentificationLine = field(default_factory=ShortIdentificationLine)
     doc_lines: List[Line] = field(default_factory=list)
     linemap = {}
+    doctype_codes = {}
+    doctype_code = ""
+    version_code = ""
+
+    def get_doctype_version(self) -> str:
+        """
+        Produces the sinli version string, like "09"
+        from the package of the instance class, such as sinli.libros.v9
+        """
+        pkg = self.__class__.__module__
+        version_code = pkg.split('.')[-1]
+        return version_code.replace('v', '').zfill(2)
 
     def __post_init__(self):
-        self.long_id_line.TYPE = "I"
-        self.long_id_line.FANDE = "FANDE"
-        self.short_id_line.TYPE = "I"
+        from .doctype import DocumentType
+        for doctype in DocumentType:
+            name = doctype.name
+            version_map = doctype.value[1]
+            if not version_map: continue
+            if version_map['??'] == self.__class__:
+                self.doctype_code = name
+
+        self.version_code = self.get_doctype_version()
+        self.long_id_line.DOCTYPE = self.doctype_code
+        self.long_id_line.VERSION = self.version_code
+        self.short_id_line.DOCTYPE = self.doctype_code
+        self.short_id_line.VERSION = self.version_code
 
     def consume_line(line: str, doc: Self) -> Self:
         print(f"\n[DEBUG] line: '{line}'")
 
         tdoc = line[0:1]
         if tdoc == "I" and not doc.long_id_line.FROM: # generic processing, we still don't know the doctype:  # Long id
             doc.long_id_line = LongIdentificationLine.from_str(line)
```

### Comparing `sinli-1.1.2/src/sinli/line.py` & `sinli-1.1.3/src/sinli/line.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,18 @@
         try:
             return str(c.get(k).value[0].get(v) or c.get(k).value[0].get("??"))
         except:
             return str(v)
         return str(v)
 
 class LongIdentificationLine(Line):
+    def __post_init__(self):
+        super().__post_init__()
+        self.TYPE = "I"
+
     class Field(Enum):
         TYPE = (0, 1, t.STR, "Tipo de registro (I)")
         FORMAT = (1, 1, t.STR, "Tipo de formato (N=Normalizado ; ?=Libre)")
         DOCTYPE = (2, 6, t.STR, "Nombre del tipo de documento")
         VERSION = (8, 2, t.STR, "Versión del tipo de documento")
         FROM = (10, 8, t.STR, "Identificador ESFANDE del remitente")
         TO = (18, 8, t.STR, "Identificador ESFANDE del destinatario")
@@ -179,14 +183,18 @@
         NUM_TRANS = (31, 7, t.INT, "Número de transmisión s/emisor")
         LOCAL_FROM = (38, 15, t.STR, "Usuario local del emisor")
         LOCAL_TO = (53, 15, t.STR, "Usuario local del destino")
         TEXT = (68, 7, t.STR, "Texto libre")
         FANDE = (75, 5, t.STR, "FANDE")
 
 class ShortIdentificationLine(Line):
+    def __post_init__(self):
+        super().__post_init__()
+        self.TYPE = "I"
+
     class Field(Enum):
         TYPE = (0, 1, t.STR, "Tipo de registro (I)")
         FROM = (1, 50, t.STR, "E-mail origen")
         TO = (51, 50, t.STR, "E-mail destino")
         DOCTYPE = (101, 6, t.STR, "Tipo de Fichero")
         VERSION = (107, 2, t.STR, "Versión fichero")
         TRANSMISION_NUMBER = (109, 8, t.INT, "Nº de transmisión emisor")
```

### Comparing `sinli-1.1.2/src/sinli.egg-info/PKG-INFO` & `sinli-1.1.3/src/sinli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.2
+Version: 1.1.3
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -708,14 +708,76 @@
 SINLI documents or messages are text-based, one file each, and line-based. There is no special syntax, instead, each line is to be processed separately,
 and the different fields in each line are split by their byte position in the line. Therefore, each field has a fixed lenght. In fields where the data has variable lenght, the data is padded with spaces in case of text, and ascii 0 characters in case of numerical fields.
 
 ### SINLI versions
 
 There are no standard-wide versions in SINLI. Instead, each message type has its own version number. New versions are meant to be backwards compatible to older clients. The standaring committee tries to only add fields at the end of the line, not modifying the lengths or meanings of the existing ones. However, they do not commit to it and call for "get what you can" and for a human check before importing to a system. We support implementing different versions of a document type and parsing them accordingly, but will only implement older versions in a case by case basis. SINLI editors do not like developers implementing old versions because in their opinion, it makes users lazier to update. Because of this and other reasons, older versions specifications are not publicly available.
 
+## Example code
+
+Read a document from a SINLI file
+```python
+from sinli import Document
+
+d = Document.from_filename("/path/to/document.sinli")
+```
+
+Generate a SINLI document
+```python
+from sinli import *
+from stdnum import isbn
+
+# Create a catalog document
+catalog = libros.v9.LibrosDoc()
+catalog.long_id_line.FROM = "LIB12345"
+catalog.long_id_line.TO = "LIB98765"
+catalog.short_id_line.FROM = "sinli@provider.example.org"
+catalog.short_id_line.TO = "sinli@library.example.org"
+
+# Create the header line of the doc
+header = libros.v9.LibrosDoc.Header()
+header.TYPE = "C"
+header.PROVIDER = "Traficantes de Sueños"
+header.CURRENCY = "E"
+
+catalog.doc_lines.append(header)
+                                                                               
+# Create one book for the catalog document                                     
+book = libros.v9.LibrosDoc.Book()
+
+book.EAN = "9788494597879"
+book.ISBN_INVOICE = isbn.format(book.EAN)
+book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
+book.TITLE_FULL = "Horizontes comunitario-populares"
+book.PRICE_PV = 12.00
+book.TAX_IVA = 4.00
+book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
+book.PRICE_TYPE = "F"
+
+catalog.doc_lines.append(book)
+
+# Final details
+catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
+```
+
+Export a SINLI document object to string
+```python
+import sinli
+
+catalog: libros.v9.LibrosDoc
+
+# ...
+
+# SINLI message string
+print(str(catalog))
+
+# Debugging string
+print(repr(catalog))
+```
+
 ## Goals
 
 ### Generic
 
 - [x] Basic architecture for reading documents and lines
 - [x] Read LIBRO doctype
 - [x] Prepare the repo as an importable python package
```

### Comparing `sinli-1.1.2/src/sinli.egg-info/SOURCES.txt` & `sinli-1.1.3/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

