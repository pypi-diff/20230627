# Comparing `tmp/genopyc-1.1.4-py3-none-any.whl.zip` & `tmp/genopyc-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 424193 bytes, number of entries: 8
+Zip file size: 424202 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      978 b- defN 23-Jun-24 20:45 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    42535 b- defN 23-Jun-24 21:02 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    42568 b- defN 23-Jun-27 08:49 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/RECORD
-8 files, 1381467 bytes uncompressed, 423093 bytes compressed:  69.4%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/RECORD
+8 files, 1381500 bytes uncompressed, 423102 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.1.4.dist-info/LICENSE.txt
+Filename: genopyc-1.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.1.4.dist-info/METADATA
+Filename: genopyc-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.1.4.dist-info/WHEEL
+Filename: genopyc-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.1.4.dist-info/top_level.txt
+Filename: genopyc-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.1.4.dist-info/RECORD
+Filename: genopyc-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -1,11 +1,12 @@
 import requests
 import pandas as pd
 import biomapy as bp
 import os
+import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 import matplotlib
 import requests
 from gprofiler import GProfiler
 import igraph as ig 
@@ -14,14 +15,15 @@
 import dash
 import dash_core_components as dcc
 import dash_html_components as html
 from dash.dependencies import Input,Output
 import dash_cytoscape as cyto
 
 
+
 def get_associations(efotrait,verbose=False):
     """Retrieve snps associated to an EFO trait"""
     df=pd.DataFrame(columns=['variantid','p-value','risk_allele','RAF','beta','CI','mapped_gene'])
     http= 'https://www.ebi.ac.uk/gwas/rest/api/efoTraits/%s/associations' %(efotrait)
     if verbose:
         print('querying associations... \n')
     resp=requests.get(http)
```

## Comparing `genopyc-1.1.4.dist-info/LICENSE.txt` & `genopyc-1.1.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.1.4.dist-info/METADATA` & `genopyc-1.1.5.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.1.4
+Version: 1.1.5
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

## Comparing `genopyc-1.1.4.dist-info/RECORD` & `genopyc-1.1.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 genopyc/__init__.py,sha256=njXl6cbbGkaY8POLyttPL5C6oBSA9LENNwW1zhzKHvE,978
-genopyc/genopyc.py,sha256=xl-V8kwxQhVruqhoc25gpbuG5NFieNT2xcUBdC3BJCA,42535
+genopyc/genopyc.py,sha256=UkfwGGEldnbkvb5Wlxfs_DSUgBthfiXs46Cv28nAVJk,42568
 genopyc/data/hippie_interactome.sif,sha256=iqdnCWTnTXIs43-jMLNijQ2PJWd7CRSVMHnh8miE1vs,1302100
-genopyc-1.1.4.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-1.1.4.dist-info/METADATA,sha256=urmBb1062jrGqW7jCy5VEUzivRGqQ1xWwQzhr23GfUs,596
-genopyc-1.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-1.1.4.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-1.1.4.dist-info/RECORD,,
+genopyc-1.1.5.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-1.1.5.dist-info/METADATA,sha256=k186vfjYuWHaaQA63AZBYpnXm2Q2xxvMhbJ0h3enAHI,596
+genopyc-1.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-1.1.5.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-1.1.5.dist-info/RECORD,,
```

