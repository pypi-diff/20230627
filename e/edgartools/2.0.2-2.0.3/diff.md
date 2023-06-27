# Comparing `tmp/edgartools-2.0.2.tar.gz` & `tmp/edgartools-2.0.3.tar.gz`

## Comparing `edgartools-2.0.2.tar` & `edgartools-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/__about__.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_codes.py
--rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_companies.py
--rw-r--r--   0        0        0    69101 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_filings.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_gaap.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_markdown.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_party.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_rich.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_xbrl.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_xml.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/core.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/effect.py
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/financials.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/form144.py
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/forms.py
--rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/fundreports.py
--rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/muniadvisors.py
--rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/offerings.py
--rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/ownership.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/search.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/shelfofferings.py
--rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/data/GAAP_Taxonomy_2022.csv
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 edgartools-2.0.2/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    25209 2020-02-02 00:00:00.000000 edgartools-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/__about__.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_codes.py
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_companies.py
+-rw-r--r--   0        0        0    70263 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_filings.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_gaap.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_markdown.py
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_party.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_rich.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_xbrl.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/_xml.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/core.py
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/effect.py
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/financials.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/form144.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/forms.py
+-rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/fundreports.py
+-rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/muniadvisors.py
+-rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/offerings.py
+-rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/ownership.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/search.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/shelfofferings.py
+-rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.3/edgar/data/GAAP_Taxonomy_2022.csv
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.3/LICENSE.txt
+-rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 edgartools-2.0.3/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    25209 2020-02-02 00:00:00.000000 edgartools-2.0.3/PKG-INFO
```

### Comparing `edgartools-2.0.2/edgar/__init__.py` & `edgartools-2.0.3/edgar/__init__.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_codes.py` & `edgartools-2.0.3/edgar/_codes.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_companies.py` & `edgartools-2.0.3/edgar/_companies.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_filings.py` & `edgartools-2.0.3/edgar/_filings.py`

 * *Files 2% similar despite different names*

```diff
@@ -940,15 +940,19 @@
             else:
                 if line.strip().startswith("<"):
                     # The line looks like this <KEY>VALUE
                     key, value = line.split('>')
                     # Strip the leading '<' from the key
                     data[key[1:]] = value
                 elif ':' in line:
-                    key, value = line.strip().split(':')
+                    parts = line.strip().split(':')
+                    if len(parts) == 2:
+                        key, value = line.strip().split(':')
+                    else:
+                        key, value = parts[0], ":".join(parts[1:])
                     value = value.strip()
                     if not current_header:
                         data[key] = value
                     elif not current_subheader:
                         continue
                     else:
                         if current_subheader == "FORMER COMPANY":
@@ -1535,14 +1539,28 @@
         return repr_rich(self.__rich__())
 
 
 # These are the columns on the table on the filing homepage
 filing_file_cols = ['Seq', 'Description', 'Document', 'Type', 'Size', 'Url']
 
 
+@dataclass(frozen=True)
+class ClassContractSeries:
+
+    cik: str
+
+@dataclass(frozen=True)
+class ClassContract:
+
+    cik: str
+    name: str
+    ticker: str
+    status:str
+
+
 class FilingHomepage:
     """
     A class that represents the homepage for the filing allowing us to get the documents and datafiles
     """
 
     def __init__(self,
                  files: pd.DataFrame,
@@ -1637,15 +1655,15 @@
     def from_html(cls,
                   homepage_html: str,
                   url: str,
                   filing: Filing):
         """Parse the HTML and create the Homepage from it"""
 
         # It is html so use "html.parser" (instead of "xml", or "lxml")
-        soup = BeautifulSoup(homepage_html, features="html.parser")
+        soup = BeautifulSoup(homepage_html, "html.parser")
 
         # Keep track of the tables as dataframes so we can append later
         dfs = []
 
         # The table containin the attachments
         tables = soup.find_all("table", class_="tableFile")
         for table in tables:
@@ -1668,24 +1686,38 @@
                            )
             dfs.append(table_as_df)
 
         # Now concat into a single dataframe
         files = pd.concat(dfs, ignore_index=True)
 
         # The table containing the contract series
-
+        # TODO: Implement Table Series
         """
         table_series = soup.find("table", class_="tableSeries")
-        TODO: Implement Table Series
+        
         if table_series:
-            for row in table_series.find_all("tr"):
+            rows = table_series.find_all("tr")
+            for row in rows:
                 cells = row.find_all("td")
-                print(cells)
-         """
-
+                if len(cells) > 0:
+                    # print the class of the first cell
+                    cell_class = cells[0].attrs.get("class")[0]
+                    class_series:Optional[ClassContractSeries] = None
+                    if cell_class == "seriesName":
+                        class_series = ClassContractSeries(cik=cells[0].text.replace("Series ", ""))
+                    
+                    print(cell_class, cells[0].text)
+                    
+                    if cell_class == 'seriesName':
+                        series_name = cells[0].text
+                        print(series_name)
+                    elif cell_class == 'classContract':
+                        class_contract = cells[0].text
+                        print(class_contract)
+        """
         return cls(files,
                    url=url,
                    filing=filing)
 
     def __str__(self):
         return f"Homepage for {self.description}"
```

### Comparing `edgartools-2.0.2/edgar/_gaap.py` & `edgartools-2.0.3/edgar/_gaap.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_markdown.py` & `edgartools-2.0.3/edgar/_markdown.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_party.py` & `edgartools-2.0.3/edgar/_party.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_rich.py` & `edgartools-2.0.3/edgar/_rich.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_xbrl.py` & `edgartools-2.0.3/edgar/_xbrl.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/_xml.py` & `edgartools-2.0.3/edgar/_xml.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/core.py` & `edgartools-2.0.3/edgar/core.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/effect.py` & `edgartools-2.0.3/edgar/effect.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/financials.py` & `edgartools-2.0.3/edgar/financials.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/form144.py` & `edgartools-2.0.3/edgar/form144.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/forms.py` & `edgartools-2.0.3/edgar/forms.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/fundreports.py` & `edgartools-2.0.3/edgar/fundreports.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/muniadvisors.py` & `edgartools-2.0.3/edgar/muniadvisors.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/offerings.py` & `edgartools-2.0.3/edgar/offerings.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/ownership.py` & `edgartools-2.0.3/edgar/ownership.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/search.py` & `edgartools-2.0.3/edgar/search.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/edgar/data/GAAP_Taxonomy_2022.csv` & `edgartools-2.0.3/edgar/data/GAAP_Taxonomy_2022.csv`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/LICENSE.txt` & `edgartools-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/README.md` & `edgartools-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/pyproject.toml` & `edgartools-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.2/PKG-INFO` & `edgartools-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgartools
-Version: 2.0.2
+Version: 2.0.3
 Summary: One of the nicest looking EDGAR libraries out there
 Project-URL: Documentation, https://dgunning.github.io/edgartools/
 Project-URL: Issues, https://github.com/dgunning/edgartools/issues
 Project-URL: Source, https://github.com/dgunning/edgartools
 Author-email: Dwight Gunning <dgunning@gmail.com>
 License-File: LICENSE.txt
 Keywords: company,edgar,filings,finance,financial,python,reports,sec
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edgartools Version: 2.0.2 Summary: One of the
+Metadata-Version: 2.1 Name: edgartools Version: 2.0.3 Summary: One of the
 nicest looking EDGAR libraries out there Project-URL: Documentation, https://
 dgunning.github.io/edgartools/ Project-URL: Issues, https://github.com/
 dgunning/edgartools/issues Project-URL: Source, https://github.com/dgunning/
 edgartools Author-email: Dwight Gunning
 gmail.com> License-File: LICENSE.txt Keywords:
 company,edgar,filings,finance,financial,python,reports,sec Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
```

