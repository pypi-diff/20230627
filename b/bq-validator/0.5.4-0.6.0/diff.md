# Comparing `tmp/bq-validator-0.5.4.tar.gz` & `tmp/bq_validator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bq-validator-0.5.4.tar", last modified: Tue May  9 09:13:04 2023, max compression
+gzip compressed data, was "bq_validator-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bq-validator-0.5.4.tar` & `bq_validator-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0      804 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      961 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      966 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0      967 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.gitignore
--rw-r--r--   0        0        0      150 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.pypirc
--rw-r--r--   0        0        0       32 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.style.yapf
--rw-r--r--   0        0        0    11357 2023-05-09 09:12:38.440499 bq-validator-0.5.4/LICENSE
--rw-r--r--   0        0        0      100 2023-05-09 09:12:38.440499 bq-validator-0.5.4/MANIFEST.in
--rw-r--r--   0        0        0      749 2023-05-09 09:12:38.440499 bq-validator-0.5.4/Makefile
--rw-r--r--   0        0        0     1788 2023-05-09 09:12:38.440499 bq-validator-0.5.4/README.md
--rw-r--r--   0        0        0      890 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/__init__.py
--rw-r--r--   0        0        0     4443 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/bigquery.py
--rw-r--r--   0        0        0     2876 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/cli.py
--rw-r--r--   0        0        0     1445 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/utils.py
--rwxr-xr-x   0        0        0     1121 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/clean.sh
--rwxr-xr-x   0        0        0     1013 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/format_python.sh
--rw-r--r--   0        0        0      970 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1366 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/setup.sh
--rw-r--r--   0        0        0      921 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/test_entry_point.sh
--rwxr-xr-x   0        0        0      958 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/test_python.sh
--rw-r--r--   0        0        0    14273 2023-05-09 09:12:38.440499 bq-validator-0.5.4/pylintrc
--rw-r--r--   0        0        0     1989 2023-05-09 09:12:38.440499 bq-validator-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      830 2023-05-09 09:12:38.440499 bq-validator-0.5.4/setup.py
--rw-r--r--   0        0        0      792 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0     1160 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/orders.sql
--rw-r--r--   0        0        0      218 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
--rw-r--r--   0        0        0      241 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
--rw-r--r--   0        0        0      330 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
--rw-r--r--   0        0        0      166 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
--rw-r--r--   0        0        0      166 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
--rw-r--r--   0        0        0     1442 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/test_utils.py
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 bq-validator-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-27 01:35:06.444168 bq_validator-0.6.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      981 2023-06-27 01:35:06.444168 bq_validator-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      986 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0      980 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.gitignore
+-rw-r--r--   0        0        0      648 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    13990 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pypirc
+-rw-r--r--   0        0        0       32 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-27 01:35:06.448168 bq_validator-0.6.0/LICENSE
+-rw-r--r--   0        0        0      100 2023-06-27 01:35:06.448168 bq_validator-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0      967 2023-06-27 01:35:06.448168 bq_validator-0.6.0/Makefile
+-rw-r--r--   0        0        0     1788 2023-06-27 01:35:06.448168 bq_validator-0.6.0/README.md
+-rw-r--r--   0        0        0      890 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/__init__.py
+-rw-r--r--   0        0        0     4456 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/bigquery.py
+-rw-r--r--   0        0        0     2891 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/cli.py
+-rw-r--r--   0        0        0     1444 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/utils.py
+-rwxr-xr-x   0        0        0     1121 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/clean.sh
+-rwxr-xr-x   0        0        0     1013 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/format_python.sh
+-rw-r--r--   0        0        0      970 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1394 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/publish.sh
+-rwxr-xr-x   0        0        0     1023 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/setup.sh
+-rw-r--r--   0        0        0      921 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/test_entry_point.sh
+-rwxr-xr-x   0        0        0      958 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/test_python.sh
+-rw-r--r--   0        0        0    14273 2023-06-27 01:35:06.448168 bq_validator-0.6.0/pylintrc
+-rw-r--r--   0        0        0     2002 2023-06-27 01:35:06.448168 bq_validator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-27 01:35:06.448168 bq_validator-0.6.0/setup.py
+-rw-r--r--   0        0        0      792 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1160 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql
+-rw-r--r--   0        0        0      218 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
+-rw-r--r--   0        0        0      241 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
+-rw-r--r--   0        0        0      330 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
+-rw-r--r--   0        0        0      167 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
+-rw-r--r--   0        0        0      167 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
+-rw-r--r--   0        0        0     1442 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 bq_validator-0.6.0/PKG-INFO
```

### Comparing `bq-validator-0.5.4/.github/CODEOWNERS` & `bq_validator-0.6.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/.github/workflows/publish.yml` & `bq_validator-0.6.0/.github/workflows/publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,20 @@
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
       - uses: actions/checkout@v3
       - name: Set up Python
+        id: python
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
       - name: Install Flit
-        if: steps.cache.outputs.cache-hit != 'true'
+        if: steps.python.outputs.cache-hit != 'true'
         run: bash dev/setup.sh
       - name: Publish
         env:
           # SEE https://packaging.python.org/en/latest/specifications/pypirc/?highlight=token#using-a-pypi-token
           FLIT_USERNAME: __token__
           FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
         run: bash dev/publish.sh "pypi"
```

### Comparing `bq-validator-0.5.4/.github/workflows/test-publish.yml` & `bq_validator-0.6.0/.github/workflows/test-publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
       - uses: actions/checkout@v3
       - name: Set up Python
+        id: python
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
       - name: Install Flit
-        if: steps.cache.outputs.cache-hit != 'true'
+        if: steps.python.outputs.cache-hit != 'true'
         run: bash dev/setup.sh
       - name: Test publish
         env:
           # SEE https://packaging.python.org/en/latest/specifications/pypirc/?highlight=token#using-a-pypi-token
           FLIT_USERNAME: __token__
           FLIT_PASSWORD: ${{ secrets.TESTPYPI_API_TOKEN }}
         run: bash dev/publish.sh "testpypi"
```

### Comparing `bq-validator-0.5.4/.github/workflows/test.yml` & `bq_validator-0.6.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,30 @@
       - main
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
       fail-fast: false
 
     defaults:
       run:
         shell: bash
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
+        id: python
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install Flit
-        if: steps.cache.outputs.cache-hit != 'true'
+        if: steps.python.outputs.cache-hit != 'true'
         run: bash dev/setup.sh
       - name: Lint
         if: ${{ matrix.python-version != '3.6' }}
         run: bash dev/lint_python.sh
       - name: Test
         run: bash dev/test_python.sh
       - name: Check the `bq-validator` command
```

### Comparing `bq-validator-0.5.4/.gitignore` & `bq_validator-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/LICENSE` & `bq_validator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/README.md` & `bq_validator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/bq_validator/__init__.py` & `bq_validator-0.6.0/bq_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
 The `bq-validator` command enables us to validate BigQuery queries.
 """
-__version__ = "0.5.4"
+__version__ = "0.6.0"
```

### Comparing `bq-validator-0.5.4/bq_validator/bigquery.py` & `bq_validator-0.6.0/bq_validator/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,8 +113,8 @@
     job_config.dry_run = True
     # Query dry run
     try:
         client.query(query=query, job_config=job_config)
         return True, None
     # pylint: disable=W0703
     except Exception as e:
-        return False, e
+        return False, str(e).strip()
```

### Comparing `bq-validator-0.5.4/bq_validator/cli.py` & `bq_validator-0.6.0/bq_validator/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import json
 import sys
 from typing import Optional
 
 import click
 import click_completion
 
 import bq_validator
 from bq_validator.bigquery import create_bigquery_client, validate_query
-from bq_validator.utils import read_file, get_sql_files
+from bq_validator.utils import get_sql_files, read_file
 
 # Initialize click-completion
 click_completion.init()
 
 
 @click.command()
 @click.argument('path', type=click.Path(exists=True))
@@ -41,17 +42,15 @@
               required=False,
               help="BigQuery client location")
 @click.option("--impersonate_service_account",
               type=str,
               required=False,
               help="Impersonate service account email")
 @click.version_option(version=bq_validator.__version__)
-def main(path: str,
-         quota_project: Optional[str],
-         client_project: Optional[str],
+def main(path: str, quota_project: Optional[str], client_project: Optional[str],
          client_location: Optional[str],
          impersonate_service_account: Optional[str]):
     """Validate BigQuery queries
 
     PATH is either of a SQL file path or a directory.
     When it is a directory, the command recursively validates all SQL files in the directory.
     """
@@ -64,13 +63,15 @@
     # Validate queries
     sql_files = get_sql_files(path=path)
     errors = {}
     for query_file in sql_files:
         query = read_file(path=query_file)
         is_valid, error_message = validate_query(client=client, query=query)
         if is_valid is False:
-            errors[query_file] = error_message
+            errors[query_file] = {
+                "query": query,
+                "error": error_message,
+            }
     # Show errors
     if len(errors) > 0:
-        for file, error_message in errors.items():
-            click.echo(f"{file}: {error_message}")
+        click.echo(json.dumps(errors, indent=2))
         sys.exit(1)
```

### Comparing `bq-validator-0.5.4/bq_validator/utils.py` & `bq_validator-0.6.0/bq_validator/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import os.path
 import glob
-
-from typing import List, Iterator, Union
+import os.path
+from typing import Iterator, List, Union
 
 
 def get_project_root():
     """Get the path to the project root"""
     return os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
```

### Comparing `bq-validator-0.5.4/dev/clean.sh` & `bq_validator-0.6.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/dev/format_python.sh` & `bq_validator-0.6.0/dev/format_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/dev/lint_python.sh` & `bq_validator-0.6.0/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/dev/publish.sh` & `bq_validator-0.6.0/dev/publish.sh`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 cd "$MODULE_DIR"
 
 # Arguments
 target=${1:?"target is not set"}
 
 # SEE https://flit.readthedocs.io/en/latest/reproducible.html
+# shellcheck disable=SC2034
 SOURCE_DATE_EPOCH=$(date +%s)
 
 if [[ "$target" == "pypi" ]] ; then
   flit publish --repository "${target}" --pypirc "${MODULE_DIR}/.pypirc" --setup-py
 elif [[ "$target" == "testpypi" ]] ; then
   flit publish --repository "${target}" --pypirc "${MODULE_DIR}/.pypirc" --setup-py
 else
```

### Comparing `bq-validator-0.5.4/dev/setup.sh` & `bq_validator-0.6.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/dev/test_entry_point.sh` & `bq_validator-0.6.0/dev/test_entry_point.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/dev/test_python.sh` & `bq_validator-0.6.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/pylintrc` & `bq_validator-0.6.0/pylintrc`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/pyproject.toml` & `bq_validator-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,36 +28,36 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest >=6.2.4,<7.0.0",
-    "pylint >=2.12.0",
-    "mypy ==0.910",
-    "flake8 >=3.8.3,<4.0.0",
-    "black ==21.9b0",
-    "isort >=5.0.6,<6.0.0",
-    "yapf >=0.29.0",
 ]
 dev = [
     "flit ==3.7.1",
     "build ==0.7.0",
     "yapf >=0.29.0",
     "pyyaml >=5.3",
     "pdoc3 >=0.9.2",
+    "isort >=5.0.6,<6.0.0",
+    "mypy ==0.910",
+    "black ==21.9b0",
+    "pylint >=2.12.0",
+    "flake8 >=3.8.3,<4.0.0",
+    "pre-commit >=3.0.0,<4.0.0",
 ]
 
 [project.scripts]
 bq-validator = 'bq_validator.cli:main'
 
 
 [tool.pytest.ini_options]
```

### Comparing `bq-validator-0.5.4/setup.py` & `bq_validator-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/tests/__init__.py` & `bq_validator-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/orders.sql` & `bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/tests/test_utils.py` & `bq_validator-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.4/PKG-INFO` & `bq_validator-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-validator
-Version: 0.5.4
+Version: 0.6.0
 Summary: The `bq-validator` command enables us to validate BigQuery queries.
 Author: yu-iskw
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -13,33 +13,33 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click >=8.0.0,<9.0.0
 Requires-Dist: click-completion >=0.5.2
 Requires-Dist: google-cloud-bigquery >=1.25.0,<4.0.0
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
+Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "dev"
+Requires-Dist: mypy ==0.910 ; extra == "dev"
+Requires-Dist: black ==21.9b0 ; extra == "dev"
+Requires-Dist: pylint >=2.12.0 ; extra == "dev"
+Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "dev"
+Requires-Dist: pre-commit >=3.0.0,<4.0.0 ; extra == "dev"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
-Requires-Dist: pylint >=2.12.0 ; extra == "test"
-Requires-Dist: mypy ==0.910 ; extra == "test"
-Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
-Requires-Dist: black ==21.9b0 ; extra == "test"
-Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
-Requires-Dist: yapf >=0.29.0 ; extra == "test"
 Provides-Extra: dev
 Provides-Extra: test
 
 [![Test python](https://github.com/yu-iskw/bq-validator/actions/workflows/test.yml/badge.svg)](https://github.com/yu-iskw/bq-validator/actions/workflows/test.yml)
 <a href="https://pypi.org/project/bq-validator" target="_blank">
     <img src="https://img.shields.io/pypi/v/bq-validator?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: bq-validator Version: 0.5.4 Summary: The `bq-
+Metadata-Version: 2.1 Name: bq-validator Version: 0.6.0 Summary: The `bq-
 validator` command enables us to validate BigQuery queries. Author: yu-iskw
 Requires-Python: >=3.6.1 Description-Content-Type: text/markdown Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
-click >=8.0.0,<9.0.0 Requires-Dist: click-completion >=0.5.2 Requires-Dist:
-google-cloud-bigquery >=1.25.0,<4.0.0 Requires-Dist: flit ==3.7.1 ; extra ==
-"dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist: yapf
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: click >=8.0.0,<9.0.0 Requires-Dist: click-completion >=0.5.2 Requires-
+Dist: google-cloud-bigquery >=1.25.0,<4.0.0 Requires-Dist: flit ==3.7.1 ; extra
+== "dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist: yapf
 >=0.29.0 ; extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev"
-Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pytest
->=6.2.4,<7.0.0 ; extra == "test" Requires-Dist: pylint >=2.12.0 ; extra ==
-"test" Requires-Dist: mypy ==0.910 ; extra == "test" Requires-Dist: flake8
->=3.8.3,<4.0.0 ; extra == "test" Requires-Dist: black ==21.9b0 ; extra ==
-"test" Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test" Requires-Dist:
-yapf >=0.29.0 ; extra == "test" Provides-Extra: dev Provides-Extra: test [!
+Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: isort
+>=5.0.6,<6.0.0 ; extra == "dev" Requires-Dist: mypy ==0.910 ; extra == "dev"
+Requires-Dist: black ==21.9b0 ; extra == "dev" Requires-Dist: pylint >=2.12.0 ;
+extra == "dev" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "dev" Requires-
+Dist: pre-commit >=3.0.0,<4.0.0 ; extra == "dev" Requires-Dist: pytest
+>=6.2.4,<7.0.0 ; extra == "test" Provides-Extra: dev Provides-Extra: test [!
 [Test python](https://github.com/yu-iskw/bq-validator/actions/workflows/
 test.yml/badge.svg)](https://github.com/yu-iskw/bq-validator/actions/workflows/
 test.yml) [Package_version] [Supported_Python_versions] # bq-validator This is
 a yet another python-based BigQuery query validator. The `bq query --dry_run`
 command enables us to validate queries. However, the `bq` command doesn't
 support service account impersonation, even though it supports workload
 identity federation credentials at Google Cloud SDK 390.0.0. The `bq-validator`
```

