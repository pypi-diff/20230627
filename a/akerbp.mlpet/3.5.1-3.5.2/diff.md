# Comparing `tmp/akerbp.mlpet-3.5.1.tar.gz` & `tmp/akerbp.mlpet-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akerbp.mlpet-3.5.1.tar", last modified: Mon May 15 12:49:52 2023, max compression
+gzip compressed data, was "akerbp.mlpet-3.5.2.tar", last modified: Tue Jun 27 13:17:47 2023, max compression
```

## Comparing `akerbp.mlpet-3.5.1.tar` & `akerbp.mlpet-3.5.2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    19183 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5504 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2813 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.551735 akerbp.mlpet-3.5.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/Makefile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/docs/build/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/doctrees/
--rw-rw-rw-   0 root         (0) root         (0)    45723 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataloader.doctree
--rw-rw-rw-   0 root         (0) root         (0)    75232 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataset.doctree
--rw-rw-rw-   0 root         (0) root         (0)   102852 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.doctree
--rw-rw-rw-   0 root         (0) root         (0)   206422 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.feature_engineering.doctree
--rw-rw-rw-   0 root         (0) root         (0)    91063 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.imputers.doctree
--rw-rw-rw-   0 root         (0) root         (0)   180488 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.preprocessors.doctree
--rw-rw-rw-   0 root         (0) root         (0)   260035 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.utilities.doctree
--rw-rw-rw-   0 root         (0) root         (0)   231460 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/environment.pickle
--rw-rw-rw-   0 root         (0) root         (0)    20072 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/doctrees/index.doctree
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/html/
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/.buildinfo
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.555735 akerbp.mlpet-3.5.1/docs/build/html/_modules/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.559735 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/
--rw-rw-rw-   0 root         (0) root         (0)    25163 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataloader.html
--rw-rw-rw-   0 root         (0) root         (0)   104462 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataset.html
--rw-rw-rw-   0 root         (0) root         (0)   179606 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/feature_engineering.html
--rw-rw-rw-   0 root         (0) root         (0)    63553 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/imputers.html
--rw-rw-rw-   0 root         (0) root         (0)   114510 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/preprocessors.html
--rw-rw-rw-   0 root         (0) root         (0)    25544 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/transformer.html
--rw-rw-rw-   0 root         (0) root         (0)   158706 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/utilities.html
--rw-rw-rw-   0 root         (0) root         (0)    10828 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_modules/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.559735 akerbp.mlpet-3.5.1/docs/build/html/_sources/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.dataloader.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.dataset.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.feature_engineering.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.imputers.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.preprocessors.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.utilities.rst.txt
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/
--rw-rw-rw-   0 root         (0) root         (0)    14692 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)     9758 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/doctools.js
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/documentation_options.js
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/file.png
--rw-rw-rw-   0 root         (0) root         (0)   287630 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0 root         (0) root         (0)    89476 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    10854 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/language_data.js
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/plus.png
--rw-rw-rw-   0 root         (0) root         (0)    20800 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/pygments.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo-extensions.js
--rw-rw-rw-   0 root         (0) root         (0)     4861 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    27037 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js.map
--rw-rw-rw-   0 root         (0) root         (0)    16793 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/searchtools.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/
--rw-rw-rw-   0 root         (0) root         (0)     5286 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css
--rw-rw-rw-   0 root         (0) root         (0)     7166 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css.map
--rw-rw-rw-   0 root         (0) root         (0)    46533 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css
--rw-rw-rw-   0 root         (0) root         (0)    68704 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css.map
--rw-rw-rw-   0 root         (0) root         (0)    68420 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0 root         (0) root         (0)    19530 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/_static/underscore.js
--rw-rw-rw-   0 root         (0) root         (0)    23735 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataloader.html
--rw-rw-rw-   0 root         (0) root         (0)    31194 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataset.html
--rw-rw-rw-   0 root         (0) root         (0)    80364 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.feature_engineering.html
--rw-rw-rw-   0 root         (0) root         (0)    40397 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.html
--rw-rw-rw-   0 root         (0) root         (0)    34042 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.imputers.html
--rw-rw-rw-   0 root         (0) root         (0)    56620 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.preprocessors.html
--rw-rw-rw-   0 root         (0) root         (0)    80790 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.utilities.html
--rw-rw-rw-   0 root         (0) root         (0)    33642 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/genindex.html
--rw-rw-rw-   0 root         (0) root         (0)    18106 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/objects.inv
--rw-rw-rw-   0 root         (0) root         (0)    12305 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/py-modindex.html
--rw-rw-rw-   0 root         (0) root         (0)    10462 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/search.html
--rw-rw-rw-   0 root         (0) root         (0)    17979 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/build/html/searchindex.js
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.563736 akerbp.mlpet-3.5.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.dataloader.rst
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.dataset.rst
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.feature_engineering.rst
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.imputers.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.preprocessors.rst
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.rst
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)     2199 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.547735 akerbp.mlpet-3.5.1/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/mappings.py
--rw-rw-rw-   0 root         (0) root         (0)    10241 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataloader.py
--rw-rw-rw-   0 root         (0) root         (0)    38374 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    29870 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/feature_engineering.py
--rw-rw-rw-   0 root         (0) root         (0)    16008 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/imputers.py
--rw-rw-rw-   0 root         (0) root         (0)    14307 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/petrophysical_features.py
--rw-rw-rw-   0 root         (0) root         (0)    18016 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    51691 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_variables.py
--rw-rw-rw-   0 root         (0) root         (0)    37276 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/preprocessors.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.571735 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-15 12:49:28.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.591736 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)  5616970 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/15_9-23.las
--rw-rw-rw-   0 root         (0) root         (0)  7480569 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/25_2-7.las
--rw-rw-rw-   0 root         (0) root         (0)  4598499 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/35_12-1.las
--rw-rw-rw-   0 root         (0) root         (0)    28130 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/data.py
--rw-rw-rw-   0 root         (0) root         (0)     4140 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_mappings.yaml
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_settings.yaml
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataloader.py
--rw-rw-rw-   0 root         (0) root         (0)     5361 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_feature_engineering.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_imputers.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_petrophysical_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_preprocessors.py
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     4548 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     4160 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)    63414 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/src/akerbp/mlpet/utilities.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 12:49:52.567736 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    19183 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-15 12:49:52.000000 akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-15 12:49:29.000000 akerbp.mlpet-3.5.1/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.505447 akerbp.mlpet-3.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    19183 2023-06-27 13:17:47.505447 akerbp.mlpet-3.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5504 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.461447 akerbp.mlpet-3.5.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/Makefile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.445447 akerbp.mlpet-3.5.2/docs/build/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.461447 akerbp.mlpet-3.5.2/docs/build/doctrees/
+-rw-rw-rw-   0 root         (0) root         (0)    45723 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.dataloader.doctree
+-rw-rw-rw-   0 root         (0) root         (0)    75232 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.dataset.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   102852 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   206422 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.feature_engineering.doctree
+-rw-rw-rw-   0 root         (0) root         (0)    91063 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.imputers.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   180488 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.preprocessors.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   260035 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.utilities.doctree
+-rw-rw-rw-   0 root         (0) root         (0)   231460 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/environment.pickle
+-rw-rw-rw-   0 root         (0) root         (0)    20072 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/doctrees/index.doctree
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.465447 akerbp.mlpet-3.5.2/docs/build/html/
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/.buildinfo
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.465447 akerbp.mlpet-3.5.2/docs/build/html/_modules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.445447 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.469447 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/
+-rw-rw-rw-   0 root         (0) root         (0)    25163 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/dataloader.html
+-rw-rw-rw-   0 root         (0) root         (0)   104462 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/dataset.html
+-rw-rw-rw-   0 root         (0) root         (0)   179606 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/feature_engineering.html
+-rw-rw-rw-   0 root         (0) root         (0)    63553 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/imputers.html
+-rw-rw-rw-   0 root         (0) root         (0)   114510 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/preprocessors.html
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/transformer.html
+-rw-rw-rw-   0 root         (0) root         (0)   158706 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/utilities.html
+-rw-rw-rw-   0 root         (0) root         (0)    10828 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_modules/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.469447 akerbp.mlpet-3.5.2/docs/build/html/_sources/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.dataloader.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.dataset.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.feature_engineering.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.imputers.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.preprocessors.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.utilities.rst.txt
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.473447 akerbp.mlpet-3.5.2/docs/build/html/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    14692 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     9758 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/doctools.js
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/documentation_options.js
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/file.png
+-rw-rw-rw-   0 root         (0) root         (0)   287630 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0 root         (0) root         (0)    89476 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    10854 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/language_data.js
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/minus.png
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)    20800 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/pygments.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.477447 akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo-extensions.js
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo.js
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    27037 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    16793 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/searchtools.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.477447 akerbp.mlpet-3.5.2/docs/build/html/_static/styles/
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo-extensions.css
+-rw-rw-rw-   0 root         (0) root         (0)     7166 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo-extensions.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    46533 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo.css
+-rw-rw-rw-   0 root         (0) root         (0)    68704 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    68420 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0 root         (0) root         (0)    19530 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/_static/underscore.js
+-rw-rw-rw-   0 root         (0) root         (0)    23735 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.dataloader.html
+-rw-rw-rw-   0 root         (0) root         (0)    31194 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.dataset.html
+-rw-rw-rw-   0 root         (0) root         (0)    80364 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.feature_engineering.html
+-rw-rw-rw-   0 root         (0) root         (0)    40397 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.html
+-rw-rw-rw-   0 root         (0) root         (0)    34042 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.imputers.html
+-rw-rw-rw-   0 root         (0) root         (0)    56620 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.preprocessors.html
+-rw-rw-rw-   0 root         (0) root         (0)    80790 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.utilities.html
+-rw-rw-rw-   0 root         (0) root         (0)    33642 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/genindex.html
+-rw-rw-rw-   0 root         (0) root         (0)    18106 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/objects.inv
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/py-modindex.html
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/search.html
+-rw-rw-rw-   0 root         (0) root         (0)    17979 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/build/html/searchindex.js
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.477447 akerbp.mlpet-3.5.2/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.dataloader.rst
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.dataset.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.feature_engineering.rst
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.imputers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.preprocessors.rst
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.rst
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.utilities.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-27 13:17:47.505447 akerbp.mlpet-3.5.2/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.449447 akerbp.mlpet-3.5.2/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.449447 akerbp.mlpet-3.5.2/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.481447 akerbp.mlpet-3.5.2/src/akerbp/mlpet/
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.481447 akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/mappings.py
+-rw-rw-rw-   0 root         (0) root         (0)    10241 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/dataloader.py
+-rw-rw-rw-   0 root         (0) root         (0)    38470 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    29870 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/feature_engineering.py
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/imputers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14307 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/petrophysical_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    18016 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    51691 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    37276 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/preprocessors.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.481447 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.505447 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)  5616970 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/15_9-23.las
+-rw-rw-rw-   0 root         (0) root         (0)  7480569 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/25_2-7.las
+-rw-rw-rw-   0 root         (0) root         (0)  4598499 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/35_12-1.las
+-rw-rw-rw-   0 root         (0) root         (0)    28130 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4140 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/test_mappings.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/test_settings.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_dataloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5361 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_feature_engineering.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_imputers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_petrophysical_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_preprocessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4548 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)    63954 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/src/akerbp/mlpet/utilities.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 13:17:47.477447 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    19183 2023-06-27 13:17:47.000000 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-06-27 13:17:47.000000 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 13:17:47.000000 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-27 13:17:47.000000 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-27 13:17:47.000000 akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-27 13:17:28.000000 akerbp.mlpet-3.5.2/version.py
```

### Comparing `akerbp.mlpet-3.5.1/.flake8` & `akerbp.mlpet-3.5.2/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/.gitignore` & `akerbp.mlpet-3.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/.pre-commit-config.yaml` & `akerbp.mlpet-3.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/LICENSE` & `akerbp.mlpet-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/PKG-INFO` & `akerbp.mlpet-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlpet
-Version: 3.5.1
+Version: 3.5.2
 Summary: Package to prepare well log data for ML projects.
 Author-email: Flavia Dias Casagrande <flavia.dias.casagrande@akerbp.com>, Saghar Asadi <saghar.asadi@akerbp.com>, Yann Van Crombrugge <yann.vancrombrugge@akerbp.com>
 Maintainer-email: Yann Van Crombrugge <yann.vancrombrugge@akerbp.com>, Peder Aursand <peder.aursand@akerbp.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlpet-3.5.1/README.md` & `akerbp.mlpet-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/bitbucket-pipelines.yml` & `akerbp.mlpet-3.5.2/bitbucket-pipelines.yml`

 * *Files 3% similar despite different names*

```diff
@@ -67,27 +67,35 @@
         trigger: manual
         caches:
           - pip
         script:
           - pip install twine==4.0.2 build==0.10.0
           - python -m build
           - python -m twine upload --non-interactive dist/* --username=$TWINE_USERNAME --password=$TWINE_PASSWORD
+    - step: &sca
+        name: pip-audit for Dependency Vulnerabilities
+        caches:
+          - pip
+        script:
+          - pip install pip-audit
+          - pip-audit -S -v .
 
 pipelines:
   pull-requests:
     "**": # Run for PRs from all branches
       - parallel:
           - step: *unit-testing
           - step: *scan
           - step: *flake8-linting
           - step: *mypy-type-checking
           - step: *black-formatting
           - step: *isort-sorting
           - step: *version-checking
           - step: *check-install # Check install in empty environment with no preset environment variables.
+          - step: *sca
 
   branches:
     master:
       - step:
           name: Mirror latest version to public repo
           script:
             - git remote add public git@bitbucket.org:akerbp/akerbp.mlpet.git
```

### Comparing `akerbp.mlpet-3.5.1/docs/Makefile` & `akerbp.mlpet-3.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataloader.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.dataloader.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.dataset.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.dataset.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.feature_engineering.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.feature_engineering.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.imputers.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.imputers.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.preprocessors.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.preprocessors.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/akerbp.mlpet.utilities.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/akerbp.mlpet.utilities.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/environment.pickle` & `akerbp.mlpet-3.5.2/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/doctrees/index.doctree` & `akerbp.mlpet-3.5.2/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataloader.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/dataloader.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/dataset.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/dataset.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/feature_engineering.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/feature_engineering.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/imputers.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/imputers.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/preprocessors.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/preprocessors.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/transformer.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/transformer.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/akerbp/mlpet/utilities.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/akerbp/mlpet/utilities.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_modules/index.html` & `akerbp.mlpet-3.5.2/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.feature_engineering.rst.txt` & `akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.feature_engineering.rst.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.preprocessors.rst.txt` & `akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.preprocessors.rst.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_sources/akerbp.mlpet.utilities.rst.txt` & `akerbp.mlpet-3.5.2/docs/build/html/_sources/akerbp.mlpet.utilities.rst.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/basic.css` & `akerbp.mlpet-3.5.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/doctools.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/jquery-3.5.1.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/jquery.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/language_data.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/pygments.css` & `akerbp.mlpet-3.5.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/scripts/furo.js.map` & `akerbp.mlpet-3.5.2/docs/build/html/_static/scripts/furo.js.map`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/searchtools.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css` & `akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo-extensions.css`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo-extensions.css.map` & `akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo-extensions.css.map`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css` & `akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo.css`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/styles/furo.css.map` & `akerbp.mlpet-3.5.2/docs/build/html/_static/styles/furo.css.map`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/underscore-1.13.1.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/_static/underscore.js` & `akerbp.mlpet-3.5.2/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataloader.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.dataloader.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.dataset.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.dataset.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.feature_engineering.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.feature_engineering.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.imputers.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.imputers.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.preprocessors.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.preprocessors.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/akerbp.mlpet.utilities.html` & `akerbp.mlpet-3.5.2/docs/build/html/akerbp.mlpet.utilities.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/genindex.html` & `akerbp.mlpet-3.5.2/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/index.html` & `akerbp.mlpet-3.5.2/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/objects.inv` & `akerbp.mlpet-3.5.2/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/py-modindex.html` & `akerbp.mlpet-3.5.2/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/search.html` & `akerbp.mlpet-3.5.2/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/build/html/searchindex.js` & `akerbp.mlpet-3.5.2/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/make.bat` & `akerbp.mlpet-3.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.feature_engineering.rst` & `akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.feature_engineering.rst`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.preprocessors.rst` & `akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.preprocessors.rst`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/source/akerbp.mlpet.utilities.rst` & `akerbp.mlpet-3.5.2/docs/source/akerbp.mlpet.utilities.rst`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/docs/source/conf.py` & `akerbp.mlpet-3.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/pyproject.toml` & `akerbp.mlpet-3.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "akerbp.mlpet"
-version = "3.5.1"
+version = "3.5.2"
 description = "Package to prepare well log data for ML projects."
 authors = [
     {name = "Flavia Dias Casagrande", email = "flavia.dias.casagrande@akerbp.com"},
     {name = "Saghar Asadi", email = "saghar.asadi@akerbp.com"},
     {name = "Yann Van Crombrugge", email = "yann.vancrombrugge@akerbp.com"}
 ]
 maintainers = [
@@ -29,14 +29,15 @@
     "numpy>=1.19.5",
     "pandas>=1.3.2,<2",
     "scikit-learn>=0.24.2",
     "scipy>=1.7.1",
     "tqdm>=4.62.3",
     "plotly>=5.8.2",
     "importlib-metadata>=4.12.0",
+    "pyodbc>=4.0.35",
 ]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://bitbucket.org/akerbp/akerbp.mlpet/"
 
 [project.readme]
```

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/mappings.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/data/npd_fm_gp_sy_key_dic.pcl`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/dataset.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import warnings
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Union
 
 import numpy as np
@@ -522,14 +523,15 @@
 
         # <---------------- Perform preprocessing pipeline ------------------> #
         pbar = tqdm(
             kwargs.items(),
             desc="Preprocessing",
             disable=(not self.verbose),
             unit="function",
+            file=sys.stdout,  # Default to printing all tqdm related stuff to stdout
         )
         artifacts = {}
         start_columns = set(df.columns)
         new_features: Set[List[str]] = set([])
         for function, settings in pbar:
             if verbose:
                 tqdm.write(f"Running {function}")
```

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/feature_engineering.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/imputers.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/imputers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/petrophysical_features.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/petrophysical_features.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_helpers.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/plotting_variables.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/plotting_variables.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/preprocessors.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/preprocessors.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/15_9-23.las` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/15_9-23.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/25_2-7.las` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/25_2-7.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/35_12-1.las` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/35_12-1.las`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/data.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/data.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_mappings.yaml` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/test_mappings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/data/test_settings.yaml` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/data/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataloader.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_dataset.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_feature_engineering.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_imputers.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_imputers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_petrophysical_features.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_petrophysical_features.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_preprocessors.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_transformer.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/tests/test_utilities.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/transformer.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/transformer.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/src/akerbp/mlpet/utilities.py` & `akerbp.mlpet-3.5.2/src/akerbp/mlpet/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -807,22 +807,29 @@
         )
         if tops is None or len(tops) == 0:
             if load_from_gis:
                 try:
                     try:
                         import pyodbc
                     except ImportError as e:
-                        raise ImportError(
-                            "Could not import pyodbc. This is a very windows spesific package\
-                                and macOS/Linus users might need to install additional updates in order to install pyodbc"
+                        raise Exception(
+                            "Could not import pyodbc. If you are on a Unix "
+                            "system, you need to install additional libraries "
+                            "to be able to use pyodbc. See "
+                            "https://learn.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16&tabs=ubuntu18-install%2Calpine17-install%2Cdebian8-install%2Credhat7-13-install%2Crhel7-offline"
                         ) from e
 
-                    cnxn = pyodbc.connect(
-                        "DRIVER={SQL Server};SERVER=arcgis2.db.pertra.locale\\felles;DATABASE=GISData;Trusted_Connection=yes;"
-                    )
+                    try:
+                        cnxn = pyodbc.connect(
+                            "DRIVER={SQL Server};SERVER=arcgis2.db.pertra.locale\\felles;DATABASE=GISData;Trusted_Connection=yes;"
+                        )
+                    except pyodbc.Error as e:
+                        raise Exception(
+                            "Could not connect to GIS database. Please make sure you are connected to the Aker BP network."
+                        ) from e
                     QUERY = f"SELECT Wellbore, Chronostrat, Lithostrat, Top_MD, Base_MD FROM gisdata.Well_tops WHERE Wellbore='{well_name}'"
                     rows = pd.read_sql(QUERY, cnxn).sort_values(["Top_MD", "Base_MD"])
 
                     for i, r in rows.iterrows():
                         rows.loc[i, "Lithostrat"] = standardize_group_formation_name(
                             r.Lithostrat
                         )
```

### Comparing `akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/PKG-INFO` & `akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlpet
-Version: 3.5.1
+Version: 3.5.2
 Summary: Package to prepare well log data for ML projects.
 Author-email: Flavia Dias Casagrande <flavia.dias.casagrande@akerbp.com>, Saghar Asadi <saghar.asadi@akerbp.com>, Yann Van Crombrugge <yann.vancrombrugge@akerbp.com>
 Maintainer-email: Yann Van Crombrugge <yann.vancrombrugge@akerbp.com>, Peder Aursand <peder.aursand@akerbp.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlpet-3.5.1/src/akerbp.mlpet.egg-info/SOURCES.txt` & `akerbp.mlpet-3.5.2/src/akerbp.mlpet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlpet-3.5.1/version.py` & `akerbp.mlpet-3.5.2/version.py`

 * *Files identical despite different names*

