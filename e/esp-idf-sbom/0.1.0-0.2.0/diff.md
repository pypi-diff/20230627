# Comparing `tmp/esp-idf-sbom-0.1.0.tar.gz` & `tmp/esp-idf-sbom-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-8lkel82v/esp-idf-sbom-0.1.0.tar", last modified: Mon Jun 12 14:24:59 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-jka_u2tl/esp-idf-sbom-0.2.0.tar", last modified: Tue Jun 27 12:01:07 2023, max compression
```

## Comparing `esp-idf-sbom-0.1.0.tar` & `esp-idf-sbom-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp-idf-sbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp-idf-sbom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/nvd.py
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9797 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/sbom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp-idf-sbom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp-idf-sbom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/nvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39587 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10078 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/sbom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/setup.py
```

### Comparing `esp-idf-sbom-0.1.0/LICENSE` & `esp-idf-sbom-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.1.0/PKG-INFO` & `esp-idf-sbom-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-sbom
-Version: 0.1.0
+Version: 0.2.0
 Summary: SPDX SBOM generator for ESP-IDF projects
 Home-page: https://github.com/espressif/esp-idf-sbom
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,spdx,sbom
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-sbom-0.1.0/README.md` & `esp-idf-sbom-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/git.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,16 @@
         return ''
 
     cfg = get_config(utils.pjoin(git_dir, 'config'))
     branch = get_branch(git_dir)
     remote = cfg.get(f'branch.{branch}.remote', 'origin')
     url = cfg.get(f'remote.{remote}.url', '')
 
-    if not url or url.startswith('/') or url.startswith('file:///'):
-        # ignore local repository url
+    if not utils.is_remote_url(url):
+        # ignore local repository url and URLs not using git, http or https scheme
         return ''
 
     return url
 
 
 def get_remote_location(path: str) -> str:
     """Return remote <URL>@<HEAD sha>#<relative path> for path."""
```

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/log.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/log.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/nvd.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/nvd.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/spdx.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/spdx.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 import re
 import sys
 import uuid
 from argparse import Namespace
 from typing import Any, Dict, List, Optional
 
+import schema
 import yaml
 
 from esp_idf_sbom import __version__
 from esp_idf_sbom.libsbom import git, log, utils
 
 
 class SPDXObject(object):
@@ -31,15 +32,15 @@
     """
     # SPDXID tag value has an requirement that it should contain
     # only letters, numbers, ., and/or -. Used in sanitize_spdxid()
     # to create valid SPDXID value.
     SPDXID_RE = re.compile(r'[^0-9a-zA-Z\.\-\+]')
     SPDX_TAGS = ['SPDXVersion', 'DataLicense', 'SPDXID', 'DocumentName', 'DocumentNamespace',
                  'Creator', 'Created', 'CreatorComment', 'Relationship', 'PackageName', 'PackageSummary',
-                 'PackageVersion', 'PackageSupplier', 'PackageDownloadLocation', 'FilesAnalyzed',
+                 'PackageVersion', 'PackageSupplier', 'PackageOriginator', 'PackageDownloadLocation', 'FilesAnalyzed',
                  'PackageVerificationCode', 'PackageLicenseInfoFromFiles', 'PackageLicenseConcluded',
                  'PackageLicenseDeclared', 'PackageCopyrightText', 'PackageComment', 'FileName',
                  'LicenseInfoInFile', 'FileCopyrightText', 'FileChecksum', 'ExternalRef', 'LicenseConcluded']
     # Used to automatically identify Espressif as supplier if package URL or
     # git repository matches.
     ESPRESSIF_RE = re.compile(r'^(\w+://)?(\w+@)?(gitlab\.espressif\.|github.com[:/]espressif/).*')
     # Supplier tag value for Espressif.
@@ -177,14 +178,47 @@
                 self.is_espressif_path(path)):
             return self.ESPRESSIF_SUPPLIER
         else:
             return ''
 
     def get_manifest(self, directory: str) -> Dict[str,str]:
         """Return manifest information found in given directory."""
+        def validate_sbom_manifest(manifest: Dict[str,str]) -> None:
+            def check_person_organization(s: str) -> bool:
+                if s.startswith('Person: ') or s.startswith('Organization: '):
+                    return True
+                raise schema.SchemaError((f'Value "{s}" must have "Person: " or "Organization: " prefix.'))
+
+            def check_url(url: str) -> bool:
+                if utils.is_remote_url(url):
+                    return True
+                raise schema.SchemaError((f'Value {url} must have "git", "http" or "https" scheme and domain.'))
+
+            def check_cpe(cpe: str):
+                # Note: WFN, well-formed CPE name, attributes rules are stricter
+                if re.match(r'^cpe:2\.3:[aho](?::\S+){10}', cpe):
+                    return True
+                raise schema.SchemaError((f'Value "{cpe}" does not seem to be well-formed CPE name (WFN)'))
+
+            try:
+                sbom_schema = schema.Schema(
+                    {
+                        schema.Optional('version'): str,
+                        schema.Optional('repository'): schema.And(str, check_url),
+                        schema.Optional('url'): schema.And(str, check_url),
+                        schema.Optional('cpe'): schema.And(str, check_cpe),
+                        schema.Optional('supplier'): schema.And(str, check_person_organization),
+                        schema.Optional('originator'): schema.And(str, check_person_organization),
+                        schema.Optional('description'): str,
+                    })
+
+                sbom_schema.validate(manifest)
+            except schema.SchemaError as e:
+                log.err.die(f'The sbom.yml manifest file in "{directory}" is not valid: {e}')
+
         def load(fn: str) -> Dict[str,str]:
             # Helper to load yml files.
             path = utils.pjoin(directory, fn)
             if not os.path.isfile(path):
                 return {}
 
             with open(path, 'r') as f:
@@ -208,14 +242,15 @@
             'cpe': '',
             'supplier': '',
             'originator': '',
             'description': '',
         }
 
         sbom_yml = load('sbom.yml')
+        validate_sbom_manifest(sbom_yml)
         update(manifest, sbom_yml)
         idf_component_yml = load('idf_component.yml')
         update(manifest, idf_component_yml)
 
         if not manifest['supplier']:
             # Supplier not explicitly provided, use maintainers if present.
             if 'maintainers' in idf_component_yml and idf_component_yml['maintainers']:
```

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/utils.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Miscellaneous helpers
 """
 
 import os
 import subprocess
 from pathlib import Path
 from typing import AnyStr, Dict, List, Optional, Tuple
+from urllib.parse import urlparse
 
 
 def pjoin(*paths: str) -> str:
     """Join input paths and return resulting path with forward slashes."""
     return Path().joinpath(*paths).as_posix()
 
 
@@ -22,14 +23,21 @@
 
 
 def psplit(path: str) -> Tuple[str,...]:
     """Split path into tuple of components."""
     return Path(path).parts
 
 
+def is_remote_url(url: str='') -> bool:
+    """Check if url has git, http or https scheme and domain.
+    This is just a very basic test."""
+    res = urlparse(url)
+    return bool(res.scheme in ['git', 'http', 'https'] and res.netloc)
+
+
 def run(cmd:    List[str],
         stdin:  Optional[AnyStr]=None,
         stdout: bool=True,
         stderr: bool=True,
         text:   bool=True,
         env:    Optional[Dict[str,str]] = None,
         strip:  bool=True,
```

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom/sbom.py` & `esp-idf-sbom-0.2.0/esp_idf_sbom/sbom.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             with open(args.input_file, 'r') as f:
                 buf = f.read()
         except OSError as e:
             sys.exit(f'cannot read SBOM file: {e}')
 
     table = []
     packages = spdx.parse_packages(buf)
-    if not args.all:
+    if not args.check_all_packages:
         packages = spdx.filter_packages(packages)
     for pkg in packages.values():
         if 'ExternalRef' not in pkg:
             continue
 
         cpe_refs = [ref for ref in pkg['ExternalRef'] if ref.startswith('SECURITY cpe23Type')]
         if not cpe_refs:
@@ -167,20 +167,23 @@
     check_parser.set_defaults(func=cmd_check)
     check_parser.add_argument('input_file',
                               metavar='SBOM_FILE',
                               default='-',
                               nargs='?',
                               help=('Path to the SBOM file generated by the ESP-IDF sbom tool. '
                                     'If not provided or "-", read from stdin.'))
-    check_parser.add_argument('-a', '--all',
+
+    check_parser.add_argument('--check-all-packages',
                               action='store_true',
                               default=bool(os.environ.get('SBOM_CHECK_ALL')),
                               help=('Check all packages in the SBOM file. By default only packages, '
                                     'linked via the SPDX relationship to the main project package, '
-                                    'are checked.'))
+                                    'are checked. This may report vulnerabilities, which do not '
+                                    'affect the resulting binary! For example components with libraries, '
+                                    'which are not linked into the final binary will be checked too.'))
 
     args = parser.parse_args()
     if args.quiet:
         log_level = log.NEVER
     if args.debug:
         log_level = log.DEBUG
     elif args.verbose:
```

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/PKG-INFO` & `esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-sbom
-Version: 0.1.0
+Version: 0.2.0
 Summary: SPDX SBOM generator for ESP-IDF projects
 Home-page: https://github.com/espressif/esp-idf-sbom
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,spdx,sbom
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/SOURCES.txt` & `esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.1.0/setup.py` & `esp-idf-sbom-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     long_description=get_long_description(),
     url='https://github.com/espressif/esp-idf-sbom',
     packages=find_packages(),
     python_requires='>=3.7',
     keywords=['espressif', 'embedded', 'spdx', 'sbom'],
     install_requires=[
         'PyYAML',
+        'schema',
     ],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Environment :: Console',
         'Topic :: Software Development :: Embedded Systems',
```

