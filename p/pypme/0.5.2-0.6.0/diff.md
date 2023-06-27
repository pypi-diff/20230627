# Comparing `tmp/pypme-0.5.2.tar.gz` & `tmp/pypme-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypme-0.5.2.tar", max compression
+gzip compressed data, was "pypme-0.6.0.tar", max compression
```

## Comparing `pypme-0.5.2.tar` & `pypme-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1083 2022-03-11 09:25:24.883286 pypme-0.5.2/LICENSE
--rw-r--r--   0        0        0      186 2023-04-03 08:53:31.720258 pypme-0.5.2/pypme/__init__.py
--rw-r--r--   0        0        0     1827 2022-09-27 14:36:01.924103 pypme-0.5.2/pypme/mod_tessa_pme.py
--rw-r--r--   0        0        0     5054 2022-04-01 09:08:50.260587 pypme-0.5.2/pypme/pme.py
--rw-r--r--   0        0        0      752 2023-04-03 08:53:12.476415 pypme-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3518 2022-10-02 07:57:05.251398 pypme-0.5.2/README.md
--rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 pypme-0.5.2/setup.py
--rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 pypme-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-03-11 09:25:24.883286 pypme-0.6.0/LICENSE
+-rw-r--r--   0        0        0      163 2023-06-27 12:42:57.792391 pypme-0.6.0/pypme/__init__.py
+-rw-r--r--   0        0        0     1827 2022-09-27 14:36:01.924103 pypme-0.6.0/pypme/mod_tessa_pme.py
+-rw-r--r--   0        0        0     5054 2022-04-01 09:08:50.260587 pypme-0.6.0/pypme/pme.py
+-rw-r--r--   0        0        0      706 2023-06-27 12:52:35.332203 pypme-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3518 2022-10-02 07:57:05.251398 pypme-0.6.0/README.md
+-rw-r--r--   0        0        0     4216 1970-01-01 00:00:00.000000 pypme-0.6.0/setup.py
+-rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 pypme-0.6.0/PKG-INFO
```

### Comparing `pypme-0.5.2/LICENSE` & `pypme-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypme-0.5.2/pypme/mod_tessa_pme.py` & `pypme-0.6.0/pypme/mod_tessa_pme.py`

 * *Files identical despite different names*

### Comparing `pypme-0.5.2/pypme/pme.py` & `pypme-0.6.0/pypme/pme.py`

 * *Files identical despite different names*

### Comparing `pypme-0.5.2/README.md` & `pypme-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pypme-0.5.2/setup.py` & `pypme-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 packages = \
 ['pypme']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy-financial>=1.0.0,<2.0.0',
- 'pandas>=1.4.1,<2.0.0',
- 'tessa>=0.5',
- 'xirr>=0.1.8,<0.2.0']
+['numpy-financial>=1,<2', 'pandas>=1.4,<2.0', 'tessa>=0.8,<0.9', 'xirr>=0,<1']
 
 setup_kwargs = {
     'name': 'pypme',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': 'Python package for PME (Public Market Equivalent) calculation',
     'long_description': '# pypme – Python package for PME (Public Market Equivalent) calculation\n\nBased on the [Modified PME\nmethod](https://en.wikipedia.org/wiki/Public_Market_Equivalent#Modified_PME).\n\n## Example\n\n```python\nfrom pypme import verbose_xpme\nfrom datetime import date\n\npmeirr, assetirr, df = verbose_xpme(\n    dates=[date(2015, 1, 1), date(2015, 6, 12), date(2016, 2, 15)],\n    cashflows=[-10000, 7500],\n    prices=[100, 120, 100],\n    pme_prices=[100, 150, 100],\n)\n```\n\nWill return `0.5525698793027238` and  `0.19495150355969598` for the IRRs and produce this\ndataframe:\n\n![Example dataframe](https://raw.githubusercontent.com/ymyke/pypme/main/images/example_df.png)\n\nNotes:\n- The `cashflows` are interpreted from a transaction account that is used to buy from an\n  asset at price `prices`.\n- The corresponding prices for the PME are `pme_prices`.\n- The `cashflows` is extended with one element representing the remaining value, that\'s\n  why all the other lists (`dates`, `prices`, `pme_prices`) need to be exactly 1 element\n  longer than `cashflows`.\n\n## Variants\n\n- `xpme`: Calculate PME for unevenly spaced / scheduled cashflows and return the PME IRR\n  only. In this case, the IRR is always annual.\n- `verbose_xpme`: Calculate PME for unevenly spaced / scheduled cashflows and return\n  vebose information.\n- `pme`: Calculate PME for evenly spaced cashflows and return the PME IRR only. In this\n  case, the IRR is for the underlying period.\n- `verbose_pme`: Calculate PME for evenly spaced cashflows and return vebose\n  information.\n- `tessa_xpme` and `tessa_verbose_xpme`: Use live price information via the tessa\n  library. See below.\n\n## tessa examples – using tessa to retrieve PME prices online\n\nUse `tessa_xpme` and `tessa_verbose_xpme` to get live prices via the [tessa\nlibrary](https://github.com/ymyke/tessa) and use those prices as the PME. Like so:\n\n```python\nfrom datetime import datetime, timezone\nfrom pypme import tessa_xpme\n\ncommon_args = {\n    "dates": [\n        datetime(2012, 1, 1, tzinfo=timezone.utc), \n        datetime(2013, 1, 1, tzinfo=timezone.utc)\n    ],\n    "cashflows": [-100],\n    "prices": [1, 1],\n}\nprint(tessa_xpme(pme_ticker="LIT", **common_args))  # source will default to "yahoo"\nprint(tessa_xpme(pme_ticker="bitcoin", pme_source="coingecko", **common_args))\nprint(tessa_xpme(pme_ticker="SREN.SW", pme_source="yahoo", **common_args))\n```\n\nNote that the dates need to be timezone-aware for these functions.\n\n\n## Garbage in, garbage out\n\nNote that the package will only perform essential sanity checks and otherwise just works\nwith what it gets, also with nonsensical data. E.g.:\n\n```python\nfrom pypme import verbose_pme\n\npmeirr, assetirr, df = verbose_pme(\n    cashflows=[-10, 500], prices=[1, 1, 1], pme_prices=[1, 1, 1]\n)\n```\n\nResults in this df and IRRs of 0:\n\n![Garbage example df](https://raw.githubusercontent.com/ymyke/pypme/main/images/garbage_example_df.png)\n\n\n## Other noteworthy libraries\n\n- [tessa](https://github.com/ymyke/tessa): Find financial assets and get their price history without worrying about different APIs or rate limiting.\n- [strela](https://github.com/ymyke/strela): A python package for financial alerts.\n\n\n## References\n\n- [Google Sheet w/ reference calculation](https://docs.google.com/spreadsheets/d/1LMSBU19oWx8jw1nGoChfimY5asUA4q6Vzh7jRZ_7_HE/edit#gid=0)\n- [Modified PME on Wikipedia](https://en.wikipedia.org/wiki/Public_Market_Equivalent#Modified_PME)\n',
     'author': 'ymyke',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ymyke/pypme',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pypme-0.5.2/PKG-INFO` & `pypme-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pypme
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python package for PME (Public Market Equivalent) calculation
 Home-page: https://github.com/ymyke/pypme
 License: MIT
 Keywords: python,finance,investing,financial-analysis,pme,investment-analysis
 Author: ymyke
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy-financial (>=1.0.0,<2.0.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0)
-Requires-Dist: tessa (>=0.5)
-Requires-Dist: xirr (>=0.1.8,<0.2.0)
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: numpy-financial (>=1,<2)
+Requires-Dist: pandas (>=1.4,<2.0)
+Requires-Dist: tessa (>=0.8,<0.9)
+Requires-Dist: xirr (>=0,<1)
 Project-URL: Repository, https://github.com/ymyke/pypme
 Description-Content-Type: text/markdown
 
 # pypme – Python package for PME (Public Market Equivalent) calculation
 
 Based on the [Modified PME
 method](https://en.wikipedia.org/wiki/Public_Market_Equivalent#Modified_PME).
```

