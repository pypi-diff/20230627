# Comparing `tmp/psalpsdtools-0.5.tar.gz` & `tmp/psalpsdtools-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psalpsdtools-0.5.tar", last modified: Mon Jun 26 09:28:36 2023, max compression
+gzip compressed data, was "psalpsdtools-0.6.tar", last modified: Tue Jun 27 12:31:01 2023, max compression
```

## Comparing `psalpsdtools-0.5.tar` & `psalpsdtools-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.860101 psalpsdtools-0.5/
--rw-rw-rw-   0        0        0      118 2023-06-26 09:28:36.860101 psalpsdtools-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.844580 psalpsdtools-0.5/psalpsdtools/
--rw-rw-rw-   0        0        0     6990 2023-06-26 09:25:25.000000 psalpsdtools-0.5/psalpsdtools/Edrw.py
--rw-rw-rw-   0        0        0     3561 2023-06-26 09:28:20.000000 psalpsdtools-0.5/psalpsdtools/PhRegPrv.py
--rw-rw-rw-   0        0        0       54 2023-06-26 08:56:22.000000 psalpsdtools-0.5/psalpsdtools/__init__.py
--rw-rw-rw-   0        0        0      343 2023-06-26 09:28:12.000000 psalpsdtools-0.5/psalpsdtools/usage.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.860101 psalpsdtools-0.5/psalpsdtools.egg-info/
--rw-rw-rw-   0        0        0      118 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 09:28:36.860101 psalpsdtools-0.5/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-06-26 09:27:56.000000 psalpsdtools-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:31:01.025628 psalpsdtools-0.6/
+-rw-rw-rw-   0        0        0      214 2023-06-27 12:31:01.025628 psalpsdtools-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 12:31:01.009624 psalpsdtools-0.6/psalpsdtools/
+-rw-rw-rw-   0        0        0     7501 2023-06-27 12:28:30.000000 psalpsdtools-0.6/psalpsdtools/Edrw.py
+-rw-rw-rw-   0        0        0     3556 2023-06-26 11:33:05.000000 psalpsdtools-0.6/psalpsdtools/PhRegPrv.py
+-rw-rw-rw-   0        0        0       54 2023-06-26 11:33:05.000000 psalpsdtools-0.6/psalpsdtools/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-06-27 12:28:30.000000 psalpsdtools-0.6/psalpsdtools/usage.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:31:01.025628 psalpsdtools-0.6/psalpsdtools.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-06-27 12:31:00.000000 psalpsdtools-0.6/psalpsdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-27 12:31:00.000000 psalpsdtools-0.6/psalpsdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:31:00.000000 psalpsdtools-0.6/psalpsdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 12:31:00.000000 psalpsdtools-0.6/psalpsdtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-27 12:31:00.000000 psalpsdtools-0.6/psalpsdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:31:01.025628 psalpsdtools-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-27 12:28:30.000000 psalpsdtools-0.6/setup.py
```

### Comparing `psalpsdtools-0.5/psalpsdtools/Edrw.py` & `psalpsdtools-0.6/psalpsdtools/Edrw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 from .PhRegPrv import PhRegPrv
 from openpyxl import load_workbook
 import os
 #import xlrd
 class Edrw:
     def __init__(self):
         pass
-    def update_sources(self, regName, qtr, baseFolder, sdFile):
+    def update_sources(self, regName, qtr, baseFolder, sdFile, commcode, yr):
         philippines = PhRegPrv()
         selected_provinces = philippines.get_provinces(regName)
         src = load_workbook(filename = baseFolder + "/" + sdFile, data_only=True)
         src_active = src["native B"]
         comm_arr = ["native","gamefowl","broiler","layer"]
         srv_arr = [" B"," C","_T"]
 
-        if selected_provinces:
-            for province in selected_provinces:
-                srcFile = '08 ' + str(province) + '_23'
-                fileExt = '.xlsm'
-                fpath = str(baseFolder) + '/Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt)
-                if os.path.isfile(fpath) == True:
-                    for row in src_active.iter_rows(min_row=17, min_col=1, max_row=135, max_col=1):
-                        for cell in row:
-                            if cell.value == province:
-                                #print(f"{province} {cell.row}")
-                                rNumSrc = cell.row
-
-                                dst = load_workbook(filename=str(baseFolder) + '/Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt))
-                                #dst = xlrd.open_workbook('Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt))
-                                q1_dst_ws = dst[qtr]
-                                #q1_dst_ws = dst.sheet_by_name(qtr)
-
-                                if os.path.isfile(fpath) == True:
-                                    for comm in comm_arr:
-                                        for srv in srv_arr:
-                                            if comm == "native":
-                                                if srv == " B":
-                                                    rNumDst = 22
-                                                elif srv == " C":
-                                                    rNumDst = 28
+        if commcode == '08':
+            if selected_provinces:
+                for province in selected_provinces:
+                    srcFile = str(commcode) + ' ' + str(province) + '_' + str(yr)
+                    fileExt = '.xlsm'
+                    fpath = str(baseFolder) + '/Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt)
+                    if os.path.isfile(fpath) == True:
+                        for row in src_active.iter_rows(min_row=17, min_col=1, max_row=135, max_col=1):
+                            for cell in row:
+                                if cell.value == province:
+                                    #print(f"{province} {cell.row}")
+                                    rNumSrc = cell.row
+
+                                    dst = load_workbook(filename=str(baseFolder) + '/Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt))
+                                    #dst = xlrd.open_workbook('Sources/' + str(regName) + '/' + str(srcFile) + str(fileExt))
+                                    q1_dst_ws = dst[qtr]
+                                    #q1_dst_ws = dst.sheet_by_name(qtr)
+
+                                    if os.path.isfile(fpath) == True:
+                                        for comm in comm_arr:
+                                            for srv in srv_arr:
+                                                if comm == "native":
+                                                    if srv == " B":
+                                                        rNumDst = 22
+                                                    elif srv == " C":
+                                                        rNumDst = 28
+                                                    elif srv == "_T":
+                                                        rNumDst = 34
+                                                elif comm == "gamefowl":
+                                                    if srv == " B":
+                                                        rNumDst = 40
+                                                    elif srv == " C":
+                                                        rNumDst = 46
+                                                    elif srv == "_T":
+                                                        rNumDst = 52
+                                                elif comm == "broiler":
+                                                    if srv == " B":
+                                                        rNumDst = 58
+                                                    elif srv == " C":
+                                                        rNumDst = 64
+                                                    elif srv == "_T":
+                                                        rNumDst = 70
+                                                elif comm == "layer":
+                                                    if srv == " B":
+                                                        rNumDst = 76
+                                                    elif srv == " C":
+                                                        rNumDst = 82
+                                                    elif srv == "_T":
+                                                        rNumDst = 88
+
+                                                sheetNameSrc = str(comm) + str(srv)
+                                                qtr_src_ws = src[sheetNameSrc]
+                                                print(f"PSA-LPSD (EDRW): Loading source -> {province} - {comm} - {srv}")
+
+                                                if srv != "_T":
+                                                    #print(f"Copying Source B{rNumSrc} to E{rNumDst}")
+                                                    q1_dst_ws['E' + str(rNumDst)].value = qtr_src_ws['B' + str(rNumSrc)].value
+                                                    q1_dst_ws['F' + str(rNumDst)].value = qtr_src_ws['C' + str(rNumSrc)].value
+                                                    q1_dst_ws['H' + str(rNumDst)].value = qtr_src_ws['E' + str(rNumSrc)].value
+                                                    q1_dst_ws['I' + str(rNumDst)].value = qtr_src_ws['F' + str(rNumSrc)].value
+                                                    q1_dst_ws['J' + str(rNumDst)].value = qtr_src_ws['G' + str(rNumSrc)].value
+                                                    q1_dst_ws['M' + str(rNumDst)].value = qtr_src_ws['J' + str(rNumSrc)].value
+                                                    q1_dst_ws['N' + str(rNumDst)].value = qtr_src_ws['K' + str(rNumSrc)].value
+                                                    q1_dst_ws['Q' + str(rNumDst)].value = qtr_src_ws['N' + str(rNumSrc)].value
+                                                    q1_dst_ws['R' + str(rNumDst)].value = qtr_src_ws['U' + str(rNumSrc)].value
+                                                    q1_dst_ws['S' + str(rNumDst)].value = qtr_src_ws['V' + str(rNumSrc)].value
+                                                    q1_dst_ws['V' + str(rNumDst)].value = qtr_src_ws['Y' + str(rNumSrc)].value
+                                                    q1_dst_ws['X' + str(rNumDst)].value = qtr_src_ws['AA' + str(rNumSrc)].value
                                                 elif srv == "_T":
-                                                    rNumDst = 34
-                                            elif comm == "gamefowl":
-                                                if srv == " B":
-                                                    rNumDst = 40
-                                                elif srv == " C":
-                                                    rNumDst = 46
-                                                elif srv == "_T":
-                                                    rNumDst = 52
-                                            elif comm == "broiler":
-                                                if srv == " B":
-                                                    rNumDst = 58
-                                                elif srv == " C":
-                                                    rNumDst = 64
-                                                elif srv == "_T":
-                                                    rNumDst = 70
-                                            elif comm == "layer":
-                                                if srv == " B":
-                                                    rNumDst = 76
-                                                elif srv == " C":
-                                                    rNumDst = 82
-                                                elif srv == "_T":
-                                                    rNumDst = 88
-
-                                            sheetNameSrc = str(comm) + str(srv)
-                                            qtr_src_ws = src[sheetNameSrc]
-                                            print(f"PSA-LPSD (EDRW): Loading source -> {province} - {comm} - {srv}")
-
-                                            if srv != "_T":
-                                                #print(f"Copying Source B{rNumSrc} to E{rNumDst}")
-                                                q1_dst_ws['E' + str(rNumDst)].value = qtr_src_ws['B' + str(rNumSrc)].value
-                                                q1_dst_ws['F' + str(rNumDst)].value = qtr_src_ws['C' + str(rNumSrc)].value
-                                                q1_dst_ws['H' + str(rNumDst)].value = qtr_src_ws['E' + str(rNumSrc)].value
-                                                q1_dst_ws['I' + str(rNumDst)].value = qtr_src_ws['F' + str(rNumSrc)].value
-                                                q1_dst_ws['J' + str(rNumDst)].value = qtr_src_ws['G' + str(rNumSrc)].value
-                                                q1_dst_ws['M' + str(rNumDst)].value = qtr_src_ws['J' + str(rNumSrc)].value
-                                                q1_dst_ws['N' + str(rNumDst)].value = qtr_src_ws['K' + str(rNumSrc)].value
-                                                q1_dst_ws['Q' + str(rNumDst)].value = qtr_src_ws['N' + str(rNumSrc)].value
-                                                q1_dst_ws['R' + str(rNumDst)].value = qtr_src_ws['U' + str(rNumSrc)].value
-                                                q1_dst_ws['S' + str(rNumDst)].value = qtr_src_ws['V' + str(rNumSrc)].value
-                                                q1_dst_ws['V' + str(rNumDst)].value = qtr_src_ws['Y' + str(rNumSrc)].value
-                                                q1_dst_ws['X' + str(rNumDst)].value = qtr_src_ws['AA' + str(rNumSrc)].value
-                                            elif srv == "_T":
-                                                if comm == "native" or comm == "broiler" or comm == "layer":
-                                                    q1_dst_ws['AA' + str(rNumDst)].value = qtr_src_ws['AD' + str(rNumSrc)].value
-                                                if comm == "broiler" or comm == "layer":
-                                                    q1_dst_ws['AC' + str(rNumDst)].value = qtr_src_ws['AF' + str(rNumSrc)].value
-                                            print(f"PSA-LPSD (EDRW): Copied to destination -> {province} - {comm} - {srv} at row {rNumSrc}")
-
-                                    fpath = str(baseFolder) + '/Final/' + str(regName)
-                                    if os.path.isdir(fpath) == False:
-                                        os.mkdir(fpath)
-                                    finalFile = str(baseFolder) + '/Final/' + str(regName) + '/08 ' + str(province) + '_23.xls'
-                                    print(f"PSA-LPSD (EDRW): Saving to file -> {finalFile}")
-                                    dst.save(finalFile)
-                                else:
-                                    print(f"File {srcFile}{fileExt} Not Found.")
-                else:
-                    print(f"File {srcFile}{fileExt} Not Found.")
+                                                    if comm == "native" or comm == "broiler" or comm == "layer":
+                                                        q1_dst_ws['AA' + str(rNumDst)].value = qtr_src_ws['AD' + str(rNumSrc)].value
+                                                    if comm == "broiler" or comm == "layer":
+                                                        q1_dst_ws['AC' + str(rNumDst)].value = qtr_src_ws['AF' + str(rNumSrc)].value
+                                                print(f"PSA-LPSD (EDRW): Copied to destination -> {province} - {comm} - {srv} at row {rNumSrc}")
+
+                                        fpath = str(baseFolder) + '/Final/' + str(regName)
+                                        if os.path.isdir(fpath) == False:
+                                            os.mkdir(fpath)
+                                        finalFile = str(baseFolder) + '/Final/' + str(regName) + '/' + str(commcode) + ' ' + str(province) + '_' + str(yr) + '.xls'
+                                        print(f"PSA-LPSD (EDRW): Saving to file -> {finalFile}")
+                                        dst.save(finalFile)
+                                    else:
+                                        print(f"File {srcFile}{fileExt} Not Found.")
+                    else:
+                        print(f"File {srcFile}{fileExt} Not Found.")
+            else:
+                print("Region not found or has no provinces.")
         else:
-            print("Region not found or has no provinces.")
+            print(f"Commodity code {commcode} not found.")
+
```

### Comparing `psalpsdtools-0.5/psalpsdtools/PhRegPrv.py` & `psalpsdtools-0.6/psalpsdtools/PhRegPrv.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 "Bukidnon",
                 "Camiguin",
                 "Lanao del Norte",
                 "Misamis Occidental",
                 "Misamis Oriental"
             ],
             "Davao Region": [
-                "Compostela Valley",
+                "Davao de Oro",
                 "Davao del Norte",
                 "Davao del Sur",
                 "Davao Occidental",
                 "Davao Oriental"
             ],
             "SOCCSKSARGEN": [
                 "Cotabato",
```

