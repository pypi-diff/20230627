# Comparing `tmp/dbl_discoverx-0.0.1.tar.gz` & `tmp/dbl_discoverx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbl_discoverx-0.0.1.tar", last modified: Tue Jun 20 14:47:53 2023, max compression
+gzip compressed data, was "dbl_discoverx-0.0.2.tar", last modified: Tue Jun 27 18:07:10 2023, max compression
```

## Comparing `dbl_discoverx-0.0.1.tar` & `dbl_discoverx-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:53.401645 dbl_discoverx-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-20 14:47:53.401645 dbl_discoverx-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:53.397645 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-20 14:47:53.000000 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 14:47:53.000000 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:47:53.000000 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 14:47:53.000000 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:47:53.000000 dbl_discoverx-0.0.1/dbl_discoverx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:53.401645 dbl_discoverx-0.0.1/discoverx/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:53.401645 dbl_discoverx-0.0.1/discoverx/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/dx.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/msql.py
--rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/discoverx/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:47:53.401645 dbl_discoverx-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-20 14:47:41.000000 dbl_discoverx-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.910896 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 18:07:10.000000 dbl_discoverx-0.0.2/dbl_discoverx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/discoverx/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/discoverx/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/dx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/msql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/discoverx/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:07:10.914896 dbl_discoverx-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-27 18:06:58.000000 dbl_discoverx-0.0.2/setup.py
```

### Comparing `dbl_discoverx-0.0.1/LICENSE` & `dbl_discoverx-0.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 DB license
 
-Copyright (2023) Databricks, Inc.
+Copyright (2022) Databricks, Inc.
 
 Definitions.
 
 Agreement: The agreement between Databricks, Inc., and you governing the use of the Databricks Services, which shall be, with respect to Databricks, the Databricks Terms of Service located at www.databricks.com/termsofservice, and with respect to Databricks Community Edition, the Community Edition Terms of Service located at www.databricks.com/ce-termsofuse, in each case unless you have entered into a separate written agreement with Databricks governing the use of the applicable Databricks Services.
 
 Software: The source code and object code to which this license applies.
 
@@ -18,8 +18,8 @@
 If the source code form includes a "NOTICE" text file as part of its distribution, then any derivative works that you distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the derivative works.
 You may add your own copyright statement to your modifications and may provide additional license terms and conditions for use, reproduction, or distribution of your modifications, or for any such derivative works as a whole, provided your use, reproduction, and distribution of the Software otherwise complies with the conditions stated in this License.
 
 Termination. This license terminates automatically upon your breach of these terms or upon the termination of your Agreement. Additionally, Databricks may terminate this license at any time on notice. Upon termination, you must permanently delete the Software and all copies thereof.
 
 DISCLAIMER; LIMITATION OF LIABILITY.
 
-THE SOFTWARE IS PROVIDED “AS-IS” AND WITH ALL FAULTS. DATABRICKS, ON BEHALF OF ITSELF AND ITS LICENSORS, SPECIFICALLY DISCLAIMS ALL WARRANTIES RELATING TO THE SOURCE CODE, EXPRESS AND IMPLIED, INCLUDING, WITHOUT LIMITATION, IMPLIED WARRANTIES, CONDITIONS AND OTHER TERMS OF MERCHANTABILITY, SATISFACTORY QUALITY OR FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT. DATABRICKS AND ITS LICENSORS TOTAL AGGREGATE LIABILITY RELATING TO OR ARISING OUT OF YOUR USE OF OR DATABRICKS’ PROVISIONING OF THE SOURCE CODE SHALL BE LIMITED TO ONE THOUSAND ($1,000) DOLLARS. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS-IS” AND WITH ALL FAULTS. DATABRICKS, ON BEHALF OF ITSELF AND ITS LICENSORS, SPECIFICALLY DISCLAIMS ALL WARRANTIES RELATING TO THE SOURCE CODE, EXPRESS AND IMPLIED, INCLUDING, WITHOUT LIMITATION, IMPLIED WARRANTIES, CONDITIONS AND OTHER TERMS OF MERCHANTABILITY, SATISFACTORY QUALITY OR FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT. DATABRICKS AND ITS LICENSORS TOTAL AGGREGATE LIABILITY RELATING TO OR ARISING OUT OF YOUR USE OF OR DATABRICKS’ PROVISIONING OF THE SOURCE CODE SHALL BE LIMITED TO ONE THOUSAND ($1,000) DOLLARS. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `dbl_discoverx-0.0.1/PKG-INFO` & `dbl_discoverx-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl_discoverx
-Version: 0.0.1
+Version: 0.0.2
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 %pip install dbl-discoverx
 ```
 
 Get started
 
 ```
 from discoverx import DX
-dx = DX()
+dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
 You can now scan the content of any set of tables for
 - IP addresses (v4 and v6)
 - Email addresses
@@ -49,40 +49,51 @@
 
 ```
 dx.display_rules()
 ```
 
 You can also provide your [custom matching rules](#custom-rules).
 
-The scan will automatically classify columns where the number of matching records exceeds a [classification threshold](#classification-threshold) (95% by default).
+The scan will automatically classify columns.
 
 
 ### Example
 
 Scan all (samples 10k rows from each table)
 
 ```
 dx.scan(from_tables="*.*.*")
 ```
 
 Check out the [scan parameters](#scan-parameters).
 
-The result is a dataset with a `frequency` column, which defines the fraction of matched records against the total records scanned for each rule.
+The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
+The full scan result can be displayed using
 
-## Publish the classificaiton
+```
+dx.scan_result
+```
+
+## Save & Load the Scan Results
 
-After a `scan` you can save the classificaiton results in a delta table (by default the table is `_discoverx.classification.classes`).
+After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
-dx.save()
+dx.save(full_table_name=<your-table-name>)
+```
+
+To load the saved results at a later time or in a different session use
+
+```
+dx.load(full_table_name=<your-table-name>)
 ```
 
 ## Cross-table queries
 
-After a `save` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
+After a `scan` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
 
 
 ### Search
 
 Search for a specific value across multiple tables.
 
 ```
@@ -93,44 +104,54 @@
 
 You can also specify the classes where the search should be performed explicitly:
 
 ```
 dx.search("example_email@databricks.com", from_tables="*.*.*", by_classes=["dx_email"])
 ```
 
+If you want to limit the search to columns with a specific classification score
+you need to provide it as parameter, i.e.
+
+```
+dx.search("example_email@databricks.com", from_tables="*.*.*", min_score=0.95)
+```
+
+The score refers to the frequency of matching rules during the scan for
+the respective column.
+
 ### Delete
 
 Delete 
 
 Preview delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False, min_score=0.95)
 ```
 
 Execute delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True, min_score=0.95)
 ```
 
-Note: You need to regularely [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
+Note: You need to regularly [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
 
 ### Select
 
 Select all columns classified with specified classes from multiple tables
 
 ```
-dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"])
+dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"], min_score=None)
 ```
 
 You can apply further transformations to build your summary tables. 
 Eg. Count the occurrence of each IP address per day across multiple tables and columns
 
 ```
 df = (dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_ip_v4"])
-    .groupby(["catalog", "schema", "table", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
+    .groupby(["table_catalog", "table_schema", "table_name", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
     .agg(func.count("classified_columns.dx_ip_v4.value").alias("count"))
 )
 ```
 
 
 ## Configuration
 
@@ -169,20 +190,12 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
-### Classification threshold
-
-You can customize the classification threshold with
-
-```
-dx = DX(classification_threshold=0.99)
-```
-
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.1/README.md` & `dbl_discoverx-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 %pip install dbl-discoverx
 ```
 
 Get started
 
 ```
 from discoverx import DX
-dx = DX()
+dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
 You can now scan the content of any set of tables for
 - IP addresses (v4 and v6)
 - Email addresses
@@ -34,40 +34,51 @@
 
 ```
 dx.display_rules()
 ```
 
 You can also provide your [custom matching rules](#custom-rules).
 
-The scan will automatically classify columns where the number of matching records exceeds a [classification threshold](#classification-threshold) (95% by default).
+The scan will automatically classify columns.
 
 
 ### Example
 
 Scan all (samples 10k rows from each table)
 
 ```
 dx.scan(from_tables="*.*.*")
 ```
 
 Check out the [scan parameters](#scan-parameters).
 
-The result is a dataset with a `frequency` column, which defines the fraction of matched records against the total records scanned for each rule.
+The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
+The full scan result can be displayed using
 
-## Publish the classificaiton
+```
+dx.scan_result
+```
+
+## Save & Load the Scan Results
 
-After a `scan` you can save the classificaiton results in a delta table (by default the table is `_discoverx.classification.classes`).
+After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
-dx.save()
+dx.save(full_table_name=<your-table-name>)
+```
+
+To load the saved results at a later time or in a different session use
+
+```
+dx.load(full_table_name=<your-table-name>)
 ```
 
 ## Cross-table queries
 
-After a `save` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
+After a `scan` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
 
 
 ### Search
 
 Search for a specific value across multiple tables.
 
 ```
@@ -78,44 +89,54 @@
 
 You can also specify the classes where the search should be performed explicitly:
 
 ```
 dx.search("example_email@databricks.com", from_tables="*.*.*", by_classes=["dx_email"])
 ```
 
+If you want to limit the search to columns with a specific classification score
+you need to provide it as parameter, i.e.
+
+```
+dx.search("example_email@databricks.com", from_tables="*.*.*", min_score=0.95)
+```
+
+The score refers to the frequency of matching rules during the scan for
+the respective column.
+
 ### Delete
 
 Delete 
 
 Preview delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False, min_score=0.95)
 ```
 
 Execute delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True, min_score=0.95)
 ```
 
-Note: You need to regularely [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
+Note: You need to regularly [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
 
 ### Select
 
 Select all columns classified with specified classes from multiple tables
 
 ```
-dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"])
+dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"], min_score=None)
 ```
 
 You can apply further transformations to build your summary tables. 
 Eg. Count the occurrence of each IP address per day across multiple tables and columns
 
 ```
 df = (dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_ip_v4"])
-    .groupby(["catalog", "schema", "table", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
+    .groupby(["table_catalog", "table_schema", "table_name", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
     .agg(func.count("classified_columns.dx_ip_v4.value").alias("count"))
 )
 ```
 
 
 ## Configuration
 
@@ -154,20 +175,12 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
-### Classification threshold
-
-You can customize the classification threshold with
-
-```
-dx = DX(classification_threshold=0.99)
-```
-
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.1/dbl_discoverx.egg-info/PKG-INFO` & `dbl_discoverx-0.0.2/dbl_discoverx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl-discoverx
-Version: 0.0.1
+Version: 0.0.2
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 %pip install dbl-discoverx
 ```
 
 Get started
 
 ```
 from discoverx import DX
-dx = DX()
+dx = DX(locale="US")
 ```
 
 ## Scan & classify
 
 You can now scan the content of any set of tables for
 - IP addresses (v4 and v6)
 - Email addresses
@@ -49,40 +49,51 @@
 
 ```
 dx.display_rules()
 ```
 
 You can also provide your [custom matching rules](#custom-rules).
 
-The scan will automatically classify columns where the number of matching records exceeds a [classification threshold](#classification-threshold) (95% by default).
+The scan will automatically classify columns.
 
 
 ### Example
 
 Scan all (samples 10k rows from each table)
 
 ```
 dx.scan(from_tables="*.*.*")
 ```
 
 Check out the [scan parameters](#scan-parameters).
 
-The result is a dataset with a `frequency` column, which defines the fraction of matched records against the total records scanned for each rule.
+The result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
+The full scan result can be displayed using
 
-## Publish the classificaiton
+```
+dx.scan_result
+```
+
+## Save & Load the Scan Results
 
-After a `scan` you can save the classificaiton results in a delta table (by default the table is `_discoverx.classification.classes`).
+After a `scan` you can save the scan results in a delta table of your choice.
 
 ```
-dx.save()
+dx.save(full_table_name=<your-table-name>)
+```
+
+To load the saved results at a later time or in a different session use
+
+```
+dx.load(full_table_name=<your-table-name>)
 ```
 
 ## Cross-table queries
 
-After a `save` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
+After a `scan` you can leverage the classified column classes to run cross-table `search`, `delete_by_class` and `select_by_classes` actions.
 
 
 ### Search
 
 Search for a specific value across multiple tables.
 
 ```
@@ -93,44 +104,54 @@
 
 You can also specify the classes where the search should be performed explicitly:
 
 ```
 dx.search("example_email@databricks.com", from_tables="*.*.*", by_classes=["dx_email"])
 ```
 
+If you want to limit the search to columns with a specific classification score
+you need to provide it as parameter, i.e.
+
+```
+dx.search("example_email@databricks.com", from_tables="*.*.*", min_score=0.95)
+```
+
+The score refers to the frequency of matching rules during the scan for
+the respective column.
+
 ### Delete
 
 Delete 
 
 Preview delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=False, min_score=0.95)
 ```
 
 Execute delete statements
 ```
-dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True)
+dx.delete_by_class(from_tables="*.*.*", by_class="dx_email", values=['example_email@databricks.com'], yes_i_am_sure=True, min_score=0.95)
 ```
 
-Note: You need to regularely [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
+Note: You need to regularly [vacuum](https://docs.delta.io/latest/delta-utility.html#remove-files-no-longer-referenced-by-a-delta-table) all your delta tables to remove all traces of your deleted rows. 
 
 ### Select
 
 Select all columns classified with specified classes from multiple tables
 
 ```
-dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"])
+dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_email"], min_score=None)
 ```
 
 You can apply further transformations to build your summary tables. 
 Eg. Count the occurrence of each IP address per day across multiple tables and columns
 
 ```
 df = (dx.select_by_classes(from_tables="*.*.*", by_classes=["dx_iso_date", "dx_ip_v4"])
-    .groupby(["catalog", "schema", "table", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
+    .groupby(["table_catalog", "table_schema", "table_name", "classified_columns.dx_iso_date.column", "classified_columns.dx_iso_date.value", "classified_columns.dx_ip_v4.column"])
     .agg(func.count("classified_columns.dx_ip_v4.value").alias("count"))
 )
 ```
 
 
 ## Configuration
 
@@ -169,20 +190,12 @@
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
 ```
 
-### Classification threshold
-
-You can customize the classification threshold with
-
-```
-dx = DX(classification_threshold=0.99)
-```
-
 ## Project Support
 Please note that all projects in the /databrickslabs github account are provided for your exploration only, and are not formally supported by Databricks with Service Level Agreements (SLAs).  They are provided AS-IS and we do not make any guarantees of any kind.  Please do not submit a support ticket relating to any issues arising from the use of these projects.
 
 Any issues discovered through the use of this project should be filed as GitHub Issues on the Repo.  They will be reviewed as time permits, but there are no formal SLAs for support.
```

### Comparing `dbl_discoverx-0.0.1/discoverx/common/helper.py` & `dbl_discoverx-0.0.2/discoverx/common/helper.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.1/discoverx/dx.py` & `dbl_discoverx-0.0.2/discoverx/dx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,107 @@
-from functools import wraps
+from delta.tables import DeltaTable
+import pandas as pd
 from pyspark.sql import SparkSession
 import pyspark.sql.functions as func
 from typing import List, Optional, Union
 from discoverx import logging
 from discoverx.msql import Msql
 from discoverx.rules import Rules, Rule
-from discoverx.scanner import Scanner
-from discoverx.classification import Classifier
+from discoverx.scanner import Scanner, ScanResult
 
 
 class DX:
     """DiscoverX scans and searches your lakehouse
 
     DiscoverX scans your data for patterns which have been pre-defined
     as rules. You can either use standard rules which come with
     DiscoverX or define and add custom rules.
     Attributes:
         custom_rules (List[Rule], Optional): Custom rules which will be
             used to detect columns with corresponding patterns in your
             data
-        classification_threshold (float, optional):
-            The threshold which will associate a column with a specific
-            rule and classify accordingly. The minimum and maximum
-            threshold values which can be specified are 0 and 1
-            respectively. The former corresponds to none of the records
-            for that column conforming to the given rule while the
-            latter means that all records conform.
         spark (SparkSession, optional): The SparkSession which will be
             used to scan your data. Defaults to None.
         locale (str, optional): The two-letter country code which will be
             used to determine the localized scanning rules.
             Defaults to None.
     """
 
+    COLUMNS_TABLE_NAME = "system.information_schema.columns"
+    MAX_WORKERS = 10
+
     def __init__(
         self,
         custom_rules: Optional[List[Rule]] = None,
-        classification_threshold: float = 0.95,
         spark: Optional[SparkSession] = None,
         locale: str = None,
-        classification_table_name: str = "_discoverx.classification.classes",
     ):
-
         if spark is None:
             spark = SparkSession.getActiveSession()
         self.spark = spark
         self.logger = logging.Logging()
 
         self.rules = Rules(custom_rules=custom_rules, locale=locale)
-
-        self.classification_threshold = self._validate_classification_threshold(classification_threshold)
-        self.classification_table_name = classification_table_name
-
-        self.uc_enabled = self.spark.conf.get("spark.databricks.unityCatalog.enabled", "false")
+        self.uc_enabled = self.spark.conf.get("spark.databricks.unityCatalog.enabled", "false") == "true"
 
         self.scanner: Optional[Scanner] = None
-        self.classifier: Optional[Classifier] = None
+        self._scan_result: Optional[ScanResult] = None
 
         self.intro()
 
+    def _can_read_columns_table(self) -> bool:
+        try:
+            self.spark.sql(f"SELECT * FROM {self.COLUMNS_TABLE_NAME} LIMIT 1")
+            return True
+        except Exception as e:
+            self.logger.error(f"Error while reading table {self.COLUMNS_TABLE_NAME}: {e}")
+            return False
+
     def intro(self):
         # TODO: Decide on how to do the introduction
         intro_text = """
         <h1>Hi there, I'm DiscoverX.</h1>
 
         <p>
           I'm here to help you discover data in your lakehouse.<br />
           You can scan your lakehouse by using
         </p>
-        <pre><code>dx.scan()</code></pre>
+        <pre><code>dx.scan(from_tables="*.*.*")</code></pre>
         <p>
           For more detailed instructions, check out the <a href="https://github.com/databrickslabs/discoverx">readme</a> or use
         </p>
         <pre><code>help(DX)</code></pre>
         """
 
         missing_uc_text = """
         <h1 style="color: red">Uch! DiscoverX needs Unity Catalog to be enabled</h1>
 
         <p>
           Please make sure you have Unity Catalog enabled, and that you are running a Cluster that supports Unity Catalog.
         </p>
         """
 
-        if self.uc_enabled == "true":
-            self.logger.friendlyHTML(intro_text)
-        else:
+        missing_access_to_columns_table_text = """
+        <h1 style="color: red">DiscoverX needs access to the system tables `system.information_schema.columns`</h1>
+        
+        <p>
+            Please make sure you have access to the system tables `system.information_schema.columns` and that you are running a Cluster that supports Unity Catalog.
+            To grant access to the system tables, execute the following commands:<br />
+            <code>GRANT USE CATALOG ON CATALOG system TO `account users`;</code><br /> 
+            <code>GRANT USE SCHEMA ON CATALOG system TO `account users`;</code><br />
+            <code>GRANT SELECT ON CATALOG system TO `account users`;</code>
+        </p>
+        """
+
+        if not self.uc_enabled:
             self.logger.friendlyHTML(missing_uc_text)
+        if not self._can_read_columns_table():
+            self.logger.friendlyHTML(missing_access_to_columns_table_text)
+        else:
+            self.logger.friendlyHTML(intro_text)
 
     def display_rules(self):
         """Displays the available rules in a friendly HTML format"""
         text = self.rules.get_rules_info()
         self.logger.friendlyHTML(text)
 
     def scan(
@@ -115,73 +126,82 @@
             self.rules,
             catalogs=catalogs,
             schemas=schemas,
             tables=tables,
             rule_filter=rules,
             sample_size=sample_size,
             what_if=what_if,
+            columns_table_name=self.COLUMNS_TABLE_NAME,
+            max_workers=self.MAX_WORKERS,
         )
 
-        self.scanner.scan()
-        self._classify(self.classification_threshold)
+        self._scan_result = self.scanner.scan()
+        self.logger.friendlyHTML(self.scanner.summary_html)
+
+    def _check_scan_result(self):
+        if self._scan_result is None:
+            raise Exception("You first need to scan your lakehouse using Scanner.scan()")
 
+    @property
     def scan_result(self):
         """Returns the scan results as a pandas DataFrame
 
         Raises:
             Exception: If the scan has not been run
         """
-        if self.scanner is None:
-            raise Exception("You first need to scan your lakehouse using Scanner.scan()")
-        if self.scanner.scan_result is None:
-            raise Exception("Your scan did not finish successfully. Please consider rerunning Scanner.scan()")
+        self._check_scan_result()
 
-        return self.scanner.scan_result.df
+        return self._scan_result.df
 
-    def _classify(self, classification_threshold: float):
-        """Classifies the columns in the lakehouse
+    def save(self, full_table_name: str):
+        """Saves the scan results to the lakehouse
 
         Args:
-            classification_threshold (float): The frequency threshold (0 to 1) above which a column will be classified
-
+            full_table_name (str): The full table name to be
+                used to save the scan results.
         Raises:
-            Exception: If the scan has not been run"""
-
-        if self.scanner is None:
-            raise Exception("You first need to scan your lakehouse using Scanner.scan()")
-        if self.scanner.scan_result is None:
-            raise Exception("Your scan did not finish successfully. Please consider rerunning Scanner.scan()")
-
-        self.classifier = Classifier(
-            classification_threshold,
-            self.scanner,
-            self.spark,
-            self.classification_table_name,
-        )
+            Exception: If the scan has not been run
 
-        self.logger.friendlyHTML(self.classifier.summary_html)
+        """
+        self._check_scan_result()
+        # save classes
+        self._scan_result.save(full_table_name)
 
-    def save(self):
-        """Publishes the classification results to the lakehouse
+    def load(self, full_table_name: str):
+        """Loads previously saved scan results from a table
 
+        Args:
+            full_table_name (str, optional): The full table name to be
+                used to load the scan results.
         Raises:
-            Exception: If the classification has not been run
-
+            Exception: If the table to be loaded does not exist
         """
+        self._scan_result = ScanResult(df=pd.DataFrame(), spark=self.spark)
+        self._scan_result.load(full_table_name)
 
-        # save classes
-        self.classifier.save()
-
-    def search(self, search_term: str, from_tables: str = "*.*.*", by_class: Optional[str] = None):
+    def search(
+        self,
+        search_term: str,
+        from_tables: str = "*.*.*",
+        by_class: Optional[str] = None,
+        min_score: Optional[float] = None,
+    ):
         """Searches your lakehouse for columns matching the given search term
 
         Args:
             search_term (str): The search term to be used to search for columns.
-            from_tables (str, optional): The tables to be searched in format "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
-            by_class (str, optional): The class to be used to search for columns. Defaults to None.
+            from_tables (str, optional): The tables to be searched in format
+                "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
+            by_class (str, optional): The class to be used to search for columns.
+                Defaults to None.
+            min_score (float, optional): Defines the classification score or frequency
+                threshold for columns to be considered during the scan. Defaults to None
+                which means that all columns where at least one record matched the
+                respective rule during the scan will be included. Has to be either None
+                or between 0 and 1.
 
         Raises:
             ValueError: If search_term is not provided
             ValueError: If the search_term type is not valid
             ValueError: If the by_class type is not valid
 
         Returns:
@@ -220,36 +240,49 @@
             raise ValueError(f"The provided by_class {by_class} must be of string type.")
 
         sql_filter = f"[{search_matching_rules[0]}] = '{search_term}'"
         select_statement = (
             "named_struct("
             + ", ".join(
                 [
-                    f"'{rule_name}', named_struct('column', '[{rule_name}]', 'value', [{rule_name}])"
+                    f"'{rule_name}', named_struct('column_name', '[{rule_name}]', 'value', [{rule_name}])"
                     for rule_name in search_matching_rules
                 ]
             )
             + ") AS search_result"
         )
 
         if search_term is None:
             where_statement = ""
         else:
             where_statement = f"WHERE {sql_filter}"
 
         return self._msql(
-            f"SELECT {select_statement}, to_json(struct(*)) AS row_content FROM {from_tables} {where_statement}"
+            f"SELECT {select_statement}, to_json(struct(*)) AS row_content FROM {from_tables} {where_statement}",
+            min_score=min_score,
         )
 
-    def select_by_classes(self, from_tables: str = "*.*.*", by_classes: Optional[Union[List[str], str]] = None):
+    def select_by_classes(
+        self,
+        from_tables: str = "*.*.*",
+        by_classes: Optional[Union[List[str], str]] = None,
+        min_score: Optional[float] = None,
+    ):
         """Selects all columns in the lakehouse from tables that match ALL the given classes
 
         Args:
-            from_tables (str, optional): The tables to be selected in format "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
-            by_classes (Union[List[str], str], optional): The classes to be used to search for columns. Defaults to None.
+            from_tables (str, optional): The tables to be selected in format
+                "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
+            by_classes (Union[List[str], str], optional): The classes to be used to
+                search for columns. Defaults to None.
+            min_score (float, optional): Defines the classification score or frequency
+                threshold for columns to be considered during the scan. Defaults to None
+                which means that all columns where at least one record matched the
+                respective rule during the scan will be included. Has to be either None
+                or between 0 and 1.
 
         Raises:
             ValueError: If the by_classes type is not valid
 
         Returns:
             DataFrame: A dataframe containing the UNION ALL results of the select"""
 
@@ -265,37 +298,49 @@
                 f" either a str or List[str]."
             )
 
         from_statement = (
             "named_struct("
             + ", ".join(
                 [
-                    f"'{class_name}', named_struct('column', '[{class_name}]', 'value', [{class_name}])"
+                    f"'{class_name}', named_struct('column_name', '[{class_name}]', 'value', [{class_name}])"
                     for class_name in by_classes
                 ]
             )
             + ") AS classified_columns"
         )
 
-        return self._msql(f"SELECT {from_statement}, to_json(struct(*)) AS row_content FROM {from_tables}")
+        return self._msql(
+            f"SELECT {from_statement}, to_json(struct(*)) AS row_content FROM {from_tables}", min_score=min_score
+        )
 
     def delete_by_class(
         self,
         from_tables="*.*.*",
         by_class: str = None,
         values: Optional[Union[List[str], str]] = None,
         yes_i_am_sure: bool = False,
+        min_score: Optional[float] = None,
     ):
         """Deletes all rows in the lakehouse that match any of the provided values in a column classified with the given class
 
         Args:
-            from_tables (str, optional): The tables to delete from in format "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
-            by_class (str, optional): The class to be used to search for columns. Defaults to None.
-            values (Union[List[str], str], optional): The values to be deleted. Defaults to None.
-            yes_i_am_sure (bool, optional): Whether you are sure that you want to delete the data. If False prints the SQL statements instead of executing them. Defaults to False.
+            from_tables (str, optional): The tables to delete from in format
+                "catalog.schema.table", use "*" as a wildcard. Defaults to "*.*.*".
+            by_class (str, optional): The class to be used to search for columns.
+                Defaults to None.
+            values (Union[List[str], str], optional): The values to be deleted.
+                Defaults to None.
+            yes_i_am_sure (bool, optional): Whether you are sure that you want to delete
+                the data. If False prints the SQL statements instead of executing them. Defaults to False.
+            min_score (float, optional): Defines the classification score or frequency
+                threshold for columns to be considered during the scan. Defaults to None
+                which means that all columns where at least one record matched the
+                respective rule during the scan will be included. Has to be either None
+                or between 0 and 1.
 
         Raises:
             ValueError: If the from_tables is not valid
             ValueError: If the by_class is not valid
             ValueError: If the values is not valid
         """
 
@@ -321,60 +366,37 @@
             self.logger.friendly(
                 f"Please confirm that you want to delete the following values from the table {from_tables} using the class {by_class}: {values}"
             )
             self.logger.friendly(
                 f"If you are sure, please run the same command again but set the parameter yes_i_am_sure to True."
             )
 
-        return self._msql(
-            f"DELETE FROM {from_tables} WHERE [{by_class}] IN ({value_string})", what_if=(not yes_i_am_sure)
+        delete_result = self._msql(
+            f"DELETE FROM {from_tables} WHERE [{by_class}] IN ({value_string})",
+            what_if=(not yes_i_am_sure),
+            min_score=min_score,
         )
 
-    def _msql(self, msql: str, what_if: bool = False):
+        if delete_result is not None:
+            delete_result = delete_result.toPandas()
+            self.logger.friendlyHTML(f"<p>The affcted tables are</p>{delete_result.to_html()}")
 
+    def _msql(self, msql: str, what_if: bool = False, min_score: Optional[float] = None):
         self.logger.debug(f"Executing sql template: {msql}")
 
         msql_builder = Msql(msql)
 
         # check if classification is available
         # Check for more specific exception
-        try:
-            classification_result_pdf = (
-                self.spark.sql(f"SELECT * FROM {self.classification_table_name}")
-                .filter(func.col("current") == True)
-                .select(
-                    func.col("table_catalog").alias("catalog"),
-                    func.col("table_schema").alias("schema"),
-                    func.col("table_name").alias("table"),
-                    func.col("column_name").alias("column"),
-                    "class_name",
-                )
-                .toPandas()
-            )
-        except Exception:
-            raise Exception("Classification is not available")
-
+        classification_result_pdf = self._scan_result.get_classes(min_score)
         sql_rows = msql_builder.build(classification_result_pdf)
 
         if what_if:
             self.logger.friendly(f"SQL that would be executed:")
 
             for sql_row in sql_rows:
                 self.logger.friendly(sql_row.sql)
 
             return None
         else:
             self.logger.debug(f"Executing SQL:\n{sql_rows}")
             return msql_builder.execute_sql_rows(sql_rows, self.spark)
-
-    def _validate_classification_threshold(self, threshold) -> float:
-        """Validate that threshold is in interval [0,1]
-        Args:
-            threshold (float): The threshold value to be validated
-        Returns:
-            float: The validated threshold value
-        """
-        if (threshold < 0) or (threshold > 1):
-            error_msg = f"classification_threshold has to be in interval [0,1]. Given value is {threshold}"
-            self.logger.error(error_msg)
-            raise ValueError(error_msg)
-        return threshold
```

### Comparing `dbl_discoverx-0.0.1/discoverx/logging.py` & `dbl_discoverx-0.0.2/discoverx/logging.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.1/discoverx/msql.py` & `dbl_discoverx-0.0.2/discoverx/msql.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,28 +69,27 @@
             for classified_col in classified_cols:
                 temp_sql = temp_sql.replace(f"[{classified_col.class_name}]", classified_col.name)
             sql_statements.append(SQLRow(table_info.catalog, table_info.schema, table_info.table, temp_sql))
 
         return sql_statements
 
     def build(self, classified_result_pdf) -> list[SQLRow]:
-
         """Builds the M-SQL expression into a SQL expression"""
 
         classified_cols = classified_result_pdf.copy()
         classified_cols = classified_cols[classified_cols["class_name"].isin(self.classes)]
         classified_cols = (
-            classified_cols.groupby(["catalog", "schema", "table", "column"])
+            classified_cols.groupby(["table_catalog", "table_schema", "table_name", "column_name"])
             .aggregate(lambda x: list(x))[["class_name"]]
             .reset_index()
         )
 
-        classified_cols["col_classes"] = classified_cols[["column", "class_name"]].apply(tuple, axis=1)
+        classified_cols["col_classes"] = classified_cols[["column_name", "class_name"]].apply(tuple, axis=1)
         df = (
-            classified_cols.groupby(["catalog", "schema", "table"])
+            classified_cols.groupby(["table_catalog", "table_schema", "table_name"])
             .aggregate(lambda x: list(x))[["col_classes"]]
             .reset_index()
         )
 
         # Filter tables by matching filter
         filtered_tables = [
             TableInfo(
@@ -111,20 +110,25 @@
         return sqls
 
     def execute_sql_row(self, sql_row: SQLRow, spark: SparkSession) -> DataFrame:
         """Executes the SQL statement"""
         try:
             result = (
                 spark.sql(sql_row.sql)
-                .withColumn("catalog", lit(sql_row.catalog))
-                .withColumn("schema", lit(sql_row.schema))
-                .withColumn("table", lit(sql_row.table))
+                .withColumn("table_catalog", lit(sql_row.catalog))
+                .withColumn("table_schema", lit(sql_row.schema))
+                .withColumn("table_name", lit(sql_row.table))
             )
             if self.command == "DELETE":
                 result = result.withColumn("sql", lit(sql_row.sql))
+
+            table_info_cols = ["table_catalog", "table_schema", "table_name"]
+            select_cols = table_info_cols + [col for col in result.columns if col not in table_info_cols]
+            result = result.select(*select_cols)
+
         except Exception as e:
             self.logger.info(f"Unable to execute SQL for {sql_row.catalog}.{sql_row.schema}.{sql_row.table}: {e}")
             result = None
 
         return result
 
     def execute_sql_rows(self, sqls: list[SQLRow], spark: SparkSession):
@@ -160,15 +164,15 @@
     def validate_from_components(from_tables: str):
         """Extracts the catalog, schema and table name from the from_table string"""
         matches = re.findall(Msql.from_components_expr, from_tables)
         if len(matches) == 1 and len(matches[0]) == 4:
             return (matches[0][1], matches[0][2], matches[0][3])
         else:
             raise ValueError(
-                f"Invalid from_tables statement '{from_tables}'. Should be a string in format 'catalog.schema.table'. You can use '*' as wildcard."
+                f"Invalid from_tables statement '{from_tables}'. Should be a string in format 'table_catalog.table_schema.table_name'. You can use '*' as wildcard."
             )
 
     def _extract_command(self):
         """Extracts the command from the M-SQL expression"""
         commands = re.findall(self.command_expr, self.msql)
         if len(commands) != 1:
             raise ValueError(
```

### Comparing `dbl_discoverx-0.0.1/discoverx/rules.py` & `dbl_discoverx-0.0.2/discoverx/rules.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.1/pyproject.toml` & `dbl_discoverx-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.1/setup.py` & `dbl_discoverx-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 TEST_REQUIREMENTS = [
     # development & testing tools
     "pytest",
     "pylint",
     "black",
     "coverage[toml]",
     "pytest-cov",
-    "dbx>=0.7,<0.8",
+    "dbx>=0.7,<0.9",
 ]
 
 setup(
     name="dbl_discoverx",
     packages=find_packages(exclude=["tests", "tests.*"]),
     setup_requires=["setuptools", "wheel"],
     install_requires=PACKAGE_REQUIREMENTS,
```

