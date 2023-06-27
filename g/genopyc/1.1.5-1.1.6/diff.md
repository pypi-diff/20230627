# Comparing `tmp/genopyc-1.1.5-py3-none-any.whl.zip` & `tmp/genopyc-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 424202 bytes, number of entries: 8
+Zip file size: 424218 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      978 b- defN 23-Jun-24 20:45 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    42568 b- defN 23-Jun-27 08:49 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    42603 b- defN 23-Jun-27 09:05 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-27 08:49 genopyc-1.1.5.dist-info/RECORD
-8 files, 1381500 bytes uncompressed, 423102 bytes compressed:  69.4%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-27 09:08 genopyc-1.1.6.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-27 09:08 genopyc-1.1.6.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-27 09:08 genopyc-1.1.6.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-27 09:07 genopyc-1.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-27 09:08 genopyc-1.1.6.dist-info/RECORD
+8 files, 1381535 bytes uncompressed, 423118 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.1.5.dist-info/LICENSE.txt
+Filename: genopyc-1.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.1.5.dist-info/METADATA
+Filename: genopyc-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.1.5.dist-info/WHEEL
+Filename: genopyc-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.1.5.dist-info/top_level.txt
+Filename: genopyc-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.1.5.dist-info/RECORD
+Filename: genopyc-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -31,15 +31,15 @@
         associ=resp.json()
         if verbose:
             print('building the dataframe...')
         for i,element in enumerate(associ['_embedded']['associations']):
             try:
                 df.at[i,'variantid']=''.join(element['loci'][0]['strongestRiskAlleles'][0]['riskAlleleName'].split('-')[0:1])
                 df.at[i,'risk_allele']=element['loci'][0]['strongestRiskAlleles'][0]['riskAlleleName'].split('-')[-1]
-                df.at[i,'mapped_gene']=[e['geneName'] for e in element['loci'][0]['authorReportedGenes']]
+                df.at[i,'mapped_gene']= ' '.join([str(elem) for elem in [e['geneName'] for e in element['loci'][0]['authorReportedGenes']]])
                 df.at[i,'p-value']=float(element['pvalueMantissa'])*10**int(element['pvalueExponent'])
                 try: 
                     df.at[i,'RAF']=float(element['riskFrequency'])
                 except:
                     df.at[i,'RAF']=np.nan
                     
                 df.at[i,'beta']=[float(element['betaNum']) if type(element['betaNum'])==float else np.nan][0]
```

## Comparing `genopyc-1.1.5.dist-info/LICENSE.txt` & `genopyc-1.1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.1.5.dist-info/METADATA` & `genopyc-1.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.1.5
+Version: 1.1.6
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

