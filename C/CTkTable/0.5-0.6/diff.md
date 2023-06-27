# Comparing `tmp/CTkTable-0.5.tar.gz` & `tmp/CTkTable-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkTable-0.5.tar", last modified: Fri Jun 23 16:32:18 2023, max compression
+gzip compressed data, was "CTkTable-0.6.tar", last modified: Tue Jun 27 06:10:13 2023, max compression
```

## Comparing `CTkTable-0.5.tar` & `CTkTable-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:32:18.409017 CTkTable-0.5/
-drwxrwxrwx   0        0        0        0 2023-06-23 16:32:18.382084 CTkTable-0.5/CTkTable/
--rw-rw-rw-   0        0        0      227 2023-06-23 16:31:27.000000 CTkTable-0.5/CTkTable/__init__.py
--rw-rw-rw-   0        0        0    12941 2023-06-23 16:31:16.000000 CTkTable-0.5/CTkTable/ctktable.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:32:18.408237 CTkTable-0.5/CTkTable.egg-info/
--rw-rw-rw-   0        0        0     3348 2023-06-23 16:32:18.000000 CTkTable-0.5/CTkTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-23 16:32:18.000000 CTkTable-0.5/CTkTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-06-23 16:32:18.000000 CTkTable-0.5/CTkTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-23 16:32:18.000000 CTkTable-0.5/CTkTable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 16:32:18.000000 CTkTable-0.5/CTkTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.5/LICENSE
--rw-rw-rw-   0        0        0     3348 2023-06-23 16:32:18.409017 CTkTable-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2762 2023-06-22 11:03:43.000000 CTkTable-0.5/README.md
--rw-rw-rw-   0        0        0      519 2023-06-23 16:32:18.409017 CTkTable-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-06-23 16:31:49.000000 CTkTable-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.703554 CTkTable-0.6/
+drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.687886 CTkTable-0.6/CTkTable/
+-rw-rw-rw-   0        0        0      227 2023-06-27 06:09:31.000000 CTkTable-0.6/CTkTable/__init__.py
+-rw-rw-rw-   0        0        0    13103 2023-06-27 06:06:40.000000 CTkTable-0.6/CTkTable/ctktable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:10:13.703554 CTkTable-0.6/CTkTable.egg-info/
+-rw-rw-rw-   0        0        0     3348 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 06:10:13.000000 CTkTable-0.6/CTkTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.6/LICENSE
+-rw-rw-rw-   0        0        0     3348 2023-06-27 06:10:13.703554 CTkTable-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2762 2023-06-22 11:03:43.000000 CTkTable-0.6/README.md
+-rw-rw-rw-   0        0        0      519 2023-06-27 06:10:13.719180 CTkTable-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-06-27 06:09:44.000000 CTkTable-0.6/setup.py
```

### Comparing `CTkTable-0.5/CTkTable/ctktable.py` & `CTkTable-0.6/CTkTable/ctktable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # CTkTable Widget by Akascape
 # License: MIT
 # Author: Akash Bora
 
 import customtkinter
+import copy
 
 class CTkTable(customtkinter.CTkFrame):
     """ CTkTable Widget """
     
     def __init__(
         self,
         master: any,
@@ -45,18 +46,20 @@
         self.header_color = header_color # specify the topmost row color
         self.phase = color_phase
         self.corner = corner_radius
         self.write = write
         self.justify = justify
         if self.write:
             border_width = border_width=+1
-        if hover_color:
+        if hover_color is not None:
             hover=True
+        else:
+            hover=False
         self.anchor = anchor
-        self.hover = hover
+        self.hover = hover 
         self.border_width = border_width
         self.hover_color = customtkinter.ThemeManager.theme["CTkButton"]["hover_color"] if hover_color is None else hover_color
         self.orient = orientation
         self.border_color = customtkinter.ThemeManager.theme["CTkButton"]["border_color"] if border_color is None else border_color
         self.text_color = customtkinter.ThemeManager.theme["CTkButton"]["text_color"] if text_color is None else text_color
         self.font = font
         # if colors are None then use the default frame colors:
@@ -115,43 +118,44 @@
                         if self.orient=="horizontal":
                             value = self.values[i][j]
                         else:
                             value = self.values[j][i]
                     except IndexError: value = " "
                 else:
                     value = " "
-
+                
                 if (i,j) in self.data.keys():
                     if self.data[i,j]["args"]: 
                         args = self.data[i,j]["args"]
                     else:
-                        args = kwargs
+                        args = copy.deepcopy(kwargs)
                 else:
-                    args = kwargs
+                    args = copy.deepcopy(kwargs)
                 
-                self.data[i,j] = {"row": i, "column" : j, "value" : value, "args": args }
+                self.data[i,j] = {"row": i, "column" : j, "value" : value, "args": args}
                 
                 args = self.data[i,j]["args"]
-                
 
                 if "text_color" not in args:
                     args["text_color"] = self.text_color
                 if "border_width" not in args:
                     args["border_width"] = self.border_width
                 if "border_color" not in args:
                     args["border_color"] = self.border_color
-                
+                if "fg_color" not in args:
+                    args["fg_color"] = fg
+
                 if self.write:
                     if "justify" not in args:
                         args["justify"] = self.justify
                     if self.padx==1: self.padx=0
                     self.frame[i,j] = customtkinter.CTkEntry(self,
                                                              font=self.font,
                                                              corner_radius=0,
-                                                             fg_color=fg, **args)
+                                                             **args)
                     self.frame[i,j].insert("0", value)
                     self.frame[i,j].bind("<Key>", lambda e, row=i, column=j, data=self.data: self.after(100, lambda: self.manipulate_data(row, column)))
                     self.frame[i,j].grid(column=j, row=i, padx=self.padx, pady=self.pady, sticky="nsew")
                     if self.header_color:
                         if i==0:
                             self.frame[i,j].configure(state="readonly")
     
@@ -161,15 +165,15 @@
                     if "hover_color" not in args:
                         args["hover_color"] = self.hover_color
                     if "hover" not in args:
                         args["hover"] = self.hover
                     self.frame[i,j] = customtkinter.CTkButton(self, background_corner_colors=corners,
                                                               font=self.font, 
                                                               corner_radius=corner_radius,
-                                                              fg_color=fg, text=value, 
+                                                              text=value, 
                                                               command=(lambda e=self.data[i,j]: self.command(e)) if self.command else None, **args)
                     self.frame[i,j].grid(column=j, row=i, padx=self.padx, pady=self.pady, sticky="nsew")
                 
                 self.rowconfigure(i, weight=1)
                 self.columnconfigure(j, weight=1)
                 
     def manipulate_data(self, row, column):
@@ -193,22 +197,22 @@
                 row_data.append(self.data[i,j]["value"])
             self.values.append(row_data)
             
     def edit_row(self, row, **kwargs):
         """ edit all parameters of a single row """
         for i in range(self.columns):
             self.frame[row, i].configure(**kwargs)
-            self.data[row, i]["args"] = kwargs
+            self.data[row, i]["args"].update(kwargs)
         self.update_data()
         
     def edit_column(self, column, **kwargs):
         """ edit all parameters of a single column """
         for i in range(self.rows):
             self.frame[i, column].configure(**kwargs)
-            self.data[i, column]["args"] = kwargs
+            self.data[i, column]["args"].update(kwargs)
         self.update_data()
         
     def update_values(self, values, **kwargs):
         """ update all values at once """
         for i in self.frame.values():
             i.destroy()
         self.frame = {}
@@ -277,25 +281,25 @@
         """ insert value in a specific block [row, column] """
         if self.write:
             self.frame[row,column].delete(0, customtkinter.END)
             self.frame[row,column].insert(0, value)
             self.frame[row,column].configure(**kwargs)
         else:        
             self.frame[row,column].configure(text=value, **kwargs)
-        if kwargs: self.data[row,column]["args"] = kwargs
+        if kwargs: self.data[row,column]["args"].update(kwargs)
         self.update_data()
         
     def delete(self, row, column, **kwargs):
         """ delete a value from a specific block [row, column] """
         if self.write:
             self.frame[row,column].delete(0, customtkinter.END)
             self.frame[row,column].configure(**kwargs)
         else:     
             self.frame[row,column].configure(text="", **kwargs)
-        if kwargs: self.data[row,column]["args"] = kwargs
+        if kwargs: self.data[row,column]["args"].update(kwargs)
         self.update_data()
         
     def get(self, row=None, column=None):
         if row and column:
             return self.data[row,column]["values"]
         else:
             return self.values
```

### Comparing `CTkTable-0.5/CTkTable.egg-info/PKG-INFO` & `CTkTable-0.6/CTkTable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.5
+Version: 0.6
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkTable-0.5/LICENSE` & `CTkTable-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkTable-0.5/PKG-INFO` & `CTkTable-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.5
+Version: 0.6
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkTable-0.5/README.md` & `CTkTable-0.6/README.md`

 * *Files identical despite different names*

### Comparing `CTkTable-0.5/setup.cfg` & `CTkTable-0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 5461 626c 650d 0a76 6572   = CTkTable..ver
-00000020: 7369 6f6e 203d 2030 2e35 0d0a 6465 7363  sion = 0.5..desc
+00000020: 7369 6f6e 203d 2030 2e36 0d0a 6465 7363  sion = 0.6..desc
 00000030: 7269 7074 696f 6e20 3d20 4375 7374 6f6d  ription = Custom
 00000040: 746b 696e 7465 7220 5461 626c 6520 7769  tkinter Table wi
 00000050: 6467 6574 0d0a 6c6f 6e67 5f64 6573 6372  dget..long_descr
 00000060: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000070: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000080: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 00000090: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
```

### Comparing `CTkTable-0.5/setup.py` & `CTkTable-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkTable',
-    version = '0.5',
+    version = '0.6',
     description = "Customtkinter Table widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkTable",
```

