# Comparing `tmp/cadquery-2.2.0b2.tar.gz` & `tmp/cadquery-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadquery-2.2.0b2.tar", last modified: Mon Oct 10 18:41:03 2022, max compression
+gzip compressed data, was "cadquery-2.3.0.tar", last modified: Tue Jun 27 20:17:25 2023, max compression
```

## Comparing `cadquery-2.2.0b2.tar` & `cadquery-2.3.0.tar`

### file list

```diff
@@ -1,206 +1,207 @@
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.130442 cadquery-2.2.0b2/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      151 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.coveragerc
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      271 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.gitattributes
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.102442 cadquery-2.2.0b2/.github/
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.106442 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      270 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/00-generic-issue.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      396 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1140 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/exception_crash_report.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1087 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/modelling-question.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      338 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/occt-feature-request.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      272 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.gitignore
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       49 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/.readthedocs.yaml
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    11582 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/LICENSE
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       44 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/MANIFEST.in
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    19292 2022-10-10 18:41:03.130442 cadquery-2.2.0b2/PKG-INFO
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    18177 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/README.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1110 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/appveyor.yml
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      869 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/azure-pipelines.yml
--rwxrwxr-x   0 jwright   (1000) jwright   (1000)       60 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/build-docs.sh
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.106442 cadquery-2.2.0b2/cadquery/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      238 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/README.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1570 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    15978 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/assembly.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.106442 cadquery-2.2.0b2/cadquery/contrib/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      786 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/contrib/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   164077 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/cq.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    10468 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/cq_directive.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    17515 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/cqgi.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9319 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/hull.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.106442 cadquery-2.2.0b2/cadquery/occ_impl/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       37 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/README.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6383 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/assembly.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/cadquery/occ_impl/exporters/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6441 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1335 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/amf.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5236 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/assembly.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3026 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/dxf.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1878 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/json.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9136 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/svg.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5019 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/threemf.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      202 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/utils.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      656 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/exporters/vtk.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    31346 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/geom.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/cadquery/occ_impl/importers/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2324 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/importers/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5213 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/importers/dxf.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5733 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/jupyter_tools.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   110314 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/shapes.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9353 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/sketch_solver.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    17972 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/occ_impl/solver.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/cadquery/plugins/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      841 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/plugins/__init__.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/py.typed
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    26128 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/selectors.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    26847 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/sketch.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       51 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/types.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       59 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/units.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1727 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/cadquery/utils.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.106442 cadquery-2.2.0b2/cadquery.egg-info/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    19292 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/PKG-INFO
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5219 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/SOURCES.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)        1 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/dependency_links.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)        1 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/not-zip-safe
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      170 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/requires.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)        9 2022-10-10 18:41:03.000000 cadquery-2.2.0b2/cadquery.egg-info/top_level.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    20690 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/changes.md
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/conda/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      726 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/meta.yaml
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/conda/web-installer/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       96 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/.gitignore
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      886 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/Readme.md
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2106 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/build.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      591 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/construct.yaml.jinja2
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      239 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/post-install.bat.jinja2
--rwxrwxr-x   0 jwright   (1000) jwright   (1000)      270 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda/web-installer/post-install.sh.jinja2
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       73 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda_build.bat
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       73 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda_build.sh
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       17 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/conda_build_config.yaml
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.110442 cadquery-2.2.0b2/doc/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       76 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/README
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.114441 cadquery-2.2.0b2/doc/_static/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    59186 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/ParametricPulley.PNG
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   139192 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/assy.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9385 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/block.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    27451 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/cadquery_cheatsheet.html
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    40378 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/door_assy.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    39775 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/door_assy_freecad.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    27301 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/hyOzd-cablefix.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   149415 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/hyOzd-finished.jpg
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.118441 cadquery-2.2.0b2/doc/_static/importexport/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1528 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/importexport/box_custom_options.svg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2405 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/importexport/box_default_options.svg
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.118441 cadquery-2.2.0b2/doc/_static/logo/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      121 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/README.md
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.118441 cadquery-2.2.0b2/doc/_static/logo/Roboto_Font/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    11560 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/Roboto_Font/LICENSE.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   170760 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/Roboto_Font/Roboto-Bold.ttf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3965 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_dark.svg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2783 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_dark_inkscape.svg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3973 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_light.svg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2785 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_light_inkscape.svg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3163 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/new_badge.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    66208 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/parametric-cup-screencap.PNG
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    59428 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/parametric-pillowblock-screencap.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    17582 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/pillowblock.png
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.118441 cadquery-2.2.0b2/doc/_static/quickstart/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    36021 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/000.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    38803 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/001.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   125731 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/002.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   147791 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/003.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   185063 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/004.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   192146 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart/005.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6162 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart-1.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6162 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart-2.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7084 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart-3.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7095 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart-4.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    11703 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart-5.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    17947 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/quickstart.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    21577 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/simple_assy.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     8698 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/simpleblock.png
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      138 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/tables.css
--rw-rw-r--   0 jwright   (1000) jwright   (1000)  2398290 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/_static/vtk.js
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5316 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/apireference.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    92540 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/assy.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1719 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/classreference.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    10473 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/conf.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7750 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/cqgi.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3299 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/designprinciples.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    49613 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/examples.rst
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.118441 cadquery-2.2.0b2/doc/ext/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    11026 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/ext/sphinx_autodoc_multimethod.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7714 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/extending.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      862 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/fileformat.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1873 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/gen_colors.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    10580 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/importexport.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1588 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/index.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     3391 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/installation.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     4150 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/intro.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    36904 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/primer.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9129 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/quickstart.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1993 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/roadmap.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6878 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/selectors.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7180 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/sketch.rst
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    56566 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/doc/vslot-2020_1.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      482 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/environment.yml
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.126442 cadquery-2.2.0b2/examples/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)  4570724 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/CQ examples.ipynb
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      754 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex001_Simple_Block.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      954 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex002_Block_With_Bored_Center_Hole.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1932 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex003_Pillow_Block_With_Counterbored_Holes.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1420 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex004_Extruded_Cylindrical_Plate.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2451 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex005_Extruded_Lines_and_Arcs.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1680 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex006_Moving_the_Current_Working_Point.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1422 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex007_Using_Point_Lists.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2073 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex008_Polygon_Creation.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1541 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex009_Polylines.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      730 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex010_Defining_an_Edge_with_a_Spline.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      786 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex011_Mirroring_Symmetric_Geometry.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      625 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex012_Creating_Workplanes_on_Faces.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      953 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex013_Locating_a_Workplane_on_a_Vertex.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      811 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex014_Offset_Workplanes.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1067 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex015_Rotated_Workplanes.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      960 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex016_Using_Construction_Geometry.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      631 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex017_Shelling_to_Create_Thin_Features.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      937 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex018_Making_Lofts.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      940 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex019_Counter_Sunk_Holes.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      630 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex020_Rounding_Corners_with_Fillets.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1259 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex021_Splitting_an_Object.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1054 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex022_Revolution.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1538 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex023_Sweep.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2232 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex024_Sweep_With_Multiple_Sections.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      620 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex025_Swept_Helix.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1274 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex026_Case_Seam_Lip.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1634 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex100_Lego_Brick.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5427 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/examples/Ex101_InterpPlate.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      594 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/mypy.ini
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       38 2022-10-10 18:41:03.130442 cadquery-2.2.0b2/setup.cfg
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     2882 2022-10-10 18:38:48.000000 cadquery-2.2.0b2/setup.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.126442 cadquery-2.2.0b2/tests/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)       67 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/README.txt
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     1409 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/__init__.py
--rwxrwxr-x   0 jwright   (1000) jwright   (1000)     2128 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/naca.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    20693 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_assembly.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    24442 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_cad_objects.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   184331 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_cadquery.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6525 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_cqgi.py
--rwxrwxr-x   0 jwright   (1000) jwright   (1000)     1751 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_examples.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    10404 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_exporters.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      806 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_hull.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     6111 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_importers.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      746 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_jupyter.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    41524 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_selectors.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    17966 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_sketch.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)      580 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_utils.py
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     9975 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/test_workplanes.py
-drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2022-10-10 18:41:03.130442 cadquery-2.2.0b2/tests/testdata/
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   184298 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/1001.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   267838 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/MC 12x31.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    96932 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/OpenSans-Regular.ttf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   108437 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/gear.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     7428 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/genshi.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    13267 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/rational_spline.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)    18322 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/red_cube_blue_cylinder.step
--rw-rw-r--   0 jwright   (1000) jwright   (1000)     5135 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/spline.dxf
--rw-rw-r--   0 jwright   (1000) jwright   (1000)   135695 2022-10-10 18:35:27.000000 cadquery-2.2.0b2/tests/testdata/three_layers.dxf
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.713999 cadquery-2.3.0/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      151 2023-04-08 16:04:46.000000 cadquery-2.3.0/.coveragerc
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      271 2023-04-08 16:04:46.000000 cadquery-2.3.0/.gitattributes
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.645998 cadquery-2.3.0/.github/
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.653998 cadquery-2.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      270 2023-04-08 16:04:46.000000 cadquery-2.3.0/.github/ISSUE_TEMPLATE/00-generic-issue.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      396 2023-04-08 16:04:46.000000 cadquery-2.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1140 2023-04-08 16:04:46.000000 cadquery-2.3.0/.github/ISSUE_TEMPLATE/exception_crash_report.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1087 2023-04-08 16:04:46.000000 cadquery-2.3.0/.github/ISSUE_TEMPLATE/modelling-question.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      338 2023-04-08 16:04:46.000000 cadquery-2.3.0/.github/ISSUE_TEMPLATE/occt-feature-request.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      337 2023-06-15 00:40:35.000000 cadquery-2.3.0/.gitignore
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      118 2023-04-08 16:04:46.000000 cadquery-2.3.0/.readthedocs.yaml
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    11582 2023-04-08 16:04:46.000000 cadquery-2.3.0/LICENSE
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       44 2023-04-08 16:04:46.000000 cadquery-2.3.0/MANIFEST.in
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    15946 2023-06-27 20:17:25.713999 cadquery-2.3.0/PKG-INFO
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    14839 2023-06-15 00:40:43.000000 cadquery-2.3.0/README.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1509 2023-06-15 00:40:35.000000 cadquery-2.3.0/appveyor.yml
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      510 2023-06-15 00:31:54.000000 cadquery-2.3.0/azure-pipelines.yml
+-rwxrwxr-x   0 jwright   (1000) jwright   (1000)       60 2023-04-08 16:04:46.000000 cadquery-2.3.0/build-docs.sh
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.657998 cadquery-2.3.0/cadquery/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      238 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/README.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1568 2023-06-27 20:15:43.000000 cadquery-2.3.0/cadquery/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    16664 2023-06-15 00:40:35.000000 cadquery-2.3.0/cadquery/assembly.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.657998 cadquery-2.3.0/cadquery/contrib/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      786 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/contrib/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   163068 2023-06-26 13:17:13.000000 cadquery-2.3.0/cadquery/cq.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9855 2023-06-22 20:40:20.000000 cadquery-2.3.0/cadquery/cq_directive.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    17535 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/cqgi.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9319 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/hull.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.661998 cadquery-2.3.0/cadquery/occ_impl/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       37 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/README.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)        0 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    12712 2023-06-15 00:40:35.000000 cadquery-2.3.0/cadquery/occ_impl/assembly.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.665998 cadquery-2.3.0/cadquery/occ_impl/exporters/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6458 2023-06-26 13:17:13.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1335 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/amf.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6883 2023-06-15 00:40:35.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/assembly.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    10908 2023-06-15 00:31:54.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/dxf.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1878 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/json.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9480 2023-06-22 20:40:17.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/svg.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5019 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/threemf.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      202 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/utils.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      656 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/exporters/vtk.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    31346 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/geom.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.665998 cadquery-2.3.0/cadquery/occ_impl/importers/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2411 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/importers/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5213 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/importers/dxf.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5733 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/jupyter_tools.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   111494 2023-06-15 00:40:35.000000 cadquery-2.3.0/cadquery/occ_impl/shapes.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9363 2023-06-22 20:40:20.000000 cadquery-2.3.0/cadquery/occ_impl/sketch_solver.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    18100 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/occ_impl/solver.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.665998 cadquery-2.3.0/cadquery/plugins/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      841 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/plugins/__init__.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)        0 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/py.typed
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    26129 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/selectors.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    26884 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/sketch.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       51 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/types.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       59 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/units.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1671 2023-04-08 16:04:46.000000 cadquery-2.3.0/cadquery/utils.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.657998 cadquery-2.3.0/cadquery.egg-info/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    15946 2023-06-27 20:17:25.000000 cadquery-2.3.0/cadquery.egg-info/PKG-INFO
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5279 2023-06-27 20:17:25.000000 cadquery-2.3.0/cadquery.egg-info/SOURCES.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)        1 2023-06-27 20:17:25.000000 cadquery-2.3.0/cadquery.egg-info/dependency_links.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)        1 2023-04-08 16:06:38.000000 cadquery-2.3.0/cadquery.egg-info/not-zip-safe
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       78 2023-06-27 20:17:25.000000 cadquery-2.3.0/cadquery.egg-info/requires.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)        9 2023-06-27 20:17:25.000000 cadquery-2.3.0/cadquery.egg-info/top_level.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    31014 2023-06-27 20:15:43.000000 cadquery-2.3.0/changes.md
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.665998 cadquery-2.3.0/conda/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      705 2023-06-15 00:31:54.000000 cadquery-2.3.0/conda/meta.yaml
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.669998 cadquery-2.3.0/conda/web-installer/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       96 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/.gitignore
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      886 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/Readme.md
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2106 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/build.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      591 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/construct.yaml.jinja2
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      239 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/post-install.bat.jinja2
+-rwxrwxr-x   0 jwright   (1000) jwright   (1000)      270 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda/web-installer/post-install.sh.jinja2
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       73 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda_build.bat
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       73 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda_build.sh
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       17 2023-04-08 16:04:46.000000 cadquery-2.3.0/conda_build_config.yaml
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.673998 cadquery-2.3.0/doc/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       76 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/README
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.681998 cadquery-2.3.0/doc/_static/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    59186 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/ParametricPulley.PNG
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   139192 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/assy.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9385 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/block.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    27453 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/cadquery_cheatsheet.html
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    40378 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/door_assy.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    39775 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/door_assy_freecad.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    27301 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/hyOzd-cablefix.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   149415 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/hyOzd-finished.jpg
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.685998 cadquery-2.3.0/doc/_static/importexport/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1528 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/importexport/box_custom_options.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1484 2023-06-15 00:31:54.000000 cadquery-2.3.0/doc/_static/importexport/box_custom_options_perspective.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2405 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/importexport/box_default_options.svg
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.685998 cadquery-2.3.0/doc/_static/logo/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      121 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/README.md
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.689998 cadquery-2.3.0/doc/_static/logo/Roboto_Font/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    11560 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/Roboto_Font/LICENSE.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   170760 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/Roboto_Font/Roboto-Bold.ttf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     3965 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/cadquery_logo_dark.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2783 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/cadquery_logo_dark_inkscape.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     3973 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/cadquery_logo_light.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2785 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/logo/cadquery_logo_light_inkscape.svg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     3163 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/new_badge.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    66208 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/parametric-cup-screencap.PNG
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    59428 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/parametric-pillowblock-screencap.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    17582 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/pillowblock.png
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.689998 cadquery-2.3.0/doc/_static/quickstart/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    36021 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/000.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    38803 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/001.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   125731 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/002.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   147791 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/003.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   185063 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/004.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   192146 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart/005.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6162 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart-1.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6162 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart-2.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7084 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart-3.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7095 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart-4.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    11703 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart-5.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    17947 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/quickstart.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    21577 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/simple_assy.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     8698 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/simpleblock.png
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      138 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/tables.css
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)  2398290 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/_static/vtk.js
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5355 2023-06-15 00:31:54.000000 cadquery-2.3.0/doc/apireference.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    92272 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/assy.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1874 2023-06-15 00:31:54.000000 cadquery-2.3.0/doc/classreference.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    10681 2023-06-27 20:15:43.000000 cadquery-2.3.0/doc/conf.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7750 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/cqgi.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     3299 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/designprinciples.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    49613 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/examples.rst
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.689998 cadquery-2.3.0/doc/ext/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    11026 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/ext/sphinx_autodoc_multimethod.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7714 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/extending.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      862 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/fileformat.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1873 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/gen_colors.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    17965 2023-06-22 20:40:17.000000 cadquery-2.3.0/doc/importexport.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1588 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/index.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     8789 2023-06-15 00:40:43.000000 cadquery-2.3.0/doc/installation.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     4150 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/intro.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    36905 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/primer.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9113 2023-06-15 00:40:35.000000 cadquery-2.3.0/doc/quickstart.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1993 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/roadmap.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6878 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/selectors.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7323 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/sketch.rst
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    56566 2023-04-08 16:04:46.000000 cadquery-2.3.0/doc/vslot-2020_1.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      458 2023-06-22 20:40:20.000000 cadquery-2.3.0/environment.yml
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.705999 cadquery-2.3.0/examples/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)  4570724 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/CQ examples.ipynb
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      754 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex001_Simple_Block.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      954 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex002_Block_With_Bored_Center_Hole.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1932 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex003_Pillow_Block_With_Counterbored_Holes.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1420 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex004_Extruded_Cylindrical_Plate.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2451 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex005_Extruded_Lines_and_Arcs.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1680 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex006_Moving_the_Current_Working_Point.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1422 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex007_Using_Point_Lists.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2073 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex008_Polygon_Creation.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1541 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex009_Polylines.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      730 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex010_Defining_an_Edge_with_a_Spline.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      786 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex011_Mirroring_Symmetric_Geometry.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      625 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex012_Creating_Workplanes_on_Faces.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      953 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex013_Locating_a_Workplane_on_a_Vertex.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      811 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex014_Offset_Workplanes.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1067 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex015_Rotated_Workplanes.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      960 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex016_Using_Construction_Geometry.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      631 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex017_Shelling_to_Create_Thin_Features.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      937 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex018_Making_Lofts.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      940 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex019_Counter_Sunk_Holes.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      630 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex020_Rounding_Corners_with_Fillets.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1259 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex021_Splitting_an_Object.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1054 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex022_Revolution.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1538 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex023_Sweep.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2232 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex024_Sweep_With_Multiple_Sections.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      620 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex025_Swept_Helix.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1274 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex026_Case_Seam_Lip.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1634 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex100_Lego_Brick.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5427 2023-04-08 16:04:46.000000 cadquery-2.3.0/examples/Ex101_InterpPlate.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      623 2023-04-08 16:04:46.000000 cadquery-2.3.0/mypy.ini
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       38 2023-06-27 20:17:25.713999 cadquery-2.3.0/setup.cfg
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     2927 2023-06-27 20:15:43.000000 cadquery-2.3.0/setup.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.709999 cadquery-2.3.0/tests/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)       67 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/README.txt
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     1409 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/__init__.py
+-rwxrwxr-x   0 jwright   (1000) jwright   (1000)     2128 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/naca.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    45440 2023-06-15 00:40:35.000000 cadquery-2.3.0/tests/test_assembly.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    24915 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_cad_objects.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   186495 2023-06-26 13:17:13.000000 cadquery-2.3.0/tests/test_cadquery.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6525 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_cqgi.py
+-rwxrwxr-x   0 jwright   (1000) jwright   (1000)     1751 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_examples.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    27003 2023-06-26 13:17:13.000000 cadquery-2.3.0/tests/test_exporters.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      806 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_hull.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     6111 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_importers.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      746 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_jupyter.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    41524 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_selectors.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    17973 2023-06-22 20:40:20.000000 cadquery-2.3.0/tests/test_sketch.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)      580 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_utils.py
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     9975 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/test_workplanes.py
+drwxrwxr-x   0 jwright   (1000) jwright   (1000)        0 2023-06-27 20:17:25.713999 cadquery-2.3.0/tests/testdata/
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   184298 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/1001.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   267838 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/MC 12x31.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    96932 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/OpenSans-Regular.ttf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   108437 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/gear.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     7428 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/genshi.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    13267 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/rational_spline.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)    18322 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/red_cube_blue_cylinder.step
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)     5135 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/spline.dxf
+-rw-rw-r--   0 jwright   (1000) jwright   (1000)   135695 2023-04-08 16:04:46.000000 cadquery-2.3.0/tests/testdata/three_layers.dxf
```

### Comparing `cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/exception_crash_report.md` & `cadquery-2.3.0/.github/ISSUE_TEMPLATE/exception_crash_report.md`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/.github/ISSUE_TEMPLATE/modelling-question.md` & `cadquery-2.3.0/.github/ISSUE_TEMPLATE/modelling-question.md`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/LICENSE` & `cadquery-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/PKG-INFO` & `cadquery-2.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadquery
-Version: 2.2.0b2
+Version: 2.3.0
 Summary: CadQuery is a parametric  scripting language for creating and traversing CAD models
 Home-page: https://github.com/CadQuery/cadquery
 Author: David Cowden
 Author-email: dave.cowden@gmail.com
 License: Apache Public License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ipython
 License-File: LICENSE
 
 ![CadQuery logo](./doc/_static/logo/cadquery_logo_dark.svg)
 # CadQuery
@@ -52,14 +52,18 @@
 
 1. The scripts use a standard programming language, Python, and thus can benefit from the associated infrastructure. This includes many standard libraries and IDEs.
 2. CadQuery's CAD kernel Open CASCADE Technology ([OCCT](https://en.wikipedia.org/wiki/Open_Cascade_Technology)) is much more powerful than the [CGAL](https://en.wikipedia.org/wiki/CGAL) used by OpenSCAD. Features supported natively by OCCT include NURBS, splines, surface sewing, STL repair, STEP import/export, and other complex operations, in addition to the standard CSG operations supported by CGAL
 3. Ability to import/export [STEP](https://en.wikipedia.org/wiki/ISO_10303) and the ability to begin with a STEP model, created in a CAD package, and then add parametric features. This is possible in OpenSCAD using STL, but STL is a lossy format.
 4. CadQuery scripts require less code to create most objects, because it is possible to locate features based on the position of other features, workplanes, vertices, etc.
 5. CadQuery scripts can build STL, STEP, AMF and 3MF faster than OpenSCAD.
 
+CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts.  Options for visualziation are also available including CQ-Editor and JupyterLab.
+
+For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+
 ### Key features
 * Build 3D models with scripts that are as close as possible to how you would describe the object to a human.
 * Create parametric models that can be very easily customized by end users.
 * Output high quality (loss-less) CAD formats like STEP and DXF in addition to STL, VRML, AMF and 3MF.
 * Provide a non-proprietary, plain text model format that can be edited and executed with only a web browser.
 * Offer advanced modeling capabilities such as fillets, curvilinear extrudes, parametric curves and lofts.
 * Build nested assemblies out of individual parts and other assemblies.
@@ -68,131 +72,86 @@
 
 The original version of CadQuery was built on the FreeCAD API. This was great because it allowed for fast development and easy cross-platform capability. However, we eventually started reaching the limits of the API for some advanced operations and selectors. This 2.0 version of CadQuery is based directly on a Python wrapper of the OCCT kernel. This gives us a great deal more control and flexibility, at the expense of some simplicity and having to handle the cross-platform aspects of deployment ourselves. We believe this is a worthwhile trade-off to allow CadQuery to continue to grow and expand in the future.
 
 ## Getting started
 
 To learn more about designing with CadQuery, visit the [documentation](https://cadquery.readthedocs.io/en/latest/intro.html), [examples](https://cadquery.readthedocs.io/en/latest/examples.html), and [cheatsheet](https://cadquery.readthedocs.io/en/latest/_static/cadquery_cheatsheet.html).
 
-To get started playing around with CadQuery and see it's capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.
+To get started playing around with CadQuery and see its capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.  The CQ-editor installer bundles both CQ-editor and CadQuery (recommended).  See the [CQ-editor installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor).
 
-There are currently 4 different ways to use CadQuery for designing your next project:
-* Using the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor)
-* From a [Jupyter notebook](https://github.com/bernhard-42/jupyter-cadquery)
-* Using a [VSCode extension](https://marketplace.visualstudio.com/items?itemName=roipoussiere.cadquery)
-* As a standalone library
-    * Linux [installation video](https://youtu.be/sjLTePOq8bQ)
-    * Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
+The CadQuery library (with or without CQ-editor) and its dependencies may be installed using conda, or pip.  Note that conda (or the CQ-editor installer) is the better supported option.
 
-There are two ways to install CadQuery and its dependencies. One is using conda, and the other is using pip. Pip is shown first below, followed by two sections on installing CadQuery via conda, and a non-intrusive way to install conda on a system. Note that conda is the better supported option.
-
-### CadQuery Installation Via Pip
-
-CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method outlined in the next two sections.
-
-It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
-```
-python3 -m pip install --upgrade pip
-```
-Once a current version of pip is installed, CadQuery can be installed using the following command line.
-```
-pip install --pre cadquery
-```
-NB: CadQuery has only recently returned to PyPI, and a full release has not happened yet. When the final release of CadQuery 2.2 is published, it will be possible to simply type `pip install cadquery`.
+See the documentation for detailed CadQuery [installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html).
 
-It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
-```
-pip install git+https://github.com/CadQuery/cadquery.git
-```
+There are also videos covering installation:
 
-You should now have a working CadQuery installation, but developers or users who want to use CadQuery with IPython/Jupyter or to set up a developer environment can read the rest of this section.
+* Linux [installation video](https://youtu.be/sjLTePOq8bQ)
+* Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
-If you are installing CadQuery to use with IPython/Jupyter, you may want to run the following command line to install the extra dependencies.
-```
-pip install cadquery[ipython]==2.2.0b0
-```
+### CadQuery Installation Via Conda
 
-If you want to create a developer setup to contribute to CadQuery, the following command line will install all the development dependencies that are needed.
-```
-pip install cadquery[dev]==2.2.0b0
-```
+To first install the Conda package manager see [Install the Conda Package Manager](https://cadquery.readthedocs.io/en/latest/installation.html#install-the-conda-package-manager).
 
-### CadQuery Installation Via Conda
+The steps to install cadquery with conda are as follows:
 
-conda is included as part of a [miniforge](https://github.com/conda-forge/miniforge) installation (other distributions can be used as well). See the next section for more details regarding conda. The steps to install cadquery are as follows:
 ```
 # Set up a new environment
 conda create -n cadquery
 
 # Activate the new environment
 conda activate cadquery
 
-# CadQuery development is moving quickly, so it is best to install the latest version from GitHub master
+# Install the latest released version
+conda install -c conda-forge cadquery occt=7.7.0
+
+# Or install the dev version to get the latest changes
 conda install -c conda-forge -c cadquery cadquery=master
 ```
 
-For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+### CadQuery Installation Via Pip
 
-### Conda Installation
+CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method.
 
-For those unfamiliar (or uncomfortable) with conda, it is probably best to install Miniforge to a local directory and to avoid running `conda init`. After performing a local directory installation, Miniforge can be activated via the [scripts,bin]/activate scripts. This will help avoid polluting and breaking the local Python installation. In Linux, the local directory installation method looks something like this:
+It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
 ```
-# Install the script to ~/miniforge
-wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh -O miniforge.sh
-bash miniforge.sh -b -p $HOME/miniforge
-
-# To activate and use Miniconda
-source $HOME/miniforge/bin/activate
+python3 -m pip install --upgrade pip
 ```
-On Windows one can install locally as follows:
+Once a current version of pip is installed, CadQuery can be installed using the following command line.
+```
+pip install cadquery
 ```
-:: Install
-curl -L -o miniforge.exe https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe
-start /wait "" miniforge.exe /InstallationType=JustMe /RegisterPython=0 /NoRegistry=1 /NoScripts=1 /S /D=%USERPROFILE%\Miniforge3
 
-:: Activate
-cmd /K ""%USERPROFILE%/Miniforge3/Scripts/activate.bat" "%USERPROFILE%/Miniforge3""
+It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
 ```
-You might want to consider using `/NoScripts=0` to have an activation shortcut added to the start menu.
+pip install git+https://github.com/CadQuery/cadquery.git
+```
+
 
 ### CQ-editor GUI
 
 CQ-editor is an IDE that allows users to edit CadQuery model scripts in a GUI environment. It includes features such as:
 
 * A graphical debugger that allows you to step through your scripts.
 * A CadQuery stack inspector.
 * Export to various formats, including STEP and STL, directly from the menu.
 
-The installation instructions for CQ-editor can be found [here](https://github.com/CadQuery/CQ-editor#installation).
+More on CQ-editor:
+* [CQ-editor README](https://github.com/CadQuery/CQ-editor/blob/master/README.md)
+* [Installation](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor)
+
 
 <img src="https://raw.githubusercontent.com/CadQuery/CQ-editor/master/screenshots/screenshot3.png" alt="CQ editor screenshot" width="800"/>
 
 ### Jupyter
 
-CadQuery supports Jupyter notebook out of the box using the jupyter-cadquery extension created by @bernhard-42:
-
-* [Installation](https://github.com/bernhard-42/jupyter-cadquery#installation)
-* [Usage](https://github.com/bernhard-42/jupyter-cadquery#jupyter-cadquery)
-
-<img src="https://raw.githubusercontent.com/bernhard-42/jupyter-cadquery/master/screenshots/0_intro.png" alt="CadQuery Jupyter extension screenshot" width="800"/>
+CadQuery supports Jupyter out-of-the-box.  Run your CadQuery code in the notebook and visualize the model by calling ```display(<CadQuery object>)```.
 
-### Docker
+ * [JupyterLab installation](https://cadquery.readthedocs.io/en/latest/installation.html#jupyter).
 
-A list of Docker images can be found [here](https://github.com/RubenRubens/cq-containers), and includes images for the following projects.
-* [Core CadQuery library](https://github.com/RubenRubens/cq-containers/tree/master/cq-conda), which allows users to run CadQuery Python scripts without a GUI.
-* [cq-cli](https://github.com/RubenRubens/cq-containers/tree/master/cq-cli), a command line utility which is used to export the results of a CadQuery script to an output format (i.e. STL, STEP).
-* [jupyter-cadquery](https://github.com/bernhard-42/jupyter-cadquery#b-using-a-docker-image), makes CadQuery accessible through Jupyter Labs and provides a web-based GUI. This is currently the only image that provides a GUI.
-
-### Standalone Stable Version
-
-CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts. Use Anaconda/Miniconda to install CadQuery, and then add `import cadquery` to the top of your Python scripts. If the stable version of CadQuery is desired, the following command will install it. However, be aware that the stable version can fall significantly behind the current state of CadQuery, so in many cases the `master` installation method at the beginning of the Getting Started section is preferable.
-
-```
-conda install -c conda-forge -c cadquery cadquery=2
-```
 
 ## Getting help
 
 You can find the full CadQuery documentation at [cadquery.readthedocs.io](https://cadquery.readthedocs.io/).
 
 We also have a [Google Group](https://groups.google.com/forum/#!forum/cadquery) to make it easy to get help from other CadQuery users. We want you to feel welcome and encourage you to join the group and introduce yourself. We would also love to hear what you are doing with CadQuery.
 
@@ -212,15 +171,15 @@
 
 Hexidor is an expanded take on the Quoridor board game, and the development process has been chronicled [here](https://bruceisonfire.net/2020/04/23/my-adventure-with-flosscad-the-birth-of-hexidor/). CadQuery was used to generate the game board. Thanks to Bruce for this example.
 
 <img src="https://bruceisonfire.net/wp-content/uploads/2020/04/16-945x709.jpg" alt="Hexidor Board Game" width="400"/>
 
 ### Spindle assembly
 
-Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example). 
+Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example).
 
 <img src="./doc/_static/assy.png" width="400">
 
 ### 3D Printed Resin Mold
 
 Thanks to @eddieliberato for sharing [this example](https://jungletools.blogspot.com/2017/06/an-anti-kink-device-for-novel-high-tech.html) of an anti-kink resin mold for a cable.
```

### Comparing `cadquery-2.2.0b2/README.md` & `cadquery-2.3.0/cadquery.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: cadquery
+Version: 2.3.0
+Summary: CadQuery is a parametric  scripting language for creating and traversing CAD models
+Home-page: https://github.com/CadQuery/cadquery
+Author: David Cowden
+Author-email: dave.cowden@gmail.com
+License: Apache Public License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: ipython
+License-File: LICENSE
+
 ![CadQuery logo](./doc/_static/logo/cadquery_logo_dark.svg)
 # CadQuery
 
 [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/79ox42i6smelx7n8/branch/master?svg=true)](https://ci.appveyor.com/project/jmwright/cadquery-o18bh/branch/master)
 [![Build Status](https://dev.azure.com/cadquery/conda-packages/_apis/build/status/CadQuery.cadquery?branchName=master)](https://dev.azure.com/cadquery/conda-packages/_build/latest?definitionId=2&branchName=master)
 [![codecov](https://codecov.io/gh/CadQuery/cadquery/branch/master/graph/badge.svg)](https://codecov.io/gh/CadQuery/cadquery)
 [![Documentation Status](https://readthedocs.org/projects/cadquery/badge/?version=latest)](https://cadquery.readthedocs.io/en/latest/?badge=latest)
@@ -23,14 +52,18 @@
 
 1. The scripts use a standard programming language, Python, and thus can benefit from the associated infrastructure. This includes many standard libraries and IDEs.
 2. CadQuery's CAD kernel Open CASCADE Technology ([OCCT](https://en.wikipedia.org/wiki/Open_Cascade_Technology)) is much more powerful than the [CGAL](https://en.wikipedia.org/wiki/CGAL) used by OpenSCAD. Features supported natively by OCCT include NURBS, splines, surface sewing, STL repair, STEP import/export, and other complex operations, in addition to the standard CSG operations supported by CGAL
 3. Ability to import/export [STEP](https://en.wikipedia.org/wiki/ISO_10303) and the ability to begin with a STEP model, created in a CAD package, and then add parametric features. This is possible in OpenSCAD using STL, but STL is a lossy format.
 4. CadQuery scripts require less code to create most objects, because it is possible to locate features based on the position of other features, workplanes, vertices, etc.
 5. CadQuery scripts can build STL, STEP, AMF and 3MF faster than OpenSCAD.
 
+CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts.  Options for visualziation are also available including CQ-Editor and JupyterLab.
+
+For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+
 ### Key features
 * Build 3D models with scripts that are as close as possible to how you would describe the object to a human.
 * Create parametric models that can be very easily customized by end users.
 * Output high quality (loss-less) CAD formats like STEP and DXF in addition to STL, VRML, AMF and 3MF.
 * Provide a non-proprietary, plain text model format that can be edited and executed with only a web browser.
 * Offer advanced modeling capabilities such as fillets, curvilinear extrudes, parametric curves and lofts.
 * Build nested assemblies out of individual parts and other assemblies.
@@ -39,131 +72,86 @@
 
 The original version of CadQuery was built on the FreeCAD API. This was great because it allowed for fast development and easy cross-platform capability. However, we eventually started reaching the limits of the API for some advanced operations and selectors. This 2.0 version of CadQuery is based directly on a Python wrapper of the OCCT kernel. This gives us a great deal more control and flexibility, at the expense of some simplicity and having to handle the cross-platform aspects of deployment ourselves. We believe this is a worthwhile trade-off to allow CadQuery to continue to grow and expand in the future.
 
 ## Getting started
 
 To learn more about designing with CadQuery, visit the [documentation](https://cadquery.readthedocs.io/en/latest/intro.html), [examples](https://cadquery.readthedocs.io/en/latest/examples.html), and [cheatsheet](https://cadquery.readthedocs.io/en/latest/_static/cadquery_cheatsheet.html).
 
-To get started playing around with CadQuery and see it's capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.
+To get started playing around with CadQuery and see its capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.  The CQ-editor installer bundles both CQ-editor and CadQuery (recommended).  See the [CQ-editor installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor).
 
-There are currently 4 different ways to use CadQuery for designing your next project:
-* Using the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor)
-* From a [Jupyter notebook](https://github.com/bernhard-42/jupyter-cadquery)
-* Using a [VSCode extension](https://marketplace.visualstudio.com/items?itemName=roipoussiere.cadquery)
-* As a standalone library
-    * Linux [installation video](https://youtu.be/sjLTePOq8bQ)
-    * Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
+The CadQuery library (with or without CQ-editor) and its dependencies may be installed using conda, or pip.  Note that conda (or the CQ-editor installer) is the better supported option.
 
-There are two ways to install CadQuery and its dependencies. One is using conda, and the other is using pip. Pip is shown first below, followed by two sections on installing CadQuery via conda, and a non-intrusive way to install conda on a system. Note that conda is the better supported option.
+See the documentation for detailed CadQuery [installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html).
 
-### CadQuery Installation Via Pip
+There are also videos covering installation:
 
-CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method outlined in the next two sections.
+* Linux [installation video](https://youtu.be/sjLTePOq8bQ)
+* Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
-It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
-```
-python3 -m pip install --upgrade pip
-```
-Once a current version of pip is installed, CadQuery can be installed using the following command line.
-```
-pip install --pre cadquery
-```
-NB: CadQuery has only recently returned to PyPI, and a full release has not happened yet. When the final release of CadQuery 2.2 is published, it will be possible to simply type `pip install cadquery`.
+### CadQuery Installation Via Conda
 
-It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
-```
-pip install git+https://github.com/CadQuery/cadquery.git
-```
+To first install the Conda package manager see [Install the Conda Package Manager](https://cadquery.readthedocs.io/en/latest/installation.html#install-the-conda-package-manager).
 
-You should now have a working CadQuery installation, but developers or users who want to use CadQuery with IPython/Jupyter or to set up a developer environment can read the rest of this section.
+The steps to install cadquery with conda are as follows:
 
-If you are installing CadQuery to use with IPython/Jupyter, you may want to run the following command line to install the extra dependencies.
-```
-pip install cadquery[ipython]==2.2.0b0
-```
-
-If you want to create a developer setup to contribute to CadQuery, the following command line will install all the development dependencies that are needed.
-```
-pip install cadquery[dev]==2.2.0b0
-```
-
-### CadQuery Installation Via Conda
-
-conda is included as part of a [miniforge](https://github.com/conda-forge/miniforge) installation (other distributions can be used as well). See the next section for more details regarding conda. The steps to install cadquery are as follows:
 ```
 # Set up a new environment
 conda create -n cadquery
 
 # Activate the new environment
 conda activate cadquery
 
-# CadQuery development is moving quickly, so it is best to install the latest version from GitHub master
+# Install the latest released version
+conda install -c conda-forge cadquery occt=7.7.0
+
+# Or install the dev version to get the latest changes
 conda install -c conda-forge -c cadquery cadquery=master
 ```
 
-For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+### CadQuery Installation Via Pip
 
-### Conda Installation
+CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method.
 
-For those unfamiliar (or uncomfortable) with conda, it is probably best to install Miniforge to a local directory and to avoid running `conda init`. After performing a local directory installation, Miniforge can be activated via the [scripts,bin]/activate scripts. This will help avoid polluting and breaking the local Python installation. In Linux, the local directory installation method looks something like this:
+It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
 ```
-# Install the script to ~/miniforge
-wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh -O miniforge.sh
-bash miniforge.sh -b -p $HOME/miniforge
-
-# To activate and use Miniconda
-source $HOME/miniforge/bin/activate
+python3 -m pip install --upgrade pip
 ```
-On Windows one can install locally as follows:
+Once a current version of pip is installed, CadQuery can be installed using the following command line.
+```
+pip install cadquery
 ```
-:: Install
-curl -L -o miniforge.exe https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe
-start /wait "" miniforge.exe /InstallationType=JustMe /RegisterPython=0 /NoRegistry=1 /NoScripts=1 /S /D=%USERPROFILE%\Miniforge3
 
-:: Activate
-cmd /K ""%USERPROFILE%/Miniforge3/Scripts/activate.bat" "%USERPROFILE%/Miniforge3""
+It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
 ```
-You might want to consider using `/NoScripts=0` to have an activation shortcut added to the start menu.
+pip install git+https://github.com/CadQuery/cadquery.git
+```
+
 
 ### CQ-editor GUI
 
 CQ-editor is an IDE that allows users to edit CadQuery model scripts in a GUI environment. It includes features such as:
 
 * A graphical debugger that allows you to step through your scripts.
 * A CadQuery stack inspector.
 * Export to various formats, including STEP and STL, directly from the menu.
 
-The installation instructions for CQ-editor can be found [here](https://github.com/CadQuery/CQ-editor#installation).
+More on CQ-editor:
+* [CQ-editor README](https://github.com/CadQuery/CQ-editor/blob/master/README.md)
+* [Installation](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor)
+
 
 <img src="https://raw.githubusercontent.com/CadQuery/CQ-editor/master/screenshots/screenshot3.png" alt="CQ editor screenshot" width="800"/>
 
 ### Jupyter
 
-CadQuery supports Jupyter notebook out of the box using the jupyter-cadquery extension created by @bernhard-42:
-
-* [Installation](https://github.com/bernhard-42/jupyter-cadquery#installation)
-* [Usage](https://github.com/bernhard-42/jupyter-cadquery#jupyter-cadquery)
-
-<img src="https://raw.githubusercontent.com/bernhard-42/jupyter-cadquery/master/screenshots/0_intro.png" alt="CadQuery Jupyter extension screenshot" width="800"/>
+CadQuery supports Jupyter out-of-the-box.  Run your CadQuery code in the notebook and visualize the model by calling ```display(<CadQuery object>)```.
 
-### Docker
+ * [JupyterLab installation](https://cadquery.readthedocs.io/en/latest/installation.html#jupyter).
 
-A list of Docker images can be found [here](https://github.com/RubenRubens/cq-containers), and includes images for the following projects.
-* [Core CadQuery library](https://github.com/RubenRubens/cq-containers/tree/master/cq-conda), which allows users to run CadQuery Python scripts without a GUI.
-* [cq-cli](https://github.com/RubenRubens/cq-containers/tree/master/cq-cli), a command line utility which is used to export the results of a CadQuery script to an output format (i.e. STL, STEP).
-* [jupyter-cadquery](https://github.com/bernhard-42/jupyter-cadquery#b-using-a-docker-image), makes CadQuery accessible through Jupyter Labs and provides a web-based GUI. This is currently the only image that provides a GUI.
-
-### Standalone Stable Version
-
-CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts. Use Anaconda/Miniconda to install CadQuery, and then add `import cadquery` to the top of your Python scripts. If the stable version of CadQuery is desired, the following command will install it. However, be aware that the stable version can fall significantly behind the current state of CadQuery, so in many cases the `master` installation method at the beginning of the Getting Started section is preferable.
-
-```
-conda install -c conda-forge -c cadquery cadquery=2
-```
 
 ## Getting help
 
 You can find the full CadQuery documentation at [cadquery.readthedocs.io](https://cadquery.readthedocs.io/).
 
 We also have a [Google Group](https://groups.google.com/forum/#!forum/cadquery) to make it easy to get help from other CadQuery users. We want you to feel welcome and encourage you to join the group and introduce yourself. We would also love to hear what you are doing with CadQuery.
 
@@ -183,15 +171,15 @@
 
 Hexidor is an expanded take on the Quoridor board game, and the development process has been chronicled [here](https://bruceisonfire.net/2020/04/23/my-adventure-with-flosscad-the-birth-of-hexidor/). CadQuery was used to generate the game board. Thanks to Bruce for this example.
 
 <img src="https://bruceisonfire.net/wp-content/uploads/2020/04/16-945x709.jpg" alt="Hexidor Board Game" width="400"/>
 
 ### Spindle assembly
 
-Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example). 
+Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example).
 
 <img src="./doc/_static/assy.png" width="400">
 
 ### 3D Printed Resin Mold
 
 Thanks to @eddieliberato for sharing [this example](https://jungletools.blogspot.com/2017/06/an-anti-kink-device-for-novel-high-tech.html) of an anti-kink resin mold for a cable.
```

### Comparing `cadquery-2.2.0b2/cadquery/__init__.py` & `cadquery-2.3.0/cadquery/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from importlib.metadata import version, PackageNotFoundError
 
 try:
     __version__ = version("cadquery")
 except PackageNotFoundError:
     # package is not installed
-    __version__ = "2.2-dev"
+    __version__ = "2.3.0"
 
 # these items point to the OCC implementation
 from .occ_impl.geom import Plane, BoundBox, Vector, Matrix, Location
 from .occ_impl.shapes import (
     Shape,
     Vertex,
     Edge,
```

### Comparing `cadquery-2.2.0b2/cadquery/assembly.py` & `cadquery-2.3.0/cadquery/assembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from functools import reduce
-from typing import Union, Optional, List, Dict, Any, overload, Tuple, Iterator, cast
+from typing import (
+    Union,
+    Optional,
+    List,
+    Dict,
+    Any,
+    overload,
+    Tuple,
+    Iterator,
+    cast,
+    get_args,
+)
 from typing_extensions import Literal
 from typish import instance_of
 from uuid import uuid1 as uuid
 
 from .cq import Workplane
 from .occ_impl.shapes import Shape, Compound
 from .occ_impl.geom import Location
 from .occ_impl.assembly import Color
 from .occ_impl.solver import (
+    ConstraintKind,
     ConstraintSolver,
     ConstraintSpec as Constraint,
     UnaryConstraintKind,
     BinaryConstraintKind,
 )
 from .occ_impl.exporters.assembly import (
     exportAssembly,
     exportCAF,
     exportVTKJS,
     exportVRML,
     exportGLTF,
+    STEPExportModeLiterals,
+    ExportModes,
 )
 
 from .selectors import _expression_grammar as _selector_grammar
 
 # type definitions
 AssemblyObjects = Union[Shape, Workplane, None]
-ConstraintKinds = Literal["Plane", "Point", "Axis", "PointInPlane"]
-ExportLiterals = Literal["STEP", "XML", "GLTF", "VTKJS", "VRML"]
+ExportLiterals = Literal["STEP", "XML", "GLTF", "VTKJS", "VRML", "STL"]
 
 PATH_DELIM = "/"
 
 # entity selector grammar definiiton
 def _define_grammar():
 
     from pyparsing import (
@@ -167,24 +180,26 @@
     @overload
     def add(
         self,
         obj: AssemblyObjects,
         loc: Optional[Location] = None,
         name: Optional[str] = None,
         color: Optional[Color] = None,
+        metadata: Optional[Dict[str, Any]] = None,
     ) -> "Assembly":
         """
         Add a subassembly to the current assembly with explicit location and name.
 
         :param obj: object to be added as a subassembly
         :param loc: location of the root object (default: None, interpreted as identity
           transformation)
         :param name: unique name of the root object (default: None, resulting in an UUID being
           generated)
         :param color: color of the added object (default: None)
+        :param metadata: a store for user-defined metadata (default: None)
         """
         ...
 
     def add(self, arg, **kwargs):
         """
         Add a subassembly to the current assembly.
         """
@@ -197,14 +212,17 @@
                 raise ValueError("Unique name is required")
 
             subassy = arg._copy()
 
             subassy.loc = kwargs["loc"] if kwargs.get("loc") else arg.loc
             subassy.name = kwargs["name"] if kwargs.get("name") else arg.name
             subassy.color = kwargs["color"] if kwargs.get("color") else arg.color
+            subassy.metadata = (
+                kwargs["metadata"] if kwargs.get("metadata") else arg.metadata
+            )
             subassy.parent = self
 
             self.children.append(subassy)
             self.objects.update(subassy._flatten())
 
         else:
             assy = self.__class__(arg, **kwargs)
@@ -274,39 +292,37 @@
 
             rv = reduce(lambda l1, l2: l1 * l2, locs)
 
         return (rv, name_out)
 
     @overload
     def constrain(
-        self, q1: str, q2: str, kind: ConstraintKinds, param: Any = None
+        self, q1: str, q2: str, kind: ConstraintKind, param: Any = None
     ) -> "Assembly":
         ...
 
     @overload
-    def constrain(
-        self, q1: str, kind: ConstraintKinds, param: Any = None
-    ) -> "Assembly":
+    def constrain(self, q1: str, kind: ConstraintKind, param: Any = None) -> "Assembly":
         ...
 
     @overload
     def constrain(
         self,
         id1: str,
         s1: Shape,
         id2: str,
         s2: Shape,
-        kind: ConstraintKinds,
+        kind: ConstraintKind,
         param: Any = None,
     ) -> "Assembly":
         ...
 
     @overload
     def constrain(
-        self, id1: str, s1: Shape, kind: ConstraintKinds, param: Any = None,
+        self, id1: str, s1: Shape, kind: ConstraintKind, param: Any = None,
     ) -> "Assembly":
         ...
 
     def constrain(self, *args, param=None):
         """
         Define a new constraint.
         """
@@ -344,15 +360,15 @@
         else:
             raise ValueError(f"Unknown constraint: {kind}")
 
         self.constraints.append(c)
 
         return self
 
-    def solve(self) -> "Assembly":
+    def solve(self, verbosity: int = 0) -> "Assembly":
         """
         Solve the constraints.
         """
 
         # Get all entities and number them. First entity is marked as locked
         ents = {}
 
@@ -410,15 +426,15 @@
             raise ValueError("At least two entities need to be constrained")
 
         # instantiate the solver
         scale = self.toCompound().BoundingBox().DiagonalLength
         solver = ConstraintSolver(locs, constraints, locked=locked, scale=scale)
 
         # solve
-        locs_new, self._solve_result = solver.solve()
+        locs_new, self._solve_result = solver.solve(verbosity)
 
         # update positions
 
         # find the inverse root loc
         loc_root_inv = Location()
 
         if self.obj:
@@ -434,46 +450,53 @@
 
         return self
 
     def save(
         self,
         path: str,
         exportType: Optional[ExportLiterals] = None,
+        mode: STEPExportModeLiterals = "default",
         tolerance: float = 0.1,
         angularTolerance: float = 0.1,
         **kwargs,
     ) -> "Assembly":
         """
         Save assembly to a file.
 
         :param path: Path and filename for writing.
         :param exportType: export format (default: None, results in format being inferred form the path)
         :param tolerance: the deflection tolerance, in model units. Only used for GLTF, VRML. Default 0.1.
         :param angularTolerance: the angular tolerance, in radians. Only used for GLTF, VRML. Default 0.1.
-        :param **kwargs: Additional keyword arguments.  Only used for STEP.
+        :param \**kwargs: Additional keyword arguments.  Only used for STEP.
             See :meth:`~cadquery.occ_impl.exporters.assembly.exportAssembly`.
         """
 
+        # Make sure the export mode setting is correct
+        if mode not in get_args(STEPExportModeLiterals):
+            raise ValueError(f"Unknown assembly export mode {mode} for STEP")
+
         if exportType is None:
             t = path.split(".")[-1].upper()
-            if t in ("STEP", "XML", "VRML", "VTKJS", "GLTF"):
+            if t in ("STEP", "XML", "VRML", "VTKJS", "GLTF", "STL"):
                 exportType = cast(ExportLiterals, t)
             else:
                 raise ValueError("Unknown extension, specify export type explicitly")
 
         if exportType == "STEP":
-            exportAssembly(self, path, **kwargs)
+            exportAssembly(self, path, mode, **kwargs)
         elif exportType == "XML":
             exportCAF(self, path)
         elif exportType == "VRML":
             exportVRML(self, path, tolerance, angularTolerance)
         elif exportType == "GLTF":
             exportGLTF(self, path, True, tolerance, angularTolerance)
         elif exportType == "VTKJS":
             exportVTKJS(self, path)
+        elif exportType == "STL":
+            self.toCompound().exportStl(path, tolerance, angularTolerance)
         else:
             raise ValueError(f"Unknown format: {exportType}")
 
         return self
 
     @classmethod
     def load(cls, path: str) -> "Assembly":
```

### Comparing `cadquery-2.2.0b2/cadquery/contrib/__init__.py` & `cadquery-2.3.0/cadquery/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/cq.py` & `cadquery-2.3.0/cadquery/cq.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         s = Workplane("XY")
 
     After creation, the stack contains a single point, the origin of the underlying plane,
     and the *current point* is on the origin.
 
     .. note::
         You can also create workplanes on the surface of existing faces using
-        :py:meth:`CQ.workplane`
+        :meth:`workplane`
     """
 
     objects: List[CQObject]
     ctx: CQContext
     parent: Optional["Workplane"]
     plane: Plane
 
@@ -223,16 +223,15 @@
         self._tag = None
 
     def tag(self: T, name: str) -> T:
         """
         Tags the current CQ object for later reference.
 
         :param name: the name to tag this object with
-        :type name: string
-        :returns: self, a cq object with tag applied
+        :returns: self, a CQ object with tag applied
         """
         self._tag = name
         self.ctx.tags[name] = self
 
         return self
 
     def _collectProperty(self, propName: str) -> List[CQObject]:
@@ -275,22 +274,22 @@
     def split(self: T, splitter: Union[T, Shape]) -> T:
         ...
 
     def split(self: T, *args, **kwargs) -> T:
         """
         Splits a solid on the stack into two parts, optionally keeping the separate parts.
 
-        :param boolean keepTop: True to keep the top, False or None to discard it
-        :param boolean keepBottom: True to keep the bottom, False or None to discard it
+        :param bool keepTop: True to keep the top, False or None to discard it
+        :param bool keepBottom: True to keep the bottom, False or None to discard it
         :raises ValueError: if keepTop and keepBottom are both false.
         :raises ValueError: if there is no solid in the current stack or parent chain
         :returns: CQ object with the desired objects on the stack.
 
         The most common operation splits a solid and keeps one half. This sample creates
-        split bushing::
+        a split bushing::
 
             # drill a hole in the side
             c = Workplane().box(1,1,1).faces(">Z").workplane().circle(0.25).cutThruAll()
 
             # now cut it in half sideways
             c = c.faces(">Y").workplane(-0.5).split(keepTop=True)
         """
@@ -364,15 +363,15 @@
         !!!DEPRECATED!!! use union()
         Combines all solids on the current stack, and any context object, together
         into a single object.
 
         After the operation, the returned solid is also the context solid.
 
         :param otherCQToCombine: another CadQuery to combine.
-        :return: a cQ object with the resulting combined solid on the stack.
+        :return: a CQ object with the resulting combined solid on the stack.
 
         Most of the time, both objects will contain a single solid, which is
         combined and returned on the stack of the new object.
         """
         # loop through current stack objects, and combine them
         toCombine = cast(List[Solid], self.solids().vals())
 
@@ -419,15 +418,15 @@
     def vals(self) -> List[CQObject]:
         """
         get the values in the current list
 
         :rtype: list of occ_impl objects
         :returns: the values of the objects on the stack.
 
-        Contrast with :py:meth:`all`, which returns CQ objects for all of the items on the stack
+        Contrast with :meth:`all`, which returns CQ objects for all of the items on the stack
         """
         return self.objects
 
     @overload
     def add(self: T, obj: "Workplane") -> T:
         ...
 
@@ -443,15 +442,15 @@
         """
         Adds an object or a list of objects to the stack
 
         :param obj: an object to add
         :type obj: a Workplane, CAD primitive, or list of CAD primitives
         :return: a Workplane with the requested operation performed
 
-        If an Workplane object, the values of that object's stack are added. If
+        If a Workplane object, the values of that object's stack are added. If
         a list of cad primitives, they are all added. If a single CAD primitive
         then it is added.
 
         Used in rare cases when you need to combine the results of several CQ
         results into a single Workplane object.
         """
         if isinstance(obj, list):
@@ -498,16 +497,17 @@
             self.ctx.tags = {**obj.ctx.tags, **self.ctx.tags}
 
         return self
 
     def toOCC(self) -> Any:
         """
         Directly returns the wrapped OCCT object.
+
         :return: The wrapped OCCT object
-        :rtype TopoDS_Shape or a subclass
+        :rtype: TopoDS_Shape or a subclass
         """
 
         v = self.val()
 
         return v._faces if isinstance(v, Sketch) else v.wrapped
 
     def workplane(
@@ -522,18 +522,15 @@
         """
         Creates a new 2D workplane, located relative to the first face on the stack.
 
         :param offset:  offset for the workplane in its normal direction . Default
         :param invert:  invert the normal direction from that of the face.
         :param centerOption: how local origin of workplane is determined.
         :param origin: origin for plane center, requires 'ProjectedOrigin' centerOption.
-        :type offset: float or None=0.0
-        :type invert: boolean or None=False
         :type centerOption: string or None='ProjectedOrigin'
-        :type origin: Vector or None
         :rtype: Workplane object
 
         The first element on the stack must be a face, a set of
         co-planar faces or a vertex.  If a vertex, then the parent
         item on the chain immediately before the vertex must be a
         face.
 
@@ -575,16 +572,17 @@
 
             # test if p1 is on the plane of f0 (offset of planes)
             return abs(n0.dot(p0.sub(p1)) < self.ctx.tolerance)
 
         def _computeXdir(normal):
             """
             Figures out the X direction based on the given normal.
-            :param :normal The direction that's normal to the plane.
-            :type :normal A Vector
+
+            :param normal: The direction that's normal to the plane.
+            :type normal: A Vector
             :return A vector representing the X direction.
             """
             xd = Vector(0, 0, 1).cross(normal)
             if xd.Length < self.ctx.tolerance:
                 # this face is parallel with the x-y plane, so choose x to be in global coordinates
                 xd = Vector(1, 0, 0)
             return xd
@@ -687,47 +685,49 @@
         return out
 
     def workplaneFromTagged(self, name: str) -> "Workplane":
         """
         Copies the workplane from a tagged parent.
 
         :param name: tag to search for
-        :type name: string
         :returns: a CQ object with name's workplane
         """
         tagged = self._getTagged(name)
         out = self.copyWorkplane(tagged)
         return out
 
     def first(self: T) -> T:
         """
         Return the first item on the stack
+
         :returns: the first item on the stack.
         :rtype: a CQ object
         """
         return self.newObject(self.objects[0:1])
 
     def item(self: T, i: int) -> T:
         """
-
         Return the ith item on the stack.
+
         :rtype: a CQ object
         """
         return self.newObject([self.objects[i]])
 
     def last(self: T) -> T:
         """
         Return the last item on the stack.
+
         :rtype: a CQ object
         """
         return self.newObject([self.objects[-1]])
 
     def end(self, n: int = 1) -> "Workplane":
         """
         Return the nth parent of this CQ element
+
         :param n: number of ancestor to return (default: 1)
         :rtype: a CQ object
         :raises: ValueError if there are no more parents in the chain.
 
         For example::
 
             CQ(obj).faces("+Z").vertices().end()
@@ -819,15 +819,14 @@
     ) -> T:
         """
         Filters objects of the selected type with the specified selector,and returns results
 
         :param objType: the type of object we are searching for
         :type objType: string: (Vertex|Edge|Wire|Solid|Shell|Compound|CompSolid)
         :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
         :return: a CQ object with the selected objects on the stack.
 
         **Implementation Note**: This is the base implementation of the vertices,edges,faces,
         solids,shells, and other similar selector methods.  It is a useful extension point for
         plugin developers to make other selector methods.
         """
         self_as_workplane: Workplane = self
@@ -851,72 +850,68 @@
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the vertices of objects on the stack, optionally filtering the selection. If there
         are multiple objects on the stack, the vertices of all objects are collected and a list of
         all the distinct vertices is returned.
 
-        :param selector:
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
         :return: a CQ object who's stack contains  the *distinct* vertices of *all* objects on the
-           current stack, after being filtered by the selector, if provided
+            current stack, after being filtered by the selector, if provided
 
         If there are no vertices for any objects on the current stack, an empty CQ object
         is returned
 
         The typical use is to select the vertices of a single object on the stack. For example::
 
-           Workplane().box(1,1,1).faces("+Z").vertices().size()
+            Workplane().box(1, 1, 1).faces("+Z").vertices().size()
 
-        returns 4, because the topmost face of cube will contain four vertices. While this::
+        returns 4, because the topmost face of a cube will contain four vertices. While this::
 
-           Workplane().box(1,1,1).faces().vertices().size()
+            Workplane().box(1, 1, 1).faces().vertices().size()
 
         returns 8, because a cube has a total of 8 vertices
 
         **Note** Circles are peculiar, they have a single vertex at the center!
 
-        :py:class:`StringSyntaxSelector`
-
         """
         return self._selectObjects("Vertices", selector, tag)
 
     def faces(
         self: T,
         selector: Optional[Union[Selector, str]] = None,
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the faces of objects on the stack, optionally filtering the selection. If there are
         multiple objects on the stack, the faces of all objects are collected and a list of all the
         distinct faces is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
         :return: a CQ object who's stack contains all of the *distinct* faces of *all* objects on
             the current stack, filtered by the provided selector.
 
-        If there are no vertices for any objects on the current stack, an empty CQ object
+        If there are no faces for any objects on the current stack, an empty CQ object
         is returned.
 
         The typical use is to select the faces of a single object on the stack. For example::
 
-           CQ(aCube).faces("+Z").size()
+            Workplane().box(1, 1, 1).faces("+Z").size()
 
         returns 1, because a cube has one face with a normal in the +Z direction. Similarly::
 
-           CQ(aCube).faces().size()
+            Workplane().box(1, 1, 1).faces().size()
 
         returns 6, because a cube has a total of 6 faces, And::
 
-            CQ(aCube).faces("|Z").size()
+            Workplane().box(1, 1, 1).faces("|Z").size()
 
         returns 2, because a cube has 2 faces having normals parallel to the z direction
         """
         return self._selectObjects("Faces", selector, tag)
 
     def edges(
         self: T,
@@ -924,34 +919,33 @@
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the edges of objects on the stack, optionally filtering the selection. If there are
         multiple objects on the stack, the edges of all objects are collected and a list of all the
         distinct edges is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
         :return: a CQ object who's stack contains all of the *distinct* edges of *all* objects on
             the current stack, filtered by the provided selector.
 
         If there are no edges for any objects on the current stack, an empty CQ object is returned
 
         The typical use is to select the edges of a single object on the stack. For example::
 
-           CQ(aCube).faces("+Z").edges().size()
+            Workplane().box(1, 1, 1).faces("+Z").edges().size()
 
-        returns 4, because a cube has one face with a normal in the +Z direction. Similarly::
+        returns 4, because the topmost face of a cube will contain four edges. Similarly::
 
-           CQ(aCube).edges().size()
+            Workplane().box(1, 1, 1).edges().size()
 
         returns 12, because a cube has a total of 12 edges, And::
 
-            CQ(aCube).edges("|Z").size()
+            Workplane().box(1, 1, 1).edges("|Z").size()
 
         returns 4, because a cube has 4 edges parallel to the z direction
         """
         return self._selectObjects("Edges", selector, tag)
 
     def wires(
         self: T,
@@ -959,26 +953,25 @@
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the wires of objects on the stack, optionally filtering the selection. If there are
         multiple objects on the stack, the wires of all objects are collected and a list of all the
         distinct wires is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
         :return: a CQ object who's stack contains all of the *distinct* wires of *all* objects on
             the current stack, filtered by the provided selector.
 
         If there are no wires for any objects on the current stack, an empty CQ object is returned
 
         The typical use is to select the wires of a single object on the stack. For example::
 
-           CQ(aCube).faces("+Z").wires().size()
+            Workplane().box(1, 1, 1).faces("+Z").wires().size()
 
         returns 1, because a face typically only has one outer wire
         """
         return self._selectObjects("Wires", selector, tag)
 
     def solids(
         self: T,
@@ -986,49 +979,47 @@
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the solids of objects on the stack, optionally filtering the selection. If there are
         multiple objects on the stack, the solids of all objects are collected and a list of all the
         distinct solids is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
         :return: a CQ object who's stack contains all of the *distinct* solids of *all* objects on
             the current stack, filtered by the provided selector.
 
         If there are no solids for any objects on the current stack, an empty CQ object is returned
 
-        The typical use is to select the  a single object on the stack. For example::
+        The typical use is to select a single object on the stack. For example::
 
-           CQ(aCube).solids().size()
+            Workplane().box(1, 1, 1).solids().size()
 
         returns 1, because a cube consists of one solid.
 
-        It is possible for single CQ object ( or even a single CAD primitive ) to contain
+        It is possible for a single CQ object ( or even a single CAD primitive ) to contain
         multiple solids.
         """
         return self._selectObjects("Solids", selector, tag)
 
     def shells(
         self: T,
         selector: Optional[Union[Selector, str]] = None,
         tag: Optional[str] = None,
     ) -> T:
         """
         Select the shells of objects on the stack, optionally filtering the selection. If there are
         multiple objects on the stack, the shells of all objects are collected and a list of all the
         distinct shells is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
-        :return: a CQ object who's stack contains all of the *distinct* solids of *all* objects on
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
+        :return: a CQ object who's stack contains all of the *distinct* shells of *all* objects on
             the current stack, filtered by the provided selector.
 
         If there are no shells for any objects on the current stack, an empty CQ object is returned
 
         Most solids will have a single shell, which represents the outer surface. A shell will
         typically be composed of multiple faces.
         """
@@ -1040,19 +1031,18 @@
         tag: Optional[str] = None,
     ) -> T:
         """
         Select compounds on the stack, optionally filtering the selection. If there are multiple
         objects on the stack, they are collected and a list of all the distinct compounds
         is returned.
 
-        :param selector: A selector
-        :type selector:  None, a Selector object, or a string selector expression.
-        :param tag: if set, search the tagged CQ object instead of self
-        :type tag: string
-        :return: a CQ object who's stack contains all of the *distinct* solids of *all* objects on
+        :param selector: optional Selector object, or string selector expression
+            (see :class:`StringSyntaxSelector`)
+        :param tag: if set, search the tagged object instead of self
+        :return: a CQ object who's stack contains all of the *distinct* compounds of *all* objects on
             the current stack, filtered by the provided selector.
 
         A compound contains multiple CAD primitives that resulted from a single operation, such as
         a union, cut, split, or fillet.  Compounds can contain multiple edges, wires, or solids.
         """
         return self._selectObjects("Compounds", selector, tag)
 
@@ -1070,33 +1060,31 @@
 
     def exportSvg(self, fileName: str) -> None:
         """
         Exports the first item on the stack as an SVG file
 
         For testing purposes mainly.
 
-        :param fileName: the filename to export
-        :type fileName: String, absolute path to the file
+        :param fileName: the filename to export, absolute path to the file
         """
         exportSVG(self, fileName)
 
     def rotateAboutCenter(self: T, axisEndPoint: VectorLike, angleDegrees: float) -> T:
         """
         Rotates all items on the stack by the specified angle, about the specified axis
 
         The center of rotation is a vector starting at the center of the object on the stack,
         and ended at the specified point.
 
         :param axisEndPoint: the second point of axis of rotation
         :type axisEndPoint: a three-tuple in global coordinates
         :param angleDegrees: the rotation angle, in degrees
-        :type angleDegrees: float
         :returns: a CQ object, with all items rotated.
 
-        WARNING: This version returns the same cq object instead of a new one-- the
+        WARNING: This version returns the same CQ object instead of a new one-- the
         old object is not accessible.
 
         Future Enhancements:
             * A version of this method that returns a transformed copy, rather than modifying
               the originals
             * This method doesn't expose a very good interface, because the axis of rotation
               could be inconsistent between multiple objects.  This is because the beginning
@@ -1125,15 +1113,14 @@
         of rotation.
 
         :param axisStartPoint: The first point of the axis of rotation
         :type axisStartPoint: a 3-tuple of floats
         :param axisEndPoint: The second point of the axis of rotation
         :type axisEndPoint: a 3-tuple of floats
         :param angleDegrees: the rotation angle, in degrees
-        :type angleDegrees: float
         :returns: a CQ object
         """
         return self.newObject(
             [
                 o.rotate(Vector(axisStartPoint), Vector(axisEndPoint), angleDegrees)
                 if isinstance(o, Shape)
                 else o
@@ -1150,19 +1137,17 @@
         union: bool = False,
     ) -> T:
         """
         Mirror a single CQ object.
 
         :param mirrorPlane: the plane to mirror about
         :type mirrorPlane: string, one of "XY", "YX", "XZ", "ZX", "YZ", "ZY" the planes
-        or the normal vector of the plane eg (1,0,0) or a Face object
+            or the normal vector of the plane eg (1,0,0) or a Face object
         :param basePointVector: the base point to mirror about (this is overwritten if a Face is passed)
-        :type basePointVector: tuple
         :param union: If true will perform a union operation on the mirrored object
-        :type union: bool
         """
 
         mp: Union[Literal["XY", "YX", "XZ", "ZX", "YZ", "ZY"], Vector]
         bp: Vector
         face: Optional[Face] = None
 
         # handle mirrorPLane
@@ -1253,18 +1238,17 @@
         """
         Fillets a solid on the selected edges.
 
         The edges on the stack are filleted. The solid to which the edges belong must be in the
         parent chain of the selected edges.
 
         :param radius: the radius of the fillet, must be > zero
-        :type radius: positive float
         :raises ValueError: if at least one edge is not selected
         :raises ValueError: if the solid containing the edge is not in the chain
-        :returns: cq object with the resulting solid selected.
+        :returns: CQ object with the resulting solid selected.
 
         This example will create a unit cube, with the top edges filleted::
 
             s = Workplane().box(1,1,1).faces("+Z").edges().fillet(0.1)
         """
         # TODO: ensure that edges selected actually belong to the solid in the chain, otherwise,
         # TODO: we segfault
@@ -1288,19 +1272,17 @@
 
         Optional parameter `length2` can be supplied with a different
         value than `length` for a chamfer that is shorter on one side
         longer on the other side.
 
         :param length: the length of the chamfer, must be greater than zero
         :param length2: optional parameter for asymmetrical chamfer
-        :type length: positive float
-        :type length2: positive float
         :raises ValueError: if at least one edge is not selected
         :raises ValueError: if the solid containing the edge is not in the chain
-        :returns: cq object with the resulting solid selected.
+        :returns: CQ object with the resulting solid selected.
 
         This example will create a unit cube, with the top edges chamfered::
 
             s = Workplane("XY").box(1,1,1).faces("+Z").chamfer(0.1)
 
         This example will create chamfers longer on the sides::
 
@@ -1321,14 +1303,15 @@
     ) -> T:
         """
         Create a new workplane based on the current one.
         The origin of the new plane is located at the existing origin+offset vector, where offset is
         given in coordinates local to the current plane
         The new plane is rotated through the angles specified by the components of the rotation
         vector.
+
         :param rotate: 3-tuple of angles to rotate, in degrees relative to work plane coordinates
         :param offset: 3-tuple to offset the new plane, in local work plane coordinates
         :return: a new work plane, transformed as requested
         """
 
         # old api accepted a vector, so we'll check for that.
         if isinstance(rotate, Vector):
@@ -1379,15 +1362,14 @@
 
         The algorithm is this:
             * If an Edge is on the stack, its end point is used.yp
             * if a vector is on the stack, it is used
 
         WARNING: only the last object on the stack is used.
 
-        NOTE:
         """
         obj = self.objects[-1] if self.objects else self.plane.origin
 
         if isinstance(obj, Edge):
             p = obj.endPoint()
         elif isinstance(obj, Vector):
             p = obj
@@ -1534,15 +1516,15 @@
         based on three points::
 
             s = Workplane().box(1,1,1).faces(">Z").workplane().\
                 pushPoints([(-0.3,0.3),(0.3,0.3),(0,0)])
             body = s.circle(0.05).cutThruAll()
 
         Here the circle function operates on all three points, and is then extruded to create three
-        holes. See :py:meth:`circle` for how it works.
+        holes. See :meth:`circle` for how it works.
         """
         vecs: List[Union[Location, Vector]] = []
         for pnt in pntList:
             vecs.append(
                 pnt if isinstance(pnt, Location) else self.plane.toWorldCoords(pnt)
             )
 
@@ -1550,17 +1532,17 @@
 
     def center(self: T, x: float, y: float) -> T:
         """
         Shift local coordinates to the specified location.
 
         The location is specified in terms of local coordinates.
 
-        :param float x: the new x location
-        :param float y: the new y location
-        :returns: the workplane object, with the center adjusted.
+        :param x: the new x location
+        :param y: the new y location
+        :returns: the Workplane object, with the center adjusted.
 
         The current point is set to the new center.
         This method is useful to adjust the center point after it has been created automatically on
         a face, but not where you'd like it to be.
 
         In this example, we adjust the workplane center to be at the corner of a cube, instead of
         the center of a face, which is the default::
@@ -1570,29 +1552,28 @@
 
             s = s.center(-0.5,-0.5) # move the center to the corner
             t = s.circle(0.25).extrude(0.2)
             assert ( t.faces().size() == 9 ) # a cube with a cylindrical nub at the top right corner
 
         The result is a cube with a round boss on the corner
         """
-        "Shift local coordinates to the specified location, according to current coordinates"
         new_origin = self.plane.toWorldCoords((x, y))
         n = self.newObject([new_origin])
         n.plane.setOrigin2d(x, y)
         return n
 
     def lineTo(self: T, x: float, y: float, forConstruction: bool = False) -> T:
         """
         Make a line from the current point to the provided point
 
-        :param float x: the x point, in workplane plane coordinates
-        :param float y: the y point, in workplane plane coordinates
+        :param x: the x point, in workplane plane coordinates
+        :param y: the y point, in workplane plane coordinates
         :return: the Workplane object with the current point at the end of the new line
 
-        see :py:meth:`line` if you want to use relative dimensions to make a line instead.
+        See :meth:`line` if you want to use relative dimensions to make a line instead.
         """
         startPoint = self._findFromPoint(False)
 
         endPoint = self.plane.toWorldCoords((x, y))
 
         p = Edge.makeLine(startPoint, endPoint)
 
@@ -1603,75 +1584,75 @@
 
     # line a specified incremental amount from current point
     def line(self: T, xDist: float, yDist: float, forConstruction: bool = False) -> T:
         """
         Make a line from the current point to the provided point, using
         dimensions relative to the current point
 
-        :param float xDist: x distance from current point
-        :param float yDist: y distance from current point
+        :param xDist: x distance from current point
+        :param yDist: y distance from current point
         :return: the workplane object with the current point at the end of the new line
 
-        see :py:meth:`lineTo` if you want to use absolute coordinates to make a line instead.
+        see :meth:`lineTo` if you want to use absolute coordinates to make a line instead.
         """
         p = self._findFromPoint(True)  # return local coordinates
         return self.lineTo(p.x + xDist, yDist + p.y, forConstruction)
 
     def vLine(self: T, distance: float, forConstruction: bool = False) -> T:
         """
         Make a vertical line from the current point the provided distance
 
-        :param float distance: (y) distance from current point
-        :return: the workplane object with the current point at the end of the new line
+        :param distance: (y) distance from current point
+        :return: the Workplane object with the current point at the end of the new line
         """
         return self.line(0, distance, forConstruction)
 
     def hLine(self: T, distance: float, forConstruction: bool = False) -> T:
         """
         Make a horizontal line from the current point the provided distance
 
-        :param float distance: (x) distance from current point
+        :param distance: (x) distance from current point
         :return: the Workplane object with the current point at the end of the new line
         """
         return self.line(distance, 0, forConstruction)
 
     def vLineTo(self: T, yCoord: float, forConstruction: bool = False) -> T:
         """
         Make a vertical line from the current point to the provided y coordinate.
 
         Useful if it is more convenient to specify the end location rather than distance,
-        as in :py:meth:`vLine`
+        as in :meth:`vLine`
 
-        :param float yCoord: y coordinate for the end of the line
+        :param yCoord: y coordinate for the end of the line
         :return: the Workplane object with the current point at the end of the new line
         """
         p = self._findFromPoint(True)
         return self.lineTo(p.x, yCoord, forConstruction)
 
     def hLineTo(self: T, xCoord: float, forConstruction: bool = False) -> T:
         """
         Make a horizontal line from the current point to the provided x coordinate.
 
         Useful if it is more convenient to specify the end location rather than distance,
-        as in :py:meth:`hLine`
+        as in :meth:`hLine`
 
-        :param float xCoord: x coordinate for the end of the line
+        :param xCoord: x coordinate for the end of the line
         :return: the Workplane object with the current point at the end of the new line
         """
         p = self._findFromPoint(True)
         return self.lineTo(xCoord, p.y, forConstruction)
 
     def polarLine(
         self: T, distance: float, angle: float, forConstruction: bool = False
     ) -> T:
         """
         Make a line of the given length, at the given angle from the current point
 
-        :param float distance: distance of the end of the line from the current point
-        :param float angle: angle of the vector to the end of the line with the x-axis
+        :param distance: distance of the end of the line from the current point
+        :param angle: angle of the vector to the end of the line with the x-axis
         :return: the Workplane object with the current point at the end of the new line
         """
         x = math.cos(math.radians(angle)) * distance
         y = math.sin(math.radians(angle)) * distance
 
         return self.line(x, y, forConstruction)
 
@@ -1680,16 +1661,16 @@
     ) -> T:
         """
         Make a line from the current point to the given polar coordinates
 
         Useful if it is more convenient to specify the end location rather than
         the distance and angle from the current point
 
-        :param float distance: distance of the end of the line from the origin
-        :param float angle: angle of the vector to the end of the line with the x-axis
+        :param distance: distance of the end of the line from the origin
+        :param angle: angle of the vector to the end of the line with the x-axis
         :return: the Workplane object with the current point at the end of the new line
         """
         x = math.cos(math.radians(angle)) * distance
         y = math.sin(math.radians(angle)) * distance
 
         return self.lineTo(x, y, forConstruction)
 
@@ -1699,55 +1680,55 @@
         Move to the specified point, without drawing.
 
         :param x: desired x location, in local coordinates
         :type x: float, or none for zero
         :param y: desired y location, in local coordinates
         :type y: float, or none for zero.
 
-        Not to be confused with :py:meth:`center`, which moves the center of the entire
+        Not to be confused with :meth:`center`, which moves the center of the entire
         workplane, this method only moves the current point ( and therefore does not affect objects
         already drawn ).
 
-        See :py:meth:`move` to do the same thing but using relative dimensions
+        See :meth:`move` to do the same thing but using relative dimensions
         """
         newCenter = Vector(x, y, 0)
         return self.newObject([self.plane.toWorldCoords(newCenter)])
 
     # relative move in current plane, not drawing
     def move(self: T, xDist: float = 0, yDist: float = 0) -> T:
         """
         Move the specified distance from the current point, without drawing.
 
         :param xDist: desired x distance, in local coordinates
         :type xDist: float, or none for zero
         :param yDist: desired y distance, in local coordinates
         :type yDist: float, or none for zero.
 
-        Not to be confused with :py:meth:`center`, which moves the center of the entire
+        Not to be confused with :meth:`center`, which moves the center of the entire
         workplane, this method only moves the current point ( and therefore does not affect objects
         already drawn ).
 
-        See :py:meth:`moveTo` to do the same thing but using absolute coordinates
+        See :meth:`moveTo` to do the same thing but using absolute coordinates
         """
         p = self._findFromPoint(True)
         newCenter = p + Vector(xDist, yDist, 0)
         return self.newObject([self.plane.toWorldCoords(newCenter)])
 
     def slot2D(self: T, length: float, diameter: float, angle: float = 0) -> T:
         """
         Creates a rounded slot for each point on the stack.
 
         :param diameter: desired diameter, or width, of slot
         :param length: desired end to end length of slot
         :param angle: angle of slot in degrees, with 0 being along x-axis
         :return: a new CQ object with the created wires on the stack
 
-        Can be used to create arrays of slots, such as in cooling applications:
+        Can be used to create arrays of slots, such as in cooling applications::
 
-        result = cq.Workplane("XY").box(10,25,1).rarray(1,2,1,10).slot2D(8,1,0).cutThruAll()
+            Workplane().box(10, 25, 1).rarray(1, 2, 1, 10).slot2D(8, 1, 0).cutThruAll()
         """
 
         radius = diameter / 2
 
         p1 = Vector((-length / 2) + radius, diameter / 2)
         p2 = p1 + Vector(length - diameter, 0)
         p3 = p1 + Vector(length - diameter, -diameter)
@@ -1830,16 +1811,16 @@
             interpolation may fail.)
 
             Set to None to use the default tolerance.
         :param includeCurrent: use current point as a starting point of the curve
         :param makeWire: convert the resulting spline edge to a wire
         :return: a Workplane object with the current point at the end of the spline
 
-        The spline will begin at the current point, and
-        end with the last point in the XY tuple list
+        The spline will begin at the current point, and end with the last point in the
+        XY tuple list.
 
         This example creates a block with a spline for one side::
 
             s = Workplane(Plane.XY())
             sPnts = [
                 (2.75,1.5),
                 (2.5,1.75),
@@ -2121,15 +2102,15 @@
         :param sag: the sagitta of the arc
         :type sag: float, perpendicular distance from arc center to arc baseline.
         :return: a workplane with the current point at the end of the arc
 
         The sagitta is the distance from the center of the arc to the arc base.
         Given that a closed contour is drawn clockwise;
         A positive sagitta means convex arc and negative sagitta means concave arc.
-        See "https://en.wikipedia.org/wiki/Sagitta_(geometry)" for more information.
+        See `<https://en.wikipedia.org/wiki/Sagitta_(geometry)>`_ for more information.
         """
 
         startPoint = self._findFromPoint(useLocalCoords=True)
         endPoint = Vector(endPoint)
         midPoint = endPoint.add(startPoint).multiply(0.5)
 
         sagVector = endPoint.sub(startPoint).normalized().multiply(abs(sag))
@@ -2188,15 +2169,14 @@
     ) -> T:
         """
         Draw an arc as a tangent from the end of the current edge to endpoint.
 
         :param endpoint: point for the arc to end at
         :type endpoint: 2-tuple, 3-tuple or Vector
         :param relative: True if endpoint is specified relative to the current point, False if endpoint is in workplane coordinates
-        :type relative: Bool
         :return: a Workplane object with an arc on the stack
 
         Requires the the current first object on the stack is an Edge, as would
         be the case after a lineTo operation or similar.
         """
 
         if not isinstance(endpoint, Vector):
@@ -2272,16 +2252,14 @@
         # attempt again to consolidate all of the wires
         return consolidated.consolidateWires()
 
     def _addPendingEdge(self, edge: Edge) -> None:
         """
         Queues an edge for later combination into a wire.
 
-        :param edge:
-        :return:
         """
         self.ctx.pendingEdges.append(edge)
 
         if self.ctx.firstPoint is None:
             self.ctx.firstPoint = self.plane.toLocalCoords(edge.startPoint())
 
     def _addPendingWire(self, wire: Wire) -> None:
@@ -2292,15 +2270,15 @@
 
         but users do not normally care about these distinctions.  Users 'think' in terms
         of edges, and solids.
 
         CadQuery tracks edges as they are drawn, and automatically combines them into wires
         when the user does an operation that needs it.
 
-        Similarly, cadQuery tracks pending wires, and automatically combines them into faces
+        Similarly, CadQuery tracks pending wires, and automatically combines them into faces
         when necessary to make a solid.
         """
         self.ctx.pendingWires.append(wire)
 
     def _consolidateWires(self) -> List[Wire]:
 
         # note: do not use CQContext.popPendingEdges or Wires here, this method does not
@@ -2382,17 +2360,18 @@
         Runs the provided function on each value in the stack, and collects the return values into
         a new CQ object.
 
         Special note: a newly created workplane always has its center point as its only stack item
 
         :param callBackFunction: the function to call for each item on the current stack.
         :param useLocalCoordinates: should  values be converted from local coordinates first?
-        :type useLocalCoordinates: boolean
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
 
         The callback function must accept one argument, which is the item on the stack, and return
         one object, which is collected. If the function returns None, nothing is added to the stack.
         The object passed into the callBackFunction is potentially transformed to local coordinates,
         if useLocalCoordinates is true
 
@@ -2439,17 +2418,18 @@
         """
         Same as each(), except each item on the stack is converted into a point before it
         is passed into the callback function.
 
         :return: CadQuery object which contains a list of  vectors (points ) on its stack.
 
         :param useLocalCoordinates: should points be in local or global coordinates
-        :type useLocalCoordinates: boolean
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
 
         The resulting object has a point on the stack for each object on the original stack.
         Vertices and points remain a point.  Faces, Wires, Solids, Edges, and Shells are converted
         to a point by using their center of mass.
 
         If the stack has zero length, a single point is returned, which is the center of the current
@@ -2546,15 +2526,14 @@
 
     # circle from current point
     def circle(self: T, radius: float, forConstruction: bool = False) -> T:
         """
         Make a circle for each item on the stack.
 
         :param radius: radius of the circle
-        :type radius: float > 0
         :param forConstruction: should the new wires be reference geometry only?
         :type forConstruction: true if the wires are for reference, false if they are creating
             part geometry
         :return: a new CQ object with the created wires on the stack
 
         A common use case is to use a for-construction rectangle to define the centers of a
         hole pattern::
@@ -2588,27 +2567,26 @@
         rotation_angle: float = 0.0,
         forConstruction: bool = False,
     ) -> T:
         """
         Make an ellipse for each item on the stack.
 
         :param x_radius: x radius of the ellipse (x-axis of plane the ellipse should lie in)
-        :type x_radius: float > 0
         :param y_radius: y radius of the ellipse (y-axis of plane the ellipse should lie in)
-        :type y_radius: float > 0
-        :param rotation_angle: angle to rotate the ellipse (0 = no rotation = default)
-        :type rotation_angle: float
+        :param rotation_angle: angle to rotate the ellipse
         :param forConstruction: should the new wires be reference geometry only?
         :type forConstruction: true if the wires are for reference, false if they are creating
             part geometry
         :return: a new CQ object with the created wires on the stack
 
         *NOTE* Due to a bug in opencascade (https://tracker.dev.opencascade.org/view.php?id=31290)
         the center of mass (equals center for next shape) is shifted. To create concentric ellipses
-        use Workplane("XY")
+        use::
+
+            Workplane("XY")
             .center(10, 20).ellipse(100,10)
             .center(0, 0).ellipse(50, 5)
         """
 
         e = Wire.makeEllipse(
             x_radius,
             y_radius,
@@ -2669,16 +2647,15 @@
         listOfXYTuple: Sequence[VectorLike],
         forConstruction: bool = False,
         includeCurrent: bool = False,
     ) -> T:
         """
         Create a polyline from a list of points
 
-        :param listOfXYTuple: a list of points in Workplane coordinates
-        :type listOfXYTuple: list of 2-tuples
+        :param listOfXYTuple: a list of points in Workplane coordinates (2D or 3D)
         :param forConstruction: whether or not the edges are used for reference
         :type forConstruction: true if the edges are for reference, false if they are for creating geometry
             part geometry
         :param includeCurrent: use current point as a starting point of the polyline
         :return: a new CQ object with a list of edges on the stack
 
         *NOTE* most commonly, the resulting wire should be closed.
@@ -2706,23 +2683,23 @@
             if not forConstruction:
                 self._addPendingEdge(edges[-1])
 
         return self.newObject(edges)
 
     def close(self: T) -> T:
         """
-        End 2D construction, and attempt to build a closed wire.
+        End construction, and attempt to build a closed wire.
 
         :return: a CQ object with a completed wire on the stack, if possible.
 
-        After 2D drafting with methods such as lineTo, threePointArc,
+        After 2D (or 3D) drafting with methods such as lineTo, threePointArc,
         tangentArcPoint and polyline, it is necessary to convert the edges
         produced by these into one or more wires.
 
-        When a set of edges is closed, cadQuery assumes it is safe to build
+        When a set of edges is closed, CadQuery assumes it is safe to build
         the group of edges into a wire. This example builds a simple triangular
         prism::
 
             s = Workplane().lineTo(1,0).lineTo(1,1).close().extrude(0.2)
         """
         endPoint = self._findFromPoint(True)
 
@@ -2731,15 +2708,15 @@
         else:
             startPoint = self.ctx.firstPoint
 
         # Check if there is a distance between startPoint and endPoint
         # that is larger than what is considered a numerical error.
         # If so; add a line segment between endPoint and startPoint
         if endPoint.sub(startPoint).Length > 1e-6:
-            self.lineTo(self.ctx.firstPoint.x, self.ctx.firstPoint.y)
+            self.polyline([endPoint, startPoint])
 
         # Need to reset the first point after closing a wire
         self.ctx.firstPoint = None
 
         return self.wire()
 
     def largestDimension(self) -> float:
@@ -2762,17 +2739,18 @@
         fcn: Callable[[Location], Shape],
         useLocalCoords: bool = False,
         clean: bool = True,
     ) -> T:
         """
         Evaluates the provided function at each point on the stack (ie, eachpoint)
         and then cuts the result from the context solid.
+
         :param fcn: a function suitable for use in the eachpoint method: ie, that accepts a vector
-        :param useLocalCoords: same as for :py:meth:`eachpoint`
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param useLocalCoords: same as for :meth:`eachpoint`
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :raises ValueError: if no solids or compounds are found in the stack or parent chain
         :return: a CQ object that contains the resulting solid
         """
         ctxSolid = self.findSolid()
 
         # will contain all of the counterbores as a single compound
         results = cast(List[Shape], self.eachpoint(fcn, useLocalCoords).vals())
@@ -2794,22 +2772,20 @@
         depth: Optional[float] = None,
         clean: bool = True,
     ) -> T:
         """
         Makes a counterbored hole for each item on the stack.
 
         :param diameter: the diameter of the hole
-        :type diameter: float > 0
-        :param cboreDiameter: the diameter of the cbore
-        :type cboreDiameter: float > 0 and > diameter
+        :param cboreDiameter: the diameter of the cbore, must be greater than hole diameter
         :param cboreDepth: depth of the counterbore
         :type cboreDepth: float > 0
         :param depth: the depth of the hole
-        :type depth: float > 0 or None to drill thru the entire part.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :type depth: float > 0 or None to drill thru the entire part
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
         The surface of the hole is at the current workplane plane.
 
         One hole is created for each item on the stack.  A very common use case is to use a
         construction rectangle to define the centers of a set of holes, like so::
 
             s = (
@@ -2823,15 +2799,15 @@
             )
 
         This sample creates a plate with a set of holes at the corners.
 
         **Plugin Note**: this is one example of the power of plugins. Counterbored holes are quite
         time consuming to create, but are quite easily defined by users.
 
-        see :py:meth:`cskHole` to make countersinks instead of counterbores
+        see :meth:`cskHole` to make countersinks instead of counterbores
         """
         if depth is None:
             depth = self.largestDimension()
 
         boreDir = Vector(0, 0, -1)
         center = Vector()
         # first make the hole
@@ -2856,21 +2832,20 @@
         clean: bool = True,
     ) -> T:
         """
         Makes a countersunk hole for each item on the stack.
 
         :param diameter: the diameter of the hole
         :type diameter: float > 0
-        :param cskDiameter: the diameter of the countersink
-        :type cskDiameter: float > 0 and > diameter
+        :param cskDiameter: the diameter of the countersink, must be greater than hole diameter
         :param cskAngle: angle of the countersink, in degrees ( 82 is common )
         :type cskAngle: float > 0
         :param depth: the depth of the hole
         :type depth: float > 0 or None to drill thru the entire part.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
         The surface of the hole is at the current workplane.
 
         One hole is created for each item on the stack.  A very common use case is to use a
         construction rectangle to define the centers of a set of holes, like so::
 
             s = (
@@ -2884,15 +2859,15 @@
             )
 
         This sample creates a plate with a set of holes at the corners.
 
         **Plugin Note**: this is one example of the power of plugins. CounterSunk holes are quite
         time consuming to create, but are quite easily defined by users.
 
-        see :py:meth:`cboreHole` to make counterbores instead of countersinks
+        see :meth:`cboreHole` to make counterbores instead of countersinks
         """
 
         if depth is None:
             depth = self.largestDimension()
 
         boreDir = Vector(0, 0, -1)
         center = Vector()
@@ -2913,18 +2888,17 @@
     def hole(
         self: T, diameter: float, depth: Optional[float] = None, clean: bool = True,
     ) -> T:
         """
         Makes a hole for each item on the stack.
 
         :param diameter: the diameter of the hole
-        :type diameter: float > 0
         :param depth: the depth of the hole
         :type depth: float > 0 or None to drill thru the entire part.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
         The surface of the hole is at the current workplane.
 
         One hole is created for each item on the stack.  A very common use case is to use a
         construction rectangle to define the centers of a set of holes, like so::
 
             s = (
@@ -2938,15 +2912,15 @@
             )
 
         This sample creates a plate with a set of holes at the corners.
 
         **Plugin Note**: this is one example of the power of plugins. CounterSunk holes are quite
         time consuming to create, but are quite easily defined by users.
 
-        see :py:meth:`cboreHole` and :py:meth:`cskHole` to make counterbores or countersinks
+        see :meth:`cboreHole` and :meth:`cskHole` to make counterbores or countersinks
         """
         if depth is None:
             depth = self.largestDimension()
 
         boreDir = Vector(0, 0, -1)
         # first make the hole
         h = Solid.makeCylinder(
@@ -2973,16 +2947,18 @@
         of the angle. In fact, if angle=0, the result is the same as a linear extrude.
 
         **NOTE**  This method can create complex calculations, so be careful using it with
         complex geometries
 
         :param distance: the distance to extrude normal to the workplane
         :param angle: angle (in degrees) to rotate through the extrusion
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :return: a CQ object with the resulting solid selected.
         """
         faces = self._getFaces()
 
         # compute extrusion vector and extrude
         eDir = self.plane.zDir.multiply(distance)
 
@@ -3012,36 +2988,38 @@
         both: bool = False,
         taper: Optional[float] = None,
     ) -> T:
         """
         Use all un-extruded wires in the parent chain to create a prismatic solid.
 
         :param until: The distance to extrude, normal to the workplane plane. When a float is
-          passed, the extrusion extends this far and a negative value is in the opposite direction
-          to the normal of the plane. The string "next" extrudes until the next face orthogonal to
-          the wire normal. "last" extrudes to the last face. If a object of type Face is passed then
-          the extrusion will extend until this face. **Note that the Workplane must contain a Solid for extruding to a given face.**
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
-        :param boolean both: extrude in both directions symmetrically
-        :param float taper: angle for optional tapered extrusion
+            passed, the extrusion extends this far and a negative value is in the opposite direction
+            to the normal of the plane. The string "next" extrudes until the next face orthogonal to
+            the wire normal. "last" extrudes to the last face. If a object of type Face is passed then
+            the extrusion will extend until this face. **Note that the Workplane must contain a Solid for extruding to a given face.**
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param both: extrude in both directions symmetrically
+        :param taper: angle for optional tapered extrusion
         :return: a CQ object with the resulting solid selected.
 
         The returned object is always a CQ object, and depends on whether combine is True, and
         whether a context solid is already defined:
 
         *  if combine is False, the new value is pushed onto the stack. Note that when extruding
-          until a specified face, combine can not be False
+            until a specified face, combine can not be False
         *  if combine is true, the value is combined with the context solid if it exists,
-           and the resulting solid becomes the new context solid.
+            and the resulting solid becomes the new context solid.
         """
 
         # If subtractive mode is requested, use cutBlind
         if combine in ("cut", "s"):
-            return self.cutBlind(until, clean, taper)
+            return self.cutBlind(until, clean, both, taper)
 
         # Handle `until` multiple values
         elif until in ("next", "last") and combine in (True, "a"):
             if until == "next":
                 faceIndex = 0
             elif until == "last":
                 faceIndex = -1
@@ -3076,31 +3054,31 @@
     ) -> T:
         """
         Use all un-revolved wires in the parent chain to create a solid.
 
         :param angleDegrees: the angle to revolve through.
         :type angleDegrees: float, anything less than 360 degrees will leave the shape open
         :param axisStart: the start point of the axis of rotation
-        :type axisStart: tuple, a two tuple
         :param axisEnd: the end point of the axis of rotation
-        :type axisEnd: tuple, a two tuple
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :return: a CQ object with the resulting solid selected.
 
         The returned object is always a CQ object, and depends on whether combine is True, and
         whether a context solid is already defined:
 
         *  if combine is False, the new value is pushed onto the stack.
         *  if combine is true, the value is combined with the context solid if it exists,
            and the resulting solid becomes the new context solid.
 
         .. note::
             Keep in mind that `axisStart` and `axisEnd` are defined relative to the current Workplane center position.
-            So if for example you want to revolve a circle centered at (10,0,0) around the Y axis, be sure to either :py:meth:`move` (or :py:meth:`moveTo`)
+            So if for example you want to revolve a circle centered at (10,0,0) around the Y axis, be sure to either :meth:`move` (or :meth:`moveTo`)
             the current Workplane position or specify `axisStart` and `axisEnd` with the correct vector position.
             In this example (0,0,0), (0,1,0) as axis coords would fail.
         """
         # Make sure we account for users specifying angles larger than 360 degrees
         angleDegrees %= 360.0
 
         # Compensate for OCCT not assuming that a 0 degree revolve means a 360 degree revolve
@@ -3143,30 +3121,33 @@
         normal: Optional[VectorLike] = None,
         auxSpine: Optional["Workplane"] = None,
     ) -> T:
         """
         Use all un-extruded wires in the parent chain to create a swept solid.
 
         :param path: A wire along which the pending wires will be swept
-        :param boolean multiSection: False to create multiple swept from wires on the chain along path. True to create only one solid swept along path with shape following the list of wires on the chain
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param multiSection: False to create multiple swept from wires on the chain along path.
+            True to create only one solid swept along path with shape following the list of wires on the chain
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :param transition: handling of profile orientation at C1 path discontinuities. Possible values are {'transformed','round', 'right'} (default: 'right').
         :param normal: optional fixed normal for extrusion
         :param auxSpine: a wire defining the binormal along the extrusion path
         :return: a CQ object with the resulting solid selected.
         """
 
         if not sweepAlongWires is None:
             multisection = sweepAlongWires
 
             from warnings import warn
 
             warn(
-                "sweepAlongWires keyword argument is is deprecated and will "
+                "sweepAlongWires keyword argument is deprecated and will "
                 "be removed in the next version; use multisection instead",
                 DeprecationWarning,
             )
 
         r = self._sweep(
             path.wire() if isinstance(path, Workplane) else path,
             multisection,
@@ -3183,14 +3164,15 @@
         self: T,
         obj: Union[Shape, Iterable[Shape]],
         mode: CombineMode = True,
         clean: bool = False,
     ) -> T:
         """
         Combines the provided object with the base solid, if one can be found.
+
         :param obj: The object to be combined with the context solid
         :param mode: The mode to combine with the base solid (True, False, "cut", "a" or "s")
         :return: a new object that represents the result of combining the base object with obj,
            or obj if one could not be found
         """
 
         if mode:
@@ -3215,14 +3197,15 @@
             ]
 
         return newS
 
     def _fuseWithBase(self: T, obj: Shape) -> T:
         """
         Fuse the provided object with the base solid, if one can be found.
+
         :param obj:
         :return: a new object that represents the result of combining the base object with obj,
            or obj if one could not be found
         """
         baseSolid = self._findType(
             (Solid, Compound), searchStack=True, searchParents=True
         )
@@ -3232,14 +3215,15 @@
         elif isinstance(obj, Compound):
             r = obj.fuse()
         return self.newObject([r])
 
     def _cutFromBase(self: T, obj: Shape) -> T:
         """
         Cuts the provided object from the base solid, if one can be found.
+
         :param obj:
         :return: a new object that represents the result of combining the base object with obj,
            or obj if one could not be found
         """
         baseSolid = self._findType((Solid, Compound), True, True)
 
         r = obj
@@ -3249,19 +3233,20 @@
         return self.newObject([r])
 
     def combine(
         self: T, clean: bool = True, glue: bool = False, tol: Optional[float] = None,
     ) -> T:
         """
         Attempts to combine all of the items on the stack into a single item.
+
         WARNING: all of the items must be of the same type!
 
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
-        :param boolean glue: use a faster gluing mode for non-overlapping shapes (default False)
-        :param float tol: tolerance value for fuzzy bool operation mode (default None)
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param glue: use a faster gluing mode for non-overlapping shapes (default False)
+        :param tol: tolerance value for fuzzy bool operation mode (default None)
         :raises: ValueError if there are no items on the stack, or if they cannot be combined
         :return: a CQ object with the resulting object selected
         """
 
         items: List[Shape] = [o for o in self.objects if isinstance(o, Shape)]
         s = items.pop(0)
 
@@ -3280,17 +3265,16 @@
         glue: bool = False,
         tol: Optional[float] = None,
     ) -> T:
         """
         Unions all of the items on the stack of toUnion with the current solid.
         If there is no current solid, the items in toUnion are unioned together.
 
-        :param toUnion:
-        :type toUnion: a solid object, or a Workplane object having a solid,
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape (default True)
+        :param toUnion: a solid object, or a Workplane object having a solid
+        :param clean: call :meth:`clean` afterwards to have a clean shape (default True)
         :param glue: use a faster gluing mode for non-overlapping shapes (default False)
         :param tol: tolerance value for fuzzy bool operation mode (default None)
         :raises: ValueError if there is no solid to add to in the chain
         :return: a Workplane object with the resulting object selected
         """
 
         # first collect all of the items together
@@ -3323,40 +3307,45 @@
             r = r.clean()
 
         return self.newObject([r])
 
     def __or__(self: T, toUnion: Union["Workplane", Solid, Compound]) -> T:
         """
         Syntactic sugar for union.
+
         Notice that :code:`r = a | b` is equivalent to :code:`r = a.union(b)` and :code:`r = a + b`.
 
         Example::
 
             Box = Workplane("XY").box(1, 1, 1, centered=(False, False, False))
             Sphere = Workplane("XY").sphere(1)
             result = Box | Sphere
         """
         return self.union(toUnion)
 
     def __add__(self: T, toUnion: Union["Workplane", Solid, Compound]) -> T:
         """
         Syntactic sugar for union.
+
         Notice that :code:`r = a + b` is equivalent to :code:`r = a.union(b)` and :code:`r = a | b`.
         """
         return self.union(toUnion)
 
     def cut(
-        self: T, toCut: Union["Workplane", Solid, Compound], clean: bool = True
+        self: T,
+        toCut: Union["Workplane", Solid, Compound],
+        clean: bool = True,
+        tol: Optional[float] = None,
     ) -> T:
         """
         Cuts the provided solid from the current solid, IE, perform a solid subtraction.
 
-        :param toCut: object to cut
-        :type toCut: a solid object, or a Workplane object having a solid,
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param toCut: a solid object, or a Workplane object having a solid
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param tol: tolerance value for fuzzy bool operation mode (default None)
         :raises ValueError: if there is no solid to subtract from in the chain
         :return: a Workplane object with the resulting object selected
         """
 
         # look for parents to cut from
         solidRef = self.findSolid(searchStack=True, searchParents=True)
 
@@ -3366,43 +3355,47 @@
             solidToCut = _selectShapes(toCut.vals())
             self._mergeTags(toCut)
         elif isinstance(toCut, (Solid, Compound)):
             solidToCut = (toCut,)
         else:
             raise ValueError("Cannot cut type '{}'".format(type(toCut)))
 
-        newS = solidRef.cut(*solidToCut)
+        newS = solidRef.cut(*solidToCut, tol=tol)
 
         if clean:
             newS = newS.clean()
 
         return self.newObject([newS])
 
     def __sub__(self: T, toUnion: Union["Workplane", Solid, Compound]) -> T:
         """
         Syntactic sugar for cut.
+
         Notice that :code:`r = a - b` is equivalent to :code:`r = a.cut(b)`.
 
         Example::
 
             Box = Workplane("XY").box(1, 1, 1, centered=(False, False, False))
             Sphere = Workplane("XY").sphere(1)
             result = Box - Sphere
         """
         return self.cut(toUnion)
 
     def intersect(
-        self: T, toIntersect: Union["Workplane", Solid, Compound], clean: bool = True,
+        self: T,
+        toIntersect: Union["Workplane", Solid, Compound],
+        clean: bool = True,
+        tol: Optional[float] = None,
     ) -> T:
         """
         Intersects the provided solid from the current solid.
 
-        :param toIntersect: object to intersect
-        :type toIntersect: a solid object, or a Workplane object having a solid,
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param toIntersect: a solid object, or a Workplane object having a solid
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param tol: tolerance value for fuzzy bool operation mode (default None)
         :raises ValueError: if there is no solid to intersect with in the chain
         :return: a Workplane object with the resulting object selected
         """
 
         # look for parents to intersect with
         solidRef = self.findSolid(searchStack=True, searchParents=True)
 
@@ -3412,74 +3405,102 @@
             solidToIntersect = _selectShapes(toIntersect.vals())
             self._mergeTags(toIntersect)
         elif isinstance(toIntersect, (Solid, Compound)):
             solidToIntersect = (toIntersect,)
         else:
             raise ValueError("Cannot intersect type '{}'".format(type(toIntersect)))
 
-        newS = solidRef.intersect(*solidToIntersect)
+        newS = solidRef.intersect(*solidToIntersect, tol=tol)
 
         if clean:
             newS = newS.clean()
 
         return self.newObject([newS])
 
     def __and__(self: T, toUnion: Union["Workplane", Solid, Compound]) -> T:
         """
         Syntactic sugar for intersect.
+
         Notice that :code:`r = a & b` is equivalent to :code:`r = a.intersect(b)`.
 
         Example::
 
             Box = Workplane("XY").box(1, 1, 1, centered=(False, False, False))
             Sphere = Workplane("XY").sphere(1)
             result = Box & Sphere
         """
         return self.intersect(toUnion)
 
     def cutBlind(
         self: T,
         until: Union[float, Literal["next", "last"], Face],
         clean: bool = True,
+        both: bool = False,
         taper: Optional[float] = None,
     ) -> T:
         """
         Use all un-extruded wires in the parent chain to create a prismatic cut from existing solid.
-        You must define either :distance: , :untilNextFace: or :untilLastFace:
+
+        Specify either a distance value, or one of "next", "last" to indicate a face to cut to.
 
         Similar to extrude, except that a solid in the parent chain is required to remove material
         from. cutBlind always removes material from a part.
 
         :param until: The distance to cut to, normal to the workplane plane. When a negative float
-          is passed the cut extends this far in the opposite direction to the normal of the plane
-          (i.e in the solid). The string "next" cuts until the next face orthogonal to the wire
-          normal.  "last" cuts to the last face. If a object of type Face is passed then the cut
-          will extend until this face.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
-        :param float taper: angle for optional tapered extrusion
+            is passed the cut extends this far in the opposite direction to the normal of the plane
+            (i.e in the solid). The string "next" cuts until the next face orthogonal to the wire
+            normal.  "last" cuts to the last face. If an object of type Face is passed, then the cut
+            will extend until this face.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param both: cut in both directions symmetrically
+        :param taper: angle for optional tapered extrusion
         :raises ValueError: if there is no solid to subtract from in the chain
         :return: a CQ object with the resulting object selected
 
-        see :py:meth:`cutThruAll` to cut material from the entire part
+        see :meth:`cutThruAll` to cut material from the entire part
         """
         # Handling of `until` passed values
         s: Union[Compound, Solid, Shape]
+        if isinstance(both, float) and taper == None:
+            # Because inserting a new paramater "both" in front of "taper",
+            # existing code calling this function with position arguments will
+            # pass the taper argument (float) to the "both" argument. This
+            # warning is to catch that.
+            from warnings import warn
+
+            warn(
+                "cutBlind added a new keyword argument `both=True`. "
+                "The signature is changed from "
+                "(until, clean, taper) -> (until, clean, both, taper)",
+                DeprecationWarning,
+            )
+
+            # assign 3rd argument value to taper
+            taper = both
+            both = False
+
         if isinstance(until, str) and until in ("next", "last"):
             if until == "next":
                 faceIndex = 0
             elif until == "last":
                 faceIndex = -1
 
-            s = self._extrude(None, taper=taper, upToFace=faceIndex, additive=False)
+            s = self._extrude(
+                None, both=both, taper=taper, upToFace=faceIndex, additive=False
+            )
 
         elif isinstance(until, Face):
-            s = self._extrude(None, taper=taper, upToFace=until, additive=False)
+            s = self._extrude(
+                None, both=both, taper=taper, upToFace=until, additive=False
+            )
 
         elif isinstance(until, (int, float)):
-            toCut = self._extrude(until, taper=taper, upToFace=None, additive=False)
+            toCut = self._extrude(
+                until, both=both, taper=taper, upToFace=None, additive=False
+            )
             solidRef = self.findSolid()
             s = solidRef.cut(toCut)
         else:
             raise ValueError(
                 f"Do not know how to handle until argument of type {type(until)}"
             )
         if clean:
@@ -3491,20 +3512,20 @@
         """
         Use all un-extruded wires in the parent chain to create a prismatic cut from existing solid.
         Cuts through all material in both normal directions of workplane.
 
         Similar to extrude, except that a solid in the parent chain is required to remove material
         from. cutThruAll always removes material from a part.
 
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :raises ValueError: if there is no solid to subtract from in the chain
         :raises ValueError: if there are no pending wires to cut with
         :return: a CQ object with the resulting object selected
 
-        see :py:meth:`cutBlind` to cut material to a limited depth
+        see :meth:`cutBlind` to cut material to a limited depth
         """
         solidRef = self.findSolid()
 
         s = solidRef.dprism(
             None, self._getFaces(), thruAll=True, additive=False, taper=-taper
         )
 
@@ -3515,17 +3536,19 @@
 
     def loft(
         self: T, ruled: bool = False, combine: CombineMode = True, clean: bool = True
     ) -> T:
         """
         Make a lofted solid, through the set of wires.
 
-        :param boolean ruled: When set to `True` connects each section linearly and without continuity
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param ruled: When set to `True` connects each section linearly and without continuity
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
         :return: a Workplane object containing the created loft
 
         """
 
         if self.ctx.pendingWires:
             wiresToLoft = self.ctx.popPendingWires()
@@ -3565,16 +3588,16 @@
         upToFace: Optional[Union[int, Face]] = None,
         additive: bool = True,
     ) -> Union[Solid, Compound]:
         """
         Make a prismatic solid from the existing set of pending wires.
 
         :param distance: distance to extrude
-        :param boolean both: extrude in both directions symetrically
-        :param upToFace: if specified extrude up to the :upToFace: face, 0 for the next, -1 for the last
+        :param both: extrude in both directions symetrically
+        :param upToFace: if specified, extrude up to a face: 0 for the next, -1 for the last face
         :param additive: specify if extruding or cutting, required param for uptoface algorithm
 
         :return: OCCT solid(s), suitable for boolean operations.
 
         This method is a utility method, primarily for plugin and internal use.
         It is the basis for cutBlind, extrude, cutThruAll, and all similar methods.
         """
@@ -3617,16 +3640,14 @@
             eDir = self.plane.zDir
         elif distance is not None:
             eDir = self.plane.zDir.multiply(distance)
 
         direction = "AlongAxis" if additive else "Opposite"
         taper = 0.0 if taper is None else taper
 
-        toFuse = []
-
         if upToFace is not None:
             res = self.findSolid()
             for face in faces:
                 if isinstance(upToFace, int):
                     facesList = getFacesList(face, eDir, direction, both=both)
                     if (
                         res.isInside(face.outerWire().Center())
@@ -3651,38 +3672,39 @@
                     res = res.dprism(
                         None,
                         [face],
                         taper=taper,
                         upToFace=limitFace2,
                         additive=additive,
                     )
-
         else:
+            toFuse = []
             for face in faces:
-                res = Solid.extrudeLinear(face, eDir, taper=taper)
-                toFuse.append(res)
+                s1 = Solid.extrudeLinear(face, eDir, taper=taper)
 
                 if both:
-                    res = Solid.extrudeLinear(face, eDir.multiply(-1.0), taper=taper)
-                    toFuse.append(res)
+                    s2 = Solid.extrudeLinear(face, eDir.multiply(-1.0), taper=taper)
+                    toFuse.append(s1.fuse(s2, glue=True))
+                else:
+                    toFuse.append(s1)
 
-        return res if upToFace is not None else Compound.makeCompound(toFuse)
+            res = Compound.makeCompound(toFuse)
+
+        return res
 
     def _revolve(
         self, angleDegrees: float, axisStart: VectorLike, axisEnd: VectorLike
     ) -> Compound:
         """
         Make a solid from the existing set of pending wires.
 
         :param angleDegrees: the angle to revolve through.
         :type angleDegrees: float, anything less than 360 degrees will leave the shape open
         :param axisStart: the start point of the axis of rotation
-        :type axisStart: tuple, a two tuple
         :param axisEnd: the end point of the axis of rotation
-        :type axisEnd: tuple, a two tuple
         :return: a OCCT solid(s), suitable for boolean operations.
 
         This method is a utility method, primarily for plugin and internal use.
         """
 
         # Revolve, make a compound out of them and then fuse them
         toFuse = []
@@ -3702,15 +3724,15 @@
         normal: Optional[VectorLike] = None,
         auxSpine: Optional["Workplane"] = None,
     ) -> Compound:
         """
         Makes a swept solid from an existing set of pending wires.
 
         :param path: A wire along which the pending wires will be swept
-        :param boolean multisection:
+        :param multisection:
             False to create multiple swept from wires on the chain along path
             True to create only one solid swept along path with shape following the list of wires on the chain
         :param transition:
             handling of profile orientation at C1 path discontinuities.
             Possible values are {'transformed','round', 'right'} (default: 'right').
         :param normal: optional fixed normal for extrusion
         :param auxSpine: a wire defining the binormal along the extrusion path
@@ -3760,49 +3782,33 @@
         tol3d: float = 0.0001,
         tolAng: float = 0.01,
         tolCurv: float = 0.1,
         maxDeg: int = 8,
         maxSegments: int = 9,
     ) -> T:
         """
-        Returns a plate surface that is 'thickness' thick, enclosed by 'surf_edge_pts' points,  and going
+        Returns a plate surface that is 'thickness' thick, enclosed by 'surf_edge_pts' points, and going
         through 'surf_pts' points.  Using pushPoints directly with interpPlate and combine=True, can be
-        very resources intensive depending on the complexity of the shape. In this case set combine=False.
+        very resource intensive depending on the complexity of the shape. In this case set combine=False.
 
-        :param surf_edges
-        :type 1 surf_edges: list of [x,y,z] float ordered coordinates
-        :type 2 surf_edges: list of ordered or unordered CadQuery wires
-        :param surf_pts = [] (uses only edges if [])
-        :type surf_pts: list of [x,y,z] float coordinates
-        :param thickness = 0 (returns 2D surface if 0)
-        :type thickness: float (may be negative or positive depending on thickening direction)
-        :param combine: should the results be combined with other solids on the stack
-            (and each other)?
-        :type combine: true to combine shapes, false otherwise.
-        :param boolean clean: call :py:meth:`clean` afterwards to have a clean shape
-        :param Degree = 3 (OCCT default)
-        :type Degree: Integer >= 2
-        :param NbPtsOnCur = 15 (OCCT default)
-        :type: NbPtsOnCur Integer >= 15
-        :param NbIter = 2 (OCCT default)
-        :type: NbIterInteger >= 2
-        :param anisotropy = False (OCCT default)
-        :type anisotropy: Boolean
-        :param: Tol2d = 0.00001 (OCCT default)
-        :type Tol2d: float > 0
-        :param Tol3d = 0.0001 (OCCT default)
-        :type Tol3dReal: float > 0
-        :param TolAng = 0.01 (OCCT default)
-        :type TolAngReal: float > 0
-        :param TolCurv = 0.1 (OCCT default)
-        :type TolCurvReal: float > 0
-        :param MaxDeg = 8 (OCCT default)
-        :type MaxDegInteger: Integer >= 2 (?)
-        :param MaxSegments = 9 (OCCT default)
-        :type MaxSegments: Integer >= 2 (?)
+        :param surf_edges: list of [x,y,z] ordered coordinates or list of ordered or unordered edges, wires
+        :param surf_pts: list of points (uses only edges if [])
+        :param thickness: value may be negative or positive depending on thickening direction (2D surface if 0)
+        :param combine: should the results be combined with other solids on the stack (and each other)?
+        :param clean: call :meth:`clean` afterwards to have a clean shape
+        :param degree: >= 2
+        :param nbPtsOnCur: number of points on curve >= 15
+        :param nbIter: number of iterations >= 2
+        :param anisotropy: = bool Anisotropy
+        :param tol2d: 2D tolerance
+        :param tol3d: 3D tolerance
+        :param tolAng: angular tolerance
+        :param tolCurv: tolerance for curvature
+        :param maxDeg: highest polynomial degree >= 2
+        :param maxSegments: greatest number of segments >= 2
         """
 
         # convert points to edges if needed
         edges: List[Union[Edge, Wire]] = []
         points = []
 
         if isinstance(surf_edges, Workplane):
@@ -3812,15 +3818,15 @@
                 if isinstance(el, (Edge, Wire)):
                     edges.append(el)
                 else:
                     points.append(el)
 
         # Creates interpolated plate
         f: Face = Face.makeNSidedSurface(
-            edges if not points else [Wire.makePolygon(points).close()],
+            edges if not points else [Wire.makePolygon(points, False, True)],
             surf_pts,
             degree=degree,
             nbPtsOnCur=nbPtsOnCur,
             nbIter=nbIter,
             anisotropy=anisotropy,
             tol2d=tol2d,
             tol3d=tol3d,
@@ -3844,26 +3850,23 @@
         combine: CombineMode = True,
         clean: bool = True,
     ) -> T:
         """
         Return a 3d box with specified dimensions for each object on the stack.
 
         :param length: box size in X direction
-        :type length: float > 0
         :param width: box size in Y direction
-        :type width: float > 0
         :param height: box size in Z direction
-        :type height: float > 0
         :param centered: If True, the box will be centered around the reference point.
-          If False, the corner of the box will be on the reference point and it will
-          extend in the positive x, y and z directions. Can also use a 3-tuple to
-          specify centering along each axis.
+            If False, the corner of the box will be on the reference point and it will
+            extend in the positive x, y and z directions. Can also use a 3-tuple to
+            specify centering along each axis.
         :param combine: should the results be combined with other solids on the stack
             (and each other)?
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
 
         One box is created for each item on the current stack. If no items are on the stack, one box
         using the current workplane center is created.
 
         If combine is true, the result will be a single object on the stack. If a solid was found
         in the chain, the result is that solid with all boxes produced fused onto it otherwise, the
         result is the combination of all the produced boxes.
@@ -3916,31 +3919,30 @@
         combine: CombineMode = True,
         clean: bool = True,
     ) -> T:
         """
         Returns a 3D sphere with the specified radius for each point on the stack.
 
         :param radius: The radius of the sphere
-        :type radius: float > 0
         :param direct: The direction axis for the creation of the sphere
         :type direct: A three-tuple
         :param angle1: The first angle to sweep the sphere arc through
         :type angle1: float > 0
         :param angle2: The second angle to sweep the sphere arc through
         :type angle2: float > 0
         :param angle3: The third angle to sweep the sphere arc through
         :type angle3: float > 0
         :param centered: If True, the sphere will be centered around the reference point. If False,
-          the corner of a bounding box around the sphere will be on the reference point and it
-          will extend in the positive x, y and z directions. Can also use a 3-tuple to specify
-          centering along each axis.
+            the corner of a bounding box around the sphere will be on the reference point and it
+            will extend in the positive x, y and z directions. Can also use a 3-tuple to specify
+            centering along each axis.
         :param combine: Whether the results should be combined with other solids on the stack
             (and each other)
         :type combine: true to combine shapes, false otherwise
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :return: A sphere object for each point on the stack
 
         One sphere is created for each item on the current stack. If no items are on the stack, one
         box using the current workplane center is created.
 
         If combine is true, the result will be a single object on the stack. If a solid was found
         in the chain, the result is that solid with all spheres produced fused onto it otherwise,
@@ -3979,29 +3981,27 @@
         combine: CombineMode = True,
         clean: bool = True,
     ) -> T:
         """
         Returns a cylinder with the specified radius and height for each point on the stack
 
         :param height: The height of the cylinder
-        :type height: float > 0
         :param radius: The radius of the cylinder
-        :type radius: float > 0
         :param direct: The direction axis for the creation of the cylinder
         :type direct: A three-tuple
         :param angle: The angle to sweep the cylinder arc through
         :type angle: float > 0
         :param centered: If True, the cylinder will be centered around the reference point. If False,
             the corner of a bounding box around the cylinder will be on the reference point and it
             will extend in the positive x, y and z directions. Can also use a 3-tuple to specify
             centering along each axis.
         :param combine: Whether the results should be combined with other solids on the stack
             (and each other)
         :type combine: true to combine shapes, false otherwise
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :return: A cylinder object for each point on the stack
 
         One cylinder is created for each item on the current stack. If no items are on the stack, one
         cylinder is created using the current workplane center.
 
         If combine is true, the result will be a single object on the stack. If a solid was found
         in the chain, the result is that solid with all cylinders produced fused onto it otherwise,
@@ -4143,16 +4143,18 @@
         Returns a 3D text.
 
         :param txt: text to be rendered
         :param fontsize: size of the font in model units
         :param distance: the distance to extrude or cut, normal to the workplane plane
         :type distance: float, negative means opposite the normal direction
         :param cut: True to cut the resulting solid from the parent solids if found
-        :param combine: True or "a" to combine the resulting solid with parent solids if found, "cut" or "s" to remove the resulting solid from the parent solids if found. False to keep the resulting solid separated from the parent solids.
-        :param clean: call :py:meth:`clean` afterwards to have a clean shape
+        :param combine: True or "a" to combine the resulting solid with parent solids if found,
+            "cut" or "s" to remove the resulting solid from the parent solids if found.
+            False to keep the resulting solid separated from the parent solids.
+        :param clean: call :meth:`clean` afterwards to have a clean shape
         :param font: font name
         :param fontPath: path to font file
         :param kind: font type
         :param halign: horizontal alignment
         :param valign: vertical alignment
         :return: a CQ object with the resulting solid selected
 
@@ -4197,15 +4199,15 @@
 
         return self._combineWithBase(r, combine, clean)
 
     def section(self: T, height: float = 0.0) -> T:
         """
         Slices current solid at the given height.
 
-        :param float height: height to slice at (default: 0)
+        :param height: height to slice at (default: 0)
         :raises ValueError: if no solids or compounds are found
         :return: a CQ object with the resulting face(s).
         """
 
         solidRef = self.findSolid(searchStack=True, searchParents=True)
 
         plane = Face.makePlane(
```

### Comparing `cadquery-2.2.0b2/cadquery/cq_directive.py` & `cadquery-2.3.0/cadquery/cq_directive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 """
 A special directive for including a cq object.
 
 """
 
 import traceback
 
-from pathlib import Path
-from uuid import uuid1 as uuid
-from textwrap import indent
+from json import dumps
 
 from cadquery import exporters, Assembly, Compound, Color, Sketch
 from cadquery import cqgi
-from cadquery.occ_impl.jupyter_tools import (
-    toJSON,
-    dumps,
-    TEMPLATE_RENDER,
-    DEFAULT_COLOR,
-)
+from cadquery.occ_impl.assembly import toJSON
+from cadquery.occ_impl.jupyter_tools import DEFAULT_COLOR
 from docutils.parsers.rst import directives, Directive
 
 template = """
 
 .. raw:: html
 
     <div class="cq" style="text-align:%(txt_align)s;float:left;">
         %(out_svg)s
     </div>
     <div style="clear:both;">
     </div>
 
 """
-template_content_indent = "      "
 
 rendering_code = """
 const RENDERERS = {};
 var ID =  0;
 
 const renderWindow = vtk.Rendering.Core.vtkRenderWindow.newInstance();
 const openglRenderWindow = vtk.Rendering.OpenGL.vtkRenderWindow.newInstance();
@@ -195,15 +188,15 @@
 
 
 template_vtk = """
 
 .. raw:: html
 
     <div class="cq-vtk"
-     style="text-align:{txt_align}s;float:left;border: 1px solid #ddd; width:{width}; height:{height}"">
+     style="text-align:{txt_align};float:left;border: 1px solid #ddd; width:{width}; height:{height}">
        <script>
        var parent_element = {element};
        var data = {data};
        render(data, parent_element);
        </script>
     </div>
     <div style="clear:both;">
@@ -212,18 +205,16 @@
 """
 
 
 class cq_directive(Directive):
 
     has_content = True
     required_arguments = 0
-    optional_arguments = 2
+    optional_arguments = 0
     option_spec = {
-        "height": directives.length_or_unitless,
-        "width": directives.length_or_percentage_or_unitless,
         "align": directives.unchanged,
     }
 
     def run(self):
 
         options = self.options
         content = self.content
@@ -274,30 +265,27 @@
         return []
 
 
 class cq_directive_vtk(Directive):
 
     has_content = True
     required_arguments = 0
-    optional_arguments = 2
+    optional_arguments = 0
     option_spec = {
         "height": directives.length_or_unitless,
         "width": directives.length_or_percentage_or_unitless,
         "align": directives.unchanged,
         "select": directives.unchanged,
     }
 
     def run(self):
 
         options = self.options
         content = self.content
         state_machine = self.state_machine
-        env = self.state.document.settings.env
-        build_path = Path(env.app.builder.outdir)
-        out_path = build_path / "_static"
 
         # only consider inline snippets
         plot_code = "\n".join(content)
 
         # collect the result
         try:
             result = cqgi.parse(plot_code).build()
@@ -317,29 +305,22 @@
             else:
                 raise result.exception
 
         except Exception:
             traceback.print_exc()
             assy = Assembly(Compound.makeText("CQGI error", 10, 5))
 
-        # save vtkjs to static
-        fname = Path(str(uuid()))
-        exporters.assembly.exportVTKJS(assy, out_path / fname)
-        fname = str(fname) + ".zip"
-
         # add the output
         lines = []
 
         data = dumps(toJSON(assy))
 
         lines.extend(
             template_vtk.format(
-                code=indent(TEMPLATE_RENDER.format(), "    "),
                 data=data,
-                ratio="null",
                 element="document.currentScript.parentNode",
                 txt_align=options.get("align", "left"),
                 width=options.get("width", "100%"),
                 height=options.get("height", "500px"),
             ).splitlines()
         )
```

### Comparing `cadquery-2.2.0b2/cadquery/cqgi.py` & `cadquery-2.3.0/cadquery/cqgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     Parses the script as a model, and returns a model.
 
     If you would prefer to access the underlying model without building it,
     for example, to inspect its available parameters, construct a CQModel object.
 
     :param script_source: the script to run. Must be a valid cadquery script
     :return: a CQModel object that defines the script and allows execution
-
     """
     model = CQModel(script_source)
     return model
 
 
 class CQModel(object):
     """
@@ -35,14 +34,15 @@
 
     the build method can be used to generate a 3d model
     """
 
     def __init__(self, script_source):
         """
         Create an object by parsing the supplied python script.
+
         :param script_source: a python script to parse
         """
         self.metadata = ScriptMetadata()
         self.ast_tree = ast.parse(script_source, CQSCRIPT)
         self.script_source = script_source
         self._find_vars()
 
@@ -72,30 +72,32 @@
         description_finder = ParameterDescriptionFinder(self.metadata)
         description_finder.visit(self.ast_tree)
 
     def validate(self, params):
         """
         Determine if the supplied parameters are valid.
         NOT IMPLEMENTED YET-- raises NotImplementedError
+
         :param params: a dictionary of parameters
 
         """
         raise NotImplementedError("not yet implemented")
 
     def build(self, build_parameters=None, build_options=None):
         """
         Executes the script, using the optional parameters to override those in the model
+
         :param build_parameters: a dictionary of variables. The variables must be
-        assignable to the underlying variable type. These variables override default values in the script
+            assignable to the underlying variable type. These variables override default values in the script
         :param build_options: build options for how to build the model. Build options include things like
-        timeouts, tessellation tolerances, etc
+            timeouts, tessellation tolerances, etc
         :raises: Nothing. If there is an exception, it will be on the exception property of the result.
-        This is the interface so that we can return other information on the result, such as the build time
+            This is the interface so that we can return other information on the result, such as the build time
         :return: a BuildResult object, which includes the status of the result, and either
-        a resulting shape or an exception
+            a resulting shape or an exception
         """
         if not build_parameters:
             build_parameters = {}
 
         start = time.perf_counter()
         result = BuildResult()
 
@@ -322,15 +324,16 @@
 
     def __init__(self):
         self.outputObjects = []
         self.debugObjects = []
 
     def show_object(self, shape, options={}, **kwargs):
         """
-        return an object to the executing environment, with options
+        Return an object to the executing environment, with options.
+
         :param shape: a cadquery object
         :param options: a dictionary of options that will be made available to the executing environment
         """
         options.update(kwargs)
 
         o = ShapeResult()
         o.options = options
```

### Comparing `cadquery-2.2.0b2/cadquery/hull.py` & `cadquery-2.3.0/cadquery/hull.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/__init__.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import tempfile
 import os
 import io as StringIO
 
-from typing import IO, Optional, Union, cast
+from typing import IO, Optional, Union, cast, Dict, Any
 from typing_extensions import Literal
 
 from OCP.VrmlAPI import VrmlAPI
 
 from ...cq import Workplane
 from ...utils import deprecate
 from ..shapes import Shape
 
 from .svg import getSVG
 from .json import JsonMesh
 from .amf import AmfWriter
 from .threemf import ThreeMFWriter
-from .dxf import exportDXF
+from .dxf import exportDXF, DxfDocument
 from .vtk import exportVTP
 from .utils import toCompound
 
 
 class ExportTypes:
     STL = "STL"
     STEP = "STEP"
@@ -39,15 +39,15 @@
 
 def export(
     w: Union[Shape, Workplane],
     fname: str,
     exportType: Optional[ExportLiterals] = None,
     tolerance: float = 0.1,
     angularTolerance: float = 0.1,
-    opt=None,
+    opt: Optional[Dict[str, Any]] = None,
 ):
 
     """
     Export Workplane or Shape to file. Multiple entities are converted to compound.
 
     :param w:  Shape or Workplane to be exported.
     :param fname: output filename.
@@ -56,14 +56,17 @@
     :param angularTolerance: the angular tolerance, in radians. Default 0.1.
     :param opt: additional options passed to the specific exporter. Default None.
     """
 
     shape: Shape
     f: IO
 
+    if not opt:
+        opt = {}
+
     if isinstance(w, Workplane):
         shape = toCompound(w)
     else:
         shape = w
 
     if exportType is None:
         t = fname.split(".")[-1].upper()
@@ -94,29 +97,26 @@
     elif exportType == ExportTypes.AMF:
         tess = shape.tessellate(tolerance, angularTolerance)
         aw = AmfWriter(tess)
         with open(fname, "wb") as f:
             aw.writeAmf(f)
 
     elif exportType == ExportTypes.THREEMF:
-        tmfw = ThreeMFWriter(shape, tolerance, angularTolerance, **opt or {})
+        tmfw = ThreeMFWriter(shape, tolerance, angularTolerance, **opt)
         with open(fname, "wb") as f:
             tmfw.write3mf(f)
 
     elif exportType == ExportTypes.DXF:
         if isinstance(w, Workplane):
-            exportDXF(w, fname)
+            exportDXF(w, fname, **opt)
         else:
             raise ValueError("Only Workplanes can be exported as DXF")
 
     elif exportType == ExportTypes.STEP:
-        if opt:
-            shape.exportStep(fname, **opt)
-        else:
-            shape.exportStep(fname)
+        shape.exportStep(fname, **opt)
 
     elif exportType == ExportTypes.STL:
         if opt:
             useascii = opt.get("ascii", False) or opt.get("ASCII", False)
         else:
             useascii = False
```

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/amf.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/amf.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/json.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/json.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/svg.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/svg.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,28 +140,31 @@
         projectionDir: Direction the camera will view the shape from.
         showAxes: Whether or not to show the axes indicator, which will only be
                   visible when the projectionDir is also at the default.
         strokeWidth: Width of the line that visible edges are drawn with.
         strokeColor: Color of the line that visible edges are drawn with.
         hiddenColor: Color of the line that hidden edges are drawn with.
         showHidden: Whether or not to show hidden lines.
+        focus: If specified, creates a perspective SVG with the projector
+               at the distance specified.
     """
 
     # Available options and their defaults
     d = {
         "width": 800,
         "height": 240,
         "marginLeft": 200,
         "marginTop": 20,
         "projectionDir": (-1.75, 1.1, 5),
         "showAxes": True,
         "strokeWidth": -1.0,  # -1 = calculated based on unitScale
         "strokeColor": (0, 0, 0),  # RGB 0-255
         "hiddenColor": (160, 160, 160),  # RGB 0-255
         "showHidden": True,
+        "focus": None,
     }
 
     if opts:
         d.update(opts)
 
     # need to guess the scale and the coordinate center
     uom = guessUnitOfMeasure(shape)
@@ -172,19 +175,25 @@
     marginTop = float(d["marginTop"])
     projectionDir = tuple(d["projectionDir"])
     showAxes = bool(d["showAxes"])
     strokeWidth = float(d["strokeWidth"])
     strokeColor = tuple(d["strokeColor"])
     hiddenColor = tuple(d["hiddenColor"])
     showHidden = bool(d["showHidden"])
+    focus = float(d["focus"]) if d.get("focus") else None
 
     hlr = HLRBRep_Algo()
     hlr.Add(shape.wrapped)
 
-    projector = HLRAlgo_Projector(gp_Ax2(gp_Pnt(), gp_Dir(*projectionDir)))
+    coordinate_system = gp_Ax2(gp_Pnt(), gp_Dir(*projectionDir))
+
+    if focus is not None:
+        projector = HLRAlgo_Projector(coordinate_system, focus)
+    else:
+        projector = HLRAlgo_Projector(coordinate_system)
 
     hlr.Projector(projector)
     hlr.Update()
     hlr.Hide()
 
     hlr_shapes = HLRBRep_HLRToShape(hlr)
```

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/threemf.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/threemf.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/exporters/vtk.py` & `cadquery-2.3.0/cadquery/occ_impl/exporters/vtk.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/geom.py` & `cadquery-2.3.0/cadquery/occ_impl/geom.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/importers/__init__.py` & `cadquery-2.3.0/cadquery/occ_impl/importers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from math import pi
+from typing import List
 
 from ... import cq
 from ..shapes import Shape
 from .dxf import _importDXF
 
 
 from OCP.STEPControl import STEPControl_Reader
@@ -63,22 +64,24 @@
     solids = []
     for shape in occ_shapes:
         solids.append(Shape.cast(shape))
 
     return cq.Workplane("XY").newObject(solids)
 
 
-def importDXF(filename, tol=1e-6, exclude=[], include=[]):
+def importDXF(
+    filename: str, tol: float = 1e-6, exclude: List[str] = [], include: List[str] = []
+) -> "cq.Workplane":
     """
     Loads a DXF file into a Workplane.
 
     All layers are imported by default.  Provide a layer include or exclude list
-     to select layers.  Layer names are handled as case-insensitive.
+    to select layers.  Layer names are handled as case-insensitive.
 
-    :param fileName: The path and name of the DXF file to be imported
+    :param filename: The path and name of the DXF file to be imported
     :param tol: The tolerance used for merging edges into wires
     :param exclude: a list of layer names not to import
     :param include: a list of layer names to import
     """
 
     faces = _importDXF(filename, tol, exclude, include)
```

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/importers/dxf.py` & `cadquery-2.3.0/cadquery/occ_impl/importers/dxf.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/jupyter_tools.py` & `cadquery-2.3.0/cadquery/occ_impl/jupyter_tools.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/shapes.py` & `cadquery-2.3.0/cadquery/occ_impl/shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,19 @@
 
 from OCP.BRepFilletAPI import (
     BRepFilletAPI_MakeChamfer,
     BRepFilletAPI_MakeFillet,
     BRepFilletAPI_MakeFillet2d,
 )
 
-from OCP.TopTools import TopTools_IndexedDataMapOfShapeListOfShape, TopTools_ListOfShape
+from OCP.TopTools import (
+    TopTools_IndexedDataMapOfShapeListOfShape,
+    TopTools_ListOfShape,
+    TopTools_MapOfShape,
+)
 
 from OCP.TopExp import TopExp
 
 from OCP.ShapeFix import ShapeFix_Shape, ShapeFix_Solid, ShapeFix_Face
 
 from OCP.STEPControl import STEPControl_Writer, STEPControl_AsIs
 
@@ -232,14 +236,18 @@
 
 from OCP.Prs3d import Prs3d_IsoAspect
 from OCP.Quantity import Quantity_Color
 from OCP.Aspect import Aspect_TOL_SOLID
 
 from OCP.Interface import Interface_Static
 
+from OCP.ShapeCustom import ShapeCustom, ShapeCustom_RestrictionParameters
+
+from OCP.BRepAlgo import BRepAlgo
+
 from math import pi, sqrt, inf
 
 import warnings
 
 from ..utils import deprecate
 
 Real = Union[float, int]
@@ -474,15 +482,15 @@
 
         kwargs is used to provide optional keyword arguments to configure the exporter.
 
         :param fileName: Path and filename for writing.
         :param write_pcurves: Enable or disable writing parametric curves to the STEP file. Default True.
 
             If False, writes STEP file without pcurves. This decreases the size of the resulting STEP file.
-        :type write_pcurves: boolean
+        :type write_pcurves: bool
         :param precision_mode: Controls the uncertainty value for STEP entities. Specify -1, 0, or 1. Default 0.
             See OCCT documentation.
         :type precision_mode: int
         """
 
         # Handle the extra settings for the STEP export
         pcurves = 1
@@ -533,16 +541,18 @@
             CQ(object).faces("%mytype")
 
         The expectation is that the geomType attribute will return 'mytype'
 
         The return values depend on the type of the shape:
 
         | Vertex:  always 'Vertex'
-        | Edge:   LINE, ARC, CIRCLE, SPLINE
-        | Face:   PLANE, SPHERE, CONE
+        | Edge:   LINE, CIRCLE, ELLIPSE, HYPERBOLA, PARABOLA, BEZIER, 
+        |         BSPLINE, OFFSET, OTHER
+        | Face:   PLANE, CYLINDER, CONE, SPHERE, TORUS, BEZIER, BSPLINE, 
+        |         REVOLUTION, EXTRUSION, OFFSET, OTHER
         | Solid:  'Solid'
         | Shell:  'Shell'
         | Compound: 'Compound'
         | Wire:   'Wire'
 
         :returns: A string according to the geometry type
         """
@@ -599,16 +609,16 @@
 
     def BoundingBox(
         self, tolerance: Optional[float] = None
     ) -> BoundBox:  # need to implement that in GEOM
         """
         Create a bounding box for this Shape.
 
-        :param tolerance: Tolerance value passed to :py:class:`BoundBox`
-        :returns: A :py:class:`BoundBox` object for this Shape
+        :param tolerance: Tolerance value passed to :class:`BoundBox`
+        :returns: A :class:`BoundBox` object for this Shape
         """
         return BoundBox._fromTopoDS(self.wrapped, tol=tolerance)
 
     def mirror(
         self,
         mirrorPlane: Union[
             Literal["XY", "YX", "XZ", "ZX", "YZ", "ZY"], VectorLike
@@ -743,26 +753,29 @@
         return self.wrapped.Closed()
 
     def ShapeType(self) -> Shapes:
         return tcast(Shapes, shape_LUT[shapetype(self.wrapped)])
 
     def _entities(self, topo_type: Shapes) -> List[TopoDS_Shape]:
 
-        out = {}  # using dict to prevent duplicates
+        rv = []
+        shape_set = TopTools_MapOfShape()
 
         explorer = TopExp_Explorer(self.wrapped, inverse_shape_LUT[topo_type])
 
         while explorer.More():
             item = explorer.Current()
-            out[
-                item.HashCode(HASH_CODE_MAX)
-            ] = item  # needed to avoid pseudo-duplicate entities
+
+            # needed to avoid pseudo-duplicate entities
+            if shape_set.Add(item):
+                rv.append(item)
+
             explorer.Next()
 
-        return list(out.values())
+        return rv
 
     def _entitiesFrom(
         self, child_type: Shapes, parent_type: Shapes
     ) -> Dict["Shape", List["Shape"]]:
 
         res = TopTools_IndexedDataMapOfShapeListOfShape()
 
@@ -908,20 +921,23 @@
         """
 
         T = gp_Trsf()
         T.SetScale(gp_Pnt(), factor)
 
         return self._apply_transform(T)
 
-    def copy(self: T) -> T:
+    def copy(self: T, mesh: bool = False) -> T:
         """
         Creates a new object that is a copy of this object.
+
+        :param mesh: should I copy the triangulation too (default: False)
+        :returns: a copy of the object
         """
 
-        return self.__class__(BRepBuilderAPI_Copy(self.wrapped).Shape())
+        return self.__class__(BRepBuilderAPI_Copy(self.wrapped, True, mesh).Shape())
 
     def transformShape(self, tMatrix: Matrix) -> "Shape":
         """
         Transforms this Shape by tMatrix. Also see :py:meth:`transformGeometry`.
 
         :param tMatrix: The transformation matrix
         :returns: a copy of the object, transformed by the provided matrix,
@@ -1033,70 +1049,80 @@
         op.SetTools(tool)
 
         op.SetRunParallel(True)
         op.Build()
 
         return Shape.cast(op.Shape())
 
-    def cut(self, *toCut: "Shape") -> "Shape":
+    def cut(self, *toCut: "Shape", tol: Optional[float] = None) -> "Shape":
         """
         Remove the positional arguments from this Shape.
+        
+        :param tol: Fuzzy mode tolerance
         """
 
         cut_op = BRepAlgoAPI_Cut()
 
+        if tol:
+            cut_op.SetFuzzyValue(tol)
+
         return self._bool_op((self,), toCut, cut_op)
 
     def fuse(
         self, *toFuse: "Shape", glue: bool = False, tol: Optional[float] = None
     ) -> "Shape":
         """
         Fuse the positional arguments with this Shape.
 
         :param glue: Sets the glue option for the algorithm, which allows
             increasing performance of the intersection of the input shapes
-        :param tol: Additional tolerance
+        :param tol: Fuzzy mode tolerance
         """
 
         fuse_op = BRepAlgoAPI_Fuse()
         if glue:
             fuse_op.SetGlue(BOPAlgo_GlueEnum.BOPAlgo_GlueShift)
         if tol:
             fuse_op.SetFuzzyValue(tol)
 
         rv = self._bool_op((self,), toFuse, fuse_op)
 
         return rv
 
-    def intersect(self, *toIntersect: "Shape") -> "Shape":
+    def intersect(self, *toIntersect: "Shape", tol: Optional[float] = None) -> "Shape":
         """
         Intersection of the positional arguments and this Shape.
+        
+        :param tol: Fuzzy mode tolerance
         """
 
         intersect_op = BRepAlgoAPI_Common()
 
+        if tol:
+            intersect_op.SetFuzzyValue(tol)
+
         return self._bool_op((self,), toIntersect, intersect_op)
 
     def facesIntersectedByLine(
         self,
         point: VectorLike,
         axis: VectorLike,
         tol: float = 1e-4,
         direction: Optional[Literal["AlongAxis", "Opposite"]] = None,
     ):
         """
         Computes the intersections between the provided line and the faces of this Shape
 
-        :point: Base point for defining a line
-        :axis: Axis on which the line rest
-        :tol: Intersection tolerance
-        :direction: Valid values : "AlongAxis", "Opposite", if specified will ignore all faces that are not in the specified direction
-        including the face where the :point: lies if it is the case
-
-        :returns: A list of intersected faces sorted by distance from :point:
+        :param point: Base point for defining a line
+        :param axis: Axis on which the line rests
+        :param tol: Intersection tolerance
+        :param direction: Valid values: "AlongAxis", "Opposite";
+            If specified, will ignore all faces that are not in the specified direction
+            including the face where the point lies if it is the case
+        :returns: A list of intersected faces sorted by distance from point
         """
 
         oc_point = (
             gp_Pnt(*point.toTuple()) if isinstance(point, Vector) else gp_Pnt(*point)
         )
         oc_axis = (
             gp_Dir(Vector(axis).wrapped)
@@ -1238,14 +1264,42 @@
                 for t in poly.Triangles()
             ]
 
             offset += poly.NbNodes()
 
         return vertices, triangles
 
+    def toSplines(
+        self: T, degree: int = 3, tolerance: float = 1e-3, nurbs: bool = False
+    ) -> T:
+        """
+        Approximate shape with b-splines of the specified degree.
+
+        :param degree: Maximum degree.
+        :param tolerance: Approximation tolerance.
+        :param nurbs: Use rational splines.
+        """
+
+        params = ShapeCustom_RestrictionParameters()
+
+        result = ShapeCustom.BSplineRestriction_s(
+            self.wrapped,
+            tolerance,  # 3D tolerance
+            tolerance,  # 2D tolerance
+            degree,
+            1,  # dumy value, degree is leading
+            ga.GeomAbs_C0,
+            ga.GeomAbs_C0,
+            True,  # set degree to be leading
+            not nurbs,
+            params,
+        )
+
+        return self.__class__(result)
+
     def toVtkPolyData(
         self,
         tolerance: Optional[float] = None,
         angularTolerance: Optional[float] = None,
         normals: bool = False,
     ) -> vtkPolyData:
         """
@@ -1320,15 +1374,15 @@
     A Single Point in Space
     """
 
     wrapped: TopoDS_Vertex
 
     def __init__(self, obj: TopoDS_Shape, forConstruction: bool = False):
         """
-        Create a vertex from a FreeCAD Vertex
+        Create a vertex
         """
         super(Vertex, self).__init__(obj)
 
         self.forConstruction = forConstruction
         self.X, self.Y, self.Z = self.toTuple()
 
     def toTuple(self) -> Tuple[float, float, float]:
@@ -1506,14 +1560,15 @@
 
     def positionAt(
         self: Mixin1DProtocol,
         d: float,
         mode: Literal["length", "parameter"] = "length",
     ) -> Vector:
         """Generate a position along the underlying curve.
+
         :param d: distance or parameter value
         :param mode: position calculation mode (default: length)
         :return: A Vector on the underlying curve located at the specified d value.
         """
 
         curve = self._geomAdaptor()
 
@@ -1526,14 +1581,15 @@
 
     def positions(
         self: Mixin1DProtocol,
         ds: Iterable[float],
         mode: Literal["length", "parameter"] = "length",
     ) -> List[Vector]:
         """Generate positions along the underlying curve
+
         :param ds: distance or parameter values
         :param mode: position calculation mode (default: length)
         :return: A list of Vector objects.
         """
 
         return [self.positionAt(d, mode) for d in ds]
 
@@ -1541,14 +1597,15 @@
         self: Mixin1DProtocol,
         d: float,
         mode: Literal["length", "parameter"] = "length",
         frame: Literal["frenet", "corrected"] = "frenet",
         planar: bool = False,
     ) -> Location:
         """Generate a location along the underlying curve.
+
         :param d: distance or parameter value
         :param mode: position calculation mode (default: length)
         :param frame: moving frame calculation method (default: frenet)
         :param planar: planar mode
         :return: A Location object representing local coordinate system at the specified distance.
         """
 
@@ -1588,14 +1645,15 @@
         self: Mixin1DProtocol,
         ds: Iterable[float],
         mode: Literal["length", "parameter"] = "length",
         frame: Literal["frenet", "corrected"] = "frenet",
         planar: bool = False,
     ) -> List[Location]:
         """Generate location along the curve
+
         :param ds: distance or parameter values
         :param mode: position calculation mode (default: length)
         :param frame: moving frame calculation method (default: frenet)
         :param planar: planar mode
         :return: A list of Location objects representing local coordinate systems at the specified distances.
         """
 
@@ -1880,14 +1938,15 @@
 
     @classmethod
     def makeThreePointArc(
         cls, v1: VectorLike, v2: VectorLike, v3: VectorLike
     ) -> "Edge":
         """
         Makes a three point arc through the provided points
+
         :param cls:
         :param v1: start vector
         :param v2: middle vector
         :param v3: end vector
         :return: an edge object through the three points
         """
         circle_geom = GC_MakeArcOfCircle(
@@ -1895,16 +1954,16 @@
         ).Value()
 
         return cls(BRepBuilderAPI_MakeEdge(circle_geom).Edge())
 
     @classmethod
     def makeTangentArc(cls, v1: VectorLike, v2: VectorLike, v3: VectorLike) -> "Edge":
         """
-        Makes a tangent arc from point v1, in the direction of v2 and ends at
-        v3.
+        Makes a tangent arc from point v1, in the direction of v2 and ends at v3.
+
         :param cls:
         :param v1: start vector
         :param v2: tangent vector
         :param v3: end vector
         :return: an edge
         """
         circle_geom = GC_MakeArcOfCircle(
@@ -1913,14 +1972,15 @@
 
         return cls(BRepBuilderAPI_MakeEdge(circle_geom).Edge())
 
     @classmethod
     def makeLine(cls, v1: VectorLike, v2: VectorLike) -> "Edge":
         """
         Create a line between two points
+
         :param v1: Vector that represents the first point
         :param v2: Vector that represents the second point
         :return: A linear edge between the two provided points
         """
         return cls(
             BRepBuilderAPI_MakeEdge(Vector(v1).toPnt(), Vector(v2).toPnt()).Edge()
         )
@@ -1955,14 +2015,15 @@
 
     @classmethod
     def combine(
         cls, listOfWires: Iterable[Union["Wire", Edge]], tol: float = 1e-9
     ) -> List["Wire"]:
         """
         Attempt to combine a list of wires and edges into a new wire.
+
         :param cls:
         :param listOfWires:
         :param tol: default 1e-9
         :return: List[Wire]
         """
 
         edges_in = TopTools_HSequenceOfShape()
@@ -1975,22 +2036,25 @@
 
         return [cls(el) for el in wires_out]
 
     @classmethod
     def assembleEdges(cls, listOfEdges: Iterable[Edge]) -> "Wire":
         """
         Attempts to build a wire that consists of the edges in the provided list
+
         :param cls:
         :param listOfEdges: a list of Edge objects. The edges are not to be consecutive.
         :return: a wire with the edges assembled
-        :BRepBuilderAPI_MakeWire::Error() values
-            :BRepBuilderAPI_WireDone = 0
-            :BRepBuilderAPI_EmptyWire = 1
-            :BRepBuilderAPI_DisconnectedWire = 2
-            :BRepBuilderAPI_NonManifoldWire = 3
+
+        BRepBuilderAPI_MakeWire::Error() values:
+
+        * BRepBuilderAPI_WireDone = 0
+        * BRepBuilderAPI_EmptyWire = 1
+        * BRepBuilderAPI_DisconnectedWire = 2
+        * BRepBuilderAPI_NonManifoldWire = 3
         """
         wire_builder = BRepBuilderAPI_MakeWire()
 
         occ_edges_list = TopTools_ListOfShape()
         for e in listOfEdges:
             occ_edges_list.Append(e.wrapped)
         wire_builder.Add(occ_edges_list)
@@ -2008,18 +2072,18 @@
 
     @classmethod
     def makeCircle(
         cls, radius: float, center: VectorLike, normal: VectorLike
     ) -> "Wire":
         """
         Makes a Circle centered at the provided point, having normal in the provided direction
+
         :param radius: floating point radius of the circle, must be > 0
         :param center: vector representing the center of the circle
         :param normal: vector representing the direction of the plane the circle should lie in
-        :return:
         """
 
         circle_edge = Edge.makeCircle(radius, center, normal)
         w = cls.assembleEdges([circle_edge])
         return w
 
     @classmethod
@@ -2033,22 +2097,22 @@
         angle1: float = 360.0,
         angle2: float = 360.0,
         rotation_angle: float = 0.0,
         closed: bool = True,
     ) -> "Wire":
         """
         Makes an Ellipse centered at the provided point, having normal in the provided direction
+
         :param x_radius: floating point major radius of the ellipse (x-axis), must be > 0
         :param y_radius: floating point minor radius of the ellipse (y-axis), must be > 0
         :param center: vector representing the center of the circle
         :param normal: vector representing the direction of the plane the circle should lie in
         :param angle1: start angle of arc
         :param angle2: end angle of arc
         :param rotation_angle: angle to rotate the created ellipse / arc
-        :return: Wire
         """
 
         ellipse_edge = Edge.makeEllipse(
             x_radius, y_radius, center, normal, xDir, angle1, angle2
         )
 
         if angle1 != angle2 and closed:
@@ -2060,22 +2124,31 @@
         if rotation_angle != 0.0:
             w = w.rotate(center, Vector(center) + Vector(normal), rotation_angle)
 
         return w
 
     @classmethod
     def makePolygon(
-        cls, listOfVertices: Iterable[VectorLike], forConstruction: bool = False,
+        cls,
+        listOfVertices: Iterable[VectorLike],
+        forConstruction: bool = False,
+        close: bool = False,
     ) -> "Wire":
-        # convert list of tuples into Vectors.
+        """
+        Construct a polygonal wire from points.
+        """
+
         wire_builder = BRepBuilderAPI_MakePolygon()
 
         for v in listOfVertices:
             wire_builder.Add(Vector(v).toPnt())
 
+        if close:
+            wire_builder.Close()
+
         w = cls(wire_builder.Wire())
         w.forConstruction = forConstruction
 
         return w
 
     @classmethod
     def makeHelix(
@@ -2123,15 +2196,15 @@
         # 4. Convert to wire and fix building 3d geom from 2d geom
         w = BRepBuilderAPI_MakeWire(e).Wire()
         BRepLib.BuildCurves3d_s(w, 1e-6, MaxSegment=2000)  # NB: preliminary values
 
         return cls(w)
 
     def stitch(self, other: "Wire") -> "Wire":
-        """Attempt to stich wires"""
+        """Attempt to stitch wires"""
 
         wire_builder = BRepBuilderAPI_MakeWire()
         wire_builder.Add(TopoDS.Wire_s(self.wrapped))
         wire_builder.Add(TopoDS.Wire_s(other.wrapped))
         wire_builder.Build()
 
         return self.__class__(wire_builder.Wire())
@@ -2197,15 +2270,15 @@
 
         return BRepTools.UVBounds_s(self.wrapped)
 
     def normalAt(self, locationVector: Optional[Vector] = None) -> Vector:
         """
         Computes the normal vector at the desired location on the face.
 
-        :returns: a  vector representing the direction
+        :returns: a vector representing the direction
         :param locationVector: the location to compute the normal at. If none, the center of the face is used.
         :type locationVector: a vector that lies on the surface.
         """
         # get the geometry
         surface = self._geomAdaptor()
 
         if locationVector is None:
@@ -2255,41 +2328,31 @@
         tol3d: float = 0.0001,
         tolAng: float = 0.01,
         tolCurv: float = 0.1,
         maxDeg: int = 8,
         maxSegments: int = 9,
     ) -> "Face":
         """
-        Returns a surface enclosed by a closed polygon defined by 'edges' and going through 'points'.
-        :param constraints
-        :type points: list of constraints (points or edges)
-        :param edges
-        :type edges: list of Edge
-        :param continuity=GeomAbs_C0
-        :type continuity: OCC.Core.GeomAbs continuity condition
-        :param Degree = 3 (OCCT default)
-        :type Degree: Integer >= 2
-        :param NbPtsOnCur = 15 (OCCT default)
-        :type: NbPtsOnCur Integer >= 15
-        :param NbIter = 2 (OCCT default)
-        :type: NbIterInteger >= 2
-        :param Anisotropie = False (OCCT default)
-        :type Anisotropie: Boolean
-        :param: Tol2d = 0.00001 (OCCT default)
-        :type Tol2d: float > 0
-        :param Tol3d = 0.0001 (OCCT default)
-        :type Tol3dReal: float > 0
-        :param TolAng = 0.01 (OCCT default)
-        :type TolAngReal: float > 0
-        :param TolCurv = 0.1 (OCCT default)
-        :type TolCurvReal: float > 0
-        :param MaxDeg = 8 (OCCT default)
-        :type MaxDegInteger: Integer >= 2 (?)
-        :param MaxSegments = 9 (OCCT default)
-        :type MaxSegments: Integer >= 2 (?)
+        Returns a surface enclosed by a closed polygon defined by 'edges' and 'constraints'.
+
+        :param edges: edges
+        :type edges: list of edges or wires
+        :param constraints: constraints
+        :type constraints: list of points or edges
+        :param continuity: OCC.Core.GeomAbs continuity condition
+        :param degree: >=2
+        :param nbPtsOnCur: number of points on curve >= 15
+        :param nbIter: number of iterations >= 2
+        :param anisotropy: bool Anisotropy
+        :param tol2d: 2D tolerance >0
+        :param tol3d: 3D tolerance >0
+        :param tolAng: angular tolerance
+        :param tolCurv: tolerance for curvature >0
+        :param maxDeg: highest polynomial degree >= 2
+        :param maxSegments: greatest number of segments >= 2
         """
 
         n_sided = BRepOffsetAPI_MakeFilling(
             degree,
             nbPtsOnCur,
             nbIter,
             anisotropy,
@@ -2363,15 +2426,15 @@
     @classmethod
     def makeRuledSurface(cls, edgeOrWire1: Wire, edgeOrWire2: Wire) -> "Face":
         ...
 
     @classmethod
     def makeRuledSurface(cls, edgeOrWire1, edgeOrWire2):
         """
-        'makeRuledSurface(Edge|Wire,Edge|Wire) -- Make a ruled surface
+        makeRuledSurface(Edge|Wire,Edge|Wire) -- Make a ruled surface
         Create a ruled surface out of two edges or wires. If wires are used then
         these must have the same number of edges
         """
 
         if isinstance(edgeOrWire1, Wire):
             return cls.cast(BRepFill.Shell_s(edgeOrWire1.wrapped, edgeOrWire2.wrapped))
         else:
@@ -2429,15 +2492,14 @@
         Approximate a spline surface through the provided points.
 
         :param points: a 2D list of Vectors that represent the points
         :param tol: tolerance of the algorithm (consult OCC documentation).
         :param smoothing: optional tuple of 3 weights use for variational smoothing (default: None)
         :param minDeg: minimum spline degree. Enforced only when smothing is None (default: 1)
         :param maxDeg: maximum spline degree (default: 6)
-        :return: an Face
         """
         points_ = TColgp_HArray2OfPnt(1, len(points), 1, len(points[0]))
 
         for i, vi in enumerate(points):
             for j, v in enumerate(vi):
                 points_.SetValue(i + 1, j + 1, v.toPnt())
 
@@ -2540,14 +2602,23 @@
     def project(self, other: "Face", d: VectorLike) -> "Face":
 
         outer_p = tcast(Wire, self.outerWire().project(other, d))
         inner_p = (tcast(Wire, w.project(other, d)) for w in self.innerWires())
 
         return self.constructOn(other, outer_p, *inner_p)
 
+    def toArcs(self, tolerance: float = 1e-3) -> "Face":
+        """
+        Approximate planar face with arcs and straight line segments.
+
+        :param tolerance: Approximation tolerance.
+        """
+
+        return self.__class__(BRepAlgo.ConvertFace_s(self.wrapped, tolerance))
+
 
 class Shell(Shape):
     """
     the outer boundary of a surface
     """
 
     wrapped: TopoDS_Shell
@@ -2569,14 +2640,15 @@
 TS = TypeVar("TS", bound=ShapeProtocol)
 
 
 class Mixin3D(object):
     def fillet(self: Any, radius: float, edgeList: Iterable[Edge]) -> Any:
         """
         Fillets the specified edges of this solid.
+
         :param radius: float > 0, the radius of the fillet
         :param edgeList:  a list of Edge objects, which must belong to this solid
         :return: Filleted solid
         """
         nativeEdges = [e.wrapped for e in edgeList]
 
         fillet_builder = BRepFilletAPI_MakeFillet(self.wrapped)
@@ -2587,14 +2659,15 @@
         return self.__class__(fillet_builder.Shape())
 
     def chamfer(
         self: Any, length: float, length2: Optional[float], edgeList: Iterable[Edge]
     ) -> Any:
         """
         Chamfers the specified edges of this solid.
+
         :param length: length > 0, the length (length) of the chamfer
         :param length2: length2 > 0, optional parameter for asymmetrical chamfer. Should be `None` if not required.
         :param edgeList:  a list of Edge objects, which must belong to this solid
         :return: Chamfered solid
         """
         nativeEdges = [e.wrapped for e in edgeList]
 
@@ -2782,43 +2855,31 @@
         tol3d=0.0001,
         tolAng=0.01,
         tolCurv=0.1,
         maxDeg=8,
         maxSegments=9,
     ) -> Union["Solid", Face]:
         """
-        Returns a plate surface that is 'thickness' thick, enclosed by 'surf_edge_pts' points,  and going through 'surf_pts' points.
+        Returns a plate surface that is 'thickness' thick, enclosed by 'surf_edge_pts' points, and going through 'surf_pts' points.
 
-        :param surf_edges
-        :type 1 surf_edges: list of [x,y,z] float ordered coordinates
-        :type 2 surf_edges: list of ordered or unordered CadQuery wires
-        :param surf_pts = [] (uses only edges if [])
-        :type surf_pts: list of [x,y,z] float coordinates
-        :param thickness = 0 (returns 2D surface if 0)
-        :type thickness: float (may be negative or positive depending on thickening direction)
-        :param Degree = 3 (OCCT default)
-        :type Degree: Integer >= 2
-        :param NbPtsOnCur = 15 (OCCT default)
-        :type: NbPtsOnCur Integer >= 15
-        :param NbIter = 2 (OCCT default)
-        :type: NbIterInteger >= 2
-        :param Anisotropie = False (OCCT default)
-        :type Anisotropie: Boolean
-        :param: Tol2d = 0.00001 (OCCT default)
-        :type Tol2d: float > 0
-        :param Tol3d = 0.0001 (OCCT default)
-        :type Tol3dReal: float > 0
-        :param TolAng = 0.01 (OCCT default)
-        :type TolAngReal: float > 0
-        :param TolCurv = 0.1 (OCCT default)
-        :type TolCurvReal: float > 0
-        :param MaxDeg = 8 (OCCT default)
-        :type MaxDegInteger: Integer >= 2 (?)
-        :param MaxSegments = 9 (OCCT default)
-        :type MaxSegments: Integer >= 2 (?)
+        :param surf_edges:
+            list of [x,y,z] float ordered coordinates
+            or list of ordered or unordered wires
+        :param surf_pts: list of [x,y,z] float coordinates (uses only edges if [])
+        :param thickness: thickness may be negative or positive depending on direction, (returns 2D surface if 0)
+        :param degree: >=2
+        :param nbPtsOnCur: number of points on curve >= 15
+        :param nbIter: number of iterations >= 2
+        :param anisotropy: bool Anisotropy
+        :param tol2d: 2D tolerance >0
+        :param tol3d: 3D tolerance >0
+        :param tolAng: angular tolerance
+        :param tolCurv: tolerance for curvature >0
+        :param maxDeg: highest polynomial degree >= 2
+        :param maxSegments: greatest number of segments >= 2
         """
 
         # POINTS CONSTRAINTS: list of (x,y,z) points, optional.
         pts_array = [gp_Pnt(*pt) for pt in surf_pts]
 
         # EDGE CONSTRAINTS
         # If a list of wires is provided, make a closed wire
@@ -2889,15 +2950,15 @@
         width: float,
         height: float,
         pnt: VectorLike = Vector(0, 0, 0),
         dir: VectorLike = Vector(0, 0, 1),
     ) -> "Solid":
         """
         makeBox(length,width,height,[pnt,dir]) -- Make a box located in pnt with the dimensions (length,width,height)
-        By default pnt=Vector(0,0,0) and dir=Vector(0,0,1)'
+        By default pnt=Vector(0,0,0) and dir=Vector(0,0,1)
         """
         return cls(
             BRepPrimAPI_MakeBox(
                 gp_Ax2(Vector(pnt).toPnt(), Vector(dir).toDir()), length, width, height
             ).Shape()
         )
 
@@ -2910,15 +2971,15 @@
         pnt: VectorLike = Vector(0, 0, 0),
         dir: VectorLike = Vector(0, 0, 1),
         angleDegrees: float = 360,
     ) -> "Solid":
         """
         Make a cone with given radii and height
         By default pnt=Vector(0,0,0),
-        dir=Vector(0,0,1) and angle=360'
+        dir=Vector(0,0,1) and angle=360
         """
         return cls(
             BRepPrimAPI_MakeCone(
                 gp_Ax2(Vector(pnt).toPnt(), Vector(dir).toDir()),
                 radius1,
                 radius2,
                 height,
@@ -2934,15 +2995,15 @@
         pnt: VectorLike = Vector(0, 0, 0),
         dir: VectorLike = Vector(0, 0, 1),
         angleDegrees: float = 360,
     ) -> "Solid":
         """
         makeCylinder(radius,height,[pnt,dir,angle]) --
         Make a cylinder with a given radius and height
-        By default pnt=Vector(0,0,0),dir=Vector(0,0,1) and angle=360'
+        By default pnt=Vector(0,0,0),dir=Vector(0,0,1) and angle=360
         """
         return cls(
             BRepPrimAPI_MakeCylinder(
                 gp_Ax2(Vector(pnt).toPnt(), Vector(dir).toDir()),
                 radius,
                 height,
                 angleDegrees * DEG2RAD,
@@ -2959,15 +3020,15 @@
         angleDegrees1: float = 0,
         angleDegrees2: float = 360,
     ) -> "Solid":
         """
         makeTorus(radius1,radius2,[pnt,dir,angle1,angle2,angle]) --
         Make a torus with a given radii and angles
         By default pnt=Vector(0,0,0),dir=Vector(0,0,1),angle1=0
-        ,angle1=360 and angle=360'
+        ,angle1=360 and angle=360
         """
         return cls(
             BRepPrimAPI_MakeTorus(
                 gp_Ax2(Vector(pnt).toPnt(), Vector(dir).toDir()),
                 radius1,
                 radius2,
                 angleDegrees1 * DEG2RAD,
@@ -3075,26 +3136,27 @@
         """
         Creates a 'twisted prism' by extruding, while simultaneously rotating around the extrusion vector.
 
         Though the signature may appear to be similar enough to extrudeLinear to merit combining them, the
         construction methods used here are different enough that they should be separate.
 
         At a high level, the steps followed are:
+
         (1) accept a set of wires
         (2) create another set of wires like this one, but which are transformed and rotated
         (3) create a ruledSurface between the sets of wires
         (4) create a shell and compute the resulting object
 
-        :param outerWire: the outermost wire, a cad.Wire
-        :param innerWires: a list of inner wires, a list of cad.Wire
+        :param outerWire: the outermost wire
+        :param innerWires: a list of inner wires
         :param vecCenter: the center point about which to rotate.  the axis of rotation is defined by
-               vecNormal, located at vecCenter. ( a cad.Vector )
-        :param vecNormal: a vector along which to extrude the wires ( a cad.Vector )
+            vecNormal, located at vecCenter.
+        :param vecNormal: a vector along which to extrude the wires
         :param angleDegrees: the angle to rotate through while extruding
-        :return: a cad.Solid object
+        :return: a Solid object
         """
         # make straight spine
         straight_spine_e = Edge.makeLine(vecCenter, vecCenter.add(vecNormal))
         straight_spine_w = Wire.combine([straight_spine_e,])[0].wrapped
 
         # make an auxiliary spine
         pitch = 360.0 / angleDegrees * vecNormal.Length
@@ -3139,15 +3201,15 @@
         cls,
         outerWire: Wire,
         innerWires: List[Wire],
         vecNormal: VectorLike,
         taper: Real = 0,
     ) -> "Solid":
         """
-        Attempt to extrude the list of wires  into a prismatic solid in the provided direction
+        Attempt to extrude the list of wires into a prismatic solid in the provided direction
 
         :param outerWire: the outermost wire
         :param innerWires: a list of inner wires
         :param vecNormal: a vector along which to extrude the wires
         :param taper: taper angle, default=0
         :return: a Solid object
 
@@ -3204,17 +3266,15 @@
         Attempt to revolve the list of wires into a solid in the provided direction
 
         :param outerWire: the outermost wire
         :param innerWires: a list of inner wires
         :param angleDegrees: the angle to revolve through.
         :type angleDegrees: float, anything less than 360 degrees will leave the shape open
         :param axisStart: the start point of the axis of rotation
-        :type axisStart: tuple, a two tuple
         :param axisEnd: the end point of the axis of rotation
-        :type axisEnd: tuple, a two tuple
         :return: a Solid object
 
         The wires must not intersect
 
         * all wires must be closed
         * there cannot be any intersecting or self-intersecting wires
         * wires must be listed from outside in
@@ -3288,22 +3348,22 @@
         path: Union[Wire, Edge],
         makeSolid: bool = True,
         isFrenet: bool = False,
         mode: Union[Vector, Wire, Edge, None] = None,
         transitionMode: Literal["transformed", "round", "right"] = "transformed",
     ) -> "Shape":
         """
-        Attempt to sweep the list of wires  into a prismatic solid along the provided path
+        Attempt to sweep the list of wires into a prismatic solid along the provided path
 
         :param outerWire: the outermost wire
         :param innerWires: a list of inner wires
         :param path: The wire to sweep the face resulting from the wires over
-        :param boolean makeSolid: return Solid or Shell (default True)
-        :param boolean isFrenet: Frenet mode (default False)
-        :param mode: additional sweep mode parameters.
+        :param makeSolid: return Solid or Shell (default True)
+        :param isFrenet: Frenet mode (default False)
+        :param mode: additional sweep mode parameters
         :param transitionMode:
             handling of profile orientation at C1 path discontinuities.
             Possible values are {'transformed','round', 'right'} (default: 'right').
         :return: a Solid object
         """
         p = cls._toWire(path)
 
@@ -3528,21 +3588,26 @@
     def __bool__(self) -> bool:
         """
         Check if empty.
         """
 
         return TopoDS_Iterator(self.wrapped).More()
 
-    def cut(self, *toCut: Shape) -> "Compound":
+    def cut(self, *toCut: "Shape", tol: Optional[float] = None) -> "Compound":
         """
-        Remove a shape from another one
+        Remove the positional arguments from this Shape.
+        
+        :param tol: Fuzzy mode tolerance
         """
 
         cut_op = BRepAlgoAPI_Cut()
 
+        if tol:
+            cut_op.SetFuzzyValue(tol)
+
         return tcast(Compound, self._bool_op(self, toCut, cut_op))
 
     def fuse(
         self, *toFuse: Shape, glue: bool = False, tol: Optional[float] = None
     ) -> "Compound":
         """
         Fuse shapes together
@@ -3562,21 +3627,28 @@
             rv = self._bool_op(args[:1], args[1:], fuse_op)
 
         # fuse_op.RefineEdges()
         # fuse_op.FuseEdges()
 
         return tcast(Compound, rv)
 
-    def intersect(self, *toIntersect: Shape) -> "Compound":
+    def intersect(
+        self, *toIntersect: "Shape", tol: Optional[float] = None
+    ) -> "Compound":
         """
-        Construct shape intersection
+        Intersection of the positional arguments and this Shape.
+        
+        :param tol: Fuzzy mode tolerance
         """
 
         intersect_op = BRepAlgoAPI_Common()
 
+        if tol:
+            intersect_op.SetFuzzyValue(tol)
+
         return tcast(Compound, self._bool_op(self, toIntersect, intersect_op))
 
 
 def sortWiresByBuildOrder(wireList: List[Wire]) -> List[List[Wire]]:
     """Tries to determine how wires should be combined into faces.
 
     Assume:
```

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/sketch_solver.py` & `cadquery-2.3.0/cadquery/occ_impl/sketch_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         rv = array((x[0] + x[2] * sin(a), x[1] + x[2] * cos(a)))
 
     return rv
 
 
 def line_point(x, val):
 
-    return x[:2] + val * x[2:]
+    return x[:2] + val * (x[2:] - x[:2])
 
 
 def arc_first_tangent(x):
 
     return gp_Vec2d(sign(x[4]) * cos(x[3]), -sign(x[4]) * sin(x[3]))
```

### Comparing `cadquery-2.2.0b2/cadquery/occ_impl/solver.py` & `cadquery-2.3.0/cadquery/occ_impl/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,17 @@
                 2 * a / (m + 1), 2 * b / (m + 1), 2 * c / (m + 1), (1 - m) / (m + 1),
             )
         )
         rv.SetTranslationPart(gp_Vec(*opti.value(T)))
 
         return rv
 
-    def solve(self) -> Tuple[List[Location], Dict[str, Any]]:
+    def solve(self, verbosity: int = 0) -> Tuple[List[Location], Dict[str, Any]]:
+
+        suppress_banner = "yes" if verbosity == 0 else "no"
 
         opti = self.opti
 
         constraints = self.constraints
         variables = self.variables
         start_points = self.start_points
 
@@ -705,15 +707,16 @@
                 "acceptable_obj_change_tol": 1e-12,
                 "acceptable_iter": 1,
                 "tol": 1e-14,
                 "hessian_approximation": "exact",
                 "nlp_scaling_method": "none",
                 "honor_original_bounds": "yes",
                 "bound_relax_factor": 0,
-                "print_level": 5,
+                "print_level": verbosity,
+                "sb": suppress_banner,
                 "print_timing_statistics": "no",
                 "linear_solver": "mumps",
             },
         )
         sol = opti.solve_limited()
 
         result = sol.stats()
```

### Comparing `cadquery-2.2.0b2/cadquery/plugins/__init__.py` & `cadquery-2.3.0/cadquery/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/cadquery/selectors.py` & `cadquery-2.3.0/cadquery/selectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     """
 
     def filter(self, objectList):
         """
         Filter the provided list.
 
         The default implementation returns the original list unfiltered.
+
         :param objectList: list to filter
         :type objectList: list of OCCT primitives
         :return: filtered list
         """
         return objectList
 
     def __and__(self, other):
```

### Comparing `cadquery-2.2.0b2/cadquery/sketch.py` & `cadquery-2.3.0/cadquery/sketch.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,17 @@
         mode: Modes = "a",
         tag: Optional[str] = None,
     ) -> T:
         """
         Construct a polygonal face.
         """
 
-        w = Wire.makePolygon(p if isinstance(p, Vector) else Vector(*p) for p in pts)
+        w = Wire.makePolygon(
+            (p if isinstance(p, Vector) else Vector(*p) for p in pts), False, True
+        )
 
         return self.face(w, angle, mode, tag)
 
     # distribute locations
 
     def rarray(self: T, xs: Real, ys: Real, nx: int, ny: int) -> T:
         """
```

### Comparing `cadquery-2.2.0b2/cadquery/utils.py` & `cadquery-2.3.0/cadquery/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         self.name = name
         self.new_name = new_name
 
     def __call__(self, f):
         @wraps(f)
         def wrapped(*args, **kwargs):
 
-            f_sig_params = signature(f).parameters
-
-            if f_sig_params[self.name]:
+            if self.name in kwargs:
                 warn(
                     f"Kwarg <{self.name}> will be removed. Please use <{self.new_name}>",
                     FutureWarning,
                 )
 
             return f(*args, **kwargs)
```

### Comparing `cadquery-2.2.0b2/cadquery.egg-info/PKG-INFO` & `cadquery-2.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: cadquery
-Version: 2.2.0b2
-Summary: CadQuery is a parametric  scripting language for creating and traversing CAD models
-Home-page: https://github.com/CadQuery/cadquery
-Author: David Cowden
-Author-email: dave.cowden@gmail.com
-License: Apache Public License 2.0
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8,<3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: ipython
-License-File: LICENSE
-
 ![CadQuery logo](./doc/_static/logo/cadquery_logo_dark.svg)
 # CadQuery
 
 [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/79ox42i6smelx7n8/branch/master?svg=true)](https://ci.appveyor.com/project/jmwright/cadquery-o18bh/branch/master)
 [![Build Status](https://dev.azure.com/cadquery/conda-packages/_apis/build/status/CadQuery.cadquery?branchName=master)](https://dev.azure.com/cadquery/conda-packages/_build/latest?definitionId=2&branchName=master)
 [![codecov](https://codecov.io/gh/CadQuery/cadquery/branch/master/graph/badge.svg)](https://codecov.io/gh/CadQuery/cadquery)
 [![Documentation Status](https://readthedocs.org/projects/cadquery/badge/?version=latest)](https://cadquery.readthedocs.io/en/latest/?badge=latest)
@@ -52,14 +23,18 @@
 
 1. The scripts use a standard programming language, Python, and thus can benefit from the associated infrastructure. This includes many standard libraries and IDEs.
 2. CadQuery's CAD kernel Open CASCADE Technology ([OCCT](https://en.wikipedia.org/wiki/Open_Cascade_Technology)) is much more powerful than the [CGAL](https://en.wikipedia.org/wiki/CGAL) used by OpenSCAD. Features supported natively by OCCT include NURBS, splines, surface sewing, STL repair, STEP import/export, and other complex operations, in addition to the standard CSG operations supported by CGAL
 3. Ability to import/export [STEP](https://en.wikipedia.org/wiki/ISO_10303) and the ability to begin with a STEP model, created in a CAD package, and then add parametric features. This is possible in OpenSCAD using STL, but STL is a lossy format.
 4. CadQuery scripts require less code to create most objects, because it is possible to locate features based on the position of other features, workplanes, vertices, etc.
 5. CadQuery scripts can build STL, STEP, AMF and 3MF faster than OpenSCAD.
 
+CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts.  Options for visualziation are also available including CQ-Editor and JupyterLab.
+
+For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+
 ### Key features
 * Build 3D models with scripts that are as close as possible to how you would describe the object to a human.
 * Create parametric models that can be very easily customized by end users.
 * Output high quality (loss-less) CAD formats like STEP and DXF in addition to STL, VRML, AMF and 3MF.
 * Provide a non-proprietary, plain text model format that can be edited and executed with only a web browser.
 * Offer advanced modeling capabilities such as fillets, curvilinear extrudes, parametric curves and lofts.
 * Build nested assemblies out of individual parts and other assemblies.
@@ -68,131 +43,86 @@
 
 The original version of CadQuery was built on the FreeCAD API. This was great because it allowed for fast development and easy cross-platform capability. However, we eventually started reaching the limits of the API for some advanced operations and selectors. This 2.0 version of CadQuery is based directly on a Python wrapper of the OCCT kernel. This gives us a great deal more control and flexibility, at the expense of some simplicity and having to handle the cross-platform aspects of deployment ourselves. We believe this is a worthwhile trade-off to allow CadQuery to continue to grow and expand in the future.
 
 ## Getting started
 
 To learn more about designing with CadQuery, visit the [documentation](https://cadquery.readthedocs.io/en/latest/intro.html), [examples](https://cadquery.readthedocs.io/en/latest/examples.html), and [cheatsheet](https://cadquery.readthedocs.io/en/latest/_static/cadquery_cheatsheet.html).
 
-To get started playing around with CadQuery and see it's capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.
+To get started playing around with CadQuery and see its capabilities, take a look at the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor). This easy-to-use IDE is a great way to get started desiging with CadQuery.  The CQ-editor installer bundles both CQ-editor and CadQuery (recommended).  See the [CQ-editor installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor).
 
-There are currently 4 different ways to use CadQuery for designing your next project:
-* Using the [CQ-editor GUI](https://github.com/CadQuery/CQ-editor)
-* From a [Jupyter notebook](https://github.com/bernhard-42/jupyter-cadquery)
-* Using a [VSCode extension](https://marketplace.visualstudio.com/items?itemName=roipoussiere.cadquery)
-* As a standalone library
-    * Linux [installation video](https://youtu.be/sjLTePOq8bQ)
-    * Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
+The CadQuery library (with or without CQ-editor) and its dependencies may be installed using conda, or pip.  Note that conda (or the CQ-editor installer) is the better supported option.
 
-There are two ways to install CadQuery and its dependencies. One is using conda, and the other is using pip. Pip is shown first below, followed by two sections on installing CadQuery via conda, and a non-intrusive way to install conda on a system. Note that conda is the better supported option.
+See the documentation for detailed CadQuery [installation instructions](https://cadquery.readthedocs.io/en/latest/installation.html).
 
-### CadQuery Installation Via Pip
+There are also videos covering installation:
 
-CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method outlined in the next two sections.
+* Linux [installation video](https://youtu.be/sjLTePOq8bQ)
+* Windows [installation video](https://youtu.be/3Tg_RJhqZRg)
 
-It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
-```
-python3 -m pip install --upgrade pip
-```
-Once a current version of pip is installed, CadQuery can be installed using the following command line.
-```
-pip install --pre cadquery
-```
-NB: CadQuery has only recently returned to PyPI, and a full release has not happened yet. When the final release of CadQuery 2.2 is published, it will be possible to simply type `pip install cadquery`.
+### CadQuery Installation Via Conda
 
-It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
-```
-pip install git+https://github.com/CadQuery/cadquery.git
-```
+To first install the Conda package manager see [Install the Conda Package Manager](https://cadquery.readthedocs.io/en/latest/installation.html#install-the-conda-package-manager).
 
-You should now have a working CadQuery installation, but developers or users who want to use CadQuery with IPython/Jupyter or to set up a developer environment can read the rest of this section.
+The steps to install cadquery with conda are as follows:
 
-If you are installing CadQuery to use with IPython/Jupyter, you may want to run the following command line to install the extra dependencies.
-```
-pip install cadquery[ipython]==2.2.0b0
-```
-
-If you want to create a developer setup to contribute to CadQuery, the following command line will install all the development dependencies that are needed.
-```
-pip install cadquery[dev]==2.2.0b0
-```
-
-### CadQuery Installation Via Conda
-
-conda is included as part of a [miniforge](https://github.com/conda-forge/miniforge) installation (other distributions can be used as well). See the next section for more details regarding conda. The steps to install cadquery are as follows:
 ```
 # Set up a new environment
 conda create -n cadquery
 
 # Activate the new environment
 conda activate cadquery
 
-# CadQuery development is moving quickly, so it is best to install the latest version from GitHub master
+# Install the latest released version
+conda install -c conda-forge cadquery occt=7.7.0
+
+# Or install the dev version to get the latest changes
 conda install -c conda-forge -c cadquery cadquery=master
 ```
 
-For those who are interested, the [OCP repository](https://github.com/CadQuery/OCP) contains the current OCCT wrapper used by CQ.
+### CadQuery Installation Via Pip
 
-### Conda Installation
+CadQuery has a complex set of dependencies including OCP, which is our set of bindings to the OpenCASCADE CAD kernel. OCP is distributed as binary wheels for Linux, MacOS and Windows. However, there are some limitations. Only Python 3.8 through 3.10 are currently supported, and some older Linux distributions such as Ubuntu 18.04 are not supported. If the pip installation method does not work for your system, you can try the conda installation method.
 
-For those unfamiliar (or uncomfortable) with conda, it is probably best to install Miniforge to a local directory and to avoid running `conda init`. After performing a local directory installation, Miniforge can be activated via the [scripts,bin]/activate scripts. This will help avoid polluting and breaking the local Python installation. In Linux, the local directory installation method looks something like this:
+It is highly recommended that a virtual environment is used when installing CadQuery, although it is not strictly required. Installing CadQuery via pip requires a up-to-date version of pip, which can be obtained with the following command line (or a slight variation thereof).
 ```
-# Install the script to ~/miniforge
-wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh -O miniforge.sh
-bash miniforge.sh -b -p $HOME/miniforge
-
-# To activate and use Miniconda
-source $HOME/miniforge/bin/activate
+python3 -m pip install --upgrade pip
 ```
-On Windows one can install locally as follows:
+Once a current version of pip is installed, CadQuery can be installed using the following command line.
+```
+pip install cadquery
 ```
-:: Install
-curl -L -o miniforge.exe https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe
-start /wait "" miniforge.exe /InstallationType=JustMe /RegisterPython=0 /NoRegistry=1 /NoScripts=1 /S /D=%USERPROFILE%\Miniforge3
 
-:: Activate
-cmd /K ""%USERPROFILE%/Miniforge3/Scripts/activate.bat" "%USERPROFILE%/Miniforge3""
+It is also possible to install the very latest changes directly from CadQuery's GitHub repository, with the understanding that sometimes breaking changes can occur. To install from the git repository, run the following command line.
 ```
-You might want to consider using `/NoScripts=0` to have an activation shortcut added to the start menu.
+pip install git+https://github.com/CadQuery/cadquery.git
+```
+
 
 ### CQ-editor GUI
 
 CQ-editor is an IDE that allows users to edit CadQuery model scripts in a GUI environment. It includes features such as:
 
 * A graphical debugger that allows you to step through your scripts.
 * A CadQuery stack inspector.
 * Export to various formats, including STEP and STL, directly from the menu.
 
-The installation instructions for CQ-editor can be found [here](https://github.com/CadQuery/CQ-editor#installation).
+More on CQ-editor:
+* [CQ-editor README](https://github.com/CadQuery/CQ-editor/blob/master/README.md)
+* [Installation](https://cadquery.readthedocs.io/en/latest/installation.html#adding-a-nicer-gui-via-cq-editor)
+
 
 <img src="https://raw.githubusercontent.com/CadQuery/CQ-editor/master/screenshots/screenshot3.png" alt="CQ editor screenshot" width="800"/>
 
 ### Jupyter
 
-CadQuery supports Jupyter notebook out of the box using the jupyter-cadquery extension created by @bernhard-42:
-
-* [Installation](https://github.com/bernhard-42/jupyter-cadquery#installation)
-* [Usage](https://github.com/bernhard-42/jupyter-cadquery#jupyter-cadquery)
-
-<img src="https://raw.githubusercontent.com/bernhard-42/jupyter-cadquery/master/screenshots/0_intro.png" alt="CadQuery Jupyter extension screenshot" width="800"/>
+CadQuery supports Jupyter out-of-the-box.  Run your CadQuery code in the notebook and visualize the model by calling ```display(<CadQuery object>)```.
 
-### Docker
+ * [JupyterLab installation](https://cadquery.readthedocs.io/en/latest/installation.html#jupyter).
 
-A list of Docker images can be found [here](https://github.com/RubenRubens/cq-containers), and includes images for the following projects.
-* [Core CadQuery library](https://github.com/RubenRubens/cq-containers/tree/master/cq-conda), which allows users to run CadQuery Python scripts without a GUI.
-* [cq-cli](https://github.com/RubenRubens/cq-containers/tree/master/cq-cli), a command line utility which is used to export the results of a CadQuery script to an output format (i.e. STL, STEP).
-* [jupyter-cadquery](https://github.com/bernhard-42/jupyter-cadquery#b-using-a-docker-image), makes CadQuery accessible through Jupyter Labs and provides a web-based GUI. This is currently the only image that provides a GUI.
-
-### Standalone Stable Version
-
-CadQuery was built to be used as a Python library without any GUI. This makes it great for use cases such as integration into servers, or creating scientific and engineering scripts. Use Anaconda/Miniconda to install CadQuery, and then add `import cadquery` to the top of your Python scripts. If the stable version of CadQuery is desired, the following command will install it. However, be aware that the stable version can fall significantly behind the current state of CadQuery, so in many cases the `master` installation method at the beginning of the Getting Started section is preferable.
-
-```
-conda install -c conda-forge -c cadquery cadquery=2
-```
 
 ## Getting help
 
 You can find the full CadQuery documentation at [cadquery.readthedocs.io](https://cadquery.readthedocs.io/).
 
 We also have a [Google Group](https://groups.google.com/forum/#!forum/cadquery) to make it easy to get help from other CadQuery users. We want you to feel welcome and encourage you to join the group and introduce yourself. We would also love to hear what you are doing with CadQuery.
 
@@ -212,15 +142,15 @@
 
 Hexidor is an expanded take on the Quoridor board game, and the development process has been chronicled [here](https://bruceisonfire.net/2020/04/23/my-adventure-with-flosscad-the-birth-of-hexidor/). CadQuery was used to generate the game board. Thanks to Bruce for this example.
 
 <img src="https://bruceisonfire.net/wp-content/uploads/2020/04/16-945x709.jpg" alt="Hexidor Board Game" width="400"/>
 
 ### Spindle assembly
 
-Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example). 
+Thanks to @marcus7070 for this example from [here](https://github.com/marcus7070/spindle-assy-example).
 
 <img src="./doc/_static/assy.png" width="400">
 
 ### 3D Printed Resin Mold
 
 Thanks to @eddieliberato for sharing [this example](https://jungletools.blogspot.com/2017/06/an-anti-kink-device-for-novel-high-tech.html) of an anti-kink resin mold for a cable.
```

### Comparing `cadquery-2.2.0b2/cadquery.egg-info/SOURCES.txt` & `cadquery-2.3.0/cadquery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 doc/_static/quickstart-5.png
 doc/_static/quickstart.png
 doc/_static/simple_assy.png
 doc/_static/simpleblock.png
 doc/_static/tables.css
 doc/_static/vtk.js
 doc/_static/importexport/box_custom_options.svg
+doc/_static/importexport/box_custom_options_perspective.svg
 doc/_static/importexport/box_default_options.svg
 doc/_static/logo/README.md
 doc/_static/logo/cadquery_logo_dark.svg
 doc/_static/logo/cadquery_logo_dark_inkscape.svg
 doc/_static/logo/cadquery_logo_light.svg
 doc/_static/logo/cadquery_logo_light_inkscape.svg
 doc/_static/logo/Roboto_Font/LICENSE.txt
```

### Comparing `cadquery-2.2.0b2/changes.md` & `cadquery-2.3.0/changes.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,53 @@
 Changes
 =======
 
-master
+2.3.0 (latest release)
 ------
+
+### Highlights
+   * Explicit Python 3.11 support [#1247](https://github.com/CadQuery/cadquery/pull/1247) [#1280](https://github.com/CadQuery/cadquery/pull/1280)
+
+ ### Experimental Features
+   * Constraint-based sketches are still being worked on and improved, and are not production ready. There have been fixes, but multiple issues are still open including [#959](https://github.com/CadQuery/cadquery/issues/959), [#968](https://github.com/CadQuery/cadquery/issues/968) and [#960](https://github.com/CadQuery/cadquery/issues/960).
+   * The Convex Hull feature should also be considered experimental. Issues open for that feature include [#931](https://github.com/CadQuery/cadquery/issues/931), [#1190](https://github.com/CadQuery/cadquery/issues/1190), [#1224](https://github.com/CadQuery/cadquery/issues/1224) and [#943](https://github.com/CadQuery/cadquery/issues/943).
+
+ ### Other changes
+   * Various documentation fixes and updates [#1250](https://github.com/CadQuery/cadquery/pull/1250) [#1251](https://github.com/CadQuery/cadquery/pull/1251) [#1256](https://github.com/CadQuery/cadquery/pull/1256) [#1262](https://github.com/CadQuery/cadquery/pull/1262) [#1305](https://github.com/CadQuery/cadquery/pull/1305) [#1306](https://github.com/CadQuery/cadquery/pull/1306) [#1309](https://github.com/CadQuery/cadquery/pull/1309) [#1240](https://github.com/CadQuery/cadquery/pull/1340)
+   * Added a `close` option to `Wire.makePolygon()` [#1257](https://github.com/CadQuery/cadquery/pull/1257)
+   * Fixed iteration over entities and avoid hash collisions to help solve intermittent test failures [#1260](https://github.com/CadQuery/cadquery/pull/1260)
+   * Added fused export for assemblies that preserves face colors [#1261](https://github.com/CadQuery/cadquery/pull/1261)
+   * Added multilayer support to DXF export [#1267](https://github.com/CadQuery/cadquery/pull/1267)
+   * Removed one unneeded layer of hierarchy from STEP export [#1270](https://github.com/CadQuery/cadquery/pull/1270)
+   * Fixed a bug where `Workplane.close()` would not work with a set of 3D points [#1271](https://github.com/CadQuery/cadquery/pull/1271)
+   * Fixed a missing `distance` parameter in an extrude example [#1275](https://github.com/CadQuery/cadquery/pull/1275)
+   * Started building noarch packages in Azure Pipelines [#1293](https://github.com/CadQuery/cadquery/pull/1293)
+   * Added a better version string to identify conda master builds [#1315](https://github.com/CadQuery/cadquery/pull/1315)
+   * Fixed metadata being lost when adding a subassembly to an assembly [#1327](https://github.com/CadQuery/cadquery/pull/1327)
+   * Added tolerance (`tol`) to enable fuzzy `cut()` and `intersect()` operations [#1332](https://github.com/CadQuery/cadquery/pull/1332)
+   * Fixed relative/absolute bug in `line_point` sketch solver method [#1336](https://github.com/CadQuery/cadquery/pull/1336)
+
+2.2.0
+------
+   ### Highlights
+   * Introduced a new Sketch API dedicated to 2D planar operations.
+   * New constraint types were added to use with the Assembly solver.
+
    ### Breaking changes
-   * Renamed the argument for `Workplane.extrude` from `distance` to `until` and `Workplane.cutBlind`'s `distanceToCut` also to `until`. This is only a breaking change if you use the named parameters, i.e. `extrude(distance = 10.0)` or `cutBlind(distanceToCut)` instead of using positional them as positional parameters.
+   * Renamed the argument for `Workplane.extrude` from `distance` to `until` and `Workplane.cutBlind`'s `distanceToCut` also to `until`. This is only a breaking change if you use the named parameters, i.e. `extrude(distance = 10.0)` or `cutBlind(distanceToCut)` instead of using them as positional parameters.
    * Fixed a bug in `Mixin1DProtocol.tangentAt()` where `paramAt()` was being called twice. This should only break scripts that relied on the incorrect behavior. [#641](https://github.com/CadQuery/cadquery/pull/641)
    * `each` and `eachpoint` accept now `combine` argument defaulted to `True` [#954](https://github.com/CadQuery/cadquery/pull/954). This only affects use cases involving solids.
 
+   ### Experimental Features
+   * Constraint-based sketches are still being worked on and improved, and are not production ready. There are multiple issues open including [#1127](https://github.com/CadQuery/cadquery/issues/1127), [#959](https://github.com/CadQuery/cadquery/issues/959), [#968](https://github.com/CadQuery/cadquery/issues/968) and [#960](https://github.com/CadQuery/cadquery/issues/960).
+   * The Convex Hull feature should also be considered experimental. Issues open for that feature include [#931](https://github.com/CadQuery/cadquery/issues/931), [#1190](https://github.com/CadQuery/cadquery/issues/1190), [#1224](https://github.com/CadQuery/cadquery/issues/1224) and [#943](https://github.com/CadQuery/cadquery/issues/943).
+
    ### Other changes
    * Combine option can be set to "cut" (or "s") resulting in a subtractive operation [#954](https://github.com/CadQuery/cadquery/pull/954)
-   * Documentation updates [#648](https://github.com/CadQuery/cadquery/pull/648) [#654](https://github.com/CadQuery/cadquery/pull/654) [#656](https://github.com/CadQuery/cadquery/pull/656) [#659](https://github.com/CadQuery/cadquery/pull/659) [#668](https://github.com/CadQuery/cadquery/pull/668) [#689](https://github.com/CadQuery/cadquery/pull/689) [#695](https://github.com/CadQuery/cadquery/pull/695) [#699](https://github.com/CadQuery/cadquery/pull/699) [#711](https://github.com/CadQuery/cadquery/pull/711) [#727](https://github.com/CadQuery/cadquery/pull/727) [#733](https://github.com/CadQuery/cadquery/pull/733) [#734](https://github.com/CadQuery/cadquery/pull/734) [#737](https://github.com/CadQuery/cadquery/pull/737) [#738](https://github.com/CadQuery/cadquery/pull/738) [#748](https://github.com/CadQuery/cadquery/pull/748) [#757](https://github.com/CadQuery/cadquery/pull/757) [#774](https://github.com/CadQuery/cadquery/pull/774) [#775](https://github.com/CadQuery/cadquery/pull/775) [#805](https://github.com/CadQuery/cadquery/pull/805) [#813](https://github.com/CadQuery/cadquery/pull/813) [#837](https://github.com/CadQuery/cadquery/pull/837) [#839](https://github.com/CadQuery/cadquery/pull/839) [#843](https://github.com/CadQuery/cadquery/pull/843) [#845](https://github.com/CadQuery/cadquery/pull/845) [#846](https://github.com/CadQuery/cadquery/pull/846) [#847](https://github.com/CadQuery/cadquery/pull/847) [#848](https://github.com/CadQuery/cadquery/pull/848) [#852](https://github.com/CadQuery/cadquery/pull/852) [#863](https://github.com/CadQuery/cadquery/pull/863) [#866](https://github.com/CadQuery/cadquery/pull/866) [#867](https://github.com/CadQuery/cadquery/pull/867) [#887](https://github.com/CadQuery/cadquery/pull/887) [#908](https://github.com/CadQuery/cadquery/pull/908) [#910](https://github.com/CadQuery/cadquery/pull/910) [#912] (https://github.com/CadQuery/cadquery/pull/912) [#921](https://github.com/CadQuery/cadquery/pull/921)
+   * Documentation updates [#648](https://github.com/CadQuery/cadquery/pull/648) [#654](https://github.com/CadQuery/cadquery/pull/654) [#656](https://github.com/CadQuery/cadquery/pull/656) [#659](https://github.com/CadQuery/cadquery/pull/659) [#668](https://github.com/CadQuery/cadquery/pull/668) [#689](https://github.com/CadQuery/cadquery/pull/689) [#695](https://github.com/CadQuery/cadquery/pull/695) [#699](https://github.com/CadQuery/cadquery/pull/699) [#711](https://github.com/CadQuery/cadquery/pull/711) [#727](https://github.com/CadQuery/cadquery/pull/727) [#733](https://github.com/CadQuery/cadquery/pull/733) [#734](https://github.com/CadQuery/cadquery/pull/734) [#737](https://github.com/CadQuery/cadquery/pull/737) [#738](https://github.com/CadQuery/cadquery/pull/738) [#748](https://github.com/CadQuery/cadquery/pull/748) [#757](https://github.com/CadQuery/cadquery/pull/757) [#774](https://github.com/CadQuery/cadquery/pull/774) [#775](https://github.com/CadQuery/cadquery/pull/775) [#805](https://github.com/CadQuery/cadquery/pull/805) [#813](https://github.com/CadQuery/cadquery/pull/813) [#837](https://github.com/CadQuery/cadquery/pull/837) [#839](https://github.com/CadQuery/cadquery/pull/839) [#843](https://github.com/CadQuery/cadquery/pull/843) [#845](https://github.com/CadQuery/cadquery/pull/845) [#846](https://github.com/CadQuery/cadquery/pull/846) [#847](https://github.com/CadQuery/cadquery/pull/847) [#848](https://github.com/CadQuery/cadquery/pull/848) [#852](https://github.com/CadQuery/cadquery/pull/852) [#863](https://github.com/CadQuery/cadquery/pull/863) [#866](https://github.com/CadQuery/cadquery/pull/866) [#867](https://github.com/CadQuery/cadquery/pull/867) [#887](https://github.com/CadQuery/cadquery/pull/887) [#908](https://github.com/CadQuery/cadquery/pull/908) [#910](https://github.com/CadQuery/cadquery/pull/910) [#912](https://github.com/CadQuery/cadquery/pull/912) [#921](https://github.com/CadQuery/cadquery/pull/921)
    * Added better documentation on the internals of CadQuery [#821](https://github.com/CadQuery/cadquery/pull/821)
    * Added documentation for assembly constraints [#850](https://github.com/CadQuery/cadquery/pull/850)
    * Bugfix for center option of functions such as box and rect [#617](https://github.com/CadQuery/cadquery/pull/617)
    * Fixes for DXF import [#630](https://github.com/CadQuery/cadquery/pull/630)
    * Updated to OCCT 7.5 [#633](https://github.com/CadQuery/cadquery/pull/633) [#818](https://github.com/CadQuery/cadquery/pull/818)
    * Added ability to specify arbitrary tangents in `spline()` [#636](https://github.com/CadQuery/cadquery/pull/636)
    * Added `forConstruction` option to `offset2D()` [#639](https://github.com/CadQuery/cadquery/pull/639)
@@ -53,17 +86,65 @@
    * Made the loading of the VTK modules more efficient and less error prone [#918](https://github.com/CadQuery/cadquery/pull/918)
    * Changes to allow any cq.Shape to be a sweep path [#919](https://github.com/CadQuery/cadquery/pull/919)
    * Improved edge rendering quality in the documentation [#920](https://github.com/CadQuery/cadquery/pull/920)
    * Properly initialized metadata in Assembly instances [#928](https://github.com/CadQuery/cadquery/pull/928)
    * Fixed bug in ArcAngle Sketch constraint [#932](https://github.com/CadQuery/cadquery/pull/932)
    * Implemented tag merging when performing boolean operations [#934](https://github.com/CadQuery/cadquery/pull/934)
    * Fixed a bug where the height and width were switched in the Sketch rect call [#939](https://github.com/CadQuery/cadquery/pull/939)
+   * Made Face.makeFromWires check that wires are closed to prevent a certain class of segfault [#946](https://github.com/CadQuery/cadquery/pull/946)
+   * Added __repr__ to plane object to get nicer output when converted to a string [#952](https://github.com/CadQuery/cadquery/pull/952)
+   * Added `cut` option to `combine` parameter which removes material from the context solid [#954](https://github.com/CadQuery/cadquery/pull/954)
+   * Updated the dependencies for OCP 7.5.3 [#956](https://github.com/CadQuery/cadquery/pull/956)
+   * Added a fixed arc length cost to the sketch solver [#962](https://github.com/CadQuery/cadquery/pull/962)
+   * Fixed installation doc to use rst instead of markdown [#974](https://github.com/CadQuery/cadquery/pull/974)
+   * Reworked the assembly solder and added PointOnLine, FixedPoint, FixedAxis and FixedRotation assembly constraints [#975](https://github.com/CadQuery/cadquery/pull/975)
+   * Implemented Python 3.10 support [#978](https://github.com/CadQuery/cadquery/pull/978)
+   * Updated conda related sections in the README and docs [#980](https://github.com/CadQuery/cadquery/pull/980)
+   * Added rotateAboutCenter regression test [#982](https://github.com/CadQuery/cadquery/pull/982)
+   * Use `TopTools_ListOfShape` in `assembleEdges()` to prevent some classes of invalid surfaces due to unclosed wires [#986](https://github.com/CadQuery/cadquery/pull/986)
+   * Removed the pinned hdf dependency [#992](https://github.com/CadQuery/cadquery/pull/992)
+   * Fixed bug with extra translation being applied when `rarray` is used with `push` [#994](https://github.com/CadQuery/cadquery/pull/994)
+   * Added a conda web installer for Windows and Linux [#1000](https://github.com/CadQuery/cadquery/pull/1000)
+   * Multiple parray Sketch fixes [#1005](https://github.com/CadQuery/cadquery/pull/1005)
+   * Additional surface modelling functionality [#1007](https://github.com/CadQuery/cadquery/pull/1007)
+   * Fixed a bug with `polarArray` start angle and rotation [#1016](https://github.com/CadQuery/cadquery/pull/1016)
+   * Fixed a bug where Sketch.distribute was creating an extra location [#1018](https://github.com/CadQuery/cadquery/pull/1018)
+   * Fixed the screw holes in the parametric enclosure example [#1023](https://github.com/CadQuery/cadquery/pull/1023)
+   * Switched to nptyping 2.x [#1050](https://github.com/CadQuery/cadquery/pull/1050)
+   * Ability to specify DXF layer names [#1061](https://github.com/CadQuery/cadquery/pull/1061)
+   * Switch to Casadi and iPOPT for assembly solver [#1063](https://github.com/CadQuery/cadquery/pull/1063)
+   * Added adjustment parameters for linear and angular tolerances in VRML tessellation [#1066](https://github.com/CadQuery/cadquery/pull/1066)
+   * Pinned VTK to 9.0.1 for OCP 7.5.3 [#1075](https://github.com/CadQuery/cadquery/pull/1075)
+   * Fixed VTK-based assembly export rotation issue [#1078](https://github.com/CadQuery/cadquery/pull/1078)
+   * Added quality controls to STEP export for shapes and assemblies [#1083](https://github.com/CadQuery/cadquery/pull/1083)
+   * Updated setup.py for OCP being available on PyPI [#1085](https://github.com/CadQuery/cadquery/pull/1085)
+   * Added Sphinx customization for multimethod handling [#1088](https://github.com/CadQuery/cadquery/pull/1088) [#1123](https://github.com/CadQuery/cadquery/pull/1123)
+   * Pinned the nptyping version [#1095](https://github.com/CadQuery/cadquery/pull/1095) [#1096](https://github.com/CadQuery/cadquery/pull/1096)
+   * Added STL to Assembly export formats [#1101](https://github.com/CadQuery/cadquery/pull/1101)
+   * Updated the mutlimethod version pin [#1118](https://github.com/CadQuery/cadquery/pull/1118)
+   * Reworked the cheatsheet [#1129](https://github.com/CadQuery/cadquery/pull/1129)
+   * Pass clean to eachpoint in box, cylinder, interpPlate, sphere and wedge [#1145](https://github.com/CadQuery/cadquery/pull/1145)
+   * Moved to OCCT 7.6 [#1156](https://github.com/CadQuery/cadquery/pull/1156)
+   * Do not add a leaf component when assembly shapes are empty [#993](https://github.com/CadQuery/cadquery/pull/1157)
+   * Fixed an indexing bug in tessellation [#1163](https://github.com/CadQuery/cadquery/pull/1163)
+   * Pinned cadquery-ocp version to 7.6.* [#1164](https://github.com/CadQuery/cadquery/pull/1164)
+   * Disabled recompute of normals when converting to VTK [#1167](https://github.com/CadQuery/cadquery/pull/1167)
+   * Added Fixed to ConstraintKinds type definition [#1177](https://github.com/CadQuery/cadquery/pull/1177)
+   * Added option to control the verbosity of the assembly solver [#1198](https://github.com/CadQuery/cadquery/pull/1198)
+   * Only show deprecation warning when required [#1201](https://github.com/CadQuery/cadquery/pull/1201)
+   * Untangled indirect exports [#1204](https://github.com/CadQuery/cadquery/pull/1204)
+   * Added parameter and return types to `importDXF` [#1205](https://github.com/CadQuery/cadquery/pull/1205)
+   * Fixed incorrect coordinate system in glTF exports [#1211](https://github.com/CadQuery/cadquery/pull/1211)
+   * Updated to allow OCP 7.7.0 to be used [#1215](https://github.com/CadQuery/cadquery/pull/1215)
+   * Fixed VTK HTML template [#1216](https://github.com/CadQuery/cadquery/pull/1216) [#1217](https://github.com/CadQuery/cadquery/pull/1217)
+   * Cleaned up environment.yml file [#1233](https://github.com/CadQuery/cadquery/pull/1233)
+   * Various documentation fixes [#1033](https://github.com/CadQuery/cadquery/pull/1033) [#1041](https://github.com/CadQuery/cadquery/pull/1041) [#1044](https://github.com/CadQuery/cadquery/pull/1044) [#1049](https://github.com/CadQuery/cadquery/pull/1049) [#1056](https://github.com/CadQuery/cadquery/pull/1056) [#1058](https://github.com/CadQuery/cadquery/pull/1058) [#1059](https://github.com/CadQuery/cadquery/pull/1059) [#1060](https://github.com/CadQuery/cadquery/pull/1060) [#1062](https://github.com/CadQuery/cadquery/pull/1062) [#1079](https://github.com/CadQuery/cadquery/pull/1079) [#1089](https://github.com/CadQuery/cadquery/pull/1089) [#1116](https://github.com/CadQuery/cadquery/pull/1116) [#1140](https://github.com/CadQuery/cadquery/pull/1140) [#1143](https://github.com/CadQuery/cadquery/pull/1143) [#1151](https://github.com/CadQuery/cadquery/pull/1151) [#1166](https://github.com/CadQuery/cadquery/pull/1166) [#1176](https://github.com/CadQuery/cadquery/pull/1176) [#1207](https://github.com/CadQuery/cadquery/pull/1207) [#1210](https://github.com/CadQuery/cadquery/pull/1210) [#1241](https://github.com/CadQuery/cadquery/pull/1241)
 
 
-2.1 (stable release)
+2.1
 ------
    ### Breaking changes
    * Fixed bug in ParallelDirSelector where non-planar faces could be selected. Note this will be breaking if you've used DirectionNthSelector and a non-planar face made it into your object list. In that case eg. ">X[2]" will have to become ">X[1]".
 
    ### Other changes
    * Refactored selectors and added CenterNthSelector [#549](https://github.com/CadQuery/cadquery/pull/549)
    * Added new installation video links to the readme [#550](https://github.com/CadQuery/cadquery/pull/550)
```

### Comparing `cadquery-2.2.0b2/conda/meta.yaml` & `cadquery-2.3.0/conda/meta.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,31 @@
   name: cadquery
   version:  {{ environ.get('PACKAGE_VERSION') }}
 
 source:
   path: ..
 
 build:
-  string: {{ 'py'+environ.get('PYTHON_VERSION')}}
+  string: {{ GIT_DESCRIBE_TAG }}_{{ GIT_BUILD_STR }}
+  noarch: python
   script: python setup.py install --single-version-externally-managed --record=record.txt
 
 requirements:
   build:
-    - python {{ environ.get('PYTHON_VERSION') }}
+    - python >=3.8
     - setuptools
   run:
-    - python {{ environ.get('PYTHON_VERSION') }}
-    - ocp 7.6.*
+    - python >=3.8
+    - ocp 7.7.0
+    - occt 7.7.0
     - pyparsing >=2.1.9
     - ezdxf
     - ipython
     - typing_extensions
-    - nptyping 2.0.1
+    - nptyping >=2.0.1
     - nlopt
     - multimethod >=1.7,<2.0
     - casadi
 
 test:
   requires:
     - pytest
```

### Comparing `cadquery-2.2.0b2/conda/web-installer/Readme.md` & `cadquery-2.3.0/conda/web-installer/Readme.md`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/conda/web-installer/build.py` & `cadquery-2.3.0/conda/web-installer/build.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/conda/web-installer/construct.yaml.jinja2` & `cadquery-2.3.0/conda/web-installer/construct.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/ParametricPulley.PNG` & `cadquery-2.3.0/doc/_static/ParametricPulley.PNG`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/assy.png` & `cadquery-2.3.0/doc/_static/assy.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/block.png` & `cadquery-2.3.0/doc/_static/block.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/cadquery_cheatsheet.html` & `cadquery-2.3.0/doc/_static/cadquery_cheatsheet.html`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
 						<th style="width:40%;">Selects</th>
 						<th style="width:10%;"># Objects Returned</th>
 					</tr>
 					<tr>
 						<td>&#43;Z</td>
 						<td>DirectionSelector</td>
 						<td>Faces with normal in +z direction</td>
-						<td>0 or 1</td>
+						<td>0..many</td>
 					</tr>
 					<tr>
 						<td>&#124;Z</td>
 						<td>ParallelDirSelector</td>
 						<td>Faces parallel to xy plane</td>
 						<td>0..many</td>
 					</tr>
@@ -649,8 +649,8 @@
 	}
 
 	window.onload = () => {	
 		if(getCookie("dark") == "1") {
 			enableDark()
 		}
 	}
-</script>
+</script>
```

#### html2text {}

```diff
@@ -113,15 +113,15 @@
 ***** Examples of Filtering Faces *****
 
 All types of filters work on faces. In most cases, the selector refers to the
 direction of the normal vector of the face. If a face is not planar, selectors
 are evaluated at the center of mass of the face. This can lead to results that
 are quite unexpected.
 Selector Selector Class           Selects                    # Objects Returned
-+Z       DirectionSelector        Faces with normal in +z    0 or 1
++Z       DirectionSelector        Faces with normal in +z    0..many
                                   direction
 |Z       ParallelDirSelector      Faces parallel to xy plane 0..many
 -X       DirectionSelector        Faces with normal in neg x 0..many
                                   direction
 #Z       PerpendicularDirSelector Faces perpendicular to z   0..many
                                   direction
 %Plane   TypeSelector             Faces of type plane        0..many
@@ -154,7 +154,8 @@
 Only a few of the filter types apply to vertices. The location of the vertex is
 the subject of the filter.
 Selector Selector Class          Selects
 >Y       DirectionMinMaxSelector Vertices farthest in the +Y dir
 <Y       DirectionMinMaxSelector Vertices farthest in the -Y dir
 >>Y[-2]  CenterNthSelector       2nd farthest vertex in the +Y dir
 <<Y[0]   CenterNthSelector       1st closest vertex in the Y dir
+
```

### Comparing `cadquery-2.2.0b2/doc/_static/door_assy.png` & `cadquery-2.3.0/doc/_static/door_assy.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/door_assy_freecad.png` & `cadquery-2.3.0/doc/_static/door_assy_freecad.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/hyOzd-cablefix.png` & `cadquery-2.3.0/doc/_static/hyOzd-cablefix.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/hyOzd-finished.jpg` & `cadquery-2.3.0/doc/_static/hyOzd-finished.jpg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/importexport/box_custom_options.svg` & `cadquery-2.3.0/doc/_static/importexport/box_custom_options.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/importexport/box_default_options.svg` & `cadquery-2.3.0/doc/_static/importexport/box_default_options.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/Roboto_Font/LICENSE.txt` & `cadquery-2.3.0/doc/_static/logo/Roboto_Font/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/Roboto_Font/Roboto-Bold.ttf` & `cadquery-2.3.0/doc/_static/logo/Roboto_Font/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_dark.svg` & `cadquery-2.3.0/doc/_static/logo/cadquery_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_dark_inkscape.svg` & `cadquery-2.3.0/doc/_static/logo/cadquery_logo_dark_inkscape.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_light.svg` & `cadquery-2.3.0/doc/_static/logo/cadquery_logo_light.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/logo/cadquery_logo_light_inkscape.svg` & `cadquery-2.3.0/doc/_static/logo/cadquery_logo_light_inkscape.svg`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/new_badge.png` & `cadquery-2.3.0/doc/_static/new_badge.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/parametric-cup-screencap.PNG` & `cadquery-2.3.0/doc/_static/parametric-cup-screencap.PNG`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/parametric-pillowblock-screencap.png` & `cadquery-2.3.0/doc/_static/parametric-pillowblock-screencap.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/pillowblock.png` & `cadquery-2.3.0/doc/_static/pillowblock.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/000.png` & `cadquery-2.3.0/doc/_static/quickstart/000.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/001.png` & `cadquery-2.3.0/doc/_static/quickstart/001.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/002.png` & `cadquery-2.3.0/doc/_static/quickstart/002.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/003.png` & `cadquery-2.3.0/doc/_static/quickstart/003.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/004.png` & `cadquery-2.3.0/doc/_static/quickstart/004.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart/005.png` & `cadquery-2.3.0/doc/_static/quickstart/005.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart-1.png` & `cadquery-2.3.0/doc/_static/quickstart-1.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart-2.png` & `cadquery-2.3.0/doc/_static/quickstart-2.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart-3.png` & `cadquery-2.3.0/doc/_static/quickstart-3.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart-4.png` & `cadquery-2.3.0/doc/_static/quickstart-4.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart-5.png` & `cadquery-2.3.0/doc/_static/quickstart-5.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/quickstart.png` & `cadquery-2.3.0/doc/_static/quickstart.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/simple_assy.png` & `cadquery-2.3.0/doc/_static/simple_assy.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/simpleblock.png` & `cadquery-2.3.0/doc/_static/simpleblock.png`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/_static/vtk.js` & `cadquery-2.3.0/doc/_static/vtk.js`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/apireference.rst` & `cadquery-2.3.0/doc/apireference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     Workplane.exportSvg
 
 
 .. autosummary::
     importers.importStep
     importers.importDXF
     exporters.export
+    occ_impl.exporters.dxf.DxfDocument
 
 
 Iteration Methods
 ------------------
 
 Methods that allow iteration over the stack or objects
```

### Comparing `cadquery-2.2.0b2/doc/assy.rst` & `cadquery-2.3.0/doc/assy.rst`

 * *Files 0% similar despite different names*

```diff
@@ -366,16 +366,14 @@
 
 .. code-block:: python
    :linenos:
 
     door.save('door.step')
     door.save('door.xml')
     
-In the case of STEP colors are preserved but not transparency.
-
 ..  image:: _static/door_assy_freecad.png
 
 
 Object locations
 ----------------
 
 Objects can be added to an assembly with initial locations supplied, such as:
@@ -385,17 +383,17 @@
     import cadquery as cq
 
     cone = cq.Solid.makeCone(1, 0, 2)
 
     assy = cq.Assembly()
     assy.add(
         cone,
-        loc=cq.Location(cq.Vector(0, 0, 0), cq.Vector(1, 0, 0), 180),
+        loc=cq.Location((0, 0, 0), (1, 0, 0), 180),
         name="cone0",
-        color=cq.Color("green")
+        color=cq.Color("green"),
     )
     assy.add(cone, name="cone1", color=cq.Color("blue"))
 
     show_object(assy)
 
 
 As an alternative to the user calculating locations, constraints and the method
@@ -729,29 +727,29 @@
   line :math:`b`.
 
 
 .. cadquery::
 
     import cadquery as cq
 
-    b1 = cq.Workplane().box(1,1,1)
+    b1 = cq.Workplane().box(1, 1, 1)
     b2 = cq.Workplane().sphere(0.15)
 
     assy = (
         cq.Assembly()
-        .add(b1,name='b1')
-        .add(b2, loc=cq.Location(cq.Vector(0,0,4)), name='b2', color=cq.Color('red'))
+        .add(b1, name="b1")
+        .add(b2, loc=cq.Location((0, 0, 4)), name="b2", color=cq.Color("red"))
     )
 
     # fix the position of b1
-    assy.constrain('b1','Fixed')
+    assy.constrain("b1", "Fixed")
     # b2 on one of the edges of b1
-    assy.constrain('b2','b1@edges@>>Z and >>Y','PointOnLine')
+    assy.constrain("b2", "b1@edges@>>Z and >>Y", "PointOnLine")
     # b2 on another of the edges of b1
-    assy.constrain('b2','b1@edges@>>Z and >>X','PointOnLine')
+    assy.constrain("b2", "b1@edges@>>Z and >>X", "PointOnLine")
     # effectively b2 will be constrained to be on the intersection of the two edges
 
     assy.solve()
     show_object(assy)
 
 
 FixedPoint
@@ -764,48 +762,48 @@
 
    \left\lVert \vec{ c } - \vec{param} \right\rVert ^2
 
 
 Where:
 
 - :math:`\vec{ c }` is the center of the argument,
-- :math:`param` is the parameter of the constraint - tuple specifying the target position,
-- :math:`\operatorname{dist}( \vec{ a }, b)` is the distance between point :math:`\vec{ a }` and
-  line :math:`b`.
+- :math:`param` is the parameter of the constraint - tuple specifying the target position.
 
 
 .. cadquery::
 
     import cadquery as cq
 
-    b1 = cq.Workplane().box(1,1,1)
+    b1 = cq.Workplane().box(1, 1, 1)
     b2 = cq.Workplane().sphere(0.15)
 
     assy = (
         cq.Assembly()
-        .add(b1,name='b1')
-        .add(b2, loc=cq.Location(cq.Vector(0,0,4)), name='b2', color=cq.Color('red'))
+        .add(b1, name="b1")
+        .add(b2, loc=cq.Location((0, 0, 4)), name="b2", color=cq.Color("red"))
+        .add(b1, loc=cq.Location((-2, 0, 0)), name="b3", color=cq.Color("red"))
     )
 
+    pnt = (0.5, 0.5, 0.5)
+
     # fix the position of b1
-    assy.constrain('b1','Fixed')
-    # b2 on one of the edges of b1
-    assy.constrain('b2','b1@edges@>>Z and >>Y','PointOnLine')
-    # b2 on another of the edges of b1
-    assy.constrain('b2','b1@edges@>>Z and >>X','PointOnLine')
-    # effectively b2 will be constrained to be on the intersection of the two edges
+    assy.constrain("b1", "Fixed")
+    # fix b2 center at point
+    assy.constrain("b2", "FixedPoint", pnt)
+    # fix b3 vertex position at point
+    assy.constrain("b3@vertices@<X and <Y and <Z", "FixedPoint", pnt)
 
     assy.solve()
     show_object(assy)
 
 
 FixedRotation
 =============
 
-FixedRotation fixes the rotation of the given argument to be equal to the value specified via the parameter of the constraint. The argument is rotated about it's origin firstly by the Z angle, then Y and finally X.
+FixedRotation fixes the rotation of the given argument to be equal to the value specified via the parameter of the constraint.
 
 This constraint locks all rotational degrees of freedom of the argument.
 The cost function is:
 
 .. math::
 
    \left\lVert \vec{ R } - \vec{param} \right\rVert ^2
@@ -817,29 +815,29 @@
 - :math:`param` is the parameter of the constraint - tuple specifying the target rotation.
 
 
 .. cadquery::
 
     import cadquery as cq
 
-    b1 = cq.Workplane().box(1,1,1)
-    b2 = cq.Workplane().rect(0.1, 0.1).extrude(1,taper=-15)
+    b1 = cq.Workplane().box(1, 1, 1)
+    b2 = cq.Workplane().rect(0.1, 0.1).extrude(1, taper=-15)
 
     assy = (
         cq.Assembly()
-        .add(b1,name='b1')
-        .add(b2, loc=cq.Location(cq.Vector(0,0,4)), name='b2', color=cq.Color('red'))
+        .add(b1, name="b1")
+        .add(b2, loc=cq.Location((0, 0, 4)), name="b2", color=cq.Color("red"))
     )
 
     # fix the position of b1
-    assy.constrain('b1','Fixed')
+    assy.constrain("b1", "Fixed")
     # fix b2 bottom face position (but not rotation)
-    assy.constrain('b2@faces@<Z','FixedPoint',(0,0,0.5))
+    assy.constrain("b2@faces@<Z", "FixedPoint", (0, 0, 0.5))
     # fix b2 rotational degrees of freedom too
-    assy.constrain('b2','FixedRotation',(45,0,45))
+    assy.constrain("b2", "FixedRotation", (45, 0, 45))
 
     assy.solve()
     show_object(assy)
 
 
 FixedAxis
 =========
@@ -858,29 +856,29 @@
 - :math:`param` is the parameter of the constraint - tuple specifying the target direction.
 
 
 .. cadquery::
 
     import cadquery as cq
 
-    b1 = cq.Workplane().box(1,1,1)
-    b2 = cq.Workplane().rect(0.1, 0.1).extrude(1,taper=-15)
+    b1 = cq.Workplane().box(1, 1, 1)
+    b2 = cq.Workplane().rect(0.1, 0.1).extrude(1, taper=-15)
 
     assy = (
         cq.Assembly()
-        .add(b1,name='b1')
-        .add(b2, loc=cq.Location(cq.Vector(0,0,4)), name='b2', color=cq.Color('red'))
+        .add(b1, name="b1")
+        .add(b2, loc=cq.Location((0, 0, 4)), name="b2", color=cq.Color("red"))
     )
 
     # fix the position of b1
-    assy.constrain('b1','Fixed')
+    assy.constrain("b1", "Fixed")
     # fix b2 bottom face position (but not rotation)
-    assy.constrain('b2@faces@<Z','FixedPoint',(0,0,0.5))
+    assy.constrain("b2@faces@<Z", "FixedPoint", (0, 0, 0.5))
     # fix b2 some rotational degrees of freedom too
-    assy.constrain('b2@faces@>Z','FixedAxis',(1,0,2))
+    assy.constrain("b2@faces@>Z", "FixedAxis", (1, 0, 2))
 
     assy.solve()
     show_object(assy)
 
 
 Assembly colors
 ---------------
```

### Comparing `cadquery-2.2.0b2/doc/classreference.rst` & `cadquery-2.3.0/doc/classreference.rst`

 * *Files 12% similar despite different names*

```diff
@@ -95,7 +95,14 @@
 .. automodule:: cadquery.selectors
    :show-inheritance: 
    :members:
 
 .. automodule:: cadquery.occ_impl.exporters.assembly
    :show-inheritance:
    :members:
+
+.. autofunction:: cadquery.occ_impl.assembly.toJSON
+
+.. autoclass:: cadquery.occ_impl.exporters.dxf.DxfDocument
+   :members:
+
+   .. automethod:: __init__
```

### Comparing `cadquery-2.2.0b2/doc/conf.py` & `cadquery-2.3.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosummary",
+    "sphinx.ext.intersphinx",
     "cadquery.cq_directive",
     "sphinx.ext.mathjax",
     "sphinx_autodoc_multimethod",
 ]
 
 autodoc_typehints = "both"
 autodoc_typehints_description_target = "all"
@@ -63,17 +64,17 @@
 copyright = "Parametric Products Intellectual Holdings LLC, All Rights Reserved"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "1.0"
+version = "2.3"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.0"
+release = "2.3.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -208,14 +209,19 @@
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "CadQuerydoc"
 
+# -- Options for intersphinx --------------------------------------------------
+
+intersphinx_mapping = {
+    "ezdxf-stable": ("https://ezdxf.readthedocs.io/en/stable/", None),
+}
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
```

### Comparing `cadquery-2.2.0b2/doc/cqgi.rst` & `cadquery-2.3.0/doc/cqgi.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/designprinciples.rst` & `cadquery-2.3.0/doc/designprinciples.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/examples.rst` & `cadquery-2.3.0/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/ext/sphinx_autodoc_multimethod.py` & `cadquery-2.3.0/doc/ext/sphinx_autodoc_multimethod.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/extending.rst` & `cadquery-2.3.0/doc/extending.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/fileformat.rst` & `cadquery-2.3.0/doc/fileformat.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/gen_colors.py` & `cadquery-2.3.0/doc/gen_colors.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/importexport.rst` & `cadquery-2.3.0/doc/importexport.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .. _importexport:
+.. py:currentmodule:: cadquery
 
 ******************************
 Importing and Exporting Files
 ******************************
 
 Introduction
 #############
@@ -41,63 +42,184 @@
 * TJS is short for ThreeJS, and is a JSON mesh format that is useful for displaying 3D models in web browsers. The TJS format is used to display embedded 3D examples within the CadQuery documentation.
 * VRML is a mesh-based format for representing interactive 3D objects in a web browser.
 * VTP is a mesh-based format used by the VTK library.
 
 Importing DXF
 ##############
 
-DXF files can be imported using the :py:meth:`importers.importDXF` method.
+DXF files can be imported using the :meth:`importers.importDXF` method.
 
 .. automethod::
-    cadquery.importers.importDXF
+    importers.importDXF
 
 Importing a DXF profile with default settings and using it within a CadQuery script is shown in the following code.
 
 .. code-block:: python
 
     import cadquery as cq
 
     result = (
-        cq.importers.importDXF('/path/to/dxf/circle.dxf')
-        .wires().toPending()
-        .extrude(10)
-        )
+        cq.importers.importDXF("/path/to/dxf/circle.dxf").wires().toPending().extrude(10)
+    )
 
-Note the use of the :py:meth:`Workplane.wires` and :py:meth:`Workplane.toPending` methods to make the DXF profile 
+Note the use of the :meth:`Workplane.wires` and :meth:`Workplane.toPending` methods to make the DXF profile
 ready for use during subsequent operations. Calling ``toPending()`` tells CadQuery to make the edges/wires available 
 to the next modelling operation that is called in the chain.
 
 Importing STEP
 ###############
 
-STEP files can be imported using the :py:meth:`importers.importStep` method (note the capitalization of "Step"). 
+STEP files can be imported using the :meth:`importers.importStep` method (note the capitalization of "Step").
 There are no parameters for this method other than the file path to import.
 
 .. code-block:: python
 
     import cadquery as cq
 
     result = cq.importers.importStep('/path/to/step/block.stp')
 
+Exporting STEP
+###############
+
+This section covers exporting CadQuery Workplane objects to STEP. For exporting assemblies to STEP, see the next section.
+
+Default
+--------
+
+The exporters module handles exporting Workplane objects to STEP. It is not necessary to set the export type explicitly
+since it will be determined from the file extension. Below is an example.
+
+.. code-block:: python
+
+    # Create a simple object
+    box = cq.Workplane().box(10, 10, 10)
+
+    # Export the box
+    cq.exporters.export(box, "/path/to/step/box.step")
+
+Non-Default File Extensions
+----------------------------
+
+If there is a requirement to export the STEP file using an "stp" extension, CadQuery will throw an error saying that it does
+not recognize the file extension. In that case the export type has to be specified.
+
+.. code-block:: python
+
+    # Create a simple object
+    box = cq.Workplane().box(10, 10, 10)
+
+    # Export the box
+    cq.exporters.export(box, "/path/to/step/box.stp", cq.exporters.ExportTypes.STEP)
+
+    # The export type may also be specified as a literal
+    cq.exporters.export(box, "/path/to/step/box2.stp", "STEP")
+
+Setting Extra Options
+----------------------
+
+There are additional options that can be set when exporting an object to a STEP file.
+For an explanation of the options available, see the documentation of the :meth:`Shape.exportStep` method
+or the :meth:`Assembly.exportAssembly`` method.
+
+.. code-block:: python
+
+    # Create a simple object
+    box = cq.Workplane().box(10, 10, 10)
+
+    # Export the box, provide additional options with the opt dict
+    cq.exporters.export(box, "/path/to/step/box.step", opt={"write_pcurves": False})
+
+    # or equivalently when exporting a lower level Shape object
+    box.val().exportStep("/path/to/step/box2.step", write_pcurves=False)
+
+
+Exporting Assemblies to STEP
+#############################
+
+It is possible to export CadQuery assemblies directly to STEP. The STEP exporter has multiple options which change the way
+exported STEP files will appear and operate when opened in other CAD programs. All assembly export methods shown here will
+preserve the color information from the assembly.
+
+Default
+--------
+
+CadQuery assemblies have a :meth:`Assembly.save` method which can write an assembly to a STEP file. An example assembly
+export with all defaults is shown below.
+
+.. code-block:: python
+
+    import cadquery as cq
+
+    # Create a sample assembly
+    assy = cq.Assembly()
+    body = cq.Workplane().box(10, 10, 10)
+    assy.add(body, color=cq.Color(1, 0, 0), name="body")
+    pin = cq.Workplane().center(2, 2).cylinder(radius=2, height=20)
+    assy.add(pin, color=cq.Color(0, 1, 0), name="pin")
+
+    # Save the assembly to STEP
+    assy.save('out.step')
+
+This will produce a STEP file that is nested with auto-generated object names. The colors of each assembly object will be
+preserved, but the names that were set for each will not.
+
+Fused
+------
+
+The following will attempt to create a single, fused shape while preserving the name and color information of each assembly
+object. The process of fusing the solid may cause performance issues in some cases, and is likely to alter the faces of the
+fused solids.
+
+.. code-block:: python
+
+    import cadquery as cq
+
+    # Create a sample assembly
+    assy = cq.Assembly()
+    body = cq.Workplane().box(10, 10, 10)
+    assy.add(body, color=cq.Color(1, 0, 0), name="body")
+    pin = cq.Workplane().center(2, 2).cylinder(radius=2, height=20)
+    assy.add(pin, color=cq.Color(0, 1, 0), name="pin")
+
+    # Save the assembly to STEP
+    assy.save("out.stp", "STEP", mode="fused")
+
+    # Specify additional options such as glue as keyword arguments
+    assy.save("out_glue.step", mode="fused", glue=True, write_pcurves=False)
+
+Naming
+-------
+
+It is also possible to set the name of the top level assembly object in the STEP file with either the DEFAULT or FUSED methods.
+This is done by setting the name property of the assembly before calling :meth:`Assembly.save`.
+
+.. code-block:: python
+
+    assy = Assembly(name="my_assembly")
+    assy.save("out.stp", cq.exporters.ExportTypes.STEP, mode=cq.exporters.assembly.ExportModes.FUSED)
+
+If an assembly name is not specified, a UUID will be used to avoid name conflicts.
+
 Exporting SVG
-##############
+###############
 
 The SVG exporter has several options which can be useful for achieving the desired final output. Those 
 options are as follows.
 
 * *width* - Document width of the resulting image.
 * *height* - Document height of the resulting image.
 * *marginLeft* - Inset margin from the left side of the document.
 * *marginTop* - Inset margin from the top side of the document.
 * *projectionDir* - Direction the camera will view the shape from.
 * *showAxes* - Whether or not to show the axes indicator, which will only be visible when the projectionDir is also at the default.
 * *strokeWidth* - Width of the line that visible edges are drawn with.
 * *strokeColor* - Color of the line that visible edges are drawn with.
 * *hiddenColor* - Color of the line that hidden edges are drawn with.
 * *showHidden* - Whether or not to show hidden lines.
+* *focus* - If specified, creates a perspective SVG with the projector at the distance specified.
 
 The options are passed to the exporter in a dictionary, and can be left out to force the SVG to be created with default options. 
 Below are examples with and without options set.
 
 Without options:
 
 .. code-block:: python
@@ -142,14 +264,18 @@
                 },
             )
 
 Which results in the following image:
 
 ..  image:: _static/importexport/box_custom_options.svg
 
+Exporting with the additional option ``"focus": 25`` results in the following output SVG with perspective:
+
+.. image:: _static/importexport/box_custom_options_perspective.svg
+
 Exporting STL
 ##############
 
 The STL exporter is capable of adjusting the quality of the resulting mesh, and accepts the following parameters.
 
 .. automethod::
     cadquery.occ_impl.shapes.Shape.exportStl
@@ -229,14 +355,114 @@
     import cadquery as cq
     from cadquery import exporters
 
     result = cq.Workplane().box(10, 10, 10)
 
     exporters.export(result, '/path/to/file/mesh.vrml', tolerance=0.01, angularTolerance=0.1)
 
+Exporting DXF
+##############
+
+.. seealso::
+
+    :class:`cadquery.occ_impl.exporters.dxf.DxfDocument` for exporting multiple
+    Workplanes to one or many layers of a DXF document.
+
+Options
+-------
+
+``approx``
+    Approximation strategy for converting :class:`cadquery.Workplane` objects to DXF entities:
+
+        ``None``
+            no approximation applied
+        ``"spline"``
+            all splines approximated as cubic splines
+        ``"arc"``
+            all curves approximated as arcs and straight segments
+``tolerance``
+    Approximation tolerance for converting :class:`cadquery.Workplane` objects to DXF entities.
+    See `Approximation strategy`_.
+``doc_units``
+    Ezdxf document/modelspace :doc:`units <ezdxf-stable:concepts/units>`.
+    See `Units`_.
+
+.. code-block:: python
+    :caption: DXF document without options.
+
+    import cadquery as cq
+    from cadquery import exporters
+
+    result = cq.Workplane().box(10, 10, 10)
+
+    exporters.exportDXF(result, "/path/to/file/object.dxf")
+    # or
+    exporters.export(result, "/path/to/file/object.dxf")
+
+
+Units
+-----
+
+The default DXF document units are mm (:code:`doc_units = 4`).
+
+========= ===============
+doc_units Unit
+========= ===============
+0         Unitless
+1         Inches
+2         Feet
+3         Miles
+4         Millimeters
+5         Centimeters
+6         Meters
+========= ===============
+
+Document units can be set to any :doc:`unit supported by ezdxf <ezdxf-stable:concepts/units>`.
+
+.. code-block:: python
+    :caption: DXF document with units set to meters.
+
+    import cadquery as cq
+    from cadquery import exporters
+
+    result = cq.Workplane().box(10, 10, 10)
+
+    exporters.exportDXF(
+        result, "/path/to/file/object.dxf", doc_units=6,  # set DXF document units to meters
+    )
+
+    # or
+
+    exporters.export(
+        result,
+        "/path/to/file/object.dxf",
+        opt={"doc_units": 6},  # set DXF document units to meters
+    )
+
+
+.. _Approximation strategy:
+
+Approximation strategy
+----------------------
+
+By default, the DXF exporter will output splines exactly as they are represented by the OpenCascade kernel. Unfortunately some software cannot handle higher-order splines resulting in missing curves after DXF import. To resolve this, specify an approximation strategy controlled by the following options:
+
+* ``approx`` - ``None``, ``"spline"`` or ``"arc"``. ``"spline"`` results in all splines approximated with cubic splines. ``"arc"`` results in all curves approximated with arcs and line segments.
+* ``tolerance``: Acceptable error of the approximation, in document/modelspace units. Defaults to 0.001 (1 thou for inch-scale drawings, 1 µm for mm-scale drawings).
+
+.. code-block:: python
+    :caption: DXF document with curves approximated with cubic splines.
+
+    cq.exporters.exportDXF(
+        result,
+        "/path/to/file/object.dxf",
+        approx="spline"
+    )
+
+
 Exporting Other Formats
 ########################
 
 The remaining export formats do not accept any additional parameters other than file name, and can be exported 
 using the following structure.
 
 .. code-block:: python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cadquery-2.2.0b2/doc/index.rst` & `cadquery-2.3.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/intro.rst` & `cadquery-2.3.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/primer.rst` & `cadquery-2.3.0/doc/primer.rst`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 ---------------------------
 
 Most of the time, you are building a single object, and adding features to that single object.  CadQuery watches
 your operations, and defines the first solid object created as the 'context solid'.  After that, any features
 you create are automatically combined (unless you specify otherwise) with that solid.  This happens even if the
 solid was created  a long way up in the stack.  For example::
 
-    Workplane('XY').box(1,2,3).faces(">Z").circle(0.25).extrude()
+    Workplane('XY').box(1,2,3).faces(">Z").circle(0.25).extrude(1)
 
 Will create a 1x2x3 box, with a cylindrical boss extending from the top face.  It was not necessary to manually
 combine the cylinder created by extruding the circle with the box, because the default behavior for extrude is
 to combine the result with the context solid. The hole() method works similarly -- CadQuery presumes that you want
 to subtract the hole from the context solid.
 
 If you want to avoid this, you can specify ``combine=False``, and CadQuery will create the solid separately.
```

### Comparing `cadquery-2.2.0b2/doc/quickstart.rst` & `cadquery-2.3.0/doc/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 CadQuery QuickStart
 ***********************
 
 .. currentmodule:: cadquery
 
 Want a quick glimpse of what CadQuery can do?  This quickstart will demonstrate the basics of CadQuery using a simple example
 
-Prerequisites: conda + CQ-editor running from an environment
-==============================================================
+Prerequisites: CadQuery and CQ-editor installation
+==================================================
 
-If you have not already done so, follow the :ref:`installation`, to install conda and CQ-editor.
+If you have not already done so, follow the :ref:`installation`, to install CadQuery and CQ-editor.
 
 After installation, run CQ-editor:
 
 ..  image:: _static/quickstart/001.png
 
 Find the CadQuery code editor, on the left side.  You'll see that we start out with the script for a simple block.
 
@@ -41,15 +41,15 @@
 Hopefully our finished script will not be too much more complex than this human-oriented description.
 
 Let's see how we do.
 
 Start With A single, simple Plate
 ======================================
 
-Lets start with a simple model that makes nothing but a rectangular block, but
+Let's start with a simple model that makes nothing but a rectangular block, but
 with place-holders for the dimensions. Paste this into the code editor:
 
 .. code-block:: python
    :linenos:
 
     height = 60.0
     width = 80.0
@@ -92,15 +92,15 @@
     show_object(result)
 
 Rebuild your model by clicking the Render button. Your block should look like this:
 
 ..  image:: _static/quickstart/003.png
 
 
-The code is pretty compact, lets step through it.
+The code is pretty compact, let's step through it.
 
 **Line 4** adds a new parameter, diameter, for the diameter of the hole
 
 **Line 8**, we're adding the hole.
 :py:meth:`cadquery.Workplane.faces` selects the top-most face in the Z direction, and then
 :py:meth:`cadquery.Workplane.workplane` begins a new workplane located on this face. The center of this workplane
 is located at the center of mass of the shape, which in this case is the center of the plate.
@@ -152,15 +152,15 @@
 
 
 After clicking the Render button to re-execute the model, you should see something like this:
 
         ..  image:: _static/quickstart/004.png
 
 
-There is quite a bit going on here, so lets break it down a bit.
+There is quite a bit going on here, so let's break it down a bit.
 
 **Line 5** creates a new padding parameter that decides how far the holes are from the edges of the plate.
 
 **Line 10** selects the top-most face of the block, and creates a workplane on the top of that face, which we'll use to
 define the centers of the holes in the corners.
 
 There are a couple of things to note about this line:
```

### Comparing `cadquery-2.2.0b2/doc/roadmap.rst` & `cadquery-2.3.0/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/selectors.rst` & `cadquery-2.3.0/doc/selectors.rst`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/doc/sketch.rst` & `cadquery-2.3.0/doc/sketch.rst`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 Once the construction is finished it has to be converted to the face-based representation
 using :meth:`~cadquery.Sketch.assemble`. Afterwards, face based operations can be applied.
 
 
 Convex hull
 ===========
 
+.. warning:: The Convex Hull feature is currently experimental.
+
 For certain special use-cases convex hull can be constructed from straight segments
 and circles.
 
 .. cadquery::
     :height: 600px
 
     result = (
@@ -100,14 +102,16 @@
         .segment((0.,2),(-1,3.))
         .hull()
        )
 
 Constraint-based sketches
 =========================
 
+.. warning:: The 2D Sketch constraints and solver is currently experimental.
+
 Finally, if desired, geometric constraints can be used to construct sketches. So
 far only line segments and arcs can be used in such a use case.
 
 .. cadquery::
     :height: 600px
 
     import cadquery as cq
```

### Comparing `cadquery-2.2.0b2/doc/vslot-2020_1.dxf` & `cadquery-2.3.0/doc/vslot-2020_1.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/CQ examples.ipynb` & `cadquery-2.3.0/examples/CQ examples.ipynb`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex001_Simple_Block.py` & `cadquery-2.3.0/examples/Ex001_Simple_Block.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex002_Block_With_Bored_Center_Hole.py` & `cadquery-2.3.0/examples/Ex002_Block_With_Bored_Center_Hole.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex003_Pillow_Block_With_Counterbored_Holes.py` & `cadquery-2.3.0/examples/Ex003_Pillow_Block_With_Counterbored_Holes.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex004_Extruded_Cylindrical_Plate.py` & `cadquery-2.3.0/examples/Ex004_Extruded_Cylindrical_Plate.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex005_Extruded_Lines_and_Arcs.py` & `cadquery-2.3.0/examples/Ex005_Extruded_Lines_and_Arcs.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex006_Moving_the_Current_Working_Point.py` & `cadquery-2.3.0/examples/Ex006_Moving_the_Current_Working_Point.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex007_Using_Point_Lists.py` & `cadquery-2.3.0/examples/Ex007_Using_Point_Lists.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex008_Polygon_Creation.py` & `cadquery-2.3.0/examples/Ex008_Polygon_Creation.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex009_Polylines.py` & `cadquery-2.3.0/examples/Ex009_Polylines.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex010_Defining_an_Edge_with_a_Spline.py` & `cadquery-2.3.0/examples/Ex010_Defining_an_Edge_with_a_Spline.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex011_Mirroring_Symmetric_Geometry.py` & `cadquery-2.3.0/examples/Ex011_Mirroring_Symmetric_Geometry.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex012_Creating_Workplanes_on_Faces.py` & `cadquery-2.3.0/examples/Ex012_Creating_Workplanes_on_Faces.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex013_Locating_a_Workplane_on_a_Vertex.py` & `cadquery-2.3.0/examples/Ex013_Locating_a_Workplane_on_a_Vertex.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex014_Offset_Workplanes.py` & `cadquery-2.3.0/examples/Ex014_Offset_Workplanes.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex015_Rotated_Workplanes.py` & `cadquery-2.3.0/examples/Ex015_Rotated_Workplanes.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex016_Using_Construction_Geometry.py` & `cadquery-2.3.0/examples/Ex016_Using_Construction_Geometry.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex017_Shelling_to_Create_Thin_Features.py` & `cadquery-2.3.0/examples/Ex017_Shelling_to_Create_Thin_Features.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex018_Making_Lofts.py` & `cadquery-2.3.0/examples/Ex018_Making_Lofts.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex019_Counter_Sunk_Holes.py` & `cadquery-2.3.0/examples/Ex019_Counter_Sunk_Holes.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex020_Rounding_Corners_with_Fillets.py` & `cadquery-2.3.0/examples/Ex020_Rounding_Corners_with_Fillets.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex021_Splitting_an_Object.py` & `cadquery-2.3.0/examples/Ex021_Splitting_an_Object.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex022_Revolution.py` & `cadquery-2.3.0/examples/Ex022_Revolution.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex023_Sweep.py` & `cadquery-2.3.0/examples/Ex023_Sweep.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex024_Sweep_With_Multiple_Sections.py` & `cadquery-2.3.0/examples/Ex024_Sweep_With_Multiple_Sections.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex025_Swept_Helix.py` & `cadquery-2.3.0/examples/Ex025_Swept_Helix.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex026_Case_Seam_Lip.py` & `cadquery-2.3.0/examples/Ex026_Case_Seam_Lip.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex100_Lego_Brick.py` & `cadquery-2.3.0/examples/Ex100_Lego_Brick.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/examples/Ex101_InterpPlate.py` & `cadquery-2.3.0/examples/Ex101_InterpPlate.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/mypy.ini` & `cadquery-2.3.0/mypy.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [mypy]
 ignore_missing_imports = False
 disable_error_code = no-redef
 
 [mypy-ezdxf.*]
 ignore_missing_imports = True
+no_implicit_optional = False
 
 [mypy-pyparsing.*]
 ignore_missing_imports = True
 
 [mypy-IPython.*]
 ignore_missing_imports = True
```

### Comparing `cadquery-2.2.0b2/setup.py` & `cadquery-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,43 +17,42 @@
 reqs = []
 setup_reqs = []
 
 # ReadTheDocs, AppVeyor and Azure builds will break when trying to instal pip deps in a conda env
 is_rtd = "READTHEDOCS" in os.environ
 is_appveyor = "APPVEYOR" in os.environ
 is_azure = "CONDA_PY" in os.environ
+is_conda = "CONDA_PREFIX_1" in os.environ
 
-# Only include the installation dependencies if we are not running on RTD or AppVeyor
-if not is_rtd and not is_appveyor and not is_azure:
+# Only include the installation dependencies if we are not running on RTD or AppVeyor or in a conda env
+if not is_rtd and not is_appveyor and not is_azure and not is_conda:
     reqs = [
-        "cadquery-ocp>=7.6,<7.7",
+        "cadquery-ocp>=7.7.0a0,<7.8",
         "ezdxf",
         "multimethod>=1.7,<2.0",
         "nlopt",
         "nptyping==2.0.1",
         "typish",
         "casadi",
         "path",
     ]
 
-    setup_reqs = ["setuptools_scm"]
 
 setup(
     name="cadquery",
-    version="2.2.0b2",
-    # use_scm_version=True,
+    version="2.3.0",  # Update this for the next release
     url="https://github.com/CadQuery/cadquery",
     license="Apache Public License 2.0",
     author="David Cowden",
     author_email="dave.cowden@gmail.com",
     description="CadQuery is a parametric  scripting language for creating and traversing CAD models",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8",
     setup_requires=setup_reqs,
     install_requires=reqs,
     extras_require={
         "dev": ["docutils", "ipython", "pytest", "black==19.10b0", "click==8.0.4",],
         "ipython": ["ipython",],
     },
     include_package_data=True,
```

### Comparing `cadquery-2.2.0b2/tests/__init__.py` & `cadquery-2.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/naca.py` & `cadquery-2.3.0/tests/naca.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_cad_objects.py` & `cadquery-2.3.0/tests/test_cad_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # system modules
 import math
+import pytest
 import unittest
 from tests import BaseTest
 from OCP.gp import gp_Vec, gp_Pnt, gp_Ax2, gp_Circ, gp_Elips, gp, gp_XYZ, gp_Trsf
 from OCP.BRepBuilderAPI import BRepBuilderAPI_MakeEdge
 
 from cadquery import *
 
@@ -717,9 +718,22 @@
                 Edge.makeCircle(1.0, angle1=0, angle2=180),
                 Edge.makeCircle(3.0, pnt=Vector(2, 0, 0), angle1=180, angle2=359),
             ]
         )
         self.assertAlmostEqual(many_rad.radius(), 1.0)
 
 
+@pytest.mark.parametrize(
+    "points, close, expected_edges",
+    [
+        (((0, 0, 0), (0, 1, 0), (1, 0, 0)), False, 2),
+        (((0, 0, 0), (0, 1, 0), (1, 0, 0)), True, 3),
+        (((0, 0, 0), (0, 1, 0), (1, 0, 0), (0, 0, 0)), False, 3),
+        (((0, 0, 0), (0, 1, 0), (1, 0, 0), (0, 0, 0)), True, 3),
+    ],
+)
+def test_wire_makepolygon(points, close, expected_edges):
+    assert len(Wire.makePolygon(points, False, close).Edges()) == expected_edges
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cadquery-2.2.0b2/tests/test_cadquery.py` & `cadquery-2.3.0/tests/test_cadquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -7623,3899 +7623,4034 @@
 0001dc60: 5472 7565 292e 6369 7263 6c65 2830 2e35  True).circle(0.5
 0001dc70: 292e 6578 7472 7564 6528 342c 2063 6f6d  ).extrude(4, com
 0001dc80: 6269 6e65 3d22 6375 7422 290a 2020 2020  bine="cut").    
 0001dc90: 2020 2020 7365 6c66 2e61 7373 6572 7447      self.assertG
 0001dca0: 7265 6174 6572 2862 6f78 2e76 616c 2829  reater(box.val()
 0001dcb0: 2e56 6f6c 756d 6528 292c 2072 2e76 616c  .Volume(), r.val
 0001dcc0: 2829 2e56 6f6c 756d 6528 2929 0a0a 2020  ().Volume())..  
-0001dcd0: 2020 6465 6620 7465 7374 5461 7065 7265    def testTapere
-0001dce0: 6445 7874 7275 6465 4375 7442 6c69 6e64  dExtrudeCutBlind
-0001dcf0: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
-0001dd00: 2068 203d 2031 2e30 0a20 2020 2020 2020   h = 1.0.       
-0001dd10: 2072 203d 2031 2e30 0a20 2020 2020 2020   r = 1.0.       
-0001dd20: 2074 203d 2035 0a0a 2020 2020 2020 2020   t = 5..        
-0001dd30: 2320 6578 7472 7564 6520 7769 7468 2061  # extrude with a
-0001dd40: 2070 6f73 6974 6976 6520 7461 7065 720a   positive taper.
-0001dd50: 2020 2020 2020 2020 7320 3d20 576f 726b          s = Work
-0001dd60: 706c 616e 6528 2258 5922 292e 6369 7263  plane("XY").circ
-0001dd70: 6c65 2872 292e 6578 7472 7564 6528 682c  le(r).extrude(h,
-0001dd80: 2074 6170 6572 3d74 290a 0a20 2020 2020   taper=t)..     
-0001dd90: 2020 2074 6f70 5f66 6163 6520 3d20 732e     top_face = s.
-0001dda0: 6661 6365 7328 223e 5a22 290a 2020 2020  faces(">Z").    
-0001ddb0: 2020 2020 626f 7474 6f6d 5f66 6163 6520      bottom_face 
-0001ddc0: 3d20 732e 6661 6365 7328 223c 5a22 290a  = s.faces("<Z").
-0001ddd0: 0a20 2020 2020 2020 2023 2074 6f70 2061  .        # top a
-0001dde0: 6e64 2062 6f74 746f 6d20 6661 6365 2061  nd bottom face a
-0001ddf0: 7265 610a 2020 2020 2020 2020 6465 6c74  rea.        delt
-0001de00: 6120 3d20 746f 705f 6661 6365 2e76 616c  a = top_face.val
-0001de10: 2829 2e41 7265 6128 2920 2d20 626f 7474  ().Area() - bott
-0001de20: 6f6d 5f66 6163 652e 7661 6c28 292e 4172  om_face.val().Ar
-0001de30: 6561 2829 0a0a 2020 2020 2020 2020 7365  ea()..        se
-0001de40: 6c66 2e61 7373 6572 7454 7275 6528 6465  lf.assertTrue(de
-0001de50: 6c74 6120 3c20 3029 0a0a 2020 2020 2020  lta < 0)..      
-0001de60: 2020 2320 6578 7472 7564 6520 7769 7468    # extrude with
-0001de70: 2061 206e 6567 6174 6976 6520 7461 7065   a negative tape
-0001de80: 720a 2020 2020 2020 2020 7320 3d20 576f  r.        s = Wo
-0001de90: 726b 706c 616e 6528 2258 5922 292e 6369  rkplane("XY").ci
-0001dea0: 7263 6c65 2872 292e 6578 7472 7564 6528  rcle(r).extrude(
-0001deb0: 682c 2074 6170 6572 3d2d 7429 0a0a 2020  h, taper=-t)..  
-0001dec0: 2020 2020 2020 746f 705f 6661 6365 203d        top_face =
-0001ded0: 2073 2e66 6163 6573 2822 3e5a 2229 0a20   s.faces(">Z"). 
-0001dee0: 2020 2020 2020 2062 6f74 746f 6d5f 6661         bottom_fa
-0001def0: 6365 203d 2073 2e66 6163 6573 2822 3c5a  ce = s.faces("<Z
-0001df00: 2229 0a0a 2020 2020 2020 2020 2320 746f  ")..        # to
-0001df10: 7020 616e 6420 626f 7474 6f6d 2066 6163  p and bottom fac
-0001df20: 6520 6172 6561 0a20 2020 2020 2020 2064  e area.        d
-0001df30: 656c 7461 203d 2074 6f70 5f66 6163 652e  elta = top_face.
-0001df40: 7661 6c28 292e 4172 6561 2829 202d 2062  val().Area() - b
-0001df50: 6f74 746f 6d5f 6661 6365 2e76 616c 2829  ottom_face.val()
-0001df60: 2e41 7265 6128 290a 0a20 2020 2020 2020  .Area()..       
-0001df70: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0001df80: 2864 656c 7461 203e 2030 290a 0a20 2020  (delta > 0)..   
-0001df90: 2020 2020 2023 2063 7574 2061 2074 6170       # cut a tap
-0001dfa0: 6572 6564 2068 6f6c 650a 2020 2020 2020  ered hole.      
-0001dfb0: 2020 7320 3d20 280a 2020 2020 2020 2020    s = (.        
-0001dfc0: 2020 2020 576f 726b 706c 616e 6528 2258      Workplane("X
-0001dfd0: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
-0001dfe0: 2e72 6563 7428 3220 2a20 722c 2032 202a  .rect(2 * r, 2 *
-0001dff0: 2072 290a 2020 2020 2020 2020 2020 2020   r).            
-0001e000: 2e65 7874 7275 6465 2832 202a 2068 290a  .extrude(2 * h).
-0001e010: 2020 2020 2020 2020 2020 2020 2e66 6163              .fac
-0001e020: 6573 2822 3e5a 2229 0a20 2020 2020 2020  es(">Z").       
-0001e030: 2020 2020 202e 776f 726b 706c 616e 6528       .workplane(
-0001e040: 290a 2020 2020 2020 2020 2020 2020 2e72  ).            .r
-0001e050: 6563 7428 722c 2072 290a 2020 2020 2020  ect(r, r).      
-0001e060: 2020 2020 2020 2e63 7574 426c 696e 6428        .cutBlind(
-0001e070: 2d68 2c20 7461 7065 723d 7429 0a20 2020  -h, taper=t).   
-0001e080: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001e090: 6d69 6464 6c65 5f66 6163 6520 3d20 732e  middle_face = s.
-0001e0a0: 6661 6365 7328 223e 5a5b 2d32 5d22 290a  faces(">Z[-2]").
-0001e0b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001e0c0: 7365 7274 5472 7565 286d 6964 646c 655f  sertTrue(middle_
-0001e0d0: 6661 6365 2e76 616c 2829 2e41 7265 6128  face.val().Area(
-0001e0e0: 2920 3c20 3129 0a0a 2020 2020 6465 6620  ) < 1)..    def 
-0001e0f0: 7465 7374 436c 6f73 6528 7365 6c66 293a  testClose(self):
-0001e100: 0a20 2020 2020 2020 2023 2043 6c6f 7365  .        # Close
-0001e110: 2077 6974 686f 7574 2065 6e64 506f 696e   without endPoin
-0001e120: 7420 616e 6420 7374 6172 7450 6f69 6e74  t and startPoint
-0001e130: 2063 6f69 6e63 6964 652e 0a20 2020 2020   coincide..     
-0001e140: 2020 2023 2043 7265 6174 6520 6120 6861     # Create a ha
-0001e150: 6c66 2d63 6972 636c 650a 2020 2020 2020  lf-circle.      
-0001e160: 2020 6120 3d20 576f 726b 706c 616e 6528    a = Workplane(
-0001e170: 506c 616e 652e 5859 2829 292e 7361 6769  Plane.XY()).sagi
-0001e180: 7474 6141 7263 2828 3130 2c20 3029 2c20  ttaArc((10, 0), 
-0001e190: 3229 2e63 6c6f 7365 2829 2e65 7874 7275  2).close().extru
-0001e1a0: 6465 2832 290a 0a20 2020 2020 2020 2023  de(2)..        #
-0001e1b0: 2043 6c6f 7365 2077 6865 6e20 656e 6450   Close when endP
-0001e1c0: 6f69 6e74 2061 6e64 2073 7461 7274 506f  oint and startPo
-0001e1d0: 696e 7420 636f 696e 6369 6465 2e0a 2020  int coincide..  
-0001e1e0: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-0001e1f0: 2064 6f75 626c 6520 6861 6c66 2d63 6972   double half-cir
-0001e200: 636c 650a 2020 2020 2020 2020 6220 3d20  cle.        b = 
-0001e210: 280a 2020 2020 2020 2020 2020 2020 576f  (.            Wo
-0001e220: 726b 706c 616e 6528 506c 616e 652e 5859  rkplane(Plane.XY
-0001e230: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-0001e240: 2e73 6167 6974 7461 4172 6328 2831 302c  .sagittaArc((10,
-0001e250: 2030 292c 2032 290a 2020 2020 2020 2020   0), 2).        
-0001e260: 2020 2020 2e73 6167 6974 7461 4172 6328      .sagittaArc(
-0001e270: 2830 2c20 3029 2c20 3229 0a20 2020 2020  (0, 0), 2).     
-0001e280: 2020 2020 2020 202e 636c 6f73 6528 290a         .close().
-0001e290: 2020 2020 2020 2020 2020 2020 2e65 7874              .ext
-0001e2a0: 7275 6465 2832 290a 2020 2020 2020 2020  rude(2).        
-0001e2b0: 290a 0a20 2020 2020 2020 2023 2054 6865  )..        # The
-0001e2c0: 2062 2073 6861 7065 2073 6861 6c6c 2068   b shape shall h
-0001e2d0: 6176 6520 7477 6963 6520 7468 6520 766f  ave twice the vo
-0001e2e0: 6c75 6d65 206f 6620 7468 6520 6120 7368  lume of the a sh
-0001e2f0: 6170 652e 0a20 2020 2020 2020 2073 656c  ape..        sel
-0001e300: 662e 6173 7365 7274 416c 6d6f 7374 4571  f.assertAlmostEq
-0001e310: 7561 6c28 612e 7661 6c28 292e 566f 6c75  ual(a.val().Volu
-0001e320: 6d65 2829 202a 2032 2e30 2c20 622e 7661  me() * 2.0, b.va
-0001e330: 6c28 292e 566f 6c75 6d65 2829 290a 0a20  l().Volume()).. 
-0001e340: 2020 2020 2020 2023 2054 6573 7463 6173         # Testcas
-0001e350: 6520 3320 6672 6f6d 2069 7373 7565 2023  e 3 from issue #
-0001e360: 3233 380a 2020 2020 2020 2020 7468 6963  238.        thic
-0001e370: 6b6e 6573 7320 3d20 332e 300a 2020 2020  kness = 3.0.    
-0001e380: 2020 2020 6c65 6e67 7468 203d 2031 302e      length = 10.
-0001e390: 300a 2020 2020 2020 2020 7769 6474 6820  0.        width 
-0001e3a0: 3d20 352e 300a 0a20 2020 2020 2020 206f  = 5.0..        o
-0001e3b0: 626a 3120 3d20 280a 2020 2020 2020 2020  bj1 = (.        
-0001e3c0: 2020 2020 576f 726b 706c 616e 6528 2258      Workplane("X
-0001e3d0: 5922 2c20 6f72 6967 696e 3d28 302c 2030  Y", origin=(0, 0
-0001e3e0: 2c20 2d74 6869 636b 6e65 7373 202f 2032  , -thickness / 2
-0001e3f0: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
-0001e400: 6d6f 7665 546f 286c 656e 6774 6820 2f20  moveTo(length / 
-0001e410: 322c 2030 290a 2020 2020 2020 2020 2020  2, 0).          
-0001e420: 2020 2e74 6872 6565 506f 696e 7441 7263    .threePointArc
-0001e430: 2828 302c 2077 6964 7468 202f 2032 292c  ((0, width / 2),
-0001e440: 2028 2d6c 656e 6774 6820 2f20 322c 2030   (-length / 2, 0
-0001e450: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
-0001e460: 7468 7265 6550 6f69 6e74 4172 6328 2830  threePointArc((0
-0001e470: 2c20 2d77 6964 7468 202f 2032 292c 2028  , -width / 2), (
-0001e480: 6c65 6e67 7468 202f 2032 2c20 3029 290a  length / 2, 0)).
-0001e490: 2020 2020 2020 2020 2020 2020 2e63 6c6f              .clo
-0001e4a0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-0001e4b0: 202e 6578 7472 7564 6528 7468 6963 6b6e   .extrude(thickn
-0001e4c0: 6573 7329 0a20 2020 2020 2020 2029 0a0a  ess).        )..
-0001e4d0: 2020 2020 2020 2020 6f73 5f78 203d 2038          os_x = 8
-0001e4e0: 2e30 2020 2320 4f66 6673 6574 2069 6e20  .0  # Offset in 
-0001e4f0: 580a 2020 2020 2020 2020 6f73 5f79 203d  X.        os_y =
-0001e500: 202d 3139 2e35 2020 2320 4f66 6673 6574   -19.5  # Offset
-0001e510: 2069 6e20 590a 0a20 2020 2020 2020 206f   in Y..        o
-0001e520: 626a 3220 3d20 280a 2020 2020 2020 2020  bj2 = (.        
-0001e530: 2020 2020 576f 726b 706c 616e 6528 2259      Workplane("Y
-0001e540: 5a22 2c20 6f72 6967 696e 3d28 6f73 5f78  Z", origin=(os_x
-0001e550: 2c20 6f73 5f79 2c20 2d74 6869 636b 6e65  , os_y, -thickne
-0001e560: 7373 202f 2032 2929 0a20 2020 2020 2020  ss / 2)).       
-0001e570: 2020 2020 202e 6d6f 7665 546f 286f 735f       .moveTo(os_
-0001e580: 7820 2b20 6c65 6e67 7468 202f 2032 2c20  x + length / 2, 
-0001e590: 6f73 5f79 290a 2020 2020 2020 2020 2020  os_y).          
-0001e5a0: 2020 2e73 6167 6974 7461 4172 6328 286f    .sagittaArc((o
-0001e5b0: 735f 7820 2d20 6c65 6e67 7468 202f 2032  s_x - length / 2
-0001e5c0: 2c20 6f73 5f79 292c 2077 6964 7468 202f  , os_y), width /
-0001e5d0: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-0001e5e0: 2e73 6167 6974 7461 4172 6328 286f 735f  .sagittaArc((os_
-0001e5f0: 7820 2b20 6c65 6e67 7468 202f 2032 2c20  x + length / 2, 
-0001e600: 6f73 5f79 292c 2077 6964 7468 202f 2032  os_y), width / 2
-0001e610: 290a 2020 2020 2020 2020 2020 2020 2e63  ).            .c
-0001e620: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
-0001e630: 2020 202e 6578 7472 7564 6528 7468 6963     .extrude(thic
-0001e640: 6b6e 6573 7329 0a20 2020 2020 2020 2029  kness).        )
-0001e650: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
-0001e660: 6f62 6a31 2073 6861 7065 2073 6861 6c6c  obj1 shape shall
-0001e670: 2068 6176 6520 7468 6520 7361 6d65 2076   have the same v
-0001e680: 6f6c 756d 6520 6173 2074 6865 206f 626a  olume as the obj
-0001e690: 3220 7368 6170 652e 0a20 2020 2020 2020  2 shape..       
-0001e6a0: 2073 656c 662e 6173 7365 7274 416c 6d6f   self.assertAlmo
-0001e6b0: 7374 4571 7561 6c28 6f62 6a31 2e76 616c  stEqual(obj1.val
-0001e6c0: 2829 2e56 6f6c 756d 6528 292c 206f 626a  ().Volume(), obj
-0001e6d0: 322e 7661 6c28 292e 566f 6c75 6d65 2829  2.val().Volume()
-0001e6e0: 290a 0a20 2020 2064 6566 2074 6573 7454  )..    def testT
-0001e6f0: 6578 7428 7365 6c66 293a 0a20 2020 2020  ext(self):.     
-0001e700: 2020 2067 6c6f 6261 6c20 7465 7374 6461     global testda
-0001e710: 7461 4469 720a 0a20 2020 2020 2020 2062  taDir..        b
-0001e720: 6f78 203d 2057 6f72 6b70 6c61 6e65 2822  ox = Workplane("
-0001e730: 5859 2229 2e62 6f78 2834 2c20 342c 2030  XY").box(4, 4, 0
-0001e740: 2e35 290a 0a20 2020 2020 2020 206f 626a  .5)..        obj
-0001e750: 3120 3d20 280a 2020 2020 2020 2020 2020  1 = (.          
-0001e760: 2020 626f 782e 6661 6365 7328 223e 5a22    box.faces(">Z"
-0001e770: 290a 2020 2020 2020 2020 2020 2020 2e77  ).            .w
-0001e780: 6f72 6b70 6c61 6e65 2829 0a20 2020 2020  orkplane().     
-0001e790: 2020 2020 2020 202e 7465 7874 280a 2020         .text(.  
-0001e7a0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
-0001e7b0: 5120 322e 3022 2c0a 2020 2020 2020 2020  Q 2.0",.        
-0001e7c0: 2020 2020 2020 2020 302e 352c 0a20 2020          0.5,.   
-0001e7d0: 2020 2020 2020 2020 2020 2020 202d 302e               -0.
-0001e7e0: 3035 2c0a 2020 2020 2020 2020 2020 2020  05,.            
-0001e7f0: 2020 2020 6375 743d 5472 7565 2c0a 2020      cut=True,.  
-0001e800: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-0001e810: 6c69 676e 3d22 6c65 6674 222c 0a20 2020  lign="left",.   
-0001e820: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0001e830: 6967 6e3d 2262 6f74 746f 6d22 2c0a 2020  ign="bottom",.  
-0001e840: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0001e850: 6e74 3d22 5361 6e73 222c 0a20 2020 2020  nt="Sans",.     
-0001e860: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001e870: 2029 0a0a 2020 2020 2020 2020 2320 636f   )..        # co
-0001e880: 6d62 696e 6564 206f 626a 6563 7420 7368  mbined object sh
-0001e890: 6f75 6c64 2068 6176 6520 736d 616c 6c65  ould have smalle
-0001e8a0: 7220 766f 6c75 6d65 0a20 2020 2020 2020  r volume.       
-0001e8b0: 2073 656c 662e 6173 7365 7274 4772 6561   self.assertGrea
-0001e8c0: 7465 7228 626f 782e 7661 6c28 292e 566f  ter(box.val().Vo
-0001e8d0: 6c75 6d65 2829 2c20 6f62 6a31 2e76 616c  lume(), obj1.val
-0001e8e0: 2829 2e56 6f6c 756d 6528 2929 0a0a 2020  ().Volume())..  
-0001e8f0: 2020 2020 2020 6f62 6a32 203d 2028 0a20        obj2 = (. 
-0001e900: 2020 2020 2020 2020 2020 2062 6f78 2e66             box.f
-0001e910: 6163 6573 2822 3e5a 2229 0a20 2020 2020  aces(">Z").     
-0001e920: 2020 2020 2020 202e 776f 726b 706c 616e         .workplan
-0001e930: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0001e940: 2e74 6578 7428 2243 5120 322e 3022 2c20  .text("CQ 2.0", 
-0001e950: 302e 352c 2030 2e30 352c 2063 7574 3d46  0.5, 0.05, cut=F
-0001e960: 616c 7365 2c20 636f 6d62 696e 653d 5472  alse, combine=Tr
-0001e970: 7565 2c20 666f 6e74 3d22 5361 6e73 2229  ue, font="Sans")
-0001e980: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0001e990: 2020 2020 2320 636f 6d62 696e 6564 206f      # combined o
-0001e9a0: 626a 6563 7420 7368 6f75 6c64 2068 6176  bject should hav
-0001e9b0: 6520 6269 6767 6572 2076 6f6c 756d 650a  e bigger volume.
-0001e9c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001e9d0: 6572 744c 6573 7328 626f 782e 7661 6c28  ertLess(box.val(
-0001e9e0: 292e 566f 6c75 6d65 2829 2c20 6f62 6a32  ).Volume(), obj2
-0001e9f0: 2e76 616c 2829 2e56 6f6c 756d 6528 2929  .val().Volume())
-0001ea00: 0a0a 2020 2020 2020 2020 2320 7665 7269  ..        # veri
-0001ea10: 6679 2074 6861 7420 7468 6520 6e75 6d62  fy that the numb
-0001ea20: 6572 206f 6620 746f 7020 6661 6365 7320  er of top faces 
-0001ea30: 6973 2063 6f72 7265 6374 2028 4e42 3a20  is correct (NB: 
-0001ea40: 7468 6973 2069 7320 666f 6e74 2073 7065  this is font spe
-0001ea50: 6369 6669 6329 0a20 2020 2020 2020 2073  cific).        s
-0001ea60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001ea70: 6c65 6e28 6f62 6a32 2e66 6163 6573 2822  len(obj2.faces("
-0001ea80: 3e5a 2229 2e76 616c 7328 2929 2c20 3529  >Z").vals()), 5)
-0001ea90: 0a0a 2020 2020 2020 2020 6f62 6a33 203d  ..        obj3 =
-0001eaa0: 2028 0a20 2020 2020 2020 2020 2020 2062   (.            b
-0001eab0: 6f78 2e66 6163 6573 2822 3e5a 2229 0a20  ox.faces(">Z"). 
-0001eac0: 2020 2020 2020 2020 2020 202e 776f 726b             .work
-0001ead0: 706c 616e 6528 290a 2020 2020 2020 2020  plane().        
-0001eae0: 2020 2020 2e74 6578 7428 0a20 2020 2020      .text(.     
-0001eaf0: 2020 2020 2020 2020 2020 2022 4351 2032             "CQ 2
-0001eb00: 2e30 222c 0a20 2020 2020 2020 2020 2020  .0",.           
-0001eb10: 2020 2020 2030 2e35 2c0a 2020 2020 2020       0.5,.      
-0001eb20: 2020 2020 2020 2020 2020 302e 3035 2c0a            0.05,.
-0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb40: 6375 743d 4661 6c73 652c 0a20 2020 2020  cut=False,.     
-0001eb50: 2020 2020 2020 2020 2020 2063 6f6d 6269             combi
-0001eb60: 6e65 3d46 616c 7365 2c0a 2020 2020 2020  ne=False,.      
-0001eb70: 2020 2020 2020 2020 2020 6861 6c69 676e            halign
-0001eb80: 3d22 7269 6768 7422 2c0a 2020 2020 2020  ="right",.      
-0001eb90: 2020 2020 2020 2020 2020 7661 6c69 676e            valign
-0001eba0: 3d22 746f 7022 2c0a 2020 2020 2020 2020  ="top",.        
-0001ebb0: 2020 2020 2020 2020 666f 6e74 3d22 5361          font="Sa
-0001ebc0: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
-0001ebd0: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
-0001ebe0: 2020 2020 2020 2320 7665 7269 6679 2074        # verify t
-0001ebf0: 6861 7420 7468 6520 6e75 6d62 6572 206f  hat the number o
-0001ec00: 6620 736f 6c69 6473 2069 7320 636f 7272  f solids is corr
-0001ec10: 6563 740a 2020 2020 2020 2020 7365 6c66  ect.        self
-0001ec20: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-0001ec30: 286f 626a 332e 736f 6c69 6473 2829 2e76  (obj3.solids().v
-0001ec40: 616c 7328 2929 2c20 3529 0a0a 2020 2020  als()), 5)..    
-0001ec50: 2020 2020 6f62 6a34 203d 2028 0a20 2020      obj4 = (.   
-0001ec60: 2020 2020 2020 2020 2062 6f78 2e66 6163           box.fac
-0001ec70: 6573 2822 3e5a 2229 0a20 2020 2020 2020  es(">Z").       
-0001ec80: 2020 2020 202e 776f 726b 706c 616e 6528       .workplane(
-0001ec90: 290a 2020 2020 2020 2020 2020 2020 2e74  ).            .t
-0001eca0: 6578 7428 0a20 2020 2020 2020 2020 2020  ext(.           
-0001ecb0: 2020 2020 2022 4351 2032 2e30 222c 0a20       "CQ 2.0",. 
-0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-0001ecd0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
-0001ece0: 2020 2020 302e 3035 2c0a 2020 2020 2020      0.05,.      
-0001ecf0: 2020 2020 2020 2020 2020 666f 6e74 5061            fontPa
-0001ed00: 7468 3d6f 732e 7061 7468 2e6a 6f69 6e28  th=os.path.join(
-0001ed10: 7465 7374 6461 7461 4469 722c 2022 4f70  testdataDir, "Op
-0001ed20: 656e 5361 6e73 2d52 6567 756c 6172 2e74  enSans-Regular.t
-0001ed30: 7466 2229 2c0a 2020 2020 2020 2020 2020  tf"),.          
-0001ed40: 2020 2020 2020 6375 743d 4661 6c73 652c        cut=False,
-0001ed50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ed60: 2063 6f6d 6269 6e65 3d46 616c 7365 2c0a   combine=False,.
-0001ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed80: 6861 6c69 676e 3d22 7269 6768 7422 2c0a  halign="right",.
-0001ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eda0: 7661 6c69 676e 3d22 746f 7022 2c0a 2020  valign="top",.  
-0001edb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0001edc0: 6e74 3d22 5361 6e73 222c 0a20 2020 2020  nt="Sans",.     
-0001edd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001ede0: 2029 0a0a 2020 2020 2020 2020 2320 7665   )..        # ve
-0001edf0: 7269 6679 2074 6861 7420 7468 6520 6e75  rify that the nu
-0001ee00: 6d62 6572 206f 6620 736f 6c69 6473 2069  mber of solids i
-0001ee10: 7320 636f 7272 6563 740a 2020 2020 2020  s correct.      
-0001ee20: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0001ee30: 616c 286c 656e 286f 626a 342e 736f 6c69  al(len(obj4.soli
-0001ee40: 6473 2829 2e76 616c 7328 2929 2c20 3529  ds().vals()), 5)
-0001ee50: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
-0001ee60: 2074 6f20 7365 6520 6966 206e 6f6e 2d65   to see if non-e
-0001ee70: 7869 7374 656e 7420 6669 6c65 2063 6175  xistent file cau
-0001ee80: 7365 7320 7365 6766 6175 6c74 0a20 2020  ses segfault.   
-0001ee90: 2020 2020 206f 626a 3520 3d20 280a 2020       obj5 = (.  
-0001eea0: 2020 2020 2020 2020 2020 626f 782e 6661            box.fa
-0001eeb0: 6365 7328 223e 5a22 290a 2020 2020 2020  ces(">Z").      
-0001eec0: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
-0001eed0: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-0001eee0: 7465 7874 280a 2020 2020 2020 2020 2020  text(.          
-0001eef0: 2020 2020 2020 2243 5120 322e 3022 2c0a        "CQ 2.0",.
-0001ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef10: 302e 352c 0a20 2020 2020 2020 2020 2020  0.5,.           
-0001ef20: 2020 2020 2030 2e30 352c 0a20 2020 2020       0.05,.     
-0001ef30: 2020 2020 2020 2020 2020 2066 6f6e 7450             fontP
-0001ef40: 6174 683d 6f73 2e70 6174 682e 6a6f 696e  ath=os.path.join
-0001ef50: 2874 6573 7464 6174 6144 6972 2c20 224f  (testdataDir, "O
-0001ef60: 7065 6e53 616e 732d 4972 7265 6775 6c61  penSans-Irregula
-0001ef70: 722e 7474 6622 292c 0a20 2020 2020 2020  r.ttf"),.       
-0001ef80: 2020 2020 2020 2020 2063 7574 3d46 616c           cut=Fal
-0001ef90: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0001efa0: 2020 2020 636f 6d62 696e 653d 4661 6c73      combine=Fals
-0001efb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001efc0: 2020 2068 616c 6967 6e3d 2272 6967 6874     halign="right
-0001efd0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0001efe0: 2020 2076 616c 6967 6e3d 2274 6f70 222c     valign="top",
-0001eff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f000: 2066 6f6e 743d 2253 616e 7322 2c0a 2020   font="Sans",.  
-0001f010: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001f020: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001f030: 2076 6572 6966 7920 7468 6174 2074 6865   verify that the
-0001f040: 206e 756d 6265 7220 6f66 2073 6f6c 6964   number of solid
-0001f050: 7320 6973 2063 6f72 7265 6374 0a20 2020  s is correct.   
-0001f060: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001f070: 4571 7561 6c28 6c65 6e28 6f62 6a35 2e73  Equal(len(obj5.s
-0001f080: 6f6c 6964 7328 292e 7661 6c73 2829 292c  olids().vals()),
-0001f090: 2035 290a 0a20 2020 2020 2020 2023 2063   5)..        # c
-0001f0a0: 6865 636b 2069 7420 646f 6573 6e27 7420  heck it doesn't 
-0001f0b0: 6661 6c6c 206f 7665 7220 7769 7468 2069  fall over with i
-0001f0c0: 6e74 2073 697a 6573 0a20 2020 2020 2020  nt sizes.       
-0001f0d0: 206f 626a 3120 3d20 280a 2020 2020 2020   obj1 = (.      
-0001f0e0: 2020 2020 2020 626f 782e 6661 6365 7328        box.faces(
-0001f0f0: 223e 5a22 290a 2020 2020 2020 2020 2020  ">Z").          
-0001f100: 2020 2e77 6f72 6b70 6c61 6e65 2829 0a20    .workplane(). 
-0001f110: 2020 2020 2020 2020 2020 202e 7465 7874             .text
-0001f120: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001f130: 2020 2243 5120 322e 3022 2c20 3130 2c20    "CQ 2.0", 10, 
-0001f140: 2d31 2c20 6375 743d 5472 7565 2c20 6861  -1, cut=True, ha
-0001f150: 6c69 676e 3d22 6c65 6674 222c 2076 616c  lign="left", val
-0001f160: 6967 6e3d 2262 6f74 746f 6d22 2c20 666f  ign="bottom", fo
-0001f170: 6e74 3d22 5361 6e73 222c 0a20 2020 2020  nt="Sans",.     
-0001f180: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001f190: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-0001f1a0: 5061 7261 6d65 7472 6963 4375 7276 6528  ParametricCurve(
-0001f1b0: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-0001f1c0: 6672 6f6d 206d 6174 6820 696d 706f 7274  from math import
-0001f1d0: 2073 696e 2c20 636f 732c 2070 690a 0a20   sin, cos, pi.. 
-0001f1e0: 2020 2020 2020 206b 203d 2034 0a20 2020         k = 4.   
-0001f1f0: 2020 2020 2072 203d 2031 0a0a 2020 2020       r = 1..    
-0001f200: 2020 2020 6675 6e63 203d 206c 616d 6264      func = lambd
-0001f210: 6120 743a 2028 0a20 2020 2020 2020 2020  a t: (.         
-0001f220: 2020 2072 202a 2028 6b20 2b20 3129 202a     r * (k + 1) *
-0001f230: 2063 6f73 2874 2920 2d20 7220 2a20 636f   cos(t) - r * co
-0001f240: 7328 286b 202b 2031 2920 2a20 7429 2c0a  s((k + 1) * t),.
-0001f250: 2020 2020 2020 2020 2020 2020 7220 2a20              r * 
-0001f260: 286b 202b 2031 2920 2a20 7369 6e28 7429  (k + 1) * sin(t)
-0001f270: 202d 2072 202a 2073 696e 2828 6b20 2b20   - r * sin((k + 
-0001f280: 3129 202a 2074 292c 0a20 2020 2020 2020  1) * t),.       
-0001f290: 2029 0a0a 2020 2020 2020 2020 7265 735f   )..        res_
-0001f2a0: 6f70 656e 203d 2057 6f72 6b70 6c61 6e65  open = Workplane
-0001f2b0: 2822 5859 2229 2e70 6172 616d 6574 7269  ("XY").parametri
-0001f2c0: 6343 7572 7665 2866 756e 6329 2e65 7874  cCurve(func).ext
-0001f2d0: 7275 6465 2833 290a 0a20 2020 2020 2020  rude(3)..       
-0001f2e0: 2023 206f 7065 6e20 7072 6f66 696c 6520   # open profile 
-0001f2f0: 6765 6e65 7261 7465 7320 616e 2069 6e76  generates an inv
-0001f300: 616c 6964 2073 6f6c 6964 0a20 2020 2020  alid solid.     
-0001f310: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-0001f320: 6c73 6528 7265 735f 6f70 656e 2e73 6f6c  lse(res_open.sol
-0001f330: 6964 7328 292e 7661 6c28 292e 6973 5661  ids().val().isVa
-0001f340: 6c69 6428 2929 0a0a 2020 2020 2020 2020  lid())..        
-0001f350: 7265 735f 636c 6f73 6564 203d 2028 0a20  res_closed = (. 
-0001f360: 2020 2020 2020 2020 2020 2057 6f72 6b70             Workp
-0001f370: 6c61 6e65 2822 5859 2229 2e70 6172 616d  lane("XY").param
-0001f380: 6574 7269 6343 7572 7665 2866 756e 632c  etricCurve(func,
-0001f390: 2073 7461 7274 3d30 2c20 7374 6f70 3d32   start=0, stop=2
-0001f3a0: 202a 2070 6929 2e65 7874 7275 6465 2833   * pi).extrude(3
-0001f3b0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0001f3c0: 2020 2020 2023 2063 6c6f 7365 6420 7072       # closed pr
-0001f3d0: 6f66 696c 6520 7769 6c6c 2067 656e 6572  ofile will gener
-0001f3e0: 6174 6520 6120 7661 6c69 6420 736f 6c69  ate a valid soli
-0001f3f0: 6420 7769 7468 2033 2066 6163 6573 0a20  d with 3 faces. 
-0001f400: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001f410: 7274 5472 7565 2872 6573 5f63 6c6f 7365  rtTrue(res_close
-0001f420: 642e 736f 6c69 6473 2829 2e76 616c 2829  d.solids().val()
-0001f430: 2e69 7356 616c 6964 2829 290a 2020 2020  .isValid()).    
-0001f440: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001f450: 7175 616c 286c 656e 2872 6573 5f63 6c6f  qual(len(res_clo
-0001f460: 7365 642e 6661 6365 7328 292e 7661 6c73  sed.faces().vals
-0001f470: 2829 292c 2033 290a 0a20 2020 2020 2020  ()), 3)..       
-0001f480: 2072 6573 5f65 6467 6520 3d20 576f 726b   res_edge = Work
-0001f490: 706c 616e 6528 2258 5922 292e 7061 7261  plane("XY").para
-0001f4a0: 6d65 7472 6963 4375 7276 6528 6675 6e63  metricCurve(func
-0001f4b0: 2c20 6d61 6b65 5769 7265 3d46 616c 7365  , makeWire=False
-0001f4c0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001f4d0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-0001f4e0: 7265 735f 6564 6765 2e63 7478 2e70 656e  res_edge.ctx.pen
-0001f4f0: 6469 6e67 4564 6765 7329 2c20 3129 0a20  dingEdges), 1). 
-0001f500: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001f510: 7274 4571 7561 6c28 6c65 6e28 7265 735f  rtEqual(len(res_
-0001f520: 6564 6765 2e63 7478 2e70 656e 6469 6e67  edge.ctx.pending
-0001f530: 5769 7265 7329 2c20 3029 0a0a 2020 2020  Wires), 0)..    
-0001f540: 6465 6620 7465 7374 4d61 6b65 5368 656c  def testMakeShel
-0001f550: 6c53 6f6c 6964 2873 656c 6629 3a0a 0a20  lSolid(self):.. 
-0001f560: 2020 2020 2020 2063 3020 3d20 6d61 7468         c0 = math
-0001f570: 2e73 7172 7428 3229 202f 2034 0a20 2020  .sqrt(2) / 4.   
-0001f580: 2020 2020 2076 6572 7469 6365 7320 3d20       vertices = 
-0001f590: 5b5b 6330 2c20 2d63 302c 2063 305d 2c20  [[c0, -c0, c0], 
-0001f5a0: 5b63 302c 2063 302c 202d 6330 5d2c 205b  [c0, c0, -c0], [
-0001f5b0: 2d63 302c 2063 302c 2063 305d 2c20 5b2d  -c0, c0, c0], [-
-0001f5c0: 6330 2c20 2d63 302c 202d 6330 5d5d 0a20  c0, -c0, -c0]]. 
-0001f5d0: 2020 2020 2020 2066 6163 6573 5f69 7873         faces_ixs
-0001f5e0: 203d 205b 5b30 2c20 312c 2032 2c20 305d   = [[0, 1, 2, 0]
-0001f5f0: 2c20 5b31 2c20 302c 2033 2c20 315d 2c20  , [1, 0, 3, 1], 
-0001f600: 5b32 2c20 332c 2030 2c20 325d 2c20 5b33  [2, 3, 0, 2], [3
-0001f610: 2c20 322c 2031 2c20 335d 5d0a 0a20 2020  , 2, 1, 3]]..   
-0001f620: 2020 2020 2066 6163 6573 203d 205b 5d0a       faces = [].
-0001f630: 2020 2020 2020 2020 666f 7220 6978 7320          for ixs 
-0001f640: 696e 2066 6163 6573 5f69 7873 3a0a 2020  in faces_ixs:.  
-0001f650: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
-0001f660: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-0001f670: 2066 6f72 2076 312c 2076 3220 696e 207a   for v1, v2 in z
-0001f680: 6970 2869 7873 2c20 6978 735b 313a 5d29  ip(ixs, ixs[1:])
-0001f690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001f6a0: 2020 6c69 6e65 732e 6170 7065 6e64 280a    lines.append(.
-0001f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f6c0: 2020 2020 4564 6765 2e6d 616b 654c 696e      Edge.makeLin
-0001f6d0: 6528 5665 6374 6f72 282a 7665 7274 6963  e(Vector(*vertic
-0001f6e0: 6573 5b76 315d 292c 2056 6563 746f 7228  es[v1]), Vector(
-0001f6f0: 2a76 6572 7469 6365 735b 7632 5d29 290a  *vertices[v2])).
-0001f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f710: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0001f720: 7265 203d 2057 6972 652e 636f 6d62 696e  re = Wire.combin
-0001f730: 6528 6c69 6e65 7329 5b30 5d0a 2020 2020  e(lines)[0].    
-0001f740: 2020 2020 2020 2020 6661 6365 732e 6170          faces.ap
-0001f750: 7065 6e64 2846 6163 652e 6d61 6b65 4672  pend(Face.makeFr
-0001f760: 6f6d 5769 7265 7328 7769 7265 2929 0a0a  omWires(wire))..
-0001f770: 2020 2020 2020 2020 7368 656c 6c20 3d20          shell = 
-0001f780: 5368 656c 6c2e 6d61 6b65 5368 656c 6c28  Shell.makeShell(
-0001f790: 6661 6365 7329 0a20 2020 2020 2020 2073  faces).        s
-0001f7a0: 6f6c 6964 203d 2053 6f6c 6964 2e6d 616b  olid = Solid.mak
-0001f7b0: 6553 6f6c 6964 2873 6865 6c6c 290a 0a20  eSolid(shell).. 
-0001f7c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001f7d0: 7274 5472 7565 2873 6865 6c6c 2e69 7356  rtTrue(shell.isV
-0001f7e0: 616c 6964 2829 290a 2020 2020 2020 2020  alid()).        
-0001f7f0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-0001f800: 736f 6c69 642e 6973 5661 6c69 6428 2929  solid.isValid())
-0001f810: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0001f820: 7373 6572 7445 7175 616c 286c 656e 2873  ssertEqual(len(s
-0001f830: 6f6c 6964 2e56 6572 7469 6365 7328 2929  olid.Vertices())
-0001f840: 2c20 3429 0a20 2020 2020 2020 2073 656c  , 4).        sel
-0001f850: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-0001f860: 6e28 736f 6c69 642e 4661 6365 7328 2929  n(solid.Faces())
-0001f870: 2c20 3429 0a0a 2020 2020 6465 6620 7465  , 4)..    def te
-0001f880: 7374 4973 496e 7369 6465 536f 6c69 6428  stIsInsideSolid(
-0001f890: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-0001f8a0: 2074 6573 7420 736f 6c69 640a 2020 2020   test solid.    
-0001f8b0: 2020 2020 6d6f 6465 6c20 3d20 576f 726b      model = Work
-0001f8c0: 706c 616e 6528 2258 5922 292e 626f 7828  plane("XY").box(
-0001f8d0: 3130 2c20 3130 2c20 3130 290a 2020 2020  10, 10, 10).    
-0001f8e0: 2020 2020 736f 6c69 6420 3d20 6d6f 6465      solid = mode
-0001f8f0: 6c2e 7661 6c28 2920 2023 2067 6574 2066  l.val()  # get f
-0001f900: 6972 7374 206f 626a 6563 7420 6f6e 2073  irst object on s
-0001f910: 7461 636b 0a0a 2020 2020 2020 2020 7365  tack..        se
-0001f920: 6c66 2e61 7373 6572 7454 7275 6528 736f  lf.assertTrue(so
-0001f930: 6c69 642e 6973 496e 7369 6465 2828 302c  lid.isInside((0,
-0001f940: 2030 2c20 3029 2929 0a20 2020 2020 2020   0, 0))).       
-0001f950: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-0001f960: 6528 736f 6c69 642e 6973 496e 7369 6465  e(solid.isInside
-0001f970: 2828 3130 2c20 3130 2c20 3130 2929 290a  ((10, 10, 10))).
-0001f980: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001f990: 6572 7454 7275 6528 736f 6c69 642e 6973  ertTrue(solid.is
-0001f9a0: 496e 7369 6465 2828 5665 6374 6f72 2833  Inside((Vector(3
-0001f9b0: 2c20 332c 2033 2929 2929 0a20 2020 2020  , 3, 3)))).     
-0001f9c0: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-0001f9d0: 6c73 6528 736f 6c69 642e 6973 496e 7369  lse(solid.isInsi
-0001f9e0: 6465 2828 5665 6374 6f72 2833 302e 302c  de((Vector(30.0,
-0001f9f0: 2033 302e 302c 2033 302e 3029 2929 290a   30.0, 30.0)))).
-0001fa00: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001fa10: 7365 7274 5472 7565 2873 6f6c 6964 2e69  sertTrue(solid.i
-0001fa20: 7349 6e73 6964 6528 2830 2c20 302c 2034  sInside((0, 0, 4
-0001fa30: 2e39 3929 2c20 746f 6c65 7261 6e63 653d  .99), tolerance=
-0001fa40: 302e 3129 290a 2020 2020 2020 2020 7365  0.1)).        se
-0001fa50: 6c66 2e61 7373 6572 7454 7275 6528 736f  lf.assertTrue(so
-0001fa60: 6c69 642e 6973 496e 7369 6465 2828 302c  lid.isInside((0,
-0001fa70: 2030 2c20 3529 2929 2020 2320 6368 6563   0, 5)))  # chec
-0001fa80: 6b20 706f 696e 7420 6f6e 2073 7572 6661  k point on surfa
-0001fa90: 6365 0a20 2020 2020 2020 2073 656c 662e  ce.        self.
-0001faa0: 6173 7365 7274 5472 7565 2873 6f6c 6964  assertTrue(solid
-0001fab0: 2e69 7349 6e73 6964 6528 2830 2c20 302c  .isInside((0, 0,
-0001fac0: 2035 2e30 3129 2c20 746f 6c65 7261 6e63   5.01), toleranc
-0001fad0: 653d 302e 3129 290a 2020 2020 2020 2020  e=0.1)).        
-0001fae0: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
-0001faf0: 2873 6f6c 6964 2e69 7349 6e73 6964 6528  (solid.isInside(
-0001fb00: 2830 2c20 302c 2035 2e31 292c 2074 6f6c  (0, 0, 5.1), tol
-0001fb10: 6572 616e 6365 3d30 2e31 2929 0a0a 2020  erance=0.1))..  
-0001fb20: 2020 2020 2020 2320 7465 7374 2063 6f6d        # test com
-0001fb30: 706f 756e 6420 736f 6c69 640a 2020 2020  pound solid.    
-0001fb40: 2020 2020 6d6f 6465 6c20 3d20 576f 726b      model = Work
-0001fb50: 706c 616e 6528 2258 5922 292e 626f 7828  plane("XY").box(
-0001fb60: 3130 2c20 3130 2c20 3130 290a 2020 2020  10, 10, 10).    
-0001fb70: 2020 2020 6d6f 6465 6c20 3d20 6d6f 6465      model = mode
-0001fb80: 6c2e 6d6f 7665 546f 2835 302c 2035 3029  l.moveTo(50, 50)
-0001fb90: 2e62 6f78 2831 302c 2031 302c 2031 3029  .box(10, 10, 10)
-0001fba0: 0a20 2020 2020 2020 2073 6f6c 6964 203d  .        solid =
-0001fbb0: 206d 6f64 656c 2e76 616c 2829 0a0a 2020   model.val()..  
-0001fbc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001fbd0: 7454 7275 6528 736f 6c69 642e 6973 496e  tTrue(solid.isIn
-0001fbe0: 7369 6465 2828 302c 2030 2c20 3029 2929  side((0, 0, 0)))
-0001fbf0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001fc00: 7365 7274 5472 7565 2873 6f6c 6964 2e69  sertTrue(solid.i
-0001fc10: 7349 6e73 6964 6528 2835 302c 2035 302c  sInside((50, 50,
-0001fc20: 2030 2929 290a 2020 2020 2020 2020 7365   0))).        se
-0001fc30: 6c66 2e61 7373 6572 7446 616c 7365 2873  lf.assertFalse(s
-0001fc40: 6f6c 6964 2e69 7349 6e73 6964 6528 2835  olid.isInside((5
-0001fc50: 302c 2035 362c 2030 2929 290a 0a20 2020  0, 56, 0)))..   
-0001fc60: 2020 2020 2023 206d 616b 6520 7375 7265       # make sure
-0001fc70: 2072 6169 7365 7320 6f6e 206e 6f6e 2073   raises on non s
-0001fc80: 6f6c 6964 0a20 2020 2020 2020 206d 6f64  olid.        mod
-0001fc90: 656c 203d 2057 6f72 6b70 6c61 6e65 2822  el = Workplane("
-0001fca0: 5859 2229 2e72 6563 7428 3130 2c20 3130  XY").rect(10, 10
-0001fcb0: 290a 2020 2020 2020 2020 736f 6c69 6420  ).        solid 
-0001fcc0: 3d20 6d6f 6465 6c2e 7661 6c28 290a 2020  = model.val().  
-0001fcd0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0001fce0: 6173 7365 7274 5261 6973 6573 2841 7474  assertRaises(Att
-0001fcf0: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
-0001fd00: 2020 2020 2020 2020 2020 736f 6c69 642e            solid.
-0001fd10: 6973 496e 7369 6465 2828 302c 2030 2c20  isInside((0, 0, 
-0001fd20: 3029 290a 0a20 2020 2020 2020 2023 2074  0))..        # t
-0001fd30: 6573 7420 736f 6c69 6420 7769 7468 2061  est solid with a
-0001fd40: 6e20 696e 7465 726e 616c 2076 6f69 640a  n internal void.
-0001fd50: 2020 2020 2020 2020 766f 6964 203d 2057          void = W
-0001fd60: 6f72 6b70 6c61 6e65 2822 5859 2229 2e62  orkplane("XY").b
-0001fd70: 6f78 2831 302c 2031 302c 2031 3029 0a20  ox(10, 10, 10). 
-0001fd80: 2020 2020 2020 206d 6f64 656c 203d 2057         model = W
-0001fd90: 6f72 6b70 6c61 6e65 2822 5859 2229 2e62  orkplane("XY").b
-0001fda0: 6f78 2831 3030 2c20 3130 302c 2031 3030  ox(100, 100, 100
-0001fdb0: 292e 6375 7428 766f 6964 290a 2020 2020  ).cut(void).    
-0001fdc0: 2020 2020 736f 6c69 6420 3d20 6d6f 6465      solid = mode
-0001fdd0: 6c2e 7661 6c28 290a 0a20 2020 2020 2020  l.val()..       
-0001fde0: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-0001fdf0: 6528 736f 6c69 642e 6973 496e 7369 6465  e(solid.isInside
-0001fe00: 2828 302c 2030 2c20 3029 2929 0a20 2020  ((0, 0, 0))).   
-0001fe10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001fe20: 5472 7565 2873 6f6c 6964 2e69 7349 6e73  True(solid.isIns
-0001fe30: 6964 6528 2834 302c 2034 302c 2034 3029  ide((40, 40, 40)
-0001fe40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001fe50: 6173 7365 7274 4661 6c73 6528 736f 6c69  assertFalse(soli
-0001fe60: 642e 6973 496e 7369 6465 2828 3535 2c20  d.isInside((55, 
-0001fe70: 3535 2c20 3535 2929 290a 0a20 2020 2064  55, 55)))..    d
-0001fe80: 6566 2074 6573 7457 6f72 6b70 6c61 6e65  ef testWorkplane
-0001fe90: 4365 6e74 6572 4f70 7469 6f6e 7328 7365  CenterOptions(se
-0001fea0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0001feb0: 0a20 2020 2020 2020 2054 6573 7420 6f70  .        Test op
-0001fec0: 7469 6f6e 7320 666f 7220 7370 6563 6966  tions for specif
-0001fed0: 7969 6e67 206f 7269 6769 6e20 6f66 2077  ying origin of w
-0001fee0: 6f72 6b70 6c61 6e65 0a20 2020 2020 2020  orkplane.       
-0001fef0: 2022 2222 0a20 2020 2020 2020 2064 6563   """.        dec
-0001ff00: 696d 616c 5f70 6c61 6365 7320 3d20 390a  imal_places = 9.
-0001ff10: 0a20 2020 2020 2020 2070 7473 203d 205b  .        pts = [
-0001ff20: 2830 2c20 3029 2c20 2839 302c 2030 292c  (0, 0), (90, 0),
-0001ff30: 2028 3930 2c20 3330 292c 2028 3330 2c20   (90, 30), (30, 
-0001ff40: 3330 292c 2028 3330 2c20 3630 292c 2028  30), (30, 60), (
-0001ff50: 302e 302c 2036 3029 5d0a 0a20 2020 2020  0.0, 60)]..     
-0001ff60: 2020 2072 203d 2057 6f72 6b70 6c61 6e65     r = Workplane
-0001ff70: 2822 5859 2229 2e70 6f6c 796c 696e 6528  ("XY").polyline(
-0001ff80: 7074 7329 2e63 6c6f 7365 2829 2e65 7874  pts).close().ext
-0001ff90: 7275 6465 2831 302e 3029 0a0a 2020 2020  rude(10.0)..    
-0001ffa0: 2020 2020 6f72 6967 696e 203d 2028 0a20      origin = (. 
-0001ffb0: 2020 2020 2020 2020 2020 2072 2e66 6163             r.fac
-0001ffc0: 6573 2822 3e5a 2229 0a20 2020 2020 2020  es(">Z").       
-0001ffd0: 2020 2020 202e 776f 726b 706c 616e 6528       .workplane(
-0001ffe0: 6365 6e74 6572 4f70 7469 6f6e 3d22 5072  centerOption="Pr
-0001fff0: 6f6a 6563 7465 644f 7269 6769 6e22 290a  ojectedOrigin").
-00020000: 2020 2020 2020 2020 2020 2020 2e70 6c61              .pla
-00020010: 6e65 2e6f 7269 6769 6e2e 746f 5475 706c  ne.origin.toTupl
-00020020: 6528 290a 2020 2020 2020 2020 290a 2020  e().        ).  
-00020030: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00020040: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
-00020050: 6c73 286f 7269 6769 6e2c 2028 302e 302c  ls(origin, (0.0,
-00020060: 2030 2e30 2c20 3130 2e30 292c 2064 6563   0.0, 10.0), dec
-00020070: 696d 616c 5f70 6c61 6365 7329 0a0a 2020  imal_places)..  
-00020080: 2020 2020 2020 6f72 6967 696e 203d 2028        origin = (
-00020090: 0a20 2020 2020 2020 2020 2020 2072 2e66  .            r.f
-000200a0: 6163 6573 2822 3e5a 2229 2e77 6f72 6b70  aces(">Z").workp
-000200b0: 6c61 6e65 2863 656e 7465 724f 7074 696f  lane(centerOptio
-000200c0: 6e3d 2243 656e 7465 724f 664d 6173 7322  n="CenterOfMass"
-000200d0: 292e 706c 616e 652e 6f72 6967 696e 2e74  ).plane.origin.t
-000200e0: 6f54 7570 6c65 2829 0a20 2020 2020 2020  oTuple().       
-000200f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00020100: 6173 7365 7274 5475 706c 6541 6c6d 6f73  assertTupleAlmos
-00020110: 7445 7175 616c 7328 6f72 6967 696e 2c20  tEquals(origin, 
-00020120: 2833 372e 352c 2032 322e 352c 2031 302e  (37.5, 22.5, 10.
-00020130: 3029 2c20 6465 6369 6d61 6c5f 706c 6163  0), decimal_plac
-00020140: 6573 290a 0a20 2020 2020 2020 206f 7269  es)..        ori
-00020150: 6769 6e20 3d20 280a 2020 2020 2020 2020  gin = (.        
-00020160: 2020 2020 722e 6661 6365 7328 223e 5a22      r.faces(">Z"
-00020170: 290a 2020 2020 2020 2020 2020 2020 2e77  ).            .w
-00020180: 6f72 6b70 6c61 6e65 2863 656e 7465 724f  orkplane(centerO
-00020190: 7074 696f 6e3d 2243 656e 7465 724f 6642  ption="CenterOfB
-000201a0: 6f75 6e64 426f 7822 290a 2020 2020 2020  oundBox").      
-000201b0: 2020 2020 2020 2e70 6c61 6e65 2e6f 7269        .plane.ori
-000201c0: 6769 6e2e 746f 5475 706c 6528 290a 2020  gin.toTuple().  
-000201d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000201e0: 7365 6c66 2e61 7373 6572 7454 7570 6c65  self.assertTuple
-000201f0: 416c 6d6f 7374 4571 7561 6c73 286f 7269  AlmostEquals(ori
-00020200: 6769 6e2c 2028 3435 2e30 2c20 3330 2e30  gin, (45.0, 30.0
-00020210: 2c20 3130 2e30 292c 2064 6563 696d 616c  , 10.0), decimal
-00020220: 5f70 6c61 6365 7329 0a0a 2020 2020 2020  _places)..      
-00020230: 2020 6f72 6967 696e 203d 2028 0a20 2020    origin = (.   
-00020240: 2020 2020 2020 2020 2072 2e66 6163 6573           r.faces
-00020250: 2822 3e5a 2229 0a20 2020 2020 2020 2020  (">Z").         
-00020260: 2020 202e 776f 726b 706c 616e 6528 6365     .workplane(ce
-00020270: 6e74 6572 4f70 7469 6f6e 3d22 5072 6f6a  nterOption="Proj
-00020280: 6563 7465 644f 7269 6769 6e22 2c20 6f72  ectedOrigin", or
-00020290: 6967 696e 3d28 3330 2c20 3130 2c20 3230  igin=(30, 10, 20
-000202a0: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
-000202b0: 706c 616e 652e 6f72 6967 696e 2e74 6f54  plane.origin.toT
-000202c0: 7570 6c65 2829 0a20 2020 2020 2020 2029  uple().        )
-000202d0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000202e0: 7365 7274 5475 706c 6541 6c6d 6f73 7445  sertTupleAlmostE
-000202f0: 7175 616c 7328 6f72 6967 696e 2c20 2833  quals(origin, (3
-00020300: 302e 302c 2031 302e 302c 2031 302e 3029  0.0, 10.0, 10.0)
-00020310: 2c20 6465 6369 6d61 6c5f 706c 6163 6573  , decimal_places
-00020320: 290a 0a20 2020 2020 2020 206f 7269 6769  )..        origi
-00020330: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-00020340: 2020 722e 6661 6365 7328 223e 5a22 290a    r.faces(">Z").
-00020350: 2020 2020 2020 2020 2020 2020 2e77 6f72              .wor
-00020360: 6b70 6c61 6e65 2863 656e 7465 724f 7074  kplane(centerOpt
-00020370: 696f 6e3d 2250 726f 6a65 6374 6564 4f72  ion="ProjectedOr
-00020380: 6967 696e 222c 206f 7269 6769 6e3d 5665  igin", origin=Ve
-00020390: 6374 6f72 2833 302c 2031 302c 2032 3029  ctor(30, 10, 20)
-000203a0: 290a 2020 2020 2020 2020 2020 2020 2e70  ).            .p
-000203b0: 6c61 6e65 2e6f 7269 6769 6e2e 746f 5475  lane.origin.toTu
-000203c0: 706c 6528 290a 2020 2020 2020 2020 290a  ple().        ).
-000203d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000203e0: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
-000203f0: 7561 6c73 286f 7269 6769 6e2c 2028 3330  uals(origin, (30
-00020400: 2e30 2c20 3130 2e30 2c20 3130 2e30 292c  .0, 10.0, 10.0),
-00020410: 2064 6563 696d 616c 5f70 6c61 6365 7329   decimal_places)
-00020420: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00020430: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00020440: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
-00020450: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-00020460: 203d 2072 2e66 6163 6573 2822 3e5a 2229   = r.faces(">Z")
-00020470: 2e77 6f72 6b70 6c61 6e65 2863 656e 7465  .workplane(cente
-00020480: 724f 7074 696f 6e3d 2275 6e64 6566 696e  rOption="undefin
-00020490: 6564 2229 0a0a 2020 2020 2020 2020 2320  ed")..        # 
-000204a0: 7465 7374 2063 6173 6520 7768 6572 6520  test case where 
-000204b0: 706c 616e 6520 6f72 6967 696e 2069 7320  plane origin is 
-000204c0: 7368 6966 7465 6420 7769 7468 2063 656e  shifted with cen
-000204d0: 7465 7220 6361 6c6c 0a20 2020 2020 2020  ter call.       
-000204e0: 2072 203d 2028 0a20 2020 2020 2020 2020   r = (.         
-000204f0: 2020 2072 2e66 6163 6573 2822 3e5a 2229     r.faces(">Z")
-00020500: 0a20 2020 2020 2020 2020 2020 202e 776f  .            .wo
-00020510: 726b 706c 616e 6528 6365 6e74 6572 4f70  rkplane(centerOp
-00020520: 7469 6f6e 3d22 5072 6f6a 6563 7465 644f  tion="ProjectedO
-00020530: 7269 6769 6e22 290a 2020 2020 2020 2020  rigin").        
-00020540: 2020 2020 2e63 656e 7465 7228 3330 2c20      .center(30, 
-00020550: 3029 0a20 2020 2020 2020 2020 2020 202e  0).            .
-00020560: 686f 6c65 2839 3029 0a20 2020 2020 2020  hole(90).       
-00020570: 2029 0a0a 2020 2020 2020 2020 6f72 6967   )..        orig
-00020580: 696e 203d 2028 0a20 2020 2020 2020 2020  in = (.         
-00020590: 2020 2072 2e66 6163 6573 2822 3e5a 2229     r.faces(">Z")
-000205a0: 0a20 2020 2020 2020 2020 2020 202e 776f  .            .wo
-000205b0: 726b 706c 616e 6528 6365 6e74 6572 4f70  rkplane(centerOp
-000205c0: 7469 6f6e 3d22 5072 6f6a 6563 7465 644f  tion="ProjectedO
-000205d0: 7269 6769 6e22 290a 2020 2020 2020 2020  rigin").        
-000205e0: 2020 2020 2e70 6c61 6e65 2e6f 7269 6769      .plane.origi
-000205f0: 6e2e 746f 5475 706c 6528 290a 2020 2020  n.toTuple().    
-00020600: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00020610: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
-00020620: 6d6f 7374 4571 7561 6c73 286f 7269 6769  mostEquals(origi
-00020630: 6e2c 2028 3330 2e30 2c20 302e 302c 2031  n, (30.0, 0.0, 1
-00020640: 302e 3029 2c20 6465 6369 6d61 6c5f 706c  0.0), decimal_pl
-00020650: 6163 6573 290a 0a20 2020 2020 2020 206f  aces)..        o
-00020660: 7269 6769 6e20 3d20 280a 2020 2020 2020  rigin = (.      
-00020670: 2020 2020 2020 722e 6661 6365 7328 223e        r.faces(">
-00020680: 5a22 290a 2020 2020 2020 2020 2020 2020  Z").            
-00020690: 2e77 6f72 6b70 6c61 6e65 2863 656e 7465  .workplane(cente
-000206a0: 724f 7074 696f 6e3d 2250 726f 6a65 6374  rOption="Project
-000206b0: 6564 4f72 6967 696e 222c 206f 7269 6769  edOrigin", origi
-000206c0: 6e3d 2830 2c20 302c 2030 2929 0a20 2020  n=(0, 0, 0)).   
-000206d0: 2020 2020 2020 2020 202e 706c 616e 652e           .plane.
-000206e0: 6f72 6967 696e 2e74 6f54 7570 6c65 2829  origin.toTuple()
-000206f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00020700: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
-00020710: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
-00020720: 6f72 6967 696e 2c20 2830 2e30 2c20 302e  origin, (0.0, 0.
-00020730: 302c 2031 302e 3029 2c20 6465 6369 6d61  0, 10.0), decima
-00020740: 6c5f 706c 6163 6573 290a 0a20 2020 2020  l_places)..     
-00020750: 2020 2023 206d 616b 6520 7375 7265 2070     # make sure p
-00020760: 726f 6a65 6374 696f 6e20 776f 726b 7320  rojection works 
-00020770: 696e 2061 6c6c 2064 6972 6563 7469 6f6e  in all direction
-00020780: 730a 2020 2020 2020 2020 7220 3d20 576f  s.        r = Wo
-00020790: 726b 706c 616e 6528 2259 5a22 292e 706f  rkplane("YZ").po
-000207a0: 6c79 6c69 6e65 2870 7473 292e 636c 6f73  lyline(pts).clos
-000207b0: 6528 292e 6578 7472 7564 6528 3130 2e30  e().extrude(10.0
-000207c0: 290a 0a20 2020 2020 2020 206f 7269 6769  )..        origi
-000207d0: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-000207e0: 2020 722e 6661 6365 7328 223e 5822 290a    r.faces(">X").
-000207f0: 2020 2020 2020 2020 2020 2020 2e77 6f72              .wor
-00020800: 6b70 6c61 6e65 2863 656e 7465 724f 7074  kplane(centerOpt
-00020810: 696f 6e3d 2250 726f 6a65 6374 6564 4f72  ion="ProjectedOr
-00020820: 6967 696e 2229 0a20 2020 2020 2020 2020  igin").         
-00020830: 2020 202e 706c 616e 652e 6f72 6967 696e     .plane.origin
-00020840: 2e74 6f54 7570 6c65 2829 0a20 2020 2020  .toTuple().     
-00020850: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00020860: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
-00020870: 6f73 7445 7175 616c 7328 6f72 6967 696e  ostEquals(origin
-00020880: 2c20 2831 302e 302c 2030 2e30 2c20 302e  , (10.0, 0.0, 0.
-00020890: 3029 2c20 6465 6369 6d61 6c5f 706c 6163  0), decimal_plac
-000208a0: 6573 290a 0a20 2020 2020 2020 206f 7269  es)..        ori
-000208b0: 6769 6e20 3d20 280a 2020 2020 2020 2020  gin = (.        
-000208c0: 2020 2020 722e 6661 6365 7328 223e 5822      r.faces(">X"
-000208d0: 292e 776f 726b 706c 616e 6528 6365 6e74  ).workplane(cent
-000208e0: 6572 4f70 7469 6f6e 3d22 4365 6e74 6572  erOption="Center
-000208f0: 4f66 4d61 7373 2229 2e70 6c61 6e65 2e6f  OfMass").plane.o
-00020900: 7269 6769 6e2e 746f 5475 706c 6528 290a  rigin.toTuple().
-00020910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00020920: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
-00020930: 6c65 416c 6d6f 7374 4571 7561 6c73 286f  leAlmostEquals(o
-00020940: 7269 6769 6e2c 2028 3130 2e30 2c20 3337  rigin, (10.0, 37
-00020950: 2e35 2c20 3232 2e35 292c 2064 6563 696d  .5, 22.5), decim
-00020960: 616c 5f70 6c61 6365 7329 0a0a 2020 2020  al_places)..    
-00020970: 2020 2020 6f72 6967 696e 203d 2028 0a20      origin = (. 
-00020980: 2020 2020 2020 2020 2020 2072 2e66 6163             r.fac
-00020990: 6573 2822 3e58 2229 0a20 2020 2020 2020  es(">X").       
-000209a0: 2020 2020 202e 776f 726b 706c 616e 6528       .workplane(
-000209b0: 6365 6e74 6572 4f70 7469 6f6e 3d22 4365  centerOption="Ce
-000209c0: 6e74 6572 4f66 426f 756e 6442 6f78 2229  nterOfBoundBox")
-000209d0: 0a20 2020 2020 2020 2020 2020 202e 706c  .            .pl
-000209e0: 616e 652e 6f72 6967 696e 2e74 6f54 7570  ane.origin.toTup
-000209f0: 6c65 2829 0a20 2020 2020 2020 2029 0a20  le().        ). 
-00020a00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00020a10: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
-00020a20: 616c 7328 6f72 6967 696e 2c20 2831 302e  als(origin, (10.
-00020a30: 302c 2034 352e 302c 2033 302e 3029 2c20  0, 45.0, 30.0), 
-00020a40: 6465 6369 6d61 6c5f 706c 6163 6573 290a  decimal_places).
-00020a50: 0a20 2020 2020 2020 2072 203d 2057 6f72  .        r = Wor
-00020a60: 6b70 6c61 6e65 2822 585a 2229 2e70 6f6c  kplane("XZ").pol
-00020a70: 796c 696e 6528 7074 7329 2e63 6c6f 7365  yline(pts).close
-00020a80: 2829 2e65 7874 7275 6465 2831 302e 3029  ().extrude(10.0)
-00020a90: 0a0a 2020 2020 2020 2020 6f72 6967 696e  ..        origin
-00020aa0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00020ab0: 2072 2e66 6163 6573 2822 3c59 2229 0a20   r.faces("<Y"). 
-00020ac0: 2020 2020 2020 2020 2020 202e 776f 726b             .work
-00020ad0: 706c 616e 6528 6365 6e74 6572 4f70 7469  plane(centerOpti
-00020ae0: 6f6e 3d22 5072 6f6a 6563 7465 644f 7269  on="ProjectedOri
-00020af0: 6769 6e22 290a 2020 2020 2020 2020 2020  gin").          
-00020b00: 2020 2e70 6c61 6e65 2e6f 7269 6769 6e2e    .plane.origin.
-00020b10: 746f 5475 706c 6528 290a 2020 2020 2020  toTuple().      
-00020b20: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00020b30: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
-00020b40: 7374 4571 7561 6c73 286f 7269 6769 6e2c  stEquals(origin,
-00020b50: 2028 302e 302c 202d 3130 2e30 2c20 302e   (0.0, -10.0, 0.
-00020b60: 3029 2c20 6465 6369 6d61 6c5f 706c 6163  0), decimal_plac
-00020b70: 6573 290a 0a20 2020 2020 2020 206f 7269  es)..        ori
-00020b80: 6769 6e20 3d20 280a 2020 2020 2020 2020  gin = (.        
-00020b90: 2020 2020 722e 6661 6365 7328 223c 5922      r.faces("<Y"
-00020ba0: 292e 776f 726b 706c 616e 6528 6365 6e74  ).workplane(cent
-00020bb0: 6572 4f70 7469 6f6e 3d22 4365 6e74 6572  erOption="Center
-00020bc0: 4f66 4d61 7373 2229 2e70 6c61 6e65 2e6f  OfMass").plane.o
-00020bd0: 7269 6769 6e2e 746f 5475 706c 6528 290a  rigin.toTuple().
-00020be0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00020bf0: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
-00020c00: 6c65 416c 6d6f 7374 4571 7561 6c73 286f  leAlmostEquals(o
-00020c10: 7269 6769 6e2c 2028 3337 2e35 2c20 2d31  rigin, (37.5, -1
-00020c20: 302e 302c 2032 322e 3529 2c20 6465 6369  0.0, 22.5), deci
-00020c30: 6d61 6c5f 706c 6163 6573 290a 0a20 2020  mal_places)..   
-00020c40: 2020 2020 206f 7269 6769 6e20 3d20 280a       origin = (.
-00020c50: 2020 2020 2020 2020 2020 2020 722e 6661              r.fa
-00020c60: 6365 7328 223c 5922 290a 2020 2020 2020  ces("<Y").      
-00020c70: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
-00020c80: 2863 656e 7465 724f 7074 696f 6e3d 2243  (centerOption="C
-00020c90: 656e 7465 724f 6642 6f75 6e64 426f 7822  enterOfBoundBox"
-00020ca0: 290a 2020 2020 2020 2020 2020 2020 2e70  ).            .p
-00020cb0: 6c61 6e65 2e6f 7269 6769 6e2e 746f 5475  lane.origin.toTu
-00020cc0: 706c 6528 290a 2020 2020 2020 2020 290a  ple().        ).
-00020cd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00020ce0: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
-00020cf0: 7561 6c73 286f 7269 6769 6e2c 2028 3435  uals(origin, (45
-00020d00: 2e30 2c20 2d31 302e 302c 2033 302e 3029  .0, -10.0, 30.0)
-00020d10: 2c20 6465 6369 6d61 6c5f 706c 6163 6573  , decimal_places
-00020d20: 290a 0a20 2020 2064 6566 2074 6573 7446  )..    def testF
-00020d30: 696e 6453 6f6c 6964 2873 656c 6629 3a0a  indSolid(self):.
-00020d40: 0a20 2020 2020 2020 2072 203d 2057 6f72  .        r = Wor
-00020d50: 6b70 6c61 6e65 2822 5859 2229 2e70 7573  kplane("XY").pus
-00020d60: 6850 6f69 6e74 7328 5b28 2d32 2c20 3029  hPoints([(-2, 0)
-00020d70: 2c20 2832 2c20 3029 5d29 2e62 6f78 2831  , (2, 0)]).box(1
-00020d80: 2c20 312c 2031 2c20 636f 6d62 696e 653d  , 1, 1, combine=
-00020d90: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-00020da0: 2320 7468 6572 6520 7368 6f75 6c64 2062  # there should b
-00020db0: 6520 7477 6f20 736f 6c69 6473 206f 6e20  e two solids on 
-00020dc0: 7468 6520 7374 6163 6b0a 2020 2020 2020  the stack.      
-00020dd0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00020de0: 616c 286c 656e 2872 2e6f 626a 6563 7473  al(len(r.objects
-00020df0: 292c 2032 290a 2020 2020 2020 2020 7365  ), 2).        se
-00020e00: 6c66 2e61 7373 6572 7454 7275 6528 6973  lf.assertTrue(is
-00020e10: 696e 7374 616e 6365 2872 2e76 616c 2829  instance(r.val()
-00020e20: 2c20 536f 6c69 6429 290a 0a20 2020 2020  , Solid))..     
-00020e30: 2020 2023 2066 696e 6420 736f 6c69 6420     # find solid 
-00020e40: 7368 6f75 6c64 2072 6574 7572 6e20 6120  should return a 
-00020e50: 636f 6d70 6f75 6e64 206f 6620 7477 6f20  compound of two 
-00020e60: 736f 6c69 6473 0a20 2020 2020 2020 2073  solids.        s
-00020e70: 203d 2072 2e66 696e 6453 6f6c 6964 2829   = r.findSolid()
-00020e80: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00020e90: 7365 7274 4571 7561 6c28 6c65 6e28 732e  sertEqual(len(s.
-00020ea0: 536f 6c69 6473 2829 292c 2032 290a 2020  Solids()), 2).  
-00020eb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00020ec0: 7454 7275 6528 6973 696e 7374 616e 6365  tTrue(isinstance
-00020ed0: 2873 2c20 436f 6d70 6f75 6e64 2929 0a0a  (s, Compound))..
-00020ee0: 2020 2020 2020 2020 2320 6966 206e 6f20          # if no 
-00020ef0: 736f 6c69 6473 2061 7265 2066 6f75 6e64  solids are found
-00020f00: 2c20 7368 6f75 6c64 2072 6169 7365 2056  , should raise V
-00020f10: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
-00020f20: 2020 7720 3d20 576f 726b 706c 616e 6528    w = Workplane(
-00020f30: 292e 684c 696e 6528 3129 2e63 6c6f 7365  ).hLine(1).close
-00020f40: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
-00020f50: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
-00020f60: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00020f70: 772e 6669 6e64 536f 6c69 6428 290a 0a20  w.findSolid().. 
-00020f80: 2020 2064 6566 2074 6573 7453 6c6f 7432     def testSlot2
-00020f90: 4428 7365 6c66 293a 0a0a 2020 2020 2020  D(self):..      
-00020fa0: 2020 6465 6369 6d61 6c5f 706c 6163 6573    decimal_places
-00020fb0: 203d 2039 0a0a 2020 2020 2020 2020 2320   = 9..        # 
-00020fc0: 456e 7375 7265 2069 7420 7072 6f64 7563  Ensure it produc
-00020fd0: 6573 2061 2073 6f6c 6964 2077 6974 6820  es a solid with 
-00020fe0: 7468 6520 636f 7272 6563 7420 766f 6c75  the correct volu
-00020ff0: 6d65 0a20 2020 2020 2020 2072 6573 756c  me.        resul
-00021000: 7420 3d20 576f 726b 706c 616e 6528 2258  t = Workplane("X
-00021010: 5922 292e 736c 6f74 3244 2834 2c20 312c  Y").slot2D(4, 1,
-00021020: 2030 292e 6578 7472 7564 6528 3129 0a20   0).extrude(1). 
-00021030: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00021040: 7274 416c 6d6f 7374 4571 7561 6c28 7265  rtAlmostEqual(re
-00021050: 7375 6c74 2e76 616c 2829 2e56 6f6c 756d  sult.val().Volum
-00021060: 6528 292c 2033 2e37 3835 3339 3831 3633  e(), 3.785398163
-00021070: 2c20 6465 6369 6d61 6c5f 706c 6163 6573  , decimal_places
-00021080: 290a 0a20 2020 2020 2020 2023 2054 6573  )..        # Tes
-00021090: 7420 666f 7220 7072 6f70 6572 2065 7870  t for proper exp
-000210a0: 6563 7465 6420 6265 6861 7669 6f75 7220  ected behaviour 
-000210b0: 7768 656e 2063 7574 7469 6e67 0a20 2020  when cutting.   
-000210c0: 2020 2020 2062 6f78 203d 2057 6f72 6b70       box = Workp
-000210d0: 6c61 6e65 2822 5859 2229 2e62 6f78 2835  lane("XY").box(5
-000210e0: 2c20 352c 2031 290a 2020 2020 2020 2020  , 5, 1).        
-000210f0: 7265 7375 6c74 203d 2062 6f78 2e66 6163  result = box.fac
-00021100: 6573 2822 3e5a 2229 2e77 6f72 6b70 6c61  es(">Z").workpla
-00021110: 6e65 2829 2e73 6c6f 7432 4428 342c 2031  ne().slot2D(4, 1
-00021120: 2c20 3029 2e63 7574 5468 7275 416c 6c28  , 0).cutThruAll(
-00021130: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00021140: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
-00021150: 2872 6573 756c 742e 7661 6c28 292e 566f  (result.val().Vo
-00021160: 6c75 6d65 2829 2c20 3231 2e32 3134 3630  lume(), 21.21460
-00021170: 3138 3337 2c20 6465 6369 6d61 6c5f 706c  1837, decimal_pl
-00021180: 6163 6573 290a 2020 2020 2020 2020 7265  aces).        re
-00021190: 7375 6c74 203d 2062 6f78 2e66 6163 6573  sult = box.faces
-000211a0: 2822 3e5a 2229 2e77 6f72 6b70 6c61 6e65  (">Z").workplane
-000211b0: 2829 2e73 6c6f 7432 4428 342c 2031 2c20  ().slot2D(4, 1, 
-000211c0: 3029 2e63 7574 426c 696e 6428 2d30 2e35  0).cutBlind(-0.5
-000211d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000211e0: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
-000211f0: 2872 6573 756c 742e 7661 6c28 292e 566f  (result.val().Vo
-00021200: 6c75 6d65 2829 2c20 3233 2e31 3037 3330  lume(), 23.10730
-00021210: 3039 3138 2c20 6465 6369 6d61 6c5f 706c  0918, decimal_pl
-00021220: 6163 6573 290a 0a20 2020 2020 2020 2023  aces)..        #
-00021230: 2054 6573 7420 746f 2073 6565 2069 6620   Test to see if 
-00021240: 736c 6f74 2069 7320 726f 7461 7465 6420  slot is rotated 
-00021250: 636f 7272 6563 746c 790a 2020 2020 2020  correctly.      
-00021260: 2020 7265 7375 6c74 203d 2057 6f72 6b70    result = Workp
-00021270: 6c61 6e65 2822 5859 2229 2e73 6c6f 7432  lane("XY").slot2
-00021280: 4428 342c 2031 2c20 3435 292e 6578 7472  D(4, 1, 45).extr
-00021290: 7564 6528 3129 0a20 2020 2020 2020 2070  ude(1).        p
-000212a0: 6f69 6e74 203d 2072 6573 756c 742e 6661  oint = result.fa
-000212b0: 6365 7328 223e 5a22 292e 6564 6765 7328  ces(">Z").edges(
-000212c0: 223e 5822 292e 6669 7273 7428 292e 7661  ">X").first().va
-000212d0: 6c28 292e 7374 6172 7450 6f69 6e74 2829  l().startPoint()
-000212e0: 2e74 6f54 7570 6c65 2829 0a20 2020 2020  .toTuple().     
-000212f0: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
-00021300: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
-00021310: 0a20 2020 2020 2020 2020 2020 2070 6f69  .            poi
-00021320: 6e74 2c20 2830 2e37 3037 3130 3637 3831  nt, (0.707106781
-00021330: 2c20 312e 3431 3432 3133 3536 322c 2031  , 1.414213562, 1
-00021340: 2e30 292c 2064 6563 696d 616c 5f70 6c61  .0), decimal_pla
-00021350: 6365 730a 2020 2020 2020 2020 290a 0a20  ces.        ).. 
-00021360: 2020 2064 6566 2074 6573 745f 6173 7365     def test_asse
-00021370: 6d62 6c65 4564 6765 7328 7365 6c66 293a  mbleEdges(self):
-00021380: 0a0a 2020 2020 2020 2020 2320 506c 6174  ..        # Plat
-00021390: 6520 7769 7468 2035 2073 6964 6573 2061  e with 5 sides a
-000213a0: 6e64 2032 2062 756d 7073 2c20 6f6e 6520  nd 2 bumps, one 
-000213b0: 7369 6465 2069 7320 6e6f 7420 636f 2d70  side is not co-p
-000213c0: 6c61 6e61 7220 7769 7468 2074 6865 206f  lanar with the o
-000213d0: 7468 6572 2073 6964 6573 0a20 2020 2020  ther sides.     
-000213e0: 2020 2023 2050 6173 7365 7320 616e 206f     # Passes an o
-000213f0: 7065 6e20 7769 7265 2074 6f20 6173 7365  pen wire to asse
-00021400: 6d62 6c65 4564 6765 7320 736f 2074 6861  mbleEdges so tha
-00021410: 7420 4973 446f 6e65 2069 7320 7472 7565  t IsDone is true
-00021420: 2062 7574 2045 7272 6f72 2072 6574 7572   but Error retur
-00021430: 6e73 2032 2074 6f20 7465 7374 2074 6865  ns 2 to test the
-00021440: 2077 6172 6e69 6e67 2066 756e 6374 696f   warning functio
-00021450: 6e61 6c69 7479 2e0a 2020 2020 2020 2020  nality..        
-00021460: 6564 6765 5f70 6f69 6e74 7320 3d20 5b0a  edge_points = [.
-00021470: 2020 2020 2020 2020 2020 2020 5b2d 372e              [-7.
-00021480: 302c 202d 372e 302c 2030 2e30 5d2c 0a20  0, -7.0, 0.0],. 
-00021490: 2020 2020 2020 2020 2020 205b 2d33 2e30             [-3.0
-000214a0: 2c20 2d31 302e 302c 2033 2e30 5d2c 0a20  , -10.0, 3.0],. 
-000214b0: 2020 2020 2020 2020 2020 205b 372e 302c             [7.0,
-000214c0: 202d 372e 302c 2030 2e30 5d2c 0a20 2020   -7.0, 0.0],.   
-000214d0: 2020 2020 2020 2020 205b 372e 302c 2037           [7.0, 7
-000214e0: 2e30 2c20 302e 305d 2c0a 2020 2020 2020  .0, 0.0],.      
-000214f0: 2020 2020 2020 5b2d 372e 302c 2037 2e30        [-7.0, 7.0
-00021500: 2c20 302e 305d 2c0a 2020 2020 2020 2020  , 0.0],.        
-00021510: 5d0a 2020 2020 2020 2020 6564 6765 5f77  ].        edge_w
-00021520: 6972 6520 3d20 576f 726b 706c 616e 6528  ire = Workplane(
-00021530: 2258 5922 292e 706f 6c79 6c69 6e65 280a  "XY").polyline(.
-00021540: 2020 2020 2020 2020 2020 2020 5b28 2d37              [(-7
-00021550: 2e30 2c20 2d37 2e30 292c 2028 372e 302c  .0, -7.0), (7.0,
-00021560: 202d 372e 3029 2c20 2837 2e30 2c20 372e   -7.0), (7.0, 7.
-00021570: 3029 2c20 282d 372e 302c 2037 2e30 295d  0), (-7.0, 7.0)]
-00021580: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00021590: 2020 2065 6467 655f 7769 7265 203d 2065     edge_wire = e
-000215a0: 6467 655f 7769 7265 2e61 6464 280a 2020  dge_wire.add(.  
-000215b0: 2020 2020 2020 2020 2020 576f 726b 706c            Workpl
-000215c0: 616e 6528 2259 5a22 290a 2020 2020 2020  ane("YZ").      
-000215d0: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
-000215e0: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-000215f0: 7472 616e 7366 6f72 6d65 6428 6f66 6673  transformed(offs
-00021600: 6574 3d56 6563 746f 7228 302c 2030 2c20  et=Vector(0, 0, 
-00021610: 2d37 292c 2072 6f74 6174 653d 5665 6374  -7), rotate=Vect
-00021620: 6f72 2834 352c 2030 2c20 3029 290a 2020  or(45, 0, 0)).  
-00021630: 2020 2020 2020 2020 2020 2e73 706c 696e            .splin
-00021640: 6528 5b28 2d37 2e30 2c20 302e 3029 2c20  e([(-7.0, 0.0), 
-00021650: 2833 2c20 2d33 292c 2028 372e 302c 2030  (3, -3), (7.0, 0
-00021660: 2e30 295d 290a 2020 2020 2020 2020 290a  .0)]).        ).
-00021670: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
-00021680: 6520 3d20 5b6f 2e76 616c 7328 295b 305d  e = [o.vals()[0]
-00021690: 2066 6f72 206f 2069 6e20 6564 6765 5f77   for o in edge_w
-000216a0: 6972 652e 616c 6c28 295d 0a20 2020 2020  ire.all()].     
-000216b0: 2020 2065 6467 655f 7769 7265 203d 2057     edge_wire = W
-000216c0: 6972 652e 6173 7365 6d62 6c65 4564 6765  ire.assembleEdge
-000216d0: 7328 6564 6765 5f77 6972 6529 0a0a 2020  s(edge_wire)..  
-000216e0: 2020 2020 2020 2320 456d 626f 7373 6564        # Embossed
-000216f0: 2073 7461 722c 206e 6565 6420 746f 2063   star, need to c
-00021700: 6861 6e67 6520 6f70 7469 6f6e 616c 2070  hange optional p
-00021710: 6172 616d 6574 6572 7320 746f 206f 6274  arameters to obt
-00021720: 6169 6e20 6e69 6365 206c 6f6f 6b69 6e67  ain nice looking
-00021730: 2072 6573 756c 742e 0a20 2020 2020 2020   result..       
-00021740: 2072 3120 3d20 332e 300a 2020 2020 2020   r1 = 3.0.      
-00021750: 2020 7232 203d 2031 302e 300a 2020 2020    r2 = 10.0.    
-00021760: 2020 2020 666e 203d 2036 0a20 2020 2020      fn = 6.     
-00021770: 2020 2065 6467 655f 706f 696e 7473 203d     edge_points =
-00021780: 205b 0a20 2020 2020 2020 2020 2020 205b   [.            [
-00021790: 7231 202a 206d 6174 682e 636f 7328 6920  r1 * math.cos(i 
-000217a0: 2a20 6d61 7468 2e70 6920 2f20 666e 292c  * math.pi / fn),
-000217b0: 2072 3120 2a20 6d61 7468 2e73 696e 2869   r1 * math.sin(i
-000217c0: 202a 206d 6174 682e 7069 202f 2066 6e29   * math.pi / fn)
-000217d0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-000217e0: 2069 2025 2032 203d 3d20 300a 2020 2020   i % 2 == 0.    
-000217f0: 2020 2020 2020 2020 656c 7365 205b 7232          else [r2
-00021800: 202a 206d 6174 682e 636f 7328 6920 2a20   * math.cos(i * 
-00021810: 6d61 7468 2e70 6920 2f20 666e 292c 2072  math.pi / fn), r
-00021820: 3220 2a20 6d61 7468 2e73 696e 2869 202a  2 * math.sin(i *
-00021830: 206d 6174 682e 7069 202f 2066 6e29 5d0a   math.pi / fn)].
-00021840: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00021850: 6920 696e 2072 616e 6765 2832 202a 2066  i in range(2 * f
-00021860: 6e20 2b20 3129 0a20 2020 2020 2020 205d  n + 1).        ]
-00021870: 0a20 2020 2020 2020 2065 6467 655f 7769  .        edge_wi
-00021880: 7265 203d 2057 6f72 6b70 6c61 6e65 2822  re = Workplane("
-00021890: 5859 2229 2e70 6f6c 796c 696e 6528 6564  XY").polyline(ed
-000218a0: 6765 5f70 6f69 6e74 7329 0a20 2020 2020  ge_points).     
-000218b0: 2020 2065 6467 655f 7769 7265 203d 205b     edge_wire = [
-000218c0: 6f2e 7661 6c73 2829 5b30 5d20 666f 7220  o.vals()[0] for 
-000218d0: 6f20 696e 2065 6467 655f 7769 7265 2e61  o in edge_wire.a
-000218e0: 6c6c 2829 5d0a 2020 2020 2020 2020 6564  ll()].        ed
-000218f0: 6765 5f77 6972 6520 3d20 5769 7265 2e61  ge_wire = Wire.a
-00021900: 7373 656d 626c 6545 6467 6573 2865 6467  ssembleEdges(edg
-00021910: 655f 7769 7265 290a 0a20 2020 2020 2020  e_wire)..       
-00021920: 2023 2050 6f69 6e74 7320 6f6e 2068 6578   # Points on hex
-00021930: 6167 6f6e 616c 2070 6174 7465 726e 2063  agonal pattern c
-00021940: 6f6f 7264 696e 6174 6573 2c20 7573 6520  oordinates, use 
-00021950: 6f66 2070 7573 6870 6f69 6e74 732e 0a20  of pushpoints.. 
-00021960: 2020 2020 2020 2072 3120 3d20 312e 300a         r1 = 1.0.
-00021970: 2020 2020 2020 2020 666e 203d 2036 0a20          fn = 6. 
-00021980: 2020 2020 2020 2065 6467 655f 706f 696e         edge_poin
-00021990: 7473 203d 205b 0a20 2020 2020 2020 2020  ts = [.         
-000219a0: 2020 205b 7231 202a 206d 6174 682e 636f     [r1 * math.co
-000219b0: 7328 6920 2a20 3220 2a20 6d61 7468 2e70  s(i * 2 * math.p
-000219c0: 6920 2f20 666e 292c 2072 3120 2a20 6d61  i / fn), r1 * ma
-000219d0: 7468 2e73 696e 2869 202a 2032 202a 206d  th.sin(i * 2 * m
-000219e0: 6174 682e 7069 202f 2066 6e29 5d0a 2020  ath.pi / fn)].  
-000219f0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00021a00: 696e 2072 616e 6765 2866 6e20 2b20 3129  in range(fn + 1)
-00021a10: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00021a20: 2020 2073 7572 6661 6365 5f70 6f69 6e74     surface_point
-00021a30: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00021a40: 2020 5b30 2e32 352c 2030 2c20 302e 3735    [0.25, 0, 0.75
-00021a50: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00021a60: 2d30 2e32 352c 2030 2c20 302e 3735 5d2c  -0.25, 0, 0.75],
-00021a70: 0a20 2020 2020 2020 2020 2020 205b 302c  .            [0,
-00021a80: 2030 2e32 352c 2030 2e37 355d 2c0a 2020   0.25, 0.75],.  
-00021a90: 2020 2020 2020 2020 2020 5b30 2c20 2d30            [0, -0
-00021aa0: 2e32 352c 2030 2e37 355d 2c0a 2020 2020  .25, 0.75],.    
-00021ab0: 2020 2020 2020 2020 5b30 2c20 302c 2032          [0, 0, 2
-00021ac0: 5d2c 0a20 2020 2020 2020 205d 0a20 2020  ],.        ].   
-00021ad0: 2020 2020 2065 6467 655f 7769 7265 203d       edge_wire =
-00021ae0: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
-00021af0: 2e70 6f6c 796c 696e 6528 6564 6765 5f70  .polyline(edge_p
-00021b00: 6f69 6e74 7329 0a20 2020 2020 2020 2065  oints).        e
-00021b10: 6467 655f 7769 7265 203d 205b 6f2e 7661  dge_wire = [o.va
-00021b20: 6c73 2829 5b30 5d20 666f 7220 6f20 696e  ls()[0] for o in
-00021b30: 2065 6467 655f 7769 7265 2e61 6c6c 2829   edge_wire.all()
-00021b40: 5d0a 2020 2020 2020 2020 6564 6765 5f77  ].        edge_w
-00021b50: 6972 6520 3d20 5769 7265 2e61 7373 656d  ire = Wire.assem
-00021b60: 626c 6545 6467 6573 2865 6467 655f 7769  bleEdges(edge_wi
-00021b70: 7265 290a 0a20 2020 2020 2020 2023 2047  re)..        # G
-00021b80: 7972 6fc3 af64 2c20 616c 6c20 6564 6765  yro..d, all edge
-00021b90: 7320 6172 6520 7370 6c69 6e65 7320 6f6e  s are splines on
-00021ba0: 2064 6966 6665 7265 6e74 2077 6f72 6b70   different workp
-00021bb0: 6c61 6e65 732e 0a20 2020 2020 2020 2065  lanes..        e
-00021bc0: 6467 655f 706f 696e 7473 203d 205b 0a20  dge_points = [. 
-00021bd0: 2020 2020 2020 2020 2020 205b 5b33 2e35             [[3.5
-00021be0: 342c 2033 2e35 345d 2c20 5b31 2e37 372c  4, 3.54], [1.77,
-00021bf0: 2030 2e30 5d2c 205b 332e 3534 2c20 2d33   0.0], [3.54, -3
-00021c00: 2e35 345d 5d2c 0a20 2020 2020 2020 2020  .54]],.         
-00021c10: 2020 205b 5b2d 332e 3534 2c20 2d33 2e35     [[-3.54, -3.5
-00021c20: 345d 2c20 5b30 2e30 2c20 2d31 2e37 375d  4], [0.0, -1.77]
-00021c30: 2c20 5b33 2e35 342c 202d 332e 3534 5d5d  , [3.54, -3.54]]
-00021c40: 2c0a 2020 2020 2020 2020 2020 2020 5b5b  ,.            [[
-00021c50: 2d33 2e35 342c 202d 332e 3534 5d2c 205b  -3.54, -3.54], [
-00021c60: 302e 302c 202d 312e 3737 5d2c 205b 332e  0.0, -1.77], [3.
-00021c70: 3534 2c20 2d33 2e35 345d 5d2c 0a20 2020  54, -3.54]],.   
-00021c80: 2020 2020 2020 2020 205b 5b2d 332e 3534           [[-3.54
-00021c90: 2c20 2d33 2e35 345d 2c20 5b2d 312e 3737  , -3.54], [-1.77
-00021ca0: 2c20 302e 305d 2c20 5b2d 332e 3534 2c20  , 0.0], [-3.54, 
-00021cb0: 332e 3534 5d5d 2c0a 2020 2020 2020 2020  3.54]],.        
-00021cc0: 2020 2020 5b5b 332e 3534 2c20 332e 3534      [[3.54, 3.54
-00021cd0: 5d2c 205b 302e 302c 2031 2e37 375d 2c20  ], [0.0, 1.77], 
-00021ce0: 5b2d 332e 3534 2c20 332e 3534 5d5d 2c0a  [-3.54, 3.54]],.
-00021cf0: 2020 2020 2020 2020 2020 2020 5b5b 332e              [[3.
-00021d00: 3534 2c20 332e 3534 5d2c 205b 302e 302c  54, 3.54], [0.0,
-00021d10: 2031 2e37 375d 2c20 5b2d 332e 3534 2c20   1.77], [-3.54, 
-00021d20: 332e 3534 5d5d 2c0a 2020 2020 2020 2020  3.54]],.        
-00021d30: 5d0a 2020 2020 2020 2020 706c 616e 655f  ].        plane_
-00021d40: 6c69 7374 203d 205b 2258 5a22 2c20 2258  list = ["XZ", "X
-00021d50: 5922 2c20 2259 5a22 2c20 2258 5a22 2c20  Y", "YZ", "XZ", 
-00021d60: 2259 5a22 2c20 2258 5922 5d0a 2020 2020  "YZ", "XY"].    
-00021d70: 2020 2020 6f66 6673 6574 5f6c 6973 7420      offset_list 
-00021d80: 3d20 5b2d 332e 3534 2c20 332e 3534 2c20  = [-3.54, 3.54, 
-00021d90: 332e 3534 2c20 332e 3534 2c20 2d33 2e35  3.54, 3.54, -3.5
-00021da0: 342c 202d 332e 3534 5d0a 2020 2020 2020  4, -3.54].      
-00021db0: 2020 6564 6765 5f77 6972 6520 3d20 280a    edge_wire = (.
-00021dc0: 2020 2020 2020 2020 2020 2020 576f 726b              Work
-00021dd0: 706c 616e 6528 706c 616e 655f 6c69 7374  plane(plane_list
-00021de0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-00021df0: 202e 776f 726b 706c 616e 6528 6f66 6673   .workplane(offs
-00021e00: 6574 3d2d 6f66 6673 6574 5f6c 6973 745b  et=-offset_list[
-00021e10: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00021e20: 2e73 706c 696e 6528 6564 6765 5f70 6f69  .spline(edge_poi
-00021e30: 6e74 735b 305d 290a 2020 2020 2020 2020  nts[0]).        
-00021e40: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
-00021e50: 696e 2072 616e 6765 286c 656e 2865 6467  in range(len(edg
-00021e60: 655f 706f 696e 7473 2920 2d20 3129 3a0a  e_points) - 1):.
-00021e70: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-00021e80: 5f77 6972 6520 3d20 6564 6765 5f77 6972  _wire = edge_wir
-00021e90: 652e 6164 6428 0a20 2020 2020 2020 2020  e.add(.         
-00021ea0: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
-00021eb0: 2870 6c61 6e65 5f6c 6973 745b 6920 2b20  (plane_list[i + 
-00021ec0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-00021ed0: 2020 2020 2e77 6f72 6b70 6c61 6e65 286f      .workplane(o
-00021ee0: 6666 7365 743d 2d6f 6666 7365 745f 6c69  ffset=-offset_li
-00021ef0: 7374 5b69 202b 2031 5d29 0a20 2020 2020  st[i + 1]).     
-00021f00: 2020 2020 2020 2020 2020 202e 7370 6c69             .spli
-00021f10: 6e65 2865 6467 655f 706f 696e 7473 5b69  ne(edge_points[i
-00021f20: 202b 2031 5d29 0a20 2020 2020 2020 2020   + 1]).         
-00021f30: 2020 2029 0a20 2020 2020 2020 2065 6467     ).        edg
-00021f40: 655f 7769 7265 203d 205b 6f2e 7661 6c73  e_wire = [o.vals
-00021f50: 2829 5b30 5d20 666f 7220 6f20 696e 2065  ()[0] for o in e
-00021f60: 6467 655f 7769 7265 2e61 6c6c 2829 5d0a  dge_wire.all()].
-00021f70: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
-00021f80: 6520 3d20 5769 7265 2e61 7373 656d 626c  e = Wire.assembl
-00021f90: 6545 6467 6573 2865 6467 655f 7769 7265  eEdges(edge_wire
-00021fa0: 290a 0a20 2020 2064 6566 2074 6573 7454  )..    def testT
-00021fb0: 6167 2873 656c 6629 3a0a 0a20 2020 2020  ag(self):..     
-00021fc0: 2020 2023 2074 6573 7420 7461 6767 696e     # test taggin
-00021fd0: 670a 2020 2020 2020 2020 7265 7375 6c74  g.        result
-00021fe0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00021ff0: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
-00022000: 0a20 2020 2020 2020 2020 2020 202e 7075  .            .pu
-00022010: 7368 506f 696e 7473 285b 282d 322c 2030  shPoints([(-2, 0
-00022020: 292c 2028 322c 2030 295d 290a 2020 2020  ), (2, 0)]).    
-00022030: 2020 2020 2020 2020 2e62 6f78 2831 2c20          .box(1, 
-00022040: 312c 2031 2c20 636f 6d62 696e 653d 4661  1, 1, combine=Fa
-00022050: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00022060: 202e 7461 6728 2232 2073 6f6c 6964 7322   .tag("2 solids"
-00022070: 290a 2020 2020 2020 2020 2020 2020 2e75  ).            .u
-00022080: 6e69 6f6e 2857 6f72 6b70 6c61 6e65 2822  nion(Workplane("
-00022090: 5859 2229 2e62 6f78 2836 2c20 312c 2031  XY").box(6, 1, 1
-000220a0: 2929 0a20 2020 2020 2020 2029 0a20 2020  )).        ).   
-000220b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000220c0: 4571 7561 6c28 6c65 6e28 7265 7375 6c74  Equal(len(result
-000220d0: 2e6f 626a 6563 7473 292c 2031 290a 2020  .objects), 1).  
-000220e0: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
-000220f0: 6573 756c 742e 5f67 6574 5461 6767 6564  esult._getTagged
-00022100: 2822 3220 736f 6c69 6473 2229 0a20 2020  ("2 solids").   
-00022110: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00022120: 4571 7561 6c28 6c65 6e28 7265 7375 6c74  Equal(len(result
-00022130: 2e6f 626a 6563 7473 292c 2032 290a 0a20  .objects), 2).. 
-00022140: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00022150: 2e61 7373 6572 7452 6169 7365 7328 5661  .assertRaises(Va
-00022160: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
-00022170: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00022180: 7265 7375 6c74 2e5f 6765 7454 6167 6765  result._getTagge
-00022190: 6428 2233 2073 6f6c 6964 7322 290a 0a20  d("3 solids").. 
-000221a0: 2020 2064 6566 2074 6573 7443 6f70 7957     def testCopyW
-000221b0: 6f72 6b70 6c61 6e65 2873 656c 6629 3a0a  orkplane(self):.
-000221c0: 0a20 2020 2020 2020 206f 626a 3020 3d20  .        obj0 = 
-000221d0: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
-000221e0: 626f 7828 312c 2031 2c20 3130 292e 6661  box(1, 1, 10).fa
-000221f0: 6365 7328 223e 5a22 292e 776f 726b 706c  ces(">Z").workpl
-00022200: 616e 6528 290a 2020 2020 2020 2020 6f62  ane().        ob
-00022210: 6a31 203d 2057 6f72 6b70 6c61 6e65 2822  j1 = Workplane("
-00022220: 5859 2229 2e63 6f70 7957 6f72 6b70 6c61  XY").copyWorkpla
-00022230: 6e65 286f 626a 3029 2e62 6f78 2831 2c20  ne(obj0).box(1, 
-00022240: 312c 2031 290a 2020 2020 2020 2020 7365  1, 1).        se
-00022250: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
-00022260: 6d6f 7374 4571 7561 6c73 2828 302c 2030  mostEquals((0, 0
-00022270: 2c20 3529 2c20 6f62 6a31 2e76 616c 2829  , 5), obj1.val()
-00022280: 2e43 656e 7465 7228 292e 746f 5475 706c  .Center().toTupl
-00022290: 6528 292c 2039 290a 0a20 2020 2064 6566  e(), 9)..    def
-000222a0: 2074 6573 7457 6f72 6b70 6c61 6e65 4672   testWorkplaneFr
-000222b0: 6f6d 5461 6767 6564 2873 656c 6629 3a0a  omTagged(self):.
-000222c0: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-000222d0: 6520 6120 666c 6174 2c20 7769 6465 2062  e a flat, wide b
-000222e0: 6173 652e 2045 7874 7275 6465 206f 6e65  ase. Extrude one
-000222f0: 206f 626a 6563 7420 3420 756e 6974 7320   object 4 units 
-00022300: 6869 6768 2c20 616e 6f74 6865 720a 2020  high, another.  
-00022310: 2020 2020 2020 2320 6f62 6a65 6374 206f        # object o
-00022320: 6e20 746f 7020 6f66 2069 7420 3620 756e  n top of it 6 un
-00022330: 6974 7320 6869 6768 2e20 476f 2062 6163  its high. Go bac
-00022340: 6b20 746f 2062 6173 6520 706c 616e 652e  k to base plane.
-00022350: 2045 7874 7275 6465 2061 6e0a 2020 2020   Extrude an.    
-00022360: 2020 2020 2320 6f62 6a65 6374 2031 3120      # object 11 
-00022370: 756e 6974 7320 6869 6768 2e20 4173 7365  units high. Asse
-00022380: 7274 2074 6861 7420 746f 7020 6661 6365  rt that top face
-00022390: 2069 7320 3131 2075 6e69 7473 2068 6967   is 11 units hig
-000223a0: 682e 0a20 2020 2020 2020 2072 6573 756c  h..        resul
-000223b0: 7420 3d20 280a 2020 2020 2020 2020 2020  t = (.          
-000223c0: 2020 576f 726b 706c 616e 6528 2258 5922    Workplane("XY"
-000223d0: 290a 2020 2020 2020 2020 2020 2020 2e62  ).            .b
-000223e0: 6f78 2831 302c 2031 302c 2031 2c20 6365  ox(10, 10, 1, ce
-000223f0: 6e74 6572 6564 3d28 5472 7565 2c20 5472  ntered=(True, Tr
-00022400: 7565 2c20 4661 6c73 6529 290a 2020 2020  ue, False)).    
-00022410: 2020 2020 2020 2020 2e66 6163 6573 2822          .faces("
-00022420: 3e5a 2229 0a20 2020 2020 2020 2020 2020  >Z").           
-00022430: 202e 776f 726b 706c 616e 6528 290a 2020   .workplane().  
-00022440: 2020 2020 2020 2020 2020 2e74 6167 2822            .tag("
-00022450: 6261 7365 2229 0a20 2020 2020 2020 2020  base").         
-00022460: 2020 202e 6365 6e74 6572 2833 2c20 3029     .center(3, 0)
-00022470: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
-00022480: 6374 2832 2c20 3229 0a20 2020 2020 2020  ct(2, 2).       
-00022490: 2020 2020 202e 6578 7472 7564 6528 3429       .extrude(4)
-000224a0: 0a20 2020 2020 2020 2020 2020 202e 6661  .            .fa
-000224b0: 6365 7328 223e 5a22 290a 2020 2020 2020  ces(">Z").      
-000224c0: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
-000224d0: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-000224e0: 6369 7263 6c65 2831 290a 2020 2020 2020  circle(1).      
-000224f0: 2020 2020 2020 2e65 7874 7275 6465 2836        .extrude(6
-00022500: 290a 2020 2020 2020 2020 2020 2020 2e77  ).            .w
-00022510: 6f72 6b70 6c61 6e65 4672 6f6d 5461 6767  orkplaneFromTagg
-00022520: 6564 2822 6261 7365 2229 0a20 2020 2020  ed("base").     
-00022530: 2020 2020 2020 202e 6365 6e74 6572 282d         .center(-
-00022540: 332c 2030 290a 2020 2020 2020 2020 2020  3, 0).          
-00022550: 2020 2e63 6972 636c 6528 3129 0a20 2020    .circle(1).   
-00022560: 2020 2020 2020 2020 202e 6578 7472 7564           .extrud
-00022570: 6528 3131 290a 2020 2020 2020 2020 290a  e(11).        ).
-00022580: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00022590: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
-000225a0: 7561 6c73 280a 2020 2020 2020 2020 2020  uals(.          
-000225b0: 2020 7265 7375 6c74 2e66 6163 6573 2822    result.faces("
-000225c0: 3e5a 2229 2e76 616c 2829 2e43 656e 7465  >Z").val().Cente
-000225d0: 7228 292e 746f 5475 706c 6528 292c 2028  r().toTuple(), (
-000225e0: 2d33 2c20 302c 2031 3229 2c20 390a 2020  -3, 0, 12), 9.  
-000225f0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00022600: 2074 6573 7457 6f72 6b70 6c61 6e65 4f72   testWorkplaneOr
-00022610: 6965 6e74 6174 696f 6e4f 6e56 6572 7465  ientationOnVerte
-00022620: 7828 7365 6c66 293a 0a0a 2020 2020 2020  x(self):..      
-00022630: 2020 2320 6372 6561 7465 2061 2031 3020    # create a 10 
-00022640: 756e 6974 2073 697a 6564 2063 7562 6520  unit sized cube 
-00022650: 6f6e 2074 6865 2058 5920 706c 616e 650a  on the XY plane.
-00022660: 2020 2020 2020 2020 7061 7265 6e74 203d          parent =
-00022670: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
-00022680: 2e72 6563 7428 3130 2e30 2c20 3130 2e30  .rect(10.0, 10.0
-00022690: 292e 6578 7472 7564 6528 3130 290a 0a20  ).extrude(10).. 
-000226a0: 2020 2020 2020 2023 2061 7373 6572 7420         # assert 
-000226b0: 7468 6174 2074 6865 2064 6972 6563 7469  that the directi
-000226c0: 6f6e 2074 7570 6c65 7320 7265 666c 6563  on tuples reflec
-000226d0: 7420 6163 636f 7264 696e 676c 790a 2020  t accordingly.  
-000226e0: 2020 2020 2020 6173 7365 7274 2070 6172        assert par
-000226f0: 656e 742e 706c 616e 652e 7844 6972 2e74  ent.plane.xDir.t
-00022700: 6f54 7570 6c65 2829 203d 3d20 6170 7072  oTuple() == appr
-00022710: 6f78 2828 312e 302c 2030 2e30 2c20 302e  ox((1.0, 0.0, 0.
-00022720: 3029 290a 2020 2020 2020 2020 6173 7365  0)).        asse
-00022730: 7274 2070 6172 656e 742e 706c 616e 652e  rt parent.plane.
-00022740: 7a44 6972 2e74 6f54 7570 6c65 2829 203d  zDir.toTuple() =
-00022750: 3d20 6170 7072 6f78 2828 302e 302c 2030  = approx((0.0, 0
-00022760: 2e30 2c20 312e 3029 290a 0a20 2020 2020  .0, 1.0))..     
-00022770: 2020 2023 2073 656c 6563 7420 7468 6520     # select the 
-00022780: 3c58 5a20 7665 7274 6578 206f 6e20 7468  <XZ vertex on th
-00022790: 6520 3c59 2066 6163 6520 616e 6420 6372  e <Y face and cr
-000227a0: 6561 7465 2061 206e 6577 2077 6f72 6b70  eate a new workp
-000227b0: 6c61 6e65 2e0a 2020 2020 2020 2020 6368  lane..        ch
-000227c0: 696c 6420 3d20 7061 7265 6e74 2e66 6163  ild = parent.fac
-000227d0: 6573 2822 3c59 2229 2e76 6572 7469 6365  es("<Y").vertice
-000227e0: 7328 223c 585a 2229 2e77 6f72 6b70 6c61  s("<XZ").workpla
-000227f0: 6e65 2829 0a0a 2020 2020 2020 2020 2320  ne()..        # 
-00022800: 6173 7365 7274 2074 6861 7420 7468 6520  assert that the 
-00022810: 6469 7265 6374 696f 6e20 7475 706c 6573  direction tuples
-00022820: 2072 6566 6c65 6374 2074 6865 206e 6577   reflect the new
-00022830: 2077 6f72 6b70 6c61 6e65 206f 6e20 7468   workplane on th
-00022840: 6520 3c59 2066 6163 650a 2020 2020 2020  e <Y face.      
-00022850: 2020 6173 7365 7274 2063 6869 6c64 2e70    assert child.p
-00022860: 6c61 6e65 2e78 4469 722e 746f 5475 706c  lane.xDir.toTupl
-00022870: 6528 2920 3d3d 2061 7070 726f 7828 2831  e() == approx((1
-00022880: 2e30 2c20 302e 302c 202d 302e 3029 290a  .0, 0.0, -0.0)).
-00022890: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
-000228a0: 6869 6c64 2e70 6c61 6e65 2e7a 4469 722e  hild.plane.zDir.
-000228b0: 746f 5475 706c 6528 2920 3d3d 2061 7070  toTuple() == app
-000228c0: 726f 7828 2830 2e30 2c20 2d31 2e30 2c20  rox((0.0, -1.0, 
-000228d0: 2d30 2e30 2929 0a0a 2020 2020 6465 6620  -0.0))..    def 
-000228e0: 7465 7374 5461 6753 656c 6563 746f 7273  testTagSelectors
-000228f0: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
-00022900: 2072 6573 756c 7430 203d 2057 6f72 6b70   result0 = Workp
-00022910: 6c61 6e65 2822 5859 2229 2e62 6f78 2831  lane("XY").box(1
-00022920: 2c20 312c 2031 292e 7461 6728 2262 6f78  , 1, 1).tag("box
-00022930: 2229 2e73 7068 6572 6528 3129 0a20 2020  ").sphere(1).   
-00022940: 2020 2020 2023 2072 6573 756c 7420 6973       # result is
-00022950: 2063 7572 7265 6e74 6c79 2061 2073 7068   currently a sph
-00022960: 6572 650a 2020 2020 2020 2020 7365 6c66  ere.        self
-00022970: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
-00022980: 7265 7375 6c74 302e 6661 6365 7328 292e  result0.faces().
-00022990: 7369 7a65 2829 290a 2020 2020 2020 2020  size()).        
-000229a0: 2320 6120 626f 7820 6861 7320 3820 7665  # a box has 8 ve
-000229b0: 7274 6963 6573 0a20 2020 2020 2020 2073  rtices.        s
-000229c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000229d0: 382c 2072 6573 756c 7430 2e76 6572 7469  8, result0.verti
-000229e0: 6365 7328 7461 673d 2262 6f78 2229 2e73  ces(tag="box").s
-000229f0: 697a 6528 2929 0a20 2020 2020 2020 2023  ize()).        #
-00022a00: 2036 2066 6163 6573 0a20 2020 2020 2020   6 faces.       
-00022a10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00022a20: 6c28 362c 2072 6573 756c 7430 2e66 6163  l(6, result0.fac
-00022a30: 6573 2874 6167 3d22 626f 7822 292e 7369  es(tag="box").si
-00022a40: 7a65 2829 290a 2020 2020 2020 2020 2320  ze()).        # 
-00022a50: 3132 2065 6467 6573 0a20 2020 2020 2020  12 edges.       
-00022a60: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00022a70: 6c28 3132 2c20 7265 7375 6c74 302e 6564  l(12, result0.ed
-00022a80: 6765 7328 7461 673d 2262 6f78 2229 2e73  ges(tag="box").s
-00022a90: 697a 6528 2929 0a20 2020 2020 2020 2023  ize()).        #
-00022aa0: 2036 2077 6972 6573 0a20 2020 2020 2020   6 wires.       
-00022ab0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00022ac0: 6c28 362c 2072 6573 756c 7430 2e77 6972  l(6, result0.wir
-00022ad0: 6573 2874 6167 3d22 626f 7822 292e 7369  es(tag="box").si
-00022ae0: 7a65 2829 290a 0a20 2020 2020 2020 2023  ze())..        #
-00022af0: 2063 7265 6174 6520 7477 6f20 736f 6c69   create two soli
-00022b00: 6473 2c20 7461 6720 7468 656d 2c20 6a6f  ds, tag them, jo
-00022b10: 696e 2074 6f20 6f6e 6520 736f 6c69 640a  in to one solid.
-00022b20: 2020 2020 2020 2020 7265 7375 6c74 3120          result1 
-00022b30: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00022b40: 576f 726b 706c 616e 6528 2258 5922 290a  Workplane("XY").
-00022b50: 2020 2020 2020 2020 2020 2020 2e70 7573              .pus
-00022b60: 6850 6f69 6e74 7328 5b28 312c 2030 292c  hPoints([(1, 0),
-00022b70: 2028 2d31 2c20 3029 5d29 0a20 2020 2020   (-1, 0)]).     
-00022b80: 2020 2020 2020 202e 626f 7828 312c 2031         .box(1, 1
-00022b90: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-00022ba0: 202e 7461 6728 2262 6f78 6573 2229 0a20   .tag("boxes"). 
-00022bb0: 2020 2020 2020 2020 2020 202e 7370 6865             .sphe
-00022bc0: 7265 2831 290a 2020 2020 2020 2020 290a  re(1).        ).
-00022bd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00022be0: 6572 7445 7175 616c 2831 2c20 7265 7375  ertEqual(1, resu
-00022bf0: 6c74 312e 736f 6c69 6473 2829 2e73 697a  lt1.solids().siz
-00022c00: 6528 2929 0a20 2020 2020 2020 2073 656c  e()).        sel
-00022c10: 662e 6173 7365 7274 4571 7561 6c28 322c  f.assertEqual(2,
-00022c20: 2072 6573 756c 7431 2e73 6f6c 6964 7328   result1.solids(
-00022c30: 7461 673d 2262 6f78 6573 2229 2e73 697a  tag="boxes").siz
-00022c40: 6528 2929 0a20 2020 2020 2020 2073 656c  e()).        sel
-00022c50: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
-00022c60: 2072 6573 756c 7431 2e73 6865 6c6c 7328   result1.shells(
-00022c70: 292e 7369 7a65 2829 290a 2020 2020 2020  ).size()).      
-00022c80: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00022c90: 616c 2832 2c20 7265 7375 6c74 312e 7368  al(2, result1.sh
-00022ca0: 656c 6c73 2874 6167 3d22 626f 7865 7322  ells(tag="boxes"
-00022cb0: 292e 7369 7a65 2829 290a 0a20 2020 2020  ).size())..     
-00022cc0: 2020 2023 2063 7265 6174 6520 3420 696e     # create 4 in
-00022cd0: 6469 7669 6475 616c 206f 626a 6563 7473  dividual objects
-00022ce0: 2c20 7461 6720 6974 2c20 7468 656e 2063  , tag it, then c
-00022cf0: 6f6d 6269 6e65 2074 6f20 6f6e 6520 636f  ombine to one co
-00022d00: 6d70 6f75 6e64 0a20 2020 2020 2020 2072  mpound.        r
-00022d10: 6573 756c 7432 203d 2028 0a20 2020 2020  esult2 = (.     
-00022d20: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
-00022d30: 2822 5859 2229 0a20 2020 2020 2020 2020  ("XY").         
-00022d40: 2020 202e 7265 6374 2834 2c20 3429 0a20     .rect(4, 4). 
-00022d50: 2020 2020 2020 2020 2020 202e 7665 7274             .vert
-00022d60: 6963 6573 2829 0a20 2020 2020 2020 2020  ices().         
-00022d70: 2020 202e 626f 7828 312c 2031 2c20 312c     .box(1, 1, 1,
-00022d80: 2063 6f6d 6269 6e65 3d46 616c 7365 290a   combine=False).
-00022d90: 2020 2020 2020 2020 2020 2020 2e74 6167              .tag
-00022da0: 2822 3420 6f62 6a73 2229 0a20 2020 2020  ("4 objs").     
-00022db0: 2020 2029 0a20 2020 2020 2020 2072 6573     ).        res
-00022dc0: 756c 7432 203d 2072 6573 756c 7432 2e6e  ult2 = result2.n
-00022dd0: 6577 4f62 6a65 6374 285b 436f 6d70 6f75  ewObject([Compou
-00022de0: 6e64 2e6d 616b 6543 6f6d 706f 756e 6428  nd.makeCompound(
-00022df0: 7265 7375 6c74 322e 6f62 6a65 6374 7329  result2.objects)
-00022e00: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
-00022e10: 6173 7365 7274 4571 7561 6c28 312c 2072  assertEqual(1, r
-00022e20: 6573 756c 7432 2e63 6f6d 706f 756e 6473  esult2.compounds
-00022e30: 2829 2e73 697a 6528 2929 0a20 2020 2020  ().size()).     
-00022e40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00022e50: 7561 6c28 302c 2072 6573 756c 7432 2e63  ual(0, result2.c
-00022e60: 6f6d 706f 756e 6473 2874 6167 3d22 3420  ompounds(tag="4 
-00022e70: 6f62 6a73 2229 2e73 697a 6528 2929 0a0a  objs").size())..
-00022e80: 2020 2020 6465 6620 7465 7374 5f69 6e74      def test_int
-00022e90: 6572 7050 6c61 7465 2873 656c 6629 3a0a  erpPlate(self):.
-00022ea0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00022eb0: 2020 2020 5465 7374 7320 7468 6520 696e      Tests the in
-00022ec0: 7465 7270 506c 6174 6528 2920 6675 6e63  terpPlate() func
-00022ed0: 7469 6f6e 616c 6974 6965 730a 2020 2020  tionalities.    
-00022ee0: 2020 2020 4e75 6d65 7269 6361 6c20 7661      Numerical va
-00022ef0: 6c75 6573 206f 6620 4172 6561 7320 616e  lues of Areas an
-00022f00: 6420 566f 6c75 6d65 7320 7765 7265 206f  d Volumes were o
-00022f10: 6274 6169 6e65 6420 7769 7468 2074 6865  btained with the
-00022f20: 2041 7265 6128 2920 616e 6420 566f 6c75   Area() and Volu
-00022f30: 6d65 2829 2066 756e 6374 696f 6e73 206f  me() functions o
-00022f40: 6e20 6120 4c69 6e75 7820 6d61 6368 696e  n a Linux machin
-00022f50: 6520 756e 6465 7220 4465 6269 616e 2031  e under Debian 1
-00022f60: 3020 7769 7468 2070 7974 686f 6e20 332e  0 with python 3.
-00022f70: 372e 0a20 2020 2020 2020 2022 2222 0a0a  7..        """..
-00022f80: 2020 2020 2020 2020 2320 6578 616d 706c          # exampl
-00022f90: 6520 6672 6f6d 2050 7974 686f 6e4f 4343  e from PythonOCC
-00022fa0: 2063 6f72 655f 6765 6f6d 6574 7279 5f67   core_geometry_g
-00022fb0: 656f 6d70 6c61 7465 2e70 792c 2075 7365  eomplate.py, use
-00022fc0: 206f 6620 7468 6963 6b6e 6573 7320 3d20   of thickness = 
-00022fd0: 3020 7265 7475 726e 7320 3244 2073 7572  0 returns 2D sur
-00022fe0: 6661 6365 2e0a 2020 2020 2020 2020 7468  face..        th
-00022ff0: 6963 6b6e 6573 7320 3d20 300a 2020 2020  ickness = 0.    
-00023000: 2020 2020 6564 6765 5f70 6f69 6e74 7320      edge_points 
-00023010: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00023020: 2830 2e30 2c20 302e 302c 2030 2e30 292c  (0.0, 0.0, 0.0),
-00023030: 0a20 2020 2020 2020 2020 2020 2028 302e  .            (0.
-00023040: 302c 2031 302e 302c 2030 2e30 292c 0a20  0, 10.0, 0.0),. 
-00023050: 2020 2020 2020 2020 2020 2028 302e 302c             (0.0,
-00023060: 2031 302e 302c 2031 302e 3029 2c0a 2020   10.0, 10.0),.  
-00023070: 2020 2020 2020 2020 2020 2830 2e30 2c20            (0.0, 
-00023080: 302e 302c 2031 302e 3029 2c0a 2020 2020  0.0, 10.0),.    
-00023090: 2020 2020 5d0a 2020 2020 2020 2020 7375      ].        su
-000230a0: 7266 6163 655f 706f 696e 7473 203d 205b  rface_points = [
-000230b0: 2835 2e30 2c20 352e 302c 2035 2e30 295d  (5.0, 5.0, 5.0)]
-000230c0: 0a20 2020 2020 2020 2070 6c61 7465 5f30  .        plate_0
-000230d0: 203d 2057 6f72 6b70 6c61 6e65 2822 5859   = Workplane("XY
-000230e0: 2229 2e69 6e74 6572 7050 6c61 7465 2865  ").interpPlate(e
-000230f0: 6467 655f 706f 696e 7473 2c20 7375 7266  dge_points, surf
-00023100: 6163 655f 706f 696e 7473 2c20 7468 6963  ace_points, thic
-00023110: 6b6e 6573 7329 0a20 2020 2020 2020 2073  kness).        s
-00023120: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
-00023130: 6c61 7465 5f30 2e76 616c 2829 2e69 7356  late_0.val().isV
-00023140: 616c 6964 2829 290a 2020 2020 2020 2020  alid()).        
-00023150: 7365 6c66 2e61 7373 6572 7441 6c6d 6f73  self.assertAlmos
-00023160: 7445 7175 616c 2870 6c61 7465 5f30 2e76  tEqual(plate_0.v
-00023170: 616c 2829 2e41 7265 6128 292c 2031 3431  al().Area(), 141
-00023180: 2e32 3138 3832 3338 3932 2c20 3129 0a0a  .218823892, 1)..
-00023190: 2020 2020 2020 2020 2320 506c 6174 6520          # Plate 
-000231a0: 7769 7468 2035 2073 6964 6573 2061 6e64  with 5 sides and
-000231b0: 2032 2062 756d 7073 2c20 6f6e 6520 7369   2 bumps, one si
-000231c0: 6465 2069 7320 6e6f 7420 636f 2d70 6c61  de is not co-pla
-000231d0: 6e61 7220 7769 7468 2074 6865 206f 7468  nar with the oth
-000231e0: 6572 2073 6964 6573 0a20 2020 2020 2020  er sides.       
-000231f0: 2074 6869 636b 6e65 7373 203d 2030 2e31   thickness = 0.1
-00023200: 0a20 2020 2020 2020 2065 6467 655f 706f  .        edge_po
-00023210: 696e 7473 203d 205b 0a20 2020 2020 2020  ints = [.       
-00023220: 2020 2020 2028 2d37 2e30 2c20 2d37 2e30       (-7.0, -7.0
-00023230: 2c20 302e 3029 2c0a 2020 2020 2020 2020  , 0.0),.        
-00023240: 2020 2020 282d 332e 302c 202d 3130 2e30      (-3.0, -10.0
-00023250: 2c20 332e 3029 2c0a 2020 2020 2020 2020  , 3.0),.        
-00023260: 2020 2020 2837 2e30 2c20 2d37 2e30 2c20      (7.0, -7.0, 
-00023270: 302e 3029 2c0a 2020 2020 2020 2020 2020  0.0),.          
-00023280: 2020 2837 2e30 2c20 372e 302c 2030 2e30    (7.0, 7.0, 0.0
-00023290: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000232a0: 2d37 2e30 2c20 372e 302c 2030 2e30 292c  -7.0, 7.0, 0.0),
-000232b0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-000232c0: 2020 2065 6467 655f 7769 7265 203d 2057     edge_wire = W
-000232d0: 6f72 6b70 6c61 6e65 2822 5859 2229 2e70  orkplane("XY").p
-000232e0: 6f6c 796c 696e 6528 0a20 2020 2020 2020  olyline(.       
-000232f0: 2020 2020 205b 282d 372e 302c 202d 372e       [(-7.0, -7.
-00023300: 3029 2c20 2837 2e30 2c20 2d37 2e30 292c  0), (7.0, -7.0),
-00023310: 2028 372e 302c 2037 2e30 292c 2028 2d37   (7.0, 7.0), (-7
-00023320: 2e30 2c20 372e 3029 5d0a 2020 2020 2020  .0, 7.0)].      
-00023330: 2020 290a 2020 2020 2020 2020 2320 6564    ).        # ed
-00023340: 6765 5f77 6972 6520 3d20 6564 6765 5f77  ge_wire = edge_w
-00023350: 6972 652e 6164 6428 576f 726b 706c 616e  ire.add(Workplan
-00023360: 6528 2759 5a27 292e 776f 726b 706c 616e  e('YZ').workplan
-00023370: 6528 292e 7472 616e 7366 6f72 6d65 6428  e().transformed(
-00023380: 6f66 6673 6574 3d56 6563 746f 7228 302c  offset=Vector(0,
-00023390: 2030 2c20 2d37 292c 2072 6f74 6174 653d   0, -7), rotate=
-000233a0: 5665 6374 6f72 2834 352c 2030 2c20 3029  Vector(45, 0, 0)
-000233b0: 292e 706f 6c79 6c69 6e65 285b 282d 372e  ).polyline([(-7.
-000233c0: 2c30 2e29 2c20 2833 2c2d 3329 2c20 2837  ,0.), (3,-3), (7
-000233d0: 2e2c 302e 295d 2929 0a20 2020 2020 2020  .,0.)])).       
-000233e0: 2023 2049 6e20 4361 6451 7565 7279 2053   # In CadQuery S
-000233f0: 6570 742d 3230 3139 2069 7420 776f 726b  ept-2019 it work
-00023400: 6564 2077 6974 6820 726f 7461 7465 3d56  ed with rotate=V
-00023410: 6563 746f 7228 302c 2034 352c 2030 292e  ector(0, 45, 0).
-00023420: 2049 6e20 4361 6451 7565 7279 2044 6563   In CadQuery Dec
-00023430: 2d32 3031 3920 726f 7461 7465 3d56 6563  -2019 rotate=Vec
-00023440: 746f 7228 3435 2c20 302c 2030 2920 6f6e  tor(45, 0, 0) on
-00023450: 6c79 2063 6c6f 7365 7320 7468 6520 7769  ly closes the wi
-00023460: 7265 2e0a 2020 2020 2020 2020 6564 6765  re..        edge
-00023470: 5f77 6972 6520 3d20 6564 6765 5f77 6972  _wire = edge_wir
-00023480: 652e 6164 6428 0a20 2020 2020 2020 2020  e.add(.         
-00023490: 2020 2057 6f72 6b70 6c61 6e65 2822 595a     Workplane("YZ
-000234a0: 2229 0a20 2020 2020 2020 2020 2020 202e  ").            .
-000234b0: 776f 726b 706c 616e 6528 290a 2020 2020  workplane().    
-000234c0: 2020 2020 2020 2020 2e74 7261 6e73 666f          .transfo
-000234d0: 726d 6564 286f 6666 7365 743d 5665 6374  rmed(offset=Vect
-000234e0: 6f72 2830 2c20 302c 202d 3729 2c20 726f  or(0, 0, -7), ro
-000234f0: 7461 7465 3d56 6563 746f 7228 3435 2c20  tate=Vector(45, 
-00023500: 302c 2030 2929 0a20 2020 2020 2020 2020  0, 0)).         
-00023510: 2020 202e 7370 6c69 6e65 285b 282d 372e     .spline([(-7.
-00023520: 302c 2030 2e30 292c 2028 332c 202d 3329  0, 0.0), (3, -3)
-00023530: 2c20 2837 2e30 2c20 302e 3029 5d29 0a20  , (7.0, 0.0)]). 
-00023540: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023550: 2073 7572 6661 6365 5f70 6f69 6e74 7320   surface_points 
-00023560: 3d20 5b28 2d33 2e30 2c20 2d33 2e30 2c20  = [(-3.0, -3.0, 
-00023570: 2d33 2e30 292c 2028 332e 302c 2033 2e30  -3.0), (3.0, 3.0
-00023580: 2c20 332e 3029 5d0a 2020 2020 2020 2020  , 3.0)].        
-00023590: 706c 6174 655f 3120 3d20 576f 726b 706c  plate_1 = Workpl
-000235a0: 616e 6528 2258 5922 292e 696e 7465 7270  ane("XY").interp
-000235b0: 506c 6174 6528 6564 6765 5f77 6972 652c  Plate(edge_wire,
-000235c0: 2073 7572 6661 6365 5f70 6f69 6e74 732c   surface_points,
-000235d0: 2074 6869 636b 6e65 7373 290a 2020 2020   thickness).    
-000235e0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-000235f0: 7275 6528 706c 6174 655f 312e 7661 6c28  rue(plate_1.val(
-00023600: 292e 6973 5661 6c69 6428 2929 0a20 2020  ).isValid()).   
-00023610: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00023620: 416c 6d6f 7374 4571 7561 6c28 706c 6174  AlmostEqual(plat
-00023630: 655f 312e 7661 6c28 292e 566f 6c75 6d65  e_1.val().Volume
-00023640: 2829 2c20 3236 2e31 3234 3937 3032 3036  (), 26.124970206
-00023650: 2c20 3229 0a0a 2020 2020 2020 2020 2320  , 2)..        # 
-00023660: 456d 626f 7373 6564 2073 7461 722c 206e  Embossed star, n
-00023670: 6565 6420 746f 2063 6861 6e67 6520 6f70  eed to change op
-00023680: 7469 6f6e 616c 2070 6172 616d 6574 6572  tional parameter
-00023690: 7320 746f 206f 6274 6169 6e20 6e69 6365  s to obtain nice
-000236a0: 206c 6f6f 6b69 6e67 2072 6573 756c 742e   looking result.
-000236b0: 0a20 2020 2020 2020 2072 3120 3d20 332e  .        r1 = 3.
-000236c0: 300a 2020 2020 2020 2020 7232 203d 2031  0.        r2 = 1
-000236d0: 302e 300a 2020 2020 2020 2020 666e 203d  0.0.        fn =
-000236e0: 2036 0a20 2020 2020 2020 2074 6869 636b   6.        thick
-000236f0: 6e65 7373 203d 2030 2e31 0a20 2020 2020  ness = 0.1.     
-00023700: 2020 2065 6467 655f 706f 696e 7473 203d     edge_points =
-00023710: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
-00023720: 7231 202a 206d 6174 682e 636f 7328 6920  r1 * math.cos(i 
-00023730: 2a20 6d61 7468 2e70 6920 2f20 666e 292c  * math.pi / fn),
-00023740: 2072 3120 2a20 6d61 7468 2e73 696e 2869   r1 * math.sin(i
-00023750: 202a 206d 6174 682e 7069 202f 2066 6e29   * math.pi / fn)
-00023760: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00023770: 2069 2025 2032 203d 3d20 300a 2020 2020   i % 2 == 0.    
-00023780: 2020 2020 2020 2020 656c 7365 2028 7232          else (r2
-00023790: 202a 206d 6174 682e 636f 7328 6920 2a20   * math.cos(i * 
-000237a0: 6d61 7468 2e70 6920 2f20 666e 292c 2072  math.pi / fn), r
-000237b0: 3220 2a20 6d61 7468 2e73 696e 2869 202a  2 * math.sin(i *
-000237c0: 206d 6174 682e 7069 202f 2066 6e29 290a   math.pi / fn)).
-000237d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000237e0: 6920 696e 2072 616e 6765 2832 202a 2066  i in range(2 * f
-000237f0: 6e20 2b20 3129 0a20 2020 2020 2020 205d  n + 1).        ]
-00023800: 0a20 2020 2020 2020 2065 6467 655f 7769  .        edge_wi
-00023810: 7265 203d 2057 6f72 6b70 6c61 6e65 2822  re = Workplane("
-00023820: 5859 2229 2e70 6f6c 796c 696e 6528 6564  XY").polyline(ed
-00023830: 6765 5f70 6f69 6e74 7329 0a20 2020 2020  ge_points).     
-00023840: 2020 2072 3220 3d20 342e 350a 2020 2020     r2 = 4.5.    
-00023850: 2020 2020 7375 7266 6163 655f 706f 696e      surface_poin
-00023860: 7473 203d 205b 0a20 2020 2020 2020 2020  ts = [.         
-00023870: 2020 2028 7232 202a 206d 6174 682e 636f     (r2 * math.co
-00023880: 7328 6920 2a20 6d61 7468 2e70 6920 2f20  s(i * math.pi / 
-00023890: 666e 292c 2072 3220 2a20 6d61 7468 2e73  fn), r2 * math.s
-000238a0: 696e 2869 202a 206d 6174 682e 7069 202f  in(i * math.pi /
-000238b0: 2066 6e29 2c20 312e 3029 0a20 2020 2020   fn), 1.0).     
-000238c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000238d0: 7261 6e67 6528 3220 2a20 666e 290a 2020  range(2 * fn).  
-000238e0: 2020 2020 2020 5d20 2b20 5b28 302e 302c        ] + [(0.0,
-000238f0: 2030 2e30 2c20 2d32 2e30 295d 0a20 2020   0.0, -2.0)].   
-00023900: 2020 2020 2070 6c61 7465 5f32 203d 2057       plate_2 = W
-00023910: 6f72 6b70 6c61 6e65 2822 5859 2229 2e69  orkplane("XY").i
-00023920: 6e74 6572 7050 6c61 7465 280a 2020 2020  nterpPlate(.    
-00023930: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
-00023940: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
-00023950: 7572 6661 6365 5f70 6f69 6e74 732c 0a20  urface_points,. 
-00023960: 2020 2020 2020 2020 2020 2074 6869 636b             thick
-00023970: 6e65 7373 2c0a 2020 2020 2020 2020 2020  ness,.          
-00023980: 2020 636f 6d62 696e 653d 5472 7565 2c0a    combine=True,.
-00023990: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-000239a0: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
-000239b0: 2020 2020 6465 6772 6565 3d33 2c0a 2020      degree=3,.  
-000239c0: 2020 2020 2020 2020 2020 6e62 5074 734f            nbPtsO
-000239d0: 6e43 7572 3d31 352c 0a20 2020 2020 2020  nCur=15,.       
-000239e0: 2020 2020 206e 6249 7465 723d 322c 0a20       nbIter=2,. 
-000239f0: 2020 2020 2020 2020 2020 2061 6e69 736f             aniso
-00023a00: 7472 6f70 793d 4661 6c73 652c 0a20 2020  tropy=False,.   
-00023a10: 2020 2020 2020 2020 2074 6f6c 3264 3d30           tol2d=0
-00023a20: 2e30 3030 3031 2c0a 2020 2020 2020 2020  .00001,.        
-00023a30: 2020 2020 746f 6c33 643d 302e 3030 3031      tol3d=0.0001
-00023a40: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-00023a50: 6c41 6e67 3d30 2e30 312c 0a20 2020 2020  lAng=0.01,.     
-00023a60: 2020 2020 2020 2074 6f6c 4375 7276 3d30         tolCurv=0
-00023a70: 2e31 2c0a 2020 2020 2020 2020 2020 2020  .1,.            
-00023a80: 6d61 7844 6567 3d38 2c0a 2020 2020 2020  maxDeg=8,.      
-00023a90: 2020 2020 2020 6d61 7853 6567 6d65 6e74        maxSegment
-00023aa0: 733d 3439 2c0a 2020 2020 2020 2020 290a  s=49,.        ).
-00023ab0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00023ac0: 6572 7454 7275 6528 706c 6174 655f 322e  ertTrue(plate_2.
-00023ad0: 7661 6c28 292e 6973 5661 6c69 6428 2929  val().isValid())
-00023ae0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00023af0: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
-00023b00: 706c 6174 655f 322e 7661 6c28 292e 566f  plate_2.val().Vo
-00023b10: 6c75 6d65 2829 2c20 3130 2e39 3536 3035  lume(), 10.95605
-00023b20: 3433 3134 2c20 3029 0a0a 2020 2020 2020  4314, 0)..      
-00023b30: 2020 2320 506f 696e 7473 206f 6e20 6865    # Points on he
-00023b40: 7861 676f 6e61 6c20 7061 7474 6572 6e20  xagonal pattern 
-00023b50: 636f 6f72 6469 6e61 7465 732c 2075 7365  coordinates, use
-00023b60: 206f 6620 7075 7368 706f 696e 7473 2e0a   of pushpoints..
-00023b70: 2020 2020 2020 2020 7231 203d 2031 2e30          r1 = 1.0
-00023b80: 0a20 2020 2020 2020 204e 203d 2033 0a20  .        N = 3. 
-00023b90: 2020 2020 2020 2063 6120 3d20 6d61 7468         ca = math
-00023ba0: 2e63 6f73 2833 302e 3020 2a20 6d61 7468  .cos(30.0 * math
-00023bb0: 2e70 6920 2f20 3138 302e 3029 0a20 2020  .pi / 180.0).   
-00023bc0: 2020 2020 2073 6120 3d20 6d61 7468 2e73       sa = math.s
-00023bd0: 696e 2833 302e 3020 2a20 6d61 7468 2e70  in(30.0 * math.p
-00023be0: 6920 2f20 3138 302e 3029 0a20 2020 2020  i / 180.0).     
-00023bf0: 2020 2023 2045 5645 4e20 524f 5753 0a20     # EVEN ROWS. 
-00023c00: 2020 2020 2020 2070 7473 203d 205b 0a20         pts = [. 
-00023c10: 2020 2020 2020 2020 2020 2028 2d33 2e30             (-3.0
-00023c20: 2c20 2d33 2e30 292c 0a20 2020 2020 2020  , -3.0),.       
-00023c30: 2020 2020 2028 2d31 2e32 3637 3934 392c       (-1.267949,
-00023c40: 202d 332e 3029 2c0a 2020 2020 2020 2020   -3.0),.        
-00023c50: 2020 2020 2830 2e34 3634 3130 322c 202d      (0.464102, -
-00023c60: 332e 3029 2c0a 2020 2020 2020 2020 2020  3.0),.          
-00023c70: 2020 2832 2e31 3936 3135 322c 202d 332e    (2.196152, -3.
-00023c80: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00023c90: 282d 332e 302c 2030 2e30 292c 0a20 2020  (-3.0, 0.0),.   
-00023ca0: 2020 2020 2020 2020 2028 2d31 2e32 3637           (-1.267
-00023cb0: 3934 392c 2030 2e30 292c 0a20 2020 2020  949, 0.0),.     
-00023cc0: 2020 2020 2020 2028 302e 3436 3431 3032         (0.464102
-00023cd0: 2c20 302e 3029 2c0a 2020 2020 2020 2020  , 0.0),.        
-00023ce0: 2020 2020 2832 2e31 3936 3135 322c 2030      (2.196152, 0
-00023cf0: 2e30 292c 0a20 2020 2020 2020 2020 2020  .0),.           
-00023d00: 2028 2d32 2e31 3333 3937 342c 202d 312e   (-2.133974, -1.
-00023d10: 3529 2c0a 2020 2020 2020 2020 2020 2020  5),.            
-00023d20: 282d 302e 3430 3139 3233 2c20 2d31 2e35  (-0.401923, -1.5
-00023d30: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00023d40: 312e 3333 3031 3237 2c20 2d31 2e35 292c  1.330127, -1.5),
-00023d50: 0a20 2020 2020 2020 2020 2020 2028 332e  .            (3.
-00023d60: 3036 3231 3738 2c20 2d31 2e35 292c 0a20  062178, -1.5),. 
-00023d70: 2020 2020 2020 2020 2020 2028 2d32 2e31             (-2.1
-00023d80: 3333 3937 352c 2031 2e35 292c 0a20 2020  33975, 1.5),.   
-00023d90: 2020 2020 2020 2020 2028 2d30 2e34 3031           (-0.401
-00023da0: 3932 342c 2031 2e35 292c 0a20 2020 2020  924, 1.5),.     
-00023db0: 2020 2020 2020 2028 312e 3333 3031 3237         (1.330127
-00023dc0: 2c20 312e 3529 2c0a 2020 2020 2020 2020  , 1.5),.        
-00023dd0: 2020 2020 2833 2e30 3632 3137 382c 2031      (3.062178, 1
-00023de0: 2e35 292c 0a20 2020 2020 2020 205d 0a20  .5),.        ]. 
-00023df0: 2020 2020 2020 2023 2053 7069 6b65 2073         # Spike s
-00023e00: 7572 6661 6365 0a20 2020 2020 2020 2074  urface.        t
-00023e10: 6869 636b 6e65 7373 203d 2030 2e31 0a20  hickness = 0.1. 
-00023e20: 2020 2020 2020 2066 6e20 3d20 360a 2020         fn = 6.  
-00023e30: 2020 2020 2020 6564 6765 5f70 6f69 6e74        edge_point
-00023e40: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00023e50: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00023e60: 2020 2020 7231 202a 206d 6174 682e 636f      r1 * math.co
-00023e70: 7328 6920 2a20 3220 2a20 6d61 7468 2e70  s(i * 2 * math.p
-00023e80: 6920 2f20 666e 202b 2033 3020 2a20 6d61  i / fn + 30 * ma
-00023e90: 7468 2e70 6920 2f20 3138 3029 2c0a 2020  th.pi / 180),.  
-00023ea0: 2020 2020 2020 2020 2020 2020 2020 7231                r1
-00023eb0: 202a 206d 6174 682e 7369 6e28 6920 2a20   * math.sin(i * 
-00023ec0: 3220 2a20 6d61 7468 2e70 6920 2f20 666e  2 * math.pi / fn
-00023ed0: 202b 2033 3020 2a20 6d61 7468 2e70 6920   + 30 * math.pi 
-00023ee0: 2f20 3138 3029 2c0a 2020 2020 2020 2020  / 180),.        
-00023ef0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00023f00: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00023f10: 2866 6e20 2b20 3129 0a20 2020 2020 2020  (fn + 1).       
-00023f20: 205d 0a20 2020 2020 2020 2073 7572 6661   ].        surfa
-00023f30: 6365 5f70 6f69 6e74 7320 3d20 5b0a 2020  ce_points = [.  
-00023f40: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-00023f50: 2020 2020 2020 2020 2020 2020 7231 202f              r1 /
-00023f60: 2034 202a 206d 6174 682e 636f 7328 6920   4 * math.cos(i 
-00023f70: 2a20 3220 2a20 6d61 7468 2e70 6920 2f20  * 2 * math.pi / 
-00023f80: 666e 202b 2033 3020 2a20 6d61 7468 2e70  fn + 30 * math.p
-00023f90: 6920 2f20 3138 3029 2c0a 2020 2020 2020  i / 180),.      
-00023fa0: 2020 2020 2020 2020 2020 7231 202f 2034            r1 / 4
-00023fb0: 202a 206d 6174 682e 7369 6e28 6920 2a20   * math.sin(i * 
-00023fc0: 3220 2a20 6d61 7468 2e70 6920 2f20 666e  2 * math.pi / fn
-00023fd0: 202b 2033 3020 2a20 6d61 7468 2e70 6920   + 30 * math.pi 
-00023fe0: 2f20 3138 3029 2c0a 2020 2020 2020 2020  / 180),.        
-00023ff0: 2020 2020 2020 2020 302e 3735 2c0a 2020          0.75,.  
-00024000: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00024010: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00024020: 2072 616e 6765 2866 6e20 2b20 3129 0a20   range(fn + 1). 
-00024030: 2020 2020 2020 205d 202b 205b 2830 2c20         ] + [(0, 
-00024040: 302c 2032 295d 0a20 2020 2020 2020 2065  0, 2)].        e
-00024050: 6467 655f 7769 7265 203d 2057 6f72 6b70  dge_wire = Workp
-00024060: 6c61 6e65 2822 5859 2229 2e70 6f6c 796c  lane("XY").polyl
-00024070: 696e 6528 6564 6765 5f70 6f69 6e74 7329  ine(edge_points)
-00024080: 0a20 2020 2020 2020 2070 6c61 7465 5f33  .        plate_3
-00024090: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000240a0: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
-000240b0: 0a20 2020 2020 2020 2020 2020 202e 7075  .            .pu
-000240c0: 7368 506f 696e 7473 2870 7473 290a 2020  shPoints(pts).  
-000240d0: 2020 2020 2020 2020 2020 2e69 6e74 6572            .inter
-000240e0: 7050 6c61 7465 280a 2020 2020 2020 2020  pPlate(.        
-000240f0: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
-00024100: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00024110: 2020 2073 7572 6661 6365 5f70 6f69 6e74     surface_point
-00024120: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00024130: 2020 2074 6869 636b 6e65 7373 2c0a 2020     thickness,.  
-00024140: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00024150: 6d62 696e 653d 4661 6c73 652c 0a20 2020  mbine=False,.   
-00024160: 2020 2020 2020 2020 2020 2020 2063 6c65               cle
-00024170: 616e 3d46 616c 7365 2c0a 2020 2020 2020  an=False,.      
-00024180: 2020 2020 2020 2020 2020 6465 6772 6565            degree
-00024190: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
-000241a0: 2020 2020 6e62 5074 734f 6e43 7572 3d32      nbPtsOnCur=2
-000241b0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-000241c0: 2020 206e 6249 7465 723d 322c 0a20 2020     nbIter=2,.   
-000241d0: 2020 2020 2020 2020 2020 2020 2061 6e69               ani
-000241e0: 736f 7472 6f70 793d 4661 6c73 652c 0a20  sotropy=False,. 
-000241f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00024200: 6f6c 3264 3d30 2e30 3030 3031 2c0a 2020  ol2d=0.00001,.  
-00024210: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00024220: 6c33 643d 302e 3030 3031 2c0a 2020 2020  l3d=0.0001,.    
-00024230: 2020 2020 2020 2020 2020 2020 746f 6c41              tolA
-00024240: 6e67 3d30 2e30 312c 0a20 2020 2020 2020  ng=0.01,.       
-00024250: 2020 2020 2020 2020 2074 6f6c 4375 7276           tolCurv
-00024260: 3d30 2e31 2c0a 2020 2020 2020 2020 2020  =0.1,.          
-00024270: 2020 2020 2020 6d61 7844 6567 3d38 2c0a        maxDeg=8,.
-00024280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024290: 6d61 7853 6567 6d65 6e74 733d 392c 0a20  maxSegments=9,. 
-000242a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000242b0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-000242c0: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
-000242d0: 6c61 7465 5f33 2e76 616c 2829 2e69 7356  late_3.val().isV
-000242e0: 616c 6964 2829 290a 2020 2020 2020 2020  alid()).        
-000242f0: 7365 6c66 2e61 7373 6572 7441 6c6d 6f73  self.assertAlmos
-00024300: 7445 7175 616c 2870 6c61 7465 5f33 2e76  tEqual(plate_3.v
-00024310: 616c 2829 2e56 6f6c 756d 6528 292c 2030  al().Volume(), 0
-00024320: 2e34 3538 3933 3935 3436 3835 3138 3934  .458939546851894
-00024330: 3134 2c20 3129 0a0a 2020 2020 2020 2020  14, 1)..        
-00024340: 2320 4779 726f c3af 642c 2061 6c6c 2065  # Gyro..d, all e
-00024350: 6467 6573 2061 7265 2073 706c 696e 6573  dges are splines
-00024360: 206f 6e20 6469 6666 6572 656e 7420 776f   on different wo
-00024370: 726b 706c 616e 6573 2e0a 2020 2020 2020  rkplanes..      
-00024380: 2020 7468 6963 6b6e 6573 7320 3d20 302e    thickness = 0.
-00024390: 310a 2020 2020 2020 2020 6564 6765 5f70  1.        edge_p
-000243a0: 6f69 6e74 7320 3d20 5b0a 2020 2020 2020  oints = [.      
-000243b0: 2020 2020 2020 5b5b 332e 3534 2c20 332e        [[3.54, 3.
-000243c0: 3534 5d2c 205b 312e 3737 2c20 302e 305d  54], [1.77, 0.0]
-000243d0: 2c20 5b33 2e35 342c 202d 332e 3534 5d5d  , [3.54, -3.54]]
-000243e0: 2c0a 2020 2020 2020 2020 2020 2020 5b5b  ,.            [[
-000243f0: 2d33 2e35 342c 202d 332e 3534 5d2c 205b  -3.54, -3.54], [
-00024400: 302e 302c 202d 312e 3737 5d2c 205b 332e  0.0, -1.77], [3.
-00024410: 3534 2c20 2d33 2e35 345d 5d2c 0a20 2020  54, -3.54]],.   
-00024420: 2020 2020 2020 2020 205b 5b2d 332e 3534           [[-3.54
-00024430: 2c20 2d33 2e35 345d 2c20 5b30 2e30 2c20  , -3.54], [0.0, 
-00024440: 2d31 2e37 375d 2c20 5b33 2e35 342c 202d  -1.77], [3.54, -
-00024450: 332e 3534 5d5d 2c0a 2020 2020 2020 2020  3.54]],.        
-00024460: 2020 2020 5b5b 2d33 2e35 342c 202d 332e      [[-3.54, -3.
-00024470: 3534 5d2c 205b 2d31 2e37 372c 2030 2e30  54], [-1.77, 0.0
-00024480: 5d2c 205b 2d33 2e35 342c 2033 2e35 345d  ], [-3.54, 3.54]
-00024490: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000244a0: 5b33 2e35 342c 2033 2e35 345d 2c20 5b30  [3.54, 3.54], [0
-000244b0: 2e30 2c20 312e 3737 5d2c 205b 2d33 2e35  .0, 1.77], [-3.5
-000244c0: 342c 2033 2e35 345d 5d2c 0a20 2020 2020  4, 3.54]],.     
-000244d0: 2020 2020 2020 205b 5b33 2e35 342c 2033         [[3.54, 3
-000244e0: 2e35 345d 2c20 5b30 2e30 2c20 312e 3737  .54], [0.0, 1.77
-000244f0: 5d2c 205b 2d33 2e35 342c 2033 2e35 345d  ], [-3.54, 3.54]
-00024500: 5d2c 0a20 2020 2020 2020 205d 0a20 2020  ],.        ].   
-00024510: 2020 2020 2070 6c61 6e65 5f6c 6973 7420       plane_list 
-00024520: 3d20 5b22 585a 222c 2022 5859 222c 2022  = ["XZ", "XY", "
-00024530: 595a 222c 2022 585a 222c 2022 595a 222c  YZ", "XZ", "YZ",
-00024540: 2022 5859 225d 0a20 2020 2020 2020 206f   "XY"].        o
-00024550: 6666 7365 745f 6c69 7374 203d 205b 2d33  ffset_list = [-3
-00024560: 2e35 342c 2033 2e35 342c 2033 2e35 342c  .54, 3.54, 3.54,
-00024570: 2033 2e35 342c 202d 332e 3534 2c20 2d33   3.54, -3.54, -3
-00024580: 2e35 345d 0a20 2020 2020 2020 2065 6467  .54].        edg
-00024590: 655f 7769 7265 203d 2028 0a20 2020 2020  e_wire = (.     
-000245a0: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
-000245b0: 2870 6c61 6e65 5f6c 6973 745b 305d 290a  (plane_list[0]).
-000245c0: 2020 2020 2020 2020 2020 2020 2e77 6f72              .wor
-000245d0: 6b70 6c61 6e65 286f 6666 7365 743d 2d6f  kplane(offset=-o
-000245e0: 6666 7365 745f 6c69 7374 5b30 5d29 0a20  ffset_list[0]). 
-000245f0: 2020 2020 2020 2020 2020 202e 7370 6c69             .spli
-00024600: 6e65 2865 6467 655f 706f 696e 7473 5b30  ne(edge_points[0
-00024610: 5d29 0a20 2020 2020 2020 2029 0a20 2020  ]).        ).   
-00024620: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00024630: 6e67 6528 6c65 6e28 6564 6765 5f70 6f69  nge(len(edge_poi
-00024640: 6e74 7329 202d 2031 293a 0a20 2020 2020  nts) - 1):.     
-00024650: 2020 2020 2020 2065 6467 655f 7769 7265         edge_wire
-00024660: 203d 2065 6467 655f 7769 7265 2e61 6464   = edge_wire.add
-00024670: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00024680: 2020 576f 726b 706c 616e 6528 706c 616e    Workplane(plan
-00024690: 655f 6c69 7374 5b69 202b 2031 5d29 0a20  e_list[i + 1]). 
-000246a0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-000246b0: 776f 726b 706c 616e 6528 6f66 6673 6574  workplane(offset
-000246c0: 3d2d 6f66 6673 6574 5f6c 6973 745b 6920  =-offset_list[i 
-000246d0: 2b20 315d 290a 2020 2020 2020 2020 2020  + 1]).          
-000246e0: 2020 2020 2020 2e73 706c 696e 6528 6564        .spline(ed
-000246f0: 6765 5f70 6f69 6e74 735b 6920 2b20 315d  ge_points[i + 1]
-00024700: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00024710: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
-00024720: 706f 696e 7473 203d 205b 2830 2c20 302c  points = [(0, 0,
-00024730: 2030 295d 0a20 2020 2020 2020 2070 6c61   0)].        pla
-00024740: 7465 5f34 203d 2057 6f72 6b70 6c61 6e65  te_4 = Workplane
-00024750: 2822 5859 2229 2e69 6e74 6572 7050 6c61  ("XY").interpPla
-00024760: 7465 2865 6467 655f 7769 7265 2c20 7375  te(edge_wire, su
-00024770: 7266 6163 655f 706f 696e 7473 2c20 7468  rface_points, th
-00024780: 6963 6b6e 6573 7329 0a20 2020 2020 2020  ickness).       
-00024790: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-000247a0: 2870 6c61 7465 5f34 2e76 616c 2829 2e69  (plate_4.val().i
-000247b0: 7356 616c 6964 2829 290a 2020 2020 2020  sValid()).      
-000247c0: 2020 7365 6c66 2e61 7373 6572 7441 6c6d    self.assertAlm
-000247d0: 6f73 7445 7175 616c 2870 6c61 7465 5f34  ostEqual(plate_4
-000247e0: 2e76 616c 2829 2e56 6f6c 756d 6528 292c  .val().Volume(),
-000247f0: 2037 2e37 3630 3535 3934 3930 2c20 3229   7.760559490, 2)
-00024800: 0a0a 2020 2020 2020 2020 706c 6174 655f  ..        plate_
-00024810: 3520 3d20 576f 726b 706c 616e 6528 292e  5 = Workplane().
-00024820: 696e 7465 7270 506c 6174 6528 576f 726b  interpPlate(Work
-00024830: 706c 616e 6528 292e 736c 6f74 3244 2832  plane().slot2D(2
-00024840: 2c20 3129 2e76 616c 7328 2929 0a0a 2020  , 1).vals())..  
-00024850: 2020 2020 2020 6173 7365 7274 2070 6c61        assert pla
-00024860: 7465 5f35 2e76 616c 2829 2e69 7356 616c  te_5.val().isVal
-00024870: 6964 2829 0a0a 2020 2020 2020 2020 706c  id()..        pl
-00024880: 6174 655f 3620 3d20 536f 6c69 642e 696e  ate_6 = Solid.in
-00024890: 7465 7270 506c 6174 6528 0a20 2020 2020  terpPlate(.     
-000248a0: 2020 2020 2020 205b 2830 2c20 302c 2030         [(0, 0, 0
-000248b0: 292c 2028 312c 2030 2c20 3029 2c20 2831  ), (1, 0, 0), (1
-000248c0: 2c20 312c 2030 292c 2028 302c 2031 2c20  , 1, 0), (0, 1, 
-000248d0: 3029 5d2c 205b 5d2c 2074 6869 636b 6e65  0)], [], thickne
-000248e0: 7373 3d31 0a20 2020 2020 2020 2029 0a0a  ss=1.        )..
-000248f0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-00024900: 6c61 7465 5f36 2e69 7356 616c 6964 2829  late_6.isValid()
-00024910: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00024920: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
-00024930: 706c 6174 655f 362e 566f 6c75 6d65 2829  plate_6.Volume()
-00024940: 2c20 312c 2032 290a 0a20 2020 2064 6566  , 1, 2)..    def
-00024950: 2074 6573 7454 616e 6765 6e74 4172 6354   testTangentArcT
-00024960: 6f50 6f69 6e74 2873 656c 6629 3a0a 0a20  oPoint(self):.. 
-00024970: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
-00024980: 6120 7369 6d70 6c65 2073 6861 7065 2077  a simple shape w
-00024990: 6974 6820 7461 6e67 656e 7473 206f 6620  ith tangents of 
-000249a0: 7374 7261 6967 6874 2065 6467 6573 2061  straight edges a
-000249b0: 6e64 2073 6565 2069 6620 6974 2068 6173  nd see if it has
-000249c0: 2074 6865 2063 6f72 7265 6374 2061 7265   the correct are
-000249d0: 610a 2020 2020 2020 2020 7330 203d 2028  a.        s0 = (
-000249e0: 0a20 2020 2020 2020 2020 2020 2057 6f72  .            Wor
-000249f0: 6b70 6c61 6e65 2822 5859 2229 0a20 2020  kplane("XY").   
-00024a00: 2020 2020 2020 2020 202e 684c 696e 6528           .hLine(
-00024a10: 3129 0a20 2020 2020 2020 2020 2020 202e  1).            .
-00024a20: 7461 6e67 656e 7441 7263 506f 696e 7428  tangentArcPoint(
-00024a30: 2831 2c20 3129 2c20 7265 6c61 7469 7665  (1, 1), relative
-00024a40: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00024a50: 2020 2020 2e68 4c69 6e65 546f 2830 290a      .hLineTo(0).
-00024a60: 2020 2020 2020 2020 2020 2020 2e74 616e              .tan
-00024a70: 6765 6e74 4172 6350 6f69 6e74 2828 302c  gentArcPoint((0,
-00024a80: 2030 292c 2072 656c 6174 6976 653d 4661   0), relative=Fa
-00024a90: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00024aa0: 202e 636c 6f73 6528 290a 2020 2020 2020   .close().      
-00024ab0: 2020 2020 2020 2e65 7874 7275 6465 2831        .extrude(1
-00024ac0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00024ad0: 2020 2020 6172 6561 3020 3d20 7330 2e66      area0 = s0.f
-00024ae0: 6163 6573 2822 3e5a 2229 2e76 616c 2829  aces(">Z").val()
-00024af0: 2e41 7265 6128 290a 2020 2020 2020 2020  .Area().        
-00024b00: 7365 6c66 2e61 7373 6572 7441 6c6d 6f73  self.assertAlmos
-00024b10: 7445 7175 616c 2861 7265 6130 2c20 2831  tEqual(area0, (1
-00024b20: 202b 206d 6174 682e 7069 202a 2030 2e35   + math.pi * 0.5
-00024b30: 202a 2a20 3229 2c20 3429 0a0a 2020 2020   ** 2), 4)..    
-00024b40: 2020 2020 2320 7465 7374 2072 656c 6174      # test relat
-00024b50: 6976 6520 636f 6f72 6473 0a20 2020 2020  ive coords.     
-00024b60: 2020 2073 3120 3d20 280a 2020 2020 2020     s1 = (.      
-00024b70: 2020 2020 2020 576f 726b 706c 616e 6528        Workplane(
-00024b80: 2258 5922 290a 2020 2020 2020 2020 2020  "XY").          
-00024b90: 2020 2e68 4c69 6e65 2831 290a 2020 2020    .hLine(1).    
-00024ba0: 2020 2020 2020 2020 2e74 616e 6765 6e74          .tangent
-00024bb0: 4172 6350 6f69 6e74 2828 302c 2031 292c  ArcPoint((0, 1),
-00024bc0: 2072 656c 6174 6976 653d 5472 7565 290a   relative=True).
-00024bd0: 2020 2020 2020 2020 2020 2020 2e68 4c69              .hLi
-00024be0: 6e65 546f 2830 290a 2020 2020 2020 2020  neTo(0).        
-00024bf0: 2020 2020 2e74 616e 6765 6e74 4172 6350      .tangentArcP
-00024c00: 6f69 6e74 2828 302c 202d 3129 2c20 7265  oint((0, -1), re
-00024c10: 6c61 7469 7665 3d54 7275 6529 0a20 2020  lative=True).   
-00024c20: 2020 2020 2020 2020 202e 636c 6f73 6528           .close(
-00024c30: 290a 2020 2020 2020 2020 2020 2020 2e65  ).            .e
-00024c40: 7874 7275 6465 2831 290a 2020 2020 2020  xtrude(1).      
-00024c50: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00024c60: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
-00024c70: 7374 4571 7561 6c73 280a 2020 2020 2020  stEquals(.      
-00024c80: 2020 2020 2020 7331 2e76 616c 2829 2e43        s1.val().C
-00024c90: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
-00024ca0: 292c 2073 302e 7661 6c28 292e 4365 6e74  ), s0.val().Cent
-00024cb0: 6572 2829 2e74 6f54 7570 6c65 2829 2c20  er().toTuple(), 
-00024cc0: 340a 2020 2020 2020 2020 290a 2020 2020  4.        ).    
-00024cd0: 2020 2020 7365 6c66 2e61 7373 6572 7441      self.assertA
-00024ce0: 6c6d 6f73 7445 7175 616c 2873 312e 7661  lmostEqual(s1.va
-00024cf0: 6c28 292e 566f 6c75 6d65 2829 2c20 7330  l().Volume(), s0
-00024d00: 2e76 616c 2829 2e56 6f6c 756d 6528 292c  .val().Volume(),
-00024d10: 2034 290a 0a20 2020 2020 2020 2023 2063   4)..        # c
-00024d20: 6f6e 7365 6375 7469 7665 2074 616e 6765  onsecutive tange
-00024d30: 6e74 2061 7263 730a 2020 2020 2020 2020  nt arcs.        
-00024d40: 7331 203d 2028 0a20 2020 2020 2020 2020  s1 = (.         
-00024d50: 2020 2057 6f72 6b70 6c61 6e65 2822 5859     Workplane("XY
-00024d60: 2229 0a20 2020 2020 2020 2020 2020 202e  ").            .
-00024d70: 764c 696e 6528 3229 0a20 2020 2020 2020  vLine(2).       
-00024d80: 2020 2020 202e 7461 6e67 656e 7441 7263       .tangentArc
-00024d90: 506f 696e 7428 2831 2c20 3029 290a 2020  Point((1, 0)).  
-00024da0: 2020 2020 2020 2020 2020 2e74 616e 6765            .tange
-00024db0: 6e74 4172 6350 6f69 6e74 2828 312c 2030  ntArcPoint((1, 0
-00024dc0: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
-00024dd0: 7461 6e67 656e 7441 7263 506f 696e 7428  tangentArcPoint(
-00024de0: 2831 2c20 3029 290a 2020 2020 2020 2020  (1, 0)).        
-00024df0: 2020 2020 2e76 4c69 6e65 282d 3229 0a20      .vLine(-2). 
-00024e00: 2020 2020 2020 2020 2020 202e 636c 6f73             .clos
-00024e10: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00024e20: 2e65 7874 7275 6465 2831 290a 2020 2020  .extrude(1).    
-00024e30: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00024e40: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
-00024e50: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00024e60: 2020 7331 2e66 6163 6573 2822 3e5a 2229    s1.faces(">Z")
-00024e70: 2e76 616c 2829 2e41 7265 6128 292c 2032  .val().Area(), 2
-00024e80: 202a 2033 202b 2030 2e35 202a 206d 6174   * 3 + 0.5 * mat
-00024e90: 682e 7069 202a 2030 2e35 202a 2a20 322c  h.pi * 0.5 ** 2,
-00024ea0: 2034 0a20 2020 2020 2020 2029 0a0a 2020   4.        )..  
-00024eb0: 2020 2020 2020 2320 7461 6e67 656e 7441        # tangentA
-00024ec0: 7263 206f 6e20 7468 6520 656e 6420 6f66  rc on the end of
-00024ed0: 2061 2073 706c 696e 650a 2020 2020 2020   a spline.      
-00024ee0: 2020 2320 7370 6c69 6e65 2077 696c 6c20    # spline will 
-00024ef0: 6265 2061 2073 696d 706c 6520 6172 6320  be a simple arc 
-00024f00: 6f66 2061 2063 6972 636c 652c 2074 6865  of a circle, the
-00024f10: 6e20 6669 6e69 7368 6564 206f 6666 2077  n finished off w
-00024f20: 6974 6820 610a 2020 2020 2020 2020 2320  ith a.        # 
-00024f30: 7461 6e67 656e 7441 7263 506f 696e 740a  tangentArcPoint.
-00024f40: 2020 2020 2020 2020 616e 676c 6573 203d          angles =
-00024f50: 205b 6964 7820 2a20 312e 3520 2a20 6d61   [idx * 1.5 * ma
-00024f60: 7468 2e70 6920 2f20 3130 2066 6f72 2069  th.pi / 10 for i
-00024f70: 6478 2069 6e20 7261 6e67 6528 3130 295d  dx in range(10)]
-00024f80: 0a20 2020 2020 2020 2070 7473 203d 205b  .        pts = [
-00024f90: 286d 6174 682e 7369 6e28 6129 2c20 6d61  (math.sin(a), ma
-00024fa0: 7468 2e63 6f73 2861 2929 2066 6f72 2061  th.cos(a)) for a
-00024fb0: 2069 6e20 616e 676c 6573 5d0a 2020 2020   in angles].    
-00024fc0: 2020 2020 7332 203d 2028 0a20 2020 2020      s2 = (.     
-00024fd0: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
-00024fe0: 2822 5859 2229 0a20 2020 2020 2020 2020  ("XY").         
-00024ff0: 2020 202e 7370 6c69 6e65 2870 7473 290a     .spline(pts).
-00025000: 2020 2020 2020 2020 2020 2020 2e74 616e              .tan
-00025010: 6765 6e74 4172 6350 6f69 6e74 2828 302c  gentArcPoint((0,
-00025020: 2031 292c 2072 656c 6174 6976 653d 4661   1), relative=Fa
-00025030: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00025040: 202e 636c 6f73 6528 290a 2020 2020 2020   .close().      
-00025050: 2020 2020 2020 2e65 7874 7275 6465 2831        .extrude(1
-00025060: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00025070: 2020 2020 2320 766f 6c75 6d65 2073 686f      # volume sho
-00025080: 756c 6420 616c 6d6f 7374 2062 6520 7069  uld almost be pi
-00025090: 2c20 6275 7420 6e6f 7420 6163 6375 7261  , but not accura
-000250a0: 7465 6c79 2062 6563 6175 7365 2077 6520  tely because we 
-000250b0: 6e65 6564 2074 6f0a 2020 2020 2020 2020  need to.        
-000250c0: 2320 7374 6172 7420 7769 7468 2061 2073  # start with a s
-000250d0: 706c 696e 650a 2020 2020 2020 2020 7365  pline.        se
-000250e0: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
-000250f0: 7175 616c 2873 322e 7661 6c28 292e 566f  qual(s2.val().Vo
-00025100: 6c75 6d65 2829 2c20 6d61 7468 2e70 692c  lume(), math.pi,
-00025110: 2031 290a 2020 2020 2020 2020 2320 6173   1).        # as
-00025120: 7365 7274 206c 6f63 616c 2063 6f6f 7264  sert local coord
-00025130: 7320 6172 6520 6d61 7070 6564 2074 6f20  s are mapped to 
-00025140: 676c 6f62 616c 2063 6f72 7265 6374 6c79  global correctly
-00025150: 0a20 2020 2020 2020 2061 7263 3020 3d20  .        arc0 = 
-00025160: 576f 726b 706c 616e 6528 2258 5a22 2c20  Workplane("XZ", 
-00025170: 6f72 6967 696e 3d28 312c 2031 2c20 3129  origin=(1, 1, 1)
-00025180: 292e 684c 696e 6528 3129 2e74 616e 6765  ).hLine(1).tange
-00025190: 6e74 4172 6350 6f69 6e74 2828 312c 2031  ntArcPoint((1, 1
-000251a0: 2929 2e76 616c 2829 0a20 2020 2020 2020  )).val().       
-000251b0: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
-000251c0: 6541 6c6d 6f73 7445 7175 616c 7328 6172  eAlmostEquals(ar
-000251d0: 6330 2e65 6e64 506f 696e 7428 292e 746f  c0.endPoint().to
-000251e0: 5475 706c 6528 292c 2028 332c 2031 2c20  Tuple(), (3, 1, 
-000251f0: 3229 2c20 3429 0a0a 2020 2020 2020 2020  2), 4)..        
-00025200: 2320 7461 6e67 656e 7441 7263 506f 696e  # tangentArcPoin
-00025210: 7420 7769 7468 2033 2d74 7570 6c65 2061  t with 3-tuple a
-00025220: 7267 756d 656e 740a 2020 2020 2020 2020  rgument.        
-00025230: 7730 203d 2057 6f72 6b70 6c61 6e65 2822  w0 = Workplane("
-00025240: 5859 2229 2e6c 696e 6554 6f28 312c 2031  XY").lineTo(1, 1
-00025250: 292e 7461 6e67 656e 7441 7263 506f 696e  ).tangentArcPoin
-00025260: 7428 2831 2c20 312c 2031 2929 2e77 6972  t((1, 1, 1)).wir
-00025270: 6528 290a 2020 2020 2020 2020 7a6d 6178  e().        zmax
-00025280: 203d 2077 302e 7661 6c28 292e 426f 756e   = w0.val().Boun
-00025290: 6469 6e67 426f 7828 292e 7a6d 6178 0a20  dingBox().zmax. 
-000252a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000252b0: 7274 416c 6d6f 7374 4571 7561 6c28 7a6d  rtAlmostEqual(zm
-000252c0: 6178 2c20 312c 2031 290a 0a20 2020 2064  ax, 1, 1)..    d
-000252d0: 6566 2074 6573 745f 6669 6e64 4672 6f6d  ef test_findFrom
-000252e0: 4564 6765 2873 656c 6629 3a0a 2020 2020  Edge(self):.    
-000252f0: 2020 2020 7061 7274 203d 2057 6f72 6b70      part = Workp
-00025300: 6c61 6e65 2822 5859 222c 206f 7269 6769  lane("XY", origi
-00025310: 6e3d 2831 2c20 312c 2031 2929 2e68 4c69  n=(1, 1, 1)).hLi
-00025320: 6e65 2831 290a 2020 2020 2020 2020 666f  ne(1).        fo
-00025330: 756e 645f 6564 6765 203d 2070 6172 742e  und_edge = part.
-00025340: 5f66 696e 6446 726f 6d45 6467 6528 7573  _findFromEdge(us
-00025350: 654c 6f63 616c 436f 6f72 6473 3d46 616c  eLocalCoords=Fal
-00025360: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
-00025370: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
-00025380: 7374 4571 7561 6c73 2866 6f75 6e64 5f65  stEquals(found_e
-00025390: 6467 652e 7374 6172 7450 6f69 6e74 2829  dge.startPoint()
-000253a0: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
-000253b0: 312c 2031 292c 2033 290a 2020 2020 2020  1, 1), 3).      
-000253c0: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
-000253d0: 6c65 416c 6d6f 7374 4571 7561 6c73 2866  leAlmostEquals(f
-000253e0: 6f75 6e64 5f65 6467 652e 4365 6e74 6572  ound_edge.Center
-000253f0: 2829 2e74 6f54 7570 6c65 2829 2c20 2831  ().toTuple(), (1
-00025400: 2e35 2c20 312c 2031 292c 2033 290a 2020  .5, 1, 1), 3).  
-00025410: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00025420: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
-00025430: 6c73 2866 6f75 6e64 5f65 6467 652e 656e  ls(found_edge.en
-00025440: 6450 6f69 6e74 2829 2e74 6f54 7570 6c65  dPoint().toTuple
-00025450: 2829 2c20 2832 2c20 312c 2031 292c 2033  (), (2, 1, 1), 3
-00025460: 290a 2020 2020 2020 2020 666f 756e 645f  ).        found_
-00025470: 6564 6765 203d 2070 6172 742e 5f66 696e  edge = part._fin
-00025480: 6446 726f 6d45 6467 6528 7573 654c 6f63  dFromEdge(useLoc
-00025490: 616c 436f 6f72 6473 3d54 7275 6529 0a20  alCoords=True). 
-000254a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000254b0: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
-000254c0: 616c 7328 666f 756e 645f 6564 6765 2e65  als(found_edge.e
-000254d0: 6e64 506f 696e 7428 292e 746f 5475 706c  ndPoint().toTupl
-000254e0: 6528 292c 2028 312c 2030 2c20 3029 2c20  e(), (1, 0, 0), 
-000254f0: 3329 0a20 2020 2020 2020 2023 2063 6865  3).        # che
-00025500: 636b 205f 6669 6e64 4672 6f6d 4564 6765  ck _findFromEdge
-00025510: 2063 616e 2066 696e 6420 6120 7370 6c69   can find a spli
-00025520: 6e65 0a20 2020 2020 2020 2070 7473 203d  ne.        pts =
-00025530: 205b 2830 2c20 3029 2c20 2830 2c20 3129   [(0, 0), (0, 1)
-00025540: 2c20 2831 2c20 3229 2c20 2832 2c20 3429  , (1, 2), (2, 4)
-00025550: 5d0a 2020 2020 2020 2020 7370 6c69 6e65  ].        spline
-00025560: 3020 3d20 576f 726b 706c 616e 6528 2258  0 = Workplane("X
-00025570: 5a22 292e 7370 6c69 6e65 2870 7473 292e  Z").spline(pts).
-00025580: 5f66 696e 6446 726f 6d45 6467 6528 290a  _findFromEdge().
-00025590: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000255a0: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
-000255b0: 7561 6c73 2828 322c 2030 2c20 3429 2c20  uals((2, 0, 4), 
-000255c0: 7370 6c69 6e65 302e 656e 6450 6f69 6e74  spline0.endPoint
-000255d0: 2829 2e74 6f54 7570 6c65 2829 2c20 3329  ().toTuple(), 3)
-000255e0: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
-000255f0: 206d 6574 686f 6420 6661 696c 7320 6966   method fails if
-00025600: 206e 6f20 6564 6765 2069 7320 7072 6573   no edge is pres
-00025610: 656e 740a 2020 2020 2020 2020 7061 7274  ent.        part
-00025620: 3220 3d20 576f 726b 706c 616e 6528 2258  2 = Workplane("X
-00025630: 5922 292e 626f 7828 312c 2031 2c20 3129  Y").box(1, 1, 1)
-00025640: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00025650: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00025660: 5275 6e74 696d 6545 7272 6f72 293a 0a20  RuntimeError):. 
-00025670: 2020 2020 2020 2020 2020 2070 6172 7432             part2
-00025680: 2e5f 6669 6e64 4672 6f6d 4564 6765 2829  ._findFromEdge()
-00025690: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000256a0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-000256b0: 5275 6e74 696d 6545 7272 6f72 293a 0a20  RuntimeError):. 
-000256c0: 2020 2020 2020 2020 2020 2070 6172 7432             part2
-000256d0: 2e5f 6669 6e64 4672 6f6d 4564 6765 2875  ._findFromEdge(u
-000256e0: 7365 4c6f 6361 6c43 6f6f 7264 733d 5472  seLocalCoords=Tr
-000256f0: 7565 290a 0a20 2020 2064 6566 2074 6573  ue)..    def tes
-00025700: 744d 616b 6548 656c 6978 2873 656c 6629  tMakeHelix(self)
-00025710: 3a0a 0a20 2020 2020 2020 2068 203d 2031  :..        h = 1
-00025720: 300a 2020 2020 2020 2020 7069 7463 6820  0.        pitch 
-00025730: 3d20 312e 350a 2020 2020 2020 2020 7220  = 1.5.        r 
-00025740: 3d20 312e 320a 2020 2020 2020 2020 6f62  = 1.2.        ob
-00025750: 6a20 3d20 5769 7265 2e6d 616b 6548 656c  j = Wire.makeHel
-00025760: 6978 2870 6974 6368 2c20 682c 2072 290a  ix(pitch, h, r).
-00025770: 0a20 2020 2020 2020 2062 6220 3d20 6f62  .        bb = ob
-00025780: 6a2e 426f 756e 6469 6e67 426f 7828 290a  j.BoundingBox().
-00025790: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000257a0: 6572 7441 6c6d 6f73 7445 7175 616c 2862  ertAlmostEqual(b
-000257b0: 622e 7a6c 656e 2c20 682c 2031 290a 0a20  b.zlen, h, 1).. 
-000257c0: 2020 2064 6566 2074 6573 7455 6e69 6f6e     def testUnion
-000257d0: 436f 6d70 6f75 6e64 2873 656c 6629 3a0a  Compound(self):.
-000257e0: 0a20 2020 2020 2020 2062 6f78 3120 3d20  .        box1 = 
-000257f0: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
-00025800: 626f 7828 3130 2c20 3230 2c20 3330 290a  box(10, 20, 30).
-00025810: 2020 2020 2020 2020 626f 7832 203d 2057          box2 = W
-00025820: 6f72 6b70 6c61 6e65 2822 595a 2229 2e62  orkplane("YZ").b
-00025830: 6f78 2831 302c 2032 302c 2033 3029 0a20  ox(10, 20, 30). 
-00025840: 2020 2020 2020 2073 6861 7065 5f74 6f5f         shape_to_
-00025850: 6375 7420 3d20 576f 726b 706c 616e 6528  cut = Workplane(
-00025860: 2258 5922 292e 626f 7828 3135 2c20 3135  "XY").box(15, 15
-00025870: 2c20 3135 292e 7472 616e 736c 6174 6528  , 15).translate(
-00025880: 2838 2c20 382c 2038 2929 0a0a 2020 2020  (8, 8, 8))..    
-00025890: 2020 2020 6c69 7374 5f6f 665f 7368 6170      list_of_shap
-000258a0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
-000258b0: 666f 7220 6f20 696e 2062 6f78 312e 616c  for o in box1.al
-000258c0: 6c28 293a 0a20 2020 2020 2020 2020 2020  l():.           
-000258d0: 206c 6973 745f 6f66 5f73 6861 7065 732e   list_of_shapes.
-000258e0: 6578 7465 6e64 286f 2e76 616c 7328 2929  extend(o.vals())
-000258f0: 0a20 2020 2020 2020 2066 6f72 206f 2069  .        for o i
-00025900: 6e20 626f 7832 2e61 6c6c 2829 3a0a 2020  n box2.all():.  
-00025910: 2020 2020 2020 2020 2020 6c69 7374 5f6f            list_o
-00025920: 665f 7368 6170 6573 2e65 7874 656e 6428  f_shapes.extend(
-00025930: 6f2e 7661 6c73 2829 290a 0a20 2020 2020  o.vals())..     
-00025940: 2020 206f 626a 203d 2057 6f72 6b70 6c61     obj = Workpla
-00025950: 6e65 2822 5859 2229 2e6e 6577 4f62 6a65  ne("XY").newObje
-00025960: 6374 286c 6973 745f 6f66 5f73 6861 7065  ct(list_of_shape
-00025970: 7329 2e63 7574 2873 6861 7065 5f74 6f5f  s).cut(shape_to_
-00025980: 6375 7429 0a0a 2020 2020 2020 2020 6173  cut)..        as
-00025990: 7365 7274 206f 626a 2e76 616c 2829 2e69  sert obj.val().i
-000259a0: 7356 616c 6964 2829 0a0a 2020 2020 6465  sValid()..    de
-000259b0: 6620 7465 7374 5365 6374 696f 6e28 7365  f testSection(se
-000259c0: 6c66 293a 0a0a 2020 2020 2020 2020 626f  lf):..        bo
-000259d0: 7820 3d20 576f 726b 706c 616e 6528 2258  x = Workplane("X
-000259e0: 5922 2c20 6f72 6967 696e 3d28 312c 2032  Y", origin=(1, 2
-000259f0: 2c20 3329 292e 626f 7828 312c 2031 2c20  , 3)).box(1, 1, 
-00025a00: 3129 0a0a 2020 2020 2020 2020 7331 203d  1)..        s1 =
-00025a10: 2062 6f78 2e73 6563 7469 6f6e 2829 0a20   box.section(). 
-00025a20: 2020 2020 2020 2073 3220 3d20 626f 782e         s2 = box.
-00025a30: 7365 6374 696f 6e28 302e 3529 0a0a 2020  section(0.5)..  
-00025a40: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00025a50: 7441 6c6d 6f73 7445 7175 616c 2873 312e  tAlmostEqual(s1.
-00025a60: 6661 6365 7328 292e 7661 6c28 292e 4172  faces().val().Ar
-00025a70: 6561 2829 2c20 3129 0a20 2020 2020 2020  ea(), 1).       
-00025a80: 2073 656c 662e 6173 7365 7274 416c 6d6f   self.assertAlmo
-00025a90: 7374 4571 7561 6c28 7332 2e66 6163 6573  stEqual(s2.faces
-00025aa0: 2829 2e76 616c 2829 2e41 7265 6128 292c  ().val().Area(),
-00025ab0: 2031 290a 0a20 2020 2020 2020 206c 696e   1)..        lin
-00025ac0: 6520 3d20 576f 726b 706c 616e 6528 2258  e = Workplane("X
-00025ad0: 5922 292e 684c 696e 6528 3129 0a0a 2020  Y").hLine(1)..  
-00025ae0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00025af0: 6173 7365 7274 5261 6973 6573 2856 616c  assertRaises(Val
-00025b00: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
-00025b10: 2020 2020 2020 6c69 6e65 2e73 6563 7469        line.secti
-00025b20: 6f6e 2829 0a0a 2020 2020 6465 6620 7465  on()..    def te
-00025b30: 7374 476c 7565 2873 656c 6629 3a0a 0a20  stGlue(self):.. 
-00025b40: 2020 2020 2020 2062 6f78 3120 3d20 576f         box1 = Wo
-00025b50: 726b 706c 616e 6528 2258 5922 292e 7265  rkplane("XY").re
-00025b60: 6374 2831 2c20 3129 2e65 7874 7275 6465  ct(1, 1).extrude
-00025b70: 2832 290a 2020 2020 2020 2020 626f 7832  (2).        box2
-00025b80: 203d 2057 6f72 6b70 6c61 6e65 2822 5859   = Workplane("XY
-00025b90: 222c 206f 7269 6769 6e3d 2830 2c20 312c  ", origin=(0, 1,
-00025ba0: 2030 2929 2e72 6563 7428 312c 2031 292e   0)).rect(1, 1).
-00025bb0: 6578 7472 7564 6528 3129 0a20 2020 2020  extrude(1).     
-00025bc0: 2020 2072 6573 203d 2062 6f78 312e 756e     res = box1.un
-00025bd0: 696f 6e28 626f 7832 2c20 676c 7565 3d54  ion(box2, glue=T
-00025be0: 7275 6529 0a0a 2020 2020 2020 2020 7365  rue)..        se
-00025bf0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00025c00: 6573 2e66 6163 6573 2829 2e73 697a 6528  es.faces().size(
-00025c10: 292c 2038 290a 0a20 2020 2020 2020 206f  ), 8)..        o
-00025c20: 626a 203d 206f 626a 203d 2028 0a20 2020  bj = obj = (.   
-00025c30: 2020 2020 2020 2020 2057 6f72 6b70 6c61           Workpla
-00025c40: 6e65 2822 5859 2229 2e72 6563 7428 312c  ne("XY").rect(1,
-00025c50: 2031 292e 6578 7472 7564 6528 3229 2e6d   1).extrude(2).m
-00025c60: 6f76 6554 6f28 302c 2032 292e 7265 6374  oveTo(0, 2).rect
-00025c70: 2831 2c20 3129 2e65 7874 7275 6465 2832  (1, 1).extrude(2
-00025c80: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00025c90: 2020 2020 7265 7320 3d20 6f62 6a2e 756e      res = obj.un
-00025ca0: 696f 6e28 626f 7832 2c20 676c 7565 3d54  ion(box2, glue=T
-00025cb0: 7275 6529 0a0a 2020 2020 2020 2020 7365  rue)..        se
-00025cc0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00025cd0: 6573 2e66 6163 6573 2829 2e73 697a 6528  es.faces().size(
-00025ce0: 292c 2031 3029 0a0a 2020 2020 6465 6620  ), 10)..    def 
-00025cf0: 7465 7374 4675 7a7a 7942 6f6f 6c4f 7028  testFuzzyBoolOp(
-00025d00: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-00025d10: 6570 7320 3d20 3165 2d33 0a0a 2020 2020  eps = 1e-3..    
-00025d20: 2020 2020 626f 7831 203d 2057 6f72 6b70      box1 = Workp
-00025d30: 6c61 6e65 2822 5859 2229 2e62 6f78 2831  lane("XY").box(1
-00025d40: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-00025d50: 626f 7832 203d 2057 6f72 6b70 6c61 6e65  box2 = Workplane
-00025d60: 2822 5859 222c 206f 7269 6769 6e3d 2831  ("XY", origin=(1
-00025d70: 202b 2065 7073 2c20 302e 3029 292e 626f   + eps, 0.0)).bo
-00025d80: 7828 312c 2031 2c20 3129 0a20 2020 2020  x(1, 1, 1).     
-00025d90: 2020 2062 6f78 3320 3d20 576f 726b 706c     box3 = Workpl
-00025da0: 616e 6528 2258 5922 2c20 6f72 6967 696e  ane("XY", origin
-00025db0: 3d28 322c 2030 2c20 3029 292e 626f 7828  =(2, 0, 0)).box(
-00025dc0: 312c 2031 2c20 3129 0a0a 2020 2020 2020  1, 1, 1)..      
-00025dd0: 2020 7265 7320 3d20 626f 7831 2e75 6e69    res = box1.uni
-00025de0: 6f6e 2862 6f78 3229 0a20 2020 2020 2020  on(box2).       
-00025df0: 2072 6573 5f66 757a 7a79 203d 2062 6f78   res_fuzzy = box
-00025e00: 312e 756e 696f 6e28 626f 7832 2c20 746f  1.union(box2, to
-00025e10: 6c3d 6570 7329 0a20 2020 2020 2020 2072  l=eps).        r
-00025e20: 6573 5f66 757a 7a79 3220 3d20 626f 7831  es_fuzzy2 = box1
-00025e30: 2e75 6e69 6f6e 2862 6f78 3329 2e75 6e69  .union(box3).uni
-00025e40: 6f6e 2862 6f78 322c 2074 6f6c 3d65 7073  on(box2, tol=eps
-00025e50: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00025e60: 6173 7365 7274 4571 7561 6c28 7265 732e  assertEqual(res.
-00025e70: 736f 6c69 6473 2829 2e73 697a 6528 292c  solids().size(),
-00025e80: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-00025e90: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
-00025ea0: 5f66 757a 7a79 2e73 6f6c 6964 7328 292e  _fuzzy.solids().
-00025eb0: 7369 7a65 2829 2c20 3129 0a20 2020 2020  size(), 1).     
-00025ec0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00025ed0: 7561 6c28 7265 735f 6675 7a7a 7932 2e73  ual(res_fuzzy2.s
-00025ee0: 6f6c 6964 7328 292e 7369 7a65 2829 2c20  olids().size(), 
-00025ef0: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
-00025f00: 4c6f 6361 7465 644d 6f76 6564 2873 656c  LocatedMoved(sel
-00025f10: 6629 3a0a 0a20 2020 2020 2020 2062 6f78  f):..        box
-00025f20: 203d 2053 6f6c 6964 2e6d 616b 6542 6f78   = Solid.makeBox
-00025f30: 2831 2c20 312c 2031 2c20 5665 6374 6f72  (1, 1, 1, Vector
-00025f40: 282d 302e 352c 202d 302e 352c 202d 302e  (-0.5, -0.5, -0.
-00025f50: 3529 290a 2020 2020 2020 2020 6c6f 6320  5)).        loc 
-00025f60: 3d20 4c6f 6361 7469 6f6e 2856 6563 746f  = Location(Vecto
-00025f70: 7228 312c 2031 2c20 3129 290a 0a20 2020  r(1, 1, 1))..   
-00025f80: 2020 2020 2062 6f78 3120 3d20 626f 782e       box1 = box.
-00025f90: 6c6f 6361 7465 6428 6c6f 6329 0a0a 2020  located(loc)..  
-00025fa0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00025fb0: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
-00025fc0: 6c73 2862 6f78 312e 4365 6e74 6572 2829  ls(box1.Center()
-00025fd0: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
-00025fe0: 312c 2031 292c 2036 290a 2020 2020 2020  1, 1), 6).      
-00025ff0: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
-00026000: 6c65 416c 6d6f 7374 4571 7561 6c73 2862  leAlmostEquals(b
-00026010: 6f78 2e43 656e 7465 7228 292e 746f 5475  ox.Center().toTu
-00026020: 706c 6528 292c 2028 302c 2030 2c20 3029  ple(), (0, 0, 0)
-00026030: 2c20 3629 0a0a 2020 2020 2020 2020 626f  , 6)..        bo
-00026040: 782e 6c6f 6361 7465 286c 6f63 290a 0a20  x.locate(loc).. 
-00026050: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00026060: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
-00026070: 616c 7328 626f 782e 4365 6e74 6572 2829  als(box.Center()
-00026080: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
-00026090: 312c 2031 292c 2036 290a 0a20 2020 2020  1, 1), 6)..     
-000260a0: 2020 2062 6f78 3220 3d20 626f 782e 6d6f     box2 = box.mo
-000260b0: 7665 6428 6c6f 6329 0a0a 2020 2020 2020  ved(loc)..      
-000260c0: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
-000260d0: 6c65 416c 6d6f 7374 4571 7561 6c73 2862  leAlmostEquals(b
-000260e0: 6f78 2e43 656e 7465 7228 292e 746f 5475  ox.Center().toTu
-000260f0: 706c 6528 292c 2028 312c 2031 2c20 3129  ple(), (1, 1, 1)
-00026100: 2c20 3629 0a20 2020 2020 2020 2073 656c  , 6).        sel
-00026110: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
-00026120: 6f73 7445 7175 616c 7328 626f 7832 2e43  ostEquals(box2.C
-00026130: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
-00026140: 292c 2028 322c 2032 2c20 3229 2c20 3629  ), (2, 2, 2), 6)
-00026150: 0a0a 2020 2020 2020 2020 626f 782e 6d6f  ..        box.mo
-00026160: 7665 286c 6f63 290a 0a20 2020 2020 2020  ve(loc)..       
-00026170: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
-00026180: 6541 6c6d 6f73 7445 7175 616c 7328 626f  eAlmostEquals(bo
-00026190: 782e 4365 6e74 6572 2829 2e74 6f54 7570  x.Center().toTup
-000261a0: 6c65 2829 2c20 2832 2c20 322c 2032 292c  le(), (2, 2, 2),
-000261b0: 2036 290a 0a20 2020 2064 6566 2074 6573   6)..    def tes
-000261c0: 744e 756c 6c53 6861 7065 2873 656c 6629  tNullShape(self)
-000261d0: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
-000261e0: 4f43 502e 546f 706f 4453 2069 6d70 6f72  OCP.TopoDS impor
-000261f0: 7420 546f 706f 4453 5f53 6861 7065 0a0a  t TopoDS_Shape..
-00026200: 2020 2020 2020 2020 7320 3d20 546f 706f          s = Topo
-00026210: 4453 5f53 6861 7065 2829 0a0a 2020 2020  DS_Shape()..    
-00026220: 2020 2020 2320 6d61 6b65 2073 7572 6520      # make sure 
-00026230: 7261 6973 6573 206f 6e20 6e6f 6e20 736f  raises on non so
-00026240: 6c69 640a 2020 2020 2020 2020 7769 7468  lid.        with
-00026250: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00026260: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
-00026270: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
-00026280: 6f63 635f 696d 706c 2e73 6861 7065 732e  occ_impl.shapes.
-00026290: 646f 776e 6361 7374 2873 290a 0a20 2020  downcast(s)..   
-000262a0: 2064 6566 2074 6573 7443 656e 7465 724f   def testCenterO
-000262b0: 6642 6f75 6e64 426f 7828 7365 6c66 293a  fBoundBox(self):
-000262c0: 0a0a 2020 2020 2020 2020 6f62 6a20 3d20  ..        obj = 
-000262d0: 576f 726b 706c 616e 6528 292e 7075 7368  Workplane().push
-000262e0: 506f 696e 7473 285b 2830 2c20 3029 2c20  Points([(0, 0), 
-000262f0: 2832 2c20 3229 5d29 2e62 6f78 2831 2c20  (2, 2)]).box(1, 
-00026300: 312c 2031 290a 2020 2020 2020 2020 6320  1, 1).        c 
-00026310: 3d20 6f62 6a2e 776f 726b 706c 616e 6528  = obj.workplane(
-00026320: 6365 6e74 6572 4f70 7469 6f6e 3d22 4365  centerOption="Ce
-00026330: 6e74 6572 4f66 426f 756e 6442 6f78 2229  nterOfBoundBox")
-00026340: 2e70 6c61 6e65 2e6f 7269 6769 6e0a 0a20  .plane.origin.. 
-00026350: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00026360: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
-00026370: 616c 7328 632e 746f 5475 706c 6528 292c  als(c.toTuple(),
-00026380: 2028 312c 2031 2c20 3029 2c20 3629 0a0a   (1, 1, 0), 6)..
-00026390: 2020 2020 6465 6620 7465 7374 4f66 6673      def testOffs
-000263a0: 6574 3244 2873 656c 6629 3a0a 0a20 2020  et2D(self):..   
-000263b0: 2020 2020 2077 3120 3d20 576f 726b 706c       w1 = Workpl
-000263c0: 616e 6528 292e 7265 6374 2831 2c20 3129  ane().rect(1, 1)
-000263d0: 2e6f 6666 7365 7432 4428 302e 352c 2022  .offset2D(0.5, "
-000263e0: 6172 6322 290a 2020 2020 2020 2020 7365  arc").        se
-000263f0: 6c66 2e61 7373 6572 7445 7175 616c 2877  lf.assertEqual(w
-00026400: 312e 6564 6765 7328 292e 7369 7a65 2829  1.edges().size()
-00026410: 2c20 3829 0a0a 2020 2020 2020 2020 7732  , 8)..        w2
-00026420: 203d 2057 6f72 6b70 6c61 6e65 2829 2e72   = Workplane().r
-00026430: 6563 7428 312c 2031 292e 6f66 6673 6574  ect(1, 1).offset
-00026440: 3244 2830 2e35 2c20 2274 616e 6765 6e74  2D(0.5, "tangent
-00026450: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00026460: 6173 7365 7274 4571 7561 6c28 7732 2e65  assertEqual(w2.e
-00026470: 6467 6573 2829 2e73 697a 6528 292c 2034  dges().size(), 4
-00026480: 290a 0a20 2020 2020 2020 2077 3320 3d20  )..        w3 = 
-00026490: 576f 726b 706c 616e 6528 292e 7265 6374  Workplane().rect
-000264a0: 2831 2c20 3129 2e6f 6666 7365 7432 4428  (1, 1).offset2D(
-000264b0: 302e 352c 2022 696e 7465 7273 6563 7469  0.5, "intersecti
-000264c0: 6f6e 2229 0a20 2020 2020 2020 2073 656c  on").        sel
-000264d0: 662e 6173 7365 7274 4571 7561 6c28 7733  f.assertEqual(w3
-000264e0: 2e65 6467 6573 2829 2e73 697a 6528 292c  .edges().size(),
-000264f0: 2034 290a 0a20 2020 2020 2020 2077 3420   4)..        w4 
-00026500: 3d20 576f 726b 706c 616e 6528 292e 7075  = Workplane().pu
-00026510: 7368 506f 696e 7473 285b 2830 2c20 3029  shPoints([(0, 0)
-00026520: 2c20 2830 2c20 3529 5d29 2e72 6563 7428  , (0, 5)]).rect(
-00026530: 312c 2031 292e 6f66 6673 6574 3244 282d  1, 1).offset2D(-
-00026540: 302e 3529 0a20 2020 2020 2020 2073 656c  0.5).        sel
-00026550: 662e 6173 7365 7274 4571 7561 6c28 7734  f.assertEqual(w4
-00026560: 2e77 6972 6573 2829 2e73 697a 6528 292c  .wires().size(),
-00026570: 2030 290a 0a20 2020 2020 2020 2077 3520   0)..        w5 
-00026580: 3d20 576f 726b 706c 616e 6528 292e 7075  = Workplane().pu
-00026590: 7368 506f 696e 7473 285b 2830 2c20 3029  shPoints([(0, 0)
-000265a0: 2c20 2830 2c20 3529 5d29 2e72 6563 7428  , (0, 5)]).rect(
-000265b0: 312c 2031 292e 6f66 6673 6574 3244 282d  1, 1).offset2D(-
-000265c0: 302e 3235 290a 2020 2020 2020 2020 7365  0.25).        se
-000265d0: 6c66 2e61 7373 6572 7445 7175 616c 2877  lf.assertEqual(w
-000265e0: 352e 7769 7265 7328 292e 7369 7a65 2829  5.wires().size()
-000265f0: 2c20 3229 0a0a 2020 2020 2020 2020 7220  , 2)..        r 
-00026600: 3d20 3230 0a20 2020 2020 2020 2073 203d  = 20.        s =
-00026610: 2037 0a20 2020 2020 2020 2074 203d 2031   7.        t = 1
-00026620: 2e35 0a0a 2020 2020 2020 2020 706f 696e  .5..        poin
-00026630: 7473 203d 205b 0a20 2020 2020 2020 2020  ts = [.         
-00026640: 2020 2028 302c 2074 202f 2032 292c 0a20     (0, t / 2),. 
-00026650: 2020 2020 2020 2020 2020 2028 7220 2f20             (r / 
-00026660: 3220 2d20 312e 3520 2a20 742c 2072 202f  2 - 1.5 * t, r /
-00026670: 2032 202d 2074 292c 0a20 2020 2020 2020   2 - t),.       
-00026680: 2020 2020 2028 7320 2f20 322c 2072 202f       (s / 2, r /
-00026690: 2032 202d 2074 292c 0a20 2020 2020 2020   2 - t),.       
-000266a0: 2020 2020 2028 7320 2f20 322c 2072 202f       (s / 2, r /
-000266b0: 2032 292c 0a20 2020 2020 2020 2020 2020   2),.           
-000266c0: 2028 7220 2f20 322c 2072 202f 2032 292c   (r / 2, r / 2),
-000266d0: 0a20 2020 2020 2020 2020 2020 2028 7220  .            (r 
-000266e0: 2f20 322c 2073 202f 2032 292c 0a20 2020  / 2, s / 2),.   
-000266f0: 2020 2020 2020 2020 2028 7220 2f20 3220           (r / 2 
-00026700: 2d20 742c 2073 202f 2032 292c 0a20 2020  - t, s / 2),.   
-00026710: 2020 2020 2020 2020 2028 7220 2f20 3220           (r / 2 
-00026720: 2d20 742c 2072 202f 2032 202d 2031 2e35  - t, r / 2 - 1.5
-00026730: 202a 2074 292c 0a20 2020 2020 2020 2020   * t),.         
-00026740: 2020 2028 7420 2f20 322c 2030 292c 0a20     (t / 2, 0),. 
-00026750: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00026760: 2020 7320 3d20 280a 2020 2020 2020 2020    s = (.        
-00026770: 2020 2020 576f 726b 706c 616e 6528 2258      Workplane("X
-00026780: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
-00026790: 2e70 6f6c 796c 696e 6528 706f 696e 7473  .polyline(points
-000267a0: 290a 2020 2020 2020 2020 2020 2020 2e6d  ).            .m
-000267b0: 6972 726f 7258 2829 0a20 2020 2020 2020  irrorX().       
-000267c0: 2020 2020 202e 6d69 7272 6f72 5928 290a       .mirrorY().
-000267d0: 2020 2020 2020 2020 2020 2020 2e6f 6666              .off
-000267e0: 7365 7432 4428 2d30 2e39 290a 2020 2020  set2D(-0.9).    
-000267f0: 2020 2020 2020 2020 2e65 7874 7275 6465          .extrude
-00026800: 2831 290a 2020 2020 2020 2020 290a 2020  (1).        ).  
-00026810: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00026820: 7445 7175 616c 2873 2e73 6f6c 6964 7328  tEqual(s.solids(
-00026830: 292e 7369 7a65 2829 2c20 3429 0a0a 2020  ).size(), 4)..  
-00026840: 2020 2020 2020 2320 7465 7374 2066 6f72        # test for
-00026850: 436f 6e73 7472 7563 7469 6f6e 0a20 2020  Construction.   
-00026860: 2020 2020 2023 2066 6f72 436f 6e73 7472       # forConstr
-00026870: 7563 7469 6f6e 3d54 7275 6520 7368 6f75  uction=True shou
-00026880: 6c64 2070 6c61 6365 2072 6573 756c 7473  ld place results
-00026890: 2069 6e20 6f62 6a65 6374 732c 206e 6f74   in objects, not
-000268a0: 2063 7478 2e70 656e 6469 6e67 5769 7265   ctx.pendingWire
-000268b0: 730a 2020 2020 2020 2020 7736 203d 2057  s.        w6 = W
-000268c0: 6f72 6b70 6c61 6e65 2829 2e68 4c69 6e65  orkplane().hLine
-000268d0: 2831 292e 764c 696e 6528 3129 2e63 6c6f  (1).vLine(1).clo
-000268e0: 7365 2829 2e6f 6666 7365 7432 4428 302e  se().offset2D(0.
-000268f0: 352c 2066 6f72 436f 6e73 7472 7563 7469  5, forConstructi
-00026900: 6f6e 3d54 7275 6529 0a20 2020 2020 2020  on=True).       
-00026910: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00026920: 6c28 6c65 6e28 7736 2e63 7478 2e70 656e  l(len(w6.ctx.pen
-00026930: 6469 6e67 5769 7265 7329 2c20 3029 0a20  dingWires), 0). 
-00026940: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00026950: 7274 4571 7561 6c28 7736 2e73 697a 6528  rtEqual(w6.size(
-00026960: 292c 2031 290a 2020 2020 2020 2020 7365  ), 1).        se
-00026970: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00026980: 7970 6528 7736 2e76 616c 2829 292c 2057  ype(w6.val()), W
-00026990: 6972 6529 0a20 2020 2020 2020 2023 206d  ire).        # m
-000269a0: 616b 6520 7375 7265 2074 6865 2072 6573  ake sure the res
-000269b0: 756c 7469 6e67 2077 6972 6520 6861 7320  ulting wire has 
-000269c0: 666f 7243 6f6e 7374 7275 6374 696f 6e20  forConstruction 
-000269d0: 7365 740a 2020 2020 2020 2020 7365 6c66  set.        self
-000269e0: 2e61 7373 6572 7445 7175 616c 2877 362e  .assertEqual(w6.
-000269f0: 7661 6c28 292e 666f 7243 6f6e 7374 7275  val().forConstru
-00026a00: 6374 696f 6e2c 2054 7275 6529 0a0a 2020  ction, True)..  
-00026a10: 2020 6465 6620 7465 7374 436f 6e73 6f6c    def testConsol
-00026a20: 6964 6174 6557 6972 6573 2873 656c 6629  idateWires(self)
-00026a30: 3a0a 0a20 2020 2020 2020 2077 3120 3d20  :..        w1 = 
-00026a40: 576f 726b 706c 616e 6528 292e 6c69 6e65  Workplane().line
-00026a50: 546f 2830 2c20 3129 2e6c 696e 6554 6f28  To(0, 1).lineTo(
-00026a60: 312c 2031 292e 636f 6e73 6f6c 6964 6174  1, 1).consolidat
-00026a70: 6557 6972 6573 2829 0a20 2020 2020 2020  eWires().       
-00026a80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00026a90: 6c28 7731 2e73 697a 6528 292c 2031 290a  l(w1.size(), 1).
-00026aa0: 0a20 2020 2020 2020 2077 3120 3d20 576f  .        w1 = Wo
-00026ab0: 726b 706c 616e 6528 292e 636f 6e73 6f6c  rkplane().consol
-00026ac0: 6964 6174 6557 6972 6573 2829 0a20 2020  idateWires().   
-00026ad0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00026ae0: 4571 7561 6c28 7731 2e73 697a 6528 292c  Equal(w1.size(),
-00026af0: 2030 290a 0a20 2020 2064 6566 2074 6573   0)..    def tes
-00026b00: 744c 6f63 6174 696f 6e41 7428 7365 6c66  tLocationAt(self
-00026b10: 293a 0a0a 2020 2020 2020 2020 7220 3d20  ):..        r = 
-00026b20: 310a 2020 2020 2020 2020 6520 3d20 5769  1.        e = Wi
-00026b30: 7265 2e6d 616b 6548 656c 6978 2872 2c20  re.makeHelix(r, 
-00026b40: 722c 2072 292e 4564 6765 7328 295b 305d  r, r).Edges()[0]
-00026b50: 0a0a 2020 2020 2020 2020 6c6f 6373 5f66  ..        locs_f
-00026b60: 7265 6e65 7420 3d20 652e 6c6f 6361 7469  renet = e.locati
-00026b70: 6f6e 7328 5b30 2c20 315d 2c20 6672 616d  ons([0, 1], fram
-00026b80: 653d 2266 7265 6e65 7422 290a 0a20 2020  e="frenet")..   
-00026b90: 2020 2020 2054 3120 3d20 6c6f 6373 5f66       T1 = locs_f
-00026ba0: 7265 6e65 745b 305d 2e77 7261 7070 6564  renet[0].wrapped
-00026bb0: 2e54 7261 6e73 666f 726d 6174 696f 6e28  .Transformation(
-00026bc0: 290a 2020 2020 2020 2020 5432 203d 206c  ).        T2 = l
-00026bd0: 6f63 735f 6672 656e 6574 5b31 5d2e 7772  ocs_frenet[1].wr
-00026be0: 6170 7065 642e 5472 616e 7366 6f72 6d61  apped.Transforma
-00026bf0: 7469 6f6e 2829 0a0a 2020 2020 2020 2020  tion()..        
-00026c00: 7365 6c66 2e61 7373 6572 7441 6c6d 6f73  self.assertAlmos
-00026c10: 7445 7175 616c 2854 312e 5472 616e 736c  tEqual(T1.Transl
-00026c20: 6174 696f 6e50 6172 7428 292e 5828 292c  ationPart().X(),
-00026c30: 2072 2c20 3629 0a20 2020 2020 2020 2073   r, 6).        s
-00026c40: 656c 662e 6173 7365 7274 416c 6d6f 7374  elf.assertAlmost
-00026c50: 4571 7561 6c28 5432 2e54 7261 6e73 6c61  Equal(T2.Transla
-00026c60: 7469 6f6e 5061 7274 2829 2e58 2829 2c20  tionPart().X(), 
-00026c70: 722c 2036 290a 2020 2020 2020 2020 7365  r, 6).        se
-00026c80: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
-00026c90: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00026ca0: 2020 5431 2e47 6574 526f 7461 7469 6f6e    T1.GetRotation
-00026cb0: 2829 2e47 6574 526f 7461 7469 6f6e 416e  ().GetRotationAn
-00026cc0: 676c 6528 292c 202d 5432 2e47 6574 526f  gle(), -T2.GetRo
-00026cd0: 7461 7469 6f6e 2829 2e47 6574 526f 7461  tation().GetRota
-00026ce0: 7469 6f6e 416e 676c 6528 292c 2036 0a20  tionAngle(), 6. 
-00026cf0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00026d00: 2020 6761 203d 2065 2e5f 6765 6f6d 4164    ga = e._geomAd
-00026d10: 6170 746f 7228 290a 0a20 2020 2020 2020  aptor()..       
-00026d20: 206c 6f63 735f 636f 7272 6563 7465 6420   locs_corrected 
-00026d30: 3d20 652e 6c6f 6361 7469 6f6e 7328 0a20  = e.locations(. 
-00026d40: 2020 2020 2020 2020 2020 205b 6761 2e46             [ga.F
-00026d50: 6972 7374 5061 7261 6d65 7465 7228 292c  irstParameter(),
-00026d60: 2067 612e 4c61 7374 5061 7261 6d65 7465   ga.LastParamete
-00026d70: 7228 295d 2c0a 2020 2020 2020 2020 2020  r()],.          
-00026d80: 2020 6d6f 6465 3d22 7061 7261 6d65 7465    mode="paramete
-00026d90: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-00026da0: 6672 616d 653d 2263 6f72 7265 6374 6564  frame="corrected
-00026db0: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
-00026dc0: 2020 2020 2020 5433 203d 206c 6f63 735f        T3 = locs_
-00026dd0: 636f 7272 6563 7465 645b 305d 2e77 7261  corrected[0].wra
-00026de0: 7070 6564 2e54 7261 6e73 666f 726d 6174  pped.Transformat
-00026df0: 696f 6e28 290a 2020 2020 2020 2020 5434  ion().        T4
-00026e00: 203d 206c 6f63 735f 636f 7272 6563 7465   = locs_correcte
-00026e10: 645b 315d 2e77 7261 7070 6564 2e54 7261  d[1].wrapped.Tra
-00026e20: 6e73 666f 726d 6174 696f 6e28 290a 0a20  nsformation().. 
-00026e30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00026e40: 7274 416c 6d6f 7374 4571 7561 6c28 5433  rtAlmostEqual(T3
-00026e50: 2e54 7261 6e73 6c61 7469 6f6e 5061 7274  .TranslationPart
-00026e60: 2829 2e58 2829 2c20 722c 2036 290a 2020  ().X(), r, 6).  
-00026e70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00026e80: 7441 6c6d 6f73 7445 7175 616c 2854 342e  tAlmostEqual(T4.
-00026e90: 5472 616e 736c 6174 696f 6e50 6172 7428  TranslationPart(
-00026ea0: 292e 5828 292c 2072 2c20 3629 0a0a 2020  ).X(), r, 6)..  
-00026eb0: 2020 2020 2020 7720 3d20 5769 7265 2e61        w = Wire.a
-00026ec0: 7373 656d 626c 6545 6467 6573 280a 2020  ssembleEdges(.  
-00026ed0: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
-00026ee0: 2020 2020 2020 2020 2020 2020 4564 6765              Edge
-00026ef0: 2e6d 616b 654c 696e 6528 5665 6374 6f72  .makeLine(Vector
-00026f00: 2829 2c20 5665 6374 6f72 2830 2c20 3129  (), Vector(0, 1)
-00026f10: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00026f20: 2020 2045 6467 652e 6d61 6b65 4c69 6e65     Edge.makeLine
-00026f30: 2856 6563 746f 7228 302c 2031 292c 2056  (Vector(0, 1), V
-00026f40: 6563 746f 7228 312c 2031 2929 2c0a 2020  ector(1, 1)),.  
-00026f50: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00026f60: 2020 2020 290a 2020 2020 2020 2020 6c6f      ).        lo
-00026f70: 6373 5f77 6972 6520 3d20 652e 6c6f 6361  cs_wire = e.loca
-00026f80: 7469 6f6e 7328 5b30 2c20 315d 290a 0a20  tions([0, 1]).. 
-00026f90: 2020 2020 2020 2054 3520 3d20 6c6f 6373         T5 = locs
-00026fa0: 5f77 6972 655b 305d 2e77 7261 7070 6564  _wire[0].wrapped
-00026fb0: 2e54 7261 6e73 666f 726d 6174 696f 6e28  .Transformation(
-00026fc0: 290a 2020 2020 2020 2020 5436 203d 206c  ).        T6 = l
-00026fd0: 6f63 735f 7769 7265 5b31 5d2e 7772 6170  ocs_wire[1].wrap
-00026fe0: 7065 642e 5472 616e 7366 6f72 6d61 7469  ped.Transformati
-00026ff0: 6f6e 2829 0a0a 2020 2020 2020 2020 7365  on()..        se
-00027000: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
-00027010: 7175 616c 2854 352e 5472 616e 736c 6174  qual(T5.Translat
-00027020: 696f 6e50 6172 7428 292e 5828 292c 2072  ionPart().X(), r
-00027030: 2c20 3029 0a20 2020 2020 2020 2073 656c  , 0).        sel
-00027040: 662e 6173 7365 7274 416c 6d6f 7374 4571  f.assertAlmostEq
-00027050: 7561 6c28 5436 2e54 7261 6e73 6c61 7469  ual(T6.Translati
-00027060: 6f6e 5061 7274 2829 2e58 2829 2c20 722c  onPart().X(), r,
-00027070: 2031 290a 0a20 2020 2064 6566 2074 6573   1)..    def tes
-00027080: 744e 6f72 6d61 6c28 7365 6c66 293a 0a0a  tNormal(self):..
-00027090: 2020 2020 2020 2020 6369 7263 203d 2057          circ = W
-000270a0: 6f72 6b70 6c61 6e65 2829 2e63 6972 636c  orkplane().circl
-000270b0: 6528 3129 2e65 6467 6573 2829 2e76 616c  e(1).edges().val
-000270c0: 2829 0a20 2020 2020 2020 206e 203d 2063  ().        n = c
-000270d0: 6972 632e 6e6f 726d 616c 2829 0a0a 2020  irc.normal()..  
-000270e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000270f0: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
-00027100: 6c73 286e 2e74 6f54 7570 6c65 2829 2c20  ls(n.toTuple(), 
-00027110: 2830 2c20 302c 2031 292c 2036 290a 0a20  (0, 0, 1), 6).. 
-00027120: 2020 2020 2020 2065 6c6c 203d 2057 6f72         ell = Wor
-00027130: 6b70 6c61 6e65 2829 2e65 6c6c 6970 7365  kplane().ellipse
-00027140: 2831 2c20 3229 2e65 6467 6573 2829 2e76  (1, 2).edges().v
-00027150: 616c 2829 0a20 2020 2020 2020 206e 203d  al().        n =
-00027160: 2065 6c6c 2e6e 6f72 6d61 6c28 290a 0a20   ell.normal().. 
-00027170: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00027180: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
-00027190: 616c 7328 6e2e 746f 5475 706c 6528 292c  als(n.toTuple(),
-000271a0: 2028 302c 2030 2c20 3129 2c20 3629 0a0a   (0, 0, 1), 6)..
-000271b0: 2020 2020 2020 2020 7220 3d20 576f 726b          r = Work
-000271c0: 706c 616e 6528 292e 7265 6374 2831 2c20  plane().rect(1, 
-000271d0: 3229 2e77 6972 6573 2829 2e76 616c 2829  2).wires().val()
-000271e0: 0a20 2020 2020 2020 206e 203d 2072 2e6e  .        n = r.n
-000271f0: 6f72 6d61 6c28 290a 0a20 2020 2020 2020  ormal()..       
-00027200: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
-00027210: 6541 6c6d 6f73 7445 7175 616c 7328 6e2e  eAlmostEquals(n.
-00027220: 746f 5475 706c 6528 292c 2028 302c 2030  toTuple(), (0, 0
-00027230: 2c20 3129 2c20 3629 0a0a 2020 2020 2020  , 1), 6)..      
-00027240: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-00027250: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
-00027260: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-00027270: 2020 6564 6765 203d 2057 6f72 6b70 6c61    edge = Workpla
-00027280: 6e65 2829 2e72 6563 7428 312c 2032 292e  ne().rect(1, 2).
-00027290: 6564 6765 7328 292e 7661 6c28 290a 2020  edges().val().  
-000272a0: 2020 2020 2020 2020 2020 6e20 3d20 6564            n = ed
-000272b0: 6765 2e6e 6f72 6d61 6c28 290a 0a20 2020  ge.normal()..   
-000272c0: 2064 6566 2074 6573 7450 6f73 6974 696f   def testPositio
-000272d0: 6e41 7428 7365 6c66 293a 0a0a 2020 2020  nAt(self):..    
-000272e0: 2020 2020 2320 7465 7374 2077 6974 6820      # test with 
-000272f0: 616e 206f 7065 6e20 7769 7265 0a20 2020  an open wire.   
-00027300: 2020 2020 2077 203d 2057 6f72 6b70 6c61       w = Workpla
-00027310: 6e65 2829 2e6c 696e 6554 6f28 302c 2031  ne().lineTo(0, 1
-00027320: 292e 6c69 6e65 546f 2831 2c20 3129 2e77  ).lineTo(1, 1).w
-00027330: 6972 6528 292e 7661 6c28 290a 0a20 2020  ire().val()..   
-00027340: 2020 2020 2070 3020 3d20 772e 706f 7369       p0 = w.posi
-00027350: 7469 6f6e 4174 2830 2e30 290a 2020 2020  tionAt(0.0).    
-00027360: 2020 2020 7031 203d 2077 2e70 6f73 6974      p1 = w.posit
-00027370: 696f 6e41 7428 302e 3529 0a20 2020 2020  ionAt(0.5).     
-00027380: 2020 2070 3220 3d20 772e 706f 7369 7469     p2 = w.positi
-00027390: 6f6e 4174 2831 2e30 290a 0a20 2020 2020  onAt(1.0)..     
-000273a0: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
-000273b0: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
-000273c0: 7030 2e74 6f54 7570 6c65 2829 2c20 2830  p0.toTuple(), (0
-000273d0: 2c20 302c 2030 292c 2036 290a 2020 2020  , 0, 0), 6).    
-000273e0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-000273f0: 7570 6c65 416c 6d6f 7374 4571 7561 6c73  upleAlmostEquals
-00027400: 2870 312e 746f 5475 706c 6528 292c 2028  (p1.toTuple(), (
-00027410: 302c 2031 2c20 3029 2c20 3629 0a20 2020  0, 1, 0), 6).   
-00027420: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00027430: 5475 706c 6541 6c6d 6f73 7445 7175 616c  TupleAlmostEqual
-00027440: 7328 7032 2e74 6f54 7570 6c65 2829 2c20  s(p2.toTuple(), 
-00027450: 2831 2c20 312c 2030 292c 2036 290a 0a20  (1, 1, 0), 6).. 
-00027460: 2020 2020 2020 2070 3020 3d20 772e 706f         p0 = w.po
-00027470: 7369 7469 6f6e 4174 2830 2e30 2c20 6d6f  sitionAt(0.0, mo
-00027480: 6465 3d22 7061 7261 6d22 290a 0a20 2020  de="param")..   
-00027490: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000274a0: 5475 706c 6541 6c6d 6f73 7445 7175 616c  TupleAlmostEqual
-000274b0: 7328 7030 2e74 6f54 7570 6c65 2829 2c20  s(p0.toTuple(), 
-000274c0: 2830 2c20 302c 2030 292c 2036 290a 0a20  (0, 0, 0), 6).. 
-000274d0: 2020 2020 2020 2070 302c 2070 312c 2070         p0, p1, p
-000274e0: 3220 3d20 772e 706f 7369 7469 6f6e 7328  2 = w.positions(
-000274f0: 5b30 2e30 2c20 302e 3235 2c20 302e 355d  [0.0, 0.25, 0.5]
-00027500: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00027510: 6173 7365 7274 5475 706c 6541 6c6d 6f73  assertTupleAlmos
-00027520: 7445 7175 616c 7328 7030 2e74 6f54 7570  tEquals(p0.toTup
-00027530: 6c65 2829 2c20 2830 2c20 302c 2030 292c  le(), (0, 0, 0),
-00027540: 2036 290a 2020 2020 2020 2020 7365 6c66   6).        self
-00027550: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
-00027560: 7374 4571 7561 6c73 2870 312e 746f 5475  stEquals(p1.toTu
-00027570: 706c 6528 292c 2028 302c 2030 2e35 2c20  ple(), (0, 0.5, 
-00027580: 3029 2c20 3629 0a20 2020 2020 2020 2073  0), 6).        s
-00027590: 656c 662e 6173 7365 7274 5475 706c 6541  elf.assertTupleA
-000275a0: 6c6d 6f73 7445 7175 616c 7328 7032 2e74  lmostEquals(p2.t
-000275b0: 6f54 7570 6c65 2829 2c20 2830 2c20 312c  oTuple(), (0, 1,
-000275c0: 2030 292c 2036 290a 0a20 2020 2020 2020   0), 6)..       
-000275d0: 2023 2074 6573 7420 7769 7468 2061 2063   # test with a c
-000275e0: 6c6f 7365 6420 7769 7265 0a20 2020 2020  losed wire.     
-000275f0: 2020 2077 203d 2057 6f72 6b70 6c61 6e65     w = Workplane
-00027600: 2829 2e6c 696e 6554 6f28 302c 2031 292e  ().lineTo(0, 1).
-00027610: 636c 6f73 6528 292e 7769 7265 2829 2e76  close().wire().v
-00027620: 616c 2829 0a0a 2020 2020 2020 2020 7030  al()..        p0
-00027630: 203d 2077 2e70 6f73 6974 696f 6e41 7428   = w.positionAt(
-00027640: 302e 3029 0a20 2020 2020 2020 2070 3120  0.0).        p1 
-00027650: 3d20 772e 706f 7369 7469 6f6e 4174 2830  = w.positionAt(0
-00027660: 2e35 290a 2020 2020 2020 2020 7032 203d  .5).        p2 =
-00027670: 2077 2e70 6f73 6974 696f 6e41 7428 312e   w.positionAt(1.
-00027680: 3029 0a0a 2020 2020 2020 2020 7365 6c66  0)..        self
-00027690: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
-000276a0: 7374 4571 7561 6c73 2870 302e 746f 5475  stEquals(p0.toTu
-000276b0: 706c 6528 292c 2070 322e 746f 5475 706c  ple(), p2.toTupl
-000276c0: 6528 292c 2036 290a 2020 2020 2020 2020  e(), 6).        
-000276d0: 7365 6c66 2e61 7373 6572 7454 7570 6c65  self.assertTuple
-000276e0: 416c 6d6f 7374 4571 7561 6c73 2870 312e  AlmostEquals(p1.
-000276f0: 746f 5475 706c 6528 292c 2028 302c 2031  toTuple(), (0, 1
-00027700: 2c20 3029 2c20 3629 0a0a 2020 2020 2020  , 0), 6)..      
-00027710: 2020 2320 7465 7374 2077 6974 6820 6172    # test with ar
-00027720: 6320 6f66 2063 6972 636c 650a 2020 2020  c of circle.    
-00027730: 2020 2020 6520 3d20 4564 6765 2e6d 616b      e = Edge.mak
-00027740: 6543 6972 636c 6528 312c 2028 302c 2030  eCircle(1, (0, 0
-00027750: 2c20 3029 2c20 2830 2c20 302c 2031 292c  , 0), (0, 0, 1),
-00027760: 2039 302c 2031 3830 290a 2020 2020 2020   90, 180).      
-00027770: 2020 7030 203d 2065 2e70 6f73 6974 696f    p0 = e.positio
-00027780: 6e41 7428 302e 3029 0a20 2020 2020 2020  nAt(0.0).       
-00027790: 2070 3120 3d20 652e 706f 7369 7469 6f6e   p1 = e.position
-000277a0: 4174 2831 2e30 290a 2020 2020 2020 2020  At(1.0).        
-000277b0: 6173 7365 7274 2070 302e 746f 5475 706c  assert p0.toTupl
-000277c0: 6528 2920 3d3d 2061 7070 726f 7828 2830  e() == approx((0
-000277d0: 2e30 2c20 312e 302c 2030 2e30 2929 0a20  .0, 1.0, 0.0)). 
-000277e0: 2020 2020 2020 2061 7373 6572 7420 7031         assert p1
-000277f0: 2e74 6f54 7570 6c65 2829 203d 3d20 6170  .toTuple() == ap
-00027800: 7072 6f78 2828 2d31 2e30 2c20 302e 302c  prox((-1.0, 0.0,
-00027810: 2030 2e30 2929 0a0a 2020 2020 2020 2020   0.0))..        
-00027820: 7720 3d20 5769 7265 2e61 7373 656d 626c  w = Wire.assembl
-00027830: 6545 6467 6573 285b 655d 290a 2020 2020  eEdges([e]).    
-00027840: 2020 2020 7030 203d 2077 2e70 6f73 6974      p0 = w.posit
-00027850: 696f 6e41 7428 302e 3029 0a20 2020 2020  ionAt(0.0).     
-00027860: 2020 2070 3120 3d20 772e 706f 7369 7469     p1 = w.positi
-00027870: 6f6e 4174 2831 2e30 290a 2020 2020 2020  onAt(1.0).      
-00027880: 2020 6173 7365 7274 2070 302e 746f 5475    assert p0.toTu
-00027890: 706c 6528 2920 3d3d 2061 7070 726f 7828  ple() == approx(
-000278a0: 2830 2e30 2c20 312e 302c 2030 2e30 2929  (0.0, 1.0, 0.0))
-000278b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000278c0: 7031 2e74 6f54 7570 6c65 2829 203d 3d20  p1.toTuple() == 
-000278d0: 6170 7072 6f78 2828 2d31 2e30 2c20 302e  approx((-1.0, 0.
-000278e0: 302c 2030 2e30 2929 0a0a 2020 2020 6465  0, 0.0))..    de
-000278f0: 6620 7465 7374 5461 6e67 656e 6741 7428  f testTangengAt(
-00027900: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-00027910: 7074 7320 3d20 5b28 302c 2030 292c 2028  pts = [(0, 0), (
-00027920: 2d31 2c20 3129 2c20 282d 322c 2030 292c  -1, 1), (-2, 0),
-00027930: 2028 2d31 2c20 3029 5d0a 0a20 2020 2020   (-1, 0)]..     
-00027940: 2020 2070 6174 6820 3d20 576f 726b 706c     path = Workpl
-00027950: 616e 6528 2258 5a22 292e 7370 6c69 6e65  ane("XZ").spline
-00027960: 2870 7473 2c20 7461 6e67 656e 7473 3d28  (pts, tangents=(
-00027970: 2830 2c20 3129 2c20 2831 2c20 3029 2929  (0, 1), (1, 0)))
-00027980: 2e76 616c 2829 0a0a 2020 2020 2020 2020  .val()..        
-00027990: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000279a0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-000279b0: 682e 7461 6e67 656e 7441 7428 302e 302c  h.tangentAt(0.0,
-000279c0: 206d 6f64 653d 2270 6172 616d 6574 6572   mode="parameter
-000279d0: 2229 203d 3d20 7061 7468 2e74 616e 6765  ") == path.tange
-000279e0: 6e74 4174 2830 2e30 2c20 6d6f 6465 3d22  ntAt(0.0, mode="
-000279f0: 6c65 6e67 7468 2229 0a20 2020 2020 2020  length").       
-00027a00: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00027a10: 6173 7365 7274 4661 6c73 6528 0a20 2020  assertFalse(.   
-00027a20: 2020 2020 2020 2020 2070 6174 682e 7461           path.ta
-00027a30: 6e67 656e 7441 7428 302e 352c 206d 6f64  ngentAt(0.5, mod
-00027a40: 653d 2270 6172 616d 6574 6572 2229 203d  e="parameter") =
-00027a50: 3d20 7061 7468 2e74 616e 6765 6e74 4174  = path.tangentAt
-00027a60: 2830 2e35 2c20 6d6f 6465 3d22 6c65 6e67  (0.5, mode="leng
-00027a70: 7468 2229 0a20 2020 2020 2020 2029 0a0a  th").        )..
-00027a80: 2020 2020 2020 2020 6172 6320 3d20 576f          arc = Wo
-00027a90: 726b 706c 616e 6528 292e 7261 6469 7573  rkplane().radius
-00027aa0: 4172 6328 2832 2c20 3029 2c20 3129 2e76  Arc((2, 0), 1).v
-00027ab0: 616c 2829 0a0a 2020 2020 2020 2020 7365  al()..        se
-00027ac0: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
-00027ad0: 6d6f 7374 4571 7561 6c73 280a 2020 2020  mostEquals(.    
-00027ae0: 2020 2020 2020 2020 6172 632e 7461 6e67          arc.tang
-00027af0: 656e 7441 7428 6d61 7468 2e70 6920 2f20  entAt(math.pi / 
-00027b00: 322c 2022 7061 7261 6d65 7465 7222 292e  2, "parameter").
-00027b10: 746f 5475 706c 6528 292c 2028 312c 2030  toTuple(), (1, 0
-00027b20: 2c20 3029 2c20 360a 2020 2020 2020 2020  , 0), 6.        
-00027b30: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00027b40: 7373 6572 7454 7570 6c65 416c 6d6f 7374  ssertTupleAlmost
-00027b50: 4571 7561 6c73 280a 2020 2020 2020 2020  Equals(.        
-00027b60: 2020 2020 6172 632e 7461 6e67 656e 7441      arc.tangentA
-00027b70: 7428 302e 352c 2022 6c65 6e67 7468 2229  t(0.5, "length")
-00027b80: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
-00027b90: 302c 2030 292c 2036 0a20 2020 2020 2020  0, 0), 6.       
-00027ba0: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-00027bb0: 456e 6428 7365 6c66 293a 0a0a 2020 2020  End(self):..    
-00027bc0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00027bd0: 7365 7274 5261 6973 6573 2856 616c 7565  sertRaises(Value
-00027be0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00027bf0: 2020 2020 576f 726b 706c 616e 6528 292e      Workplane().
-00027c00: 656e 6428 290a 0a20 2020 2020 2020 2073  end()..        s
-00027c10: 656c 662e 6173 7365 7274 5472 7565 2857  elf.assertTrue(W
-00027c20: 6f72 6b70 6c61 6e65 2829 2e6f 626a 6563  orkplane().objec
-00027c30: 7473 203d 3d20 5b5d 290a 2020 2020 2020  ts == []).      
-00027c40: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00027c50: 6528 576f 726b 706c 616e 6528 292e 626f  e(Workplane().bo
-00027c60: 7828 312c 2031 2c20 3129 2e65 6e64 2829  x(1, 1, 1).end()
-00027c70: 2e6f 626a 6563 7473 203d 3d20 5b5d 290a  .objects == []).
-00027c80: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00027c90: 6572 7454 7275 6528 576f 726b 706c 616e  ertTrue(Workplan
-00027ca0: 6528 292e 626f 7828 312c 2031 2c20 3129  e().box(1, 1, 1)
-00027cb0: 2e62 6f78 2832 2c20 322c 2031 292e 656e  .box(2, 2, 1).en
-00027cc0: 6428 3229 2e6f 626a 6563 7473 203d 3d20  d(2).objects == 
-00027cd0: 5b5d 290a 0a20 2020 2064 6566 2074 6573  [])..    def tes
-00027ce0: 7443 7574 4561 6368 2873 656c 6629 3a0a  tCutEach(self):.
-00027cf0: 0a20 2020 2020 2020 2023 2062 6173 6520  .        # base 
-00027d00: 7368 6170 653a 0a20 2020 2020 2020 2077  shape:.        w
-00027d10: 203d 2057 6f72 6b70 6c61 6e65 2829 2e62   = Workplane().b
-00027d20: 6f78 2833 2c20 322c 2032 290a 2020 2020  ox(3, 2, 2).    
-00027d30: 2020 2020 2320 6375 7474 6572 3a0a 2020      # cutter:.  
-00027d40: 2020 2020 2020 6320 3d20 576f 726b 706c        c = Workpl
-00027d50: 616e 6528 292e 626f 7828 322c 2032 2c20  ane().box(2, 2, 
-00027d60: 3229 2e76 616c 2829 0a20 2020 2020 2020  2).val().       
-00027d70: 2023 2063 7574 2061 6c6c 2074 6865 2063   # cut all the c
-00027d80: 6f72 6e65 7273 206f 6666 0a20 2020 2020  orners off.     
-00027d90: 2020 2077 3020 3d20 772e 7665 7274 6963     w0 = w.vertic
-00027da0: 6573 2829 2e63 7574 4561 6368 286c 616d  es().cutEach(lam
-00027db0: 6264 6120 6c6f 633a 2063 2e6c 6f63 6174  bda loc: c.locat
-00027dc0: 6564 286c 6f63 2929 0a20 2020 2020 2020  ed(loc)).       
-00027dd0: 2023 2077 6520 6172 6520 6c65 6674 2077   # we are left w
-00027de0: 6974 6820 6120 3178 3278 3220 626f 783a  ith a 1x2x2 box:
-00027df0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00027e00: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
-00027e10: 7730 2e76 616c 2829 2e56 6f6c 756d 6528  w0.val().Volume(
-00027e20: 292c 2034 2c20 3329 0a0a 2020 2020 2020  ), 4, 3)..      
-00027e30: 2020 2320 7465 7374 2065 7272 6f72 206f    # test error o
-00027e40: 6e20 6e6f 2073 6f6c 6964 2066 6f75 6e64  n no solid found
-00027e50: 0a20 2020 2020 2020 2077 3120 3d20 576f  .        w1 = Wo
-00027e60: 726b 706c 616e 6528 292e 684c 696e 6528  rkplane().hLine(
-00027e70: 3129 2e76 4c69 6e65 2831 292e 636c 6f73  1).vLine(1).clos
-00027e80: 6528 290a 2020 2020 2020 2020 7769 7468  e().        with
-00027e90: 2072 6169 7365 7328 5661 6c75 6545 7272   raises(ValueErr
-00027ea0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00027eb0: 2077 312e 6375 7445 6163 6828 6c61 6d62   w1.cutEach(lamb
-00027ec0: 6461 206c 6f63 3a20 632e 6c6f 6361 7465  da loc: c.locate
-00027ed0: 6428 6c6f 6329 290a 0a20 2020 2064 6566  d(loc))..    def
-00027ee0: 2074 6573 7443 7574 426c 696e 6428 7365   testCutBlind(se
-00027ef0: 6c66 293a 0a20 2020 2020 2020 2023 2063  lf):.        # c
-00027f00: 7574 426c 696e 6420 6973 2061 6c72 6561  utBlind is alrea
-00027f10: 6479 2074 6573 7465 6420 696e 2073 6576  dy tested in sev
-00027f20: 6572 616c 206f 6620 7468 6520 636f 6d70  eral of the comp
-00027f30: 6c69 6361 7465 6420 7465 7374 732c 2073  licated tests, s
-00027f40: 6f20 7468 6973 206d 6574 686f 6420 6973  o this method is
-00027f50: 2073 686f 7274 2e0a 2020 2020 2020 2020   short..        
-00027f60: 2320 7465 7374 2056 616c 7565 4572 726f  # test ValueErro
-00027f70: 7220 6f6e 206e 6f20 736f 6c69 6420 666f  r on no solid fo
-00027f80: 756e 640a 2020 2020 2020 2020 7730 203d  und.        w0 =
-00027f90: 2057 6f72 6b70 6c61 6e65 2829 2e68 4c69   Workplane().hLi
-00027fa0: 6e65 2831 292e 764c 696e 6528 3129 2e63  ne(1).vLine(1).c
-00027fb0: 6c6f 7365 2829 0a20 2020 2020 2020 2077  lose().        w
-00027fc0: 6974 6820 7261 6973 6573 2856 616c 7565  ith raises(Value
-00027fd0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00027fe0: 2020 2020 7730 2e63 7574 426c 696e 6428      w0.cutBlind(
-00027ff0: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
-00028000: 4669 6e64 4661 6365 2873 656c 6629 3a0a  FindFace(self):.
-00028010: 2020 2020 2020 2020 2320 6966 2074 6865          # if the
-00028020: 7265 2061 7265 206e 6f20 6661 6365 7320  re are no faces 
-00028030: 746f 2066 696e 642c 2073 686f 756c 6420  to find, should 
-00028040: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00028050: 0a20 2020 2020 2020 2077 3020 3d20 576f  .        w0 = Wo
-00028060: 726b 706c 616e 6528 290a 2020 2020 2020  rkplane().      
-00028070: 2020 7769 7468 2072 6169 7365 7328 5661    with raises(Va
-00028080: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
-00028090: 2020 2020 2020 2077 302e 6669 6e64 4661         w0.findFa
-000280a0: 6365 2829 0a0a 2020 2020 2020 2020 7731  ce()..        w1
-000280b0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e62   = Workplane().b
-000280c0: 6f78 2831 2c20 312c 2031 292e 6661 6365  ox(1, 1, 1).face
-000280d0: 7328 223e 5a22 290a 2020 2020 2020 2020  s(">Z").        
-000280e0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000280f0: 6973 696e 7374 616e 6365 2877 312e 6669  isinstance(w1.fi
-00028100: 6e64 4661 6365 2829 2c20 4661 6365 2929  ndFace(), Face))
-00028110: 0a20 2020 2020 2020 2077 6974 6820 7261  .        with ra
-00028120: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
-00028130: 3a0a 2020 2020 2020 2020 2020 2020 7731  :.            w1
-00028140: 2e66 696e 6446 6163 6528 7365 6172 6368  .findFace(search
-00028150: 5374 6163 6b3d 4661 6c73 6529 0a0a 2020  Stack=False)..  
-00028160: 2020 2020 2020 7732 203d 2077 312e 776f        w2 = w1.wo
-00028170: 726b 706c 616e 6528 292e 6369 7263 6c65  rkplane().circle
-00028180: 2830 2e31 292e 6578 7472 7564 6528 302e  (0.1).extrude(0.
-00028190: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000281a0: 6173 7365 7274 5472 7565 2869 7369 6e73  assertTrue(isins
-000281b0: 7461 6e63 6528 7732 2e66 696e 6446 6163  tance(w2.findFac
-000281c0: 6528 7365 6172 6368 5061 7265 6e74 733d  e(searchParents=
-000281d0: 5472 7565 292c 2046 6163 6529 290a 2020  True), Face)).  
-000281e0: 2020 2020 2020 7769 7468 2072 6169 7365        with raise
-000281f0: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
-00028200: 2020 2020 2020 2020 2020 2077 322e 6669             w2.fi
-00028210: 6e64 4661 6365 2873 6561 7263 6850 6172  ndFace(searchPar
-00028220: 656e 7473 3d46 616c 7365 290a 0a20 2020  ents=False)..   
-00028230: 2064 6566 2074 6573 7450 6f70 5065 6e64   def testPopPend
-00028240: 696e 6728 7365 6c66 293a 0a20 2020 2020  ing(self):.     
-00028250: 2020 2023 2074 6573 7420 7065 6e64 696e     # test pendin
-00028260: 6720 6564 6765 730a 2020 2020 2020 2020  g edges.        
-00028270: 7730 203d 2057 6f72 6b70 6c61 6e65 2829  w0 = Workplane()
-00028280: 2e68 4c69 6e65 2831 290a 2020 2020 2020  .hLine(1).      
-00028290: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000282a0: 616c 286c 656e 2877 302e 6374 782e 7065  al(len(w0.ctx.pe
-000282b0: 6e64 696e 6745 6467 6573 292c 2031 290a  ndingEdges), 1).
-000282c0: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
-000282d0: 7730 2e63 7478 2e70 6f70 5065 6e64 696e  w0.ctx.popPendin
-000282e0: 6745 6467 6573 2829 0a20 2020 2020 2020  gEdges().       
-000282f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00028300: 6c28 6c65 6e28 6564 6765 7329 2c20 3129  l(len(edges), 1)
-00028310: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00028320: 7365 7274 4571 7561 6c28 6564 6765 735b  sertEqual(edges[
-00028330: 305d 2c20 7730 2e76 616c 2829 290a 2020  0], w0.val()).  
-00028340: 2020 2020 2020 2320 7065 6e64 696e 6720        # pending 
-00028350: 6564 6765 7320 7368 6f75 6c64 206e 6f77  edges should now
-00028360: 2062 6520 636c 6561 7265 640a 2020 2020   be cleared.    
-00028370: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00028380: 7175 616c 286c 656e 2877 302e 6374 782e  qual(len(w0.ctx.
-00028390: 7065 6e64 696e 6745 6467 6573 292c 2030  pendingEdges), 0
-000283a0: 290a 0a20 2020 2020 2020 2023 2074 6573  )..        # tes
-000283b0: 7420 7065 6e64 696e 6720 7769 7265 730a  t pending wires.
-000283c0: 2020 2020 2020 2020 7731 203d 2057 6f72          w1 = Wor
-000283d0: 6b70 6c61 6e65 2829 2e68 4c69 6e65 2831  kplane().hLine(1
-000283e0: 292e 764c 696e 6528 3129 2e63 6c6f 7365  ).vLine(1).close
-000283f0: 2829 0a20 2020 2020 2020 2077 6972 6520  ().        wire 
-00028400: 3d20 7731 2e76 616c 2829 0a20 2020 2020  = w1.val().     
-00028410: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00028420: 7561 6c28 7731 2e63 7478 2e70 656e 6469  ual(w1.ctx.pendi
-00028430: 6e67 5769 7265 735b 305d 2c20 7769 7265  ngWires[0], wire
-00028440: 290a 2020 2020 2020 2020 706f 705f 7065  ).        pop_pe
-00028450: 6e64 696e 675f 6f75 7470 7574 203d 2077  nding_output = w
-00028460: 312e 6374 782e 706f 7050 656e 6469 6e67  1.ctx.popPending
-00028470: 5769 7265 7328 290a 2020 2020 2020 2020  Wires().        
-00028480: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00028490: 2870 6f70 5f70 656e 6469 6e67 5f6f 7574  (pop_pending_out
-000284a0: 7075 745b 305d 2c20 7769 7265 290a 2020  put[0], wire).  
-000284b0: 2020 2020 2020 2320 7065 6e64 696e 6720        # pending 
-000284c0: 7769 7265 7320 7368 6f75 6c64 206e 6f77  wires should now
-000284d0: 2062 6520 636c 6561 7265 640a 2020 2020   be cleared.    
-000284e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000284f0: 7175 616c 286c 656e 2877 312e 6374 782e  qual(len(w1.ctx.
-00028500: 7065 6e64 696e 6757 6972 6573 292c 2030  pendingWires), 0
-00028510: 290a 0a20 2020 2020 2020 2023 2074 6573  )..        # tes
-00028520: 7420 6572 726f 7220 7768 656e 2065 6d70  t error when emp
-00028530: 7479 2070 656e 6469 6e67 2065 6467 6573  ty pending edges
-00028540: 0a20 2020 2020 2020 2077 3220 3d20 576f  .        w2 = Wo
-00028550: 726b 706c 616e 6528 290a 2020 2020 2020  rkplane().      
-00028560: 2020 2320 7468 6520 666f 6c6c 6f77 696e    # the followin
-00028570: 6720 3220 7368 6f75 6c64 206e 6f74 2072  g 2 should not r
-00028580: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-00028590: 6e0a 2020 2020 2020 2020 7732 2e63 7478  n.        w2.ctx
-000285a0: 2e70 6f70 5065 6e64 696e 6745 6467 6573  .popPendingEdges
-000285b0: 2865 7272 6f72 4f6e 456d 7074 793d 4661  (errorOnEmpty=Fa
-000285c0: 6c73 6529 0a20 2020 2020 2020 2077 322e  lse).        w2.
-000285d0: 6374 782e 706f 7050 656e 6469 6e67 5769  ctx.popPendingWi
-000285e0: 7265 7328 6572 726f 724f 6e45 6d70 7479  res(errorOnEmpty
-000285f0: 3d46 616c 7365 290a 0a20 2020 2020 2020  =False)..       
-00028600: 2023 2065 6d70 7479 2065 6467 6573 0a20   # empty edges. 
-00028610: 2020 2020 2020 2077 3320 3d20 576f 726b         w3 = Work
-00028620: 706c 616e 6528 292e 684c 696e 6528 3129  plane().hLine(1)
-00028630: 2e76 4c69 6e65 2831 292e 636c 6f73 6528  .vLine(1).close(
-00028640: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00028650: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00028660: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
-00028670: 2020 2020 2020 2020 2020 7733 2e63 7478            w3.ctx
-00028680: 2e70 6f70 5065 6e64 696e 6745 6467 6573  .popPendingEdges
-00028690: 2829 0a0a 2020 2020 2020 2020 2320 656d  ()..        # em
-000286a0: 7074 7920 7769 7265 730a 2020 2020 2020  pty wires.      
-000286b0: 2020 7734 203d 2057 6f72 6b70 6c61 6e65    w4 = Workplane
-000286c0: 2829 2e63 6972 636c 6528 3129 2e65 7874  ().circle(1).ext
-000286d0: 7275 6465 2831 290a 2020 2020 2020 2020  rude(1).        
-000286e0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-000286f0: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
+0001dcd0: 2020 2020 2020 2320 5465 7374 2065 7874        # Test ext
+0001dce0: 7275 6465 2077 6974 6820 626f 7468 3d54  rude with both=T
+0001dcf0: 7275 6520 616e 6420 636f 6d62 696e 653d  rue and combine=
+0001dd00: 2263 7574 220a 2020 2020 2020 2020 7770  "cut".        wp
+0001dd10: 5f72 6566 203d 2057 6f72 6b70 6c61 6e65  _ref = Workplane
+0001dd20: 2822 5859 2229 2e72 6563 7428 3430 2c20  ("XY").rect(40, 
+0001dd30: 3430 292e 6578 7472 7564 6528 3230 2c20  40).extrude(20, 
+0001dd40: 626f 7468 3d54 7275 6529 0a0a 2020 2020  both=True)..    
+0001dd50: 2020 2020 7770 5f72 6566 5f72 6567 756c      wp_ref_regul
+0001dd60: 6172 5f63 7574 203d 2028 0a20 2020 2020  ar_cut = (.     
+0001dd70: 2020 2020 2020 2077 705f 7265 662e 776f         wp_ref.wo
+0001dd80: 726b 706c 616e 6528 6f66 6673 6574 3d2d  rkplane(offset=-
+0001dd90: 3230 292e 7265 6374 2832 302c 2032 3029  20).rect(20, 20)
+0001dda0: 2e65 7874 7275 6465 2834 302c 2063 6f6d  .extrude(40, com
+0001ddb0: 6269 6e65 3d22 7322 290a 2020 2020 2020  bine="s").      
+0001ddc0: 2020 290a 0a20 2020 2020 2020 2077 7020    )..        wp 
+0001ddd0: 3d20 7770 5f72 6566 2e77 6f72 6b70 6c61  = wp_ref.workpla
+0001dde0: 6e65 2829 2e72 6563 7428 3230 2c20 3230  ne().rect(20, 20
+0001ddf0: 292e 6578 7472 7564 6528 3230 2c20 626f  ).extrude(20, bo
+0001de00: 7468 3d54 7275 652c 2063 6f6d 6269 6e65  th=True, combine
+0001de10: 3d22 7322 290a 0a20 2020 2020 2020 2061  ="s")..        a
+0001de20: 7373 6572 7420 7770 2e66 6163 6573 2829  ssert wp.faces()
+0001de30: 2e73 697a 6528 2920 3d3d 2036 202b 2034  .size() == 6 + 4
+0001de40: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001de50: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
+0001de60: 7770 5f72 6566 5f72 6567 756c 6172 5f63  wp_ref_regular_c
+0001de70: 7574 2e76 616c 2829 2e56 6f6c 756d 6528  ut.val().Volume(
+0001de80: 292c 2077 702e 7661 6c28 292e 566f 6c75  ), wp.val().Volu
+0001de90: 6d65 2829 290a 0a20 2020 2064 6566 2074  me())..    def t
+0001dea0: 6573 7454 6170 6572 6564 4578 7472 7564  estTaperedExtrud
+0001deb0: 6543 7574 426c 696e 6428 7365 6c66 293a  eCutBlind(self):
+0001dec0: 0a0a 2020 2020 2020 2020 6820 3d20 312e  ..        h = 1.
+0001ded0: 300a 2020 2020 2020 2020 7220 3d20 312e  0.        r = 1.
+0001dee0: 300a 2020 2020 2020 2020 7420 3d20 350a  0.        t = 5.
+0001def0: 0a20 2020 2020 2020 2023 2065 7874 7275  .        # extru
+0001df00: 6465 2077 6974 6820 6120 706f 7369 7469  de with a positi
+0001df10: 7665 2074 6170 6572 0a20 2020 2020 2020  ve taper.       
+0001df20: 2073 203d 2057 6f72 6b70 6c61 6e65 2822   s = Workplane("
+0001df30: 5859 2229 2e63 6972 636c 6528 7229 2e65  XY").circle(r).e
+0001df40: 7874 7275 6465 2868 2c20 7461 7065 723d  xtrude(h, taper=
+0001df50: 7429 0a0a 2020 2020 2020 2020 746f 705f  t)..        top_
+0001df60: 6661 6365 203d 2073 2e66 6163 6573 2822  face = s.faces("
+0001df70: 3e5a 2229 0a20 2020 2020 2020 2062 6f74  >Z").        bot
+0001df80: 746f 6d5f 6661 6365 203d 2073 2e66 6163  tom_face = s.fac
+0001df90: 6573 2822 3c5a 2229 0a0a 2020 2020 2020  es("<Z")..      
+0001dfa0: 2020 2320 746f 7020 616e 6420 626f 7474    # top and bott
+0001dfb0: 6f6d 2066 6163 6520 6172 6561 0a20 2020  om face area.   
+0001dfc0: 2020 2020 2064 656c 7461 203d 2074 6f70       delta = top
+0001dfd0: 5f66 6163 652e 7661 6c28 292e 4172 6561  _face.val().Area
+0001dfe0: 2829 202d 2062 6f74 746f 6d5f 6661 6365  () - bottom_face
+0001dff0: 2e76 616c 2829 2e41 7265 6128 290a 0a20  .val().Area().. 
+0001e000: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001e010: 7274 5472 7565 2864 656c 7461 203c 2030  rtTrue(delta < 0
+0001e020: 290a 0a20 2020 2020 2020 2023 2065 7874  )..        # ext
+0001e030: 7275 6465 2077 6974 6820 6120 6e65 6761  rude with a nega
+0001e040: 7469 7665 2074 6170 6572 0a20 2020 2020  tive taper.     
+0001e050: 2020 2073 203d 2057 6f72 6b70 6c61 6e65     s = Workplane
+0001e060: 2822 5859 2229 2e63 6972 636c 6528 7229  ("XY").circle(r)
+0001e070: 2e65 7874 7275 6465 2868 2c20 7461 7065  .extrude(h, tape
+0001e080: 723d 2d74 290a 0a20 2020 2020 2020 2074  r=-t)..        t
+0001e090: 6f70 5f66 6163 6520 3d20 732e 6661 6365  op_face = s.face
+0001e0a0: 7328 223e 5a22 290a 2020 2020 2020 2020  s(">Z").        
+0001e0b0: 626f 7474 6f6d 5f66 6163 6520 3d20 732e  bottom_face = s.
+0001e0c0: 6661 6365 7328 223c 5a22 290a 0a20 2020  faces("<Z")..   
+0001e0d0: 2020 2020 2023 2074 6f70 2061 6e64 2062       # top and b
+0001e0e0: 6f74 746f 6d20 6661 6365 2061 7265 610a  ottom face area.
+0001e0f0: 2020 2020 2020 2020 6465 6c74 6120 3d20          delta = 
+0001e100: 746f 705f 6661 6365 2e76 616c 2829 2e41  top_face.val().A
+0001e110: 7265 6128 2920 2d20 626f 7474 6f6d 5f66  rea() - bottom_f
+0001e120: 6163 652e 7661 6c28 292e 4172 6561 2829  ace.val().Area()
+0001e130: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+0001e140: 7373 6572 7454 7275 6528 6465 6c74 6120  ssertTrue(delta 
+0001e150: 3e20 3029 0a0a 2020 2020 2020 2020 2320  > 0)..        # 
+0001e160: 6375 7420 6120 7461 7065 7265 6420 686f  cut a tapered ho
+0001e170: 6c65 0a20 2020 2020 2020 2073 203d 2028  le.        s = (
+0001e180: 0a20 2020 2020 2020 2020 2020 2057 6f72  .            Wor
+0001e190: 6b70 6c61 6e65 2822 5859 2229 0a20 2020  kplane("XY").   
+0001e1a0: 2020 2020 2020 2020 202e 7265 6374 2832           .rect(2
+0001e1b0: 202a 2072 2c20 3220 2a20 7229 0a20 2020   * r, 2 * r).   
+0001e1c0: 2020 2020 2020 2020 202e 6578 7472 7564           .extrud
+0001e1d0: 6528 3220 2a20 6829 0a20 2020 2020 2020  e(2 * h).       
+0001e1e0: 2020 2020 202e 6661 6365 7328 223e 5a22       .faces(">Z"
+0001e1f0: 290a 2020 2020 2020 2020 2020 2020 2e77  ).            .w
+0001e200: 6f72 6b70 6c61 6e65 2829 0a20 2020 2020  orkplane().     
+0001e210: 2020 2020 2020 202e 7265 6374 2872 2c20         .rect(r, 
+0001e220: 7229 0a20 2020 2020 2020 2020 2020 202e  r).            .
+0001e230: 6375 7442 6c69 6e64 282d 682c 2074 6170  cutBlind(-h, tap
+0001e240: 6572 3d74 290a 2020 2020 2020 2020 290a  er=t).        ).
+0001e250: 0a20 2020 2020 2020 206d 6964 646c 655f  .        middle_
+0001e260: 6661 6365 203d 2073 2e66 6163 6573 2822  face = s.faces("
+0001e270: 3e5a 5b2d 325d 2229 0a0a 2020 2020 2020  >Z[-2]")..      
+0001e280: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0001e290: 6528 6d69 6464 6c65 5f66 6163 652e 7661  e(middle_face.va
+0001e2a0: 6c28 292e 4172 6561 2829 203c 2031 290a  l().Area() < 1).
+0001e2b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0001e2c0: 6c66 2e61 7373 6572 7457 6172 6e73 2844  lf.assertWarns(D
+0001e2d0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+0001e2e0: 6729 3a0a 2020 2020 2020 2020 2020 2020  g):.            
+0001e2f0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
+0001e300: 2020 2020 2020 576f 726b 706c 616e 6528        Workplane(
+0001e310: 2258 5922 290a 2020 2020 2020 2020 2020  "XY").          
+0001e320: 2020 2020 2020 2e72 6563 7428 3220 2a20        .rect(2 * 
+0001e330: 722c 2032 202a 2072 290a 2020 2020 2020  r, 2 * r).      
+0001e340: 2020 2020 2020 2020 2020 2e65 7874 7275            .extru
+0001e350: 6465 2832 202a 2068 290a 2020 2020 2020  de(2 * h).      
+0001e360: 2020 2020 2020 2020 2020 2e66 6163 6573            .faces
+0001e370: 2822 3e5a 2229 0a20 2020 2020 2020 2020  (">Z").         
+0001e380: 2020 2020 2020 202e 776f 726b 706c 616e         .workplan
+0001e390: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0001e3a0: 2020 2020 2e72 6563 7428 722c 2072 290a      .rect(r, r).
+0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3c0: 2e63 7574 426c 696e 6428 2d68 2c20 5472  .cutBlind(-h, Tr
+0001e3d0: 7565 2c20 666c 6f61 7428 7429 290a 2020  ue, float(t)).  
+0001e3e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0001e3f0: 2064 6566 2074 6573 7443 6c6f 7365 2873   def testClose(s
+0001e400: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+0001e410: 436c 6f73 6520 7769 7468 6f75 7420 656e  Close without en
+0001e420: 6450 6f69 6e74 2061 6e64 2073 7461 7274  dPoint and start
+0001e430: 506f 696e 7420 636f 696e 6369 6465 2e0a  Point coincide..
+0001e440: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001e450: 2061 2068 616c 662d 6369 7263 6c65 0a20   a half-circle. 
+0001e460: 2020 2020 2020 2061 203d 2057 6f72 6b70         a = Workp
+0001e470: 6c61 6e65 2850 6c61 6e65 2e58 5928 2929  lane(Plane.XY())
+0001e480: 2e73 6167 6974 7461 4172 6328 2831 302c  .sagittaArc((10,
+0001e490: 2030 292c 2032 292e 636c 6f73 6528 292e   0), 2).close().
+0001e4a0: 6578 7472 7564 6528 3229 0a0a 2020 2020  extrude(2)..    
+0001e4b0: 2020 2020 2320 436c 6f73 6520 7768 656e      # Close when
+0001e4c0: 2065 6e64 506f 696e 7420 616e 6420 7374   endPoint and st
+0001e4d0: 6172 7450 6f69 6e74 2063 6f69 6e63 6964  artPoint coincid
+0001e4e0: 652e 0a20 2020 2020 2020 2023 2043 7265  e..        # Cre
+0001e4f0: 6174 6520 6120 646f 7562 6c65 2068 616c  ate a double hal
+0001e500: 662d 6369 7263 6c65 0a20 2020 2020 2020  f-circle.       
+0001e510: 2062 203d 2028 0a20 2020 2020 2020 2020   b = (.         
+0001e520: 2020 2057 6f72 6b70 6c61 6e65 2850 6c61     Workplane(Pla
+0001e530: 6e65 2e58 5928 2929 0a20 2020 2020 2020  ne.XY()).       
+0001e540: 2020 2020 202e 7361 6769 7474 6141 7263       .sagittaArc
+0001e550: 2828 3130 2c20 3029 2c20 3229 0a20 2020  ((10, 0), 2).   
+0001e560: 2020 2020 2020 2020 202e 7361 6769 7474           .sagitt
+0001e570: 6141 7263 2828 302c 2030 292c 2032 290a  aArc((0, 0), 2).
+0001e580: 2020 2020 2020 2020 2020 2020 2e63 6c6f              .clo
+0001e590: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
+0001e5a0: 202e 6578 7472 7564 6528 3229 0a20 2020   .extrude(2).   
+0001e5b0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001e5c0: 2320 5468 6520 6220 7368 6170 6520 7368  # The b shape sh
+0001e5d0: 616c 6c20 6861 7665 2074 7769 6365 2074  all have twice t
+0001e5e0: 6865 2076 6f6c 756d 6520 6f66 2074 6865  he volume of the
+0001e5f0: 2061 2073 6861 7065 2e0a 2020 2020 2020   a shape..      
+0001e600: 2020 7365 6c66 2e61 7373 6572 7441 6c6d    self.assertAlm
+0001e610: 6f73 7445 7175 616c 2861 2e76 616c 2829  ostEqual(a.val()
+0001e620: 2e56 6f6c 756d 6528 2920 2a20 322e 302c  .Volume() * 2.0,
+0001e630: 2062 2e76 616c 2829 2e56 6f6c 756d 6528   b.val().Volume(
+0001e640: 2929 0a0a 2020 2020 2020 2020 2320 5465  ))..        # Te
+0001e650: 7374 6361 7365 2033 2066 726f 6d20 6973  stcase 3 from is
+0001e660: 7375 6520 2332 3338 0a20 2020 2020 2020  sue #238.       
+0001e670: 2074 6869 636b 6e65 7373 203d 2033 2e30   thickness = 3.0
+0001e680: 0a20 2020 2020 2020 206c 656e 6774 6820  .        length 
+0001e690: 3d20 3130 2e30 0a20 2020 2020 2020 2077  = 10.0.        w
+0001e6a0: 6964 7468 203d 2035 2e30 0a0a 2020 2020  idth = 5.0..    
+0001e6b0: 2020 2020 6f62 6a31 203d 2028 0a20 2020      obj1 = (.   
+0001e6c0: 2020 2020 2020 2020 2057 6f72 6b70 6c61           Workpla
+0001e6d0: 6e65 2822 5859 222c 206f 7269 6769 6e3d  ne("XY", origin=
+0001e6e0: 2830 2c20 302c 202d 7468 6963 6b6e 6573  (0, 0, -thicknes
+0001e6f0: 7320 2f20 3229 290a 2020 2020 2020 2020  s / 2)).        
+0001e700: 2020 2020 2e6d 6f76 6554 6f28 6c65 6e67      .moveTo(leng
+0001e710: 7468 202f 2032 2c20 3029 0a20 2020 2020  th / 2, 0).     
+0001e720: 2020 2020 2020 202e 7468 7265 6550 6f69         .threePoi
+0001e730: 6e74 4172 6328 2830 2c20 7769 6474 6820  ntArc((0, width 
+0001e740: 2f20 3229 2c20 282d 6c65 6e67 7468 202f  / 2), (-length /
+0001e750: 2032 2c20 3029 290a 2020 2020 2020 2020   2, 0)).        
+0001e760: 2020 2020 2e74 6872 6565 506f 696e 7441      .threePointA
+0001e770: 7263 2828 302c 202d 7769 6474 6820 2f20  rc((0, -width / 
+0001e780: 3229 2c20 286c 656e 6774 6820 2f20 322c  2), (length / 2,
+0001e790: 2030 2929 0a20 2020 2020 2020 2020 2020   0)).           
+0001e7a0: 202e 636c 6f73 6528 290a 2020 2020 2020   .close().      
+0001e7b0: 2020 2020 2020 2e65 7874 7275 6465 2874        .extrude(t
+0001e7c0: 6869 636b 6e65 7373 290a 2020 2020 2020  hickness).      
+0001e7d0: 2020 290a 0a20 2020 2020 2020 206f 735f    )..        os_
+0001e7e0: 7820 3d20 382e 3020 2023 204f 6666 7365  x = 8.0  # Offse
+0001e7f0: 7420 696e 2058 0a20 2020 2020 2020 206f  t in X.        o
+0001e800: 735f 7920 3d20 2d31 392e 3520 2023 204f  s_y = -19.5  # O
+0001e810: 6666 7365 7420 696e 2059 0a0a 2020 2020  ffset in Y..    
+0001e820: 2020 2020 6f62 6a32 203d 2028 0a20 2020      obj2 = (.   
+0001e830: 2020 2020 2020 2020 2057 6f72 6b70 6c61           Workpla
+0001e840: 6e65 2822 595a 222c 206f 7269 6769 6e3d  ne("YZ", origin=
+0001e850: 286f 735f 782c 206f 735f 792c 202d 7468  (os_x, os_y, -th
+0001e860: 6963 6b6e 6573 7320 2f20 3229 290a 2020  ickness / 2)).  
+0001e870: 2020 2020 2020 2020 2020 2e6d 6f76 6554            .moveT
+0001e880: 6f28 6f73 5f78 202b 206c 656e 6774 6820  o(os_x + length 
+0001e890: 2f20 322c 206f 735f 7929 0a20 2020 2020  / 2, os_y).     
+0001e8a0: 2020 2020 2020 202e 7361 6769 7474 6141         .sagittaA
+0001e8b0: 7263 2828 6f73 5f78 202d 206c 656e 6774  rc((os_x - lengt
+0001e8c0: 6820 2f20 322c 206f 735f 7929 2c20 7769  h / 2, os_y), wi
+0001e8d0: 6474 6820 2f20 3229 0a20 2020 2020 2020  dth / 2).       
+0001e8e0: 2020 2020 202e 7361 6769 7474 6141 7263       .sagittaArc
+0001e8f0: 2828 6f73 5f78 202b 206c 656e 6774 6820  ((os_x + length 
+0001e900: 2f20 322c 206f 735f 7929 2c20 7769 6474  / 2, os_y), widt
+0001e910: 6820 2f20 3229 0a20 2020 2020 2020 2020  h / 2).         
+0001e920: 2020 202e 636c 6f73 6528 290a 2020 2020     .close().    
+0001e930: 2020 2020 2020 2020 2e65 7874 7275 6465          .extrude
+0001e940: 2874 6869 636b 6e65 7373 290a 2020 2020  (thickness).    
+0001e950: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+0001e960: 2054 6865 206f 626a 3120 7368 6170 6520   The obj1 shape 
+0001e970: 7368 616c 6c20 6861 7665 2074 6865 2073  shall have the s
+0001e980: 616d 6520 766f 6c75 6d65 2061 7320 7468  ame volume as th
+0001e990: 6520 6f62 6a32 2073 6861 7065 2e0a 2020  e obj2 shape..  
+0001e9a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001e9b0: 7441 6c6d 6f73 7445 7175 616c 286f 626a  tAlmostEqual(obj
+0001e9c0: 312e 7661 6c28 292e 566f 6c75 6d65 2829  1.val().Volume()
+0001e9d0: 2c20 6f62 6a32 2e76 616c 2829 2e56 6f6c  , obj2.val().Vol
+0001e9e0: 756d 6528 2929 0a0a 2020 2020 6465 6620  ume())..    def 
+0001e9f0: 7465 7374 5465 7874 2873 656c 6629 3a0a  testText(self):.
+0001ea00: 2020 2020 2020 2020 676c 6f62 616c 2074          global t
+0001ea10: 6573 7464 6174 6144 6972 0a0a 2020 2020  estdataDir..    
+0001ea20: 2020 2020 626f 7820 3d20 576f 726b 706c      box = Workpl
+0001ea30: 616e 6528 2258 5922 292e 626f 7828 342c  ane("XY").box(4,
+0001ea40: 2034 2c20 302e 3529 0a0a 2020 2020 2020   4, 0.5)..      
+0001ea50: 2020 6f62 6a31 203d 2028 0a20 2020 2020    obj1 = (.     
+0001ea60: 2020 2020 2020 2062 6f78 2e66 6163 6573         box.faces
+0001ea70: 2822 3e5a 2229 0a20 2020 2020 2020 2020  (">Z").         
+0001ea80: 2020 202e 776f 726b 706c 616e 6528 290a     .workplane().
+0001ea90: 2020 2020 2020 2020 2020 2020 2e74 6578              .tex
+0001eaa0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0001eab0: 2020 2022 4351 2032 2e30 222c 0a20 2020     "CQ 2.0",.   
+0001eac0: 2020 2020 2020 2020 2020 2020 2030 2e35               0.5
+0001ead0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eae0: 2020 2d30 2e30 352c 0a20 2020 2020 2020    -0.05,.       
+0001eaf0: 2020 2020 2020 2020 2063 7574 3d54 7275           cut=Tru
+0001eb00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001eb10: 2020 2068 616c 6967 6e3d 226c 6566 7422     halign="left"
+0001eb20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eb30: 2020 7661 6c69 676e 3d22 626f 7474 6f6d    valign="bottom
+0001eb40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0001eb50: 2020 2066 6f6e 743d 2253 616e 7322 2c0a     font="Sans",.
+0001eb60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001eb70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001eb80: 2023 2063 6f6d 6269 6e65 6420 6f62 6a65   # combined obje
+0001eb90: 6374 2073 686f 756c 6420 6861 7665 2073  ct should have s
+0001eba0: 6d61 6c6c 6572 2076 6f6c 756d 650a 2020  maller volume.  
+0001ebb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001ebc0: 7447 7265 6174 6572 2862 6f78 2e76 616c  tGreater(box.val
+0001ebd0: 2829 2e56 6f6c 756d 6528 292c 206f 626a  ().Volume(), obj
+0001ebe0: 312e 7661 6c28 292e 566f 6c75 6d65 2829  1.val().Volume()
+0001ebf0: 290a 0a20 2020 2020 2020 206f 626a 3220  )..        obj2 
+0001ec00: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001ec10: 626f 782e 6661 6365 7328 223e 5a22 290a  box.faces(">Z").
+0001ec20: 2020 2020 2020 2020 2020 2020 2e77 6f72              .wor
+0001ec30: 6b70 6c61 6e65 2829 0a20 2020 2020 2020  kplane().       
+0001ec40: 2020 2020 202e 7465 7874 2822 4351 2032       .text("CQ 2
+0001ec50: 2e30 222c 2030 2e35 2c20 302e 3035 2c20  .0", 0.5, 0.05, 
+0001ec60: 6375 743d 4661 6c73 652c 2063 6f6d 6269  cut=False, combi
+0001ec70: 6e65 3d54 7275 652c 2066 6f6e 743d 2253  ne=True, font="S
+0001ec80: 616e 7322 290a 2020 2020 2020 2020 290a  ans").        ).
+0001ec90: 0a20 2020 2020 2020 2023 2063 6f6d 6269  .        # combi
+0001eca0: 6e65 6420 6f62 6a65 6374 2073 686f 756c  ned object shoul
+0001ecb0: 6420 6861 7665 2062 6967 6765 7220 766f  d have bigger vo
+0001ecc0: 6c75 6d65 0a20 2020 2020 2020 2073 656c  lume.        sel
+0001ecd0: 662e 6173 7365 7274 4c65 7373 2862 6f78  f.assertLess(box
+0001ece0: 2e76 616c 2829 2e56 6f6c 756d 6528 292c  .val().Volume(),
+0001ecf0: 206f 626a 322e 7661 6c28 292e 566f 6c75   obj2.val().Volu
+0001ed00: 6d65 2829 290a 0a20 2020 2020 2020 2023  me())..        #
+0001ed10: 2076 6572 6966 7920 7468 6174 2074 6865   verify that the
+0001ed20: 206e 756d 6265 7220 6f66 2074 6f70 2066   number of top f
+0001ed30: 6163 6573 2069 7320 636f 7272 6563 7420  aces is correct 
+0001ed40: 284e 423a 2074 6869 7320 6973 2066 6f6e  (NB: this is fon
+0001ed50: 7420 7370 6563 6966 6963 290a 2020 2020  t specific).    
+0001ed60: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001ed70: 7175 616c 286c 656e 286f 626a 322e 6661  qual(len(obj2.fa
+0001ed80: 6365 7328 223e 5a22 292e 7661 6c73 2829  ces(">Z").vals()
+0001ed90: 292c 2035 290a 0a20 2020 2020 2020 206f  ), 5)..        o
+0001eda0: 626a 3320 3d20 280a 2020 2020 2020 2020  bj3 = (.        
+0001edb0: 2020 2020 626f 782e 6661 6365 7328 223e      box.faces(">
+0001edc0: 5a22 290a 2020 2020 2020 2020 2020 2020  Z").            
+0001edd0: 2e77 6f72 6b70 6c61 6e65 2829 0a20 2020  .workplane().   
+0001ede0: 2020 2020 2020 2020 202e 7465 7874 280a           .text(.
+0001edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ee00: 2243 5120 322e 3022 2c0a 2020 2020 2020  "CQ 2.0",.      
+0001ee10: 2020 2020 2020 2020 2020 302e 352c 0a20            0.5,. 
+0001ee20: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0001ee30: 2e30 352c 0a20 2020 2020 2020 2020 2020  .05,.           
+0001ee40: 2020 2020 2063 7574 3d46 616c 7365 2c0a       cut=False,.
+0001ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ee60: 636f 6d62 696e 653d 4661 6c73 652c 0a20  combine=False,. 
+0001ee70: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0001ee80: 616c 6967 6e3d 2272 6967 6874 222c 0a20  align="right",. 
+0001ee90: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0001eea0: 616c 6967 6e3d 2274 6f70 222c 0a20 2020  align="top",.   
+0001eeb0: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+0001eec0: 743d 2253 616e 7322 2c0a 2020 2020 2020  t="Sans",.      
+0001eed0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001eee0: 290a 0a20 2020 2020 2020 2023 2076 6572  )..        # ver
+0001eef0: 6966 7920 7468 6174 2074 6865 206e 756d  ify that the num
+0001ef00: 6265 7220 6f66 2073 6f6c 6964 7320 6973  ber of solids is
+0001ef10: 2063 6f72 7265 6374 0a20 2020 2020 2020   correct.       
+0001ef20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001ef30: 6c28 6c65 6e28 6f62 6a33 2e73 6f6c 6964  l(len(obj3.solid
+0001ef40: 7328 292e 7661 6c73 2829 292c 2035 290a  s().vals()), 5).
+0001ef50: 0a20 2020 2020 2020 206f 626a 3420 3d20  .        obj4 = 
+0001ef60: 280a 2020 2020 2020 2020 2020 2020 626f  (.            bo
+0001ef70: 782e 6661 6365 7328 223e 5a22 290a 2020  x.faces(">Z").  
+0001ef80: 2020 2020 2020 2020 2020 2e77 6f72 6b70            .workp
+0001ef90: 6c61 6e65 2829 0a20 2020 2020 2020 2020  lane().         
+0001efa0: 2020 202e 7465 7874 280a 2020 2020 2020     .text(.      
+0001efb0: 2020 2020 2020 2020 2020 2243 5120 322e            "CQ 2.
+0001efc0: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+0001efd0: 2020 2020 302e 352c 0a20 2020 2020 2020      0.5,.       
+0001efe0: 2020 2020 2020 2020 2030 2e30 352c 0a20           0.05,. 
+0001eff0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001f000: 6f6e 7450 6174 683d 6f73 2e70 6174 682e  ontPath=os.path.
+0001f010: 6a6f 696e 2874 6573 7464 6174 6144 6972  join(testdataDir
+0001f020: 2c20 224f 7065 6e53 616e 732d 5265 6775  , "OpenSans-Regu
+0001f030: 6c61 722e 7474 6622 292c 0a20 2020 2020  lar.ttf"),.     
+0001f040: 2020 2020 2020 2020 2020 2063 7574 3d46             cut=F
+0001f050: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+0001f060: 2020 2020 2020 636f 6d62 696e 653d 4661        combine=Fa
+0001f070: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0001f080: 2020 2020 2068 616c 6967 6e3d 2272 6967       halign="rig
+0001f090: 6874 222c 0a20 2020 2020 2020 2020 2020  ht",.           
+0001f0a0: 2020 2020 2076 616c 6967 6e3d 2274 6f70       valign="top
+0001f0b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0001f0c0: 2020 2066 6f6e 743d 2253 616e 7322 2c0a     font="Sans",.
+0001f0d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001f0e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001f0f0: 2023 2076 6572 6966 7920 7468 6174 2074   # verify that t
+0001f100: 6865 206e 756d 6265 7220 6f66 2073 6f6c  he number of sol
+0001f110: 6964 7320 6973 2063 6f72 7265 6374 0a20  ids is correct. 
+0001f120: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001f130: 7274 4571 7561 6c28 6c65 6e28 6f62 6a34  rtEqual(len(obj4
+0001f140: 2e73 6f6c 6964 7328 292e 7661 6c73 2829  .solids().vals()
+0001f150: 292c 2035 290a 0a20 2020 2020 2020 2023  ), 5)..        #
+0001f160: 2074 6573 7420 746f 2073 6565 2069 6620   test to see if 
+0001f170: 6e6f 6e2d 6578 6973 7465 6e74 2066 696c  non-existent fil
+0001f180: 6520 6361 7573 6573 2073 6567 6661 756c  e causes segfaul
+0001f190: 740a 2020 2020 2020 2020 6f62 6a35 203d  t.        obj5 =
+0001f1a0: 2028 0a20 2020 2020 2020 2020 2020 2062   (.            b
+0001f1b0: 6f78 2e66 6163 6573 2822 3e5a 2229 0a20  ox.faces(">Z"). 
+0001f1c0: 2020 2020 2020 2020 2020 202e 776f 726b             .work
+0001f1d0: 706c 616e 6528 290a 2020 2020 2020 2020  plane().        
+0001f1e0: 2020 2020 2e74 6578 7428 0a20 2020 2020      .text(.     
+0001f1f0: 2020 2020 2020 2020 2020 2022 4351 2032             "CQ 2
+0001f200: 2e30 222c 0a20 2020 2020 2020 2020 2020  .0",.           
+0001f210: 2020 2020 2030 2e35 2c0a 2020 2020 2020       0.5,.      
+0001f220: 2020 2020 2020 2020 2020 302e 3035 2c0a            0.05,.
+0001f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f240: 666f 6e74 5061 7468 3d6f 732e 7061 7468  fontPath=os.path
+0001f250: 2e6a 6f69 6e28 7465 7374 6461 7461 4469  .join(testdataDi
+0001f260: 722c 2022 4f70 656e 5361 6e73 2d49 7272  r, "OpenSans-Irr
+0001f270: 6567 756c 6172 2e74 7466 2229 2c0a 2020  egular.ttf"),.  
+0001f280: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0001f290: 743d 4661 6c73 652c 0a20 2020 2020 2020  t=False,.       
+0001f2a0: 2020 2020 2020 2020 2063 6f6d 6269 6e65           combine
+0001f2b0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0001f2c0: 2020 2020 2020 2020 6861 6c69 676e 3d22          halign="
+0001f2d0: 7269 6768 7422 2c0a 2020 2020 2020 2020  right",.        
+0001f2e0: 2020 2020 2020 2020 7661 6c69 676e 3d22          valign="
+0001f2f0: 746f 7022 2c0a 2020 2020 2020 2020 2020  top",.          
+0001f300: 2020 2020 2020 666f 6e74 3d22 5361 6e73        font="Sans
+0001f310: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+0001f320: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001f330: 2020 2020 2320 7665 7269 6679 2074 6861      # verify tha
+0001f340: 7420 7468 6520 6e75 6d62 6572 206f 6620  t the number of 
+0001f350: 736f 6c69 6473 2069 7320 636f 7272 6563  solids is correc
+0001f360: 740a 2020 2020 2020 2020 7365 6c66 2e61  t.        self.a
+0001f370: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+0001f380: 626a 352e 736f 6c69 6473 2829 2e76 616c  bj5.solids().val
+0001f390: 7328 2929 2c20 3529 0a0a 2020 2020 2020  s()), 5)..      
+0001f3a0: 2020 2320 6368 6563 6b20 6974 2064 6f65    # check it doe
+0001f3b0: 736e 2774 2066 616c 6c20 6f76 6572 2077  sn't fall over w
+0001f3c0: 6974 6820 696e 7420 7369 7a65 730a 2020  ith int sizes.  
+0001f3d0: 2020 2020 2020 6f62 6a31 203d 2028 0a20        obj1 = (. 
+0001f3e0: 2020 2020 2020 2020 2020 2062 6f78 2e66             box.f
+0001f3f0: 6163 6573 2822 3e5a 2229 0a20 2020 2020  aces(">Z").     
+0001f400: 2020 2020 2020 202e 776f 726b 706c 616e         .workplan
+0001f410: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0001f420: 2e74 6578 7428 0a20 2020 2020 2020 2020  .text(.         
+0001f430: 2020 2020 2020 2022 4351 2032 2e30 222c         "CQ 2.0",
+0001f440: 2031 302c 202d 312c 2063 7574 3d54 7275   10, -1, cut=Tru
+0001f450: 652c 2068 616c 6967 6e3d 226c 6566 7422  e, halign="left"
+0001f460: 2c20 7661 6c69 676e 3d22 626f 7474 6f6d  , valign="bottom
+0001f470: 222c 2066 6f6e 743d 2253 616e 7322 2c0a  ", font="Sans",.
+0001f480: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001f490: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0001f4a0: 2074 6573 7450 6172 616d 6574 7269 6343   testParametricC
+0001f4b0: 7572 7665 2873 656c 6629 3a0a 0a20 2020  urve(self):..   
+0001f4c0: 2020 2020 2066 726f 6d20 6d61 7468 2069       from math i
+0001f4d0: 6d70 6f72 7420 7369 6e2c 2063 6f73 2c20  mport sin, cos, 
+0001f4e0: 7069 0a0a 2020 2020 2020 2020 6b20 3d20  pi..        k = 
+0001f4f0: 340a 2020 2020 2020 2020 7220 3d20 310a  4.        r = 1.
+0001f500: 0a20 2020 2020 2020 2066 756e 6320 3d20  .        func = 
+0001f510: 6c61 6d62 6461 2074 3a20 280a 2020 2020  lambda t: (.    
+0001f520: 2020 2020 2020 2020 7220 2a20 286b 202b          r * (k +
+0001f530: 2031 2920 2a20 636f 7328 7429 202d 2072   1) * cos(t) - r
+0001f540: 202a 2063 6f73 2828 6b20 2b20 3129 202a   * cos((k + 1) *
+0001f550: 2074 292c 0a20 2020 2020 2020 2020 2020   t),.           
+0001f560: 2072 202a 2028 6b20 2b20 3129 202a 2073   r * (k + 1) * s
+0001f570: 696e 2874 2920 2d20 7220 2a20 7369 6e28  in(t) - r * sin(
+0001f580: 286b 202b 2031 2920 2a20 7429 2c0a 2020  (k + 1) * t),.  
+0001f590: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001f5a0: 2072 6573 5f6f 7065 6e20 3d20 576f 726b   res_open = Work
+0001f5b0: 706c 616e 6528 2258 5922 292e 7061 7261  plane("XY").para
+0001f5c0: 6d65 7472 6963 4375 7276 6528 6675 6e63  metricCurve(func
+0001f5d0: 292e 6578 7472 7564 6528 3329 0a0a 2020  ).extrude(3)..  
+0001f5e0: 2020 2020 2020 2320 6f70 656e 2070 726f        # open pro
+0001f5f0: 6669 6c65 2067 656e 6572 6174 6573 2061  file generates a
+0001f600: 6e20 696e 7661 6c69 6420 736f 6c69 640a  n invalid solid.
+0001f610: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001f620: 6572 7446 616c 7365 2872 6573 5f6f 7065  ertFalse(res_ope
+0001f630: 6e2e 736f 6c69 6473 2829 2e76 616c 2829  n.solids().val()
+0001f640: 2e69 7356 616c 6964 2829 290a 0a20 2020  .isValid())..   
+0001f650: 2020 2020 2072 6573 5f63 6c6f 7365 6420       res_closed 
+0001f660: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001f670: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
+0001f680: 7061 7261 6d65 7472 6963 4375 7276 6528  parametricCurve(
+0001f690: 6675 6e63 2c20 7374 6172 743d 302c 2073  func, start=0, s
+0001f6a0: 746f 703d 3220 2a20 7069 292e 6578 7472  top=2 * pi).extr
+0001f6b0: 7564 6528 3329 0a20 2020 2020 2020 2029  ude(3).        )
+0001f6c0: 0a0a 2020 2020 2020 2020 2320 636c 6f73  ..        # clos
+0001f6d0: 6564 2070 726f 6669 6c65 2077 696c 6c20  ed profile will 
+0001f6e0: 6765 6e65 7261 7465 2061 2076 616c 6964  generate a valid
+0001f6f0: 2073 6f6c 6964 2077 6974 6820 3320 6661   solid with 3 fa
+0001f700: 6365 730a 2020 2020 2020 2020 7365 6c66  ces.        self
+0001f710: 2e61 7373 6572 7454 7275 6528 7265 735f  .assertTrue(res_
+0001f720: 636c 6f73 6564 2e73 6f6c 6964 7328 292e  closed.solids().
+0001f730: 7661 6c28 292e 6973 5661 6c69 6428 2929  val().isValid())
+0001f740: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001f750: 7365 7274 4571 7561 6c28 6c65 6e28 7265  sertEqual(len(re
+0001f760: 735f 636c 6f73 6564 2e66 6163 6573 2829  s_closed.faces()
+0001f770: 2e76 616c 7328 2929 2c20 3329 0a0a 2020  .vals()), 3)..  
+0001f780: 2020 2020 2020 7265 735f 6564 6765 203d        res_edge =
+0001f790: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
+0001f7a0: 2e70 6172 616d 6574 7269 6343 7572 7665  .parametricCurve
+0001f7b0: 2866 756e 632c 206d 616b 6557 6972 653d  (func, makeWire=
+0001f7c0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0001f7d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001f7e0: 286c 656e 2872 6573 5f65 6467 652e 6374  (len(res_edge.ct
+0001f7f0: 782e 7065 6e64 696e 6745 6467 6573 292c  x.pendingEdges),
+0001f800: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+0001f810: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+0001f820: 2872 6573 5f65 6467 652e 6374 782e 7065  (res_edge.ctx.pe
+0001f830: 6e64 696e 6757 6972 6573 292c 2030 290a  ndingWires), 0).
+0001f840: 0a20 2020 2064 6566 2074 6573 744d 616b  .    def testMak
+0001f850: 6553 6865 6c6c 536f 6c69 6428 7365 6c66  eShellSolid(self
+0001f860: 293a 0a0a 2020 2020 2020 2020 6330 203d  ):..        c0 =
+0001f870: 206d 6174 682e 7371 7274 2832 2920 2f20   math.sqrt(2) / 
+0001f880: 340a 2020 2020 2020 2020 7665 7274 6963  4.        vertic
+0001f890: 6573 203d 205b 5b63 302c 202d 6330 2c20  es = [[c0, -c0, 
+0001f8a0: 6330 5d2c 205b 6330 2c20 6330 2c20 2d63  c0], [c0, c0, -c
+0001f8b0: 305d 2c20 5b2d 6330 2c20 6330 2c20 6330  0], [-c0, c0, c0
+0001f8c0: 5d2c 205b 2d63 302c 202d 6330 2c20 2d63  ], [-c0, -c0, -c
+0001f8d0: 305d 5d0a 2020 2020 2020 2020 6661 6365  0]].        face
+0001f8e0: 735f 6978 7320 3d20 5b5b 302c 2031 2c20  s_ixs = [[0, 1, 
+0001f8f0: 322c 2030 5d2c 205b 312c 2030 2c20 332c  2, 0], [1, 0, 3,
+0001f900: 2031 5d2c 205b 322c 2033 2c20 302c 2032   1], [2, 3, 0, 2
+0001f910: 5d2c 205b 332c 2032 2c20 312c 2033 5d5d  ], [3, 2, 1, 3]]
+0001f920: 0a0a 2020 2020 2020 2020 6661 6365 7320  ..        faces 
+0001f930: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0001f940: 2069 7873 2069 6e20 6661 6365 735f 6978   ixs in faces_ix
+0001f950: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+0001f960: 696e 6573 203d 205b 5d0a 2020 2020 2020  ines = [].      
+0001f970: 2020 2020 2020 666f 7220 7631 2c20 7632        for v1, v2
+0001f980: 2069 6e20 7a69 7028 6978 732c 2069 7873   in zip(ixs, ixs
+0001f990: 5b31 3a5d 293a 0a20 2020 2020 2020 2020  [1:]):.         
+0001f9a0: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
+0001f9b0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+0001f9c0: 2020 2020 2020 2020 2045 6467 652e 6d61           Edge.ma
+0001f9d0: 6b65 4c69 6e65 2856 6563 746f 7228 2a76  keLine(Vector(*v
+0001f9e0: 6572 7469 6365 735b 7631 5d29 2c20 5665  ertices[v1]), Ve
+0001f9f0: 6374 6f72 282a 7665 7274 6963 6573 5b76  ctor(*vertices[v
+0001fa00: 325d 2929 0a20 2020 2020 2020 2020 2020  2])).           
+0001fa10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0001fa20: 2020 2077 6972 6520 3d20 5769 7265 2e63     wire = Wire.c
+0001fa30: 6f6d 6269 6e65 286c 696e 6573 295b 305d  ombine(lines)[0]
+0001fa40: 0a20 2020 2020 2020 2020 2020 2066 6163  .            fac
+0001fa50: 6573 2e61 7070 656e 6428 4661 6365 2e6d  es.append(Face.m
+0001fa60: 616b 6546 726f 6d57 6972 6573 2877 6972  akeFromWires(wir
+0001fa70: 6529 290a 0a20 2020 2020 2020 2073 6865  e))..        she
+0001fa80: 6c6c 203d 2053 6865 6c6c 2e6d 616b 6553  ll = Shell.makeS
+0001fa90: 6865 6c6c 2866 6163 6573 290a 2020 2020  hell(faces).    
+0001faa0: 2020 2020 736f 6c69 6420 3d20 536f 6c69      solid = Soli
+0001fab0: 642e 6d61 6b65 536f 6c69 6428 7368 656c  d.makeSolid(shel
+0001fac0: 6c29 0a0a 2020 2020 2020 2020 7365 6c66  l)..        self
+0001fad0: 2e61 7373 6572 7454 7275 6528 7368 656c  .assertTrue(shel
+0001fae0: 6c2e 6973 5661 6c69 6428 2929 0a20 2020  l.isValid()).   
+0001faf0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001fb00: 5472 7565 2873 6f6c 6964 2e69 7356 616c  True(solid.isVal
+0001fb10: 6964 2829 290a 0a20 2020 2020 2020 2073  id())..        s
+0001fb20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001fb30: 6c65 6e28 736f 6c69 642e 5665 7274 6963  len(solid.Vertic
+0001fb40: 6573 2829 292c 2034 290a 2020 2020 2020  es()), 4).      
+0001fb50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001fb60: 616c 286c 656e 2873 6f6c 6964 2e46 6163  al(len(solid.Fac
+0001fb70: 6573 2829 292c 2034 290a 0a20 2020 2064  es()), 4)..    d
+0001fb80: 6566 2074 6573 7449 7349 6e73 6964 6553  ef testIsInsideS
+0001fb90: 6f6c 6964 2873 656c 6629 3a0a 2020 2020  olid(self):.    
+0001fba0: 2020 2020 2320 7465 7374 2073 6f6c 6964      # test solid
+0001fbb0: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
+0001fbc0: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
+0001fbd0: 2e62 6f78 2831 302c 2031 302c 2031 3029  .box(10, 10, 10)
+0001fbe0: 0a20 2020 2020 2020 2073 6f6c 6964 203d  .        solid =
+0001fbf0: 206d 6f64 656c 2e76 616c 2829 2020 2320   model.val()  # 
+0001fc00: 6765 7420 6669 7273 7420 6f62 6a65 6374  get first object
+0001fc10: 206f 6e20 7374 6163 6b0a 0a20 2020 2020   on stack..     
+0001fc20: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0001fc30: 7565 2873 6f6c 6964 2e69 7349 6e73 6964  ue(solid.isInsid
+0001fc40: 6528 2830 2c20 302c 2030 2929 290a 2020  e((0, 0, 0))).  
+0001fc50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001fc60: 7446 616c 7365 2873 6f6c 6964 2e69 7349  tFalse(solid.isI
+0001fc70: 6e73 6964 6528 2831 302c 2031 302c 2031  nside((10, 10, 1
+0001fc80: 3029 2929 0a20 2020 2020 2020 2073 656c  0))).        sel
+0001fc90: 662e 6173 7365 7274 5472 7565 2873 6f6c  f.assertTrue(sol
+0001fca0: 6964 2e69 7349 6e73 6964 6528 2856 6563  id.isInside((Vec
+0001fcb0: 746f 7228 332c 2033 2c20 3329 2929 290a  tor(3, 3, 3)))).
+0001fcc0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001fcd0: 6572 7446 616c 7365 2873 6f6c 6964 2e69  ertFalse(solid.i
+0001fce0: 7349 6e73 6964 6528 2856 6563 746f 7228  sInside((Vector(
+0001fcf0: 3330 2e30 2c20 3330 2e30 2c20 3330 2e30  30.0, 30.0, 30.0
+0001fd00: 2929 2929 0a0a 2020 2020 2020 2020 7365  ))))..        se
+0001fd10: 6c66 2e61 7373 6572 7454 7275 6528 736f  lf.assertTrue(so
+0001fd20: 6c69 642e 6973 496e 7369 6465 2828 302c  lid.isInside((0,
+0001fd30: 2030 2c20 342e 3939 292c 2074 6f6c 6572   0, 4.99), toler
+0001fd40: 616e 6365 3d30 2e31 2929 0a20 2020 2020  ance=0.1)).     
+0001fd50: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0001fd60: 7565 2873 6f6c 6964 2e69 7349 6e73 6964  ue(solid.isInsid
+0001fd70: 6528 2830 2c20 302c 2035 2929 2920 2023  e((0, 0, 5)))  #
+0001fd80: 2063 6865 636b 2070 6f69 6e74 206f 6e20   check point on 
+0001fd90: 7375 7266 6163 650a 2020 2020 2020 2020  surface.        
+0001fda0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+0001fdb0: 736f 6c69 642e 6973 496e 7369 6465 2828  solid.isInside((
+0001fdc0: 302c 2030 2c20 352e 3031 292c 2074 6f6c  0, 0, 5.01), tol
+0001fdd0: 6572 616e 6365 3d30 2e31 2929 0a20 2020  erance=0.1)).   
+0001fde0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001fdf0: 4661 6c73 6528 736f 6c69 642e 6973 496e  False(solid.isIn
+0001fe00: 7369 6465 2828 302c 2030 2c20 352e 3129  side((0, 0, 5.1)
+0001fe10: 2c20 746f 6c65 7261 6e63 653d 302e 3129  , tolerance=0.1)
+0001fe20: 290a 0a20 2020 2020 2020 2023 2074 6573  )..        # tes
+0001fe30: 7420 636f 6d70 6f75 6e64 2073 6f6c 6964  t compound solid
+0001fe40: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
+0001fe50: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
+0001fe60: 2e62 6f78 2831 302c 2031 302c 2031 3029  .box(10, 10, 10)
+0001fe70: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
+0001fe80: 206d 6f64 656c 2e6d 6f76 6554 6f28 3530   model.moveTo(50
+0001fe90: 2c20 3530 292e 626f 7828 3130 2c20 3130  , 50).box(10, 10
+0001fea0: 2c20 3130 290a 2020 2020 2020 2020 736f  , 10).        so
+0001feb0: 6c69 6420 3d20 6d6f 6465 6c2e 7661 6c28  lid = model.val(
+0001fec0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0001fed0: 6173 7365 7274 5472 7565 2873 6f6c 6964  assertTrue(solid
+0001fee0: 2e69 7349 6e73 6964 6528 2830 2c20 302c  .isInside((0, 0,
+0001fef0: 2030 2929 290a 2020 2020 2020 2020 7365   0))).        se
+0001ff00: 6c66 2e61 7373 6572 7454 7275 6528 736f  lf.assertTrue(so
+0001ff10: 6c69 642e 6973 496e 7369 6465 2828 3530  lid.isInside((50
+0001ff20: 2c20 3530 2c20 3029 2929 0a20 2020 2020  , 50, 0))).     
+0001ff30: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
+0001ff40: 6c73 6528 736f 6c69 642e 6973 496e 7369  lse(solid.isInsi
+0001ff50: 6465 2828 3530 2c20 3536 2c20 3029 2929  de((50, 56, 0)))
+0001ff60: 0a0a 2020 2020 2020 2020 2320 6d61 6b65  ..        # make
+0001ff70: 2073 7572 6520 7261 6973 6573 206f 6e20   sure raises on 
+0001ff80: 6e6f 6e20 736f 6c69 640a 2020 2020 2020  non solid.      
+0001ff90: 2020 6d6f 6465 6c20 3d20 576f 726b 706c    model = Workpl
+0001ffa0: 616e 6528 2258 5922 292e 7265 6374 2831  ane("XY").rect(1
+0001ffb0: 302c 2031 3029 0a20 2020 2020 2020 2073  0, 10).        s
+0001ffc0: 6f6c 6964 203d 206d 6f64 656c 2e76 616c  olid = model.val
+0001ffd0: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
+0001ffe0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+0001fff0: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
+00020000: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00020010: 6f6c 6964 2e69 7349 6e73 6964 6528 2830  olid.isInside((0
+00020020: 2c20 302c 2030 2929 0a0a 2020 2020 2020  , 0, 0))..      
+00020030: 2020 2320 7465 7374 2073 6f6c 6964 2077    # test solid w
+00020040: 6974 6820 616e 2069 6e74 6572 6e61 6c20  ith an internal 
+00020050: 766f 6964 0a20 2020 2020 2020 2076 6f69  void.        voi
+00020060: 6420 3d20 576f 726b 706c 616e 6528 2258  d = Workplane("X
+00020070: 5922 292e 626f 7828 3130 2c20 3130 2c20  Y").box(10, 10, 
+00020080: 3130 290a 2020 2020 2020 2020 6d6f 6465  10).        mode
+00020090: 6c20 3d20 576f 726b 706c 616e 6528 2258  l = Workplane("X
+000200a0: 5922 292e 626f 7828 3130 302c 2031 3030  Y").box(100, 100
+000200b0: 2c20 3130 3029 2e63 7574 2876 6f69 6429  , 100).cut(void)
+000200c0: 0a20 2020 2020 2020 2073 6f6c 6964 203d  .        solid =
+000200d0: 206d 6f64 656c 2e76 616c 2829 0a0a 2020   model.val()..  
+000200e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000200f0: 7446 616c 7365 2873 6f6c 6964 2e69 7349  tFalse(solid.isI
+00020100: 6e73 6964 6528 2830 2c20 302c 2030 2929  nside((0, 0, 0))
+00020110: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00020120: 7373 6572 7454 7275 6528 736f 6c69 642e  ssertTrue(solid.
+00020130: 6973 496e 7369 6465 2828 3430 2c20 3430  isInside((40, 40
+00020140: 2c20 3430 2929 290a 2020 2020 2020 2020  , 40))).        
+00020150: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00020160: 2873 6f6c 6964 2e69 7349 6e73 6964 6528  (solid.isInside(
+00020170: 2835 352c 2035 352c 2035 3529 2929 0a0a  (55, 55, 55)))..
+00020180: 2020 2020 6465 6620 7465 7374 576f 726b      def testWork
+00020190: 706c 616e 6543 656e 7465 724f 7074 696f  planeCenterOptio
+000201a0: 6e73 2873 656c 6629 3a0a 2020 2020 2020  ns(self):.      
+000201b0: 2020 2222 220a 2020 2020 2020 2020 5465    """.        Te
+000201c0: 7374 206f 7074 696f 6e73 2066 6f72 2073  st options for s
+000201d0: 7065 6369 6679 696e 6720 6f72 6967 696e  pecifying origin
+000201e0: 206f 6620 776f 726b 706c 616e 650a 2020   of workplane.  
+000201f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00020200: 2020 6465 6369 6d61 6c5f 706c 6163 6573    decimal_places
+00020210: 203d 2039 0a0a 2020 2020 2020 2020 7074   = 9..        pt
+00020220: 7320 3d20 5b28 302c 2030 292c 2028 3930  s = [(0, 0), (90
+00020230: 2c20 3029 2c20 2839 302c 2033 3029 2c20  , 0), (90, 30), 
+00020240: 2833 302c 2033 3029 2c20 2833 302c 2036  (30, 30), (30, 6
+00020250: 3029 2c20 2830 2e30 2c20 3630 295d 0a0a  0), (0.0, 60)]..
+00020260: 2020 2020 2020 2020 7220 3d20 576f 726b          r = Work
+00020270: 706c 616e 6528 2258 5922 292e 706f 6c79  plane("XY").poly
+00020280: 6c69 6e65 2870 7473 292e 636c 6f73 6528  line(pts).close(
+00020290: 292e 6578 7472 7564 6528 3130 2e30 290a  ).extrude(10.0).
+000202a0: 0a20 2020 2020 2020 206f 7269 6769 6e20  .        origin 
+000202b0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000202c0: 722e 6661 6365 7328 223e 5a22 290a 2020  r.faces(">Z").  
+000202d0: 2020 2020 2020 2020 2020 2e77 6f72 6b70            .workp
+000202e0: 6c61 6e65 2863 656e 7465 724f 7074 696f  lane(centerOptio
+000202f0: 6e3d 2250 726f 6a65 6374 6564 4f72 6967  n="ProjectedOrig
+00020300: 696e 2229 0a20 2020 2020 2020 2020 2020  in").           
+00020310: 202e 706c 616e 652e 6f72 6967 696e 2e74   .plane.origin.t
+00020320: 6f54 7570 6c65 2829 0a20 2020 2020 2020  oTuple().       
+00020330: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00020340: 6173 7365 7274 5475 706c 6541 6c6d 6f73  assertTupleAlmos
+00020350: 7445 7175 616c 7328 6f72 6967 696e 2c20  tEquals(origin, 
+00020360: 2830 2e30 2c20 302e 302c 2031 302e 3029  (0.0, 0.0, 10.0)
+00020370: 2c20 6465 6369 6d61 6c5f 706c 6163 6573  , decimal_places
+00020380: 290a 0a20 2020 2020 2020 206f 7269 6769  )..        origi
+00020390: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
+000203a0: 2020 722e 6661 6365 7328 223e 5a22 292e    r.faces(">Z").
+000203b0: 776f 726b 706c 616e 6528 6365 6e74 6572  workplane(center
+000203c0: 4f70 7469 6f6e 3d22 4365 6e74 6572 4f66  Option="CenterOf
+000203d0: 4d61 7373 2229 2e70 6c61 6e65 2e6f 7269  Mass").plane.ori
+000203e0: 6769 6e2e 746f 5475 706c 6528 290a 2020  gin.toTuple().  
+000203f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00020400: 7365 6c66 2e61 7373 6572 7454 7570 6c65  self.assertTuple
+00020410: 416c 6d6f 7374 4571 7561 6c73 286f 7269  AlmostEquals(ori
+00020420: 6769 6e2c 2028 3337 2e35 2c20 3232 2e35  gin, (37.5, 22.5
+00020430: 2c20 3130 2e30 292c 2064 6563 696d 616c  , 10.0), decimal
+00020440: 5f70 6c61 6365 7329 0a0a 2020 2020 2020  _places)..      
+00020450: 2020 6f72 6967 696e 203d 2028 0a20 2020    origin = (.   
+00020460: 2020 2020 2020 2020 2072 2e66 6163 6573           r.faces
+00020470: 2822 3e5a 2229 0a20 2020 2020 2020 2020  (">Z").         
+00020480: 2020 202e 776f 726b 706c 616e 6528 6365     .workplane(ce
+00020490: 6e74 6572 4f70 7469 6f6e 3d22 4365 6e74  nterOption="Cent
+000204a0: 6572 4f66 426f 756e 6442 6f78 2229 0a20  erOfBoundBox"). 
+000204b0: 2020 2020 2020 2020 2020 202e 706c 616e             .plan
+000204c0: 652e 6f72 6967 696e 2e74 6f54 7570 6c65  e.origin.toTuple
+000204d0: 2829 0a20 2020 2020 2020 2029 0a20 2020  ().        ).   
+000204e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000204f0: 5475 706c 6541 6c6d 6f73 7445 7175 616c  TupleAlmostEqual
+00020500: 7328 6f72 6967 696e 2c20 2834 352e 302c  s(origin, (45.0,
+00020510: 2033 302e 302c 2031 302e 3029 2c20 6465   30.0, 10.0), de
+00020520: 6369 6d61 6c5f 706c 6163 6573 290a 0a20  cimal_places).. 
+00020530: 2020 2020 2020 206f 7269 6769 6e20 3d20         origin = 
+00020540: 280a 2020 2020 2020 2020 2020 2020 722e  (.            r.
+00020550: 6661 6365 7328 223e 5a22 290a 2020 2020  faces(">Z").    
+00020560: 2020 2020 2020 2020 2e77 6f72 6b70 6c61          .workpla
+00020570: 6e65 2863 656e 7465 724f 7074 696f 6e3d  ne(centerOption=
+00020580: 2250 726f 6a65 6374 6564 4f72 6967 696e  "ProjectedOrigin
+00020590: 222c 206f 7269 6769 6e3d 2833 302c 2031  ", origin=(30, 1
+000205a0: 302c 2032 3029 290a 2020 2020 2020 2020  0, 20)).        
+000205b0: 2020 2020 2e70 6c61 6e65 2e6f 7269 6769      .plane.origi
+000205c0: 6e2e 746f 5475 706c 6528 290a 2020 2020  n.toTuple().    
+000205d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000205e0: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
+000205f0: 6d6f 7374 4571 7561 6c73 286f 7269 6769  mostEquals(origi
+00020600: 6e2c 2028 3330 2e30 2c20 3130 2e30 2c20  n, (30.0, 10.0, 
+00020610: 3130 2e30 292c 2064 6563 696d 616c 5f70  10.0), decimal_p
+00020620: 6c61 6365 7329 0a0a 2020 2020 2020 2020  laces)..        
+00020630: 6f72 6967 696e 203d 2028 0a20 2020 2020  origin = (.     
+00020640: 2020 2020 2020 2072 2e66 6163 6573 2822         r.faces("
+00020650: 3e5a 2229 0a20 2020 2020 2020 2020 2020  >Z").           
+00020660: 202e 776f 726b 706c 616e 6528 6365 6e74   .workplane(cent
+00020670: 6572 4f70 7469 6f6e 3d22 5072 6f6a 6563  erOption="Projec
+00020680: 7465 644f 7269 6769 6e22 2c20 6f72 6967  tedOrigin", orig
+00020690: 696e 3d56 6563 746f 7228 3330 2c20 3130  in=Vector(30, 10
+000206a0: 2c20 3230 2929 0a20 2020 2020 2020 2020  , 20)).         
+000206b0: 2020 202e 706c 616e 652e 6f72 6967 696e     .plane.origin
+000206c0: 2e74 6f54 7570 6c65 2829 0a20 2020 2020  .toTuple().     
+000206d0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+000206e0: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+000206f0: 6f73 7445 7175 616c 7328 6f72 6967 696e  ostEquals(origin
+00020700: 2c20 2833 302e 302c 2031 302e 302c 2031  , (30.0, 10.0, 1
+00020710: 302e 3029 2c20 6465 6369 6d61 6c5f 706c  0.0), decimal_pl
+00020720: 6163 6573 290a 0a20 2020 2020 2020 2077  aces)..        w
+00020730: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00020740: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
+00020750: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+00020760: 7269 6769 6e20 3d20 722e 6661 6365 7328  rigin = r.faces(
+00020770: 223e 5a22 292e 776f 726b 706c 616e 6528  ">Z").workplane(
+00020780: 6365 6e74 6572 4f70 7469 6f6e 3d22 756e  centerOption="un
+00020790: 6465 6669 6e65 6422 290a 0a20 2020 2020  defined")..     
+000207a0: 2020 2023 2074 6573 7420 6361 7365 2077     # test case w
+000207b0: 6865 7265 2070 6c61 6e65 206f 7269 6769  here plane origi
+000207c0: 6e20 6973 2073 6869 6674 6564 2077 6974  n is shifted wit
+000207d0: 6820 6365 6e74 6572 2063 616c 6c0a 2020  h center call.  
+000207e0: 2020 2020 2020 7220 3d20 280a 2020 2020        r = (.    
+000207f0: 2020 2020 2020 2020 722e 6661 6365 7328          r.faces(
+00020800: 223e 5a22 290a 2020 2020 2020 2020 2020  ">Z").          
+00020810: 2020 2e77 6f72 6b70 6c61 6e65 2863 656e    .workplane(cen
+00020820: 7465 724f 7074 696f 6e3d 2250 726f 6a65  terOption="Proje
+00020830: 6374 6564 4f72 6967 696e 2229 0a20 2020  ctedOrigin").   
+00020840: 2020 2020 2020 2020 202e 6365 6e74 6572           .center
+00020850: 2833 302c 2030 290a 2020 2020 2020 2020  (30, 0).        
+00020860: 2020 2020 2e68 6f6c 6528 3930 290a 2020      .hole(90).  
+00020870: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00020880: 206f 7269 6769 6e20 3d20 280a 2020 2020   origin = (.    
+00020890: 2020 2020 2020 2020 722e 6661 6365 7328          r.faces(
+000208a0: 223e 5a22 290a 2020 2020 2020 2020 2020  ">Z").          
+000208b0: 2020 2e77 6f72 6b70 6c61 6e65 2863 656e    .workplane(cen
+000208c0: 7465 724f 7074 696f 6e3d 2250 726f 6a65  terOption="Proje
+000208d0: 6374 6564 4f72 6967 696e 2229 0a20 2020  ctedOrigin").   
+000208e0: 2020 2020 2020 2020 202e 706c 616e 652e           .plane.
+000208f0: 6f72 6967 696e 2e74 6f54 7570 6c65 2829  origin.toTuple()
+00020900: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00020910: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
+00020920: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
+00020930: 6f72 6967 696e 2c20 2833 302e 302c 2030  origin, (30.0, 0
+00020940: 2e30 2c20 3130 2e30 292c 2064 6563 696d  .0, 10.0), decim
+00020950: 616c 5f70 6c61 6365 7329 0a0a 2020 2020  al_places)..    
+00020960: 2020 2020 6f72 6967 696e 203d 2028 0a20      origin = (. 
+00020970: 2020 2020 2020 2020 2020 2072 2e66 6163             r.fac
+00020980: 6573 2822 3e5a 2229 0a20 2020 2020 2020  es(">Z").       
+00020990: 2020 2020 202e 776f 726b 706c 616e 6528       .workplane(
+000209a0: 6365 6e74 6572 4f70 7469 6f6e 3d22 5072  centerOption="Pr
+000209b0: 6f6a 6563 7465 644f 7269 6769 6e22 2c20  ojectedOrigin", 
+000209c0: 6f72 6967 696e 3d28 302c 2030 2c20 3029  origin=(0, 0, 0)
+000209d0: 290a 2020 2020 2020 2020 2020 2020 2e70  ).            .p
+000209e0: 6c61 6e65 2e6f 7269 6769 6e2e 746f 5475  lane.origin.toTu
+000209f0: 706c 6528 290a 2020 2020 2020 2020 290a  ple().        ).
+00020a00: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00020a10: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
+00020a20: 7561 6c73 286f 7269 6769 6e2c 2028 302e  uals(origin, (0.
+00020a30: 302c 2030 2e30 2c20 3130 2e30 292c 2064  0, 0.0, 10.0), d
+00020a40: 6563 696d 616c 5f70 6c61 6365 7329 0a0a  ecimal_places)..
+00020a50: 2020 2020 2020 2020 2320 6d61 6b65 2073          # make s
+00020a60: 7572 6520 7072 6f6a 6563 7469 6f6e 2077  ure projection w
+00020a70: 6f72 6b73 2069 6e20 616c 6c20 6469 7265  orks in all dire
+00020a80: 6374 696f 6e73 0a20 2020 2020 2020 2072  ctions.        r
+00020a90: 203d 2057 6f72 6b70 6c61 6e65 2822 595a   = Workplane("YZ
+00020aa0: 2229 2e70 6f6c 796c 696e 6528 7074 7329  ").polyline(pts)
+00020ab0: 2e63 6c6f 7365 2829 2e65 7874 7275 6465  .close().extrude
+00020ac0: 2831 302e 3029 0a0a 2020 2020 2020 2020  (10.0)..        
+00020ad0: 6f72 6967 696e 203d 2028 0a20 2020 2020  origin = (.     
+00020ae0: 2020 2020 2020 2072 2e66 6163 6573 2822         r.faces("
+00020af0: 3e58 2229 0a20 2020 2020 2020 2020 2020  >X").           
+00020b00: 202e 776f 726b 706c 616e 6528 6365 6e74   .workplane(cent
+00020b10: 6572 4f70 7469 6f6e 3d22 5072 6f6a 6563  erOption="Projec
+00020b20: 7465 644f 7269 6769 6e22 290a 2020 2020  tedOrigin").    
+00020b30: 2020 2020 2020 2020 2e70 6c61 6e65 2e6f          .plane.o
+00020b40: 7269 6769 6e2e 746f 5475 706c 6528 290a  rigin.toTuple().
+00020b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00020b60: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
+00020b70: 6c65 416c 6d6f 7374 4571 7561 6c73 286f  leAlmostEquals(o
+00020b80: 7269 6769 6e2c 2028 3130 2e30 2c20 302e  rigin, (10.0, 0.
+00020b90: 302c 2030 2e30 292c 2064 6563 696d 616c  0, 0.0), decimal
+00020ba0: 5f70 6c61 6365 7329 0a0a 2020 2020 2020  _places)..      
+00020bb0: 2020 6f72 6967 696e 203d 2028 0a20 2020    origin = (.   
+00020bc0: 2020 2020 2020 2020 2072 2e66 6163 6573           r.faces
+00020bd0: 2822 3e58 2229 2e77 6f72 6b70 6c61 6e65  (">X").workplane
+00020be0: 2863 656e 7465 724f 7074 696f 6e3d 2243  (centerOption="C
+00020bf0: 656e 7465 724f 664d 6173 7322 292e 706c  enterOfMass").pl
+00020c00: 616e 652e 6f72 6967 696e 2e74 6f54 7570  ane.origin.toTup
+00020c10: 6c65 2829 0a20 2020 2020 2020 2029 0a20  le().        ). 
+00020c20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00020c30: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
+00020c40: 616c 7328 6f72 6967 696e 2c20 2831 302e  als(origin, (10.
+00020c50: 302c 2033 372e 352c 2032 322e 3529 2c20  0, 37.5, 22.5), 
+00020c60: 6465 6369 6d61 6c5f 706c 6163 6573 290a  decimal_places).
+00020c70: 0a20 2020 2020 2020 206f 7269 6769 6e20  .        origin 
+00020c80: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00020c90: 722e 6661 6365 7328 223e 5822 290a 2020  r.faces(">X").  
+00020ca0: 2020 2020 2020 2020 2020 2e77 6f72 6b70            .workp
+00020cb0: 6c61 6e65 2863 656e 7465 724f 7074 696f  lane(centerOptio
+00020cc0: 6e3d 2243 656e 7465 724f 6642 6f75 6e64  n="CenterOfBound
+00020cd0: 426f 7822 290a 2020 2020 2020 2020 2020  Box").          
+00020ce0: 2020 2e70 6c61 6e65 2e6f 7269 6769 6e2e    .plane.origin.
+00020cf0: 746f 5475 706c 6528 290a 2020 2020 2020  toTuple().      
+00020d00: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00020d10: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
+00020d20: 7374 4571 7561 6c73 286f 7269 6769 6e2c  stEquals(origin,
+00020d30: 2028 3130 2e30 2c20 3435 2e30 2c20 3330   (10.0, 45.0, 30
+00020d40: 2e30 292c 2064 6563 696d 616c 5f70 6c61  .0), decimal_pla
+00020d50: 6365 7329 0a0a 2020 2020 2020 2020 7220  ces)..        r 
+00020d60: 3d20 576f 726b 706c 616e 6528 2258 5a22  = Workplane("XZ"
+00020d70: 292e 706f 6c79 6c69 6e65 2870 7473 292e  ).polyline(pts).
+00020d80: 636c 6f73 6528 292e 6578 7472 7564 6528  close().extrude(
+00020d90: 3130 2e30 290a 0a20 2020 2020 2020 206f  10.0)..        o
+00020da0: 7269 6769 6e20 3d20 280a 2020 2020 2020  rigin = (.      
+00020db0: 2020 2020 2020 722e 6661 6365 7328 223c        r.faces("<
+00020dc0: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
+00020dd0: 2e77 6f72 6b70 6c61 6e65 2863 656e 7465  .workplane(cente
+00020de0: 724f 7074 696f 6e3d 2250 726f 6a65 6374  rOption="Project
+00020df0: 6564 4f72 6967 696e 2229 0a20 2020 2020  edOrigin").     
+00020e00: 2020 2020 2020 202e 706c 616e 652e 6f72         .plane.or
+00020e10: 6967 696e 2e74 6f54 7570 6c65 2829 0a20  igin.toTuple(). 
+00020e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00020e30: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
+00020e40: 6541 6c6d 6f73 7445 7175 616c 7328 6f72  eAlmostEquals(or
+00020e50: 6967 696e 2c20 2830 2e30 2c20 2d31 302e  igin, (0.0, -10.
+00020e60: 302c 2030 2e30 292c 2064 6563 696d 616c  0, 0.0), decimal
+00020e70: 5f70 6c61 6365 7329 0a0a 2020 2020 2020  _places)..      
+00020e80: 2020 6f72 6967 696e 203d 2028 0a20 2020    origin = (.   
+00020e90: 2020 2020 2020 2020 2072 2e66 6163 6573           r.faces
+00020ea0: 2822 3c59 2229 2e77 6f72 6b70 6c61 6e65  ("<Y").workplane
+00020eb0: 2863 656e 7465 724f 7074 696f 6e3d 2243  (centerOption="C
+00020ec0: 656e 7465 724f 664d 6173 7322 292e 706c  enterOfMass").pl
+00020ed0: 616e 652e 6f72 6967 696e 2e74 6f54 7570  ane.origin.toTup
+00020ee0: 6c65 2829 0a20 2020 2020 2020 2029 0a20  le().        ). 
+00020ef0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00020f00: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
+00020f10: 616c 7328 6f72 6967 696e 2c20 2833 372e  als(origin, (37.
+00020f20: 352c 202d 3130 2e30 2c20 3232 2e35 292c  5, -10.0, 22.5),
+00020f30: 2064 6563 696d 616c 5f70 6c61 6365 7329   decimal_places)
+00020f40: 0a0a 2020 2020 2020 2020 6f72 6967 696e  ..        origin
+00020f50: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00020f60: 2072 2e66 6163 6573 2822 3c59 2229 0a20   r.faces("<Y"). 
+00020f70: 2020 2020 2020 2020 2020 202e 776f 726b             .work
+00020f80: 706c 616e 6528 6365 6e74 6572 4f70 7469  plane(centerOpti
+00020f90: 6f6e 3d22 4365 6e74 6572 4f66 426f 756e  on="CenterOfBoun
+00020fa0: 6442 6f78 2229 0a20 2020 2020 2020 2020  dBox").         
+00020fb0: 2020 202e 706c 616e 652e 6f72 6967 696e     .plane.origin
+00020fc0: 2e74 6f54 7570 6c65 2829 0a20 2020 2020  .toTuple().     
+00020fd0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00020fe0: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+00020ff0: 6f73 7445 7175 616c 7328 6f72 6967 696e  ostEquals(origin
+00021000: 2c20 2834 352e 302c 202d 3130 2e30 2c20  , (45.0, -10.0, 
+00021010: 3330 2e30 292c 2064 6563 696d 616c 5f70  30.0), decimal_p
+00021020: 6c61 6365 7329 0a0a 2020 2020 6465 6620  laces)..    def 
+00021030: 7465 7374 4669 6e64 536f 6c69 6428 7365  testFindSolid(se
+00021040: 6c66 293a 0a0a 2020 2020 2020 2020 7220  lf):..        r 
+00021050: 3d20 576f 726b 706c 616e 6528 2258 5922  = Workplane("XY"
+00021060: 292e 7075 7368 506f 696e 7473 285b 282d  ).pushPoints([(-
+00021070: 322c 2030 292c 2028 322c 2030 295d 292e  2, 0), (2, 0)]).
+00021080: 626f 7828 312c 2031 2c20 312c 2063 6f6d  box(1, 1, 1, com
+00021090: 6269 6e65 3d46 616c 7365 290a 0a20 2020  bine=False)..   
+000210a0: 2020 2020 2023 2074 6865 7265 2073 686f       # there sho
+000210b0: 756c 6420 6265 2074 776f 2073 6f6c 6964  uld be two solid
+000210c0: 7320 6f6e 2074 6865 2073 7461 636b 0a20  s on the stack. 
+000210d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000210e0: 7274 4571 7561 6c28 6c65 6e28 722e 6f62  rtEqual(len(r.ob
+000210f0: 6a65 6374 7329 2c20 3229 0a20 2020 2020  jects), 2).     
+00021100: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00021110: 7565 2869 7369 6e73 7461 6e63 6528 722e  ue(isinstance(r.
+00021120: 7661 6c28 292c 2053 6f6c 6964 2929 0a0a  val(), Solid))..
+00021130: 2020 2020 2020 2020 2320 6669 6e64 2073          # find s
+00021140: 6f6c 6964 2073 686f 756c 6420 7265 7475  olid should retu
+00021150: 726e 2061 2063 6f6d 706f 756e 6420 6f66  rn a compound of
+00021160: 2074 776f 2073 6f6c 6964 730a 2020 2020   two solids.    
+00021170: 2020 2020 7320 3d20 722e 6669 6e64 536f      s = r.findSo
+00021180: 6c69 6428 290a 2020 2020 2020 2020 7365  lid().        se
+00021190: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+000211a0: 656e 2873 2e53 6f6c 6964 7328 2929 2c20  en(s.Solids()), 
+000211b0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+000211c0: 6173 7365 7274 5472 7565 2869 7369 6e73  assertTrue(isins
+000211d0: 7461 6e63 6528 732c 2043 6f6d 706f 756e  tance(s, Compoun
+000211e0: 6429 290a 0a20 2020 2020 2020 2023 2069  d))..        # i
+000211f0: 6620 6e6f 2073 6f6c 6964 7320 6172 6520  f no solids are 
+00021200: 666f 756e 642c 2073 686f 756c 6420 7261  found, should ra
+00021210: 6973 6520 5661 6c75 6545 7272 6f72 0a20  ise ValueError. 
+00021220: 2020 2020 2020 2077 203d 2057 6f72 6b70         w = Workp
+00021230: 6c61 6e65 2829 2e68 4c69 6e65 2831 292e  lane().hLine(1).
+00021240: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+00021250: 7769 7468 2072 6169 7365 7328 5661 6c75  with raises(Valu
+00021260: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+00021270: 2020 2020 2077 2e66 696e 6453 6f6c 6964       w.findSolid
+00021280: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
+00021290: 536c 6f74 3244 2873 656c 6629 3a0a 0a20  Slot2D(self):.. 
+000212a0: 2020 2020 2020 2064 6563 696d 616c 5f70         decimal_p
+000212b0: 6c61 6365 7320 3d20 390a 0a20 2020 2020  laces = 9..     
+000212c0: 2020 2023 2045 6e73 7572 6520 6974 2070     # Ensure it p
+000212d0: 726f 6475 6365 7320 6120 736f 6c69 6420  roduces a solid 
+000212e0: 7769 7468 2074 6865 2063 6f72 7265 6374  with the correct
+000212f0: 2076 6f6c 756d 650a 2020 2020 2020 2020   volume.        
+00021300: 7265 7375 6c74 203d 2057 6f72 6b70 6c61  result = Workpla
+00021310: 6e65 2822 5859 2229 2e73 6c6f 7432 4428  ne("XY").slot2D(
+00021320: 342c 2031 2c20 3029 2e65 7874 7275 6465  4, 1, 0).extrude
+00021330: 2831 290a 2020 2020 2020 2020 7365 6c66  (1).        self
+00021340: 2e61 7373 6572 7441 6c6d 6f73 7445 7175  .assertAlmostEqu
+00021350: 616c 2872 6573 756c 742e 7661 6c28 292e  al(result.val().
+00021360: 566f 6c75 6d65 2829 2c20 332e 3738 3533  Volume(), 3.7853
+00021370: 3938 3136 332c 2064 6563 696d 616c 5f70  98163, decimal_p
+00021380: 6c61 6365 7329 0a0a 2020 2020 2020 2020  laces)..        
+00021390: 2320 5465 7374 2066 6f72 2070 726f 7065  # Test for prope
+000213a0: 7220 6578 7065 6374 6564 2062 6568 6176  r expected behav
+000213b0: 696f 7572 2077 6865 6e20 6375 7474 696e  iour when cuttin
+000213c0: 670a 2020 2020 2020 2020 626f 7820 3d20  g.        box = 
+000213d0: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
+000213e0: 626f 7828 352c 2035 2c20 3129 0a20 2020  box(5, 5, 1).   
+000213f0: 2020 2020 2072 6573 756c 7420 3d20 626f       result = bo
+00021400: 782e 6661 6365 7328 223e 5a22 292e 776f  x.faces(">Z").wo
+00021410: 726b 706c 616e 6528 292e 736c 6f74 3244  rkplane().slot2D
+00021420: 2834 2c20 312c 2030 292e 6375 7454 6872  (4, 1, 0).cutThr
+00021430: 7541 6c6c 2829 0a20 2020 2020 2020 2073  uAll().        s
+00021440: 656c 662e 6173 7365 7274 416c 6d6f 7374  elf.assertAlmost
+00021450: 4571 7561 6c28 7265 7375 6c74 2e76 616c  Equal(result.val
+00021460: 2829 2e56 6f6c 756d 6528 292c 2032 312e  ().Volume(), 21.
+00021470: 3231 3436 3031 3833 372c 2064 6563 696d  214601837, decim
+00021480: 616c 5f70 6c61 6365 7329 0a20 2020 2020  al_places).     
+00021490: 2020 2072 6573 756c 7420 3d20 626f 782e     result = box.
+000214a0: 6661 6365 7328 223e 5a22 292e 776f 726b  faces(">Z").work
+000214b0: 706c 616e 6528 292e 736c 6f74 3244 2834  plane().slot2D(4
+000214c0: 2c20 312c 2030 292e 6375 7442 6c69 6e64  , 1, 0).cutBlind
+000214d0: 282d 302e 3529 0a20 2020 2020 2020 2073  (-0.5).        s
+000214e0: 656c 662e 6173 7365 7274 416c 6d6f 7374  elf.assertAlmost
+000214f0: 4571 7561 6c28 7265 7375 6c74 2e76 616c  Equal(result.val
+00021500: 2829 2e56 6f6c 756d 6528 292c 2032 332e  ().Volume(), 23.
+00021510: 3130 3733 3030 3931 382c 2064 6563 696d  107300918, decim
+00021520: 616c 5f70 6c61 6365 7329 0a0a 2020 2020  al_places)..    
+00021530: 2020 2020 2320 5465 7374 2074 6f20 7365      # Test to se
+00021540: 6520 6966 2073 6c6f 7420 6973 2072 6f74  e if slot is rot
+00021550: 6174 6564 2063 6f72 7265 6374 6c79 0a20  ated correctly. 
+00021560: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00021570: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
+00021580: 736c 6f74 3244 2834 2c20 312c 2034 3529  slot2D(4, 1, 45)
+00021590: 2e65 7874 7275 6465 2831 290a 2020 2020  .extrude(1).    
+000215a0: 2020 2020 706f 696e 7420 3d20 7265 7375      point = resu
+000215b0: 6c74 2e66 6163 6573 2822 3e5a 2229 2e65  lt.faces(">Z").e
+000215c0: 6467 6573 2822 3e58 2229 2e66 6972 7374  dges(">X").first
+000215d0: 2829 2e76 616c 2829 2e73 7461 7274 506f  ().val().startPo
+000215e0: 696e 7428 292e 746f 5475 706c 6528 290a  int().toTuple().
+000215f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00021600: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
+00021610: 7561 6c73 280a 2020 2020 2020 2020 2020  uals(.          
+00021620: 2020 706f 696e 742c 2028 302e 3730 3731    point, (0.7071
+00021630: 3036 3738 312c 2031 2e34 3134 3231 3335  06781, 1.4142135
+00021640: 3632 2c20 312e 3029 2c20 6465 6369 6d61  62, 1.0), decima
+00021650: 6c5f 706c 6163 6573 0a20 2020 2020 2020  l_places.       
+00021660: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
+00021670: 5f61 7373 656d 626c 6545 6467 6573 2873  _assembleEdges(s
+00021680: 656c 6629 3a0a 0a20 2020 2020 2020 2023  elf):..        #
+00021690: 2050 6c61 7465 2077 6974 6820 3520 7369   Plate with 5 si
+000216a0: 6465 7320 616e 6420 3220 6275 6d70 732c  des and 2 bumps,
+000216b0: 206f 6e65 2073 6964 6520 6973 206e 6f74   one side is not
+000216c0: 2063 6f2d 706c 616e 6172 2077 6974 6820   co-planar with 
+000216d0: 7468 6520 6f74 6865 7220 7369 6465 730a  the other sides.
+000216e0: 2020 2020 2020 2020 2320 5061 7373 6573          # Passes
+000216f0: 2061 6e20 6f70 656e 2077 6972 6520 746f   an open wire to
+00021700: 2061 7373 656d 626c 6545 6467 6573 2073   assembleEdges s
+00021710: 6f20 7468 6174 2049 7344 6f6e 6520 6973  o that IsDone is
+00021720: 2074 7275 6520 6275 7420 4572 726f 7220   true but Error 
+00021730: 7265 7475 726e 7320 3220 746f 2074 6573  returns 2 to tes
+00021740: 7420 7468 6520 7761 726e 696e 6720 6675  t the warning fu
+00021750: 6e63 7469 6f6e 616c 6974 792e 0a20 2020  nctionality..   
+00021760: 2020 2020 2065 6467 655f 706f 696e 7473       edge_points
+00021770: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00021780: 205b 2d37 2e30 2c20 2d37 2e30 2c20 302e   [-7.0, -7.0, 0.
+00021790: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+000217a0: 5b2d 332e 302c 202d 3130 2e30 2c20 332e  [-3.0, -10.0, 3.
+000217b0: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+000217c0: 5b37 2e30 2c20 2d37 2e30 2c20 302e 305d  [7.0, -7.0, 0.0]
+000217d0: 2c0a 2020 2020 2020 2020 2020 2020 5b37  ,.            [7
+000217e0: 2e30 2c20 372e 302c 2030 2e30 5d2c 0a20  .0, 7.0, 0.0],. 
+000217f0: 2020 2020 2020 2020 2020 205b 2d37 2e30             [-7.0
+00021800: 2c20 372e 302c 2030 2e30 5d2c 0a20 2020  , 7.0, 0.0],.   
+00021810: 2020 2020 205d 0a20 2020 2020 2020 2065       ].        e
+00021820: 6467 655f 7769 7265 203d 2057 6f72 6b70  dge_wire = Workp
+00021830: 6c61 6e65 2822 5859 2229 2e70 6f6c 796c  lane("XY").polyl
+00021840: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
+00021850: 205b 282d 372e 302c 202d 372e 3029 2c20   [(-7.0, -7.0), 
+00021860: 2837 2e30 2c20 2d37 2e30 292c 2028 372e  (7.0, -7.0), (7.
+00021870: 302c 2037 2e30 292c 2028 2d37 2e30 2c20  0, 7.0), (-7.0, 
+00021880: 372e 3029 5d0a 2020 2020 2020 2020 290a  7.0)].        ).
+00021890: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
+000218a0: 6520 3d20 6564 6765 5f77 6972 652e 6164  e = edge_wire.ad
+000218b0: 6428 0a20 2020 2020 2020 2020 2020 2057  d(.            W
+000218c0: 6f72 6b70 6c61 6e65 2822 595a 2229 0a20  orkplane("YZ"). 
+000218d0: 2020 2020 2020 2020 2020 202e 776f 726b             .work
+000218e0: 706c 616e 6528 290a 2020 2020 2020 2020  plane().        
+000218f0: 2020 2020 2e74 7261 6e73 666f 726d 6564      .transformed
+00021900: 286f 6666 7365 743d 5665 6374 6f72 2830  (offset=Vector(0
+00021910: 2c20 302c 202d 3729 2c20 726f 7461 7465  , 0, -7), rotate
+00021920: 3d56 6563 746f 7228 3435 2c20 302c 2030  =Vector(45, 0, 0
+00021930: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
+00021940: 7370 6c69 6e65 285b 282d 372e 302c 2030  spline([(-7.0, 0
+00021950: 2e30 292c 2028 332c 202d 3329 2c20 2837  .0), (3, -3), (7
+00021960: 2e30 2c20 302e 3029 5d29 0a20 2020 2020  .0, 0.0)]).     
+00021970: 2020 2029 0a20 2020 2020 2020 2065 6467     ).        edg
+00021980: 655f 7769 7265 203d 205b 6f2e 7661 6c73  e_wire = [o.vals
+00021990: 2829 5b30 5d20 666f 7220 6f20 696e 2065  ()[0] for o in e
+000219a0: 6467 655f 7769 7265 2e61 6c6c 2829 5d0a  dge_wire.all()].
+000219b0: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
+000219c0: 6520 3d20 5769 7265 2e61 7373 656d 626c  e = Wire.assembl
+000219d0: 6545 6467 6573 2865 6467 655f 7769 7265  eEdges(edge_wire
+000219e0: 290a 0a20 2020 2020 2020 2023 2045 6d62  )..        # Emb
+000219f0: 6f73 7365 6420 7374 6172 2c20 6e65 6564  ossed star, need
+00021a00: 2074 6f20 6368 616e 6765 206f 7074 696f   to change optio
+00021a10: 6e61 6c20 7061 7261 6d65 7465 7273 2074  nal parameters t
+00021a20: 6f20 6f62 7461 696e 206e 6963 6520 6c6f  o obtain nice lo
+00021a30: 6f6b 696e 6720 7265 7375 6c74 2e0a 2020  oking result..  
+00021a40: 2020 2020 2020 7231 203d 2033 2e30 0a20        r1 = 3.0. 
+00021a50: 2020 2020 2020 2072 3220 3d20 3130 2e30         r2 = 10.0
+00021a60: 0a20 2020 2020 2020 2066 6e20 3d20 360a  .        fn = 6.
+00021a70: 2020 2020 2020 2020 6564 6765 5f70 6f69          edge_poi
+00021a80: 6e74 7320 3d20 5b0a 2020 2020 2020 2020  nts = [.        
+00021a90: 2020 2020 5b72 3120 2a20 6d61 7468 2e63      [r1 * math.c
+00021aa0: 6f73 2869 202a 206d 6174 682e 7069 202f  os(i * math.pi /
+00021ab0: 2066 6e29 2c20 7231 202a 206d 6174 682e   fn), r1 * math.
+00021ac0: 7369 6e28 6920 2a20 6d61 7468 2e70 6920  sin(i * math.pi 
+00021ad0: 2f20 666e 295d 0a20 2020 2020 2020 2020  / fn)].         
+00021ae0: 2020 2069 6620 6920 2520 3220 3d3d 2030     if i % 2 == 0
+00021af0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00021b00: 6520 5b72 3220 2a20 6d61 7468 2e63 6f73  e [r2 * math.cos
+00021b10: 2869 202a 206d 6174 682e 7069 202f 2066  (i * math.pi / f
+00021b20: 6e29 2c20 7232 202a 206d 6174 682e 7369  n), r2 * math.si
+00021b30: 6e28 6920 2a20 6d61 7468 2e70 6920 2f20  n(i * math.pi / 
+00021b40: 666e 295d 0a20 2020 2020 2020 2020 2020  fn)].           
+00021b50: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00021b60: 3220 2a20 666e 202b 2031 290a 2020 2020  2 * fn + 1).    
+00021b70: 2020 2020 5d0a 2020 2020 2020 2020 6564      ].        ed
+00021b80: 6765 5f77 6972 6520 3d20 576f 726b 706c  ge_wire = Workpl
+00021b90: 616e 6528 2258 5922 292e 706f 6c79 6c69  ane("XY").polyli
+00021ba0: 6e65 2865 6467 655f 706f 696e 7473 290a  ne(edge_points).
+00021bb0: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
+00021bc0: 6520 3d20 5b6f 2e76 616c 7328 295b 305d  e = [o.vals()[0]
+00021bd0: 2066 6f72 206f 2069 6e20 6564 6765 5f77   for o in edge_w
+00021be0: 6972 652e 616c 6c28 295d 0a20 2020 2020  ire.all()].     
+00021bf0: 2020 2065 6467 655f 7769 7265 203d 2057     edge_wire = W
+00021c00: 6972 652e 6173 7365 6d62 6c65 4564 6765  ire.assembleEdge
+00021c10: 7328 6564 6765 5f77 6972 6529 0a0a 2020  s(edge_wire)..  
+00021c20: 2020 2020 2020 2320 506f 696e 7473 206f        # Points o
+00021c30: 6e20 6865 7861 676f 6e61 6c20 7061 7474  n hexagonal patt
+00021c40: 6572 6e20 636f 6f72 6469 6e61 7465 732c  ern coordinates,
+00021c50: 2075 7365 206f 6620 7075 7368 706f 696e   use of pushpoin
+00021c60: 7473 2e0a 2020 2020 2020 2020 7231 203d  ts..        r1 =
+00021c70: 2031 2e30 0a20 2020 2020 2020 2066 6e20   1.0.        fn 
+00021c80: 3d20 360a 2020 2020 2020 2020 6564 6765  = 6.        edge
+00021c90: 5f70 6f69 6e74 7320 3d20 5b0a 2020 2020  _points = [.    
+00021ca0: 2020 2020 2020 2020 5b72 3120 2a20 6d61          [r1 * ma
+00021cb0: 7468 2e63 6f73 2869 202a 2032 202a 206d  th.cos(i * 2 * m
+00021cc0: 6174 682e 7069 202f 2066 6e29 2c20 7231  ath.pi / fn), r1
+00021cd0: 202a 206d 6174 682e 7369 6e28 6920 2a20   * math.sin(i * 
+00021ce0: 3220 2a20 6d61 7468 2e70 6920 2f20 666e  2 * math.pi / fn
+00021cf0: 295d 0a20 2020 2020 2020 2020 2020 2066  )].            f
+00021d00: 6f72 2069 2069 6e20 7261 6e67 6528 666e  or i in range(fn
+00021d10: 202b 2031 290a 2020 2020 2020 2020 5d0a   + 1).        ].
+00021d20: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
+00021d30: 706f 696e 7473 203d 205b 0a20 2020 2020  points = [.     
+00021d40: 2020 2020 2020 205b 302e 3235 2c20 302c         [0.25, 0,
+00021d50: 2030 2e37 355d 2c0a 2020 2020 2020 2020   0.75],.        
+00021d60: 2020 2020 5b2d 302e 3235 2c20 302c 2030      [-0.25, 0, 0
+00021d70: 2e37 355d 2c0a 2020 2020 2020 2020 2020  .75],.          
+00021d80: 2020 5b30 2c20 302e 3235 2c20 302e 3735    [0, 0.25, 0.75
+00021d90: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00021da0: 302c 202d 302e 3235 2c20 302e 3735 5d2c  0, -0.25, 0.75],
+00021db0: 0a20 2020 2020 2020 2020 2020 205b 302c  .            [0,
+00021dc0: 2030 2c20 325d 2c0a 2020 2020 2020 2020   0, 2],.        
+00021dd0: 5d0a 2020 2020 2020 2020 6564 6765 5f77  ].        edge_w
+00021de0: 6972 6520 3d20 576f 726b 706c 616e 6528  ire = Workplane(
+00021df0: 2258 5922 292e 706f 6c79 6c69 6e65 2865  "XY").polyline(e
+00021e00: 6467 655f 706f 696e 7473 290a 2020 2020  dge_points).    
+00021e10: 2020 2020 6564 6765 5f77 6972 6520 3d20      edge_wire = 
+00021e20: 5b6f 2e76 616c 7328 295b 305d 2066 6f72  [o.vals()[0] for
+00021e30: 206f 2069 6e20 6564 6765 5f77 6972 652e   o in edge_wire.
+00021e40: 616c 6c28 295d 0a20 2020 2020 2020 2065  all()].        e
+00021e50: 6467 655f 7769 7265 203d 2057 6972 652e  dge_wire = Wire.
+00021e60: 6173 7365 6d62 6c65 4564 6765 7328 6564  assembleEdges(ed
+00021e70: 6765 5f77 6972 6529 0a0a 2020 2020 2020  ge_wire)..      
+00021e80: 2020 2320 4779 726f c3af 642c 2061 6c6c    # Gyro..d, all
+00021e90: 2065 6467 6573 2061 7265 2073 706c 696e   edges are splin
+00021ea0: 6573 206f 6e20 6469 6666 6572 656e 7420  es on different 
+00021eb0: 776f 726b 706c 616e 6573 2e0a 2020 2020  workplanes..    
+00021ec0: 2020 2020 6564 6765 5f70 6f69 6e74 7320      edge_points 
+00021ed0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00021ee0: 5b5b 332e 3534 2c20 332e 3534 5d2c 205b  [[3.54, 3.54], [
+00021ef0: 312e 3737 2c20 302e 305d 2c20 5b33 2e35  1.77, 0.0], [3.5
+00021f00: 342c 202d 332e 3534 5d5d 2c0a 2020 2020  4, -3.54]],.    
+00021f10: 2020 2020 2020 2020 5b5b 2d33 2e35 342c          [[-3.54,
+00021f20: 202d 332e 3534 5d2c 205b 302e 302c 202d   -3.54], [0.0, -
+00021f30: 312e 3737 5d2c 205b 332e 3534 2c20 2d33  1.77], [3.54, -3
+00021f40: 2e35 345d 5d2c 0a20 2020 2020 2020 2020  .54]],.         
+00021f50: 2020 205b 5b2d 332e 3534 2c20 2d33 2e35     [[-3.54, -3.5
+00021f60: 345d 2c20 5b30 2e30 2c20 2d31 2e37 375d  4], [0.0, -1.77]
+00021f70: 2c20 5b33 2e35 342c 202d 332e 3534 5d5d  , [3.54, -3.54]]
+00021f80: 2c0a 2020 2020 2020 2020 2020 2020 5b5b  ,.            [[
+00021f90: 2d33 2e35 342c 202d 332e 3534 5d2c 205b  -3.54, -3.54], [
+00021fa0: 2d31 2e37 372c 2030 2e30 5d2c 205b 2d33  -1.77, 0.0], [-3
+00021fb0: 2e35 342c 2033 2e35 345d 5d2c 0a20 2020  .54, 3.54]],.   
+00021fc0: 2020 2020 2020 2020 205b 5b33 2e35 342c           [[3.54,
+00021fd0: 2033 2e35 345d 2c20 5b30 2e30 2c20 312e   3.54], [0.0, 1.
+00021fe0: 3737 5d2c 205b 2d33 2e35 342c 2033 2e35  77], [-3.54, 3.5
+00021ff0: 345d 5d2c 0a20 2020 2020 2020 2020 2020  4]],.           
+00022000: 205b 5b33 2e35 342c 2033 2e35 345d 2c20   [[3.54, 3.54], 
+00022010: 5b30 2e30 2c20 312e 3737 5d2c 205b 2d33  [0.0, 1.77], [-3
+00022020: 2e35 342c 2033 2e35 345d 5d2c 0a20 2020  .54, 3.54]],.   
+00022030: 2020 2020 205d 0a20 2020 2020 2020 2070       ].        p
+00022040: 6c61 6e65 5f6c 6973 7420 3d20 5b22 585a  lane_list = ["XZ
+00022050: 222c 2022 5859 222c 2022 595a 222c 2022  ", "XY", "YZ", "
+00022060: 585a 222c 2022 595a 222c 2022 5859 225d  XZ", "YZ", "XY"]
+00022070: 0a20 2020 2020 2020 206f 6666 7365 745f  .        offset_
+00022080: 6c69 7374 203d 205b 2d33 2e35 342c 2033  list = [-3.54, 3
+00022090: 2e35 342c 2033 2e35 342c 2033 2e35 342c  .54, 3.54, 3.54,
+000220a0: 202d 332e 3534 2c20 2d33 2e35 345d 0a20   -3.54, -3.54]. 
+000220b0: 2020 2020 2020 2065 6467 655f 7769 7265         edge_wire
+000220c0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000220d0: 2057 6f72 6b70 6c61 6e65 2870 6c61 6e65   Workplane(plane
+000220e0: 5f6c 6973 745b 305d 290a 2020 2020 2020  _list[0]).      
+000220f0: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
+00022100: 286f 6666 7365 743d 2d6f 6666 7365 745f  (offset=-offset_
+00022110: 6c69 7374 5b30 5d29 0a20 2020 2020 2020  list[0]).       
+00022120: 2020 2020 202e 7370 6c69 6e65 2865 6467       .spline(edg
+00022130: 655f 706f 696e 7473 5b30 5d29 0a20 2020  e_points[0]).   
+00022140: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
+00022150: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00022160: 6e28 6564 6765 5f70 6f69 6e74 7329 202d  n(edge_points) -
+00022170: 2031 293a 0a20 2020 2020 2020 2020 2020   1):.           
+00022180: 2065 6467 655f 7769 7265 203d 2065 6467   edge_wire = edg
+00022190: 655f 7769 7265 2e61 6464 280a 2020 2020  e_wire.add(.    
+000221a0: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+000221b0: 706c 616e 6528 706c 616e 655f 6c69 7374  plane(plane_list
+000221c0: 5b69 202b 2031 5d29 0a20 2020 2020 2020  [i + 1]).       
+000221d0: 2020 2020 2020 2020 202e 776f 726b 706c           .workpl
+000221e0: 616e 6528 6f66 6673 6574 3d2d 6f66 6673  ane(offset=-offs
+000221f0: 6574 5f6c 6973 745b 6920 2b20 315d 290a  et_list[i + 1]).
+00022200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022210: 2e73 706c 696e 6528 6564 6765 5f70 6f69  .spline(edge_poi
+00022220: 6e74 735b 6920 2b20 315d 290a 2020 2020  nts[i + 1]).    
+00022230: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00022240: 2020 6564 6765 5f77 6972 6520 3d20 5b6f    edge_wire = [o
+00022250: 2e76 616c 7328 295b 305d 2066 6f72 206f  .vals()[0] for o
+00022260: 2069 6e20 6564 6765 5f77 6972 652e 616c   in edge_wire.al
+00022270: 6c28 295d 0a20 2020 2020 2020 2065 6467  l()].        edg
+00022280: 655f 7769 7265 203d 2057 6972 652e 6173  e_wire = Wire.as
+00022290: 7365 6d62 6c65 4564 6765 7328 6564 6765  sembleEdges(edge
+000222a0: 5f77 6972 6529 0a0a 2020 2020 6465 6620  _wire)..    def 
+000222b0: 7465 7374 5461 6728 7365 6c66 293a 0a0a  testTag(self):..
+000222c0: 2020 2020 2020 2020 2320 7465 7374 2074          # test t
+000222d0: 6167 6769 6e67 0a20 2020 2020 2020 2072  agging.        r
+000222e0: 6573 756c 7420 3d20 280a 2020 2020 2020  esult = (.      
+000222f0: 2020 2020 2020 576f 726b 706c 616e 6528        Workplane(
+00022300: 2258 5922 290a 2020 2020 2020 2020 2020  "XY").          
+00022310: 2020 2e70 7573 6850 6f69 6e74 7328 5b28    .pushPoints([(
+00022320: 2d32 2c20 3029 2c20 2832 2c20 3029 5d29  -2, 0), (2, 0)])
+00022330: 0a20 2020 2020 2020 2020 2020 202e 626f  .            .bo
+00022340: 7828 312c 2031 2c20 312c 2063 6f6d 6269  x(1, 1, 1, combi
+00022350: 6e65 3d46 616c 7365 290a 2020 2020 2020  ne=False).      
+00022360: 2020 2020 2020 2e74 6167 2822 3220 736f        .tag("2 so
+00022370: 6c69 6473 2229 0a20 2020 2020 2020 2020  lids").         
+00022380: 2020 202e 756e 696f 6e28 576f 726b 706c     .union(Workpl
+00022390: 616e 6528 2258 5922 292e 626f 7828 362c  ane("XY").box(6,
+000223a0: 2031 2c20 3129 290a 2020 2020 2020 2020   1, 1)).        
+000223b0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000223c0: 7373 6572 7445 7175 616c 286c 656e 2872  ssertEqual(len(r
+000223d0: 6573 756c 742e 6f62 6a65 6374 7329 2c20  esult.objects), 
+000223e0: 3129 0a20 2020 2020 2020 2072 6573 756c  1).        resul
+000223f0: 7420 3d20 7265 7375 6c74 2e5f 6765 7454  t = result._getT
+00022400: 6167 6765 6428 2232 2073 6f6c 6964 7322  agged("2 solids"
+00022410: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00022420: 7373 6572 7445 7175 616c 286c 656e 2872  ssertEqual(len(r
+00022430: 6573 756c 742e 6f62 6a65 6374 7329 2c20  esult.objects), 
+00022440: 3229 0a0a 2020 2020 2020 2020 7769 7468  2)..        with
+00022450: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00022460: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00022470: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00022480: 6c74 203d 2072 6573 756c 742e 5f67 6574  lt = result._get
+00022490: 5461 6767 6564 2822 3320 736f 6c69 6473  Tagged("3 solids
+000224a0: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+000224b0: 436f 7079 576f 726b 706c 616e 6528 7365  CopyWorkplane(se
+000224c0: 6c66 293a 0a0a 2020 2020 2020 2020 6f62  lf):..        ob
+000224d0: 6a30 203d 2057 6f72 6b70 6c61 6e65 2822  j0 = Workplane("
+000224e0: 5859 2229 2e62 6f78 2831 2c20 312c 2031  XY").box(1, 1, 1
+000224f0: 3029 2e66 6163 6573 2822 3e5a 2229 2e77  0).faces(">Z").w
+00022500: 6f72 6b70 6c61 6e65 2829 0a20 2020 2020  orkplane().     
+00022510: 2020 206f 626a 3120 3d20 576f 726b 706c     obj1 = Workpl
+00022520: 616e 6528 2258 5922 292e 636f 7079 576f  ane("XY").copyWo
+00022530: 726b 706c 616e 6528 6f62 6a30 292e 626f  rkplane(obj0).bo
+00022540: 7828 312c 2031 2c20 3129 0a20 2020 2020  x(1, 1, 1).     
+00022550: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
+00022560: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
+00022570: 2830 2c20 302c 2035 292c 206f 626a 312e  (0, 0, 5), obj1.
+00022580: 7661 6c28 292e 4365 6e74 6572 2829 2e74  val().Center().t
+00022590: 6f54 7570 6c65 2829 2c20 3929 0a0a 2020  oTuple(), 9)..  
+000225a0: 2020 6465 6620 7465 7374 576f 726b 706c    def testWorkpl
+000225b0: 616e 6546 726f 6d54 6167 6765 6428 7365  aneFromTagged(se
+000225c0: 6c66 293a 0a0a 2020 2020 2020 2020 2320  lf):..        # 
+000225d0: 6372 6561 7465 2061 2066 6c61 742c 2077  create a flat, w
+000225e0: 6964 6520 6261 7365 2e20 4578 7472 7564  ide base. Extrud
+000225f0: 6520 6f6e 6520 6f62 6a65 6374 2034 2075  e one object 4 u
+00022600: 6e69 7473 2068 6967 682c 2061 6e6f 7468  nits high, anoth
+00022610: 6572 0a20 2020 2020 2020 2023 206f 626a  er.        # obj
+00022620: 6563 7420 6f6e 2074 6f70 206f 6620 6974  ect on top of it
+00022630: 2036 2075 6e69 7473 2068 6967 682e 2047   6 units high. G
+00022640: 6f20 6261 636b 2074 6f20 6261 7365 2070  o back to base p
+00022650: 6c61 6e65 2e20 4578 7472 7564 6520 616e  lane. Extrude an
+00022660: 0a20 2020 2020 2020 2023 206f 626a 6563  .        # objec
+00022670: 7420 3131 2075 6e69 7473 2068 6967 682e  t 11 units high.
+00022680: 2041 7373 6572 7420 7468 6174 2074 6f70   Assert that top
+00022690: 2066 6163 6520 6973 2031 3120 756e 6974   face is 11 unit
+000226a0: 7320 6869 6768 2e0a 2020 2020 2020 2020  s high..        
+000226b0: 7265 7375 6c74 203d 2028 0a20 2020 2020  result = (.     
+000226c0: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
+000226d0: 2822 5859 2229 0a20 2020 2020 2020 2020  ("XY").         
+000226e0: 2020 202e 626f 7828 3130 2c20 3130 2c20     .box(10, 10, 
+000226f0: 312c 2063 656e 7465 7265 643d 2854 7275  1, centered=(Tru
+00022700: 652c 2054 7275 652c 2046 616c 7365 2929  e, True, False))
+00022710: 0a20 2020 2020 2020 2020 2020 202e 6661  .            .fa
+00022720: 6365 7328 223e 5a22 290a 2020 2020 2020  ces(">Z").      
+00022730: 2020 2020 2020 2e77 6f72 6b70 6c61 6e65        .workplane
+00022740: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
+00022750: 7461 6728 2262 6173 6522 290a 2020 2020  tag("base").    
+00022760: 2020 2020 2020 2020 2e63 656e 7465 7228          .center(
+00022770: 332c 2030 290a 2020 2020 2020 2020 2020  3, 0).          
+00022780: 2020 2e72 6563 7428 322c 2032 290a 2020    .rect(2, 2).  
+00022790: 2020 2020 2020 2020 2020 2e65 7874 7275            .extru
+000227a0: 6465 2834 290a 2020 2020 2020 2020 2020  de(4).          
+000227b0: 2020 2e66 6163 6573 2822 3e5a 2229 0a20    .faces(">Z"). 
+000227c0: 2020 2020 2020 2020 2020 202e 776f 726b             .work
+000227d0: 706c 616e 6528 290a 2020 2020 2020 2020  plane().        
+000227e0: 2020 2020 2e63 6972 636c 6528 3129 0a20      .circle(1). 
+000227f0: 2020 2020 2020 2020 2020 202e 6578 7472             .extr
+00022800: 7564 6528 3629 0a20 2020 2020 2020 2020  ude(6).         
+00022810: 2020 202e 776f 726b 706c 616e 6546 726f     .workplaneFro
+00022820: 6d54 6167 6765 6428 2262 6173 6522 290a  mTagged("base").
+00022830: 2020 2020 2020 2020 2020 2020 2e63 656e              .cen
+00022840: 7465 7228 2d33 2c20 3029 0a20 2020 2020  ter(-3, 0).     
+00022850: 2020 2020 2020 202e 6369 7263 6c65 2831         .circle(1
+00022860: 290a 2020 2020 2020 2020 2020 2020 2e65  ).            .e
+00022870: 7874 7275 6465 2831 3129 0a20 2020 2020  xtrude(11).     
+00022880: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00022890: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+000228a0: 6f73 7445 7175 616c 7328 0a20 2020 2020  ostEquals(.     
+000228b0: 2020 2020 2020 2072 6573 756c 742e 6661         result.fa
+000228c0: 6365 7328 223e 5a22 292e 7661 6c28 292e  ces(">Z").val().
+000228d0: 4365 6e74 6572 2829 2e74 6f54 7570 6c65  Center().toTuple
+000228e0: 2829 2c20 282d 332c 2030 2c20 3132 292c  (), (-3, 0, 12),
+000228f0: 2039 0a20 2020 2020 2020 2029 0a0a 2020   9.        )..  
+00022900: 2020 6465 6620 7465 7374 576f 726b 706c    def testWorkpl
+00022910: 616e 654f 7269 656e 7461 7469 6f6e 4f6e  aneOrientationOn
+00022920: 5665 7274 6578 2873 656c 6629 3a0a 0a20  Vertex(self):.. 
+00022930: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
+00022940: 6120 3130 2075 6e69 7420 7369 7a65 6420  a 10 unit sized 
+00022950: 6375 6265 206f 6e20 7468 6520 5859 2070  cube on the XY p
+00022960: 6c61 6e65 0a20 2020 2020 2020 2070 6172  lane.        par
+00022970: 656e 7420 3d20 576f 726b 706c 616e 6528  ent = Workplane(
+00022980: 2258 5922 292e 7265 6374 2831 302e 302c  "XY").rect(10.0,
+00022990: 2031 302e 3029 2e65 7874 7275 6465 2831   10.0).extrude(1
+000229a0: 3029 0a0a 2020 2020 2020 2020 2320 6173  0)..        # as
+000229b0: 7365 7274 2074 6861 7420 7468 6520 6469  sert that the di
+000229c0: 7265 6374 696f 6e20 7475 706c 6573 2072  rection tuples r
+000229d0: 6566 6c65 6374 2061 6363 6f72 6469 6e67  eflect according
+000229e0: 6c79 0a20 2020 2020 2020 2061 7373 6572  ly.        asser
+000229f0: 7420 7061 7265 6e74 2e70 6c61 6e65 2e78  t parent.plane.x
+00022a00: 4469 722e 746f 5475 706c 6528 2920 3d3d  Dir.toTuple() ==
+00022a10: 2061 7070 726f 7828 2831 2e30 2c20 302e   approx((1.0, 0.
+00022a20: 302c 2030 2e30 2929 0a20 2020 2020 2020  0, 0.0)).       
+00022a30: 2061 7373 6572 7420 7061 7265 6e74 2e70   assert parent.p
+00022a40: 6c61 6e65 2e7a 4469 722e 746f 5475 706c  lane.zDir.toTupl
+00022a50: 6528 2920 3d3d 2061 7070 726f 7828 2830  e() == approx((0
+00022a60: 2e30 2c20 302e 302c 2031 2e30 2929 0a0a  .0, 0.0, 1.0))..
+00022a70: 2020 2020 2020 2020 2320 7365 6c65 6374          # select
+00022a80: 2074 6865 203c 585a 2076 6572 7465 7820   the <XZ vertex 
+00022a90: 6f6e 2074 6865 203c 5920 6661 6365 2061  on the <Y face a
+00022aa0: 6e64 2063 7265 6174 6520 6120 6e65 7720  nd create a new 
+00022ab0: 776f 726b 706c 616e 652e 0a20 2020 2020  workplane..     
+00022ac0: 2020 2063 6869 6c64 203d 2070 6172 656e     child = paren
+00022ad0: 742e 6661 6365 7328 223c 5922 292e 7665  t.faces("<Y").ve
+00022ae0: 7274 6963 6573 2822 3c58 5a22 292e 776f  rtices("<XZ").wo
+00022af0: 726b 706c 616e 6528 290a 0a20 2020 2020  rkplane()..     
+00022b00: 2020 2023 2061 7373 6572 7420 7468 6174     # assert that
+00022b10: 2074 6865 2064 6972 6563 7469 6f6e 2074   the direction t
+00022b20: 7570 6c65 7320 7265 666c 6563 7420 7468  uples reflect th
+00022b30: 6520 6e65 7720 776f 726b 706c 616e 6520  e new workplane 
+00022b40: 6f6e 2074 6865 203c 5920 6661 6365 0a20  on the <Y face. 
+00022b50: 2020 2020 2020 2061 7373 6572 7420 6368         assert ch
+00022b60: 696c 642e 706c 616e 652e 7844 6972 2e74  ild.plane.xDir.t
+00022b70: 6f54 7570 6c65 2829 203d 3d20 6170 7072  oTuple() == appr
+00022b80: 6f78 2828 312e 302c 2030 2e30 2c20 2d30  ox((1.0, 0.0, -0
+00022b90: 2e30 2929 0a20 2020 2020 2020 2061 7373  .0)).        ass
+00022ba0: 6572 7420 6368 696c 642e 706c 616e 652e  ert child.plane.
+00022bb0: 7a44 6972 2e74 6f54 7570 6c65 2829 203d  zDir.toTuple() =
+00022bc0: 3d20 6170 7072 6f78 2828 302e 302c 202d  = approx((0.0, -
+00022bd0: 312e 302c 202d 302e 3029 290a 0a20 2020  1.0, -0.0))..   
+00022be0: 2064 6566 2074 6573 7454 6167 5365 6c65   def testTagSele
+00022bf0: 6374 6f72 7328 7365 6c66 293a 0a0a 2020  ctors(self):..  
+00022c00: 2020 2020 2020 7265 7375 6c74 3020 3d20        result0 = 
+00022c10: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
+00022c20: 626f 7828 312c 2031 2c20 3129 2e74 6167  box(1, 1, 1).tag
+00022c30: 2822 626f 7822 292e 7370 6865 7265 2831  ("box").sphere(1
+00022c40: 290a 2020 2020 2020 2020 2320 7265 7375  ).        # resu
+00022c50: 6c74 2069 7320 6375 7272 656e 746c 7920  lt is currently 
+00022c60: 6120 7370 6865 7265 0a20 2020 2020 2020  a sphere.       
+00022c70: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00022c80: 6c28 312c 2072 6573 756c 7430 2e66 6163  l(1, result0.fac
+00022c90: 6573 2829 2e73 697a 6528 2929 0a20 2020  es().size()).   
+00022ca0: 2020 2020 2023 2061 2062 6f78 2068 6173       # a box has
+00022cb0: 2038 2076 6572 7469 6365 730a 2020 2020   8 vertices.    
+00022cc0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00022cd0: 7175 616c 2838 2c20 7265 7375 6c74 302e  qual(8, result0.
+00022ce0: 7665 7274 6963 6573 2874 6167 3d22 626f  vertices(tag="bo
+00022cf0: 7822 292e 7369 7a65 2829 290a 2020 2020  x").size()).    
+00022d00: 2020 2020 2320 3620 6661 6365 730a 2020      # 6 faces.  
+00022d10: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00022d20: 7445 7175 616c 2836 2c20 7265 7375 6c74  tEqual(6, result
+00022d30: 302e 6661 6365 7328 7461 673d 2262 6f78  0.faces(tag="box
+00022d40: 2229 2e73 697a 6528 2929 0a20 2020 2020  ").size()).     
+00022d50: 2020 2023 2031 3220 6564 6765 730a 2020     # 12 edges.  
+00022d60: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00022d70: 7445 7175 616c 2831 322c 2072 6573 756c  tEqual(12, resul
+00022d80: 7430 2e65 6467 6573 2874 6167 3d22 626f  t0.edges(tag="bo
+00022d90: 7822 292e 7369 7a65 2829 290a 2020 2020  x").size()).    
+00022da0: 2020 2020 2320 3620 7769 7265 730a 2020      # 6 wires.  
+00022db0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00022dc0: 7445 7175 616c 2836 2c20 7265 7375 6c74  tEqual(6, result
+00022dd0: 302e 7769 7265 7328 7461 673d 2262 6f78  0.wires(tag="box
+00022de0: 2229 2e73 697a 6528 2929 0a0a 2020 2020  ").size())..    
+00022df0: 2020 2020 2320 6372 6561 7465 2074 776f      # create two
+00022e00: 2073 6f6c 6964 732c 2074 6167 2074 6865   solids, tag the
+00022e10: 6d2c 206a 6f69 6e20 746f 206f 6e65 2073  m, join to one s
+00022e20: 6f6c 6964 0a20 2020 2020 2020 2072 6573  olid.        res
+00022e30: 756c 7431 203d 2028 0a20 2020 2020 2020  ult1 = (.       
+00022e40: 2020 2020 2057 6f72 6b70 6c61 6e65 2822       Workplane("
+00022e50: 5859 2229 0a20 2020 2020 2020 2020 2020  XY").           
+00022e60: 202e 7075 7368 506f 696e 7473 285b 2831   .pushPoints([(1
+00022e70: 2c20 3029 2c20 282d 312c 2030 295d 290a  , 0), (-1, 0)]).
+00022e80: 2020 2020 2020 2020 2020 2020 2e62 6f78              .box
+00022e90: 2831 2c20 312c 2031 290a 2020 2020 2020  (1, 1, 1).      
+00022ea0: 2020 2020 2020 2e74 6167 2822 626f 7865        .tag("boxe
+00022eb0: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
+00022ec0: 2e73 7068 6572 6528 3129 0a20 2020 2020  .sphere(1).     
+00022ed0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00022ee0: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
+00022ef0: 2072 6573 756c 7431 2e73 6f6c 6964 7328   result1.solids(
+00022f00: 292e 7369 7a65 2829 290a 2020 2020 2020  ).size()).      
+00022f10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00022f20: 616c 2832 2c20 7265 7375 6c74 312e 736f  al(2, result1.so
+00022f30: 6c69 6473 2874 6167 3d22 626f 7865 7322  lids(tag="boxes"
+00022f40: 292e 7369 7a65 2829 290a 2020 2020 2020  ).size()).      
+00022f50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00022f60: 616c 2831 2c20 7265 7375 6c74 312e 7368  al(1, result1.sh
+00022f70: 656c 6c73 2829 2e73 697a 6528 2929 0a20  ells().size()). 
+00022f80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00022f90: 7274 4571 7561 6c28 322c 2072 6573 756c  rtEqual(2, resul
+00022fa0: 7431 2e73 6865 6c6c 7328 7461 673d 2262  t1.shells(tag="b
+00022fb0: 6f78 6573 2229 2e73 697a 6528 2929 0a0a  oxes").size())..
+00022fc0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+00022fd0: 2034 2069 6e64 6976 6964 7561 6c20 6f62   4 individual ob
+00022fe0: 6a65 6374 732c 2074 6167 2069 742c 2074  jects, tag it, t
+00022ff0: 6865 6e20 636f 6d62 696e 6520 746f 206f  hen combine to o
+00023000: 6e65 2063 6f6d 706f 756e 640a 2020 2020  ne compound.    
+00023010: 2020 2020 7265 7375 6c74 3220 3d20 280a      result2 = (.
+00023020: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+00023030: 706c 616e 6528 2258 5922 290a 2020 2020  plane("XY").    
+00023040: 2020 2020 2020 2020 2e72 6563 7428 342c          .rect(4,
+00023050: 2034 290a 2020 2020 2020 2020 2020 2020   4).            
+00023060: 2e76 6572 7469 6365 7328 290a 2020 2020  .vertices().    
+00023070: 2020 2020 2020 2020 2e62 6f78 2831 2c20          .box(1, 
+00023080: 312c 2031 2c20 636f 6d62 696e 653d 4661  1, 1, combine=Fa
+00023090: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+000230a0: 202e 7461 6728 2234 206f 626a 7322 290a   .tag("4 objs").
+000230b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000230c0: 2020 7265 7375 6c74 3220 3d20 7265 7375    result2 = resu
+000230d0: 6c74 322e 6e65 774f 626a 6563 7428 5b43  lt2.newObject([C
+000230e0: 6f6d 706f 756e 642e 6d61 6b65 436f 6d70  ompound.makeComp
+000230f0: 6f75 6e64 2872 6573 756c 7432 2e6f 626a  ound(result2.obj
+00023100: 6563 7473 295d 290a 2020 2020 2020 2020  ects)]).        
+00023110: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00023120: 2831 2c20 7265 7375 6c74 322e 636f 6d70  (1, result2.comp
+00023130: 6f75 6e64 7328 292e 7369 7a65 2829 290a  ounds().size()).
+00023140: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00023150: 6572 7445 7175 616c 2830 2c20 7265 7375  ertEqual(0, resu
+00023160: 6c74 322e 636f 6d70 6f75 6e64 7328 7461  lt2.compounds(ta
+00023170: 673d 2234 206f 626a 7322 292e 7369 7a65  g="4 objs").size
+00023180: 2829 290a 0a20 2020 2064 6566 2074 6573  ())..    def tes
+00023190: 745f 696e 7465 7270 506c 6174 6528 7365  t_interpPlate(se
+000231a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000231b0: 0a20 2020 2020 2020 2054 6573 7473 2074  .        Tests t
+000231c0: 6865 2069 6e74 6572 7050 6c61 7465 2829  he interpPlate()
+000231d0: 2066 756e 6374 696f 6e61 6c69 7469 6573   functionalities
+000231e0: 0a20 2020 2020 2020 204e 756d 6572 6963  .        Numeric
+000231f0: 616c 2076 616c 7565 7320 6f66 2041 7265  al values of Are
+00023200: 6173 2061 6e64 2056 6f6c 756d 6573 2077  as and Volumes w
+00023210: 6572 6520 6f62 7461 696e 6564 2077 6974  ere obtained wit
+00023220: 6820 7468 6520 4172 6561 2829 2061 6e64  h the Area() and
+00023230: 2056 6f6c 756d 6528 2920 6675 6e63 7469   Volume() functi
+00023240: 6f6e 7320 6f6e 2061 204c 696e 7578 206d  ons on a Linux m
+00023250: 6163 6869 6e65 2075 6e64 6572 2044 6562  achine under Deb
+00023260: 6961 6e20 3130 2077 6974 6820 7079 7468  ian 10 with pyth
+00023270: 6f6e 2033 2e37 2e0a 2020 2020 2020 2020  on 3.7..        
+00023280: 2222 220a 0a20 2020 2020 2020 2023 2065  """..        # e
+00023290: 7861 6d70 6c65 2066 726f 6d20 5079 7468  xample from Pyth
+000232a0: 6f6e 4f43 4320 636f 7265 5f67 656f 6d65  onOCC core_geome
+000232b0: 7472 795f 6765 6f6d 706c 6174 652e 7079  try_geomplate.py
+000232c0: 2c20 7573 6520 6f66 2074 6869 636b 6e65  , use of thickne
+000232d0: 7373 203d 2030 2072 6574 7572 6e73 2032  ss = 0 returns 2
+000232e0: 4420 7375 7266 6163 652e 0a20 2020 2020  D surface..     
+000232f0: 2020 2074 6869 636b 6e65 7373 203d 2030     thickness = 0
+00023300: 0a20 2020 2020 2020 2065 6467 655f 706f  .        edge_po
+00023310: 696e 7473 203d 205b 0a20 2020 2020 2020  ints = [.       
+00023320: 2020 2020 2028 302e 302c 2030 2e30 2c20       (0.0, 0.0, 
+00023330: 302e 3029 2c0a 2020 2020 2020 2020 2020  0.0),.          
+00023340: 2020 2830 2e30 2c20 3130 2e30 2c20 302e    (0.0, 10.0, 0.
+00023350: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
+00023360: 2830 2e30 2c20 3130 2e30 2c20 3130 2e30  (0.0, 10.0, 10.0
+00023370: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00023380: 302e 302c 2030 2e30 2c20 3130 2e30 292c  0.0, 0.0, 10.0),
+00023390: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+000233a0: 2020 2073 7572 6661 6365 5f70 6f69 6e74     surface_point
+000233b0: 7320 3d20 5b28 352e 302c 2035 2e30 2c20  s = [(5.0, 5.0, 
+000233c0: 352e 3029 5d0a 2020 2020 2020 2020 706c  5.0)].        pl
+000233d0: 6174 655f 3020 3d20 576f 726b 706c 616e  ate_0 = Workplan
+000233e0: 6528 2258 5922 292e 696e 7465 7270 506c  e("XY").interpPl
+000233f0: 6174 6528 6564 6765 5f70 6f69 6e74 732c  ate(edge_points,
+00023400: 2073 7572 6661 6365 5f70 6f69 6e74 732c   surface_points,
+00023410: 2074 6869 636b 6e65 7373 290a 2020 2020   thickness).    
+00023420: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00023430: 7275 6528 706c 6174 655f 302e 7661 6c28  rue(plate_0.val(
+00023440: 292e 6973 5661 6c69 6428 2929 0a20 2020  ).isValid()).   
+00023450: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00023460: 416c 6d6f 7374 4571 7561 6c28 706c 6174  AlmostEqual(plat
+00023470: 655f 302e 7661 6c28 292e 4172 6561 2829  e_0.val().Area()
+00023480: 2c20 3134 312e 3231 3838 3233 3839 322c  , 141.218823892,
+00023490: 2031 290a 0a20 2020 2020 2020 2023 2050   1)..        # P
+000234a0: 6c61 7465 2077 6974 6820 3520 7369 6465  late with 5 side
+000234b0: 7320 616e 6420 3220 6275 6d70 732c 206f  s and 2 bumps, o
+000234c0: 6e65 2073 6964 6520 6973 206e 6f74 2063  ne side is not c
+000234d0: 6f2d 706c 616e 6172 2077 6974 6820 7468  o-planar with th
+000234e0: 6520 6f74 6865 7220 7369 6465 730a 2020  e other sides.  
+000234f0: 2020 2020 2020 7468 6963 6b6e 6573 7320        thickness 
+00023500: 3d20 302e 310a 2020 2020 2020 2020 6564  = 0.1.        ed
+00023510: 6765 5f70 6f69 6e74 7320 3d20 5b0a 2020  ge_points = [.  
+00023520: 2020 2020 2020 2020 2020 282d 372e 302c            (-7.0,
+00023530: 202d 372e 302c 2030 2e30 292c 0a20 2020   -7.0, 0.0),.   
+00023540: 2020 2020 2020 2020 2028 2d33 2e30 2c20           (-3.0, 
+00023550: 2d31 302e 302c 2033 2e30 292c 0a20 2020  -10.0, 3.0),.   
+00023560: 2020 2020 2020 2020 2028 372e 302c 202d           (7.0, -
+00023570: 372e 302c 2030 2e30 292c 0a20 2020 2020  7.0, 0.0),.     
+00023580: 2020 2020 2020 2028 372e 302c 2037 2e30         (7.0, 7.0
+00023590: 2c20 302e 3029 2c0a 2020 2020 2020 2020  , 0.0),.        
+000235a0: 2020 2020 282d 372e 302c 2037 2e30 2c20      (-7.0, 7.0, 
+000235b0: 302e 3029 2c0a 2020 2020 2020 2020 5d0a  0.0),.        ].
+000235c0: 2020 2020 2020 2020 6564 6765 5f77 6972          edge_wir
+000235d0: 6520 3d20 576f 726b 706c 616e 6528 2258  e = Workplane("X
+000235e0: 5922 292e 706f 6c79 6c69 6e65 280a 2020  Y").polyline(.  
+000235f0: 2020 2020 2020 2020 2020 5b28 2d37 2e30            [(-7.0
+00023600: 2c20 2d37 2e30 292c 2028 372e 302c 202d  , -7.0), (7.0, -
+00023610: 372e 3029 2c20 2837 2e30 2c20 372e 3029  7.0), (7.0, 7.0)
+00023620: 2c20 282d 372e 302c 2037 2e30 295d 0a20  , (-7.0, 7.0)]. 
+00023630: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00023640: 2023 2065 6467 655f 7769 7265 203d 2065   # edge_wire = e
+00023650: 6467 655f 7769 7265 2e61 6464 2857 6f72  dge_wire.add(Wor
+00023660: 6b70 6c61 6e65 2827 595a 2729 2e77 6f72  kplane('YZ').wor
+00023670: 6b70 6c61 6e65 2829 2e74 7261 6e73 666f  kplane().transfo
+00023680: 726d 6564 286f 6666 7365 743d 5665 6374  rmed(offset=Vect
+00023690: 6f72 2830 2c20 302c 202d 3729 2c20 726f  or(0, 0, -7), ro
+000236a0: 7461 7465 3d56 6563 746f 7228 3435 2c20  tate=Vector(45, 
+000236b0: 302c 2030 2929 2e70 6f6c 796c 696e 6528  0, 0)).polyline(
+000236c0: 5b28 2d37 2e2c 302e 292c 2028 332c 2d33  [(-7.,0.), (3,-3
+000236d0: 292c 2028 372e 2c30 2e29 5d29 290a 2020  ), (7.,0.)])).  
+000236e0: 2020 2020 2020 2320 496e 2043 6164 5175        # In CadQu
+000236f0: 6572 7920 5365 7074 2d32 3031 3920 6974  ery Sept-2019 it
+00023700: 2077 6f72 6b65 6420 7769 7468 2072 6f74   worked with rot
+00023710: 6174 653d 5665 6374 6f72 2830 2c20 3435  ate=Vector(0, 45
+00023720: 2c20 3029 2e20 496e 2043 6164 5175 6572  , 0). In CadQuer
+00023730: 7920 4465 632d 3230 3139 2072 6f74 6174  y Dec-2019 rotat
+00023740: 653d 5665 6374 6f72 2834 352c 2030 2c20  e=Vector(45, 0, 
+00023750: 3029 206f 6e6c 7920 636c 6f73 6573 2074  0) only closes t
+00023760: 6865 2077 6972 652e 0a20 2020 2020 2020  he wire..       
+00023770: 2065 6467 655f 7769 7265 203d 2065 6467   edge_wire = edg
+00023780: 655f 7769 7265 2e61 6464 280a 2020 2020  e_wire.add(.    
+00023790: 2020 2020 2020 2020 576f 726b 706c 616e          Workplan
+000237a0: 6528 2259 5a22 290a 2020 2020 2020 2020  e("YZ").        
+000237b0: 2020 2020 2e77 6f72 6b70 6c61 6e65 2829      .workplane()
+000237c0: 0a20 2020 2020 2020 2020 2020 202e 7472  .            .tr
+000237d0: 616e 7366 6f72 6d65 6428 6f66 6673 6574  ansformed(offset
+000237e0: 3d56 6563 746f 7228 302c 2030 2c20 2d37  =Vector(0, 0, -7
+000237f0: 292c 2072 6f74 6174 653d 5665 6374 6f72  ), rotate=Vector
+00023800: 2834 352c 2030 2c20 3029 290a 2020 2020  (45, 0, 0)).    
+00023810: 2020 2020 2020 2020 2e73 706c 696e 6528          .spline(
+00023820: 5b28 2d37 2e30 2c20 302e 3029 2c20 2833  [(-7.0, 0.0), (3
+00023830: 2c20 2d33 292c 2028 372e 302c 2030 2e30  , -3), (7.0, 0.0
+00023840: 295d 290a 2020 2020 2020 2020 290a 2020  )]).        ).  
+00023850: 2020 2020 2020 7375 7266 6163 655f 706f        surface_po
+00023860: 696e 7473 203d 205b 282d 332e 302c 202d  ints = [(-3.0, -
+00023870: 332e 302c 202d 332e 3029 2c20 2833 2e30  3.0, -3.0), (3.0
+00023880: 2c20 332e 302c 2033 2e30 295d 0a20 2020  , 3.0, 3.0)].   
+00023890: 2020 2020 2070 6c61 7465 5f31 203d 2057       plate_1 = W
+000238a0: 6f72 6b70 6c61 6e65 2822 5859 2229 2e69  orkplane("XY").i
+000238b0: 6e74 6572 7050 6c61 7465 2865 6467 655f  nterpPlate(edge_
+000238c0: 7769 7265 2c20 7375 7266 6163 655f 706f  wire, surface_po
+000238d0: 696e 7473 2c20 7468 6963 6b6e 6573 7329  ints, thickness)
+000238e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000238f0: 7365 7274 5472 7565 2870 6c61 7465 5f31  sertTrue(plate_1
+00023900: 2e76 616c 2829 2e69 7356 616c 6964 2829  .val().isValid()
+00023910: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00023920: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
+00023930: 2870 6c61 7465 5f31 2e76 616c 2829 2e56  (plate_1.val().V
+00023940: 6f6c 756d 6528 292c 2032 362e 3132 3439  olume(), 26.1249
+00023950: 3730 3230 362c 2032 290a 0a20 2020 2020  70206, 2)..     
+00023960: 2020 2023 2045 6d62 6f73 7365 6420 7374     # Embossed st
+00023970: 6172 2c20 6e65 6564 2074 6f20 6368 616e  ar, need to chan
+00023980: 6765 206f 7074 696f 6e61 6c20 7061 7261  ge optional para
+00023990: 6d65 7465 7273 2074 6f20 6f62 7461 696e  meters to obtain
+000239a0: 206e 6963 6520 6c6f 6f6b 696e 6720 7265   nice looking re
+000239b0: 7375 6c74 2e0a 2020 2020 2020 2020 7231  sult..        r1
+000239c0: 203d 2033 2e30 0a20 2020 2020 2020 2072   = 3.0.        r
+000239d0: 3220 3d20 3130 2e30 0a20 2020 2020 2020  2 = 10.0.       
+000239e0: 2066 6e20 3d20 360a 2020 2020 2020 2020   fn = 6.        
+000239f0: 7468 6963 6b6e 6573 7320 3d20 302e 310a  thickness = 0.1.
+00023a00: 2020 2020 2020 2020 6564 6765 5f70 6f69          edge_poi
+00023a10: 6e74 7320 3d20 5b0a 2020 2020 2020 2020  nts = [.        
+00023a20: 2020 2020 2872 3120 2a20 6d61 7468 2e63      (r1 * math.c
+00023a30: 6f73 2869 202a 206d 6174 682e 7069 202f  os(i * math.pi /
+00023a40: 2066 6e29 2c20 7231 202a 206d 6174 682e   fn), r1 * math.
+00023a50: 7369 6e28 6920 2a20 6d61 7468 2e70 6920  sin(i * math.pi 
+00023a60: 2f20 666e 2929 0a20 2020 2020 2020 2020  / fn)).         
+00023a70: 2020 2069 6620 6920 2520 3220 3d3d 2030     if i % 2 == 0
+00023a80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00023a90: 6520 2872 3220 2a20 6d61 7468 2e63 6f73  e (r2 * math.cos
+00023aa0: 2869 202a 206d 6174 682e 7069 202f 2066  (i * math.pi / f
+00023ab0: 6e29 2c20 7232 202a 206d 6174 682e 7369  n), r2 * math.si
+00023ac0: 6e28 6920 2a20 6d61 7468 2e70 6920 2f20  n(i * math.pi / 
+00023ad0: 666e 2929 0a20 2020 2020 2020 2020 2020  fn)).           
+00023ae0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00023af0: 3220 2a20 666e 202b 2031 290a 2020 2020  2 * fn + 1).    
+00023b00: 2020 2020 5d0a 2020 2020 2020 2020 6564      ].        ed
+00023b10: 6765 5f77 6972 6520 3d20 576f 726b 706c  ge_wire = Workpl
+00023b20: 616e 6528 2258 5922 292e 706f 6c79 6c69  ane("XY").polyli
+00023b30: 6e65 2865 6467 655f 706f 696e 7473 290a  ne(edge_points).
+00023b40: 2020 2020 2020 2020 7232 203d 2034 2e35          r2 = 4.5
+00023b50: 0a20 2020 2020 2020 2073 7572 6661 6365  .        surface
+00023b60: 5f70 6f69 6e74 7320 3d20 5b0a 2020 2020  _points = [.    
+00023b70: 2020 2020 2020 2020 2872 3220 2a20 6d61          (r2 * ma
+00023b80: 7468 2e63 6f73 2869 202a 206d 6174 682e  th.cos(i * math.
+00023b90: 7069 202f 2066 6e29 2c20 7232 202a 206d  pi / fn), r2 * m
+00023ba0: 6174 682e 7369 6e28 6920 2a20 6d61 7468  ath.sin(i * math
+00023bb0: 2e70 6920 2f20 666e 292c 2031 2e30 290a  .pi / fn), 1.0).
+00023bc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00023bd0: 6920 696e 2072 616e 6765 2832 202a 2066  i in range(2 * f
+00023be0: 6e29 0a20 2020 2020 2020 205d 202b 205b  n).        ] + [
+00023bf0: 2830 2e30 2c20 302e 302c 202d 322e 3029  (0.0, 0.0, -2.0)
+00023c00: 5d0a 2020 2020 2020 2020 706c 6174 655f  ].        plate_
+00023c10: 3220 3d20 576f 726b 706c 616e 6528 2258  2 = Workplane("X
+00023c20: 5922 292e 696e 7465 7270 506c 6174 6528  Y").interpPlate(
+00023c30: 0a20 2020 2020 2020 2020 2020 2065 6467  .            edg
+00023c40: 655f 7769 7265 2c0a 2020 2020 2020 2020  e_wire,.        
+00023c50: 2020 2020 7375 7266 6163 655f 706f 696e      surface_poin
+00023c60: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+00023c70: 7468 6963 6b6e 6573 732c 0a20 2020 2020  thickness,.     
+00023c80: 2020 2020 2020 2063 6f6d 6269 6e65 3d54         combine=T
+00023c90: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00023ca0: 2063 6c65 616e 3d54 7275 652c 0a20 2020   clean=True,.   
+00023cb0: 2020 2020 2020 2020 2064 6567 7265 653d           degree=
+00023cc0: 332c 0a20 2020 2020 2020 2020 2020 206e  3,.            n
+00023cd0: 6250 7473 4f6e 4375 723d 3135 2c0a 2020  bPtsOnCur=15,.  
+00023ce0: 2020 2020 2020 2020 2020 6e62 4974 6572            nbIter
+00023cf0: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+00023d00: 616e 6973 6f74 726f 7079 3d46 616c 7365  anisotropy=False
+00023d10: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
+00023d20: 6c32 643d 302e 3030 3030 312c 0a20 2020  l2d=0.00001,.   
+00023d30: 2020 2020 2020 2020 2074 6f6c 3364 3d30           tol3d=0
+00023d40: 2e30 3030 312c 0a20 2020 2020 2020 2020  .0001,.         
+00023d50: 2020 2074 6f6c 416e 673d 302e 3031 2c0a     tolAng=0.01,.
+00023d60: 2020 2020 2020 2020 2020 2020 746f 6c43              tolC
+00023d70: 7572 763d 302e 312c 0a20 2020 2020 2020  urv=0.1,.       
+00023d80: 2020 2020 206d 6178 4465 673d 382c 0a20       maxDeg=8,. 
+00023d90: 2020 2020 2020 2020 2020 206d 6178 5365             maxSe
+00023da0: 676d 656e 7473 3d34 392c 0a20 2020 2020  gments=49,.     
+00023db0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00023dc0: 662e 6173 7365 7274 5472 7565 2870 6c61  f.assertTrue(pla
+00023dd0: 7465 5f32 2e76 616c 2829 2e69 7356 616c  te_2.val().isVal
+00023de0: 6964 2829 290a 2020 2020 2020 2020 7365  id()).        se
+00023df0: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
+00023e00: 7175 616c 2870 6c61 7465 5f32 2e76 616c  qual(plate_2.val
+00023e10: 2829 2e56 6f6c 756d 6528 292c 2031 302e  ().Volume(), 10.
+00023e20: 3935 3630 3534 3331 342c 2030 290a 0a20  956054314, 0).. 
+00023e30: 2020 2020 2020 2023 2050 6f69 6e74 7320         # Points 
+00023e40: 6f6e 2068 6578 6167 6f6e 616c 2070 6174  on hexagonal pat
+00023e50: 7465 726e 2063 6f6f 7264 696e 6174 6573  tern coordinates
+00023e60: 2c20 7573 6520 6f66 2070 7573 6870 6f69  , use of pushpoi
+00023e70: 6e74 732e 0a20 2020 2020 2020 2072 3120  nts..        r1 
+00023e80: 3d20 312e 300a 2020 2020 2020 2020 4e20  = 1.0.        N 
+00023e90: 3d20 330a 2020 2020 2020 2020 6361 203d  = 3.        ca =
+00023ea0: 206d 6174 682e 636f 7328 3330 2e30 202a   math.cos(30.0 *
+00023eb0: 206d 6174 682e 7069 202f 2031 3830 2e30   math.pi / 180.0
+00023ec0: 290a 2020 2020 2020 2020 7361 203d 206d  ).        sa = m
+00023ed0: 6174 682e 7369 6e28 3330 2e30 202a 206d  ath.sin(30.0 * m
+00023ee0: 6174 682e 7069 202f 2031 3830 2e30 290a  ath.pi / 180.0).
+00023ef0: 2020 2020 2020 2020 2320 4556 454e 2052          # EVEN R
+00023f00: 4f57 530a 2020 2020 2020 2020 7074 7320  OWS.        pts 
+00023f10: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00023f20: 282d 332e 302c 202d 332e 3029 2c0a 2020  (-3.0, -3.0),.  
+00023f30: 2020 2020 2020 2020 2020 282d 312e 3236            (-1.26
+00023f40: 3739 3439 2c20 2d33 2e30 292c 0a20 2020  7949, -3.0),.   
+00023f50: 2020 2020 2020 2020 2028 302e 3436 3431           (0.4641
+00023f60: 3032 2c20 2d33 2e30 292c 0a20 2020 2020  02, -3.0),.     
+00023f70: 2020 2020 2020 2028 322e 3139 3631 3532         (2.196152
+00023f80: 2c20 2d33 2e30 292c 0a20 2020 2020 2020  , -3.0),.       
+00023f90: 2020 2020 2028 2d33 2e30 2c20 302e 3029       (-3.0, 0.0)
+00023fa0: 2c0a 2020 2020 2020 2020 2020 2020 282d  ,.            (-
+00023fb0: 312e 3236 3739 3439 2c20 302e 3029 2c0a  1.267949, 0.0),.
+00023fc0: 2020 2020 2020 2020 2020 2020 2830 2e34              (0.4
+00023fd0: 3634 3130 322c 2030 2e30 292c 0a20 2020  64102, 0.0),.   
+00023fe0: 2020 2020 2020 2020 2028 322e 3139 3631           (2.1961
+00023ff0: 3532 2c20 302e 3029 2c0a 2020 2020 2020  52, 0.0),.      
+00024000: 2020 2020 2020 282d 322e 3133 3339 3734        (-2.133974
+00024010: 2c20 2d31 2e35 292c 0a20 2020 2020 2020  , -1.5),.       
+00024020: 2020 2020 2028 2d30 2e34 3031 3932 332c       (-0.401923,
+00024030: 202d 312e 3529 2c0a 2020 2020 2020 2020   -1.5),.        
+00024040: 2020 2020 2831 2e33 3330 3132 372c 202d      (1.330127, -
+00024050: 312e 3529 2c0a 2020 2020 2020 2020 2020  1.5),.          
+00024060: 2020 2833 2e30 3632 3137 382c 202d 312e    (3.062178, -1.
+00024070: 3529 2c0a 2020 2020 2020 2020 2020 2020  5),.            
+00024080: 282d 322e 3133 3339 3735 2c20 312e 3529  (-2.133975, 1.5)
+00024090: 2c0a 2020 2020 2020 2020 2020 2020 282d  ,.            (-
+000240a0: 302e 3430 3139 3234 2c20 312e 3529 2c0a  0.401924, 1.5),.
+000240b0: 2020 2020 2020 2020 2020 2020 2831 2e33              (1.3
+000240c0: 3330 3132 372c 2031 2e35 292c 0a20 2020  30127, 1.5),.   
+000240d0: 2020 2020 2020 2020 2028 332e 3036 3231           (3.0621
+000240e0: 3738 2c20 312e 3529 2c0a 2020 2020 2020  78, 1.5),.      
+000240f0: 2020 5d0a 2020 2020 2020 2020 2320 5370    ].        # Sp
+00024100: 696b 6520 7375 7266 6163 650a 2020 2020  ike surface.    
+00024110: 2020 2020 7468 6963 6b6e 6573 7320 3d20      thickness = 
+00024120: 302e 310a 2020 2020 2020 2020 666e 203d  0.1.        fn =
+00024130: 2036 0a20 2020 2020 2020 2065 6467 655f   6.        edge_
+00024140: 706f 696e 7473 203d 205b 0a20 2020 2020  points = [.     
+00024150: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+00024160: 2020 2020 2020 2020 2072 3120 2a20 6d61           r1 * ma
+00024170: 7468 2e63 6f73 2869 202a 2032 202a 206d  th.cos(i * 2 * m
+00024180: 6174 682e 7069 202f 2066 6e20 2b20 3330  ath.pi / fn + 30
+00024190: 202a 206d 6174 682e 7069 202f 2031 3830   * math.pi / 180
+000241a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000241b0: 2020 2072 3120 2a20 6d61 7468 2e73 696e     r1 * math.sin
+000241c0: 2869 202a 2032 202a 206d 6174 682e 7069  (i * 2 * math.pi
+000241d0: 202f 2066 6e20 2b20 3330 202a 206d 6174   / fn + 30 * mat
+000241e0: 682e 7069 202f 2031 3830 292c 0a20 2020  h.pi / 180),.   
+000241f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00024200: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00024210: 7261 6e67 6528 666e 202b 2031 290a 2020  range(fn + 1).  
+00024220: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00024230: 7375 7266 6163 655f 706f 696e 7473 203d  surface_points =
+00024240: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
+00024250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024260: 2072 3120 2f20 3420 2a20 6d61 7468 2e63   r1 / 4 * math.c
+00024270: 6f73 2869 202a 2032 202a 206d 6174 682e  os(i * 2 * math.
+00024280: 7069 202f 2066 6e20 2b20 3330 202a 206d  pi / fn + 30 * m
+00024290: 6174 682e 7069 202f 2031 3830 292c 0a20  ath.pi / 180),. 
+000242a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000242b0: 3120 2f20 3420 2a20 6d61 7468 2e73 696e  1 / 4 * math.sin
+000242c0: 2869 202a 2032 202a 206d 6174 682e 7069  (i * 2 * math.pi
+000242d0: 202f 2066 6e20 2b20 3330 202a 206d 6174   / fn + 30 * mat
+000242e0: 682e 7069 202f 2031 3830 292c 0a20 2020  h.pi / 180),.   
+000242f0: 2020 2020 2020 2020 2020 2020 2030 2e37               0.7
+00024300: 352c 0a20 2020 2020 2020 2020 2020 2029  5,.            )
+00024310: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00024320: 2069 2069 6e20 7261 6e67 6528 666e 202b   i in range(fn +
+00024330: 2031 290a 2020 2020 2020 2020 5d20 2b20   1).        ] + 
+00024340: 5b28 302c 2030 2c20 3229 5d0a 2020 2020  [(0, 0, 2)].    
+00024350: 2020 2020 6564 6765 5f77 6972 6520 3d20      edge_wire = 
+00024360: 576f 726b 706c 616e 6528 2258 5922 292e  Workplane("XY").
+00024370: 706f 6c79 6c69 6e65 2865 6467 655f 706f  polyline(edge_po
+00024380: 696e 7473 290a 2020 2020 2020 2020 706c  ints).        pl
+00024390: 6174 655f 3320 3d20 280a 2020 2020 2020  ate_3 = (.      
+000243a0: 2020 2020 2020 576f 726b 706c 616e 6528        Workplane(
+000243b0: 2258 5922 290a 2020 2020 2020 2020 2020  "XY").          
+000243c0: 2020 2e70 7573 6850 6f69 6e74 7328 7074    .pushPoints(pt
+000243d0: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
+000243e0: 696e 7465 7270 506c 6174 6528 0a20 2020  interpPlate(.   
+000243f0: 2020 2020 2020 2020 2020 2020 2065 6467               edg
+00024400: 655f 7769 7265 2c0a 2020 2020 2020 2020  e_wire,.        
+00024410: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
+00024420: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
+00024430: 2020 2020 2020 2020 7468 6963 6b6e 6573          thicknes
+00024440: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00024450: 2020 2063 6f6d 6269 6e65 3d46 616c 7365     combine=False
+00024460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024470: 2020 636c 6561 6e3d 4661 6c73 652c 0a20    clean=False,. 
+00024480: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00024490: 6567 7265 653d 322c 0a20 2020 2020 2020  egree=2,.       
+000244a0: 2020 2020 2020 2020 206e 6250 7473 4f6e           nbPtsOn
+000244b0: 4375 723d 3230 2c0a 2020 2020 2020 2020  Cur=20,.        
+000244c0: 2020 2020 2020 2020 6e62 4974 6572 3d32          nbIter=2
+000244d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000244e0: 2020 616e 6973 6f74 726f 7079 3d46 616c    anisotropy=Fal
+000244f0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00024500: 2020 2020 746f 6c32 643d 302e 3030 3030      tol2d=0.0000
+00024510: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00024520: 2020 2074 6f6c 3364 3d30 2e30 3030 312c     tol3d=0.0001,
+00024530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024540: 2074 6f6c 416e 673d 302e 3031 2c0a 2020   tolAng=0.01,.  
+00024550: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00024560: 6c43 7572 763d 302e 312c 0a20 2020 2020  lCurv=0.1,.     
+00024570: 2020 2020 2020 2020 2020 206d 6178 4465             maxDe
+00024580: 673d 382c 0a20 2020 2020 2020 2020 2020  g=8,.           
+00024590: 2020 2020 206d 6178 5365 676d 656e 7473       maxSegments
+000245a0: 3d39 2c0a 2020 2020 2020 2020 2020 2020  =9,.            
+000245b0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+000245c0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000245d0: 7275 6528 706c 6174 655f 332e 7661 6c28  rue(plate_3.val(
+000245e0: 292e 6973 5661 6c69 6428 2929 0a20 2020  ).isValid()).   
+000245f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00024600: 416c 6d6f 7374 4571 7561 6c28 706c 6174  AlmostEqual(plat
+00024610: 655f 332e 7661 6c28 292e 566f 6c75 6d65  e_3.val().Volume
+00024620: 2829 2c20 302e 3435 3839 3339 3534 3638  (), 0.4589395468
+00024630: 3531 3839 3431 342c 2031 290a 0a20 2020  5189414, 1)..   
+00024640: 2020 2020 2023 2047 7972 6fc3 af64 2c20       # Gyro..d, 
+00024650: 616c 6c20 6564 6765 7320 6172 6520 7370  all edges are sp
+00024660: 6c69 6e65 7320 6f6e 2064 6966 6665 7265  lines on differe
+00024670: 6e74 2077 6f72 6b70 6c61 6e65 732e 0a20  nt workplanes.. 
+00024680: 2020 2020 2020 2074 6869 636b 6e65 7373         thickness
+00024690: 203d 2030 2e31 0a20 2020 2020 2020 2065   = 0.1.        e
+000246a0: 6467 655f 706f 696e 7473 203d 205b 0a20  dge_points = [. 
+000246b0: 2020 2020 2020 2020 2020 205b 5b33 2e35             [[3.5
+000246c0: 342c 2033 2e35 345d 2c20 5b31 2e37 372c  4, 3.54], [1.77,
+000246d0: 2030 2e30 5d2c 205b 332e 3534 2c20 2d33   0.0], [3.54, -3
+000246e0: 2e35 345d 5d2c 0a20 2020 2020 2020 2020  .54]],.         
+000246f0: 2020 205b 5b2d 332e 3534 2c20 2d33 2e35     [[-3.54, -3.5
+00024700: 345d 2c20 5b30 2e30 2c20 2d31 2e37 375d  4], [0.0, -1.77]
+00024710: 2c20 5b33 2e35 342c 202d 332e 3534 5d5d  , [3.54, -3.54]]
+00024720: 2c0a 2020 2020 2020 2020 2020 2020 5b5b  ,.            [[
+00024730: 2d33 2e35 342c 202d 332e 3534 5d2c 205b  -3.54, -3.54], [
+00024740: 302e 302c 202d 312e 3737 5d2c 205b 332e  0.0, -1.77], [3.
+00024750: 3534 2c20 2d33 2e35 345d 5d2c 0a20 2020  54, -3.54]],.   
+00024760: 2020 2020 2020 2020 205b 5b2d 332e 3534           [[-3.54
+00024770: 2c20 2d33 2e35 345d 2c20 5b2d 312e 3737  , -3.54], [-1.77
+00024780: 2c20 302e 305d 2c20 5b2d 332e 3534 2c20  , 0.0], [-3.54, 
+00024790: 332e 3534 5d5d 2c0a 2020 2020 2020 2020  3.54]],.        
+000247a0: 2020 2020 5b5b 332e 3534 2c20 332e 3534      [[3.54, 3.54
+000247b0: 5d2c 205b 302e 302c 2031 2e37 375d 2c20  ], [0.0, 1.77], 
+000247c0: 5b2d 332e 3534 2c20 332e 3534 5d5d 2c0a  [-3.54, 3.54]],.
+000247d0: 2020 2020 2020 2020 2020 2020 5b5b 332e              [[3.
+000247e0: 3534 2c20 332e 3534 5d2c 205b 302e 302c  54, 3.54], [0.0,
+000247f0: 2031 2e37 375d 2c20 5b2d 332e 3534 2c20   1.77], [-3.54, 
+00024800: 332e 3534 5d5d 2c0a 2020 2020 2020 2020  3.54]],.        
+00024810: 5d0a 2020 2020 2020 2020 706c 616e 655f  ].        plane_
+00024820: 6c69 7374 203d 205b 2258 5a22 2c20 2258  list = ["XZ", "X
+00024830: 5922 2c20 2259 5a22 2c20 2258 5a22 2c20  Y", "YZ", "XZ", 
+00024840: 2259 5a22 2c20 2258 5922 5d0a 2020 2020  "YZ", "XY"].    
+00024850: 2020 2020 6f66 6673 6574 5f6c 6973 7420      offset_list 
+00024860: 3d20 5b2d 332e 3534 2c20 332e 3534 2c20  = [-3.54, 3.54, 
+00024870: 332e 3534 2c20 332e 3534 2c20 2d33 2e35  3.54, 3.54, -3.5
+00024880: 342c 202d 332e 3534 5d0a 2020 2020 2020  4, -3.54].      
+00024890: 2020 6564 6765 5f77 6972 6520 3d20 280a    edge_wire = (.
+000248a0: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+000248b0: 706c 616e 6528 706c 616e 655f 6c69 7374  plane(plane_list
+000248c0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+000248d0: 202e 776f 726b 706c 616e 6528 6f66 6673   .workplane(offs
+000248e0: 6574 3d2d 6f66 6673 6574 5f6c 6973 745b  et=-offset_list[
+000248f0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+00024900: 2e73 706c 696e 6528 6564 6765 5f70 6f69  .spline(edge_poi
+00024910: 6e74 735b 305d 290a 2020 2020 2020 2020  nts[0]).        
+00024920: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+00024930: 696e 2072 616e 6765 286c 656e 2865 6467  in range(len(edg
+00024940: 655f 706f 696e 7473 2920 2d20 3129 3a0a  e_points) - 1):.
+00024950: 2020 2020 2020 2020 2020 2020 6564 6765              edge
+00024960: 5f77 6972 6520 3d20 6564 6765 5f77 6972  _wire = edge_wir
+00024970: 652e 6164 6428 0a20 2020 2020 2020 2020  e.add(.         
+00024980: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
+00024990: 2870 6c61 6e65 5f6c 6973 745b 6920 2b20  (plane_list[i + 
+000249a0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+000249b0: 2020 2020 2e77 6f72 6b70 6c61 6e65 286f      .workplane(o
+000249c0: 6666 7365 743d 2d6f 6666 7365 745f 6c69  ffset=-offset_li
+000249d0: 7374 5b69 202b 2031 5d29 0a20 2020 2020  st[i + 1]).     
+000249e0: 2020 2020 2020 2020 2020 202e 7370 6c69             .spli
+000249f0: 6e65 2865 6467 655f 706f 696e 7473 5b69  ne(edge_points[i
+00024a00: 202b 2031 5d29 0a20 2020 2020 2020 2020   + 1]).         
+00024a10: 2020 2029 0a20 2020 2020 2020 2073 7572     ).        sur
+00024a20: 6661 6365 5f70 6f69 6e74 7320 3d20 5b28  face_points = [(
+00024a30: 302c 2030 2c20 3029 5d0a 2020 2020 2020  0, 0, 0)].      
+00024a40: 2020 706c 6174 655f 3420 3d20 576f 726b    plate_4 = Work
+00024a50: 706c 616e 6528 2258 5922 292e 696e 7465  plane("XY").inte
+00024a60: 7270 506c 6174 6528 6564 6765 5f77 6972  rpPlate(edge_wir
+00024a70: 652c 2073 7572 6661 6365 5f70 6f69 6e74  e, surface_point
+00024a80: 732c 2074 6869 636b 6e65 7373 290a 2020  s, thickness).  
+00024a90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00024aa0: 7454 7275 6528 706c 6174 655f 342e 7661  tTrue(plate_4.va
+00024ab0: 6c28 292e 6973 5661 6c69 6428 2929 0a20  l().isValid()). 
+00024ac0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00024ad0: 7274 416c 6d6f 7374 4571 7561 6c28 706c  rtAlmostEqual(pl
+00024ae0: 6174 655f 342e 7661 6c28 292e 566f 6c75  ate_4.val().Volu
+00024af0: 6d65 2829 2c20 372e 3736 3035 3539 3439  me(), 7.76055949
+00024b00: 302c 2032 290a 0a20 2020 2020 2020 2070  0, 2)..        p
+00024b10: 6c61 7465 5f35 203d 2057 6f72 6b70 6c61  late_5 = Workpla
+00024b20: 6e65 2829 2e69 6e74 6572 7050 6c61 7465  ne().interpPlate
+00024b30: 2857 6f72 6b70 6c61 6e65 2829 2e73 6c6f  (Workplane().slo
+00024b40: 7432 4428 322c 2031 292e 7661 6c73 2829  t2D(2, 1).vals()
+00024b50: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00024b60: 7420 706c 6174 655f 352e 7661 6c28 292e  t plate_5.val().
+00024b70: 6973 5661 6c69 6428 290a 0a20 2020 2020  isValid()..     
+00024b80: 2020 2070 6c61 7465 5f36 203d 2053 6f6c     plate_6 = Sol
+00024b90: 6964 2e69 6e74 6572 7050 6c61 7465 280a  id.interpPlate(.
+00024ba0: 2020 2020 2020 2020 2020 2020 5b28 302c              [(0,
+00024bb0: 2030 2c20 3029 2c20 2831 2c20 302c 2030   0, 0), (1, 0, 0
+00024bc0: 292c 2028 312c 2031 2c20 3029 2c20 2830  ), (1, 1, 0), (0
+00024bd0: 2c20 312c 2030 295d 2c20 5b5d 2c20 7468  , 1, 0)], [], th
+00024be0: 6963 6b6e 6573 733d 310a 2020 2020 2020  ickness=1.      
+00024bf0: 2020 290a 0a20 2020 2020 2020 2061 7373    )..        ass
+00024c00: 6572 7420 706c 6174 655f 362e 6973 5661  ert plate_6.isVa
+00024c10: 6c69 6428 290a 2020 2020 2020 2020 7365  lid().        se
+00024c20: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
+00024c30: 7175 616c 2870 6c61 7465 5f36 2e56 6f6c  qual(plate_6.Vol
+00024c40: 756d 6528 292c 2031 2c20 3229 0a0a 2020  ume(), 1, 2)..  
+00024c50: 2020 6465 6620 7465 7374 5461 6e67 656e    def testTangen
+00024c60: 7441 7263 546f 506f 696e 7428 7365 6c66  tArcToPoint(self
+00024c70: 293a 0a0a 2020 2020 2020 2020 2320 6372  ):..        # cr
+00024c80: 6561 7465 2061 2073 696d 706c 6520 7368  eate a simple sh
+00024c90: 6170 6520 7769 7468 2074 616e 6765 6e74  ape with tangent
+00024ca0: 7320 6f66 2073 7472 6169 6768 7420 6564  s of straight ed
+00024cb0: 6765 7320 616e 6420 7365 6520 6966 2069  ges and see if i
+00024cc0: 7420 6861 7320 7468 6520 636f 7272 6563  t has the correc
+00024cd0: 7420 6172 6561 0a20 2020 2020 2020 2073  t area.        s
+00024ce0: 3020 3d20 280a 2020 2020 2020 2020 2020  0 = (.          
+00024cf0: 2020 576f 726b 706c 616e 6528 2258 5922    Workplane("XY"
+00024d00: 290a 2020 2020 2020 2020 2020 2020 2e68  ).            .h
+00024d10: 4c69 6e65 2831 290a 2020 2020 2020 2020  Line(1).        
+00024d20: 2020 2020 2e74 616e 6765 6e74 4172 6350      .tangentArcP
+00024d30: 6f69 6e74 2828 312c 2031 292c 2072 656c  oint((1, 1), rel
+00024d40: 6174 6976 653d 4661 6c73 6529 0a20 2020  ative=False).   
+00024d50: 2020 2020 2020 2020 202e 684c 696e 6554           .hLineT
+00024d60: 6f28 3029 0a20 2020 2020 2020 2020 2020  o(0).           
+00024d70: 202e 7461 6e67 656e 7441 7263 506f 696e   .tangentArcPoin
+00024d80: 7428 2830 2c20 3029 2c20 7265 6c61 7469  t((0, 0), relati
+00024d90: 7665 3d46 616c 7365 290a 2020 2020 2020  ve=False).      
+00024da0: 2020 2020 2020 2e63 6c6f 7365 2829 0a20        .close(). 
+00024db0: 2020 2020 2020 2020 2020 202e 6578 7472             .extr
+00024dc0: 7564 6528 3129 0a20 2020 2020 2020 2029  ude(1).        )
+00024dd0: 0a20 2020 2020 2020 2061 7265 6130 203d  .        area0 =
+00024de0: 2073 302e 6661 6365 7328 223e 5a22 292e   s0.faces(">Z").
+00024df0: 7661 6c28 292e 4172 6561 2829 0a20 2020  val().Area().   
+00024e00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00024e10: 416c 6d6f 7374 4571 7561 6c28 6172 6561  AlmostEqual(area
+00024e20: 302c 2028 3120 2b20 6d61 7468 2e70 6920  0, (1 + math.pi 
+00024e30: 2a20 302e 3520 2a2a 2032 292c 2034 290a  * 0.5 ** 2), 4).
+00024e40: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
+00024e50: 7265 6c61 7469 7665 2063 6f6f 7264 730a  relative coords.
+00024e60: 2020 2020 2020 2020 7331 203d 2028 0a20          s1 = (. 
+00024e70: 2020 2020 2020 2020 2020 2057 6f72 6b70             Workp
+00024e80: 6c61 6e65 2822 5859 2229 0a20 2020 2020  lane("XY").     
+00024e90: 2020 2020 2020 202e 684c 696e 6528 3129         .hLine(1)
+00024ea0: 0a20 2020 2020 2020 2020 2020 202e 7461  .            .ta
+00024eb0: 6e67 656e 7441 7263 506f 696e 7428 2830  ngentArcPoint((0
+00024ec0: 2c20 3129 2c20 7265 6c61 7469 7665 3d54  , 1), relative=T
+00024ed0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00024ee0: 202e 684c 696e 6554 6f28 3029 0a20 2020   .hLineTo(0).   
+00024ef0: 2020 2020 2020 2020 202e 7461 6e67 656e           .tangen
+00024f00: 7441 7263 506f 696e 7428 2830 2c20 2d31  tArcPoint((0, -1
+00024f10: 292c 2072 656c 6174 6976 653d 5472 7565  ), relative=True
+00024f20: 290a 2020 2020 2020 2020 2020 2020 2e63  ).            .c
+00024f30: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
+00024f40: 2020 202e 6578 7472 7564 6528 3129 0a20     .extrude(1). 
+00024f50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00024f60: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
+00024f70: 6541 6c6d 6f73 7445 7175 616c 7328 0a20  eAlmostEquals(. 
+00024f80: 2020 2020 2020 2020 2020 2073 312e 7661             s1.va
+00024f90: 6c28 292e 4365 6e74 6572 2829 2e74 6f54  l().Center().toT
+00024fa0: 7570 6c65 2829 2c20 7330 2e76 616c 2829  uple(), s0.val()
+00024fb0: 2e43 656e 7465 7228 292e 746f 5475 706c  .Center().toTupl
+00024fc0: 6528 292c 2034 0a20 2020 2020 2020 2029  e(), 4.        )
+00024fd0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00024fe0: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
+00024ff0: 7331 2e76 616c 2829 2e56 6f6c 756d 6528  s1.val().Volume(
+00025000: 292c 2073 302e 7661 6c28 292e 566f 6c75  ), s0.val().Volu
+00025010: 6d65 2829 2c20 3429 0a0a 2020 2020 2020  me(), 4)..      
+00025020: 2020 2320 636f 6e73 6563 7574 6976 6520    # consecutive 
+00025030: 7461 6e67 656e 7420 6172 6373 0a20 2020  tangent arcs.   
+00025040: 2020 2020 2073 3120 3d20 280a 2020 2020       s1 = (.    
+00025050: 2020 2020 2020 2020 576f 726b 706c 616e          Workplan
+00025060: 6528 2258 5922 290a 2020 2020 2020 2020  e("XY").        
+00025070: 2020 2020 2e76 4c69 6e65 2832 290a 2020      .vLine(2).  
+00025080: 2020 2020 2020 2020 2020 2e74 616e 6765            .tange
+00025090: 6e74 4172 6350 6f69 6e74 2828 312c 2030  ntArcPoint((1, 0
+000250a0: 2929 0a20 2020 2020 2020 2020 2020 202e  )).            .
+000250b0: 7461 6e67 656e 7441 7263 506f 696e 7428  tangentArcPoint(
+000250c0: 2831 2c20 3029 290a 2020 2020 2020 2020  (1, 0)).        
+000250d0: 2020 2020 2e74 616e 6765 6e74 4172 6350      .tangentArcP
+000250e0: 6f69 6e74 2828 312c 2030 2929 0a20 2020  oint((1, 0)).   
+000250f0: 2020 2020 2020 2020 202e 764c 696e 6528           .vLine(
+00025100: 2d32 290a 2020 2020 2020 2020 2020 2020  -2).            
+00025110: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00025120: 2020 2020 202e 6578 7472 7564 6528 3129       .extrude(1)
+00025130: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00025140: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+00025150: 6d6f 7374 4571 7561 6c28 0a20 2020 2020  mostEqual(.     
+00025160: 2020 2020 2020 2073 312e 6661 6365 7328         s1.faces(
+00025170: 223e 5a22 292e 7661 6c28 292e 4172 6561  ">Z").val().Area
+00025180: 2829 2c20 3220 2a20 3320 2b20 302e 3520  (), 2 * 3 + 0.5 
+00025190: 2a20 6d61 7468 2e70 6920 2a20 302e 3520  * math.pi * 0.5 
+000251a0: 2a2a 2032 2c20 340a 2020 2020 2020 2020  ** 2, 4.        
+000251b0: 290a 0a20 2020 2020 2020 2023 2074 616e  )..        # tan
+000251c0: 6765 6e74 4172 6320 6f6e 2074 6865 2065  gentArc on the e
+000251d0: 6e64 206f 6620 6120 7370 6c69 6e65 0a20  nd of a spline. 
+000251e0: 2020 2020 2020 2023 2073 706c 696e 6520         # spline 
+000251f0: 7769 6c6c 2062 6520 6120 7369 6d70 6c65  will be a simple
+00025200: 2061 7263 206f 6620 6120 6369 7263 6c65   arc of a circle
+00025210: 2c20 7468 656e 2066 696e 6973 6865 6420  , then finished 
+00025220: 6f66 6620 7769 7468 2061 0a20 2020 2020  off with a.     
+00025230: 2020 2023 2074 616e 6765 6e74 4172 6350     # tangentArcP
+00025240: 6f69 6e74 0a20 2020 2020 2020 2061 6e67  oint.        ang
+00025250: 6c65 7320 3d20 5b69 6478 202a 2031 2e35  les = [idx * 1.5
+00025260: 202a 206d 6174 682e 7069 202f 2031 3020   * math.pi / 10 
+00025270: 666f 7220 6964 7820 696e 2072 616e 6765  for idx in range
+00025280: 2831 3029 5d0a 2020 2020 2020 2020 7074  (10)].        pt
+00025290: 7320 3d20 5b28 6d61 7468 2e73 696e 2861  s = [(math.sin(a
+000252a0: 292c 206d 6174 682e 636f 7328 6129 2920  ), math.cos(a)) 
+000252b0: 666f 7220 6120 696e 2061 6e67 6c65 735d  for a in angles]
+000252c0: 0a20 2020 2020 2020 2073 3220 3d20 280a  .        s2 = (.
+000252d0: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+000252e0: 706c 616e 6528 2258 5922 290a 2020 2020  plane("XY").    
+000252f0: 2020 2020 2020 2020 2e73 706c 696e 6528          .spline(
+00025300: 7074 7329 0a20 2020 2020 2020 2020 2020  pts).           
+00025310: 202e 7461 6e67 656e 7441 7263 506f 696e   .tangentArcPoin
+00025320: 7428 2830 2c20 3129 2c20 7265 6c61 7469  t((0, 1), relati
+00025330: 7665 3d46 616c 7365 290a 2020 2020 2020  ve=False).      
+00025340: 2020 2020 2020 2e63 6c6f 7365 2829 0a20        .close(). 
+00025350: 2020 2020 2020 2020 2020 202e 6578 7472             .extr
+00025360: 7564 6528 3129 0a20 2020 2020 2020 2029  ude(1).        )
+00025370: 0a20 2020 2020 2020 2023 2076 6f6c 756d  .        # volum
+00025380: 6520 7368 6f75 6c64 2061 6c6d 6f73 7420  e should almost 
+00025390: 6265 2070 692c 2062 7574 206e 6f74 2061  be pi, but not a
+000253a0: 6363 7572 6174 656c 7920 6265 6361 7573  ccurately becaus
+000253b0: 6520 7765 206e 6565 6420 746f 0a20 2020  e we need to.   
+000253c0: 2020 2020 2023 2073 7461 7274 2077 6974       # start wit
+000253d0: 6820 6120 7370 6c69 6e65 0a20 2020 2020  h a spline.     
+000253e0: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+000253f0: 6d6f 7374 4571 7561 6c28 7332 2e76 616c  mostEqual(s2.val
+00025400: 2829 2e56 6f6c 756d 6528 292c 206d 6174  ().Volume(), mat
+00025410: 682e 7069 2c20 3129 0a20 2020 2020 2020  h.pi, 1).       
+00025420: 2023 2061 7373 6572 7420 6c6f 6361 6c20   # assert local 
+00025430: 636f 6f72 6473 2061 7265 206d 6170 7065  coords are mappe
+00025440: 6420 746f 2067 6c6f 6261 6c20 636f 7272  d to global corr
+00025450: 6563 746c 790a 2020 2020 2020 2020 6172  ectly.        ar
+00025460: 6330 203d 2057 6f72 6b70 6c61 6e65 2822  c0 = Workplane("
+00025470: 585a 222c 206f 7269 6769 6e3d 2831 2c20  XZ", origin=(1, 
+00025480: 312c 2031 2929 2e68 4c69 6e65 2831 292e  1, 1)).hLine(1).
+00025490: 7461 6e67 656e 7441 7263 506f 696e 7428  tangentArcPoint(
+000254a0: 2831 2c20 3129 292e 7661 6c28 290a 2020  (1, 1)).val().  
+000254b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000254c0: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
+000254d0: 6c73 2861 7263 302e 656e 6450 6f69 6e74  ls(arc0.endPoint
+000254e0: 2829 2e74 6f54 7570 6c65 2829 2c20 2833  ().toTuple(), (3
+000254f0: 2c20 312c 2032 292c 2034 290a 0a20 2020  , 1, 2), 4)..   
+00025500: 2020 2020 2023 2074 616e 6765 6e74 4172       # tangentAr
+00025510: 6350 6f69 6e74 2077 6974 6820 332d 7475  cPoint with 3-tu
+00025520: 706c 6520 6172 6775 6d65 6e74 0a20 2020  ple argument.   
+00025530: 2020 2020 2077 3020 3d20 576f 726b 706c       w0 = Workpl
+00025540: 616e 6528 2258 5922 292e 6c69 6e65 546f  ane("XY").lineTo
+00025550: 2831 2c20 3129 2e74 616e 6765 6e74 4172  (1, 1).tangentAr
+00025560: 6350 6f69 6e74 2828 312c 2031 2c20 3129  cPoint((1, 1, 1)
+00025570: 292e 7769 7265 2829 0a20 2020 2020 2020  ).wire().       
+00025580: 207a 6d61 7820 3d20 7730 2e76 616c 2829   zmax = w0.val()
+00025590: 2e42 6f75 6e64 696e 6742 6f78 2829 2e7a  .BoundingBox().z
+000255a0: 6d61 780a 2020 2020 2020 2020 7365 6c66  max.        self
+000255b0: 2e61 7373 6572 7441 6c6d 6f73 7445 7175  .assertAlmostEqu
+000255c0: 616c 287a 6d61 782c 2031 2c20 3129 0a0a  al(zmax, 1, 1)..
+000255d0: 2020 2020 6465 6620 7465 7374 5f66 696e      def test_fin
+000255e0: 6446 726f 6d45 6467 6528 7365 6c66 293a  dFromEdge(self):
+000255f0: 0a20 2020 2020 2020 2070 6172 7420 3d20  .        part = 
+00025600: 576f 726b 706c 616e 6528 2258 5922 2c20  Workplane("XY", 
+00025610: 6f72 6967 696e 3d28 312c 2031 2c20 3129  origin=(1, 1, 1)
+00025620: 292e 684c 696e 6528 3129 0a20 2020 2020  ).hLine(1).     
+00025630: 2020 2066 6f75 6e64 5f65 6467 6520 3d20     found_edge = 
+00025640: 7061 7274 2e5f 6669 6e64 4672 6f6d 4564  part._findFromEd
+00025650: 6765 2875 7365 4c6f 6361 6c43 6f6f 7264  ge(useLocalCoord
+00025660: 733d 4661 6c73 6529 0a20 2020 2020 2020  s=False).       
+00025670: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
+00025680: 6541 6c6d 6f73 7445 7175 616c 7328 666f  eAlmostEquals(fo
+00025690: 756e 645f 6564 6765 2e73 7461 7274 506f  und_edge.startPo
+000256a0: 696e 7428 292e 746f 5475 706c 6528 292c  int().toTuple(),
+000256b0: 2028 312c 2031 2c20 3129 2c20 3329 0a20   (1, 1, 1), 3). 
+000256c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000256d0: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
+000256e0: 616c 7328 666f 756e 645f 6564 6765 2e43  als(found_edge.C
+000256f0: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
+00025700: 292c 2028 312e 352c 2031 2c20 3129 2c20  ), (1.5, 1, 1), 
+00025710: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
+00025720: 6173 7365 7274 5475 706c 6541 6c6d 6f73  assertTupleAlmos
+00025730: 7445 7175 616c 7328 666f 756e 645f 6564  tEquals(found_ed
+00025740: 6765 2e65 6e64 506f 696e 7428 292e 746f  ge.endPoint().to
+00025750: 5475 706c 6528 292c 2028 322c 2031 2c20  Tuple(), (2, 1, 
+00025760: 3129 2c20 3329 0a20 2020 2020 2020 2066  1), 3).        f
+00025770: 6f75 6e64 5f65 6467 6520 3d20 7061 7274  ound_edge = part
+00025780: 2e5f 6669 6e64 4672 6f6d 4564 6765 2875  ._findFromEdge(u
+00025790: 7365 4c6f 6361 6c43 6f6f 7264 733d 5472  seLocalCoords=Tr
+000257a0: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
+000257b0: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
+000257c0: 7374 4571 7561 6c73 2866 6f75 6e64 5f65  stEquals(found_e
+000257d0: 6467 652e 656e 6450 6f69 6e74 2829 2e74  dge.endPoint().t
+000257e0: 6f54 7570 6c65 2829 2c20 2831 2c20 302c  oTuple(), (1, 0,
+000257f0: 2030 292c 2033 290a 2020 2020 2020 2020   0), 3).        
+00025800: 2320 6368 6563 6b20 5f66 696e 6446 726f  # check _findFro
+00025810: 6d45 6467 6520 6361 6e20 6669 6e64 2061  mEdge can find a
+00025820: 2073 706c 696e 650a 2020 2020 2020 2020   spline.        
+00025830: 7074 7320 3d20 5b28 302c 2030 292c 2028  pts = [(0, 0), (
+00025840: 302c 2031 292c 2028 312c 2032 292c 2028  0, 1), (1, 2), (
+00025850: 322c 2034 295d 0a20 2020 2020 2020 2073  2, 4)].        s
+00025860: 706c 696e 6530 203d 2057 6f72 6b70 6c61  pline0 = Workpla
+00025870: 6e65 2822 585a 2229 2e73 706c 696e 6528  ne("XZ").spline(
+00025880: 7074 7329 2e5f 6669 6e64 4672 6f6d 4564  pts)._findFromEd
+00025890: 6765 2829 0a20 2020 2020 2020 2073 656c  ge().        sel
+000258a0: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+000258b0: 6f73 7445 7175 616c 7328 2832 2c20 302c  ostEquals((2, 0,
+000258c0: 2034 292c 2073 706c 696e 6530 2e65 6e64   4), spline0.end
+000258d0: 506f 696e 7428 292e 746f 5475 706c 6528  Point().toTuple(
+000258e0: 292c 2033 290a 2020 2020 2020 2020 2320  ), 3).        # 
+000258f0: 6368 6563 6b20 6d65 7468 6f64 2066 6169  check method fai
+00025900: 6c73 2069 6620 6e6f 2065 6467 6520 6973  ls if no edge is
+00025910: 2070 7265 7365 6e74 0a20 2020 2020 2020   present.       
+00025920: 2070 6172 7432 203d 2057 6f72 6b70 6c61   part2 = Workpla
+00025930: 6e65 2822 5859 2229 2e62 6f78 2831 2c20  ne("XY").box(1, 
+00025940: 312c 2031 290a 2020 2020 2020 2020 7769  1, 1).        wi
+00025950: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+00025960: 6973 6573 2852 756e 7469 6d65 4572 726f  ises(RuntimeErro
+00025970: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00025980: 7061 7274 322e 5f66 696e 6446 726f 6d45  part2._findFromE
+00025990: 6467 6528 290a 2020 2020 2020 2020 7769  dge().        wi
+000259a0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+000259b0: 6973 6573 2852 756e 7469 6d65 4572 726f  ises(RuntimeErro
+000259c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000259d0: 7061 7274 322e 5f66 696e 6446 726f 6d45  part2._findFromE
+000259e0: 6467 6528 7573 654c 6f63 616c 436f 6f72  dge(useLocalCoor
+000259f0: 6473 3d54 7275 6529 0a0a 2020 2020 6465  ds=True)..    de
+00025a00: 6620 7465 7374 4d61 6b65 4865 6c69 7828  f testMakeHelix(
+00025a10: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+00025a20: 6820 3d20 3130 0a20 2020 2020 2020 2070  h = 10.        p
+00025a30: 6974 6368 203d 2031 2e35 0a20 2020 2020  itch = 1.5.     
+00025a40: 2020 2072 203d 2031 2e32 0a20 2020 2020     r = 1.2.     
+00025a50: 2020 206f 626a 203d 2057 6972 652e 6d61     obj = Wire.ma
+00025a60: 6b65 4865 6c69 7828 7069 7463 682c 2068  keHelix(pitch, h
+00025a70: 2c20 7229 0a0a 2020 2020 2020 2020 6262  , r)..        bb
+00025a80: 203d 206f 626a 2e42 6f75 6e64 696e 6742   = obj.BoundingB
+00025a90: 6f78 2829 0a20 2020 2020 2020 2073 656c  ox().        sel
+00025aa0: 662e 6173 7365 7274 416c 6d6f 7374 4571  f.assertAlmostEq
+00025ab0: 7561 6c28 6262 2e7a 6c65 6e2c 2068 2c20  ual(bb.zlen, h, 
+00025ac0: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
+00025ad0: 556e 696f 6e43 6f6d 706f 756e 6428 7365  UnionCompound(se
+00025ae0: 6c66 293a 0a0a 2020 2020 2020 2020 626f  lf):..        bo
+00025af0: 7831 203d 2057 6f72 6b70 6c61 6e65 2822  x1 = Workplane("
+00025b00: 5859 2229 2e62 6f78 2831 302c 2032 302c  XY").box(10, 20,
+00025b10: 2033 3029 0a20 2020 2020 2020 2062 6f78   30).        box
+00025b20: 3220 3d20 576f 726b 706c 616e 6528 2259  2 = Workplane("Y
+00025b30: 5a22 292e 626f 7828 3130 2c20 3230 2c20  Z").box(10, 20, 
+00025b40: 3330 290a 2020 2020 2020 2020 7368 6170  30).        shap
+00025b50: 655f 746f 5f63 7574 203d 2057 6f72 6b70  e_to_cut = Workp
+00025b60: 6c61 6e65 2822 5859 2229 2e62 6f78 2831  lane("XY").box(1
+00025b70: 352c 2031 352c 2031 3529 2e74 7261 6e73  5, 15, 15).trans
+00025b80: 6c61 7465 2828 382c 2038 2c20 3829 290a  late((8, 8, 8)).
+00025b90: 0a20 2020 2020 2020 206c 6973 745f 6f66  .        list_of
+00025ba0: 5f73 6861 7065 7320 3d20 5b5d 0a20 2020  _shapes = [].   
+00025bb0: 2020 2020 2066 6f72 206f 2069 6e20 626f       for o in bo
+00025bc0: 7831 2e61 6c6c 2829 3a0a 2020 2020 2020  x1.all():.      
+00025bd0: 2020 2020 2020 6c69 7374 5f6f 665f 7368        list_of_sh
+00025be0: 6170 6573 2e65 7874 656e 6428 6f2e 7661  apes.extend(o.va
+00025bf0: 6c73 2829 290a 2020 2020 2020 2020 666f  ls()).        fo
+00025c00: 7220 6f20 696e 2062 6f78 322e 616c 6c28  r o in box2.all(
+00025c10: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00025c20: 6973 745f 6f66 5f73 6861 7065 732e 6578  ist_of_shapes.ex
+00025c30: 7465 6e64 286f 2e76 616c 7328 2929 0a0a  tend(o.vals())..
+00025c40: 2020 2020 2020 2020 6f62 6a20 3d20 576f          obj = Wo
+00025c50: 726b 706c 616e 6528 2258 5922 292e 6e65  rkplane("XY").ne
+00025c60: 774f 626a 6563 7428 6c69 7374 5f6f 665f  wObject(list_of_
+00025c70: 7368 6170 6573 292e 6375 7428 7368 6170  shapes).cut(shap
+00025c80: 655f 746f 5f63 7574 290a 0a20 2020 2020  e_to_cut)..     
+00025c90: 2020 2061 7373 6572 7420 6f62 6a2e 7661     assert obj.va
+00025ca0: 6c28 292e 6973 5661 6c69 6428 290a 0a20  l().isValid().. 
+00025cb0: 2020 2064 6566 2074 6573 7453 6563 7469     def testSecti
+00025cc0: 6f6e 2873 656c 6629 3a0a 0a20 2020 2020  on(self):..     
+00025cd0: 2020 2062 6f78 203d 2057 6f72 6b70 6c61     box = Workpla
+00025ce0: 6e65 2822 5859 222c 206f 7269 6769 6e3d  ne("XY", origin=
+00025cf0: 2831 2c20 322c 2033 2929 2e62 6f78 2831  (1, 2, 3)).box(1
+00025d00: 2c20 312c 2031 290a 0a20 2020 2020 2020  , 1, 1)..       
+00025d10: 2073 3120 3d20 626f 782e 7365 6374 696f   s1 = box.sectio
+00025d20: 6e28 290a 2020 2020 2020 2020 7332 203d  n().        s2 =
+00025d30: 2062 6f78 2e73 6563 7469 6f6e 2830 2e35   box.section(0.5
+00025d40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00025d50: 6173 7365 7274 416c 6d6f 7374 4571 7561  assertAlmostEqua
+00025d60: 6c28 7331 2e66 6163 6573 2829 2e76 616c  l(s1.faces().val
+00025d70: 2829 2e41 7265 6128 292c 2031 290a 2020  ().Area(), 1).  
+00025d80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00025d90: 7441 6c6d 6f73 7445 7175 616c 2873 322e  tAlmostEqual(s2.
+00025da0: 6661 6365 7328 292e 7661 6c28 292e 4172  faces().val().Ar
+00025db0: 6561 2829 2c20 3129 0a0a 2020 2020 2020  ea(), 1)..      
+00025dc0: 2020 6c69 6e65 203d 2057 6f72 6b70 6c61    line = Workpla
+00025dd0: 6e65 2822 5859 2229 2e68 4c69 6e65 2831  ne("XY").hLine(1
+00025de0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00025df0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00025e00: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
+00025e10: 2020 2020 2020 2020 2020 206c 696e 652e             line.
+00025e20: 7365 6374 696f 6e28 290a 0a20 2020 2064  section()..    d
+00025e30: 6566 2074 6573 7447 6c75 6528 7365 6c66  ef testGlue(self
+00025e40: 293a 0a0a 2020 2020 2020 2020 626f 7831  ):..        box1
+00025e50: 203d 2057 6f72 6b70 6c61 6e65 2822 5859   = Workplane("XY
+00025e60: 2229 2e72 6563 7428 312c 2031 292e 6578  ").rect(1, 1).ex
+00025e70: 7472 7564 6528 3229 0a20 2020 2020 2020  trude(2).       
+00025e80: 2062 6f78 3220 3d20 576f 726b 706c 616e   box2 = Workplan
+00025e90: 6528 2258 5922 2c20 6f72 6967 696e 3d28  e("XY", origin=(
+00025ea0: 302c 2031 2c20 3029 292e 7265 6374 2831  0, 1, 0)).rect(1
+00025eb0: 2c20 3129 2e65 7874 7275 6465 2831 290a  , 1).extrude(1).
+00025ec0: 2020 2020 2020 2020 7265 7320 3d20 626f          res = bo
+00025ed0: 7831 2e75 6e69 6f6e 2862 6f78 322c 2067  x1.union(box2, g
+00025ee0: 6c75 653d 5472 7565 290a 0a20 2020 2020  lue=True)..     
+00025ef0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00025f00: 7561 6c28 7265 732e 6661 6365 7328 292e  ual(res.faces().
+00025f10: 7369 7a65 2829 2c20 3829 0a0a 2020 2020  size(), 8)..    
+00025f20: 2020 2020 6f62 6a20 3d20 6f62 6a20 3d20      obj = obj = 
+00025f30: 280a 2020 2020 2020 2020 2020 2020 576f  (.            Wo
+00025f40: 726b 706c 616e 6528 2258 5922 292e 7265  rkplane("XY").re
+00025f50: 6374 2831 2c20 3129 2e65 7874 7275 6465  ct(1, 1).extrude
+00025f60: 2832 292e 6d6f 7665 546f 2830 2c20 3229  (2).moveTo(0, 2)
+00025f70: 2e72 6563 7428 312c 2031 292e 6578 7472  .rect(1, 1).extr
+00025f80: 7564 6528 3229 0a20 2020 2020 2020 2029  ude(2).        )
+00025f90: 0a20 2020 2020 2020 2072 6573 203d 206f  .        res = o
+00025fa0: 626a 2e75 6e69 6f6e 2862 6f78 322c 2067  bj.union(box2, g
+00025fb0: 6c75 653d 5472 7565 290a 0a20 2020 2020  lue=True)..     
+00025fc0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00025fd0: 7561 6c28 7265 732e 6661 6365 7328 292e  ual(res.faces().
+00025fe0: 7369 7a65 2829 2c20 3130 290a 0a20 2020  size(), 10)..   
+00025ff0: 2064 6566 2074 6573 7446 757a 7a79 426f   def testFuzzyBo
+00026000: 6f6c 4f70 2873 656c 6629 3a0a 0a20 2020  olOp(self):..   
+00026010: 2020 2020 2065 7073 203d 2031 652d 330a       eps = 1e-3.
+00026020: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
+00026030: 6675 7365 0a20 2020 2020 2020 2062 6f78  fuse.        box
+00026040: 3120 3d20 576f 726b 706c 616e 6528 2258  1 = Workplane("X
+00026050: 5922 292e 626f 7828 312c 2031 2c20 3129  Y").box(1, 1, 1)
+00026060: 0a20 2020 2020 2020 2062 6f78 3220 3d20  .        box2 = 
+00026070: 576f 726b 706c 616e 6528 2258 5922 2c20  Workplane("XY", 
+00026080: 6f72 6967 696e 3d28 3120 2b20 6570 732c  origin=(1 + eps,
+00026090: 2030 2e30 2929 2e62 6f78 2831 2c20 312c   0.0)).box(1, 1,
+000260a0: 2031 290a 2020 2020 2020 2020 626f 7833   1).        box3
+000260b0: 203d 2057 6f72 6b70 6c61 6e65 2822 5859   = Workplane("XY
+000260c0: 222c 206f 7269 6769 6e3d 2832 2c20 302c  ", origin=(2, 0,
+000260d0: 2030 2929 2e62 6f78 2831 2c20 312c 2031   0)).box(1, 1, 1
+000260e0: 290a 0a20 2020 2020 2020 2072 6573 203d  )..        res =
+000260f0: 2062 6f78 312e 756e 696f 6e28 626f 7832   box1.union(box2
+00026100: 290a 2020 2020 2020 2020 7265 735f 6675  ).        res_fu
+00026110: 7a7a 7920 3d20 626f 7831 2e75 6e69 6f6e  zzy = box1.union
+00026120: 2862 6f78 322c 2074 6f6c 3d65 7073 290a  (box2, tol=eps).
+00026130: 2020 2020 2020 2020 7265 735f 6675 7a7a          res_fuzz
+00026140: 7932 203d 2062 6f78 312e 756e 696f 6e28  y2 = box1.union(
+00026150: 626f 7833 292e 756e 696f 6e28 626f 7832  box3).union(box2
+00026160: 2c20 746f 6c3d 6570 7329 0a0a 2020 2020  , tol=eps)..    
+00026170: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00026180: 7175 616c 2872 6573 2e73 6f6c 6964 7328  qual(res.solids(
+00026190: 292e 7369 7a65 2829 2c20 3229 0a20 2020  ).size(), 2).   
+000261a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000261b0: 4571 7561 6c28 7265 735f 6675 7a7a 792e  Equal(res_fuzzy.
+000261c0: 736f 6c69 6473 2829 2e73 697a 6528 292c  solids().size(),
+000261d0: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+000261e0: 2e61 7373 6572 7445 7175 616c 2872 6573  .assertEqual(res
+000261f0: 5f66 757a 7a79 322e 736f 6c69 6473 2829  _fuzzy2.solids()
+00026200: 2e73 697a 6528 292c 2031 290a 0a20 2020  .size(), 1)..   
+00026210: 2020 2020 2023 2074 6573 7420 6375 7420       # test cut 
+00026220: 616e 6420 696e 7465 7273 6563 740a 2020  and intersect.  
+00026230: 2020 2020 2020 626f 7834 203d 2057 6f72        box4 = Wor
+00026240: 6b70 6c61 6e65 2822 5859 222c 206f 7269  kplane("XY", ori
+00026250: 6769 6e3d 2865 7073 2c20 302e 3029 292e  gin=(eps, 0.0)).
+00026260: 626f 7828 312c 2031 2c20 3129 0a0a 2020  box(1, 1, 1)..  
+00026270: 2020 2020 2020 7265 735f 6675 7a7a 795f        res_fuzzy_
+00026280: 6375 7420 3d20 626f 7831 2e63 7574 2862  cut = box1.cut(b
+00026290: 6f78 342c 2074 6f6c 3d65 7073 290a 2020  ox4, tol=eps).  
+000262a0: 2020 2020 2020 7265 735f 6675 7a7a 795f        res_fuzzy_
+000262b0: 696e 7465 7273 6563 7420 3d20 626f 7831  intersect = box1
+000262c0: 2e69 6e74 6572 7365 6374 2862 6f78 342c  .intersect(box4,
+000262d0: 2074 6f6c 3d65 7073 290a 0a20 2020 2020   tol=eps)..     
+000262e0: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+000262f0: 6d6f 7374 4571 7561 6c28 7265 735f 6675  mostEqual(res_fu
+00026300: 7a7a 795f 6375 742e 7661 6c28 292e 566f  zzy_cut.val().Vo
+00026310: 6c75 6d65 2829 2c20 3029 0a20 2020 2020  lume(), 0).     
+00026320: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+00026330: 6d6f 7374 4571 7561 6c28 7265 735f 6675  mostEqual(res_fu
+00026340: 7a7a 795f 696e 7465 7273 6563 742e 7661  zzy_intersect.va
+00026350: 6c28 292e 566f 6c75 6d65 2829 2c20 3129  l().Volume(), 1)
+00026360: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
+00026370: 2077 6974 6820 636f 6d70 6f75 6e64 730a   with compounds.
+00026380: 2020 2020 2020 2020 626f 7831 5f63 6d70          box1_cmp
+00026390: 203d 2043 6f6d 706f 756e 642e 6d61 6b65   = Compound.make
+000263a0: 436f 6d70 6f75 6e64 2862 6f78 312e 7661  Compound(box1.va
+000263b0: 6c73 2829 290a 2020 2020 2020 2020 626f  ls()).        bo
+000263c0: 7834 5f63 6d70 203d 2043 6f6d 706f 756e  x4_cmp = Compoun
+000263d0: 642e 6d61 6b65 436f 6d70 6f75 6e64 2862  d.makeCompound(b
+000263e0: 6f78 342e 7661 6c73 2829 290a 0a20 2020  ox4.vals())..   
+000263f0: 2020 2020 2072 6573 5f66 757a 7a79 5f63       res_fuzzy_c
+00026400: 7574 5f63 6d70 203d 2062 6f78 315f 636d  ut_cmp = box1_cm
+00026410: 702e 6375 7428 626f 7834 5f63 6d70 2c20  p.cut(box4_cmp, 
+00026420: 746f 6c3d 6570 7329 0a20 2020 2020 2020  tol=eps).       
+00026430: 2072 6573 5f66 757a 7a79 5f69 6e74 6572   res_fuzzy_inter
+00026440: 7365 6374 5f63 6d70 203d 2062 6f78 315f  sect_cmp = box1_
+00026450: 636d 702e 696e 7465 7273 6563 7428 626f  cmp.intersect(bo
+00026460: 7834 5f63 6d70 2c20 746f 6c3d 6570 7329  x4_cmp, tol=eps)
+00026470: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00026480: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
+00026490: 2872 6573 5f66 757a 7a79 5f63 7574 5f63  (res_fuzzy_cut_c
+000264a0: 6d70 2e56 6f6c 756d 6528 292c 2030 290a  mp.Volume(), 0).
+000264b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000264c0: 6572 7441 6c6d 6f73 7445 7175 616c 2872  ertAlmostEqual(r
+000264d0: 6573 5f66 757a 7a79 5f69 6e74 6572 7365  es_fuzzy_interse
+000264e0: 6374 5f63 6d70 2e56 6f6c 756d 6528 292c  ct_cmp.Volume(),
+000264f0: 2031 290a 0a20 2020 2020 2020 2023 2074   1)..        # t
+00026500: 6573 7420 7769 7468 2073 6f6c 6964 730a  est with solids.
+00026510: 2020 2020 2020 2020 7265 735f 6675 7a7a          res_fuzz
+00026520: 795f 6375 745f 7661 6c20 3d20 626f 7831  y_cut_val = box1
+00026530: 2e76 616c 2829 2e63 7574 2862 6f78 342e  .val().cut(box4.
+00026540: 7661 6c28 292c 2074 6f6c 3d65 7073 290a  val(), tol=eps).
+00026550: 2020 2020 2020 2020 7265 735f 6675 7a7a          res_fuzz
+00026560: 795f 696e 7465 7273 6563 745f 7661 6c20  y_intersect_val 
+00026570: 3d20 626f 7831 2e76 616c 2829 2e69 6e74  = box1.val().int
+00026580: 6572 7365 6374 2862 6f78 342e 7661 6c28  ersect(box4.val(
+00026590: 292c 2074 6f6c 3d65 7073 290a 0a20 2020  ), tol=eps)..   
+000265a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000265b0: 416c 6d6f 7374 4571 7561 6c28 7265 735f  AlmostEqual(res_
+000265c0: 6675 7a7a 795f 6375 745f 7661 6c2e 566f  fuzzy_cut_val.Vo
+000265d0: 6c75 6d65 2829 2c20 3029 0a20 2020 2020  lume(), 0).     
+000265e0: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+000265f0: 6d6f 7374 4571 7561 6c28 7265 735f 6675  mostEqual(res_fu
+00026600: 7a7a 795f 696e 7465 7273 6563 745f 7661  zzy_intersect_va
+00026610: 6c2e 566f 6c75 6d65 2829 2c20 3129 0a0a  l.Volume(), 1)..
+00026620: 2020 2020 6465 6620 7465 7374 4c6f 6361      def testLoca
+00026630: 7465 644d 6f76 6564 2873 656c 6629 3a0a  tedMoved(self):.
+00026640: 0a20 2020 2020 2020 2062 6f78 203d 2053  .        box = S
+00026650: 6f6c 6964 2e6d 616b 6542 6f78 2831 2c20  olid.makeBox(1, 
+00026660: 312c 2031 2c20 5665 6374 6f72 282d 302e  1, 1, Vector(-0.
+00026670: 352c 202d 302e 352c 202d 302e 3529 290a  5, -0.5, -0.5)).
+00026680: 2020 2020 2020 2020 6c6f 6320 3d20 4c6f          loc = Lo
+00026690: 6361 7469 6f6e 2856 6563 746f 7228 312c  cation(Vector(1,
+000266a0: 2031 2c20 3129 290a 0a20 2020 2020 2020   1, 1))..       
+000266b0: 2062 6f78 3120 3d20 626f 782e 6c6f 6361   box1 = box.loca
+000266c0: 7465 6428 6c6f 6329 0a0a 2020 2020 2020  ted(loc)..      
+000266d0: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
+000266e0: 6c65 416c 6d6f 7374 4571 7561 6c73 2862  leAlmostEquals(b
+000266f0: 6f78 312e 4365 6e74 6572 2829 2e74 6f54  ox1.Center().toT
+00026700: 7570 6c65 2829 2c20 2831 2c20 312c 2031  uple(), (1, 1, 1
+00026710: 292c 2036 290a 2020 2020 2020 2020 7365  ), 6).        se
+00026720: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
+00026730: 6d6f 7374 4571 7561 6c73 2862 6f78 2e43  mostEquals(box.C
+00026740: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
+00026750: 292c 2028 302c 2030 2c20 3029 2c20 3629  ), (0, 0, 0), 6)
+00026760: 0a0a 2020 2020 2020 2020 626f 782e 6c6f  ..        box.lo
+00026770: 6361 7465 286c 6f63 290a 0a20 2020 2020  cate(loc)..     
+00026780: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
+00026790: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
+000267a0: 626f 782e 4365 6e74 6572 2829 2e74 6f54  box.Center().toT
+000267b0: 7570 6c65 2829 2c20 2831 2c20 312c 2031  uple(), (1, 1, 1
+000267c0: 292c 2036 290a 0a20 2020 2020 2020 2062  ), 6)..        b
+000267d0: 6f78 3220 3d20 626f 782e 6d6f 7665 6428  ox2 = box.moved(
+000267e0: 6c6f 6329 0a0a 2020 2020 2020 2020 7365  loc)..        se
+000267f0: 6c66 2e61 7373 6572 7454 7570 6c65 416c  lf.assertTupleAl
+00026800: 6d6f 7374 4571 7561 6c73 2862 6f78 2e43  mostEquals(box.C
+00026810: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
+00026820: 292c 2028 312c 2031 2c20 3129 2c20 3629  ), (1, 1, 1), 6)
+00026830: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00026840: 7365 7274 5475 706c 6541 6c6d 6f73 7445  sertTupleAlmostE
+00026850: 7175 616c 7328 626f 7832 2e43 656e 7465  quals(box2.Cente
+00026860: 7228 292e 746f 5475 706c 6528 292c 2028  r().toTuple(), (
+00026870: 322c 2032 2c20 3229 2c20 3629 0a0a 2020  2, 2, 2), 6)..  
+00026880: 2020 2020 2020 626f 782e 6d6f 7665 286c        box.move(l
+00026890: 6f63 290a 0a20 2020 2020 2020 2073 656c  oc)..        sel
+000268a0: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+000268b0: 6f73 7445 7175 616c 7328 626f 782e 4365  ostEquals(box.Ce
+000268c0: 6e74 6572 2829 2e74 6f54 7570 6c65 2829  nter().toTuple()
+000268d0: 2c20 2832 2c20 322c 2032 292c 2036 290a  , (2, 2, 2), 6).
+000268e0: 0a20 2020 2064 6566 2074 6573 744e 756c  .    def testNul
+000268f0: 6c53 6861 7065 2873 656c 6629 3a0a 0a20  lShape(self):.. 
+00026900: 2020 2020 2020 2066 726f 6d20 4f43 502e         from OCP.
+00026910: 546f 706f 4453 2069 6d70 6f72 7420 546f  TopoDS import To
+00026920: 706f 4453 5f53 6861 7065 0a0a 2020 2020  poDS_Shape..    
+00026930: 2020 2020 7320 3d20 546f 706f 4453 5f53      s = TopoDS_S
+00026940: 6861 7065 2829 0a0a 2020 2020 2020 2020  hape()..        
+00026950: 2320 6d61 6b65 2073 7572 6520 7261 6973  # make sure rais
+00026960: 6573 206f 6e20 6e6f 6e20 736f 6c69 640a  es on non solid.
+00026970: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00026980: 662e 6173 7365 7274 5261 6973 6573 2856  f.assertRaises(V
+00026990: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
+000269a0: 2020 2020 2020 2020 7220 3d20 6f63 635f          r = occ_
+000269b0: 696d 706c 2e73 6861 7065 732e 646f 776e  impl.shapes.down
+000269c0: 6361 7374 2873 290a 0a20 2020 2064 6566  cast(s)..    def
+000269d0: 2074 6573 7443 656e 7465 724f 6642 6f75   testCenterOfBou
+000269e0: 6e64 426f 7828 7365 6c66 293a 0a0a 2020  ndBox(self):..  
+000269f0: 2020 2020 2020 6f62 6a20 3d20 576f 726b        obj = Work
+00026a00: 706c 616e 6528 292e 7075 7368 506f 696e  plane().pushPoin
+00026a10: 7473 285b 2830 2c20 3029 2c20 2832 2c20  ts([(0, 0), (2, 
+00026a20: 3229 5d29 2e62 6f78 2831 2c20 312c 2031  2)]).box(1, 1, 1
+00026a30: 290a 2020 2020 2020 2020 6320 3d20 6f62  ).        c = ob
+00026a40: 6a2e 776f 726b 706c 616e 6528 6365 6e74  j.workplane(cent
+00026a50: 6572 4f70 7469 6f6e 3d22 4365 6e74 6572  erOption="Center
+00026a60: 4f66 426f 756e 6442 6f78 2229 2e70 6c61  OfBoundBox").pla
+00026a70: 6e65 2e6f 7269 6769 6e0a 0a20 2020 2020  ne.origin..     
+00026a80: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
+00026a90: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
+00026aa0: 632e 746f 5475 706c 6528 292c 2028 312c  c.toTuple(), (1,
+00026ab0: 2031 2c20 3029 2c20 3629 0a0a 2020 2020   1, 0), 6)..    
+00026ac0: 6465 6620 7465 7374 4f66 6673 6574 3244  def testOffset2D
+00026ad0: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
+00026ae0: 2077 3120 3d20 576f 726b 706c 616e 6528   w1 = Workplane(
+00026af0: 292e 7265 6374 2831 2c20 3129 2e6f 6666  ).rect(1, 1).off
+00026b00: 7365 7432 4428 302e 352c 2022 6172 6322  set2D(0.5, "arc"
+00026b10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00026b20: 7373 6572 7445 7175 616c 2877 312e 6564  ssertEqual(w1.ed
+00026b30: 6765 7328 292e 7369 7a65 2829 2c20 3829  ges().size(), 8)
+00026b40: 0a0a 2020 2020 2020 2020 7732 203d 2057  ..        w2 = W
+00026b50: 6f72 6b70 6c61 6e65 2829 2e72 6563 7428  orkplane().rect(
+00026b60: 312c 2031 292e 6f66 6673 6574 3244 2830  1, 1).offset2D(0
+00026b70: 2e35 2c20 2274 616e 6765 6e74 2229 0a20  .5, "tangent"). 
+00026b80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00026b90: 7274 4571 7561 6c28 7732 2e65 6467 6573  rtEqual(w2.edges
+00026ba0: 2829 2e73 697a 6528 292c 2034 290a 0a20  ().size(), 4).. 
+00026bb0: 2020 2020 2020 2077 3320 3d20 576f 726b         w3 = Work
+00026bc0: 706c 616e 6528 292e 7265 6374 2831 2c20  plane().rect(1, 
+00026bd0: 3129 2e6f 6666 7365 7432 4428 302e 352c  1).offset2D(0.5,
+00026be0: 2022 696e 7465 7273 6563 7469 6f6e 2229   "intersection")
+00026bf0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00026c00: 7365 7274 4571 7561 6c28 7733 2e65 6467  sertEqual(w3.edg
+00026c10: 6573 2829 2e73 697a 6528 292c 2034 290a  es().size(), 4).
+00026c20: 0a20 2020 2020 2020 2077 3420 3d20 576f  .        w4 = Wo
+00026c30: 726b 706c 616e 6528 292e 7075 7368 506f  rkplane().pushPo
+00026c40: 696e 7473 285b 2830 2c20 3029 2c20 2830  ints([(0, 0), (0
+00026c50: 2c20 3529 5d29 2e72 6563 7428 312c 2031  , 5)]).rect(1, 1
+00026c60: 292e 6f66 6673 6574 3244 282d 302e 3529  ).offset2D(-0.5)
+00026c70: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00026c80: 7365 7274 4571 7561 6c28 7734 2e77 6972  sertEqual(w4.wir
+00026c90: 6573 2829 2e73 697a 6528 292c 2030 290a  es().size(), 0).
+00026ca0: 0a20 2020 2020 2020 2077 3520 3d20 576f  .        w5 = Wo
+00026cb0: 726b 706c 616e 6528 292e 7075 7368 506f  rkplane().pushPo
+00026cc0: 696e 7473 285b 2830 2c20 3029 2c20 2830  ints([(0, 0), (0
+00026cd0: 2c20 3529 5d29 2e72 6563 7428 312c 2031  , 5)]).rect(1, 1
+00026ce0: 292e 6f66 6673 6574 3244 282d 302e 3235  ).offset2D(-0.25
+00026cf0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00026d00: 7373 6572 7445 7175 616c 2877 352e 7769  ssertEqual(w5.wi
+00026d10: 7265 7328 292e 7369 7a65 2829 2c20 3229  res().size(), 2)
+00026d20: 0a0a 2020 2020 2020 2020 7220 3d20 3230  ..        r = 20
+00026d30: 0a20 2020 2020 2020 2073 203d 2037 0a20  .        s = 7. 
+00026d40: 2020 2020 2020 2074 203d 2031 2e35 0a0a         t = 1.5..
+00026d50: 2020 2020 2020 2020 706f 696e 7473 203d          points =
+00026d60: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
+00026d70: 302c 2074 202f 2032 292c 0a20 2020 2020  0, t / 2),.     
+00026d80: 2020 2020 2020 2028 7220 2f20 3220 2d20         (r / 2 - 
+00026d90: 312e 3520 2a20 742c 2072 202f 2032 202d  1.5 * t, r / 2 -
+00026da0: 2074 292c 0a20 2020 2020 2020 2020 2020   t),.           
+00026db0: 2028 7320 2f20 322c 2072 202f 2032 202d   (s / 2, r / 2 -
+00026dc0: 2074 292c 0a20 2020 2020 2020 2020 2020   t),.           
+00026dd0: 2028 7320 2f20 322c 2072 202f 2032 292c   (s / 2, r / 2),
+00026de0: 0a20 2020 2020 2020 2020 2020 2028 7220  .            (r 
+00026df0: 2f20 322c 2072 202f 2032 292c 0a20 2020  / 2, r / 2),.   
+00026e00: 2020 2020 2020 2020 2028 7220 2f20 322c           (r / 2,
+00026e10: 2073 202f 2032 292c 0a20 2020 2020 2020   s / 2),.       
+00026e20: 2020 2020 2028 7220 2f20 3220 2d20 742c       (r / 2 - t,
+00026e30: 2073 202f 2032 292c 0a20 2020 2020 2020   s / 2),.       
+00026e40: 2020 2020 2028 7220 2f20 3220 2d20 742c       (r / 2 - t,
+00026e50: 2072 202f 2032 202d 2031 2e35 202a 2074   r / 2 - 1.5 * t
+00026e60: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00026e70: 7420 2f20 322c 2030 292c 0a20 2020 2020  t / 2, 0),.     
+00026e80: 2020 205d 0a0a 2020 2020 2020 2020 7320     ]..        s 
+00026e90: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00026ea0: 576f 726b 706c 616e 6528 2258 5922 290a  Workplane("XY").
+00026eb0: 2020 2020 2020 2020 2020 2020 2e70 6f6c              .pol
+00026ec0: 796c 696e 6528 706f 696e 7473 290a 2020  yline(points).  
+00026ed0: 2020 2020 2020 2020 2020 2e6d 6972 726f            .mirro
+00026ee0: 7258 2829 0a20 2020 2020 2020 2020 2020  rX().           
+00026ef0: 202e 6d69 7272 6f72 5928 290a 2020 2020   .mirrorY().    
+00026f00: 2020 2020 2020 2020 2e6f 6666 7365 7432          .offset2
+00026f10: 4428 2d30 2e39 290a 2020 2020 2020 2020  D(-0.9).        
+00026f20: 2020 2020 2e65 7874 7275 6465 2831 290a      .extrude(1).
+00026f30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00026f40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00026f50: 616c 2873 2e73 6f6c 6964 7328 292e 7369  al(s.solids().si
+00026f60: 7a65 2829 2c20 3429 0a0a 2020 2020 2020  ze(), 4)..      
+00026f70: 2020 2320 7465 7374 2066 6f72 436f 6e73    # test forCons
+00026f80: 7472 7563 7469 6f6e 0a20 2020 2020 2020  truction.       
+00026f90: 2023 2066 6f72 436f 6e73 7472 7563 7469   # forConstructi
+00026fa0: 6f6e 3d54 7275 6520 7368 6f75 6c64 2070  on=True should p
+00026fb0: 6c61 6365 2072 6573 756c 7473 2069 6e20  lace results in 
+00026fc0: 6f62 6a65 6374 732c 206e 6f74 2063 7478  objects, not ctx
+00026fd0: 2e70 656e 6469 6e67 5769 7265 730a 2020  .pendingWires.  
+00026fe0: 2020 2020 2020 7736 203d 2057 6f72 6b70        w6 = Workp
+00026ff0: 6c61 6e65 2829 2e68 4c69 6e65 2831 292e  lane().hLine(1).
+00027000: 764c 696e 6528 3129 2e63 6c6f 7365 2829  vLine(1).close()
+00027010: 2e6f 6666 7365 7432 4428 302e 352c 2066  .offset2D(0.5, f
+00027020: 6f72 436f 6e73 7472 7563 7469 6f6e 3d54  orConstruction=T
+00027030: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
+00027040: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00027050: 6e28 7736 2e63 7478 2e70 656e 6469 6e67  n(w6.ctx.pending
+00027060: 5769 7265 7329 2c20 3029 0a20 2020 2020  Wires), 0).     
+00027070: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00027080: 7561 6c28 7736 2e73 697a 6528 292c 2031  ual(w6.size(), 1
+00027090: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000270a0: 7373 6572 7445 7175 616c 2874 7970 6528  ssertEqual(type(
+000270b0: 7736 2e76 616c 2829 292c 2057 6972 6529  w6.val()), Wire)
+000270c0: 0a20 2020 2020 2020 2023 206d 616b 6520  .        # make 
+000270d0: 7375 7265 2074 6865 2072 6573 756c 7469  sure the resulti
+000270e0: 6e67 2077 6972 6520 6861 7320 666f 7243  ng wire has forC
+000270f0: 6f6e 7374 7275 6374 696f 6e20 7365 740a  onstruction set.
+00027100: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00027110: 6572 7445 7175 616c 2877 362e 7661 6c28  ertEqual(w6.val(
+00027120: 292e 666f 7243 6f6e 7374 7275 6374 696f  ).forConstructio
+00027130: 6e2c 2054 7275 6529 0a0a 2020 2020 6465  n, True)..    de
+00027140: 6620 7465 7374 436f 6e73 6f6c 6964 6174  f testConsolidat
+00027150: 6557 6972 6573 2873 656c 6629 3a0a 0a20  eWires(self):.. 
+00027160: 2020 2020 2020 2077 3120 3d20 576f 726b         w1 = Work
+00027170: 706c 616e 6528 292e 6c69 6e65 546f 2830  plane().lineTo(0
+00027180: 2c20 3129 2e6c 696e 6554 6f28 312c 2031  , 1).lineTo(1, 1
+00027190: 292e 636f 6e73 6f6c 6964 6174 6557 6972  ).consolidateWir
+000271a0: 6573 2829 0a20 2020 2020 2020 2073 656c  es().        sel
+000271b0: 662e 6173 7365 7274 4571 7561 6c28 7731  f.assertEqual(w1
+000271c0: 2e73 697a 6528 292c 2031 290a 0a20 2020  .size(), 1)..   
+000271d0: 2020 2020 2077 3120 3d20 576f 726b 706c       w1 = Workpl
+000271e0: 616e 6528 292e 636f 6e73 6f6c 6964 6174  ane().consolidat
+000271f0: 6557 6972 6573 2829 0a20 2020 2020 2020  eWires().       
+00027200: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00027210: 6c28 7731 2e73 697a 6528 292c 2030 290a  l(w1.size(), 0).
+00027220: 0a20 2020 2064 6566 2074 6573 744c 6f63  .    def testLoc
+00027230: 6174 696f 6e41 7428 7365 6c66 293a 0a0a  ationAt(self):..
+00027240: 2020 2020 2020 2020 7220 3d20 310a 2020          r = 1.  
+00027250: 2020 2020 2020 6520 3d20 5769 7265 2e6d        e = Wire.m
+00027260: 616b 6548 656c 6978 2872 2c20 722c 2072  akeHelix(r, r, r
+00027270: 292e 4564 6765 7328 295b 305d 0a0a 2020  ).Edges()[0]..  
+00027280: 2020 2020 2020 6c6f 6373 5f66 7265 6e65        locs_frene
+00027290: 7420 3d20 652e 6c6f 6361 7469 6f6e 7328  t = e.locations(
+000272a0: 5b30 2c20 315d 2c20 6672 616d 653d 2266  [0, 1], frame="f
+000272b0: 7265 6e65 7422 290a 0a20 2020 2020 2020  renet")..       
+000272c0: 2054 3120 3d20 6c6f 6373 5f66 7265 6e65   T1 = locs_frene
+000272d0: 745b 305d 2e77 7261 7070 6564 2e54 7261  t[0].wrapped.Tra
+000272e0: 6e73 666f 726d 6174 696f 6e28 290a 2020  nsformation().  
+000272f0: 2020 2020 2020 5432 203d 206c 6f63 735f        T2 = locs_
+00027300: 6672 656e 6574 5b31 5d2e 7772 6170 7065  frenet[1].wrappe
+00027310: 642e 5472 616e 7366 6f72 6d61 7469 6f6e  d.Transformation
+00027320: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00027330: 2e61 7373 6572 7441 6c6d 6f73 7445 7175  .assertAlmostEqu
+00027340: 616c 2854 312e 5472 616e 736c 6174 696f  al(T1.Translatio
+00027350: 6e50 6172 7428 292e 5828 292c 2072 2c20  nPart().X(), r, 
+00027360: 3629 0a20 2020 2020 2020 2073 656c 662e  6).        self.
+00027370: 6173 7365 7274 416c 6d6f 7374 4571 7561  assertAlmostEqua
+00027380: 6c28 5432 2e54 7261 6e73 6c61 7469 6f6e  l(T2.Translation
+00027390: 5061 7274 2829 2e58 2829 2c20 722c 2036  Part().X(), r, 6
+000273a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000273b0: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
+000273c0: 280a 2020 2020 2020 2020 2020 2020 5431  (.            T1
+000273d0: 2e47 6574 526f 7461 7469 6f6e 2829 2e47  .GetRotation().G
+000273e0: 6574 526f 7461 7469 6f6e 416e 676c 6528  etRotationAngle(
+000273f0: 292c 202d 5432 2e47 6574 526f 7461 7469  ), -T2.GetRotati
+00027400: 6f6e 2829 2e47 6574 526f 7461 7469 6f6e  on().GetRotation
+00027410: 416e 676c 6528 292c 2036 0a20 2020 2020  Angle(), 6.     
+00027420: 2020 2029 0a0a 2020 2020 2020 2020 6761     )..        ga
+00027430: 203d 2065 2e5f 6765 6f6d 4164 6170 746f   = e._geomAdapto
+00027440: 7228 290a 0a20 2020 2020 2020 206c 6f63  r()..        loc
+00027450: 735f 636f 7272 6563 7465 6420 3d20 652e  s_corrected = e.
+00027460: 6c6f 6361 7469 6f6e 7328 0a20 2020 2020  locations(.     
+00027470: 2020 2020 2020 205b 6761 2e46 6972 7374         [ga.First
+00027480: 5061 7261 6d65 7465 7228 292c 2067 612e  Parameter(), ga.
+00027490: 4c61 7374 5061 7261 6d65 7465 7228 295d  LastParameter()]
+000274a0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+000274b0: 6465 3d22 7061 7261 6d65 7465 7222 2c0a  de="parameter",.
+000274c0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000274d0: 653d 2263 6f72 7265 6374 6564 222c 0a20  e="corrected",. 
+000274e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000274f0: 2020 5433 203d 206c 6f63 735f 636f 7272    T3 = locs_corr
+00027500: 6563 7465 645b 305d 2e77 7261 7070 6564  ected[0].wrapped
+00027510: 2e54 7261 6e73 666f 726d 6174 696f 6e28  .Transformation(
+00027520: 290a 2020 2020 2020 2020 5434 203d 206c  ).        T4 = l
+00027530: 6f63 735f 636f 7272 6563 7465 645b 315d  ocs_corrected[1]
+00027540: 2e77 7261 7070 6564 2e54 7261 6e73 666f  .wrapped.Transfo
+00027550: 726d 6174 696f 6e28 290a 0a20 2020 2020  rmation()..     
+00027560: 2020 2073 656c 662e 6173 7365 7274 416c     self.assertAl
+00027570: 6d6f 7374 4571 7561 6c28 5433 2e54 7261  mostEqual(T3.Tra
+00027580: 6e73 6c61 7469 6f6e 5061 7274 2829 2e58  nslationPart().X
+00027590: 2829 2c20 722c 2036 290a 2020 2020 2020  (), r, 6).      
+000275a0: 2020 7365 6c66 2e61 7373 6572 7441 6c6d    self.assertAlm
+000275b0: 6f73 7445 7175 616c 2854 342e 5472 616e  ostEqual(T4.Tran
+000275c0: 736c 6174 696f 6e50 6172 7428 292e 5828  slationPart().X(
+000275d0: 292c 2072 2c20 3629 0a0a 2020 2020 2020  ), r, 6)..      
+000275e0: 2020 7720 3d20 5769 7265 2e61 7373 656d    w = Wire.assem
+000275f0: 626c 6545 6467 6573 280a 2020 2020 2020  bleEdges(.      
+00027600: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00027610: 2020 2020 2020 2020 4564 6765 2e6d 616b          Edge.mak
+00027620: 654c 696e 6528 5665 6374 6f72 2829 2c20  eLine(Vector(), 
+00027630: 5665 6374 6f72 2830 2c20 3129 292c 0a20  Vector(0, 1)),. 
+00027640: 2020 2020 2020 2020 2020 2020 2020 2045                 E
+00027650: 6467 652e 6d61 6b65 4c69 6e65 2856 6563  dge.makeLine(Vec
+00027660: 746f 7228 302c 2031 292c 2056 6563 746f  tor(0, 1), Vecto
+00027670: 7228 312c 2031 2929 2c0a 2020 2020 2020  r(1, 1)),.      
+00027680: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00027690: 290a 2020 2020 2020 2020 6c6f 6373 5f77  ).        locs_w
+000276a0: 6972 6520 3d20 652e 6c6f 6361 7469 6f6e  ire = e.location
+000276b0: 7328 5b30 2c20 315d 290a 0a20 2020 2020  s([0, 1])..     
+000276c0: 2020 2054 3520 3d20 6c6f 6373 5f77 6972     T5 = locs_wir
+000276d0: 655b 305d 2e77 7261 7070 6564 2e54 7261  e[0].wrapped.Tra
+000276e0: 6e73 666f 726d 6174 696f 6e28 290a 2020  nsformation().  
+000276f0: 2020 2020 2020 5436 203d 206c 6f63 735f        T6 = locs_
+00027700: 7769 7265 5b31 5d2e 7772 6170 7065 642e  wire[1].wrapped.
+00027710: 5472 616e 7366 6f72 6d61 7469 6f6e 2829  Transformation()
+00027720: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00027730: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
+00027740: 2854 352e 5472 616e 736c 6174 696f 6e50  (T5.TranslationP
+00027750: 6172 7428 292e 5828 292c 2072 2c20 3029  art().X(), r, 0)
+00027760: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00027770: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
+00027780: 5436 2e54 7261 6e73 6c61 7469 6f6e 5061  T6.TranslationPa
+00027790: 7274 2829 2e58 2829 2c20 722c 2031 290a  rt().X(), r, 1).
+000277a0: 0a20 2020 2064 6566 2074 6573 744e 6f72  .    def testNor
+000277b0: 6d61 6c28 7365 6c66 293a 0a0a 2020 2020  mal(self):..    
+000277c0: 2020 2020 6369 7263 203d 2057 6f72 6b70      circ = Workp
+000277d0: 6c61 6e65 2829 2e63 6972 636c 6528 3129  lane().circle(1)
+000277e0: 2e65 6467 6573 2829 2e76 616c 2829 0a20  .edges().val(). 
+000277f0: 2020 2020 2020 206e 203d 2063 6972 632e         n = circ.
+00027800: 6e6f 726d 616c 2829 0a0a 2020 2020 2020  normal()..      
+00027810: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
+00027820: 6c65 416c 6d6f 7374 4571 7561 6c73 286e  leAlmostEquals(n
+00027830: 2e74 6f54 7570 6c65 2829 2c20 2830 2c20  .toTuple(), (0, 
+00027840: 302c 2031 292c 2036 290a 0a20 2020 2020  0, 1), 6)..     
+00027850: 2020 2065 6c6c 203d 2057 6f72 6b70 6c61     ell = Workpla
+00027860: 6e65 2829 2e65 6c6c 6970 7365 2831 2c20  ne().ellipse(1, 
+00027870: 3229 2e65 6467 6573 2829 2e76 616c 2829  2).edges().val()
+00027880: 0a20 2020 2020 2020 206e 203d 2065 6c6c  .        n = ell
+00027890: 2e6e 6f72 6d61 6c28 290a 0a20 2020 2020  .normal()..     
+000278a0: 2020 2073 656c 662e 6173 7365 7274 5475     self.assertTu
+000278b0: 706c 6541 6c6d 6f73 7445 7175 616c 7328  pleAlmostEquals(
+000278c0: 6e2e 746f 5475 706c 6528 292c 2028 302c  n.toTuple(), (0,
+000278d0: 2030 2c20 3129 2c20 3629 0a0a 2020 2020   0, 1), 6)..    
+000278e0: 2020 2020 7220 3d20 576f 726b 706c 616e      r = Workplan
+000278f0: 6528 292e 7265 6374 2831 2c20 3229 2e77  e().rect(1, 2).w
+00027900: 6972 6573 2829 2e76 616c 2829 0a20 2020  ires().val().   
+00027910: 2020 2020 206e 203d 2072 2e6e 6f72 6d61       n = r.norma
+00027920: 6c28 290a 0a20 2020 2020 2020 2073 656c  l()..        sel
+00027930: 662e 6173 7365 7274 5475 706c 6541 6c6d  f.assertTupleAlm
+00027940: 6f73 7445 7175 616c 7328 6e2e 746f 5475  ostEquals(n.toTu
+00027950: 706c 6528 292c 2028 302c 2030 2c20 3129  ple(), (0, 0, 1)
+00027960: 2c20 3629 0a0a 2020 2020 2020 2020 7769  , 6)..        wi
+00027970: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+00027980: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+00027990: 3a0a 2020 2020 2020 2020 2020 2020 6564  :.            ed
+000279a0: 6765 203d 2057 6f72 6b70 6c61 6e65 2829  ge = Workplane()
+000279b0: 2e72 6563 7428 312c 2032 292e 6564 6765  .rect(1, 2).edge
+000279c0: 7328 292e 7661 6c28 290a 2020 2020 2020  s().val().      
+000279d0: 2020 2020 2020 6e20 3d20 6564 6765 2e6e        n = edge.n
+000279e0: 6f72 6d61 6c28 290a 0a20 2020 2064 6566  ormal()..    def
+000279f0: 2074 6573 7450 6f73 6974 696f 6e41 7428   testPositionAt(
+00027a00: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+00027a10: 2320 7465 7374 2077 6974 6820 616e 206f  # test with an o
+00027a20: 7065 6e20 7769 7265 0a20 2020 2020 2020  pen wire.       
+00027a30: 2077 203d 2057 6f72 6b70 6c61 6e65 2829   w = Workplane()
+00027a40: 2e6c 696e 6554 6f28 302c 2031 292e 6c69  .lineTo(0, 1).li
+00027a50: 6e65 546f 2831 2c20 3129 2e77 6972 6528  neTo(1, 1).wire(
+00027a60: 292e 7661 6c28 290a 0a20 2020 2020 2020  ).val()..       
+00027a70: 2070 3020 3d20 772e 706f 7369 7469 6f6e   p0 = w.position
+00027a80: 4174 2830 2e30 290a 2020 2020 2020 2020  At(0.0).        
+00027a90: 7031 203d 2077 2e70 6f73 6974 696f 6e41  p1 = w.positionA
+00027aa0: 7428 302e 3529 0a20 2020 2020 2020 2070  t(0.5).        p
+00027ab0: 3220 3d20 772e 706f 7369 7469 6f6e 4174  2 = w.positionAt
+00027ac0: 2831 2e30 290a 0a20 2020 2020 2020 2073  (1.0)..        s
+00027ad0: 656c 662e 6173 7365 7274 5475 706c 6541  elf.assertTupleA
+00027ae0: 6c6d 6f73 7445 7175 616c 7328 7030 2e74  lmostEquals(p0.t
+00027af0: 6f54 7570 6c65 2829 2c20 2830 2c20 302c  oTuple(), (0, 0,
+00027b00: 2030 292c 2036 290a 2020 2020 2020 2020   0), 6).        
+00027b10: 7365 6c66 2e61 7373 6572 7454 7570 6c65  self.assertTuple
+00027b20: 416c 6d6f 7374 4571 7561 6c73 2870 312e  AlmostEquals(p1.
+00027b30: 746f 5475 706c 6528 292c 2028 302c 2031  toTuple(), (0, 1
+00027b40: 2c20 3029 2c20 3629 0a20 2020 2020 2020  , 0), 6).       
+00027b50: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
+00027b60: 6541 6c6d 6f73 7445 7175 616c 7328 7032  eAlmostEquals(p2
+00027b70: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
+00027b80: 312c 2030 292c 2036 290a 0a20 2020 2020  1, 0), 6)..     
+00027b90: 2020 2070 3020 3d20 772e 706f 7369 7469     p0 = w.positi
+00027ba0: 6f6e 4174 2830 2e30 2c20 6d6f 6465 3d22  onAt(0.0, mode="
+00027bb0: 7061 7261 6d22 290a 0a20 2020 2020 2020  param")..       
+00027bc0: 2073 656c 662e 6173 7365 7274 5475 706c   self.assertTupl
+00027bd0: 6541 6c6d 6f73 7445 7175 616c 7328 7030  eAlmostEquals(p0
+00027be0: 2e74 6f54 7570 6c65 2829 2c20 2830 2c20  .toTuple(), (0, 
+00027bf0: 302c 2030 292c 2036 290a 0a20 2020 2020  0, 0), 6)..     
+00027c00: 2020 2070 302c 2070 312c 2070 3220 3d20     p0, p1, p2 = 
+00027c10: 772e 706f 7369 7469 6f6e 7328 5b30 2e30  w.positions([0.0
+00027c20: 2c20 302e 3235 2c20 302e 355d 290a 0a20  , 0.25, 0.5]).. 
+00027c30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00027c40: 7274 5475 706c 6541 6c6d 6f73 7445 7175  rtTupleAlmostEqu
+00027c50: 616c 7328 7030 2e74 6f54 7570 6c65 2829  als(p0.toTuple()
+00027c60: 2c20 2830 2c20 302c 2030 292c 2036 290a  , (0, 0, 0), 6).
+00027c70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00027c80: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
+00027c90: 7561 6c73 2870 312e 746f 5475 706c 6528  uals(p1.toTuple(
+00027ca0: 292c 2028 302c 2030 2e35 2c20 3029 2c20  ), (0, 0.5, 0), 
+00027cb0: 3629 0a20 2020 2020 2020 2073 656c 662e  6).        self.
+00027cc0: 6173 7365 7274 5475 706c 6541 6c6d 6f73  assertTupleAlmos
+00027cd0: 7445 7175 616c 7328 7032 2e74 6f54 7570  tEquals(p2.toTup
+00027ce0: 6c65 2829 2c20 2830 2c20 312c 2030 292c  le(), (0, 1, 0),
+00027cf0: 2036 290a 0a20 2020 2020 2020 2023 2074   6)..        # t
+00027d00: 6573 7420 7769 7468 2061 2063 6c6f 7365  est with a close
+00027d10: 6420 7769 7265 0a20 2020 2020 2020 2077  d wire.        w
+00027d20: 203d 2057 6f72 6b70 6c61 6e65 2829 2e6c   = Workplane().l
+00027d30: 696e 6554 6f28 302c 2031 292e 636c 6f73  ineTo(0, 1).clos
+00027d40: 6528 292e 7769 7265 2829 2e76 616c 2829  e().wire().val()
+00027d50: 0a0a 2020 2020 2020 2020 7030 203d 2077  ..        p0 = w
+00027d60: 2e70 6f73 6974 696f 6e41 7428 302e 3029  .positionAt(0.0)
+00027d70: 0a20 2020 2020 2020 2070 3120 3d20 772e  .        p1 = w.
+00027d80: 706f 7369 7469 6f6e 4174 2830 2e35 290a  positionAt(0.5).
+00027d90: 2020 2020 2020 2020 7032 203d 2077 2e70          p2 = w.p
+00027da0: 6f73 6974 696f 6e41 7428 312e 3029 0a0a  ositionAt(1.0)..
+00027db0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00027dc0: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
+00027dd0: 7561 6c73 2870 302e 746f 5475 706c 6528  uals(p0.toTuple(
+00027de0: 292c 2070 322e 746f 5475 706c 6528 292c  ), p2.toTuple(),
+00027df0: 2036 290a 2020 2020 2020 2020 7365 6c66   6).        self
+00027e00: 2e61 7373 6572 7454 7570 6c65 416c 6d6f  .assertTupleAlmo
+00027e10: 7374 4571 7561 6c73 2870 312e 746f 5475  stEquals(p1.toTu
+00027e20: 706c 6528 292c 2028 302c 2031 2c20 3029  ple(), (0, 1, 0)
+00027e30: 2c20 3629 0a0a 2020 2020 2020 2020 2320  , 6)..        # 
+00027e40: 7465 7374 2077 6974 6820 6172 6320 6f66  test with arc of
+00027e50: 2063 6972 636c 650a 2020 2020 2020 2020   circle.        
+00027e60: 6520 3d20 4564 6765 2e6d 616b 6543 6972  e = Edge.makeCir
+00027e70: 636c 6528 312c 2028 302c 2030 2c20 3029  cle(1, (0, 0, 0)
+00027e80: 2c20 2830 2c20 302c 2031 292c 2039 302c  , (0, 0, 1), 90,
+00027e90: 2031 3830 290a 2020 2020 2020 2020 7030   180).        p0
+00027ea0: 203d 2065 2e70 6f73 6974 696f 6e41 7428   = e.positionAt(
+00027eb0: 302e 3029 0a20 2020 2020 2020 2070 3120  0.0).        p1 
+00027ec0: 3d20 652e 706f 7369 7469 6f6e 4174 2831  = e.positionAt(1
+00027ed0: 2e30 290a 2020 2020 2020 2020 6173 7365  .0).        asse
+00027ee0: 7274 2070 302e 746f 5475 706c 6528 2920  rt p0.toTuple() 
+00027ef0: 3d3d 2061 7070 726f 7828 2830 2e30 2c20  == approx((0.0, 
+00027f00: 312e 302c 2030 2e30 2929 0a20 2020 2020  1.0, 0.0)).     
+00027f10: 2020 2061 7373 6572 7420 7031 2e74 6f54     assert p1.toT
+00027f20: 7570 6c65 2829 203d 3d20 6170 7072 6f78  uple() == approx
+00027f30: 2828 2d31 2e30 2c20 302e 302c 2030 2e30  ((-1.0, 0.0, 0.0
+00027f40: 2929 0a0a 2020 2020 2020 2020 7720 3d20  ))..        w = 
+00027f50: 5769 7265 2e61 7373 656d 626c 6545 6467  Wire.assembleEdg
+00027f60: 6573 285b 655d 290a 2020 2020 2020 2020  es([e]).        
+00027f70: 7030 203d 2077 2e70 6f73 6974 696f 6e41  p0 = w.positionA
+00027f80: 7428 302e 3029 0a20 2020 2020 2020 2070  t(0.0).        p
+00027f90: 3120 3d20 772e 706f 7369 7469 6f6e 4174  1 = w.positionAt
+00027fa0: 2831 2e30 290a 2020 2020 2020 2020 6173  (1.0).        as
+00027fb0: 7365 7274 2070 302e 746f 5475 706c 6528  sert p0.toTuple(
+00027fc0: 2920 3d3d 2061 7070 726f 7828 2830 2e30  ) == approx((0.0
+00027fd0: 2c20 312e 302c 2030 2e30 2929 0a20 2020  , 1.0, 0.0)).   
+00027fe0: 2020 2020 2061 7373 6572 7420 7031 2e74       assert p1.t
+00027ff0: 6f54 7570 6c65 2829 203d 3d20 6170 7072  oTuple() == appr
+00028000: 6f78 2828 2d31 2e30 2c20 302e 302c 2030  ox((-1.0, 0.0, 0
+00028010: 2e30 2929 0a0a 2020 2020 6465 6620 7465  .0))..    def te
+00028020: 7374 5461 6e67 656e 6741 7428 7365 6c66  stTangengAt(self
+00028030: 293a 0a0a 2020 2020 2020 2020 7074 7320  ):..        pts 
+00028040: 3d20 5b28 302c 2030 292c 2028 2d31 2c20  = [(0, 0), (-1, 
+00028050: 3129 2c20 282d 322c 2030 292c 2028 2d31  1), (-2, 0), (-1
+00028060: 2c20 3029 5d0a 0a20 2020 2020 2020 2070  , 0)]..        p
+00028070: 6174 6820 3d20 576f 726b 706c 616e 6528  ath = Workplane(
+00028080: 2258 5a22 292e 7370 6c69 6e65 2870 7473  "XZ").spline(pts
+00028090: 2c20 7461 6e67 656e 7473 3d28 2830 2c20  , tangents=((0, 
+000280a0: 3129 2c20 2831 2c20 3029 2929 2e76 616c  1), (1, 0))).val
+000280b0: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
+000280c0: 2e61 7373 6572 7454 7275 6528 0a20 2020  .assertTrue(.   
+000280d0: 2020 2020 2020 2020 2070 6174 682e 7461           path.ta
+000280e0: 6e67 656e 7441 7428 302e 302c 206d 6f64  ngentAt(0.0, mod
+000280f0: 653d 2270 6172 616d 6574 6572 2229 203d  e="parameter") =
+00028100: 3d20 7061 7468 2e74 616e 6765 6e74 4174  = path.tangentAt
+00028110: 2830 2e30 2c20 6d6f 6465 3d22 6c65 6e67  (0.0, mode="leng
+00028120: 7468 2229 0a20 2020 2020 2020 2029 0a20  th").        ). 
+00028130: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00028140: 7274 4661 6c73 6528 0a20 2020 2020 2020  rtFalse(.       
+00028150: 2020 2020 2070 6174 682e 7461 6e67 656e       path.tangen
+00028160: 7441 7428 302e 352c 206d 6f64 653d 2270  tAt(0.5, mode="p
+00028170: 6172 616d 6574 6572 2229 203d 3d20 7061  arameter") == pa
+00028180: 7468 2e74 616e 6765 6e74 4174 2830 2e35  th.tangentAt(0.5
+00028190: 2c20 6d6f 6465 3d22 6c65 6e67 7468 2229  , mode="length")
+000281a0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000281b0: 2020 2020 6172 6320 3d20 576f 726b 706c      arc = Workpl
+000281c0: 616e 6528 292e 7261 6469 7573 4172 6328  ane().radiusArc(
+000281d0: 2832 2c20 3029 2c20 3129 2e76 616c 2829  (2, 0), 1).val()
+000281e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+000281f0: 7373 6572 7454 7570 6c65 416c 6d6f 7374  ssertTupleAlmost
+00028200: 4571 7561 6c73 280a 2020 2020 2020 2020  Equals(.        
+00028210: 2020 2020 6172 632e 7461 6e67 656e 7441      arc.tangentA
+00028220: 7428 6d61 7468 2e70 6920 2f20 322c 2022  t(math.pi / 2, "
+00028230: 7061 7261 6d65 7465 7222 292e 746f 5475  parameter").toTu
+00028240: 706c 6528 292c 2028 312c 2030 2c20 3029  ple(), (1, 0, 0)
+00028250: 2c20 360a 2020 2020 2020 2020 290a 2020  , 6.        ).  
+00028260: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00028270: 7454 7570 6c65 416c 6d6f 7374 4571 7561  tTupleAlmostEqua
+00028280: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
+00028290: 6172 632e 7461 6e67 656e 7441 7428 302e  arc.tangentAt(0.
+000282a0: 352c 2022 6c65 6e67 7468 2229 2e74 6f54  5, "length").toT
+000282b0: 7570 6c65 2829 2c20 2831 2c20 302c 2030  uple(), (1, 0, 0
+000282c0: 292c 2036 0a20 2020 2020 2020 2029 0a0a  ), 6.        )..
+000282d0: 2020 2020 6465 6620 7465 7374 456e 6428      def testEnd(
+000282e0: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+000282f0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00028300: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
+00028310: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00028320: 576f 726b 706c 616e 6528 292e 656e 6428  Workplane().end(
+00028330: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00028340: 6173 7365 7274 5472 7565 2857 6f72 6b70  assertTrue(Workp
+00028350: 6c61 6e65 2829 2e6f 626a 6563 7473 203d  lane().objects =
+00028360: 3d20 5b5d 290a 2020 2020 2020 2020 7365  = []).        se
+00028370: 6c66 2e61 7373 6572 7454 7275 6528 576f  lf.assertTrue(Wo
+00028380: 726b 706c 616e 6528 292e 626f 7828 312c  rkplane().box(1,
+00028390: 2031 2c20 3129 2e65 6e64 2829 2e6f 626a   1, 1).end().obj
+000283a0: 6563 7473 203d 3d20 5b5d 290a 2020 2020  ects == []).    
+000283b0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000283c0: 7275 6528 576f 726b 706c 616e 6528 292e  rue(Workplane().
+000283d0: 626f 7828 312c 2031 2c20 3129 2e62 6f78  box(1, 1, 1).box
+000283e0: 2832 2c20 322c 2031 292e 656e 6428 3229  (2, 2, 1).end(2)
+000283f0: 2e6f 626a 6563 7473 203d 3d20 5b5d 290a  .objects == []).
+00028400: 0a20 2020 2064 6566 2074 6573 7443 7574  .    def testCut
+00028410: 4561 6368 2873 656c 6629 3a0a 0a20 2020  Each(self):..   
+00028420: 2020 2020 2023 2062 6173 6520 7368 6170       # base shap
+00028430: 653a 0a20 2020 2020 2020 2077 203d 2057  e:.        w = W
+00028440: 6f72 6b70 6c61 6e65 2829 2e62 6f78 2833  orkplane().box(3
+00028450: 2c20 322c 2032 290a 2020 2020 2020 2020  , 2, 2).        
+00028460: 2320 6375 7474 6572 3a0a 2020 2020 2020  # cutter:.      
+00028470: 2020 6320 3d20 576f 726b 706c 616e 6528    c = Workplane(
+00028480: 292e 626f 7828 322c 2032 2c20 3229 2e76  ).box(2, 2, 2).v
+00028490: 616c 2829 0a20 2020 2020 2020 2023 2063  al().        # c
+000284a0: 7574 2061 6c6c 2074 6865 2063 6f72 6e65  ut all the corne
+000284b0: 7273 206f 6666 0a20 2020 2020 2020 2077  rs off.        w
+000284c0: 3020 3d20 772e 7665 7274 6963 6573 2829  0 = w.vertices()
+000284d0: 2e63 7574 4561 6368 286c 616d 6264 6120  .cutEach(lambda 
+000284e0: 6c6f 633a 2063 2e6c 6f63 6174 6564 286c  loc: c.located(l
+000284f0: 6f63 2929 0a20 2020 2020 2020 2023 2077  oc)).        # w
+00028500: 6520 6172 6520 6c65 6674 2077 6974 6820  e are left with 
+00028510: 6120 3178 3278 3220 626f 783a 0a20 2020  a 1x2x2 box:.   
+00028520: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00028530: 416c 6d6f 7374 4571 7561 6c28 7730 2e76  AlmostEqual(w0.v
+00028540: 616c 2829 2e56 6f6c 756d 6528 292c 2034  al().Volume(), 4
+00028550: 2c20 3329 0a0a 2020 2020 2020 2020 2320  , 3)..        # 
+00028560: 7465 7374 2065 7272 6f72 206f 6e20 6e6f  test error on no
+00028570: 2073 6f6c 6964 2066 6f75 6e64 0a20 2020   solid found.   
+00028580: 2020 2020 2077 3120 3d20 576f 726b 706c       w1 = Workpl
+00028590: 616e 6528 292e 684c 696e 6528 3129 2e76  ane().hLine(1).v
+000285a0: 4c69 6e65 2831 292e 636c 6f73 6528 290a  Line(1).close().
+000285b0: 2020 2020 2020 2020 7769 7468 2072 6169          with rai
+000285c0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
+000285d0: 0a20 2020 2020 2020 2020 2020 2077 312e  .            w1.
+000285e0: 6375 7445 6163 6828 6c61 6d62 6461 206c  cutEach(lambda l
+000285f0: 6f63 3a20 632e 6c6f 6361 7465 6428 6c6f  oc: c.located(lo
+00028600: 6329 290a 0a20 2020 2064 6566 2074 6573  c))..    def tes
+00028610: 7443 7574 426c 696e 6428 7365 6c66 293a  tCutBlind(self):
+00028620: 0a20 2020 2020 2020 2023 2063 7574 426c  .        # cutBl
+00028630: 696e 6420 6973 2061 6c72 6561 6479 2074  ind is already t
+00028640: 6573 7465 6420 696e 2073 6576 6572 616c  ested in several
+00028650: 206f 6620 7468 6520 636f 6d70 6c69 6361   of the complica
+00028660: 7465 6420 7465 7374 732c 2073 6f20 7468  ted tests, so th
+00028670: 6973 206d 6574 686f 6420 6973 2073 686f  is method is sho
+00028680: 7274 2e0a 2020 2020 2020 2020 2320 7465  rt..        # te
+00028690: 7374 2056 616c 7565 4572 726f 7220 6f6e  st ValueError on
+000286a0: 206e 6f20 736f 6c69 6420 666f 756e 640a   no solid found.
+000286b0: 2020 2020 2020 2020 7730 203d 2057 6f72          w0 = Wor
+000286c0: 6b70 6c61 6e65 2829 2e68 4c69 6e65 2831  kplane().hLine(1
+000286d0: 292e 764c 696e 6528 3129 2e63 6c6f 7365  ).vLine(1).close
+000286e0: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
+000286f0: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
 00028700: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00028710: 7734 2e63 7478 2e70 6f70 5065 6e64 696e  w4.ctx.popPendin
-00028720: 6757 6972 6573 2829 0a0a 2020 2020 2020  gWires()..      
-00028730: 2020 2320 7465 7374 2076 6961 2063 7574    # test via cut
-00028740: 426c 696e 640a 2020 2020 2020 2020 7735  Blind.        w5
-00028750: 203d 2057 6f72 6b70 6c61 6e65 2829 2e63   = Workplane().c
-00028760: 6972 636c 6528 3129 2e65 7874 7275 6465  ircle(1).extrude
-00028770: 2831 290a 2020 2020 2020 2020 7769 7468  (1).        with
-00028780: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00028790: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
-000287a0: 2020 2020 2020 2020 2020 2020 7735 2e63              w5.c
-000287b0: 7574 426c 696e 6428 2d31 290a 0a20 2020  utBlind(-1)..   
-000287c0: 2064 6566 2074 6573 7443 6f6d 7053 6f6c   def testCompSol
-000287d0: 6964 2873 656c 6629 3a0a 0a20 2020 2020  id(self):..     
-000287e0: 2020 2066 726f 6d20 4f43 502e 4252 6570     from OCP.BRep
-000287f0: 5072 696d 4150 4920 696d 706f 7274 2042  PrimAPI import B
-00028800: 5265 7050 7269 6d41 5049 5f4d 616b 6550  RepPrimAPI_MakeP
-00028810: 7269 736d 0a0a 2020 2020 2020 2020 746f  rism..        to
-00028820: 6f6c 203d 2053 6f6c 6964 2e6d 616b 6553  ol = Solid.makeS
-00028830: 7068 6572 6528 312c 2061 6e67 6c65 4465  phere(1, angleDe
-00028840: 6772 6565 7333 3d31 3230 290a 2020 2020  grees3=120).    
-00028850: 2020 2020 7368 656c 6c20 3d20 746f 6f6c      shell = tool
-00028860: 2e53 6865 6c6c 7328 295b 305d 0a20 2020  .Shells()[0].   
-00028870: 2020 2020 2076 203d 2056 6563 746f 7228       v = Vector(
-00028880: 302c 2030 2c20 3129 0a0a 2020 2020 2020  0, 0, 1)..      
-00028890: 2020 6275 696c 6465 7220 3d20 4252 6570    builder = BRep
-000288a0: 5072 696d 4150 495f 4d61 6b65 5072 6973  PrimAPI_MakePris
-000288b0: 6d28 7368 656c 6c2e 7772 6170 7065 642c  m(shell.wrapped,
-000288c0: 2076 2e77 7261 7070 6564 290a 2020 2020   v.wrapped).    
-000288d0: 2020 2020 7265 7375 6c74 203d 2053 6861      result = Sha
-000288e0: 7065 2e63 6173 7428 6275 696c 6465 722e  pe.cast(builder.
-000288f0: 5368 6170 6528 2929 0a0a 2020 2020 2020  Shape())..      
-00028900: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00028910: 616c 286c 656e 2872 6573 756c 742e 436f  al(len(result.Co
-00028920: 6d70 536f 6c69 6473 2829 292c 2031 290a  mpSolids()), 1).
-00028930: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00028940: 6572 7445 7175 616c 286c 656e 2872 6573  ertEqual(len(res
-00028950: 756c 742e 536f 6c69 6473 2829 292c 2034  ult.Solids()), 4
-00028960: 290a 0a20 2020 2064 6566 2074 6573 7432  )..    def test2
-00028970: 4466 696c 6c65 7428 7365 6c66 293a 0a0a  Dfillet(self):..
-00028980: 2020 2020 2020 2020 7220 3d20 576f 726b          r = Work
-00028990: 706c 616e 6528 292e 7265 6374 2831 2c20  plane().rect(1, 
-000289a0: 3229 2e77 6972 6573 2829 2e76 616c 2829  2).wires().val()
-000289b0: 0a20 2020 2020 2020 2066 203d 2046 6163  .        f = Fac
-000289c0: 652e 6d61 6b65 4672 6f6d 5769 7265 7328  e.makeFromWires(
-000289d0: 7229 0a20 2020 2020 2020 2076 6572 7473  r).        verts
-000289e0: 203d 2072 2e56 6572 7469 6365 7328 290a   = r.Vertices().
-000289f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00028a00: 7365 7274 4571 7561 6c28 6c65 6e28 662e  sertEqual(len(f.
-00028a10: 6669 6c6c 6574 3244 2830 2e35 2c20 7665  fillet2D(0.5, ve
-00028a20: 7274 7329 2e56 6572 7469 6365 7328 2929  rts).Vertices())
-00028a30: 2c20 3629 0a20 2020 2020 2020 2073 656c  , 6).        sel
-00028a40: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00028a50: 6e28 722e 6669 6c6c 6574 3244 2830 2e35  n(r.fillet2D(0.5
-00028a60: 2c20 7665 7274 7329 2e56 6572 7469 6365  , verts).Vertice
-00028a70: 7328 2929 2c20 3629 0a20 2020 2020 2020  s()), 6).       
-00028a80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00028a90: 6c28 6c65 6e28 722e 6669 6c6c 6574 3244  l(len(r.fillet2D
-00028aa0: 2830 2e32 352c 2076 6572 7473 292e 5665  (0.25, verts).Ve
-00028ab0: 7274 6963 6573 2829 292c 2038 290a 0a20  rtices()), 8).. 
-00028ac0: 2020 2020 2020 2023 2054 6573 7420 6669         # Test fi
-00028ad0: 6c6c 6574 3244 2077 6974 6820 6f70 656e  llet2D with open
-00028ae0: 2077 6972 6520 616e 6420 7369 6e67 6c65   wire and single
-00028af0: 2076 6572 7465 780a 2020 2020 2020 2020   vertex.        
-00028b00: 7730 203d 2057 6f72 6b70 6c61 6e65 2829  w0 = Workplane()
-00028b10: 2e68 4c69 6e65 2831 292e 764c 696e 6528  .hLine(1).vLine(
-00028b20: 3129 2e77 6972 6528 290a 2020 2020 2020  1).wire().      
-00028b30: 2020 7730 5f76 6572 7473 203d 2077 302e    w0_verts = w0.
-00028b40: 7665 7274 6963 6573 2822 3e58 2061 6e64  vertices(">X and
-00028b50: 203c 5922 292e 7661 6c73 2829 0a20 2020   <Y").vals().   
-00028b60: 2020 2020 2075 6e66 696c 6c65 7465 645f       unfilleted_
-00028b70: 7769 7265 3020 3d20 7730 2e76 616c 2829  wire0 = w0.val()
-00028b80: 0a20 2020 2020 2020 2066 696c 6c65 7465  .        fillete
-00028b90: 645f 7769 7265 3020 3d20 756e 6669 6c6c  d_wire0 = unfill
-00028ba0: 6574 6564 5f77 6972 6530 2e66 696c 6c65  eted_wire0.fille
-00028bb0: 7432 4428 302e 352c 2077 305f 7665 7274  t2D(0.5, w0_vert
-00028bc0: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00028bd0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00028be0: 2866 696c 6c65 7465 645f 7769 7265 302e  (filleted_wire0.
-00028bf0: 5665 7274 6963 6573 2829 292c 2034 290a  Vertices()), 4).
-00028c00: 0a20 2020 2020 2020 2023 2074 6865 2066  .        # the f
-00028c10: 696c 6c65 7465 6420 7769 7265 2069 7320  illeted wire is 
-00028c20: 7368 6f72 7465 7220 7468 616e 2074 6865  shorter than the
-00028c30: 206f 7269 6769 6e61 6c0a 2020 2020 2020   original.      
-00028c40: 2020 7365 6c66 2e61 7373 6572 7447 7265    self.assertGre
-00028c50: 6174 6572 2875 6e66 696c 6c65 7465 645f  ater(unfilleted_
-00028c60: 7769 7265 302e 4c65 6e67 7468 2829 202d  wire0.Length() -
-00028c70: 2066 696c 6c65 7465 645f 7769 7265 302e   filleted_wire0.
-00028c80: 4c65 6e67 7468 2829 2c20 302e 3129 0a0a  Length(), 0.1)..
-00028c90: 2020 2020 6465 6620 7465 7374 3244 6368      def test2Dch
-00028ca0: 616d 6665 7228 7365 6c66 293a 0a0a 2020  amfer(self):..  
-00028cb0: 2020 2020 2020 7220 3d20 576f 726b 706c        r = Workpl
-00028cc0: 616e 6528 292e 7265 6374 2831 2c20 3229  ane().rect(1, 2)
-00028cd0: 2e77 6972 6573 2829 2e76 616c 2829 0a20  .wires().val(). 
-00028ce0: 2020 2020 2020 2066 203d 2046 6163 652e         f = Face.
-00028cf0: 6d61 6b65 4672 6f6d 5769 7265 7328 7229  makeFromWires(r)
-00028d00: 0a20 2020 2020 2020 2076 6572 7473 203d  .        verts =
-00028d10: 2072 2e56 6572 7469 6365 7328 290a 0a20   r.Vertices().. 
-00028d20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00028d30: 7274 4571 7561 6c28 6c65 6e28 662e 6368  rtEqual(len(f.ch
-00028d40: 616d 6665 7232 4428 302e 352c 2076 6572  amfer2D(0.5, ver
-00028d50: 7473 292e 5665 7274 6963 6573 2829 292c  ts).Vertices()),
-00028d60: 2036 290a 2020 2020 2020 2020 7365 6c66   6).        self
-00028d70: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00028d80: 2872 2e63 6861 6d66 6572 3244 2830 2e35  (r.chamfer2D(0.5
-00028d90: 2c20 7665 7274 7329 2e56 6572 7469 6365  , verts).Vertice
-00028da0: 7328 2929 2c20 3629 0a20 2020 2020 2020  s()), 6).       
-00028db0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00028dc0: 6c28 6c65 6e28 722e 6368 616d 6665 7232  l(len(r.chamfer2
-00028dd0: 4428 302e 3235 2c20 7665 7274 7329 2e56  D(0.25, verts).V
-00028de0: 6572 7469 6365 7328 2929 2c20 3829 0a0a  ertices()), 8)..
-00028df0: 2020 2020 2020 2020 7220 3d20 576f 726b          r = Work
-00028e00: 706c 616e 6528 292e 684c 696e 6528 3129  plane().hLine(1)
-00028e10: 2e76 4c69 6e65 2831 292e 7769 7265 2829  .vLine(1).wire()
-00028e20: 2e76 616c 2829 0a20 2020 2020 2020 2076  .val().        v
-00028e30: 7320 3d20 722e 5665 7274 6963 6573 2829  s = r.Vertices()
-00028e40: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00028e50: 7373 6572 7445 7175 616c 286c 656e 2872  ssertEqual(len(r
-00028e60: 2e63 6861 6d66 6572 3244 2830 2e32 352c  .chamfer2D(0.25,
-00028e70: 205b 7673 5b31 5d5d 292e 5665 7274 6963   [vs[1]]).Vertic
-00028e80: 6573 2829 292c 2034 290a 0a20 2020 2020  es()), 4)..     
-00028e90: 2020 2077 6974 6820 7261 6973 6573 2856     with raises(V
-00028ea0: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
-00028eb0: 2020 2020 2020 2020 722e 6368 616d 6665          r.chamfe
-00028ec0: 7232 4428 302e 3235 2c20 5b76 735b 305d  r2D(0.25, [vs[0]
-00028ed0: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
-00028ee0: 5f46 6163 655f 6d61 6b65 4672 6f6d 5769  _Face_makeFromWi
-00028ef0: 7265 7328 7365 6c66 293a 0a0a 2020 2020  res(self):..    
-00028f00: 2020 2020 7730 203d 2057 6972 652e 6173      w0 = Wire.as
-00028f10: 7365 6d62 6c65 4564 6765 7328 0a20 2020  sembleEdges(.   
-00028f20: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00028f30: 2020 2020 2020 2020 2020 2045 6467 652e             Edge.
-00028f40: 6d61 6b65 4c69 6e65 2856 6563 746f 7228  makeLine(Vector(
-00028f50: 292c 2056 6563 746f 7228 302c 2031 2929  ), Vector(0, 1))
-00028f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00028f70: 2020 4564 6765 2e6d 616b 654c 696e 6528    Edge.makeLine(
-00028f80: 5665 6374 6f72 2830 2c20 3129 2c20 5665  Vector(0, 1), Ve
-00028f90: 6374 6f72 2831 2c20 3129 292c 0a20 2020  ctor(1, 1)),.   
-00028fa0: 2020 2020 2020 2020 2020 2020 2045 6467               Edg
-00028fb0: 652e 6d61 6b65 4c69 6e65 2856 6563 746f  e.makeLine(Vecto
-00028fc0: 7228 312c 2031 292c 2056 6563 746f 7228  r(1, 1), Vector(
-00028fd0: 312c 2030 2929 2c0a 2020 2020 2020 2020  1, 0)),.        
-00028fe0: 2020 2020 2020 2020 4564 6765 2e6d 616b          Edge.mak
-00028ff0: 654c 696e 6528 5665 6374 6f72 2831 2c20  eLine(Vector(1, 
-00029000: 3029 2c20 5665 6374 6f72 2830 2c20 3029  0), Vector(0, 0)
-00029010: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
-00029020: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00029030: 2020 2077 3120 3d20 5769 7265 2e61 7373     w1 = Wire.ass
-00029040: 656d 626c 6545 6467 6573 280a 2020 2020  embleEdges(.    
-00029050: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00029060: 2020 2020 2020 2020 2020 4564 6765 2e6d            Edge.m
-00029070: 616b 654c 696e 6528 5665 6374 6f72 2830  akeLine(Vector(0
-00029080: 2e32 352c 2030 2e32 3529 2c20 5665 6374  .25, 0.25), Vect
-00029090: 6f72 2830 2e32 352c 2030 2e37 3529 292c  or(0.25, 0.75)),
-000290a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000290b0: 2045 6467 652e 6d61 6b65 4c69 6e65 2856   Edge.makeLine(V
-000290c0: 6563 746f 7228 302e 3235 2c20 302e 3735  ector(0.25, 0.75
-000290d0: 292c 2056 6563 746f 7228 302e 3735 2c20  ), Vector(0.75, 
-000290e0: 302e 3735 2929 2c0a 2020 2020 2020 2020  0.75)),.        
-000290f0: 2020 2020 2020 2020 4564 6765 2e6d 616b          Edge.mak
-00029100: 654c 696e 6528 5665 6374 6f72 2830 2e37  eLine(Vector(0.7
-00029110: 352c 2030 2e37 3529 2c20 5665 6374 6f72  5, 0.75), Vector
-00029120: 2830 2e37 352c 2030 2e32 3529 292c 0a20  (0.75, 0.25)),. 
-00029130: 2020 2020 2020 2020 2020 2020 2020 2045                 E
-00029140: 6467 652e 6d61 6b65 4c69 6e65 2856 6563  dge.makeLine(Vec
-00029150: 746f 7228 302e 3735 2c20 302e 3235 292c  tor(0.75, 0.25),
-00029160: 2056 6563 746f 7228 302e 3235 2c20 302e   Vector(0.25, 0.
-00029170: 3235 2929 2c0a 2020 2020 2020 2020 2020  25)),.          
-00029180: 2020 5d0a 2020 2020 2020 2020 290a 2020    ].        ).  
-00029190: 2020 2020 2020 6620 3d20 4661 6365 2e6d        f = Face.m
-000291a0: 616b 6546 726f 6d57 6972 6573 2877 302c  akeFromWires(w0,
-000291b0: 205b 7731 5d29 0a20 2020 2020 2020 2061   [w1]).        a
-000291c0: 7373 6572 7420 662e 6973 5661 6c69 6428  ssert f.isValid(
-000291d0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-000291e0: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
-000291f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00029200: 7730 203d 2057 6972 652e 6173 7365 6d62  w0 = Wire.assemb
-00029210: 6c65 4564 6765 7328 5b45 6467 652e 6d61  leEdges([Edge.ma
-00029220: 6b65 4c69 6e65 2856 6563 746f 7228 292c  keLine(Vector(),
-00029230: 2056 6563 746f 7228 302c 2031 2929 2c5d   Vector(0, 1)),]
-00029240: 290a 2020 2020 2020 2020 2020 2020 7731  ).            w1
-00029250: 203d 2057 6972 652e 6173 7365 6d62 6c65   = Wire.assemble
-00029260: 4564 6765 7328 5b45 6467 652e 6d61 6b65  Edges([Edge.make
-00029270: 4c69 6e65 2856 6563 746f 7228 302c 2031  Line(Vector(0, 1
-00029280: 292c 2056 6563 746f 7228 312c 2031 2929  ), Vector(1, 1))
-00029290: 2c5d 290a 2020 2020 2020 2020 2020 2020  ,]).            
-000292a0: 6620 3d20 4661 6365 2e6d 616b 6546 726f  f = Face.makeFro
-000292b0: 6d57 6972 6573 2877 302c 205b 7731 5d29  mWires(w0, [w1])
-000292c0: 0a0a 2020 2020 2020 2020 7769 7468 2072  ..        with r
-000292d0: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
-000292e0: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-000292f0: 3020 3d20 5769 7265 2e61 7373 656d 626c  0 = Wire.assembl
-00029300: 6545 6467 6573 285b 4564 6765 2e6d 616b  eEdges([Edge.mak
-00029310: 654c 696e 6528 5665 6374 6f72 2829 2c20  eLine(Vector(), 
-00029320: 5665 6374 6f72 2830 2c20 3129 292c 5d29  Vector(0, 1)),])
-00029330: 0a20 2020 2020 2020 2020 2020 2077 3120  .            w1 
-00029340: 3d20 5769 7265 2e61 7373 656d 626c 6545  = Wire.assembleE
-00029350: 6467 6573 280a 2020 2020 2020 2020 2020  dges(.          
-00029360: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00029370: 2020 2020 2020 2020 2020 2020 4564 6765              Edge
-00029380: 2e6d 616b 654c 696e 6528 5665 6374 6f72  .makeLine(Vector
-00029390: 2829 2c20 5665 6374 6f72 2831 2c20 3129  (), Vector(1, 1)
-000293a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000293b0: 2020 2020 2020 2045 6467 652e 6d61 6b65         Edge.make
-000293c0: 4c69 6e65 2856 6563 746f 7228 312c 2031  Line(Vector(1, 1
-000293d0: 292c 2056 6563 746f 7228 322c 2030 2929  ), Vector(2, 0))
-000293e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000293f0: 2020 2020 2020 4564 6765 2e6d 616b 654c        Edge.makeL
-00029400: 696e 6528 5665 6374 6f72 2832 2c20 3029  ine(Vector(2, 0)
-00029410: 2c20 5665 6374 6f72 2830 2c20 3029 292c  , Vector(0, 0)),
-00029420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029430: 205d 0a20 2020 2020 2020 2020 2020 2029   ].            )
-00029440: 0a20 2020 2020 2020 2020 2020 2066 203d  .            f =
-00029450: 2046 6163 652e 6d61 6b65 4672 6f6d 5769   Face.makeFromWi
-00029460: 7265 7328 7730 2c20 5b77 315d 290a 0a20  res(w0, [w1]).. 
-00029470: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
-00029480: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
-00029490: 2020 2020 2020 2020 2020 2020 7730 203d              w0 =
-000294a0: 2057 6972 652e 6173 7365 6d62 6c65 4564   Wire.assembleEd
-000294b0: 6765 7328 0a20 2020 2020 2020 2020 2020  ges(.           
-000294c0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-000294d0: 2020 2020 2020 2020 2020 2045 6467 652e             Edge.
-000294e0: 6d61 6b65 4c69 6e65 2856 6563 746f 7228  makeLine(Vector(
-000294f0: 292c 2056 6563 746f 7228 312c 2031 2929  ), Vector(1, 1))
-00029500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00029510: 2020 2020 2020 4564 6765 2e6d 616b 654c        Edge.makeL
-00029520: 696e 6528 5665 6374 6f72 2831 2c20 3129  ine(Vector(1, 1)
-00029530: 2c20 5665 6374 6f72 2832 2c20 3029 292c  , Vector(2, 0)),
-00029540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029550: 2020 2020 2045 6467 652e 6d61 6b65 4c69       Edge.makeLi
-00029560: 6e65 2856 6563 746f 7228 322c 2030 292c  ne(Vector(2, 0),
-00029570: 2056 6563 746f 7228 302c 2030 2929 2c0a   Vector(0, 0)),.
-00029580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029590: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-000295a0: 2020 2020 2020 2020 2020 2020 7731 203d              w1 =
-000295b0: 2057 6972 652e 6173 7365 6d62 6c65 4564   Wire.assembleEd
-000295c0: 6765 7328 0a20 2020 2020 2020 2020 2020  ges(.           
-000295d0: 2020 2020 205b 4564 6765 2e6d 616b 654c       [Edge.makeL
-000295e0: 696e 6528 5665 6374 6f72 2830 2e31 2c20  ine(Vector(0.1, 
-000295f0: 302e 3129 2c20 5665 6374 6f72 2830 2e32  0.1), Vector(0.2
-00029600: 2c20 302e 3229 292c 5d0a 2020 2020 2020  , 0.2)),].      
-00029610: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00029620: 2020 2020 6620 3d20 4661 6365 2e6d 616b      f = Face.mak
-00029630: 6546 726f 6d57 6972 6573 2877 302c 205b  eFromWires(w0, [
-00029640: 7731 5d29 0a0a 2020 2020 6465 6620 7465  w1])..    def te
-00029650: 7374 5370 6c69 6e65 4170 7072 6f78 2873  stSplineApprox(s
-00029660: 656c 6629 3a0a 0a20 2020 2020 2020 2066  elf):..        f
-00029670: 726f 6d20 2e6e 6163 6120 696d 706f 7274  rom .naca import
-00029680: 206e 6163 6135 3330 350a 2020 2020 2020   naca5305.      
-00029690: 2020 6672 6f6d 206d 6174 6820 696d 706f    from math impo
-000296a0: 7274 2070 692c 2063 6f73 0a0a 2020 2020  rt pi, cos..    
-000296b0: 2020 2020 7074 7320 3d20 5b56 6563 746f      pts = [Vecto
-000296c0: 7228 655b 305d 2c20 655b 315d 2c20 3029  r(e[0], e[1], 0)
-000296d0: 2066 6f72 2065 2069 6e20 6e61 6361 3533   for e in naca53
-000296e0: 3035 5d0a 0a20 2020 2020 2020 2023 2073  05]..        # s
-000296f0: 706c 696e 650a 0a20 2020 2020 2020 2065  pline..        e
-00029700: 3120 3d20 4564 6765 2e6d 616b 6553 706c  1 = Edge.makeSpl
-00029710: 696e 6541 7070 726f 7828 7074 732c 2031  ineApprox(pts, 1
-00029720: 652d 362c 206d 6178 4465 673d 362c 2073  e-6, maxDeg=6, s
-00029730: 6d6f 6f74 6869 6e67 3d28 312c 2031 2c20  moothing=(1, 1, 
-00029740: 3129 290a 2020 2020 2020 2020 6532 203d  1)).        e2 =
-00029750: 2045 6467 652e 6d61 6b65 5370 6c69 6e65   Edge.makeSpline
-00029760: 4170 7072 6f78 2870 7473 2c20 3165 2d36  Approx(pts, 1e-6
-00029770: 2c20 6d69 6e44 6567 3d32 2c20 6d61 7844  , minDeg=2, maxD
-00029780: 6567 3d36 290a 0a20 2020 2020 2020 2073  eg=6)..        s
-00029790: 656c 662e 6173 7365 7274 5472 7565 2865  elf.assertTrue(e
-000297a0: 312e 6973 5661 6c69 6428 2929 0a20 2020  1.isValid()).   
-000297b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000297c0: 5472 7565 2865 322e 6973 5661 6c69 6428  True(e2.isValid(
-000297d0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000297e0: 6173 7365 7274 5472 7565 2865 312e 4c65  assertTrue(e1.Le
-000297f0: 6e67 7468 2829 203e 2065 322e 4c65 6e67  ngth() > e2.Leng
-00029800: 7468 2829 290a 0a20 2020 2020 2020 2077  th())..        w
-00029810: 6974 6820 7261 6973 6573 2856 616c 7565  ith raises(Value
-00029820: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00029830: 2020 2020 6534 203d 2045 6467 652e 6d61      e4 = Edge.ma
-00029840: 6b65 5370 6c69 6e65 4170 7072 6f78 2870  keSplineApprox(p
-00029850: 7473 2c20 3165 2d36 2c20 6d61 7844 6567  ts, 1e-6, maxDeg
-00029860: 3d33 2c20 736d 6f6f 7468 696e 673d 2831  =3, smoothing=(1
-00029870: 2c20 312c 2031 2e30 2929 0a0a 2020 2020  , 1, 1.0))..    
-00029880: 2020 2020 7074 735f 636c 6f73 6564 203d      pts_closed =
-00029890: 2070 7473 202b 205b 7074 735b 305d 5d0a   pts + [pts[0]].
-000298a0: 0a20 2020 2020 2020 2065 3320 3d20 4564  .        e3 = Ed
-000298b0: 6765 2e6d 616b 6553 706c 696e 6541 7070  ge.makeSplineApp
-000298c0: 726f 7828 7074 735f 636c 6f73 6564 290a  rox(pts_closed).
-000298d0: 2020 2020 2020 2020 7720 3d20 4564 6765          w = Edge
-000298e0: 2e6d 616b 6553 706c 696e 6541 7070 726f  .makeSplineAppro
-000298f0: 7828 7074 7329 2e63 6c6f 7365 2829 0a0a  x(pts).close()..
-00029900: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00029910: 6572 7454 7275 6528 6533 2e49 7343 6c6f  ertTrue(e3.IsClo
-00029920: 7365 6428 2929 0a20 2020 2020 2020 2073  sed()).        s
-00029930: 656c 662e 6173 7365 7274 5472 7565 2877  elf.assertTrue(w
-00029940: 2e49 7343 6c6f 7365 6428 2929 0a0a 2020  .IsClosed())..  
-00029950: 2020 2020 2020 2320 576f 726b 706c 616e        # Workplan
-00029960: 6520 6d65 7468 6f64 0a0a 2020 2020 2020  e method..      
-00029970: 2020 7731 203d 2057 6f72 6b70 6c61 6e65    w1 = Workplane
-00029980: 2829 2e73 706c 696e 6541 7070 726f 7828  ().splineApprox(
-00029990: 7074 7329 0a20 2020 2020 2020 2077 3220  pts).        w2 
-000299a0: 3d20 576f 726b 706c 616e 6528 292e 7370  = Workplane().sp
-000299b0: 6c69 6e65 4170 7072 6f78 2870 7473 2c20  lineApprox(pts, 
-000299c0: 666f 7243 6f6e 7374 7275 6374 696f 6e3d  forConstruction=
-000299d0: 5472 7565 290a 2020 2020 2020 2020 7733  True).        w3
-000299e0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e73   = Workplane().s
-000299f0: 706c 696e 6541 7070 726f 7828 7074 732c  plineApprox(pts,
-00029a00: 206d 616b 6557 6972 653d 5472 7565 290a   makeWire=True).
-00029a10: 2020 2020 2020 2020 7734 203d 2057 6f72          w4 = Wor
-00029a20: 6b70 6c61 6e65 2829 2e73 706c 696e 6541  kplane().splineA
-00029a30: 7070 726f 7828 7074 732c 206d 616b 6557  pprox(pts, makeW
-00029a40: 6972 653d 5472 7565 2c20 666f 7243 6f6e  ire=True, forCon
-00029a50: 7374 7275 6374 696f 6e3d 5472 7565 290a  struction=True).
-00029a60: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00029a70: 7365 7274 4571 7561 6c28 7731 2e65 6467  sertEqual(w1.edg
-00029a80: 6573 2829 2e73 697a 6528 292c 2031 290a  es().size(), 1).
-00029a90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00029aa0: 6572 7445 7175 616c 286c 656e 2877 312e  ertEqual(len(w1.
-00029ab0: 6374 782e 7065 6e64 696e 6745 6467 6573  ctx.pendingEdges
-00029ac0: 292c 2031 290a 2020 2020 2020 2020 7365  ), 1).        se
-00029ad0: 6c66 2e61 7373 6572 7445 7175 616c 2877  lf.assertEqual(w
-00029ae0: 322e 6564 6765 7328 292e 7369 7a65 2829  2.edges().size()
-00029af0: 2c20 3129 0a20 2020 2020 2020 2073 656c  , 1).        sel
-00029b00: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00029b10: 6e28 7732 2e63 7478 2e70 656e 6469 6e67  n(w2.ctx.pending
-00029b20: 4564 6765 7329 2c20 3029 0a20 2020 2020  Edges), 0).     
-00029b30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00029b40: 7561 6c28 7733 2e77 6972 6573 2829 2e73  ual(w3.wires().s
-00029b50: 697a 6528 292c 2031 290a 2020 2020 2020  ize(), 1).      
-00029b60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00029b70: 616c 286c 656e 2877 332e 6374 782e 7065  al(len(w3.ctx.pe
-00029b80: 6e64 696e 6757 6972 6573 292c 2031 290a  ndingWires), 1).
-00029b90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00029ba0: 6572 7445 7175 616c 2877 342e 7769 7265  ertEqual(w4.wire
-00029bb0: 7328 292e 7369 7a65 2829 2c20 3129 0a20  s().size(), 1). 
-00029bc0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00029bd0: 7274 4571 7561 6c28 6c65 6e28 7734 2e63  rtEqual(len(w4.c
-00029be0: 7478 2e70 656e 6469 6e67 5769 7265 7329  tx.pendingWires)
-00029bf0: 2c20 3029 0a0a 2020 2020 2020 2020 2320  , 0)..        # 
-00029c00: 7370 6c69 6e65 2073 7572 6661 6365 0a0a  spline surface..
-00029c10: 2020 2020 2020 2020 4e20 3d20 3430 0a20          N = 40. 
-00029c20: 2020 2020 2020 2054 203d 2032 300a 2020         T = 20.  
-00029c30: 2020 2020 2020 4120 3d20 350a 0a20 2020        A = 5..   
-00029c40: 2020 2020 2070 7473 203d 205b 0a20 2020       pts = [.   
-00029c50: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00029c60: 2020 2020 2020 2020 2020 2056 6563 746f             Vecto
-00029c70: 7228 692c 206a 2c20 4120 2a20 636f 7328  r(i, j, A * cos(
-00029c80: 3220 2a20 7069 202a 2069 202f 2054 2920  2 * pi * i / T) 
-00029c90: 2a20 636f 7328 3220 2a20 7069 202a 206a  * cos(2 * pi * j
-00029ca0: 202f 2054 2929 0a20 2020 2020 2020 2020   / T)).         
-00029cb0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00029cc0: 7261 6e67 6528 4e20 2b20 3129 0a20 2020  range(N + 1).   
-00029cd0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00029ce0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-00029cf0: 7261 6e67 6528 4e20 2b20 3129 0a20 2020  range(N + 1).   
-00029d00: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
-00029d10: 6631 203d 2046 6163 652e 6d61 6b65 5370  f1 = Face.makeSp
-00029d20: 6c69 6e65 4170 7072 6f78 2870 7473 2c20  lineApprox(pts, 
-00029d30: 736d 6f6f 7468 696e 673d 2831 2c20 312c  smoothing=(1, 1,
-00029d40: 2031 292c 206d 6178 4465 673d 3629 0a20   1), maxDeg=6). 
-00029d50: 2020 2020 2020 2066 3220 3d20 4661 6365         f2 = Face
-00029d60: 2e6d 616b 6553 706c 696e 6541 7070 726f  .makeSplineAppro
-00029d70: 7828 7074 7329 0a0a 2020 2020 2020 2020  x(pts)..        
-00029d80: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00029d90: 6631 2e69 7356 616c 6964 2829 290a 2020  f1.isValid()).  
-00029da0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00029db0: 7454 7275 6528 6632 2e69 7356 616c 6964  tTrue(f2.isValid
-00029dc0: 2829 290a 0a20 2020 2020 2020 2077 6974  ())..        wit
-00029dd0: 6820 7261 6973 6573 2856 616c 7565 4572  h raises(ValueEr
-00029de0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-00029df0: 2020 6633 203d 2046 6163 652e 6d61 6b65    f3 = Face.make
-00029e00: 5370 6c69 6e65 4170 7072 6f78 2870 7473  SplineApprox(pts
-00029e10: 2c20 736d 6f6f 7468 696e 673d 2831 2c20  , smoothing=(1, 
-00029e20: 312c 2031 292c 206d 6178 4465 673d 3329  1, 1), maxDeg=3)
-00029e30: 0a0a 2020 2020 6465 6620 7465 7374 5061  ..    def testPa
-00029e40: 7261 6d65 7472 6963 5375 7266 6163 6528  rametricSurface(
-00029e50: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-00029e60: 6672 6f6d 206d 6174 6820 696d 706f 7274  from math import
-00029e70: 2070 692c 2063 6f73 0a0a 2020 2020 2020   pi, cos..      
-00029e80: 2020 7231 203d 2057 6f72 6b70 6c61 6e65    r1 = Workplane
-00029e90: 2829 2e70 6172 616d 6574 7269 6353 7572  ().parametricSur
-00029ea0: 6661 6365 280a 2020 2020 2020 2020 2020  face(.          
-00029eb0: 2020 6c61 6d62 6461 2075 2c20 763a 2028    lambda u, v: (
-00029ec0: 752c 2076 2c20 636f 7328 7069 202a 2075  u, v, cos(pi * u
-00029ed0: 2920 2a20 636f 7328 7069 202a 2076 2929  ) * cos(pi * v))
-00029ee0: 2c20 7374 6172 743d 2d31 2c20 7374 6f70  , start=-1, stop
-00029ef0: 3d31 0a20 2020 2020 2020 2029 0a0a 2020  =1.        )..  
-00029f00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00029f10: 7454 7275 6528 7231 2e66 6163 6573 2829  tTrue(r1.faces()
-00029f20: 2e76 616c 2829 2e69 7356 616c 6964 2829  .val().isValid()
-00029f30: 290a 0a20 2020 2020 2020 2072 3220 3d20  )..        r2 = 
-00029f40: 576f 726b 706c 616e 6528 292e 626f 7828  Workplane().box(
-00029f50: 312c 2031 2c20 3329 2e73 706c 6974 2872  1, 1, 3).split(r
-00029f60: 3129 0a0a 2020 2020 2020 2020 7365 6c66  1)..        self
-00029f70: 2e61 7373 6572 7454 7275 6528 7232 2e73  .assertTrue(r2.s
-00029f80: 6f6c 6964 7328 292e 7661 6c28 292e 6973  olids().val().is
-00029f90: 5661 6c69 6428 2929 0a20 2020 2020 2020  Valid()).       
-00029fa0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00029fb0: 6c28 7232 2e73 6f6c 6964 7328 292e 7369  l(r2.solids().si
-00029fc0: 7a65 2829 2c20 3229 0a0a 2020 2020 6465  ze(), 2)..    de
-00029fd0: 6620 7465 7374 4564 6765 5769 7265 436c  f testEdgeWireCl
-00029fe0: 6f73 6528 7365 6c66 293a 0a0a 2020 2020  ose(self):..    
-00029ff0: 2020 2020 2320 7465 7374 2077 6974 6820      # test with 
-0002a000: 6564 6765 0a20 2020 2020 2020 2065 3020  edge.        e0 
-0002a010: 3d20 4564 6765 2e6d 616b 6554 6872 6565  = Edge.makeThree
-0002a020: 506f 696e 7441 7263 2856 6563 746f 7228  PointArc(Vector(
-0002a030: 302c 2030 2c20 3029 2c20 5665 6374 6f72  0, 0, 0), Vector
-0002a040: 2831 2c20 312c 2030 292c 2056 6563 746f  (1, 1, 0), Vecto
-0002a050: 7228 302c 2032 2c20 3029 290a 2020 2020  r(0, 2, 0)).    
-0002a060: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-0002a070: 616c 7365 2865 302e 4973 436c 6f73 6564  alse(e0.IsClosed
-0002a080: 2829 290a 2020 2020 2020 2020 7730 203d  ()).        w0 =
-0002a090: 2065 302e 636c 6f73 6528 290a 2020 2020   e0.close().    
-0002a0a0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-0002a0b0: 7275 6528 7730 2e49 7343 6c6f 7365 6428  rue(w0.IsClosed(
-0002a0c0: 2929 0a0a 2020 2020 2020 2020 2320 7465  ))..        # te
-0002a0d0: 7374 2077 6974 6820 616c 7265 6164 7920  st with already 
-0002a0e0: 636c 6f73 6564 2065 6467 650a 2020 2020  closed edge.    
-0002a0f0: 2020 2020 6531 203d 2045 6467 652e 6d61      e1 = Edge.ma
-0002a100: 6b65 4369 7263 6c65 2831 290a 2020 2020  keCircle(1).    
-0002a110: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-0002a120: 7275 6528 6531 2e49 7343 6c6f 7365 6428  rue(e1.IsClosed(
-0002a130: 2929 0a20 2020 2020 2020 2065 3220 3d20  )).        e2 = 
-0002a140: 6531 2e63 6c6f 7365 2829 0a20 2020 2020  e1.close().     
-0002a150: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-0002a160: 7565 2865 322e 4973 436c 6f73 6564 2829  ue(e2.IsClosed()
-0002a170: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002a180: 7373 6572 7445 7175 616c 2874 7970 6528  ssertEqual(type(
-0002a190: 6531 292c 2074 7970 6528 6532 2929 0a0a  e1), type(e2))..
-0002a1a0: 2020 2020 2020 2020 2320 7465 7374 2077          # test w
-0002a1b0: 6974 6820 616c 7265 6164 7920 636c 6f73  ith already clos
-0002a1c0: 6564 2057 4952 450a 2020 2020 2020 2020  ed WIRE.        
-0002a1d0: 7731 203d 2057 6972 652e 6d61 6b65 4369  w1 = Wire.makeCi
-0002a1e0: 7263 6c65 2831 2c20 5665 6374 6f72 2829  rcle(1, Vector()
-0002a1f0: 2c20 5665 6374 6f72 2830 2c20 302c 2031  , Vector(0, 0, 1
-0002a200: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0002a210: 6173 7365 7274 5472 7565 2877 312e 4973  assertTrue(w1.Is
-0002a220: 436c 6f73 6564 2829 290a 2020 2020 2020  Closed()).      
-0002a230: 2020 7732 203d 2077 312e 636c 6f73 6528    w2 = w1.close(
-0002a240: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002a250: 7373 6572 7454 7275 6528 7731 2069 7320  ssertTrue(w1 is 
-0002a260: 7732 290a 0a20 2020 2064 6566 2074 6573  w2)..    def tes
-0002a270: 7453 706c 6974 5368 6170 6528 7365 6c66  tSplitShape(self
-0002a280: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0002a290: 2020 2020 2020 2054 6573 7469 6e67 2074         Testing t
-0002a2a0: 6865 2053 6861 7065 2e73 706c 6974 206d  he Shape.split m
-0002a2b0: 6574 686f 642e 0a20 2020 2020 2020 2022  ethod..        "
-0002a2c0: 2222 0a20 2020 2020 2020 2023 2073 706c  "".        # spl
-0002a2d0: 6974 2061 6e20 6564 6765 2077 6974 6820  it an edge with 
-0002a2e0: 6120 7665 7274 6578 0a20 2020 2020 2020  a vertex.       
-0002a2f0: 2065 3020 3d20 4564 6765 2e6d 616b 6543   e0 = Edge.makeC
-0002a300: 6972 636c 6528 312c 2028 302c 2030 2c20  ircle(1, (0, 0, 
-0002a310: 3029 2c20 2830 2c20 302c 2031 2929 0a20  0), (0, 0, 1)). 
-0002a320: 2020 2020 2020 2076 3020 3d20 5665 7274         v0 = Vert
-0002a330: 6578 2e6d 616b 6556 6572 7465 7828 302c  ex.makeVertex(0,
-0002a340: 2031 2c20 3029 0a20 2020 2020 2020 206c   1, 0).        l
-0002a350: 6973 745f 6f66 5f65 6467 6573 203d 2065  ist_of_edges = e
-0002a360: 302e 7370 6c69 7428 7630 292e 4564 6765  0.split(v0).Edge
-0002a370: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
-0002a380: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-0002a390: 286c 6973 745f 6f66 5f65 6467 6573 292c  (list_of_edges),
-0002a3a0: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-0002a3b0: 2e61 7373 6572 7454 7275 6528 5665 6374  .assertTrue(Vect
-0002a3c0: 6f72 2830 2c20 312c 2030 2920 696e 205b  or(0, 1, 0) in [
-0002a3d0: 652e 656e 6450 6f69 6e74 2829 2066 6f72  e.endPoint() for
-0002a3e0: 2065 2069 6e20 6c69 7374 5f6f 665f 6564   e in list_of_ed
-0002a3f0: 6765 735d 290a 0a20 2020 2020 2020 2023  ges])..        #
-0002a400: 2073 706c 6974 2061 2063 6972 636c 6520   split a circle 
-0002a410: 7769 7468 206d 756c 7469 706c 6520 7665  with multiple ve
-0002a420: 7274 6963 6573 0a20 2020 2020 2020 2061  rtices.        a
-0002a430: 6e67 6c65 7320 3d20 5b32 202a 206d 6174  ngles = [2 * mat
-0002a440: 682e 7069 202a 2069 6478 202f 2031 3020  h.pi * idx / 10 
-0002a450: 666f 7220 6964 7820 696e 2072 616e 6765  for idx in range
-0002a460: 2831 3029 5d0a 2020 2020 2020 2020 7665  (10)].        ve
-0002a470: 6373 203d 205b 5665 6374 6f72 286d 6174  cs = [Vector(mat
-0002a480: 682e 7369 6e28 6129 2c20 6d61 7468 2e63  h.sin(a), math.c
-0002a490: 6f73 2861 292c 2030 2920 666f 7220 6120  os(a), 0) for a 
-0002a4a0: 696e 2061 6e67 6c65 735d 0a20 2020 2020  in angles].     
-0002a4b0: 2020 2076 6572 7469 6365 7320 3d20 5b56     vertices = [V
-0002a4c0: 6572 7465 782e 6d61 6b65 5665 7274 6578  ertex.makeVertex
-0002a4d0: 282a 762e 746f 5475 706c 6528 2929 2066  (*v.toTuple()) f
-0002a4e0: 6f72 2076 2069 6e20 7665 6373 5d0a 2020  or v in vecs].  
-0002a4f0: 2020 2020 2020 6564 6765 7320 3d20 6530        edges = e0
-0002a500: 2e73 706c 6974 282a 7665 7274 6963 6573  .split(*vertices
-0002a510: 292e 4564 6765 7328 290a 2020 2020 2020  ).Edges().      
-0002a520: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002a530: 616c 286c 656e 2865 6467 6573 292c 206c  al(len(edges), l
-0002a540: 656e 2876 6572 7469 6365 7329 202b 2031  en(vertices) + 1
-0002a550: 290a 2020 2020 2020 2020 656e 6470 6f69  ).        endpoi
-0002a560: 6e74 7320 3d20 5b65 2e65 6e64 506f 696e  nts = [e.endPoin
-0002a570: 7428 2920 666f 7220 6520 696e 2065 6467  t() for e in edg
-0002a580: 6573 5d0a 2020 2020 2020 2020 7365 6c66  es].        self
-0002a590: 2e61 7373 6572 7454 7275 6528 616c 6c28  .assertTrue(all(
-0002a5a0: 5b76 2069 6e20 656e 6470 6f69 6e74 7320  [v in endpoints 
-0002a5b0: 666f 7220 7620 696e 2076 6563 735d 2929  for v in vecs]))
-0002a5c0: 0a0a 2020 2020 6465 6620 7465 7374 4272  ..    def testBr
-0002a5d0: 6570 496d 706f 7274 4578 706f 7274 2873  epImportExport(s
-0002a5e0: 656c 6629 3a0a 0a20 2020 2020 2020 2023  elf):..        #
-0002a5f0: 2069 6d70 6f72 742f 6578 706f 7274 2074   import/export t
-0002a600: 6f20 6669 6c65 0a20 2020 2020 2020 2073  o file.        s
-0002a610: 203d 2057 6f72 6b70 6c61 6e65 2829 2e62   = Workplane().b
-0002a620: 6f78 2831 2c20 312c 2031 292e 7661 6c28  ox(1, 1, 1).val(
-0002a630: 290a 0a20 2020 2020 2020 2073 2e65 7870  )..        s.exp
-0002a640: 6f72 7442 7265 7028 2274 6573 742e 6272  ortBrep("test.br
-0002a650: 6570 2229 0a20 2020 2020 2020 2073 6920  ep").        si 
-0002a660: 3d20 5368 6170 652e 696d 706f 7274 4272  = Shape.importBr
-0002a670: 6570 2822 7465 7374 2e62 7265 7022 290a  ep("test.brep").
-0002a680: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002a690: 7365 7274 5472 7565 2873 692e 6973 5661  sertTrue(si.isVa
-0002a6a0: 6c69 6428 2929 0a20 2020 2020 2020 2073  lid()).        s
-0002a6b0: 656c 662e 6173 7365 7274 416c 6d6f 7374  elf.assertAlmost
-0002a6c0: 4571 7561 6c28 7369 2e56 6f6c 756d 6528  Equal(si.Volume(
-0002a6d0: 292c 2031 290a 0a20 2020 2020 2020 2023  ), 1)..        #
-0002a6e0: 2069 6d70 6f72 742f 6578 706f 7274 2074   import/export t
-0002a6f0: 6f20 4279 7465 7349 4f0a 2020 2020 2020  o BytesIO.      
-0002a700: 2020 6672 6f6d 2069 6f20 696d 706f 7274    from io import
-0002a710: 2042 7974 6573 494f 0a0a 2020 2020 2020   BytesIO..      
-0002a720: 2020 6269 6f20 3d20 4279 7465 7349 4f28    bio = BytesIO(
-0002a730: 290a 0a20 2020 2020 2020 2073 2e65 7870  )..        s.exp
-0002a740: 6f72 7442 7265 7028 6269 6f29 0a20 2020  ortBrep(bio).   
-0002a750: 2020 2020 2062 696f 2e73 6565 6b28 3029       bio.seek(0)
-0002a760: 0a0a 2020 2020 2020 2020 7369 203d 2053  ..        si = S
-0002a770: 6861 7065 2e69 6d70 6f72 7442 7265 7028  hape.importBrep(
-0002a780: 2274 6573 742e 6272 6570 2229 0a0a 2020  "test.brep")..  
-0002a790: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002a7a0: 7454 7275 6528 7369 2e69 7356 616c 6964  tTrue(si.isValid
-0002a7b0: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
-0002a7c0: 2e61 7373 6572 7441 6c6d 6f73 7445 7175  .assertAlmostEqu
-0002a7d0: 616c 2873 692e 566f 6c75 6d65 2829 2c20  al(si.Volume(), 
-0002a7e0: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
-0002a7f0: 4661 6365 546f 506c 6e28 7365 6c66 293a  FaceToPln(self):
-0002a800: 0a0a 2020 2020 2020 2020 6f72 6967 696e  ..        origin
-0002a810: 203d 2028 312c 2032 2c20 3329 0a20 2020   = (1, 2, 3).   
-0002a820: 2020 2020 206e 6f72 6d61 6c20 3d20 2831       normal = (1
-0002a830: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-0002a840: 6630 203d 2046 6163 652e 6d61 6b65 506c  f0 = Face.makePl
-0002a850: 616e 6528 6c65 6e67 7468 3d4e 6f6e 652c  ane(length=None,
-0002a860: 2077 6964 7468 3d4e 6f6e 652c 2062 6173   width=None, bas
-0002a870: 6550 6e74 3d6f 7269 6769 6e2c 2064 6972  ePnt=origin, dir
-0002a880: 3d6e 6f72 6d61 6c29 0a20 2020 2020 2020  =normal).       
-0002a890: 2070 3020 3d20 6630 2e74 6f50 6c6e 2829   p0 = f0.toPln()
-0002a8a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0002a8b0: 7373 6572 7454 7275 6528 5665 6374 6f72  ssertTrue(Vector
-0002a8c0: 2870 302e 4c6f 6361 7469 6f6e 2829 2920  (p0.Location()) 
-0002a8d0: 3d3d 2056 6563 746f 7228 6f72 6967 696e  == Vector(origin
-0002a8e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0002a8f0: 6173 7365 7274 5472 7565 2856 6563 746f  assertTrue(Vecto
-0002a900: 7228 7030 2e41 7869 7328 292e 4469 7265  r(p0.Axis().Dire
-0002a910: 6374 696f 6e28 2929 203d 3d20 5665 6374  ction()) == Vect
-0002a920: 6f72 286e 6f72 6d61 6c29 2e6e 6f72 6d61  or(normal).norma
-0002a930: 6c69 7a65 6428 2929 0a0a 2020 2020 2020  lized())..      
-0002a940: 2020 6f72 6967 696e 3120 3d20 2830 2c20    origin1 = (0, 
-0002a950: 302c 202d 3329 0a20 2020 2020 2020 206e  0, -3).        n
-0002a960: 6f72 6d61 6c31 203d 2028 2d31 2c20 312c  ormal1 = (-1, 1,
-0002a970: 202d 3129 0a20 2020 2020 2020 2066 3120   -1).        f1 
-0002a980: 3d20 4661 6365 2e6d 616b 6550 6c61 6e65  = Face.makePlane
-0002a990: 286c 656e 6774 683d 302e 312c 2077 6964  (length=0.1, wid
-0002a9a0: 7468 3d31 3030 2c20 6261 7365 506e 743d  th=100, basePnt=
-0002a9b0: 6f72 6967 696e 312c 2064 6972 3d6e 6f72  origin1, dir=nor
-0002a9c0: 6d61 6c31 290a 2020 2020 2020 2020 7031  mal1).        p1
-0002a9d0: 203d 2066 312e 746f 506c 6e28 290a 0a20   = f1.toPln().. 
-0002a9e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0002a9f0: 7274 5472 7565 2856 6563 746f 7228 7031  rtTrue(Vector(p1
-0002aa00: 2e4c 6f63 6174 696f 6e28 2929 203d 3d20  .Location()) == 
-0002aa10: 5665 6374 6f72 286f 7269 6769 6e31 2929  Vector(origin1))
-0002aa20: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002aa30: 7365 7274 5472 7565 2856 6563 746f 7228  sertTrue(Vector(
-0002aa40: 7031 2e41 7869 7328 292e 4469 7265 6374  p1.Axis().Direct
-0002aa50: 696f 6e28 2929 203d 3d20 5665 6374 6f72  ion()) == Vector
-0002aa60: 286e 6f72 6d61 6c31 292e 6e6f 726d 616c  (normal1).normal
-0002aa70: 697a 6564 2829 290a 0a20 2020 2020 2020  ized())..       
-0002aa80: 2066 3220 3d20 576f 726b 706c 616e 6528   f2 = Workplane(
-0002aa90: 292e 626f 7828 312c 2031 2c20 3130 2c20  ).box(1, 1, 10, 
-0002aaa0: 6365 6e74 6572 6564 3d46 616c 7365 292e  centered=False).
-0002aab0: 6661 6365 7328 223e 5a22 292e 7661 6c28  faces(">Z").val(
-0002aac0: 290a 2020 2020 2020 2020 7032 203d 2066  ).        p2 = f
-0002aad0: 322e 746f 506c 6e28 290a 2020 2020 2020  2.toPln().      
-0002aae0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-0002aaf0: 6528 7032 2e43 6f6e 7461 696e 7328 6632  e(p2.Contains(f2
-0002ab00: 2e43 656e 7465 7228 292e 746f 506e 7428  .Center().toPnt(
-0002ab10: 292c 2030 2e31 2929 0a20 2020 2020 2020  ), 0.1)).       
-0002ab20: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0002ab30: 2856 6563 746f 7228 7032 2e41 7869 7328  (Vector(p2.Axis(
-0002ab40: 292e 4469 7265 6374 696f 6e28 2929 203d  ).Direction()) =
-0002ab50: 3d20 6632 2e6e 6f72 6d61 6c41 7428 2929  = f2.normalAt())
-0002ab60: 0a0a 2020 2020 6465 6620 7465 7374 4561  ..    def testEa
-0002ab70: 6368 706f 696e 7428 7365 6c66 293a 0a0a  chpoint(self):..
-0002ab80: 2020 2020 2020 2020 7231 203d 2028 0a20          r1 = (. 
-0002ab90: 2020 2020 2020 2020 2020 2057 6f72 6b70             Workp
-0002aba0: 6c61 6e65 286f 7269 6769 6e3d 2830 2c20  lane(origin=(0, 
-0002abb0: 302c 2031 2929 0a20 2020 2020 2020 2020  0, 1)).         
-0002abc0: 2020 202e 6164 6428 0a20 2020 2020 2020     .add(.       
-0002abd0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-0002abe0: 2020 2020 2020 2020 2020 2020 2020 2056                 V
-0002abf0: 6563 746f 7228 292c 0a20 2020 2020 2020  ector(),.       
-0002ac00: 2020 2020 2020 2020 2020 2020 204c 6f63               Loc
-0002ac10: 6174 696f 6e28 5665 6374 6f72 2830 2c20  ation(Vector(0, 
-0002ac20: 302c 202d 312c 2929 2c0a 2020 2020 2020  0, -1,)),.      
-0002ac30: 2020 2020 2020 2020 2020 2020 2020 536b                Sk
-0002ac40: 6574 6368 2829 2e72 6563 7428 312c 2031  etch().rect(1, 1
-0002ac50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0002ac60: 2020 2020 2020 2046 6163 652e 6d61 6b65         Face.make
-0002ac70: 506c 616e 6528 312c 2031 292c 0a20 2020  Plane(1, 1),.   
-0002ac80: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-0002ac90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002aca0: 2020 2020 2020 2020 202e 6561 6368 706f           .eachpo
-0002acb0: 696e 7428 6c61 6d62 6461 206c 3a20 4661  int(lambda l: Fa
-0002acc0: 6365 2e6d 616b 6550 6c61 6e65 2831 2c20  ce.makePlane(1, 
-0002acd0: 3129 2e6c 6f63 6174 6528 6c29 290a 2020  1).locate(l)).  
-0002ace0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0002acf0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0002ad00: 286c 656e 2872 312e 6f62 6a65 6374 7329  (len(r1.objects)
-0002ad10: 203d 3d20 3429 0a0a 2020 2020 2020 2020   == 4)..        
-0002ad20: 666f 7220 7620 696e 2072 312e 7661 6c73  for v in r1.vals
-0002ad30: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0002ad40: 7365 6c66 2e61 7373 6572 7454 7570 6c65  self.assertTuple
-0002ad50: 416c 6d6f 7374 4571 7561 6c73 2876 2e43  AlmostEquals(v.C
-0002ad60: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
-0002ad70: 292c 2028 302c 2030 2c20 3029 2c20 3629  ), (0, 0, 0), 6)
-0002ad80: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
-0002ad90: 2065 6163 6870 6f69 6e74 2077 6974 6820   eachpoint with 
-0002ada0: 636f 6d62 696e 6520 3d20 5472 7565 0a20  combine = True. 
-0002adb0: 2020 2020 2020 2062 6f78 203d 2057 6f72         box = Wor
-0002adc0: 6b70 6c61 6e65 2829 2e62 6f78 2832 2c20  kplane().box(2, 
-0002add0: 312c 2031 292e 7661 6c28 290a 2020 2020  1, 1).val().    
-0002ade0: 2020 2020 7265 6620 3d20 576f 726b 706c      ref = Workpl
-0002adf0: 616e 6528 292e 626f 7828 352c 2035 2c20  ane().box(5, 5, 
-0002ae00: 3529 0a20 2020 2020 2020 2072 203d 2072  5).        r = r
-0002ae10: 6566 2e76 6572 7469 6365 7328 292e 6561  ef.vertices().ea
-0002ae20: 6368 706f 696e 7428 6c61 6d62 6461 206c  chpoint(lambda l
-0002ae30: 6f63 3a20 626f 782e 6d6f 7665 6428 6c6f  oc: box.moved(lo
-0002ae40: 6329 2c20 636f 6d62 696e 653d 5472 7565  c), combine=True
-0002ae50: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002ae60: 7373 6572 7447 7265 6174 6572 2872 2e76  ssertGreater(r.v
-0002ae70: 616c 2829 2e56 6f6c 756d 6528 292c 2072  al().Volume(), r
-0002ae80: 6566 2e76 616c 2829 2e56 6f6c 756d 6528  ef.val().Volume(
-0002ae90: 2929 0a0a 2020 2020 2020 2020 2320 7465  ))..        # te
-0002aea0: 7374 2065 6163 6870 6f69 6e74 2077 6974  st eachpoint wit
-0002aeb0: 6820 636f 6d62 696e 6520 3d20 2263 7574  h combine = "cut
-0002aec0: 220a 2020 2020 2020 2020 7220 3d20 7265  ".        r = re
-0002aed0: 662e 7665 7274 6963 6573 2829 2e65 6163  f.vertices().eac
-0002aee0: 6870 6f69 6e74 286c 616d 6264 6120 6c6f  hpoint(lambda lo
-0002aef0: 633a 2062 6f78 2e6d 6f76 6564 286c 6f63  c: box.moved(loc
-0002af00: 292c 2063 6f6d 6269 6e65 3d22 6375 7422  ), combine="cut"
-0002af10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002af20: 7373 6572 7447 7265 6174 6572 2872 6566  ssertGreater(ref
-0002af30: 2e76 616c 2829 2e56 6f6c 756d 6528 292c  .val().Volume(),
-0002af40: 2072 2e76 616c 2829 2e56 6f6c 756d 6528   r.val().Volume(
-0002af50: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-0002af60: 536b 6574 6368 2873 656c 6629 3a0a 0a20  Sketch(self):.. 
-0002af70: 2020 2020 2020 2072 3120 3d20 280a 2020         r1 = (.  
-0002af80: 2020 2020 2020 2020 2020 576f 726b 706c            Workpl
-0002af90: 616e 6528 290a 2020 2020 2020 2020 2020  ane().          
-0002afa0: 2020 2e62 6f78 2831 302c 2031 302c 2031    .box(10, 10, 1
-0002afb0: 290a 2020 2020 2020 2020 2020 2020 2e66  ).            .f
-0002afc0: 6163 6573 2822 3e5a 2229 0a20 2020 2020  aces(">Z").     
-0002afd0: 2020 2020 2020 202e 736b 6574 6368 2829         .sketch()
-0002afe0: 0a20 2020 2020 2020 2020 2020 202e 736c  .            .sl
-0002aff0: 6f74 2832 2c20 3129 0a20 2020 2020 2020  ot(2, 1).       
-0002b000: 2020 2020 202e 736c 6f74 2832 2c20 312c       .slot(2, 1,
-0002b010: 2061 6e67 6c65 3d39 3029 0a20 2020 2020   angle=90).     
-0002b020: 2020 2020 2020 202e 636c 6561 6e28 290a         .clean().
-0002b030: 2020 2020 2020 2020 2020 2020 2e66 696e              .fin
-0002b040: 616c 697a 6528 290a 2020 2020 2020 2020  alize().        
-0002b050: 2020 2020 2e65 7874 7275 6465 2831 290a      .extrude(1).
-0002b060: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0002b070: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-0002b080: 7565 2872 312e 7661 6c28 292e 6973 5661  ue(r1.val().isVa
-0002b090: 6c69 6428 2929 0a20 2020 2020 2020 2073  lid()).        s
-0002b0a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0002b0b0: 6c65 6e28 7231 2e66 6163 6573 2829 2e76  len(r1.faces().v
-0002b0c0: 616c 7328 2929 2c20 3139 290a 0a20 2020  als()), 19)..   
-0002b0d0: 2020 2020 2072 3220 3d20 280a 2020 2020       r2 = (.    
-0002b0e0: 2020 2020 2020 2020 576f 726b 706c 616e          Workplan
-0002b0f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0002b100: 2e73 6b65 7463 6828 290a 2020 2020 2020  .sketch().      
-0002b110: 2020 2020 2020 2e63 6972 636c 6528 3229        .circle(2)
-0002b120: 0a20 2020 2020 2020 2020 2020 202e 7769  .            .wi
-0002b130: 7265 7328 290a 2020 2020 2020 2020 2020  res().          
-0002b140: 2020 2e6f 6666 7365 7428 302e 312c 206d    .offset(0.1, m
-0002b150: 6f64 653d 2273 2229 0a20 2020 2020 2020  ode="s").       
-0002b160: 2020 2020 202e 6669 6e61 6c69 7a65 2829       .finalize()
-0002b170: 0a20 2020 2020 2020 2020 2020 202e 736b  .            .sk
-0002b180: 6574 6368 2829 0a20 2020 2020 2020 2020  etch().         
-0002b190: 2020 202e 7265 6374 2831 2c20 3129 0a20     .rect(1, 1). 
-0002b1a0: 2020 2020 2020 2020 2020 202e 6669 6e61             .fina
-0002b1b0: 6c69 7a65 2829 0a20 2020 2020 2020 2020  lize().         
-0002b1c0: 2020 202e 6578 7472 7564 6528 312c 2074     .extrude(1, t
-0002b1d0: 6170 6572 3d35 290a 2020 2020 2020 2020  aper=5).        
-0002b1e0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0002b1f0: 6173 7365 7274 5472 7565 2872 322e 7661  assertTrue(r2.va
-0002b200: 6c28 292e 6973 5661 6c69 6428 2929 0a20  l().isValid()). 
-0002b210: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0002b220: 7274 4571 7561 6c28 6c65 6e28 7232 2e66  rtEqual(len(r2.f
-0002b230: 6163 6573 2829 2e76 616c 7328 2929 2c20  aces().vals()), 
-0002b240: 3629 0a0a 2020 2020 2020 2020 7233 203d  6)..        r3 =
-0002b250: 2028 0a20 2020 2020 2020 2020 2020 2057   (.            W
-0002b260: 6f72 6b70 6c61 6e65 2829 0a20 2020 2020  orkplane().     
-0002b270: 2020 2020 2020 202e 7075 7368 506f 696e         .pushPoin
-0002b280: 7473 2828 4c6f 6361 7469 6f6e 2856 6563  ts((Location(Vec
-0002b290: 746f 7228 312c 2031 2c20 3029 292c 2929  tor(1, 1, 0)),))
-0002b2a0: 0a20 2020 2020 2020 2020 2020 202e 736b  .            .sk
-0002b2b0: 6574 6368 2829 0a20 2020 2020 2020 2020  etch().         
-0002b2c0: 2020 202e 6369 7263 6c65 2832 290a 2020     .circle(2).  
-0002b2d0: 2020 2020 2020 2020 2020 2e77 6972 6573            .wires
-0002b2e0: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
-0002b2f0: 6f66 6673 6574 282d 302e 312c 206d 6f64  offset(-0.1, mod
-0002b300: 653d 2273 2229 0a20 2020 2020 2020 2020  e="s").         
-0002b310: 2020 202e 6669 6e61 6c69 7a65 2829 0a20     .finalize(). 
-0002b320: 2020 2020 2020 2020 2020 202e 6578 7472             .extr
-0002b330: 7564 6528 3129 0a20 2020 2020 2020 2029  ude(1).        )
-0002b340: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0002b350: 7373 6572 7454 7275 6528 7233 2e76 616c  ssertTrue(r3.val
-0002b360: 2829 2e69 7356 616c 6964 2829 290a 2020  ().isValid()).  
-0002b370: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002b380: 7445 7175 616c 286c 656e 2872 332e 6661  tEqual(len(r3.fa
-0002b390: 6365 7328 292e 7661 6c73 2829 292c 2034  ces().vals()), 4
-0002b3a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002b3b0: 7373 6572 7454 7570 6c65 416c 6d6f 7374  ssertTupleAlmost
-0002b3c0: 4571 7561 6c73 2872 332e 7661 6c28 292e  Equals(r3.val().
-0002b3d0: 4365 6e74 6572 2829 2e74 6f54 7570 6c65  Center().toTuple
-0002b3e0: 2829 2c20 2831 2c20 312c 2030 2e35 292c  (), (1, 1, 0.5),
-0002b3f0: 2036 290a 0a20 2020 2020 2020 2073 203d   6)..        s =
-0002b400: 2053 6b65 7463 6828 292e 7472 6170 657a   Sketch().trapez
-0002b410: 6f69 6428 332c 2031 2c20 3132 3029 0a0a  oid(3, 1, 120)..
-0002b420: 2020 2020 2020 2020 7234 203d 2057 6f72          r4 = Wor
-0002b430: 6b70 6c61 6e65 2829 2e70 6c61 6365 536b  kplane().placeSk
-0002b440: 6574 6368 2873 2c20 732e 6d6f 7665 6428  etch(s, s.moved(
-0002b450: 4c6f 6361 7469 6f6e 2856 6563 746f 7228  Location(Vector(
-0002b460: 302c 2030 2c20 3329 2929 292e 6c6f 6674  0, 0, 3)))).loft
-0002b470: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
-0002b480: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-0002b490: 2872 342e 736f 6c69 6473 2829 2e76 616c  (r4.solids().val
-0002b4a0: 7328 2929 2c20 3129 0a0a 2020 2020 6465  s()), 1)..    de
-0002b4b0: 6620 7465 7374 4369 7263 756d 7363 7269  f testCircumscri
-0002b4c0: 6265 6450 6f6c 7967 6f6e 2873 656c 6629  bedPolygon(self)
-0002b4d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0002b4e0: 2020 2020 2020 5465 7374 2074 6861 7420        Test that 
-0002b4f0: 6369 7263 756d 7363 7269 6265 6420 706f  circumscribed po
-0002b500: 6c79 676f 6e73 2072 6573 756c 7420 696e  lygons result in
-0002b510: 2074 6865 2063 6f72 7265 6374 2073 6861   the correct sha
-0002b520: 7065 730a 2020 2020 2020 2020 2222 220a  pes.        """.
-0002b530: 0a20 2020 2020 2020 2064 6566 2063 6972  .        def cir
-0002b540: 6375 6d72 6164 6975 7328 6e2c 2061 293a  cumradius(n, a):
-0002b550: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002b560: 7572 6e20 6120 2f20 6d61 7468 2e63 6f73  urn a / math.cos
-0002b570: 286d 6174 682e 7069 202f 206e 290a 0a20  (math.pi / n).. 
-0002b580: 2020 2020 2020 2061 203d 2031 0a20 2020         a = 1.   
-0002b590: 2020 2020 2023 2054 6573 7420 7472 6961       # Test tria
-0002b5a0: 6e67 6c65 0a20 2020 2020 2020 2076 7320  ngle.        vs 
-0002b5b0: 3d20 576f 726b 706c 616e 6528 2258 5922  = Workplane("XY"
-0002b5c0: 292e 706f 6c79 676f 6e28 332c 2032 202a  ).polygon(3, 2 *
-0002b5d0: 2061 2c20 6369 7263 756d 7363 7269 6265   a, circumscribe
-0002b5e0: 643d 5472 7565 292e 7665 7274 6963 6573  d=True).vertices
-0002b5f0: 2829 2e76 616c 7328 290a 2020 2020 2020  ().vals().      
-0002b600: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002b610: 616c 2833 2c20 6c65 6e28 7673 2929 0a20  al(3, len(vs)). 
-0002b620: 2020 2020 2020 2052 203d 2063 6972 6375         R = circu
-0002b630: 6d72 6164 6975 7328 332c 2061 290a 2020  mradius(3, a).  
-0002b640: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002b650: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
-0002b660: 2020 2020 7673 5b30 5d2e 746f 5475 706c      vs[0].toTupl
-0002b670: 6528 292c 2061 7070 726f 7828 2861 2c20  e(), approx((a, 
-0002b680: 6120 2a20 6d61 7468 2e74 616e 286d 6174  a * math.tan(mat
-0002b690: 682e 7261 6469 616e 7328 3630 2929 2c20  h.radians(60)), 
-0002b6a0: 3029 290a 2020 2020 2020 2020 290a 2020  0)).        ).  
-0002b6b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002b6c0: 7445 7175 616c 2876 735b 315d 2e74 6f54  tEqual(vs[1].toT
-0002b6d0: 7570 6c65 2829 2c20 6170 7072 6f78 2828  uple(), approx((
-0002b6e0: 2d52 2c20 302c 2030 2929 290a 2020 2020  -R, 0, 0))).    
-0002b6f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0002b700: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-0002b710: 2020 7673 5b32 5d2e 746f 5475 706c 6528    vs[2].toTuple(
-0002b720: 292c 2061 7070 726f 7828 2861 2c20 2d61  ), approx((a, -a
-0002b730: 202a 206d 6174 682e 7461 6e28 6d61 7468   * math.tan(math
-0002b740: 2e72 6164 6961 6e73 2836 3029 292c 2030  .radians(60)), 0
-0002b750: 2929 0a20 2020 2020 2020 2029 0a0a 2020  )).        )..  
-0002b760: 2020 2020 2020 2320 5465 7374 2073 7175        # Test squ
-0002b770: 6172 650a 2020 2020 2020 2020 7673 203d  are.        vs =
-0002b780: 2057 6f72 6b70 6c61 6e65 2822 5859 2229   Workplane("XY")
-0002b790: 2e70 6f6c 7967 6f6e 2834 2c20 3220 2a20  .polygon(4, 2 * 
-0002b7a0: 612c 2063 6972 6375 6d73 6372 6962 6564  a, circumscribed
-0002b7b0: 3d54 7275 6529 2e76 6572 7469 6365 7328  =True).vertices(
-0002b7c0: 292e 7661 6c73 2829 0a20 2020 2020 2020  ).vals().       
-0002b7d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0002b7e0: 6c28 342c 206c 656e 2876 7329 290a 2020  l(4, len(vs)).  
-0002b7f0: 2020 2020 2020 5220 3d20 6369 7263 756d        R = circum
-0002b800: 7261 6469 7573 2834 2c20 6129 0a20 2020  radius(4, a).   
-0002b810: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002b820: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
-0002b830: 2020 2076 735b 305d 2e74 6f54 7570 6c65     vs[0].toTuple
-0002b840: 2829 2c20 6170 7072 6f78 2828 612c 2061  (), approx((a, a
-0002b850: 202a 206d 6174 682e 7461 6e28 6d61 7468   * math.tan(math
-0002b860: 2e72 6164 6961 6e73 2834 3529 292c 2030  .radians(45)), 0
-0002b870: 2929 0a20 2020 2020 2020 2029 0a20 2020  )).        ).   
-0002b880: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002b890: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
-0002b8a0: 2020 2076 735b 315d 2e74 6f54 7570 6c65     vs[1].toTuple
-0002b8b0: 2829 2c20 6170 7072 6f78 2828 2d61 2c20  (), approx((-a, 
-0002b8c0: 6120 2a20 6d61 7468 2e74 616e 286d 6174  a * math.tan(mat
-0002b8d0: 682e 7261 6469 616e 7328 3435 2929 2c20  h.radians(45)), 
-0002b8e0: 3029 290a 2020 2020 2020 2020 290a 2020  0)).        ).  
-0002b8f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002b900: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
-0002b910: 2020 2020 7673 5b32 5d2e 746f 5475 706c      vs[2].toTupl
-0002b920: 6528 292c 2061 7070 726f 7828 282d 612c  e(), approx((-a,
-0002b930: 202d 6120 2a20 6d61 7468 2e74 616e 286d   -a * math.tan(m
-0002b940: 6174 682e 7261 6469 616e 7328 3435 2929  ath.radians(45))
-0002b950: 2c20 3029 290a 2020 2020 2020 2020 290a  , 0)).        ).
-0002b960: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002b970: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-0002b980: 2020 2020 2020 7673 5b33 5d2e 746f 5475        vs[3].toTu
-0002b990: 706c 6528 292c 2061 7070 726f 7828 2861  ple(), approx((a
-0002b9a0: 2c20 2d61 202a 206d 6174 682e 7461 6e28  , -a * math.tan(
-0002b9b0: 6d61 7468 2e72 6164 6961 6e73 2834 3529  math.radians(45)
-0002b9c0: 292c 2030 2929 0a20 2020 2020 2020 2029  ), 0)).        )
-0002b9d0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
-0002b9e0: 6f6d 6269 6e65 5769 7468 4261 7365 2873  ombineWithBase(s
-0002b9f0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-0002ba00: 5465 7374 2074 6865 2068 656c 7065 7220  Test the helper 
-0002ba10: 6d65 686f 6420 5f63 6f6d 6269 6e65 7769  mehod _combinewi
-0002ba20: 7468 0a0a 2020 2020 2020 2020 626f 7820  th..        box 
-0002ba30: 3d20 576f 726b 706c 616e 6528 292e 626f  = Workplane().bo
-0002ba40: 7828 3130 2c20 3130 2c20 3130 290a 2020  x(10, 10, 10).  
-0002ba50: 2020 2020 2020 7370 6865 7265 203d 2062        sphere = b
-0002ba60: 6f78 2e66 6163 6573 2822 3e5a 2229 2e73  ox.faces(">Z").s
-0002ba70: 7068 6572 6528 3229 0a20 2020 2020 2020  phere(2).       
-0002ba80: 206e 6577 5f62 6f78 203d 2062 6f78 2e5f   new_box = box._
-0002ba90: 636f 6d62 696e 6557 6974 6842 6173 6528  combineWithBase(
-0002baa0: 7370 6865 7265 2e76 616c 2829 290a 0a20  sphere.val()).. 
-0002bab0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0002bac0: 7274 4772 6561 7465 7228 6e65 775f 626f  rtGreater(new_bo
-0002bad0: 782e 7661 6c28 292e 566f 6c75 6d65 2829  x.val().Volume()
-0002bae0: 2c20 626f 782e 7661 6c28 292e 566f 6c75  , box.val().Volu
-0002baf0: 6d65 2829 290a 0a20 2020 2064 6566 2074  me())..    def t
-0002bb00: 6573 745f 6375 7446 726f 6d42 6173 6528  est_cutFromBase(
-0002bb10: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-0002bb20: 2054 6573 7420 7468 6520 6865 6c70 6572   Test the helper
-0002bb30: 206d 6574 686f 6420 5f63 7574 4672 6f6d   method _cutFrom
-0002bb40: 4261 7365 0a0a 2020 2020 2020 2020 626f  Base..        bo
-0002bb50: 7820 3d20 576f 726b 706c 616e 6528 292e  x = Workplane().
-0002bb60: 626f 7828 3130 2c20 3130 2c20 3130 290a  box(10, 10, 10).
-0002bb70: 2020 2020 2020 2020 7370 6865 7265 203d          sphere =
-0002bb80: 2057 6f72 6b70 6c61 6e65 2829 2e73 7068   Workplane().sph
-0002bb90: 6572 6528 3229 0a20 2020 2020 2020 2068  ere(2).        h
-0002bba0: 6f6f 6c6f 775f 626f 7820 3d20 626f 782e  oolow_box = box.
-0002bbb0: 5f63 7574 4672 6f6d 4261 7365 2873 7068  _cutFromBase(sph
-0002bbc0: 6572 652e 7661 6c28 2929 0a0a 2020 2020  ere.val())..    
-0002bbd0: 2020 2020 7365 6c66 2e61 7373 6572 7447      self.assertG
-0002bbe0: 7265 6174 6572 2862 6f78 2e76 616c 2829  reater(box.val()
-0002bbf0: 2e56 6f6c 756d 6528 292c 2068 6f6f 6c6f  .Volume(), hoolo
-0002bc00: 775f 626f 782e 7661 6c28 292e 566f 6c75  w_box.val().Volu
-0002bc10: 6d65 2829 290a 0a20 2020 2064 6566 2074  me())..    def t
-0002bc20: 6573 745f 4d65 7267 6554 6167 7328 7365  est_MergeTags(se
-0002bc30: 6c66 293a 0a0a 2020 2020 2020 2020 6120  lf):..        a 
-0002bc40: 3d20 576f 726b 706c 616e 6528 292e 626f  = Workplane().bo
-0002bc50: 7828 312c 2031 2c20 3129 0a20 2020 2020  x(1, 1, 1).     
-0002bc60: 2020 2062 203d 2028 0a20 2020 2020 2020     b = (.       
-0002bc70: 2020 2020 2057 6f72 6b70 6c61 6e65 286f       Workplane(o
-0002bc80: 7269 6769 6e3d 2831 2c20 302c 2030 2929  rigin=(1, 0, 0))
-0002bc90: 0a20 2020 2020 2020 2020 2020 202e 626f  .            .bo
-0002bca0: 7828 312c 2031 2c20 3129 0a20 2020 2020  x(1, 1, 1).     
-0002bcb0: 2020 2020 2020 202e 7665 7274 6963 6573         .vertices
-0002bcc0: 2822 3e58 2061 6e64 203e 5920 616e 6420  (">X and >Y and 
-0002bcd0: 3e5a 2229 0a20 2020 2020 2020 2020 2020  >Z").           
-0002bce0: 202e 7461 6728 2262 6f78 5f76 6572 7465   .tag("box_verte
-0002bcf0: 7822 290a 2020 2020 2020 2020 2020 2020  x").            
-0002bd00: 2e65 6e64 2832 290a 2020 2020 2020 2020  .end(2).        
-0002bd10: 290a 2020 2020 2020 2020 6120 3d20 612e  ).        a = a.
-0002bd20: 6164 6428 6229 0a20 2020 2020 2020 2061  add(b).        a
-0002bd30: 7373 6572 7420 612e 7665 7274 6963 6573  ssert a.vertices
-0002bd40: 2874 6167 3d22 626f 785f 7665 7274 6578  (tag="box_vertex
-0002bd50: 2229 2e76 616c 2829 2e43 656e 7465 7228  ").val().Center(
-0002bd60: 292e 746f 5475 706c 6528 2920 3d3d 2061  ).toTuple() == a
-0002bd70: 7070 726f 7828 0a20 2020 2020 2020 2020  pprox(.         
-0002bd80: 2020 2028 312e 352c 2030 2e35 2c20 302e     (1.5, 0.5, 0.
-0002bd90: 3529 0a20 2020 2020 2020 2029 0a0a 2020  5).        )..  
-0002bda0: 2020 2020 2020 6120 3d20 576f 726b 706c        a = Workpl
-0002bdb0: 616e 6528 292e 626f 7828 342c 2034 2c20  ane().box(4, 4, 
-0002bdc0: 3429 0a20 2020 2020 2020 2062 203d 2057  4).        b = W
-0002bdd0: 6f72 6b70 6c61 6e65 286f 7269 6769 6e3d  orkplane(origin=
-0002bde0: 2830 2c20 302c 2031 2929 2e62 6f78 2832  (0, 0, 1)).box(2
-0002bdf0: 2c20 322c 2032 292e 6661 6365 7328 223c  , 2, 2).faces("<
-0002be00: 5a22 292e 7461 6728 2262 6f78 325f 6661  Z").tag("box2_fa
-0002be10: 6365 2229 2e65 6e64 2829 0a20 2020 2020  ce").end().     
-0002be20: 2020 2061 203d 2061 2e63 7574 2862 290a     a = a.cut(b).
-0002be30: 2020 2020 2020 2020 6173 7365 7274 2061          assert a
-0002be40: 2e76 616c 2829 2e56 6f6c 756d 6528 2920  .val().Volume() 
-0002be50: 3d3d 2061 7070 726f 7828 3420 2a2a 2033  == approx(4 ** 3
-0002be60: 202d 2032 202a 2a20 3329 0a20 2020 2020   - 2 ** 3).     
-0002be70: 2020 2061 203d 2061 2e66 6163 6573 2874     a = a.faces(t
-0002be80: 6167 3d22 626f 7832 5f66 6163 6522 292e  ag="box2_face").
-0002be90: 7769 7265 7328 292e 746f 5065 6e64 696e  wires().toPendin
-0002bea0: 6728 292e 6578 7472 7564 6528 3429 0a20  g().extrude(4). 
-0002beb0: 2020 2020 2020 2061 7373 6572 7420 612e         assert a.
-0002bec0: 7661 6c28 292e 566f 6c75 6d65 2829 203d  val().Volume() =
-0002bed0: 3d20 6170 7072 6f78 2834 202a 2a20 3320  = approx(4 ** 3 
-0002bee0: 2b20 3220 2a2a 2033 290a 0a20 2020 2020  + 2 ** 3)..     
-0002bef0: 2020 2061 203d 2057 6f72 6b70 6c61 6e65     a = Workplane
-0002bf00: 2829 2e73 7068 6572 6528 3229 0a20 2020  ().sphere(2).   
-0002bf10: 2020 2020 2062 203d 2057 6f72 6b70 6c61       b = Workpla
-0002bf20: 6e65 2829 2e63 796c 696e 6465 7228 342c  ne().cylinder(4,
-0002bf30: 2031 292e 7461 6728 2263 796c 2229 0a20   1).tag("cyl"). 
-0002bf40: 2020 2020 2020 2061 203d 2061 2e69 6e74         a = a.int
-0002bf50: 6572 7365 6374 2862 290a 2020 2020 2020  ersect(b).      
-0002bf60: 2020 6173 7365 7274 206c 656e 2861 2e73    assert len(a.s
-0002bf70: 6f6c 6964 7328 7461 673d 2263 796c 2229  olids(tag="cyl")
-0002bf80: 2e76 616c 2829 2e53 6f6c 6964 7328 2929  .val().Solids())
-0002bf90: 203d 3d20 310a 0a20 2020 2020 2020 2061   == 1..        a
-0002bfa0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e62   = Workplane().b
-0002bfb0: 6f78 2834 2c20 342c 2034 290a 2020 2020  ox(4, 4, 4).    
-0002bfc0: 2020 2020 6220 3d20 280a 2020 2020 2020      b = (.      
-0002bfd0: 2020 2020 2020 576f 726b 706c 616e 6528        Workplane(
-0002bfe0: 290a 2020 2020 2020 2020 2020 2020 2e62  ).            .b
-0002bff0: 6f78 2832 2c20 352c 2035 2c20 6365 6e74  ox(2, 5, 5, cent
-0002c000: 6572 6564 3d28 4661 6c73 652c 2054 7275  ered=(False, Tru
-0002c010: 652c 2054 7275 6529 290a 2020 2020 2020  e, True)).      
-0002c020: 2020 2020 2020 2e66 6163 6573 2822 3e58        .faces(">X
-0002c030: 2229 0a20 2020 2020 2020 2020 2020 202e  ").            .
-0002c040: 776f 726b 706c 616e 6528 290a 2020 2020  workplane().    
-0002c050: 2020 2020 2020 2020 2e74 6167 2822 7370          .tag("sp
-0002c060: 6c69 7474 6572 2229 0a20 2020 2020 2020  litter").       
-0002c070: 2020 2020 202e 656e 6428 3229 0a20 2020       .end(2).   
-0002c080: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
-0002c090: 203d 2061 2e73 706c 6974 2862 290a 2020   = a.split(b).  
-0002c0a0: 2020 2020 2020 6120 3d20 612e 736f 6c69        a = a.soli
-0002c0b0: 6473 2822 3c58 2229 0a20 2020 2020 2020  ds("<X").       
-0002c0c0: 2061 7373 6572 7420 612e 7661 6c28 292e   assert a.val().
-0002c0d0: 566f 6c75 6d65 2829 203d 3d20 6170 7072  Volume() == appr
-0002c0e0: 6f78 2828 3420 2a2a 2033 2920 2f20 322e  ox((4 ** 3) / 2.
-0002c0f0: 3029 0a20 2020 2020 2020 2061 203d 2061  0).        a = a
-0002c100: 2e77 6f72 6b70 6c61 6e65 4672 6f6d 5461  .workplaneFromTa
-0002c110: 6767 6564 2822 7370 6c69 7474 6572 2229  gged("splitter")
-0002c120: 2e72 6563 7428 342c 2034 292e 6578 7472  .rect(4, 4).extr
-0002c130: 7564 6528 756e 7469 6c3d 226e 6578 7422  ude(until="next"
-0002c140: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0002c150: 2061 2e76 616c 2829 2e56 6f6c 756d 6528   a.val().Volume(
-0002c160: 2920 3d3d 2061 7070 726f 7828 2834 202a  ) == approx((4 *
-0002c170: 2a20 3329 290a 0a20 2020 2020 2020 2061  * 3))..        a
-0002c180: 203d 2057 6f72 6b70 6c61 6e65 2829 2e62   = Workplane().b
-0002c190: 6f78 2834 2c20 342c 2034 290a 2020 2020  ox(4, 4, 4).    
-0002c1a0: 2020 2020 6220 3d20 576f 726b 706c 616e      b = Workplan
-0002c1b0: 6528 6f72 6967 696e 3d28 302c 2030 2c20  e(origin=(0, 0, 
-0002c1c0: 3329 292e 626f 7828 322c 2032 2c20 3229  3)).box(2, 2, 2)
-0002c1d0: 2e66 6163 6573 2822 3e5a 2229 2e74 6167  .faces(">Z").tag
-0002c1e0: 2822 626f 7832 5f66 6163 6522 292e 656e  ("box2_face").en
-0002c1f0: 6428 290a 2020 2020 2020 2020 6120 3d20  d().        a = 
-0002c200: 612e 756e 696f 6e28 6229 0a20 2020 2020  a.union(b).     
-0002c210: 2020 2061 203d 2061 2e66 6163 6573 2874     a = a.faces(t
-0002c220: 6167 3d22 626f 7832 5f66 6163 6522 292e  ag="box2_face").
-0002c230: 776f 726b 706c 616e 6528 6f66 6673 6574  workplane(offset
-0002c240: 3d30 2e35 292e 626f 7828 312c 2031 2c20  =0.5).box(1, 1, 
-0002c250: 3129 0a20 2020 2020 2020 2061 7373 6572  1).        asser
-0002c260: 7420 612e 7661 6c28 292e 566f 6c75 6d65  t a.val().Volume
-0002c270: 2829 203d 3d20 6170 7072 6f78 2834 202a  () == approx(4 *
-0002c280: 2a20 3320 2b20 3220 2a2a 2033 202b 2031  * 3 + 2 ** 3 + 1
-0002c290: 290a 0a20 2020 2020 2020 2023 2074 6167  )..        # tag
-0002c2a0: 206e 616d 6520 636f 6e66 6c69 6374 3b20   name conflict; 
-0002c2b0: 6b65 6570 2074 6167 2066 726f 6d20 6c65  keep tag from le
-0002c2c0: 6674 2073 6964 6520 6f66 2062 6f6f 6c65  ft side of boole
-0002c2d0: 616e 0a20 2020 2020 2020 2061 203d 2057  an.        a = W
-0002c2e0: 6f72 6b70 6c61 6e65 2829 2e62 6f78 2831  orkplane().box(1
-0002c2f0: 2c20 312c 2031 292e 6661 6365 7328 223e  , 1, 1).faces(">
-0002c300: 5a22 292e 776f 726b 706c 616e 6528 292e  Z").workplane().
-0002c310: 7461 6728 227a 6661 6365 2229 2e65 6e64  tag("zface").end
-0002c320: 2832 290a 2020 2020 2020 2020 6220 3d20  (2).        b = 
-0002c330: 280a 2020 2020 2020 2020 2020 2020 576f  (.            Wo
-0002c340: 726b 706c 616e 6528 6f72 6967 696e 3d28  rkplane(origin=(
-0002c350: 312c 2030 2c20 3029 290a 2020 2020 2020  1, 0, 0)).      
-0002c360: 2020 2020 2020 2e62 6f78 2831 2c20 312c        .box(1, 1,
-0002c370: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-0002c380: 2e66 6163 6573 2822 3e5a 2229 0a20 2020  .faces(">Z").   
-0002c390: 2020 2020 2020 2020 202e 776f 726b 706c           .workpl
-0002c3a0: 616e 6528 290a 2020 2020 2020 2020 2020  ane().          
-0002c3b0: 2020 2e74 6167 2822 7a66 6163 6522 290a    .tag("zface").
-0002c3c0: 2020 2020 2020 2020 2020 2020 2e65 6e64              .end
-0002c3d0: 2832 290a 2020 2020 2020 2020 290a 2020  (2).        ).  
-0002c3e0: 2020 2020 2020 6120 3d20 612e 756e 696f        a = a.unio
-0002c3f0: 6e28 6229 0a20 2020 2020 2020 2061 203d  n(b).        a =
-0002c400: 2061 2e77 6f72 6b70 6c61 6e65 4672 6f6d   a.workplaneFrom
-0002c410: 5461 6767 6564 2822 7a66 6163 6522 292e  Tagged("zface").
-0002c420: 6369 7263 6c65 2830 2e32 290a 2020 2020  circle(0.2).    
-0002c430: 2020 2020 6173 7365 7274 2061 2e65 6467      assert a.edg
-0002c440: 6573 2822 2543 4952 434c 4522 292e 7661  es("%CIRCLE").va
-0002c450: 6c28 292e 4365 6e74 6572 2829 2e74 6f54  l().Center().toT
-0002c460: 7570 6c65 2829 203d 3d20 6170 7072 6f78  uple() == approx
-0002c470: 2828 302c 2030 2c20 302e 3529 290a 0a20  ((0, 0, 0.5)).. 
-0002c480: 2020 2064 6566 2074 6573 745f 706c 616e     def test_plan
-0002c490: 655f 7265 7072 2873 656c 6629 3a0a 2020  e_repr(self):.  
-0002c4a0: 2020 2020 2020 7770 203d 2057 6f72 6b70        wp = Workp
-0002c4b0: 6c61 6e65 2822 5859 2229 0a20 2020 2020  lane("XY").     
-0002c4c0: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-0002c4d0: 2020 2020 2020 2020 7265 7072 2877 702e          repr(wp.
-0002c4e0: 706c 616e 6529 0a20 2020 2020 2020 2020  plane).         
-0002c4f0: 2020 203d 3d20 2250 6c61 6e65 286f 7269     == "Plane(ori
-0002c500: 6769 6e3d 2830 2e30 2c20 302e 302c 2030  gin=(0.0, 0.0, 0
-0002c510: 2e30 292c 2078 4469 723d 2831 2e30 2c20  .0), xDir=(1.0, 
-0002c520: 302e 302c 2030 2e30 292c 206e 6f72 6d61  0.0, 0.0), norma
-0002c530: 6c3d 2830 2e30 2c20 302e 302c 2031 2e30  l=(0.0, 0.0, 1.0
-0002c540: 2929 220a 2020 2020 2020 2020 290a 0a20  ))".        ).. 
-0002c550: 2020 2064 6566 2074 6573 745f 6469 7374     def test_dist
-0002c560: 616e 6365 2873 656c 6629 3a0a 0a20 2020  ance(self):..   
-0002c570: 2020 2020 2077 3120 3d20 4661 6365 2e6d       w1 = Face.m
-0002c580: 616b 6550 6c61 6e65 2832 2c20 3229 2e57  akePlane(2, 2).W
-0002c590: 6972 6573 2829 5b30 5d0a 2020 2020 2020  ires()[0].      
-0002c5a0: 2020 7732 203d 2046 6163 652e 6d61 6b65    w2 = Face.make
-0002c5b0: 506c 616e 6528 312c 2031 292e 5769 7265  Plane(1, 1).Wire
-0002c5c0: 7328 295b 305d 0a20 2020 2020 2020 2077  s()[0].        w
-0002c5d0: 3320 3d20 4661 6365 2e6d 616b 6550 6c61  3 = Face.makePla
-0002c5e0: 6e65 2833 2c20 3329 2e57 6972 6573 2829  ne(3, 3).Wires()
-0002c5f0: 5b30 5d0a 0a20 2020 2020 2020 2064 3132  [0]..        d12
-0002c600: 203d 2077 312e 6469 7374 616e 6365 2877   = w1.distance(w
-0002c610: 3229 0a0a 2020 2020 2020 2020 6173 7365  2)..        asse
-0002c620: 7274 2064 3132 203d 3d20 6170 7072 6f78  rt d12 == approx
-0002c630: 2830 2e35 290a 0a20 2020 2020 2020 2064  (0.5)..        d
-0002c640: 3132 2c20 6431 3320 3d20 7731 2e64 6973  12, d13 = w1.dis
-0002c650: 7461 6e63 6573 2877 322c 2077 3329 0a0a  tances(w2, w3)..
-0002c660: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-0002c670: 3132 203d 3d20 6170 7072 6f78 2830 2e35  12 == approx(0.5
-0002c680: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0002c690: 2064 3133 203d 3d20 6170 7072 6f78 2830   d13 == approx(0
-0002c6a0: 2e35 290a 0a20 2020 2064 6566 2074 6573  .5)..    def tes
-0002c6b0: 745f 7072 6f6a 6563 7428 7365 6c66 293a  t_project(self):
-0002c6c0: 0a0a 2020 2020 2020 2020 2320 7072 6f6a  ..        # proj
-0002c6d0: 6563 7420 6120 7369 6e67 6c65 206c 6574  ect a single let
-0002c6e0: 7465 720a 2020 2020 2020 2020 7420 3d20  ter.        t = 
-0002c6f0: 436f 6d70 6f75 6e64 2e6d 616b 6554 6578  Compound.makeTex
-0002c700: 7428 2254 222c 2035 2c20 3029 2e46 6163  t("T", 5, 0).Fac
-0002c710: 6573 2829 5b30 5d0a 2020 2020 2020 2020  es()[0].        
-0002c720: 6620 3d20 576f 726b 706c 616e 6528 2258  f = Workplane("X
-0002c730: 5a22 2c20 6f72 6967 696e 3d28 302c 2030  Z", origin=(0, 0
-0002c740: 2c20 2d37 2929 2e73 7068 6572 6528 3629  , -7)).sphere(6)
-0002c750: 2e66 6163 6573 2822 6e6f 7420 2550 4c41  .faces("not %PLA
-0002c760: 4e45 2229 2e76 616c 2829 0a0a 2020 2020  NE").val()..    
-0002c770: 2020 2020 7265 7320 3d20 742e 7072 6f6a      res = t.proj
-0002c780: 6563 7428 662c 2028 302c 2030 2c20 2d31  ect(f, (0, 0, -1
-0002c790: 2929 0a0a 2020 2020 2020 2020 6173 7365  ))..        asse
-0002c7a0: 7274 2072 6573 2e69 7356 616c 6964 2829  rt res.isValid()
-0002c7b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0002c7c0: 6c65 6e28 7265 732e 4564 6765 7328 2929  len(res.Edges())
-0002c7d0: 203d 3d20 380a 2020 2020 2020 2020 6173   == 8.        as
-0002c7e0: 7365 7274 2074 2e64 6973 7461 6e63 6528  sert t.distance(
-0002c7f0: 7265 7329 203d 3d20 6170 7072 6f78 2831  res) == approx(1
-0002c800: 290a 0a20 2020 2020 2020 2023 2065 7874  )..        # ext
-0002c810: 7275 6465 2069 740a 2020 2020 2020 2020  rude it.        
-0002c820: 7265 735f 6578 203d 2053 6f6c 6964 2e65  res_ex = Solid.e
-0002c830: 7874 7275 6465 4c69 6e65 6172 2874 2e70  xtrudeLinear(t.p
-0002c840: 726f 6a65 6374 2866 2c20 2830 2c20 302c  roject(f, (0, 0,
-0002c850: 202d 3129 292c 2028 302e 302c 2030 2e30   -1)), (0.0, 0.0
-0002c860: 2c20 302e 3529 290a 0a20 2020 2020 2020  , 0.5))..       
-0002c870: 2061 7373 6572 7420 7265 735f 6578 2e69   assert res_ex.i
-0002c880: 7356 616c 6964 2829 0a20 2020 2020 2020  sValid().       
-0002c890: 2061 7373 6572 7420 6c65 6e28 7265 735f   assert len(res_
-0002c8a0: 6578 2e46 6163 6573 2829 2920 3d3d 2031  ex.Faces()) == 1
-0002c8b0: 300a 0a20 2020 2020 2020 2023 2070 726f  0..        # pro
-0002c8c0: 6a65 6374 2061 2077 6972 650a 2020 2020  ject a wire.    
-0002c8d0: 2020 2020 7720 3d20 742e 6f75 7465 7257      w = t.outerW
-0002c8e0: 6972 6528 290a 0a20 2020 2020 2020 2072  ire()..        r
-0002c8f0: 6573 5f77 203d 2077 2e70 726f 6a65 6374  es_w = w.project
-0002c900: 2866 2c20 2830 2c20 302c 202d 3129 290a  (f, (0, 0, -1)).
-0002c910: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0002c920: 6c65 6e28 7265 735f 772e 4564 6765 7328  len(res_w.Edges(
-0002c930: 2929 203d 3d20 380a 2020 2020 2020 2020  )) == 8.        
-0002c940: 6173 7365 7274 2072 6573 5f77 2e69 7356  assert res_w.isV
-0002c950: 616c 6964 2829 0a0a 2020 2020 2020 2020  alid()..        
-0002c960: 7265 735f 7731 2c20 7265 735f 7732 203d  res_w1, res_w2 =
-0002c970: 2077 2e70 726f 6a65 6374 2866 2c20 2830   w.project(f, (0
-0002c980: 2c20 302c 202d 3129 2c20 4661 6c73 6529  , 0, -1), False)
-0002c990: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-0002c9a0: 206c 656e 2872 6573 5f77 312e 4564 6765   len(res_w1.Edge
-0002c9b0: 7328 2929 203d 3d20 380a 2020 2020 2020  s()) == 8.      
-0002c9c0: 2020 6173 7365 7274 206c 656e 2872 6573    assert len(res
-0002c9d0: 5f77 322e 4564 6765 7328 2929 203d 3d20  _w2.Edges()) == 
-0002c9e0: 380a 0a20 2020 2020 2020 2023 2070 726f  8..        # pro
-0002c9f0: 6a65 6374 2061 2073 696e 676c 6520 6c65  ject a single le
-0002ca00: 7474 6572 2077 6974 6820 6f70 656e 696e  tter with openin
-0002ca10: 6773 0a20 2020 2020 2020 206f 203d 2043  gs.        o = C
-0002ca20: 6f6d 706f 756e 642e 6d61 6b65 5465 7874  ompound.makeText
-0002ca30: 2822 4f22 2c20 352c 2030 292e 4661 6365  ("O", 5, 0).Face
-0002ca40: 7328 295b 305d 0a20 2020 2020 2020 2066  s()[0].        f
-0002ca50: 203d 2057 6f72 6b70 6c61 6e65 2822 585a   = Workplane("XZ
-0002ca60: 222c 206f 7269 6769 6e3d 2830 2c20 302c  ", origin=(0, 0,
-0002ca70: 202d 3729 292e 7370 6865 7265 2836 292e   -7)).sphere(6).
-0002ca80: 6661 6365 7328 226e 6f74 2025 504c 414e  faces("not %PLAN
-0002ca90: 4522 292e 7661 6c28 290a 0a20 2020 2020  E").val()..     
-0002caa0: 2020 2072 6573 5f6f 203d 206f 2e70 726f     res_o = o.pro
-0002cab0: 6a65 6374 2866 2c20 2830 2c20 302c 202d  ject(f, (0, 0, -
-0002cac0: 3129 290a 0a20 2020 2020 2020 2061 7373  1))..        ass
-0002cad0: 6572 7420 7265 735f 6f2e 6973 5661 6c69  ert res_o.isVali
-0002cae0: 6428 290a 0a20 2020 2020 2020 2023 2065  d()..        # e
-0002caf0: 7874 7275 6465 2069 740a 2020 2020 2020  xtrude it.      
-0002cb00: 2020 7265 735f 6f5f 6578 203d 2053 6f6c    res_o_ex = Sol
-0002cb10: 6964 2e65 7874 7275 6465 4c69 6e65 6172  id.extrudeLinear
-0002cb20: 286f 2e70 726f 6a65 6374 2866 2c20 2830  (o.project(f, (0
-0002cb30: 2c20 302c 202d 3129 292c 2028 302e 302c  , 0, -1)), (0.0,
-0002cb40: 2030 2e30 2c20 302e 3529 290a 0a20 2020   0.0, 0.5))..   
-0002cb50: 2020 2020 2061 7373 6572 7420 7265 735f       assert res_
-0002cb60: 6f5f 6578 2e69 7356 616c 6964 2829 0a0a  o_ex.isValid()..
-0002cb70: 2020 2020 6465 6620 7465 7374 5f6d 616b      def test_mak
-0002cb80: 654e 5369 6465 6453 7572 6661 6365 2873  eNSidedSurface(s
-0002cb90: 656c 6629 3a0a 0a20 2020 2020 2020 2023  elf):..        #
-0002cba0: 2069 6e6e 6572 2065 6467 652f 7769 7265   inner edge/wire
-0002cbb0: 2063 6f6e 7374 7261 696e 740a 2020 2020   constraint.    
-0002cbc0: 2020 2020 6f75 7465 725f 7720 3d20 576f      outer_w = Wo
-0002cbd0: 726b 706c 616e 6528 292e 736c 6f74 3244  rkplane().slot2D
-0002cbe0: 2832 2c20 3129 2e77 6972 6573 2829 2e76  (2, 1).wires().v
-0002cbf0: 616c 7328 290a 0a20 2020 2020 2020 2069  als()..        i
-0002cc00: 6e6e 6572 5f65 3120 3d20 280a 2020 2020  nner_e1 = (.    
-0002cc10: 2020 2020 2020 2020 576f 726b 706c 616e          Workplan
-0002cc20: 6528 6f72 6967 696e 3d28 302c 2030 2c20  e(origin=(0, 0, 
-0002cc30: 3129 292e 6d6f 7665 546f 282d 302e 352c  1)).moveTo(-0.5,
-0002cc40: 2030 292e 6c69 6e65 546f 2830 2e35 2c20   0).lineTo(0.5, 
-0002cc50: 302e 3029 2e65 6467 6573 2829 2e76 616c  0.0).edges().val
-0002cc60: 7328 290a 2020 2020 2020 2020 290a 2020  s().        ).  
-0002cc70: 2020 2020 2020 696e 6e65 725f 6532 203d        inner_e2 =
-0002cc80: 2028 0a20 2020 2020 2020 2020 2020 2057   (.            W
-0002cc90: 6f72 6b70 6c61 6e65 286f 7269 6769 6e3d  orkplane(origin=
-0002cca0: 2830 2c20 302c 2031 2929 2e6d 6f76 6554  (0, 0, 1)).moveT
-0002ccb0: 6f28 302c 202d 302e 3229 2e6c 696e 6554  o(0, -0.2).lineT
-0002ccc0: 6f28 302c 2030 2e32 292e 6564 6765 7328  o(0, 0.2).edges(
-0002ccd0: 292e 7661 6c73 2829 0a20 2020 2020 2020  ).vals().       
-0002cce0: 2029 0a20 2020 2020 2020 2069 6e6e 6572   ).        inner
-0002ccf0: 5f77 203d 2057 6f72 6b70 6c61 6e65 286f  _w = Workplane(o
-0002cd00: 7269 6769 6e3d 2830 2c20 302c 2031 2929  rigin=(0, 0, 1))
-0002cd10: 2e65 6c6c 6970 7365 2830 2e35 2c20 302e  .ellipse(0.5, 0.
-0002cd20: 3229 2e76 616c 7328 290a 0a20 2020 2020  2).vals()..     
-0002cd30: 2020 2066 3120 3d20 4661 6365 2e6d 616b     f1 = Face.mak
-0002cd40: 654e 5369 6465 6453 7572 6661 6365 286f  eNSidedSurface(o
-0002cd50: 7574 6572 5f77 2c20 696e 6e65 725f 6531  uter_w, inner_e1
-0002cd60: 202b 2069 6e6e 6572 5f65 3220 2b20 696e   + inner_e2 + in
-0002cd70: 6e65 725f 7729 0a0a 2020 2020 2020 2020  ner_w)..        
-0002cd80: 6173 7365 7274 2066 312e 6973 5661 6c69  assert f1.isVali
-0002cd90: 6428 290a 2020 2020 2020 2020 6173 7365  d().        asse
-0002cda0: 7274 206c 656e 2866 312e 4564 6765 7328  rt len(f1.Edges(
-0002cdb0: 2929 203d 3d20 340a 0a20 2020 2020 2020  )) == 4..       
-0002cdc0: 2023 2069 6e6e 6572 2070 6f69 6e74 730a   # inner points.
-0002cdd0: 2020 2020 2020 2020 6632 203d 2046 6163          f2 = Fac
-0002cde0: 652e 6d61 6b65 4e53 6964 6564 5375 7266  e.makeNSidedSurf
-0002cdf0: 6163 6528 0a20 2020 2020 2020 2020 2020  ace(.           
-0002ce00: 206f 7574 6572 5f77 2c20 5b56 6563 746f   outer_w, [Vecto
-0002ce10: 7228 2d30 2e34 2c20 302c 2031 292e 746f  r(-0.4, 0, 1).to
-0002ce20: 506e 7428 292c 2056 6563 746f 7228 302e  Pnt(), Vector(0.
-0002ce30: 342c 2030 2c20 3129 5d0a 2020 2020 2020  4, 0, 1)].      
-0002ce40: 2020 290a 0a20 2020 2020 2020 2061 7373    )..        ass
-0002ce50: 6572 7420 6632 2e69 7356 616c 6964 2829  ert f2.isValid()
-0002ce60: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0002ce70: 6c65 6e28 6632 2e45 6467 6573 2829 2920  len(f2.Edges()) 
-0002ce80: 3d3d 2034 0a0a 2020 2020 2020 2020 2320  == 4..        # 
-0002ce90: 6578 6365 7074 696f 6e20 6f6e 2069 6e76  exception on inv
-0002cea0: 616c 6964 2063 6f6e 7374 7261 696e 740a  alid constraint.
-0002ceb0: 2020 2020 2020 2020 7769 7468 2072 6169          with rai
-0002cec0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
-0002ced0: 0a20 2020 2020 2020 2020 2020 2046 6163  .            Fac
-0002cee0: 652e 6d61 6b65 4e53 6964 6564 5375 7266  e.makeNSidedSurf
-0002cef0: 6163 6528 6f75 7465 725f 772c 205b 5b30  ace(outer_w, [[0
-0002cf00: 2c20 302c 2031 5d5d 290a 0a20 2020 2064  , 0, 1]])..    d
-0002cf10: 6566 2074 6573 745f 746f 5674 6b28 7365  ef test_toVtk(se
-0002cf20: 6c66 293a 0a0a 2020 2020 2020 2020 6672  lf):..        fr
-0002cf30: 6f6d 2076 746b 6d6f 6475 6c65 732e 7674  om vtkmodules.vt
-0002cf40: 6b43 6f6d 6d6f 6e44 6174 614d 6f64 656c  kCommonDataModel
-0002cf50: 2069 6d70 6f72 7420 7674 6b50 6f6c 7944   import vtkPolyD
-0002cf60: 6174 610a 0a20 2020 2020 2020 2066 203d  ata..        f =
-0002cf70: 2046 6163 652e 6d61 6b65 506c 616e 6528   Face.makePlane(
-0002cf80: 322c 2032 290a 2020 2020 2020 2020 7674  2, 2).        vt
-0002cf90: 6b20 3d20 662e 746f 5674 6b50 6f6c 7944  k = f.toVtkPolyD
-0002cfa0: 6174 6128 6e6f 726d 616c 733d 4661 6c73  ata(normals=Fals
-0002cfb0: 6529 0a0a 2020 2020 2020 2020 6173 7365  e)..        asse
-0002cfc0: 7274 2069 7369 6e73 7461 6e63 6528 7674  rt isinstance(vt
-0002cfd0: 6b2c 2076 746b 506f 6c79 4461 7461 290a  k, vtkPolyData).
-0002cfe0: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-0002cff0: 746b 2e47 6574 4e75 6d62 6572 4f66 506f  tk.GetNumberOfPo
-0002d000: 6c79 7328 2920 3d3d 2032 0a              lys() == 2.
+00028710: 7730 2e63 7574 426c 696e 6428 3129 0a0a  w0.cutBlind(1)..
+00028720: 2020 2020 6465 6620 7465 7374 4669 6e64      def testFind
+00028730: 4661 6365 2873 656c 6629 3a0a 2020 2020  Face(self):.    
+00028740: 2020 2020 2320 6966 2074 6865 7265 2061      # if there a
+00028750: 7265 206e 6f20 6661 6365 7320 746f 2066  re no faces to f
+00028760: 696e 642c 2073 686f 756c 6420 7261 6973  ind, should rais
+00028770: 6520 5661 6c75 6545 7272 6f72 0a20 2020  e ValueError.   
+00028780: 2020 2020 2077 3020 3d20 576f 726b 706c       w0 = Workpl
+00028790: 616e 6528 290a 2020 2020 2020 2020 7769  ane().        wi
+000287a0: 7468 2072 6169 7365 7328 5661 6c75 6545  th raises(ValueE
+000287b0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+000287c0: 2020 2077 302e 6669 6e64 4661 6365 2829     w0.findFace()
+000287d0: 0a0a 2020 2020 2020 2020 7731 203d 2057  ..        w1 = W
+000287e0: 6f72 6b70 6c61 6e65 2829 2e62 6f78 2831  orkplane().box(1
+000287f0: 2c20 312c 2031 292e 6661 6365 7328 223e  , 1, 1).faces(">
+00028800: 5a22 290a 2020 2020 2020 2020 7365 6c66  Z").        self
+00028810: 2e61 7373 6572 7454 7275 6528 6973 696e  .assertTrue(isin
+00028820: 7374 616e 6365 2877 312e 6669 6e64 4661  stance(w1.findFa
+00028830: 6365 2829 2c20 4661 6365 2929 0a20 2020  ce(), Face)).   
+00028840: 2020 2020 2077 6974 6820 7261 6973 6573       with raises
+00028850: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
+00028860: 2020 2020 2020 2020 2020 7731 2e66 696e            w1.fin
+00028870: 6446 6163 6528 7365 6172 6368 5374 6163  dFace(searchStac
+00028880: 6b3d 4661 6c73 6529 0a0a 2020 2020 2020  k=False)..      
+00028890: 2020 7732 203d 2077 312e 776f 726b 706c    w2 = w1.workpl
+000288a0: 616e 6528 292e 6369 7263 6c65 2830 2e31  ane().circle(0.1
+000288b0: 292e 6578 7472 7564 6528 302e 3129 0a20  ).extrude(0.1). 
+000288c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000288d0: 7274 5472 7565 2869 7369 6e73 7461 6e63  rtTrue(isinstanc
+000288e0: 6528 7732 2e66 696e 6446 6163 6528 7365  e(w2.findFace(se
+000288f0: 6172 6368 5061 7265 6e74 733d 5472 7565  archParents=True
+00028900: 292c 2046 6163 6529 290a 2020 2020 2020  ), Face)).      
+00028910: 2020 7769 7468 2072 6169 7365 7328 5661    with raises(Va
+00028920: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+00028930: 2020 2020 2020 2077 322e 6669 6e64 4661         w2.findFa
+00028940: 6365 2873 6561 7263 6850 6172 656e 7473  ce(searchParents
+00028950: 3d46 616c 7365 290a 0a20 2020 2064 6566  =False)..    def
+00028960: 2074 6573 7450 6f70 5065 6e64 696e 6728   testPopPending(
+00028970: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
+00028980: 2074 6573 7420 7065 6e64 696e 6720 6564   test pending ed
+00028990: 6765 730a 2020 2020 2020 2020 7730 203d  ges.        w0 =
+000289a0: 2057 6f72 6b70 6c61 6e65 2829 2e68 4c69   Workplane().hLi
+000289b0: 6e65 2831 290a 2020 2020 2020 2020 7365  ne(1).        se
+000289c0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+000289d0: 656e 2877 302e 6374 782e 7065 6e64 696e  en(w0.ctx.pendin
+000289e0: 6745 6467 6573 292c 2031 290a 2020 2020  gEdges), 1).    
+000289f0: 2020 2020 6564 6765 7320 3d20 7730 2e63      edges = w0.c
+00028a00: 7478 2e70 6f70 5065 6e64 696e 6745 6467  tx.popPendingEdg
+00028a10: 6573 2829 0a20 2020 2020 2020 2073 656c  es().        sel
+00028a20: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00028a30: 6e28 6564 6765 7329 2c20 3129 0a20 2020  n(edges), 1).   
+00028a40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00028a50: 4571 7561 6c28 6564 6765 735b 305d 2c20  Equal(edges[0], 
+00028a60: 7730 2e76 616c 2829 290a 2020 2020 2020  w0.val()).      
+00028a70: 2020 2320 7065 6e64 696e 6720 6564 6765    # pending edge
+00028a80: 7320 7368 6f75 6c64 206e 6f77 2062 6520  s should now be 
+00028a90: 636c 6561 7265 640a 2020 2020 2020 2020  cleared.        
+00028aa0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00028ab0: 286c 656e 2877 302e 6374 782e 7065 6e64  (len(w0.ctx.pend
+00028ac0: 696e 6745 6467 6573 292c 2030 290a 0a20  ingEdges), 0).. 
+00028ad0: 2020 2020 2020 2023 2074 6573 7420 7065         # test pe
+00028ae0: 6e64 696e 6720 7769 7265 730a 2020 2020  nding wires.    
+00028af0: 2020 2020 7731 203d 2057 6f72 6b70 6c61      w1 = Workpla
+00028b00: 6e65 2829 2e68 4c69 6e65 2831 292e 764c  ne().hLine(1).vL
+00028b10: 696e 6528 3129 2e63 6c6f 7365 2829 0a20  ine(1).close(). 
+00028b20: 2020 2020 2020 2077 6972 6520 3d20 7731         wire = w1
+00028b30: 2e76 616c 2829 0a20 2020 2020 2020 2073  .val().        s
+00028b40: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00028b50: 7731 2e63 7478 2e70 656e 6469 6e67 5769  w1.ctx.pendingWi
+00028b60: 7265 735b 305d 2c20 7769 7265 290a 2020  res[0], wire).  
+00028b70: 2020 2020 2020 706f 705f 7065 6e64 696e        pop_pendin
+00028b80: 675f 6f75 7470 7574 203d 2077 312e 6374  g_output = w1.ct
+00028b90: 782e 706f 7050 656e 6469 6e67 5769 7265  x.popPendingWire
+00028ba0: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
+00028bb0: 2e61 7373 6572 7445 7175 616c 2870 6f70  .assertEqual(pop
+00028bc0: 5f70 656e 6469 6e67 5f6f 7574 7075 745b  _pending_output[
+00028bd0: 305d 2c20 7769 7265 290a 2020 2020 2020  0], wire).      
+00028be0: 2020 2320 7065 6e64 696e 6720 7769 7265    # pending wire
+00028bf0: 7320 7368 6f75 6c64 206e 6f77 2062 6520  s should now be 
+00028c00: 636c 6561 7265 640a 2020 2020 2020 2020  cleared.        
+00028c10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00028c20: 286c 656e 2877 312e 6374 782e 7065 6e64  (len(w1.ctx.pend
+00028c30: 696e 6757 6972 6573 292c 2030 290a 0a20  ingWires), 0).. 
+00028c40: 2020 2020 2020 2023 2074 6573 7420 6572         # test er
+00028c50: 726f 7220 7768 656e 2065 6d70 7479 2070  ror when empty p
+00028c60: 656e 6469 6e67 2065 6467 6573 0a20 2020  ending edges.   
+00028c70: 2020 2020 2077 3220 3d20 576f 726b 706c       w2 = Workpl
+00028c80: 616e 6528 290a 2020 2020 2020 2020 2320  ane().        # 
+00028c90: 7468 6520 666f 6c6c 6f77 696e 6720 3220  the following 2 
+00028ca0: 7368 6f75 6c64 206e 6f74 2072 6169 7365  should not raise
+00028cb0: 2061 6e20 6578 6365 7074 696f 6e0a 2020   an exception.  
+00028cc0: 2020 2020 2020 7732 2e63 7478 2e70 6f70        w2.ctx.pop
+00028cd0: 5065 6e64 696e 6745 6467 6573 2865 7272  PendingEdges(err
+00028ce0: 6f72 4f6e 456d 7074 793d 4661 6c73 6529  orOnEmpty=False)
+00028cf0: 0a20 2020 2020 2020 2077 322e 6374 782e  .        w2.ctx.
+00028d00: 706f 7050 656e 6469 6e67 5769 7265 7328  popPendingWires(
+00028d10: 6572 726f 724f 6e45 6d70 7479 3d46 616c  errorOnEmpty=Fal
+00028d20: 7365 290a 0a20 2020 2020 2020 2023 2065  se)..        # e
+00028d30: 6d70 7479 2065 6467 6573 0a20 2020 2020  mpty edges.     
+00028d40: 2020 2077 3320 3d20 576f 726b 706c 616e     w3 = Workplan
+00028d50: 6528 292e 684c 696e 6528 3129 2e76 4c69  e().hLine(1).vLi
+00028d60: 6e65 2831 292e 636c 6f73 6528 290a 2020  ne(1).close().  
+00028d70: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00028d80: 6173 7365 7274 5261 6973 6573 2856 616c  assertRaises(Val
+00028d90: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
+00028da0: 2020 2020 2020 7733 2e63 7478 2e70 6f70        w3.ctx.pop
+00028db0: 5065 6e64 696e 6745 6467 6573 2829 0a0a  PendingEdges()..
+00028dc0: 2020 2020 2020 2020 2320 656d 7074 7920          # empty 
+00028dd0: 7769 7265 730a 2020 2020 2020 2020 7734  wires.        w4
+00028de0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e63   = Workplane().c
+00028df0: 6972 636c 6528 3129 2e65 7874 7275 6465  ircle(1).extrude
+00028e00: 2831 290a 2020 2020 2020 2020 7769 7468  (1).        with
+00028e10: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00028e20: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00028e30: 2020 2020 2020 2020 2020 2020 7734 2e63              w4.c
+00028e40: 7478 2e70 6f70 5065 6e64 696e 6757 6972  tx.popPendingWir
+00028e50: 6573 2829 0a0a 2020 2020 2020 2020 2320  es()..        # 
+00028e60: 7465 7374 2076 6961 2063 7574 426c 696e  test via cutBlin
+00028e70: 640a 2020 2020 2020 2020 7735 203d 2057  d.        w5 = W
+00028e80: 6f72 6b70 6c61 6e65 2829 2e63 6972 636c  orkplane().circl
+00028e90: 6528 3129 2e65 7874 7275 6465 2831 290a  e(1).extrude(1).
+00028ea0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00028eb0: 662e 6173 7365 7274 5261 6973 6573 2856  f.assertRaises(V
+00028ec0: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
+00028ed0: 2020 2020 2020 2020 7735 2e63 7574 426c          w5.cutBl
+00028ee0: 696e 6428 2d31 290a 0a20 2020 2064 6566  ind(-1)..    def
+00028ef0: 2074 6573 7443 6f6d 7053 6f6c 6964 2873   testCompSolid(s
+00028f00: 656c 6629 3a0a 0a20 2020 2020 2020 2066  elf):..        f
+00028f10: 726f 6d20 4f43 502e 4252 6570 5072 696d  rom OCP.BRepPrim
+00028f20: 4150 4920 696d 706f 7274 2042 5265 7050  API import BRepP
+00028f30: 7269 6d41 5049 5f4d 616b 6550 7269 736d  rimAPI_MakePrism
+00028f40: 0a0a 2020 2020 2020 2020 746f 6f6c 203d  ..        tool =
+00028f50: 2053 6f6c 6964 2e6d 616b 6553 7068 6572   Solid.makeSpher
+00028f60: 6528 312c 2061 6e67 6c65 4465 6772 6565  e(1, angleDegree
+00028f70: 7333 3d31 3230 290a 2020 2020 2020 2020  s3=120).        
+00028f80: 7368 656c 6c20 3d20 746f 6f6c 2e53 6865  shell = tool.She
+00028f90: 6c6c 7328 295b 305d 0a20 2020 2020 2020  lls()[0].       
+00028fa0: 2076 203d 2056 6563 746f 7228 302c 2030   v = Vector(0, 0
+00028fb0: 2c20 3129 0a0a 2020 2020 2020 2020 6275  , 1)..        bu
+00028fc0: 696c 6465 7220 3d20 4252 6570 5072 696d  ilder = BRepPrim
+00028fd0: 4150 495f 4d61 6b65 5072 6973 6d28 7368  API_MakePrism(sh
+00028fe0: 656c 6c2e 7772 6170 7065 642c 2076 2e77  ell.wrapped, v.w
+00028ff0: 7261 7070 6564 290a 2020 2020 2020 2020  rapped).        
+00029000: 7265 7375 6c74 203d 2053 6861 7065 2e63  result = Shape.c
+00029010: 6173 7428 6275 696c 6465 722e 5368 6170  ast(builder.Shap
+00029020: 6528 2929 0a0a 2020 2020 2020 2020 7365  e())..        se
+00029030: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00029040: 656e 2872 6573 756c 742e 436f 6d70 536f  en(result.CompSo
+00029050: 6c69 6473 2829 292c 2031 290a 2020 2020  lids()), 1).    
+00029060: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00029070: 7175 616c 286c 656e 2872 6573 756c 742e  qual(len(result.
+00029080: 536f 6c69 6473 2829 292c 2034 290a 0a20  Solids()), 4).. 
+00029090: 2020 2064 6566 2074 6573 7432 4466 696c     def test2Dfil
+000290a0: 6c65 7428 7365 6c66 293a 0a0a 2020 2020  let(self):..    
+000290b0: 2020 2020 7220 3d20 576f 726b 706c 616e      r = Workplan
+000290c0: 6528 292e 7265 6374 2831 2c20 3229 2e77  e().rect(1, 2).w
+000290d0: 6972 6573 2829 2e76 616c 2829 0a20 2020  ires().val().   
+000290e0: 2020 2020 2066 203d 2046 6163 652e 6d61       f = Face.ma
+000290f0: 6b65 4672 6f6d 5769 7265 7328 7229 0a20  keFromWires(r). 
+00029100: 2020 2020 2020 2076 6572 7473 203d 2072         verts = r
+00029110: 2e56 6572 7469 6365 7328 290a 0a20 2020  .Vertices()..   
+00029120: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00029130: 4571 7561 6c28 6c65 6e28 662e 6669 6c6c  Equal(len(f.fill
+00029140: 6574 3244 2830 2e35 2c20 7665 7274 7329  et2D(0.5, verts)
+00029150: 2e56 6572 7469 6365 7328 2929 2c20 3629  .Vertices()), 6)
+00029160: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00029170: 7365 7274 4571 7561 6c28 6c65 6e28 722e  sertEqual(len(r.
+00029180: 6669 6c6c 6574 3244 2830 2e35 2c20 7665  fillet2D(0.5, ve
+00029190: 7274 7329 2e56 6572 7469 6365 7328 2929  rts).Vertices())
+000291a0: 2c20 3629 0a20 2020 2020 2020 2073 656c  , 6).        sel
+000291b0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+000291c0: 6e28 722e 6669 6c6c 6574 3244 2830 2e32  n(r.fillet2D(0.2
+000291d0: 352c 2076 6572 7473 292e 5665 7274 6963  5, verts).Vertic
+000291e0: 6573 2829 292c 2038 290a 0a20 2020 2020  es()), 8)..     
+000291f0: 2020 2023 2054 6573 7420 6669 6c6c 6574     # Test fillet
+00029200: 3244 2077 6974 6820 6f70 656e 2077 6972  2D with open wir
+00029210: 6520 616e 6420 7369 6e67 6c65 2076 6572  e and single ver
+00029220: 7465 780a 2020 2020 2020 2020 7730 203d  tex.        w0 =
+00029230: 2057 6f72 6b70 6c61 6e65 2829 2e68 4c69   Workplane().hLi
+00029240: 6e65 2831 292e 764c 696e 6528 3129 2e77  ne(1).vLine(1).w
+00029250: 6972 6528 290a 2020 2020 2020 2020 7730  ire().        w0
+00029260: 5f76 6572 7473 203d 2077 302e 7665 7274  _verts = w0.vert
+00029270: 6963 6573 2822 3e58 2061 6e64 203c 5922  ices(">X and <Y"
+00029280: 292e 7661 6c73 2829 0a20 2020 2020 2020  ).vals().       
+00029290: 2075 6e66 696c 6c65 7465 645f 7769 7265   unfilleted_wire
+000292a0: 3020 3d20 7730 2e76 616c 2829 0a20 2020  0 = w0.val().   
+000292b0: 2020 2020 2066 696c 6c65 7465 645f 7769       filleted_wi
+000292c0: 7265 3020 3d20 756e 6669 6c6c 6574 6564  re0 = unfilleted
+000292d0: 5f77 6972 6530 2e66 696c 6c65 7432 4428  _wire0.fillet2D(
+000292e0: 302e 352c 2077 305f 7665 7274 7329 0a0a  0.5, w0_verts)..
+000292f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00029300: 6572 7445 7175 616c 286c 656e 2866 696c  ertEqual(len(fil
+00029310: 6c65 7465 645f 7769 7265 302e 5665 7274  leted_wire0.Vert
+00029320: 6963 6573 2829 292c 2034 290a 0a20 2020  ices()), 4)..   
+00029330: 2020 2020 2023 2074 6865 2066 696c 6c65       # the fille
+00029340: 7465 6420 7769 7265 2069 7320 7368 6f72  ted wire is shor
+00029350: 7465 7220 7468 616e 2074 6865 206f 7269  ter than the ori
+00029360: 6769 6e61 6c0a 2020 2020 2020 2020 7365  ginal.        se
+00029370: 6c66 2e61 7373 6572 7447 7265 6174 6572  lf.assertGreater
+00029380: 2875 6e66 696c 6c65 7465 645f 7769 7265  (unfilleted_wire
+00029390: 302e 4c65 6e67 7468 2829 202d 2066 696c  0.Length() - fil
+000293a0: 6c65 7465 645f 7769 7265 302e 4c65 6e67  leted_wire0.Leng
+000293b0: 7468 2829 2c20 302e 3129 0a0a 2020 2020  th(), 0.1)..    
+000293c0: 6465 6620 7465 7374 3244 6368 616d 6665  def test2Dchamfe
+000293d0: 7228 7365 6c66 293a 0a0a 2020 2020 2020  r(self):..      
+000293e0: 2020 7220 3d20 576f 726b 706c 616e 6528    r = Workplane(
+000293f0: 292e 7265 6374 2831 2c20 3229 2e77 6972  ).rect(1, 2).wir
+00029400: 6573 2829 2e76 616c 2829 0a20 2020 2020  es().val().     
+00029410: 2020 2066 203d 2046 6163 652e 6d61 6b65     f = Face.make
+00029420: 4672 6f6d 5769 7265 7328 7229 0a20 2020  FromWires(r).   
+00029430: 2020 2020 2076 6572 7473 203d 2072 2e56       verts = r.V
+00029440: 6572 7469 6365 7328 290a 0a20 2020 2020  ertices()..     
+00029450: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00029460: 7561 6c28 6c65 6e28 662e 6368 616d 6665  ual(len(f.chamfe
+00029470: 7232 4428 302e 352c 2076 6572 7473 292e  r2D(0.5, verts).
+00029480: 5665 7274 6963 6573 2829 292c 2036 290a  Vertices()), 6).
+00029490: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000294a0: 6572 7445 7175 616c 286c 656e 2872 2e63  ertEqual(len(r.c
+000294b0: 6861 6d66 6572 3244 2830 2e35 2c20 7665  hamfer2D(0.5, ve
+000294c0: 7274 7329 2e56 6572 7469 6365 7328 2929  rts).Vertices())
+000294d0: 2c20 3629 0a20 2020 2020 2020 2073 656c  , 6).        sel
+000294e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+000294f0: 6e28 722e 6368 616d 6665 7232 4428 302e  n(r.chamfer2D(0.
+00029500: 3235 2c20 7665 7274 7329 2e56 6572 7469  25, verts).Verti
+00029510: 6365 7328 2929 2c20 3829 0a0a 2020 2020  ces()), 8)..    
+00029520: 2020 2020 7220 3d20 576f 726b 706c 616e      r = Workplan
+00029530: 6528 292e 684c 696e 6528 3129 2e76 4c69  e().hLine(1).vLi
+00029540: 6e65 2831 292e 7769 7265 2829 2e76 616c  ne(1).wire().val
+00029550: 2829 0a20 2020 2020 2020 2076 7320 3d20  ().        vs = 
+00029560: 722e 5665 7274 6963 6573 2829 0a0a 2020  r.Vertices()..  
+00029570: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00029580: 7445 7175 616c 286c 656e 2872 2e63 6861  tEqual(len(r.cha
+00029590: 6d66 6572 3244 2830 2e32 352c 205b 7673  mfer2D(0.25, [vs
+000295a0: 5b31 5d5d 292e 5665 7274 6963 6573 2829  [1]]).Vertices()
+000295b0: 292c 2034 290a 0a20 2020 2020 2020 2077  ), 4)..        w
+000295c0: 6974 6820 7261 6973 6573 2856 616c 7565  ith raises(Value
+000295d0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+000295e0: 2020 2020 722e 6368 616d 6665 7232 4428      r.chamfer2D(
+000295f0: 302e 3235 2c20 5b76 735b 305d 5d29 0a0a  0.25, [vs[0]])..
+00029600: 2020 2020 6465 6620 7465 7374 5f46 6163      def test_Fac
+00029610: 655f 6d61 6b65 4672 6f6d 5769 7265 7328  e_makeFromWires(
+00029620: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+00029630: 7730 203d 2057 6972 652e 6173 7365 6d62  w0 = Wire.assemb
+00029640: 6c65 4564 6765 7328 0a20 2020 2020 2020  leEdges(.       
+00029650: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00029660: 2020 2020 2020 2045 6467 652e 6d61 6b65         Edge.make
+00029670: 4c69 6e65 2856 6563 746f 7228 292c 2056  Line(Vector(), V
+00029680: 6563 746f 7228 302c 2031 2929 2c0a 2020  ector(0, 1)),.  
+00029690: 2020 2020 2020 2020 2020 2020 2020 4564                Ed
+000296a0: 6765 2e6d 616b 654c 696e 6528 5665 6374  ge.makeLine(Vect
+000296b0: 6f72 2830 2c20 3129 2c20 5665 6374 6f72  or(0, 1), Vector
+000296c0: 2831 2c20 3129 292c 0a20 2020 2020 2020  (1, 1)),.       
+000296d0: 2020 2020 2020 2020 2045 6467 652e 6d61           Edge.ma
+000296e0: 6b65 4c69 6e65 2856 6563 746f 7228 312c  keLine(Vector(1,
+000296f0: 2031 292c 2056 6563 746f 7228 312c 2030   1), Vector(1, 0
+00029700: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00029710: 2020 2020 4564 6765 2e6d 616b 654c 696e      Edge.makeLin
+00029720: 6528 5665 6374 6f72 2831 2c20 3029 2c20  e(Vector(1, 0), 
+00029730: 5665 6374 6f72 2830 2c20 3029 292c 0a20  Vector(0, 0)),. 
+00029740: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00029750: 2020 2020 2029 0a20 2020 2020 2020 2077       ).        w
+00029760: 3120 3d20 5769 7265 2e61 7373 656d 626c  1 = Wire.assembl
+00029770: 6545 6467 6573 280a 2020 2020 2020 2020  eEdges(.        
+00029780: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00029790: 2020 2020 2020 4564 6765 2e6d 616b 654c        Edge.makeL
+000297a0: 696e 6528 5665 6374 6f72 2830 2e32 352c  ine(Vector(0.25,
+000297b0: 2030 2e32 3529 2c20 5665 6374 6f72 2830   0.25), Vector(0
+000297c0: 2e32 352c 2030 2e37 3529 292c 0a20 2020  .25, 0.75)),.   
+000297d0: 2020 2020 2020 2020 2020 2020 2045 6467               Edg
+000297e0: 652e 6d61 6b65 4c69 6e65 2856 6563 746f  e.makeLine(Vecto
+000297f0: 7228 302e 3235 2c20 302e 3735 292c 2056  r(0.25, 0.75), V
+00029800: 6563 746f 7228 302e 3735 2c20 302e 3735  ector(0.75, 0.75
+00029810: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00029820: 2020 2020 4564 6765 2e6d 616b 654c 696e      Edge.makeLin
+00029830: 6528 5665 6374 6f72 2830 2e37 352c 2030  e(Vector(0.75, 0
+00029840: 2e37 3529 2c20 5665 6374 6f72 2830 2e37  .75), Vector(0.7
+00029850: 352c 2030 2e32 3529 292c 0a20 2020 2020  5, 0.25)),.     
+00029860: 2020 2020 2020 2020 2020 2045 6467 652e             Edge.
+00029870: 6d61 6b65 4c69 6e65 2856 6563 746f 7228  makeLine(Vector(
+00029880: 302e 3735 2c20 302e 3235 292c 2056 6563  0.75, 0.25), Vec
+00029890: 746f 7228 302e 3235 2c20 302e 3235 2929  tor(0.25, 0.25))
+000298a0: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
+000298b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000298c0: 2020 6620 3d20 4661 6365 2e6d 616b 6546    f = Face.makeF
+000298d0: 726f 6d57 6972 6573 2877 302c 205b 7731  romWires(w0, [w1
+000298e0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
+000298f0: 7420 662e 6973 5661 6c69 6428 290a 0a20  t f.isValid().. 
+00029900: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
+00029910: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00029920: 2020 2020 2020 2020 2020 2020 7730 203d              w0 =
+00029930: 2057 6972 652e 6173 7365 6d62 6c65 4564   Wire.assembleEd
+00029940: 6765 7328 5b45 6467 652e 6d61 6b65 4c69  ges([Edge.makeLi
+00029950: 6e65 2856 6563 746f 7228 292c 2056 6563  ne(Vector(), Vec
+00029960: 746f 7228 302c 2031 2929 2c5d 290a 2020  tor(0, 1)),]).  
+00029970: 2020 2020 2020 2020 2020 7731 203d 2057            w1 = W
+00029980: 6972 652e 6173 7365 6d62 6c65 4564 6765  ire.assembleEdge
+00029990: 7328 5b45 6467 652e 6d61 6b65 4c69 6e65  s([Edge.makeLine
+000299a0: 2856 6563 746f 7228 302c 2031 292c 2056  (Vector(0, 1), V
+000299b0: 6563 746f 7228 312c 2031 2929 2c5d 290a  ector(1, 1)),]).
+000299c0: 2020 2020 2020 2020 2020 2020 6620 3d20              f = 
+000299d0: 4661 6365 2e6d 616b 6546 726f 6d57 6972  Face.makeFromWir
+000299e0: 6573 2877 302c 205b 7731 5d29 0a0a 2020  es(w0, [w1])..  
+000299f0: 2020 2020 2020 7769 7468 2072 6169 7365        with raise
+00029a00: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
+00029a10: 2020 2020 2020 2020 2020 2077 3020 3d20             w0 = 
+00029a20: 5769 7265 2e61 7373 656d 626c 6545 6467  Wire.assembleEdg
+00029a30: 6573 285b 4564 6765 2e6d 616b 654c 696e  es([Edge.makeLin
+00029a40: 6528 5665 6374 6f72 2829 2c20 5665 6374  e(Vector(), Vect
+00029a50: 6f72 2830 2c20 3129 292c 5d29 0a20 2020  or(0, 1)),]).   
+00029a60: 2020 2020 2020 2020 2077 3120 3d20 5769           w1 = Wi
+00029a70: 7265 2e61 7373 656d 626c 6545 6467 6573  re.assembleEdges
+00029a80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00029a90: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00029aa0: 2020 2020 2020 2020 4564 6765 2e6d 616b          Edge.mak
+00029ab0: 654c 696e 6528 5665 6374 6f72 2829 2c20  eLine(Vector(), 
+00029ac0: 5665 6374 6f72 2831 2c20 3129 292c 0a20  Vector(1, 1)),. 
+00029ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ae0: 2020 2045 6467 652e 6d61 6b65 4c69 6e65     Edge.makeLine
+00029af0: 2856 6563 746f 7228 312c 2031 292c 2056  (Vector(1, 1), V
+00029b00: 6563 746f 7228 322c 2030 2929 2c0a 2020  ector(2, 0)),.  
+00029b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029b20: 2020 4564 6765 2e6d 616b 654c 696e 6528    Edge.makeLine(
+00029b30: 5665 6374 6f72 2832 2c20 3029 2c20 5665  Vector(2, 0), Ve
+00029b40: 6374 6f72 2830 2c20 3029 292c 0a20 2020  ctor(0, 0)),.   
+00029b50: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+00029b60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00029b70: 2020 2020 2020 2020 2066 203d 2046 6163           f = Fac
+00029b80: 652e 6d61 6b65 4672 6f6d 5769 7265 7328  e.makeFromWires(
+00029b90: 7730 2c20 5b77 315d 290a 0a20 2020 2020  w0, [w1])..     
+00029ba0: 2020 2077 6974 6820 7261 6973 6573 2856     with raises(V
+00029bb0: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
+00029bc0: 2020 2020 2020 2020 7730 203d 2057 6972          w0 = Wir
+00029bd0: 652e 6173 7365 6d62 6c65 4564 6765 7328  e.assembleEdges(
+00029be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029bf0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00029c00: 2020 2020 2020 2045 6467 652e 6d61 6b65         Edge.make
+00029c10: 4c69 6e65 2856 6563 746f 7228 292c 2056  Line(Vector(), V
+00029c20: 6563 746f 7228 312c 2031 2929 2c0a 2020  ector(1, 1)),.  
+00029c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c40: 2020 4564 6765 2e6d 616b 654c 696e 6528    Edge.makeLine(
+00029c50: 5665 6374 6f72 2831 2c20 3129 2c20 5665  Vector(1, 1), Ve
+00029c60: 6374 6f72 2832 2c20 3029 292c 0a20 2020  ctor(2, 0)),.   
+00029c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c80: 2045 6467 652e 6d61 6b65 4c69 6e65 2856   Edge.makeLine(V
+00029c90: 6563 746f 7228 322c 2030 292c 2056 6563  ector(2, 0), Vec
+00029ca0: 746f 7228 302c 2030 2929 2c0a 2020 2020  tor(0, 0)),.    
+00029cb0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00029cc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00029cd0: 2020 2020 2020 2020 7731 203d 2057 6972          w1 = Wir
+00029ce0: 652e 6173 7365 6d62 6c65 4564 6765 7328  e.assembleEdges(
+00029cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029d00: 205b 4564 6765 2e6d 616b 654c 696e 6528   [Edge.makeLine(
+00029d10: 5665 6374 6f72 2830 2e31 2c20 302e 3129  Vector(0.1, 0.1)
+00029d20: 2c20 5665 6374 6f72 2830 2e32 2c20 302e  , Vector(0.2, 0.
+00029d30: 3229 292c 5d0a 2020 2020 2020 2020 2020  2)),].          
+00029d40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00029d50: 6620 3d20 4661 6365 2e6d 616b 6546 726f  f = Face.makeFro
+00029d60: 6d57 6972 6573 2877 302c 205b 7731 5d29  mWires(w0, [w1])
+00029d70: 0a0a 2020 2020 6465 6620 7465 7374 5370  ..    def testSp
+00029d80: 6c69 6e65 4170 7072 6f78 2873 656c 6629  lineApprox(self)
+00029d90: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+00029da0: 2e6e 6163 6120 696d 706f 7274 206e 6163  .naca import nac
+00029db0: 6135 3330 350a 2020 2020 2020 2020 6672  a5305.        fr
+00029dc0: 6f6d 206d 6174 6820 696d 706f 7274 2070  om math import p
+00029dd0: 692c 2063 6f73 0a0a 2020 2020 2020 2020  i, cos..        
+00029de0: 7074 7320 3d20 5b56 6563 746f 7228 655b  pts = [Vector(e[
+00029df0: 305d 2c20 655b 315d 2c20 3029 2066 6f72  0], e[1], 0) for
+00029e00: 2065 2069 6e20 6e61 6361 3533 3035 5d0a   e in naca5305].
+00029e10: 0a20 2020 2020 2020 2023 2073 706c 696e  .        # splin
+00029e20: 650a 0a20 2020 2020 2020 2065 3120 3d20  e..        e1 = 
+00029e30: 4564 6765 2e6d 616b 6553 706c 696e 6541  Edge.makeSplineA
+00029e40: 7070 726f 7828 7074 732c 2031 652d 362c  pprox(pts, 1e-6,
+00029e50: 206d 6178 4465 673d 362c 2073 6d6f 6f74   maxDeg=6, smoot
+00029e60: 6869 6e67 3d28 312c 2031 2c20 3129 290a  hing=(1, 1, 1)).
+00029e70: 2020 2020 2020 2020 6532 203d 2045 6467          e2 = Edg
+00029e80: 652e 6d61 6b65 5370 6c69 6e65 4170 7072  e.makeSplineAppr
+00029e90: 6f78 2870 7473 2c20 3165 2d36 2c20 6d69  ox(pts, 1e-6, mi
+00029ea0: 6e44 6567 3d32 2c20 6d61 7844 6567 3d36  nDeg=2, maxDeg=6
+00029eb0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00029ec0: 6173 7365 7274 5472 7565 2865 312e 6973  assertTrue(e1.is
+00029ed0: 5661 6c69 6428 2929 0a20 2020 2020 2020  Valid()).       
+00029ee0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00029ef0: 2865 322e 6973 5661 6c69 6428 2929 0a20  (e2.isValid()). 
+00029f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00029f10: 7274 5472 7565 2865 312e 4c65 6e67 7468  rtTrue(e1.Length
+00029f20: 2829 203e 2065 322e 4c65 6e67 7468 2829  () > e2.Length()
+00029f30: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00029f40: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
+00029f50: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00029f60: 6534 203d 2045 6467 652e 6d61 6b65 5370  e4 = Edge.makeSp
+00029f70: 6c69 6e65 4170 7072 6f78 2870 7473 2c20  lineApprox(pts, 
+00029f80: 3165 2d36 2c20 6d61 7844 6567 3d33 2c20  1e-6, maxDeg=3, 
+00029f90: 736d 6f6f 7468 696e 673d 2831 2c20 312c  smoothing=(1, 1,
+00029fa0: 2031 2e30 2929 0a0a 2020 2020 2020 2020   1.0))..        
+00029fb0: 7074 735f 636c 6f73 6564 203d 2070 7473  pts_closed = pts
+00029fc0: 202b 205b 7074 735b 305d 5d0a 0a20 2020   + [pts[0]]..   
+00029fd0: 2020 2020 2065 3320 3d20 4564 6765 2e6d       e3 = Edge.m
+00029fe0: 616b 6553 706c 696e 6541 7070 726f 7828  akeSplineApprox(
+00029ff0: 7074 735f 636c 6f73 6564 290a 2020 2020  pts_closed).    
+0002a000: 2020 2020 7720 3d20 4564 6765 2e6d 616b      w = Edge.mak
+0002a010: 6553 706c 696e 6541 7070 726f 7828 7074  eSplineApprox(pt
+0002a020: 7329 2e63 6c6f 7365 2829 0a0a 2020 2020  s).close()..    
+0002a030: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0002a040: 7275 6528 6533 2e49 7343 6c6f 7365 6428  rue(e3.IsClosed(
+0002a050: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0002a060: 6173 7365 7274 5472 7565 2877 2e49 7343  assertTrue(w.IsC
+0002a070: 6c6f 7365 6428 2929 0a0a 2020 2020 2020  losed())..      
+0002a080: 2020 2320 576f 726b 706c 616e 6520 6d65    # Workplane me
+0002a090: 7468 6f64 0a0a 2020 2020 2020 2020 7731  thod..        w1
+0002a0a0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e73   = Workplane().s
+0002a0b0: 706c 696e 6541 7070 726f 7828 7074 7329  plineApprox(pts)
+0002a0c0: 0a20 2020 2020 2020 2077 3220 3d20 576f  .        w2 = Wo
+0002a0d0: 726b 706c 616e 6528 292e 7370 6c69 6e65  rkplane().spline
+0002a0e0: 4170 7072 6f78 2870 7473 2c20 666f 7243  Approx(pts, forC
+0002a0f0: 6f6e 7374 7275 6374 696f 6e3d 5472 7565  onstruction=True
+0002a100: 290a 2020 2020 2020 2020 7733 203d 2057  ).        w3 = W
+0002a110: 6f72 6b70 6c61 6e65 2829 2e73 706c 696e  orkplane().splin
+0002a120: 6541 7070 726f 7828 7074 732c 206d 616b  eApprox(pts, mak
+0002a130: 6557 6972 653d 5472 7565 290a 2020 2020  eWire=True).    
+0002a140: 2020 2020 7734 203d 2057 6f72 6b70 6c61      w4 = Workpla
+0002a150: 6e65 2829 2e73 706c 696e 6541 7070 726f  ne().splineAppro
+0002a160: 7828 7074 732c 206d 616b 6557 6972 653d  x(pts, makeWire=
+0002a170: 5472 7565 2c20 666f 7243 6f6e 7374 7275  True, forConstru
+0002a180: 6374 696f 6e3d 5472 7565 290a 0a20 2020  ction=True)..   
+0002a190: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0002a1a0: 4571 7561 6c28 7731 2e65 6467 6573 2829  Equal(w1.edges()
+0002a1b0: 2e73 697a 6528 292c 2031 290a 2020 2020  .size(), 1).    
+0002a1c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002a1d0: 7175 616c 286c 656e 2877 312e 6374 782e  qual(len(w1.ctx.
+0002a1e0: 7065 6e64 696e 6745 6467 6573 292c 2031  pendingEdges), 1
+0002a1f0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002a200: 7373 6572 7445 7175 616c 2877 322e 6564  ssertEqual(w2.ed
+0002a210: 6765 7328 292e 7369 7a65 2829 2c20 3129  ges().size(), 1)
+0002a220: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0002a230: 7365 7274 4571 7561 6c28 6c65 6e28 7732  sertEqual(len(w2
+0002a240: 2e63 7478 2e70 656e 6469 6e67 4564 6765  .ctx.pendingEdge
+0002a250: 7329 2c20 3029 0a20 2020 2020 2020 2073  s), 0).        s
+0002a260: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0002a270: 7733 2e77 6972 6573 2829 2e73 697a 6528  w3.wires().size(
+0002a280: 292c 2031 290a 2020 2020 2020 2020 7365  ), 1).        se
+0002a290: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+0002a2a0: 656e 2877 332e 6374 782e 7065 6e64 696e  en(w3.ctx.pendin
+0002a2b0: 6757 6972 6573 292c 2031 290a 2020 2020  gWires), 1).    
+0002a2c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002a2d0: 7175 616c 2877 342e 7769 7265 7328 292e  qual(w4.wires().
+0002a2e0: 7369 7a65 2829 2c20 3129 0a20 2020 2020  size(), 1).     
+0002a2f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002a300: 7561 6c28 6c65 6e28 7734 2e63 7478 2e70  ual(len(w4.ctx.p
+0002a310: 656e 6469 6e67 5769 7265 7329 2c20 3029  endingWires), 0)
+0002a320: 0a0a 2020 2020 2020 2020 2320 7370 6c69  ..        # spli
+0002a330: 6e65 2073 7572 6661 6365 0a0a 2020 2020  ne surface..    
+0002a340: 2020 2020 4e20 3d20 3430 0a20 2020 2020      N = 40.     
+0002a350: 2020 2054 203d 2032 300a 2020 2020 2020     T = 20.      
+0002a360: 2020 4120 3d20 350a 0a20 2020 2020 2020    A = 5..       
+0002a370: 2070 7473 203d 205b 0a20 2020 2020 2020   pts = [.       
+0002a380: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+0002a390: 2020 2020 2020 2056 6563 746f 7228 692c         Vector(i,
+0002a3a0: 206a 2c20 4120 2a20 636f 7328 3220 2a20   j, A * cos(2 * 
+0002a3b0: 7069 202a 2069 202f 2054 2920 2a20 636f  pi * i / T) * co
+0002a3c0: 7328 3220 2a20 7069 202a 206a 202f 2054  s(2 * pi * j / T
+0002a3d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0002a3e0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0002a3f0: 6528 4e20 2b20 3129 0a20 2020 2020 2020  e(N + 1).       
+0002a400: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0002a410: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+0002a420: 6528 4e20 2b20 3129 0a20 2020 2020 2020  e(N + 1).       
+0002a430: 205d 0a0a 2020 2020 2020 2020 6631 203d   ]..        f1 =
+0002a440: 2046 6163 652e 6d61 6b65 5370 6c69 6e65   Face.makeSpline
+0002a450: 4170 7072 6f78 2870 7473 2c20 736d 6f6f  Approx(pts, smoo
+0002a460: 7468 696e 673d 2831 2c20 312c 2031 292c  thing=(1, 1, 1),
+0002a470: 206d 6178 4465 673d 3629 0a20 2020 2020   maxDeg=6).     
+0002a480: 2020 2066 3220 3d20 4661 6365 2e6d 616b     f2 = Face.mak
+0002a490: 6553 706c 696e 6541 7070 726f 7828 7074  eSplineApprox(pt
+0002a4a0: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
+0002a4b0: 2e61 7373 6572 7454 7275 6528 6631 2e69  .assertTrue(f1.i
+0002a4c0: 7356 616c 6964 2829 290a 2020 2020 2020  sValid()).      
+0002a4d0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0002a4e0: 6528 6632 2e69 7356 616c 6964 2829 290a  e(f2.isValid()).
+0002a4f0: 0a20 2020 2020 2020 2077 6974 6820 7261  .        with ra
+0002a500: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+0002a510: 3a0a 2020 2020 2020 2020 2020 2020 6633  :.            f3
+0002a520: 203d 2046 6163 652e 6d61 6b65 5370 6c69   = Face.makeSpli
+0002a530: 6e65 4170 7072 6f78 2870 7473 2c20 736d  neApprox(pts, sm
+0002a540: 6f6f 7468 696e 673d 2831 2c20 312c 2031  oothing=(1, 1, 1
+0002a550: 292c 206d 6178 4465 673d 3329 0a0a 2020  ), maxDeg=3)..  
+0002a560: 2020 6465 6620 7465 7374 5061 7261 6d65    def testParame
+0002a570: 7472 6963 5375 7266 6163 6528 7365 6c66  tricSurface(self
+0002a580: 293a 0a0a 2020 2020 2020 2020 6672 6f6d  ):..        from
+0002a590: 206d 6174 6820 696d 706f 7274 2070 692c   math import pi,
+0002a5a0: 2063 6f73 0a0a 2020 2020 2020 2020 7231   cos..        r1
+0002a5b0: 203d 2057 6f72 6b70 6c61 6e65 2829 2e70   = Workplane().p
+0002a5c0: 6172 616d 6574 7269 6353 7572 6661 6365  arametricSurface
+0002a5d0: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
+0002a5e0: 6d62 6461 2075 2c20 763a 2028 752c 2076  mbda u, v: (u, v
+0002a5f0: 2c20 636f 7328 7069 202a 2075 2920 2a20  , cos(pi * u) * 
+0002a600: 636f 7328 7069 202a 2076 2929 2c20 7374  cos(pi * v)), st
+0002a610: 6172 743d 2d31 2c20 7374 6f70 3d31 0a20  art=-1, stop=1. 
+0002a620: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0002a630: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0002a640: 6528 7231 2e66 6163 6573 2829 2e76 616c  e(r1.faces().val
+0002a650: 2829 2e69 7356 616c 6964 2829 290a 0a20  ().isValid()).. 
+0002a660: 2020 2020 2020 2072 3220 3d20 576f 726b         r2 = Work
+0002a670: 706c 616e 6528 292e 626f 7828 312c 2031  plane().box(1, 1
+0002a680: 2c20 3329 2e73 706c 6974 2872 3129 0a0a  , 3).split(r1)..
+0002a690: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0002a6a0: 6572 7454 7275 6528 7232 2e73 6f6c 6964  ertTrue(r2.solid
+0002a6b0: 7328 292e 7661 6c28 292e 6973 5661 6c69  s().val().isVali
+0002a6c0: 6428 2929 0a20 2020 2020 2020 2073 656c  d()).        sel
+0002a6d0: 662e 6173 7365 7274 4571 7561 6c28 7232  f.assertEqual(r2
+0002a6e0: 2e73 6f6c 6964 7328 292e 7369 7a65 2829  .solids().size()
+0002a6f0: 2c20 3229 0a0a 2020 2020 6465 6620 7465  , 2)..    def te
+0002a700: 7374 4564 6765 5769 7265 436c 6f73 6528  stEdgeWireClose(
+0002a710: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+0002a720: 2320 7465 7374 2077 6974 6820 6564 6765  # test with edge
+0002a730: 0a20 2020 2020 2020 2065 3020 3d20 4564  .        e0 = Ed
+0002a740: 6765 2e6d 616b 6554 6872 6565 506f 696e  ge.makeThreePoin
+0002a750: 7441 7263 2856 6563 746f 7228 302c 2030  tArc(Vector(0, 0
+0002a760: 2c20 3029 2c20 5665 6374 6f72 2831 2c20  , 0), Vector(1, 
+0002a770: 312c 2030 292c 2056 6563 746f 7228 302c  1, 0), Vector(0,
+0002a780: 2032 2c20 3029 290a 2020 2020 2020 2020   2, 0)).        
+0002a790: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+0002a7a0: 2865 302e 4973 436c 6f73 6564 2829 290a  (e0.IsClosed()).
+0002a7b0: 2020 2020 2020 2020 7730 203d 2065 302e          w0 = e0.
+0002a7c0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+0002a7d0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+0002a7e0: 7730 2e49 7343 6c6f 7365 6428 2929 0a0a  w0.IsClosed())..
+0002a7f0: 2020 2020 2020 2020 2320 7465 7374 2077          # test w
+0002a800: 6974 6820 616c 7265 6164 7920 636c 6f73  ith already clos
+0002a810: 6564 2065 6467 650a 2020 2020 2020 2020  ed edge.        
+0002a820: 6531 203d 2045 6467 652e 6d61 6b65 4369  e1 = Edge.makeCi
+0002a830: 7263 6c65 2831 290a 2020 2020 2020 2020  rcle(1).        
+0002a840: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+0002a850: 6531 2e49 7343 6c6f 7365 6428 2929 0a20  e1.IsClosed()). 
+0002a860: 2020 2020 2020 2065 3220 3d20 6531 2e63         e2 = e1.c
+0002a870: 6c6f 7365 2829 0a20 2020 2020 2020 2073  lose().        s
+0002a880: 656c 662e 6173 7365 7274 5472 7565 2865  elf.assertTrue(e
+0002a890: 322e 4973 436c 6f73 6564 2829 290a 2020  2.IsClosed()).  
+0002a8a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002a8b0: 7445 7175 616c 2874 7970 6528 6531 292c  tEqual(type(e1),
+0002a8c0: 2074 7970 6528 6532 2929 0a0a 2020 2020   type(e2))..    
+0002a8d0: 2020 2020 2320 7465 7374 2077 6974 6820      # test with 
+0002a8e0: 616c 7265 6164 7920 636c 6f73 6564 2057  already closed W
+0002a8f0: 4952 450a 2020 2020 2020 2020 7731 203d  IRE.        w1 =
+0002a900: 2057 6972 652e 6d61 6b65 4369 7263 6c65   Wire.makeCircle
+0002a910: 2831 2c20 5665 6374 6f72 2829 2c20 5665  (1, Vector(), Ve
+0002a920: 6374 6f72 2830 2c20 302c 2031 2929 0a20  ctor(0, 0, 1)). 
+0002a930: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002a940: 7274 5472 7565 2877 312e 4973 436c 6f73  rtTrue(w1.IsClos
+0002a950: 6564 2829 290a 2020 2020 2020 2020 7732  ed()).        w2
+0002a960: 203d 2077 312e 636c 6f73 6528 290a 2020   = w1.close().  
+0002a970: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002a980: 7454 7275 6528 7731 2069 7320 7732 290a  tTrue(w1 is w2).
+0002a990: 0a20 2020 2064 6566 2074 6573 745f 636c  .    def test_cl
+0002a9a0: 6f73 655f 3344 5f70 6f69 6e74 7328 7365  ose_3D_points(se
+0002a9b0: 6c66 293a 0a20 2020 2020 2020 2072 203d  lf):.        r =
+0002a9c0: 2057 6f72 6b70 6c61 6e65 2829 2e70 6f6c   Workplane().pol
+0002a9d0: 796c 696e 6528 5b28 302c 2030 2c20 3130  yline([(0, 0, 10
+0002a9e0: 292c 2028 352c 2030 2c20 3132 292c 2028  ), (5, 0, 12), (
+0002a9f0: 302c 2035 2c20 3130 292c 5d29 2e63 6c6f  0, 5, 10),]).clo
+0002aa00: 7365 2829 0a20 2020 2020 2020 2061 7373  se().        ass
+0002aa10: 6572 7420 722e 7769 7265 2829 2e76 616c  ert r.wire().val
+0002aa20: 2829 2e43 6c6f 7365 6428 290a 0a20 2020  ().Closed()..   
+0002aa30: 2064 6566 2074 6573 7453 706c 6974 5368   def testSplitSh
+0002aa40: 6170 6528 7365 6c66 293a 0a20 2020 2020  ape(self):.     
+0002aa50: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
+0002aa60: 6573 7469 6e67 2074 6865 2053 6861 7065  esting the Shape
+0002aa70: 2e73 706c 6974 206d 6574 686f 642e 0a20  .split method.. 
+0002aa80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002aa90: 2020 2023 2073 706c 6974 2061 6e20 6564     # split an ed
+0002aaa0: 6765 2077 6974 6820 6120 7665 7274 6578  ge with a vertex
+0002aab0: 0a20 2020 2020 2020 2065 3020 3d20 4564  .        e0 = Ed
+0002aac0: 6765 2e6d 616b 6543 6972 636c 6528 312c  ge.makeCircle(1,
+0002aad0: 2028 302c 2030 2c20 3029 2c20 2830 2c20   (0, 0, 0), (0, 
+0002aae0: 302c 2031 2929 0a20 2020 2020 2020 2076  0, 1)).        v
+0002aaf0: 3020 3d20 5665 7274 6578 2e6d 616b 6556  0 = Vertex.makeV
+0002ab00: 6572 7465 7828 302c 2031 2c20 3029 0a20  ertex(0, 1, 0). 
+0002ab10: 2020 2020 2020 206c 6973 745f 6f66 5f65         list_of_e
+0002ab20: 6467 6573 203d 2065 302e 7370 6c69 7428  dges = e0.split(
+0002ab30: 7630 292e 4564 6765 7328 290a 2020 2020  v0).Edges().    
+0002ab40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002ab50: 7175 616c 286c 656e 286c 6973 745f 6f66  qual(len(list_of
+0002ab60: 5f65 6467 6573 292c 2032 290a 2020 2020  _edges), 2).    
+0002ab70: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0002ab80: 7275 6528 5665 6374 6f72 2830 2c20 312c  rue(Vector(0, 1,
+0002ab90: 2030 2920 696e 205b 652e 656e 6450 6f69   0) in [e.endPoi
+0002aba0: 6e74 2829 2066 6f72 2065 2069 6e20 6c69  nt() for e in li
+0002abb0: 7374 5f6f 665f 6564 6765 735d 290a 0a20  st_of_edges]).. 
+0002abc0: 2020 2020 2020 2023 2073 706c 6974 2061         # split a
+0002abd0: 2063 6972 636c 6520 7769 7468 206d 756c   circle with mul
+0002abe0: 7469 706c 6520 7665 7274 6963 6573 0a20  tiple vertices. 
+0002abf0: 2020 2020 2020 2061 6e67 6c65 7320 3d20         angles = 
+0002ac00: 5b32 202a 206d 6174 682e 7069 202a 2069  [2 * math.pi * i
+0002ac10: 6478 202f 2031 3020 666f 7220 6964 7820  dx / 10 for idx 
+0002ac20: 696e 2072 616e 6765 2831 3029 5d0a 2020  in range(10)].  
+0002ac30: 2020 2020 2020 7665 6373 203d 205b 5665        vecs = [Ve
+0002ac40: 6374 6f72 286d 6174 682e 7369 6e28 6129  ctor(math.sin(a)
+0002ac50: 2c20 6d61 7468 2e63 6f73 2861 292c 2030  , math.cos(a), 0
+0002ac60: 2920 666f 7220 6120 696e 2061 6e67 6c65  ) for a in angle
+0002ac70: 735d 0a20 2020 2020 2020 2076 6572 7469  s].        verti
+0002ac80: 6365 7320 3d20 5b56 6572 7465 782e 6d61  ces = [Vertex.ma
+0002ac90: 6b65 5665 7274 6578 282a 762e 746f 5475  keVertex(*v.toTu
+0002aca0: 706c 6528 2929 2066 6f72 2076 2069 6e20  ple()) for v in 
+0002acb0: 7665 6373 5d0a 2020 2020 2020 2020 6564  vecs].        ed
+0002acc0: 6765 7320 3d20 6530 2e73 706c 6974 282a  ges = e0.split(*
+0002acd0: 7665 7274 6963 6573 292e 4564 6765 7328  vertices).Edges(
+0002ace0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002acf0: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+0002ad00: 6467 6573 292c 206c 656e 2876 6572 7469  dges), len(verti
+0002ad10: 6365 7329 202b 2031 290a 2020 2020 2020  ces) + 1).      
+0002ad20: 2020 656e 6470 6f69 6e74 7320 3d20 5b65    endpoints = [e
+0002ad30: 2e65 6e64 506f 696e 7428 2920 666f 7220  .endPoint() for 
+0002ad40: 6520 696e 2065 6467 6573 5d0a 2020 2020  e in edges].    
+0002ad50: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0002ad60: 7275 6528 616c 6c28 5b76 2069 6e20 656e  rue(all([v in en
+0002ad70: 6470 6f69 6e74 7320 666f 7220 7620 696e  dpoints for v in
+0002ad80: 2076 6563 735d 2929 0a0a 2020 2020 6465   vecs]))..    de
+0002ad90: 6620 7465 7374 4272 6570 496d 706f 7274  f testBrepImport
+0002ada0: 4578 706f 7274 2873 656c 6629 3a0a 0a20  Export(self):.. 
+0002adb0: 2020 2020 2020 2023 2069 6d70 6f72 742f         # import/
+0002adc0: 6578 706f 7274 2074 6f20 6669 6c65 0a20  export to file. 
+0002add0: 2020 2020 2020 2073 203d 2057 6f72 6b70         s = Workp
+0002ade0: 6c61 6e65 2829 2e62 6f78 2831 2c20 312c  lane().box(1, 1,
+0002adf0: 2031 292e 7661 6c28 290a 0a20 2020 2020   1).val()..     
+0002ae00: 2020 2073 2e65 7870 6f72 7442 7265 7028     s.exportBrep(
+0002ae10: 2274 6573 742e 6272 6570 2229 0a20 2020  "test.brep").   
+0002ae20: 2020 2020 2073 6920 3d20 5368 6170 652e       si = Shape.
+0002ae30: 696d 706f 7274 4272 6570 2822 7465 7374  importBrep("test
+0002ae40: 2e62 7265 7022 290a 0a20 2020 2020 2020  .brep")..       
+0002ae50: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0002ae60: 2873 692e 6973 5661 6c69 6428 2929 0a20  (si.isValid()). 
+0002ae70: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002ae80: 7274 416c 6d6f 7374 4571 7561 6c28 7369  rtAlmostEqual(si
+0002ae90: 2e56 6f6c 756d 6528 292c 2031 290a 0a20  .Volume(), 1).. 
+0002aea0: 2020 2020 2020 2023 2069 6d70 6f72 742f         # import/
+0002aeb0: 6578 706f 7274 2074 6f20 4279 7465 7349  export to BytesI
+0002aec0: 4f0a 2020 2020 2020 2020 6672 6f6d 2069  O.        from i
+0002aed0: 6f20 696d 706f 7274 2042 7974 6573 494f  o import BytesIO
+0002aee0: 0a0a 2020 2020 2020 2020 6269 6f20 3d20  ..        bio = 
+0002aef0: 4279 7465 7349 4f28 290a 0a20 2020 2020  BytesIO()..     
+0002af00: 2020 2073 2e65 7870 6f72 7442 7265 7028     s.exportBrep(
+0002af10: 6269 6f29 0a20 2020 2020 2020 2062 696f  bio).        bio
+0002af20: 2e73 6565 6b28 3029 0a0a 2020 2020 2020  .seek(0)..      
+0002af30: 2020 7369 203d 2053 6861 7065 2e69 6d70    si = Shape.imp
+0002af40: 6f72 7442 7265 7028 2274 6573 742e 6272  ortBrep("test.br
+0002af50: 6570 2229 0a0a 2020 2020 2020 2020 7365  ep")..        se
+0002af60: 6c66 2e61 7373 6572 7454 7275 6528 7369  lf.assertTrue(si
+0002af70: 2e69 7356 616c 6964 2829 290a 2020 2020  .isValid()).    
+0002af80: 2020 2020 7365 6c66 2e61 7373 6572 7441      self.assertA
+0002af90: 6c6d 6f73 7445 7175 616c 2873 692e 566f  lmostEqual(si.Vo
+0002afa0: 6c75 6d65 2829 2c20 3129 0a0a 2020 2020  lume(), 1)..    
+0002afb0: 6465 6620 7465 7374 4661 6365 546f 506c  def testFaceToPl
+0002afc0: 6e28 7365 6c66 293a 0a0a 2020 2020 2020  n(self):..      
+0002afd0: 2020 6f72 6967 696e 203d 2028 312c 2032    origin = (1, 2
+0002afe0: 2c20 3329 0a20 2020 2020 2020 206e 6f72  , 3).        nor
+0002aff0: 6d61 6c20 3d20 2831 2c20 312c 2031 290a  mal = (1, 1, 1).
+0002b000: 2020 2020 2020 2020 6630 203d 2046 6163          f0 = Fac
+0002b010: 652e 6d61 6b65 506c 616e 6528 6c65 6e67  e.makePlane(leng
+0002b020: 7468 3d4e 6f6e 652c 2077 6964 7468 3d4e  th=None, width=N
+0002b030: 6f6e 652c 2062 6173 6550 6e74 3d6f 7269  one, basePnt=ori
+0002b040: 6769 6e2c 2064 6972 3d6e 6f72 6d61 6c29  gin, dir=normal)
+0002b050: 0a20 2020 2020 2020 2070 3020 3d20 6630  .        p0 = f0
+0002b060: 2e74 6f50 6c6e 2829 0a0a 2020 2020 2020  .toPln()..      
+0002b070: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0002b080: 6528 5665 6374 6f72 2870 302e 4c6f 6361  e(Vector(p0.Loca
+0002b090: 7469 6f6e 2829 2920 3d3d 2056 6563 746f  tion()) == Vecto
+0002b0a0: 7228 6f72 6967 696e 2929 0a20 2020 2020  r(origin)).     
+0002b0b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0002b0c0: 7565 2856 6563 746f 7228 7030 2e41 7869  ue(Vector(p0.Axi
+0002b0d0: 7328 292e 4469 7265 6374 696f 6e28 2929  s().Direction())
+0002b0e0: 203d 3d20 5665 6374 6f72 286e 6f72 6d61   == Vector(norma
+0002b0f0: 6c29 2e6e 6f72 6d61 6c69 7a65 6428 2929  l).normalized())
+0002b100: 0a0a 2020 2020 2020 2020 6f72 6967 696e  ..        origin
+0002b110: 3120 3d20 2830 2c20 302c 202d 3329 0a20  1 = (0, 0, -3). 
+0002b120: 2020 2020 2020 206e 6f72 6d61 6c31 203d         normal1 =
+0002b130: 2028 2d31 2c20 312c 202d 3129 0a20 2020   (-1, 1, -1).   
+0002b140: 2020 2020 2066 3120 3d20 4661 6365 2e6d       f1 = Face.m
+0002b150: 616b 6550 6c61 6e65 286c 656e 6774 683d  akePlane(length=
+0002b160: 302e 312c 2077 6964 7468 3d31 3030 2c20  0.1, width=100, 
+0002b170: 6261 7365 506e 743d 6f72 6967 696e 312c  basePnt=origin1,
+0002b180: 2064 6972 3d6e 6f72 6d61 6c31 290a 2020   dir=normal1).  
+0002b190: 2020 2020 2020 7031 203d 2066 312e 746f        p1 = f1.to
+0002b1a0: 506c 6e28 290a 0a20 2020 2020 2020 2073  Pln()..        s
+0002b1b0: 656c 662e 6173 7365 7274 5472 7565 2856  elf.assertTrue(V
+0002b1c0: 6563 746f 7228 7031 2e4c 6f63 6174 696f  ector(p1.Locatio
+0002b1d0: 6e28 2929 203d 3d20 5665 6374 6f72 286f  n()) == Vector(o
+0002b1e0: 7269 6769 6e31 2929 0a20 2020 2020 2020  rigin1)).       
+0002b1f0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0002b200: 2856 6563 746f 7228 7031 2e41 7869 7328  (Vector(p1.Axis(
+0002b210: 292e 4469 7265 6374 696f 6e28 2929 203d  ).Direction()) =
+0002b220: 3d20 5665 6374 6f72 286e 6f72 6d61 6c31  = Vector(normal1
+0002b230: 292e 6e6f 726d 616c 697a 6564 2829 290a  ).normalized()).
+0002b240: 0a20 2020 2020 2020 2066 3220 3d20 576f  .        f2 = Wo
+0002b250: 726b 706c 616e 6528 292e 626f 7828 312c  rkplane().box(1,
+0002b260: 2031 2c20 3130 2c20 6365 6e74 6572 6564   1, 10, centered
+0002b270: 3d46 616c 7365 292e 6661 6365 7328 223e  =False).faces(">
+0002b280: 5a22 292e 7661 6c28 290a 2020 2020 2020  Z").val().      
+0002b290: 2020 7032 203d 2066 322e 746f 506c 6e28    p2 = f2.toPln(
+0002b2a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002b2b0: 7373 6572 7454 7275 6528 7032 2e43 6f6e  ssertTrue(p2.Con
+0002b2c0: 7461 696e 7328 6632 2e43 656e 7465 7228  tains(f2.Center(
+0002b2d0: 292e 746f 506e 7428 292c 2030 2e31 2929  ).toPnt(), 0.1))
+0002b2e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0002b2f0: 7365 7274 5472 7565 2856 6563 746f 7228  sertTrue(Vector(
+0002b300: 7032 2e41 7869 7328 292e 4469 7265 6374  p2.Axis().Direct
+0002b310: 696f 6e28 2929 203d 3d20 6632 2e6e 6f72  ion()) == f2.nor
+0002b320: 6d61 6c41 7428 2929 0a0a 2020 2020 6465  malAt())..    de
+0002b330: 6620 7465 7374 4561 6368 706f 696e 7428  f testEachpoint(
+0002b340: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+0002b350: 7231 203d 2028 0a20 2020 2020 2020 2020  r1 = (.         
+0002b360: 2020 2057 6f72 6b70 6c61 6e65 286f 7269     Workplane(ori
+0002b370: 6769 6e3d 2830 2c20 302c 2031 2929 0a20  gin=(0, 0, 1)). 
+0002b380: 2020 2020 2020 2020 2020 202e 6164 6428             .add(
+0002b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b3a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0002b3b0: 2020 2020 2020 2056 6563 746f 7228 292c         Vector(),
+0002b3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b3d0: 2020 2020 204c 6f63 6174 696f 6e28 5665       Location(Ve
+0002b3e0: 6374 6f72 2830 2c20 302c 202d 312c 2929  ctor(0, 0, -1,))
+0002b3f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002b400: 2020 2020 2020 536b 6574 6368 2829 2e72        Sketch().r
+0002b410: 6563 7428 312c 2031 292c 0a20 2020 2020  ect(1, 1),.     
+0002b420: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0002b430: 6163 652e 6d61 6b65 506c 616e 6528 312c  ace.makePlane(1,
+0002b440: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
+0002b450: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0002b460: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0002b470: 202e 6561 6368 706f 696e 7428 6c61 6d62   .eachpoint(lamb
+0002b480: 6461 206c 3a20 4661 6365 2e6d 616b 6550  da l: Face.makeP
+0002b490: 6c61 6e65 2831 2c20 3129 2e6c 6f63 6174  lane(1, 1).locat
+0002b4a0: 6528 6c29 290a 2020 2020 2020 2020 290a  e(l)).        ).
+0002b4b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0002b4c0: 7365 7274 5472 7565 286c 656e 2872 312e  sertTrue(len(r1.
+0002b4d0: 6f62 6a65 6374 7329 203d 3d20 3429 0a0a  objects) == 4)..
+0002b4e0: 2020 2020 2020 2020 666f 7220 7620 696e          for v in
+0002b4f0: 2072 312e 7661 6c73 2829 3a0a 2020 2020   r1.vals():.    
+0002b500: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0002b510: 6572 7454 7570 6c65 416c 6d6f 7374 4571  ertTupleAlmostEq
+0002b520: 7561 6c73 2876 2e43 656e 7465 7228 292e  uals(v.Center().
+0002b530: 746f 5475 706c 6528 292c 2028 302c 2030  toTuple(), (0, 0
+0002b540: 2c20 3029 2c20 3629 0a0a 2020 2020 2020  , 0), 6)..      
+0002b550: 2020 2320 7465 7374 2065 6163 6870 6f69    # test eachpoi
+0002b560: 6e74 2077 6974 6820 636f 6d62 696e 6520  nt with combine 
+0002b570: 3d20 5472 7565 0a20 2020 2020 2020 2062  = True.        b
+0002b580: 6f78 203d 2057 6f72 6b70 6c61 6e65 2829  ox = Workplane()
+0002b590: 2e62 6f78 2832 2c20 312c 2031 292e 7661  .box(2, 1, 1).va
+0002b5a0: 6c28 290a 2020 2020 2020 2020 7265 6620  l().        ref 
+0002b5b0: 3d20 576f 726b 706c 616e 6528 292e 626f  = Workplane().bo
+0002b5c0: 7828 352c 2035 2c20 3529 0a20 2020 2020  x(5, 5, 5).     
+0002b5d0: 2020 2072 203d 2072 6566 2e76 6572 7469     r = ref.verti
+0002b5e0: 6365 7328 292e 6561 6368 706f 696e 7428  ces().eachpoint(
+0002b5f0: 6c61 6d62 6461 206c 6f63 3a20 626f 782e  lambda loc: box.
+0002b600: 6d6f 7665 6428 6c6f 6329 2c20 636f 6d62  moved(loc), comb
+0002b610: 696e 653d 5472 7565 290a 2020 2020 2020  ine=True).      
+0002b620: 2020 7365 6c66 2e61 7373 6572 7447 7265    self.assertGre
+0002b630: 6174 6572 2872 2e76 616c 2829 2e56 6f6c  ater(r.val().Vol
+0002b640: 756d 6528 292c 2072 6566 2e76 616c 2829  ume(), ref.val()
+0002b650: 2e56 6f6c 756d 6528 2929 0a0a 2020 2020  .Volume())..    
+0002b660: 2020 2020 2320 7465 7374 2065 6163 6870      # test eachp
+0002b670: 6f69 6e74 2077 6974 6820 636f 6d62 696e  oint with combin
+0002b680: 6520 3d20 2263 7574 220a 2020 2020 2020  e = "cut".      
+0002b690: 2020 7220 3d20 7265 662e 7665 7274 6963    r = ref.vertic
+0002b6a0: 6573 2829 2e65 6163 6870 6f69 6e74 286c  es().eachpoint(l
+0002b6b0: 616d 6264 6120 6c6f 633a 2062 6f78 2e6d  ambda loc: box.m
+0002b6c0: 6f76 6564 286c 6f63 292c 2063 6f6d 6269  oved(loc), combi
+0002b6d0: 6e65 3d22 6375 7422 290a 2020 2020 2020  ne="cut").      
+0002b6e0: 2020 7365 6c66 2e61 7373 6572 7447 7265    self.assertGre
+0002b6f0: 6174 6572 2872 6566 2e76 616c 2829 2e56  ater(ref.val().V
+0002b700: 6f6c 756d 6528 292c 2072 2e76 616c 2829  olume(), r.val()
+0002b710: 2e56 6f6c 756d 6528 2929 0a0a 2020 2020  .Volume())..    
+0002b720: 6465 6620 7465 7374 536b 6574 6368 2873  def testSketch(s
+0002b730: 656c 6629 3a0a 0a20 2020 2020 2020 2072  elf):..        r
+0002b740: 3120 3d20 280a 2020 2020 2020 2020 2020  1 = (.          
+0002b750: 2020 576f 726b 706c 616e 6528 290a 2020    Workplane().  
+0002b760: 2020 2020 2020 2020 2020 2e62 6f78 2831            .box(1
+0002b770: 302c 2031 302c 2031 290a 2020 2020 2020  0, 10, 1).      
+0002b780: 2020 2020 2020 2e66 6163 6573 2822 3e5a        .faces(">Z
+0002b790: 2229 0a20 2020 2020 2020 2020 2020 202e  ").            .
+0002b7a0: 736b 6574 6368 2829 0a20 2020 2020 2020  sketch().       
+0002b7b0: 2020 2020 202e 736c 6f74 2832 2c20 3129       .slot(2, 1)
+0002b7c0: 0a20 2020 2020 2020 2020 2020 202e 736c  .            .sl
+0002b7d0: 6f74 2832 2c20 312c 2061 6e67 6c65 3d39  ot(2, 1, angle=9
+0002b7e0: 3029 0a20 2020 2020 2020 2020 2020 202e  0).            .
+0002b7f0: 636c 6561 6e28 290a 2020 2020 2020 2020  clean().        
+0002b800: 2020 2020 2e66 696e 616c 697a 6528 290a      .finalize().
+0002b810: 2020 2020 2020 2020 2020 2020 2e65 7874              .ext
+0002b820: 7275 6465 2831 290a 2020 2020 2020 2020  rude(1).        
+0002b830: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0002b840: 6173 7365 7274 5472 7565 2872 312e 7661  assertTrue(r1.va
+0002b850: 6c28 292e 6973 5661 6c69 6428 2929 0a20  l().isValid()). 
+0002b860: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002b870: 7274 4571 7561 6c28 6c65 6e28 7231 2e66  rtEqual(len(r1.f
+0002b880: 6163 6573 2829 2e76 616c 7328 2929 2c20  aces().vals()), 
+0002b890: 3139 290a 0a20 2020 2020 2020 2072 3220  19)..        r2 
+0002b8a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0002b8b0: 576f 726b 706c 616e 6528 290a 2020 2020  Workplane().    
+0002b8c0: 2020 2020 2020 2020 2e73 6b65 7463 6828          .sketch(
+0002b8d0: 290a 2020 2020 2020 2020 2020 2020 2e63  ).            .c
+0002b8e0: 6972 636c 6528 3229 0a20 2020 2020 2020  ircle(2).       
+0002b8f0: 2020 2020 202e 7769 7265 7328 290a 2020       .wires().  
+0002b900: 2020 2020 2020 2020 2020 2e6f 6666 7365            .offse
+0002b910: 7428 302e 312c 206d 6f64 653d 2273 2229  t(0.1, mode="s")
+0002b920: 0a20 2020 2020 2020 2020 2020 202e 6669  .            .fi
+0002b930: 6e61 6c69 7a65 2829 0a20 2020 2020 2020  nalize().       
+0002b940: 2020 2020 202e 736b 6574 6368 2829 0a20       .sketch(). 
+0002b950: 2020 2020 2020 2020 2020 202e 7265 6374             .rect
+0002b960: 2831 2c20 3129 0a20 2020 2020 2020 2020  (1, 1).         
+0002b970: 2020 202e 6669 6e61 6c69 7a65 2829 0a20     .finalize(). 
+0002b980: 2020 2020 2020 2020 2020 202e 6578 7472             .extr
+0002b990: 7564 6528 312c 2074 6170 6572 3d35 290a  ude(1, taper=5).
+0002b9a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0002b9b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0002b9c0: 7565 2872 322e 7661 6c28 292e 6973 5661  ue(r2.val().isVa
+0002b9d0: 6c69 6428 2929 0a20 2020 2020 2020 2073  lid()).        s
+0002b9e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0002b9f0: 6c65 6e28 7232 2e66 6163 6573 2829 2e76  len(r2.faces().v
+0002ba00: 616c 7328 2929 2c20 3629 0a0a 2020 2020  als()), 6)..    
+0002ba10: 2020 2020 7233 203d 2028 0a20 2020 2020      r3 = (.     
+0002ba20: 2020 2020 2020 2057 6f72 6b70 6c61 6e65         Workplane
+0002ba30: 2829 0a20 2020 2020 2020 2020 2020 202e  ().            .
+0002ba40: 7075 7368 506f 696e 7473 2828 4c6f 6361  pushPoints((Loca
+0002ba50: 7469 6f6e 2856 6563 746f 7228 312c 2031  tion(Vector(1, 1
+0002ba60: 2c20 3029 292c 2929 0a20 2020 2020 2020  , 0)),)).       
+0002ba70: 2020 2020 202e 736b 6574 6368 2829 0a20       .sketch(). 
+0002ba80: 2020 2020 2020 2020 2020 202e 6369 7263             .circ
+0002ba90: 6c65 2832 290a 2020 2020 2020 2020 2020  le(2).          
+0002baa0: 2020 2e77 6972 6573 2829 0a20 2020 2020    .wires().     
+0002bab0: 2020 2020 2020 202e 6f66 6673 6574 282d         .offset(-
+0002bac0: 302e 312c 206d 6f64 653d 2273 2229 0a20  0.1, mode="s"). 
+0002bad0: 2020 2020 2020 2020 2020 202e 6669 6e61             .fina
+0002bae0: 6c69 7a65 2829 0a20 2020 2020 2020 2020  lize().         
+0002baf0: 2020 202e 6578 7472 7564 6528 3129 0a20     .extrude(1). 
+0002bb00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0002bb10: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0002bb20: 6528 7233 2e76 616c 2829 2e69 7356 616c  e(r3.val().isVal
+0002bb30: 6964 2829 290a 2020 2020 2020 2020 7365  id()).        se
+0002bb40: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+0002bb50: 656e 2872 332e 6661 6365 7328 292e 7661  en(r3.faces().va
+0002bb60: 6c73 2829 292c 2034 290a 2020 2020 2020  ls()), 4).      
+0002bb70: 2020 7365 6c66 2e61 7373 6572 7454 7570    self.assertTup
+0002bb80: 6c65 416c 6d6f 7374 4571 7561 6c73 2872  leAlmostEquals(r
+0002bb90: 332e 7661 6c28 292e 4365 6e74 6572 2829  3.val().Center()
+0002bba0: 2e74 6f54 7570 6c65 2829 2c20 2831 2c20  .toTuple(), (1, 
+0002bbb0: 312c 2030 2e35 292c 2036 290a 0a20 2020  1, 0.5), 6)..   
+0002bbc0: 2020 2020 2073 203d 2053 6b65 7463 6828       s = Sketch(
+0002bbd0: 292e 7472 6170 657a 6f69 6428 332c 2031  ).trapezoid(3, 1
+0002bbe0: 2c20 3132 3029 0a0a 2020 2020 2020 2020  , 120)..        
+0002bbf0: 7234 203d 2057 6f72 6b70 6c61 6e65 2829  r4 = Workplane()
+0002bc00: 2e70 6c61 6365 536b 6574 6368 2873 2c20  .placeSketch(s, 
+0002bc10: 732e 6d6f 7665 6428 4c6f 6361 7469 6f6e  s.moved(Location
+0002bc20: 2856 6563 746f 7228 302c 2030 2c20 3329  (Vector(0, 0, 3)
+0002bc30: 2929 292e 6c6f 6674 2829 0a0a 2020 2020  ))).loft()..    
+0002bc40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002bc50: 7175 616c 286c 656e 2872 342e 736f 6c69  qual(len(r4.soli
+0002bc60: 6473 2829 2e76 616c 7328 2929 2c20 3129  ds().vals()), 1)
+0002bc70: 0a0a 2020 2020 2020 2020 7235 203d 2028  ..        r5 = (
+0002bc80: 0a20 2020 2020 2020 2020 2020 2057 6f72  .            Wor
+0002bc90: 6b70 6c61 6e65 2829 2e73 6b65 7463 6828  kplane().sketch(
+0002bca0: 292e 706f 6c79 676f 6e28 5b28 302c 2030  ).polygon([(0, 0
+0002bcb0: 292c 2028 302c 2031 292c 2028 312c 2030  ), (0, 1), (1, 0
+0002bcc0: 295d 292e 6669 6e61 6c69 7a65 2829 2e65  )]).finalize().e
+0002bcd0: 7874 7275 6465 2831 290a 2020 2020 2020  xtrude(1).      
+0002bce0: 2020 290a 2020 2020 2020 2020 6173 7365    ).        asse
+0002bcf0: 7274 2072 352e 7661 6c28 292e 566f 6c75  rt r5.val().Volu
+0002bd00: 6d65 2829 203d 3d20 6170 7072 6f78 2830  me() == approx(0
+0002bd10: 2e35 290a 0a20 2020 2064 6566 2074 6573  .5)..    def tes
+0002bd20: 7443 6972 6375 6d73 6372 6962 6564 506f  tCircumscribedPo
+0002bd30: 6c79 676f 6e28 7365 6c66 293a 0a20 2020  lygon(self):.   
+0002bd40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002bd50: 2054 6573 7420 7468 6174 2063 6972 6375   Test that circu
+0002bd60: 6d73 6372 6962 6564 2070 6f6c 7967 6f6e  mscribed polygon
+0002bd70: 7320 7265 7375 6c74 2069 6e20 7468 6520  s result in the 
+0002bd80: 636f 7272 6563 7420 7368 6170 6573 0a20  correct shapes. 
+0002bd90: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0002bda0: 2020 2020 6465 6620 6369 7263 756d 7261      def circumra
+0002bdb0: 6469 7573 286e 2c20 6129 3a0a 2020 2020  dius(n, a):.    
+0002bdc0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0002bdd0: 202f 206d 6174 682e 636f 7328 6d61 7468   / math.cos(math
+0002bde0: 2e70 6920 2f20 6e29 0a0a 2020 2020 2020  .pi / n)..      
+0002bdf0: 2020 6120 3d20 310a 2020 2020 2020 2020    a = 1.        
+0002be00: 2320 5465 7374 2074 7269 616e 676c 650a  # Test triangle.
+0002be10: 2020 2020 2020 2020 7673 203d 2057 6f72          vs = Wor
+0002be20: 6b70 6c61 6e65 2822 5859 2229 2e70 6f6c  kplane("XY").pol
+0002be30: 7967 6f6e 2833 2c20 3220 2a20 612c 2063  ygon(3, 2 * a, c
+0002be40: 6972 6375 6d73 6372 6962 6564 3d54 7275  ircumscribed=Tru
+0002be50: 6529 2e76 6572 7469 6365 7328 292e 7661  e).vertices().va
+0002be60: 6c73 2829 0a20 2020 2020 2020 2073 656c  ls().        sel
+0002be70: 662e 6173 7365 7274 4571 7561 6c28 332c  f.assertEqual(3,
+0002be80: 206c 656e 2876 7329 290a 2020 2020 2020   len(vs)).      
+0002be90: 2020 5220 3d20 6369 7263 756d 7261 6469    R = circumradi
+0002bea0: 7573 2833 2c20 6129 0a20 2020 2020 2020  us(3, a).       
+0002beb0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002bec0: 6c28 0a20 2020 2020 2020 2020 2020 2076  l(.            v
+0002bed0: 735b 305d 2e74 6f54 7570 6c65 2829 2c20  s[0].toTuple(), 
+0002bee0: 6170 7072 6f78 2828 612c 2061 202a 206d  approx((a, a * m
+0002bef0: 6174 682e 7461 6e28 6d61 7468 2e72 6164  ath.tan(math.rad
+0002bf00: 6961 6e73 2836 3029 292c 2030 2929 0a20  ians(60)), 0)). 
+0002bf10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002bf20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002bf30: 6c28 7673 5b31 5d2e 746f 5475 706c 6528  l(vs[1].toTuple(
+0002bf40: 292c 2061 7070 726f 7828 282d 522c 2030  ), approx((-R, 0
+0002bf50: 2c20 3029 2929 0a20 2020 2020 2020 2073  , 0))).        s
+0002bf60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0002bf70: 0a20 2020 2020 2020 2020 2020 2076 735b  .            vs[
+0002bf80: 325d 2e74 6f54 7570 6c65 2829 2c20 6170  2].toTuple(), ap
+0002bf90: 7072 6f78 2828 612c 202d 6120 2a20 6d61  prox((a, -a * ma
+0002bfa0: 7468 2e74 616e 286d 6174 682e 7261 6469  th.tan(math.radi
+0002bfb0: 616e 7328 3630 2929 2c20 3029 290a 2020  ans(60)), 0)).  
+0002bfc0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002bfd0: 2023 2054 6573 7420 7371 7561 7265 0a20   # Test square. 
+0002bfe0: 2020 2020 2020 2076 7320 3d20 576f 726b         vs = Work
+0002bff0: 706c 616e 6528 2258 5922 292e 706f 6c79  plane("XY").poly
+0002c000: 676f 6e28 342c 2032 202a 2061 2c20 6369  gon(4, 2 * a, ci
+0002c010: 7263 756d 7363 7269 6265 643d 5472 7565  rcumscribed=True
+0002c020: 292e 7665 7274 6963 6573 2829 2e76 616c  ).vertices().val
+0002c030: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
+0002c040: 2e61 7373 6572 7445 7175 616c 2834 2c20  .assertEqual(4, 
+0002c050: 6c65 6e28 7673 2929 0a20 2020 2020 2020  len(vs)).       
+0002c060: 2052 203d 2063 6972 6375 6d72 6164 6975   R = circumradiu
+0002c070: 7328 342c 2061 290a 2020 2020 2020 2020  s(4, a).        
+0002c080: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002c090: 280a 2020 2020 2020 2020 2020 2020 7673  (.            vs
+0002c0a0: 5b30 5d2e 746f 5475 706c 6528 292c 2061  [0].toTuple(), a
+0002c0b0: 7070 726f 7828 2861 2c20 6120 2a20 6d61  pprox((a, a * ma
+0002c0c0: 7468 2e74 616e 286d 6174 682e 7261 6469  th.tan(math.radi
+0002c0d0: 616e 7328 3435 2929 2c20 3029 290a 2020  ans(45)), 0)).  
+0002c0e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002c0f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002c100: 280a 2020 2020 2020 2020 2020 2020 7673  (.            vs
+0002c110: 5b31 5d2e 746f 5475 706c 6528 292c 2061  [1].toTuple(), a
+0002c120: 7070 726f 7828 282d 612c 2061 202a 206d  pprox((-a, a * m
+0002c130: 6174 682e 7461 6e28 6d61 7468 2e72 6164  ath.tan(math.rad
+0002c140: 6961 6e73 2834 3529 292c 2030 2929 0a20  ians(45)), 0)). 
+0002c150: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002c160: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002c170: 6c28 0a20 2020 2020 2020 2020 2020 2076  l(.            v
+0002c180: 735b 325d 2e74 6f54 7570 6c65 2829 2c20  s[2].toTuple(), 
+0002c190: 6170 7072 6f78 2828 2d61 2c20 2d61 202a  approx((-a, -a *
+0002c1a0: 206d 6174 682e 7461 6e28 6d61 7468 2e72   math.tan(math.r
+0002c1b0: 6164 6961 6e73 2834 3529 292c 2030 2929  adians(45)), 0))
+0002c1c0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002c1d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002c1e0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+0002c1f0: 2076 735b 335d 2e74 6f54 7570 6c65 2829   vs[3].toTuple()
+0002c200: 2c20 6170 7072 6f78 2828 612c 202d 6120  , approx((a, -a 
+0002c210: 2a20 6d61 7468 2e74 616e 286d 6174 682e  * math.tan(math.
+0002c220: 7261 6469 616e 7328 3435 2929 2c20 3029  radians(45)), 0)
+0002c230: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+0002c240: 2064 6566 2074 6573 745f 636f 6d62 696e   def test_combin
+0002c250: 6557 6974 6842 6173 6528 7365 6c66 293a  eWithBase(self):
+0002c260: 0a20 2020 2020 2020 2023 2054 6573 7420  .        # Test 
+0002c270: 7468 6520 6865 6c70 6572 206d 6568 6f64  the helper mehod
+0002c280: 205f 636f 6d62 696e 6577 6974 680a 0a20   _combinewith.. 
+0002c290: 2020 2020 2020 2062 6f78 203d 2057 6f72         box = Wor
+0002c2a0: 6b70 6c61 6e65 2829 2e62 6f78 2831 302c  kplane().box(10,
+0002c2b0: 2031 302c 2031 3029 0a20 2020 2020 2020   10, 10).       
+0002c2c0: 2073 7068 6572 6520 3d20 626f 782e 6661   sphere = box.fa
+0002c2d0: 6365 7328 223e 5a22 292e 7370 6865 7265  ces(">Z").sphere
+0002c2e0: 2832 290a 2020 2020 2020 2020 6e65 775f  (2).        new_
+0002c2f0: 626f 7820 3d20 626f 782e 5f63 6f6d 6269  box = box._combi
+0002c300: 6e65 5769 7468 4261 7365 2873 7068 6572  neWithBase(spher
+0002c310: 652e 7661 6c28 2929 0a0a 2020 2020 2020  e.val())..      
+0002c320: 2020 7365 6c66 2e61 7373 6572 7447 7265    self.assertGre
+0002c330: 6174 6572 286e 6577 5f62 6f78 2e76 616c  ater(new_box.val
+0002c340: 2829 2e56 6f6c 756d 6528 292c 2062 6f78  ().Volume(), box
+0002c350: 2e76 616c 2829 2e56 6f6c 756d 6528 2929  .val().Volume())
+0002c360: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+0002c370: 7574 4672 6f6d 4261 7365 2873 656c 6629  utFromBase(self)
+0002c380: 3a0a 2020 2020 2020 2020 2320 5465 7374  :.        # Test
+0002c390: 2074 6865 2068 656c 7065 7220 6d65 7468   the helper meth
+0002c3a0: 6f64 205f 6375 7446 726f 6d42 6173 650a  od _cutFromBase.
+0002c3b0: 0a20 2020 2020 2020 2062 6f78 203d 2057  .        box = W
+0002c3c0: 6f72 6b70 6c61 6e65 2829 2e62 6f78 2831  orkplane().box(1
+0002c3d0: 302c 2031 302c 2031 3029 0a20 2020 2020  0, 10, 10).     
+0002c3e0: 2020 2073 7068 6572 6520 3d20 576f 726b     sphere = Work
+0002c3f0: 706c 616e 6528 292e 7370 6865 7265 2832  plane().sphere(2
+0002c400: 290a 2020 2020 2020 2020 686f 6f6c 6f77  ).        hoolow
+0002c410: 5f62 6f78 203d 2062 6f78 2e5f 6375 7446  _box = box._cutF
+0002c420: 726f 6d42 6173 6528 7370 6865 7265 2e76  romBase(sphere.v
+0002c430: 616c 2829 290a 0a20 2020 2020 2020 2073  al())..        s
+0002c440: 656c 662e 6173 7365 7274 4772 6561 7465  elf.assertGreate
+0002c450: 7228 626f 782e 7661 6c28 292e 566f 6c75  r(box.val().Volu
+0002c460: 6d65 2829 2c20 686f 6f6c 6f77 5f62 6f78  me(), hoolow_box
+0002c470: 2e76 616c 2829 2e56 6f6c 756d 6528 2929  .val().Volume())
+0002c480: 0a0a 2020 2020 6465 6620 7465 7374 5f4d  ..    def test_M
+0002c490: 6572 6765 5461 6773 2873 656c 6629 3a0a  ergeTags(self):.
+0002c4a0: 0a20 2020 2020 2020 2061 203d 2057 6f72  .        a = Wor
+0002c4b0: 6b70 6c61 6e65 2829 2e62 6f78 2831 2c20  kplane().box(1, 
+0002c4c0: 312c 2031 290a 2020 2020 2020 2020 6220  1, 1).        b 
+0002c4d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0002c4e0: 576f 726b 706c 616e 6528 6f72 6967 696e  Workplane(origin
+0002c4f0: 3d28 312c 2030 2c20 3029 290a 2020 2020  =(1, 0, 0)).    
+0002c500: 2020 2020 2020 2020 2e62 6f78 2831 2c20          .box(1, 
+0002c510: 312c 2031 290a 2020 2020 2020 2020 2020  1, 1).          
+0002c520: 2020 2e76 6572 7469 6365 7328 223e 5820    .vertices(">X 
+0002c530: 616e 6420 3e59 2061 6e64 203e 5a22 290a  and >Y and >Z").
+0002c540: 2020 2020 2020 2020 2020 2020 2e74 6167              .tag
+0002c550: 2822 626f 785f 7665 7274 6578 2229 0a20  ("box_vertex"). 
+0002c560: 2020 2020 2020 2020 2020 202e 656e 6428             .end(
+0002c570: 3229 0a20 2020 2020 2020 2029 0a20 2020  2).        ).   
+0002c580: 2020 2020 2061 203d 2061 2e61 6464 2862       a = a.add(b
+0002c590: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+0002c5a0: 2061 2e76 6572 7469 6365 7328 7461 673d   a.vertices(tag=
+0002c5b0: 2262 6f78 5f76 6572 7465 7822 292e 7661  "box_vertex").va
+0002c5c0: 6c28 292e 4365 6e74 6572 2829 2e74 6f54  l().Center().toT
+0002c5d0: 7570 6c65 2829 203d 3d20 6170 7072 6f78  uple() == approx
+0002c5e0: 280a 2020 2020 2020 2020 2020 2020 2831  (.            (1
+0002c5f0: 2e35 2c20 302e 352c 2030 2e35 290a 2020  .5, 0.5, 0.5).  
+0002c600: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002c610: 2061 203d 2057 6f72 6b70 6c61 6e65 2829   a = Workplane()
+0002c620: 2e62 6f78 2834 2c20 342c 2034 290a 2020  .box(4, 4, 4).  
+0002c630: 2020 2020 2020 6220 3d20 576f 726b 706c        b = Workpl
+0002c640: 616e 6528 6f72 6967 696e 3d28 302c 2030  ane(origin=(0, 0
+0002c650: 2c20 3129 292e 626f 7828 322c 2032 2c20  , 1)).box(2, 2, 
+0002c660: 3229 2e66 6163 6573 2822 3c5a 2229 2e74  2).faces("<Z").t
+0002c670: 6167 2822 626f 7832 5f66 6163 6522 292e  ag("box2_face").
+0002c680: 656e 6428 290a 2020 2020 2020 2020 6120  end().        a 
+0002c690: 3d20 612e 6375 7428 6229 0a20 2020 2020  = a.cut(b).     
+0002c6a0: 2020 2061 7373 6572 7420 612e 7661 6c28     assert a.val(
+0002c6b0: 292e 566f 6c75 6d65 2829 203d 3d20 6170  ).Volume() == ap
+0002c6c0: 7072 6f78 2834 202a 2a20 3320 2d20 3220  prox(4 ** 3 - 2 
+0002c6d0: 2a2a 2033 290a 2020 2020 2020 2020 6120  ** 3).        a 
+0002c6e0: 3d20 612e 6661 6365 7328 7461 673d 2262  = a.faces(tag="b
+0002c6f0: 6f78 325f 6661 6365 2229 2e77 6972 6573  ox2_face").wires
+0002c700: 2829 2e74 6f50 656e 6469 6e67 2829 2e65  ().toPending().e
+0002c710: 7874 7275 6465 2834 290a 2020 2020 2020  xtrude(4).      
+0002c720: 2020 6173 7365 7274 2061 2e76 616c 2829    assert a.val()
+0002c730: 2e56 6f6c 756d 6528 2920 3d3d 2061 7070  .Volume() == app
+0002c740: 726f 7828 3420 2a2a 2033 202b 2032 202a  rox(4 ** 3 + 2 *
+0002c750: 2a20 3329 0a0a 2020 2020 2020 2020 6120  * 3)..        a 
+0002c760: 3d20 576f 726b 706c 616e 6528 292e 7370  = Workplane().sp
+0002c770: 6865 7265 2832 290a 2020 2020 2020 2020  here(2).        
+0002c780: 6220 3d20 576f 726b 706c 616e 6528 292e  b = Workplane().
+0002c790: 6379 6c69 6e64 6572 2834 2c20 3129 2e74  cylinder(4, 1).t
+0002c7a0: 6167 2822 6379 6c22 290a 2020 2020 2020  ag("cyl").      
+0002c7b0: 2020 6120 3d20 612e 696e 7465 7273 6563    a = a.intersec
+0002c7c0: 7428 6229 0a20 2020 2020 2020 2061 7373  t(b).        ass
+0002c7d0: 6572 7420 6c65 6e28 612e 736f 6c69 6473  ert len(a.solids
+0002c7e0: 2874 6167 3d22 6379 6c22 292e 7661 6c28  (tag="cyl").val(
+0002c7f0: 292e 536f 6c69 6473 2829 2920 3d3d 2031  ).Solids()) == 1
+0002c800: 0a0a 2020 2020 2020 2020 6120 3d20 576f  ..        a = Wo
+0002c810: 726b 706c 616e 6528 292e 626f 7828 342c  rkplane().box(4,
+0002c820: 2034 2c20 3429 0a20 2020 2020 2020 2062   4, 4).        b
+0002c830: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0002c840: 2057 6f72 6b70 6c61 6e65 2829 0a20 2020   Workplane().   
+0002c850: 2020 2020 2020 2020 202e 626f 7828 322c           .box(2,
+0002c860: 2035 2c20 352c 2063 656e 7465 7265 643d   5, 5, centered=
+0002c870: 2846 616c 7365 2c20 5472 7565 2c20 5472  (False, True, Tr
+0002c880: 7565 2929 0a20 2020 2020 2020 2020 2020  ue)).           
+0002c890: 202e 6661 6365 7328 223e 5822 290a 2020   .faces(">X").  
+0002c8a0: 2020 2020 2020 2020 2020 2e77 6f72 6b70            .workp
+0002c8b0: 6c61 6e65 2829 0a20 2020 2020 2020 2020  lane().         
+0002c8c0: 2020 202e 7461 6728 2273 706c 6974 7465     .tag("splitte
+0002c8d0: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
+0002c8e0: 2e65 6e64 2832 290a 2020 2020 2020 2020  .end(2).        
+0002c8f0: 290a 2020 2020 2020 2020 6120 3d20 612e  ).        a = a.
+0002c900: 7370 6c69 7428 6229 0a20 2020 2020 2020  split(b).       
+0002c910: 2061 203d 2061 2e73 6f6c 6964 7328 223c   a = a.solids("<
+0002c920: 5822 290a 2020 2020 2020 2020 6173 7365  X").        asse
+0002c930: 7274 2061 2e76 616c 2829 2e56 6f6c 756d  rt a.val().Volum
+0002c940: 6528 2920 3d3d 2061 7070 726f 7828 2834  e() == approx((4
+0002c950: 202a 2a20 3329 202f 2032 2e30 290a 2020   ** 3) / 2.0).  
+0002c960: 2020 2020 2020 6120 3d20 612e 776f 726b        a = a.work
+0002c970: 706c 616e 6546 726f 6d54 6167 6765 6428  planeFromTagged(
+0002c980: 2273 706c 6974 7465 7222 292e 7265 6374  "splitter").rect
+0002c990: 2834 2c20 3429 2e65 7874 7275 6465 2875  (4, 4).extrude(u
+0002c9a0: 6e74 696c 3d22 6e65 7874 2229 0a20 2020  ntil="next").   
+0002c9b0: 2020 2020 2061 7373 6572 7420 612e 7661       assert a.va
+0002c9c0: 6c28 292e 566f 6c75 6d65 2829 203d 3d20  l().Volume() == 
+0002c9d0: 6170 7072 6f78 2828 3420 2a2a 2033 2929  approx((4 ** 3))
+0002c9e0: 0a0a 2020 2020 2020 2020 6120 3d20 576f  ..        a = Wo
+0002c9f0: 726b 706c 616e 6528 292e 626f 7828 342c  rkplane().box(4,
+0002ca00: 2034 2c20 3429 0a20 2020 2020 2020 2062   4, 4).        b
+0002ca10: 203d 2057 6f72 6b70 6c61 6e65 286f 7269   = Workplane(ori
+0002ca20: 6769 6e3d 2830 2c20 302c 2033 2929 2e62  gin=(0, 0, 3)).b
+0002ca30: 6f78 2832 2c20 322c 2032 292e 6661 6365  ox(2, 2, 2).face
+0002ca40: 7328 223e 5a22 292e 7461 6728 2262 6f78  s(">Z").tag("box
+0002ca50: 325f 6661 6365 2229 2e65 6e64 2829 0a20  2_face").end(). 
+0002ca60: 2020 2020 2020 2061 203d 2061 2e75 6e69         a = a.uni
+0002ca70: 6f6e 2862 290a 2020 2020 2020 2020 6120  on(b).        a 
+0002ca80: 3d20 612e 6661 6365 7328 7461 673d 2262  = a.faces(tag="b
+0002ca90: 6f78 325f 6661 6365 2229 2e77 6f72 6b70  ox2_face").workp
+0002caa0: 6c61 6e65 286f 6666 7365 743d 302e 3529  lane(offset=0.5)
+0002cab0: 2e62 6f78 2831 2c20 312c 2031 290a 2020  .box(1, 1, 1).  
+0002cac0: 2020 2020 2020 6173 7365 7274 2061 2e76        assert a.v
+0002cad0: 616c 2829 2e56 6f6c 756d 6528 2920 3d3d  al().Volume() ==
+0002cae0: 2061 7070 726f 7828 3420 2a2a 2033 202b   approx(4 ** 3 +
+0002caf0: 2032 202a 2a20 3320 2b20 3129 0a0a 2020   2 ** 3 + 1)..  
+0002cb00: 2020 2020 2020 2320 7461 6720 6e61 6d65        # tag name
+0002cb10: 2063 6f6e 666c 6963 743b 206b 6565 7020   conflict; keep 
+0002cb20: 7461 6720 6672 6f6d 206c 6566 7420 7369  tag from left si
+0002cb30: 6465 206f 6620 626f 6f6c 6561 6e0a 2020  de of boolean.  
+0002cb40: 2020 2020 2020 6120 3d20 576f 726b 706c        a = Workpl
+0002cb50: 616e 6528 292e 626f 7828 312c 2031 2c20  ane().box(1, 1, 
+0002cb60: 3129 2e66 6163 6573 2822 3e5a 2229 2e77  1).faces(">Z").w
+0002cb70: 6f72 6b70 6c61 6e65 2829 2e74 6167 2822  orkplane().tag("
+0002cb80: 7a66 6163 6522 292e 656e 6428 3229 0a20  zface").end(2). 
+0002cb90: 2020 2020 2020 2062 203d 2028 0a20 2020         b = (.   
+0002cba0: 2020 2020 2020 2020 2057 6f72 6b70 6c61           Workpla
+0002cbb0: 6e65 286f 7269 6769 6e3d 2831 2c20 302c  ne(origin=(1, 0,
+0002cbc0: 2030 2929 0a20 2020 2020 2020 2020 2020   0)).           
+0002cbd0: 202e 626f 7828 312c 2031 2c20 3229 0a20   .box(1, 1, 2). 
+0002cbe0: 2020 2020 2020 2020 2020 202e 6661 6365             .face
+0002cbf0: 7328 223e 5a22 290a 2020 2020 2020 2020  s(">Z").        
+0002cc00: 2020 2020 2e77 6f72 6b70 6c61 6e65 2829      .workplane()
+0002cc10: 0a20 2020 2020 2020 2020 2020 202e 7461  .            .ta
+0002cc20: 6728 227a 6661 6365 2229 0a20 2020 2020  g("zface").     
+0002cc30: 2020 2020 2020 202e 656e 6428 3229 0a20         .end(2). 
+0002cc40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002cc50: 2061 203d 2061 2e75 6e69 6f6e 2862 290a   a = a.union(b).
+0002cc60: 2020 2020 2020 2020 6120 3d20 612e 776f          a = a.wo
+0002cc70: 726b 706c 616e 6546 726f 6d54 6167 6765  rkplaneFromTagge
+0002cc80: 6428 227a 6661 6365 2229 2e63 6972 636c  d("zface").circl
+0002cc90: 6528 302e 3229 0a20 2020 2020 2020 2061  e(0.2).        a
+0002cca0: 7373 6572 7420 612e 6564 6765 7328 2225  ssert a.edges("%
+0002ccb0: 4349 5243 4c45 2229 2e76 616c 2829 2e43  CIRCLE").val().C
+0002ccc0: 656e 7465 7228 292e 746f 5475 706c 6528  enter().toTuple(
+0002ccd0: 2920 3d3d 2061 7070 726f 7828 2830 2c20  ) == approx((0, 
+0002cce0: 302c 2030 2e35 2929 0a0a 2020 2020 6465  0, 0.5))..    de
+0002ccf0: 6620 7465 7374 5f70 6c61 6e65 5f72 6570  f test_plane_rep
+0002cd00: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+0002cd10: 2077 7020 3d20 576f 726b 706c 616e 6528   wp = Workplane(
+0002cd20: 2258 5922 290a 2020 2020 2020 2020 6173  "XY").        as
+0002cd30: 7365 7274 2028 0a20 2020 2020 2020 2020  sert (.         
+0002cd40: 2020 2072 6570 7228 7770 2e70 6c61 6e65     repr(wp.plane
+0002cd50: 290a 2020 2020 2020 2020 2020 2020 3d3d  ).            ==
+0002cd60: 2022 506c 616e 6528 6f72 6967 696e 3d28   "Plane(origin=(
+0002cd70: 302e 302c 2030 2e30 2c20 302e 3029 2c20  0.0, 0.0, 0.0), 
+0002cd80: 7844 6972 3d28 312e 302c 2030 2e30 2c20  xDir=(1.0, 0.0, 
+0002cd90: 302e 3029 2c20 6e6f 726d 616c 3d28 302e  0.0), normal=(0.
+0002cda0: 302c 2030 2e30 2c20 312e 3029 2922 0a20  0, 0.0, 1.0))". 
+0002cdb0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+0002cdc0: 6620 7465 7374 5f64 6973 7461 6e63 6528  f test_distance(
+0002cdd0: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+0002cde0: 7731 203d 2046 6163 652e 6d61 6b65 506c  w1 = Face.makePl
+0002cdf0: 616e 6528 322c 2032 292e 5769 7265 7328  ane(2, 2).Wires(
+0002ce00: 295b 305d 0a20 2020 2020 2020 2077 3220  )[0].        w2 
+0002ce10: 3d20 4661 6365 2e6d 616b 6550 6c61 6e65  = Face.makePlane
+0002ce20: 2831 2c20 3129 2e57 6972 6573 2829 5b30  (1, 1).Wires()[0
+0002ce30: 5d0a 2020 2020 2020 2020 7733 203d 2046  ].        w3 = F
+0002ce40: 6163 652e 6d61 6b65 506c 616e 6528 332c  ace.makePlane(3,
+0002ce50: 2033 292e 5769 7265 7328 295b 305d 0a0a   3).Wires()[0]..
+0002ce60: 2020 2020 2020 2020 6431 3220 3d20 7731          d12 = w1
+0002ce70: 2e64 6973 7461 6e63 6528 7732 290a 0a20  .distance(w2).. 
+0002ce80: 2020 2020 2020 2061 7373 6572 7420 6431         assert d1
+0002ce90: 3220 3d3d 2061 7070 726f 7828 302e 3529  2 == approx(0.5)
+0002cea0: 0a0a 2020 2020 2020 2020 6431 322c 2064  ..        d12, d
+0002ceb0: 3133 203d 2077 312e 6469 7374 616e 6365  13 = w1.distance
+0002cec0: 7328 7732 2c20 7733 290a 0a20 2020 2020  s(w2, w3)..     
+0002ced0: 2020 2061 7373 6572 7420 6431 3220 3d3d     assert d12 ==
+0002cee0: 2061 7070 726f 7828 302e 3529 0a20 2020   approx(0.5).   
+0002cef0: 2020 2020 2061 7373 6572 7420 6431 3320       assert d13 
+0002cf00: 3d3d 2061 7070 726f 7828 302e 3529 0a0a  == approx(0.5)..
+0002cf10: 2020 2020 6465 6620 7465 7374 5f70 726f      def test_pro
+0002cf20: 6a65 6374 2873 656c 6629 3a0a 0a20 2020  ject(self):..   
+0002cf30: 2020 2020 2023 2070 726f 6a65 6374 2061       # project a
+0002cf40: 2073 696e 676c 6520 6c65 7474 6572 0a20   single letter. 
+0002cf50: 2020 2020 2020 2074 203d 2043 6f6d 706f         t = Compo
+0002cf60: 756e 642e 6d61 6b65 5465 7874 2822 5422  und.makeText("T"
+0002cf70: 2c20 352c 2030 292e 4661 6365 7328 295b  , 5, 0).Faces()[
+0002cf80: 305d 0a20 2020 2020 2020 2066 203d 2057  0].        f = W
+0002cf90: 6f72 6b70 6c61 6e65 2822 585a 222c 206f  orkplane("XZ", o
+0002cfa0: 7269 6769 6e3d 2830 2c20 302c 202d 3729  rigin=(0, 0, -7)
+0002cfb0: 292e 7370 6865 7265 2836 292e 6661 6365  ).sphere(6).face
+0002cfc0: 7328 226e 6f74 2025 504c 414e 4522 292e  s("not %PLANE").
+0002cfd0: 7661 6c28 290a 0a20 2020 2020 2020 2072  val()..        r
+0002cfe0: 6573 203d 2074 2e70 726f 6a65 6374 2866  es = t.project(f
+0002cff0: 2c20 2830 2c20 302c 2031 2929 0a0a 2020  , (0, 0, 1))..  
+0002d000: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+0002d010: 2e69 7356 616c 6964 2829 0a20 2020 2020  .isValid().     
+0002d020: 2020 2061 7373 6572 7420 6c65 6e28 7265     assert len(re
+0002d030: 732e 4564 6765 7328 2929 203d 3d20 6c65  s.Edges()) == le
+0002d040: 6e28 742e 4564 6765 7328 2929 0a20 2020  n(t.Edges()).   
+0002d050: 2020 2020 2061 7373 6572 7420 742e 6469       assert t.di
+0002d060: 7374 616e 6365 2872 6573 2920 3d3d 2061  stance(res) == a
+0002d070: 7070 726f 7828 3129 0a0a 2020 2020 2020  pprox(1)..      
+0002d080: 2020 2320 6578 7472 7564 6520 6974 0a20    # extrude it. 
+0002d090: 2020 2020 2020 2072 6573 5f65 7820 3d20         res_ex = 
+0002d0a0: 536f 6c69 642e 6578 7472 7564 654c 696e  Solid.extrudeLin
+0002d0b0: 6561 7228 742e 7072 6f6a 6563 7428 662c  ear(t.project(f,
+0002d0c0: 2028 302c 2030 2c20 2d31 2929 2c20 2830   (0, 0, -1)), (0
+0002d0d0: 2e30 2c20 302e 302c 2030 2e35 2929 0a0a  .0, 0.0, 0.5))..
+0002d0e0: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
+0002d0f0: 6573 5f65 782e 6973 5661 6c69 6428 290a  es_ex.isValid().
+0002d100: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+0002d110: 656e 2872 6573 5f65 782e 4661 6365 7328  en(res_ex.Faces(
+0002d120: 2929 203d 3d20 3130 0a0a 2020 2020 2020  )) == 10..      
+0002d130: 2020 2320 7072 6f6a 6563 7420 6120 7769    # project a wi
+0002d140: 7265 0a20 2020 2020 2020 2077 203d 2074  re.        w = t
+0002d150: 2e6f 7574 6572 5769 7265 2829 0a0a 2020  .outerWire()..  
+0002d160: 2020 2020 2020 7265 735f 7720 3d20 772e        res_w = w.
+0002d170: 7072 6f6a 6563 7428 662c 2028 302c 2030  project(f, (0, 0
+0002d180: 2c20 3129 290a 0a20 2020 2020 2020 2061  , 1))..        a
+0002d190: 7373 6572 7420 6c65 6e28 7265 735f 772e  ssert len(res_w.
+0002d1a0: 4564 6765 7328 2929 203d 3d20 380a 2020  Edges()) == 8.  
+0002d1b0: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+0002d1c0: 5f77 2e69 7356 616c 6964 2829 0a0a 2020  _w.isValid()..  
+0002d1d0: 2020 2020 2020 7265 735f 7731 2c20 7265        res_w1, re
+0002d1e0: 735f 7732 203d 2077 2e70 726f 6a65 6374  s_w2 = w.project
+0002d1f0: 2866 2c20 2830 2c20 302c 2031 292c 2046  (f, (0, 0, 1), F
+0002d200: 616c 7365 290a 0a20 2020 2020 2020 2061  alse)..        a
+0002d210: 7373 6572 7420 6c65 6e28 7265 735f 7731  ssert len(res_w1
+0002d220: 2e45 6467 6573 2829 2920 3d3d 2038 0a20  .Edges()) == 8. 
+0002d230: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
+0002d240: 6e28 7265 735f 7732 2e45 6467 6573 2829  n(res_w2.Edges()
+0002d250: 2920 3d3d 2038 0a0a 2020 2020 2020 2020  ) == 8..        
+0002d260: 2320 7072 6f6a 6563 7420 6120 7369 6e67  # project a sing
+0002d270: 6c65 206c 6574 7465 7220 7769 7468 206f  le letter with o
+0002d280: 7065 6e69 6e67 730a 2020 2020 2020 2020  penings.        
+0002d290: 6f20 3d20 436f 6d70 6f75 6e64 2e6d 616b  o = Compound.mak
+0002d2a0: 6554 6578 7428 224f 222c 2035 2c20 3029  eText("O", 5, 0)
+0002d2b0: 2e46 6163 6573 2829 5b30 5d0a 2020 2020  .Faces()[0].    
+0002d2c0: 2020 2020 6620 3d20 576f 726b 706c 616e      f = Workplan
+0002d2d0: 6528 2258 5a22 2c20 6f72 6967 696e 3d28  e("XZ", origin=(
+0002d2e0: 302c 2030 2c20 2d37 2929 2e73 7068 6572  0, 0, -7)).spher
+0002d2f0: 6528 3629 2e66 6163 6573 2822 6e6f 7420  e(6).faces("not 
+0002d300: 2550 4c41 4e45 2229 2e76 616c 2829 0a0a  %PLANE").val()..
+0002d310: 2020 2020 2020 2020 7265 735f 6f20 3d20          res_o = 
+0002d320: 6f2e 7072 6f6a 6563 7428 662c 2028 302c  o.project(f, (0,
+0002d330: 2030 2c20 3129 290a 0a20 2020 2020 2020   0, 1))..       
+0002d340: 2061 7373 6572 7420 7265 735f 6f2e 6973   assert res_o.is
+0002d350: 5661 6c69 6428 290a 0a20 2020 2020 2020  Valid()..       
+0002d360: 2023 2065 7874 7275 6465 2069 740a 2020   # extrude it.  
+0002d370: 2020 2020 2020 7265 735f 6f5f 6578 203d        res_o_ex =
+0002d380: 2053 6f6c 6964 2e65 7874 7275 6465 4c69   Solid.extrudeLi
+0002d390: 6e65 6172 286f 2e70 726f 6a65 6374 2866  near(o.project(f
+0002d3a0: 2c20 2830 2c20 302c 202d 3129 292c 2028  , (0, 0, -1)), (
+0002d3b0: 302e 302c 2030 2e30 2c20 302e 3529 290a  0.0, 0.0, 0.5)).
+0002d3c0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0002d3d0: 7265 735f 6f5f 6578 2e69 7356 616c 6964  res_o_ex.isValid
+0002d3e0: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
+0002d3f0: 5f6d 616b 654e 5369 6465 6453 7572 6661  _makeNSidedSurfa
+0002d400: 6365 2873 656c 6629 3a0a 0a20 2020 2020  ce(self):..     
+0002d410: 2020 2023 2069 6e6e 6572 2065 6467 652f     # inner edge/
+0002d420: 7769 7265 2063 6f6e 7374 7261 696e 740a  wire constraint.
+0002d430: 2020 2020 2020 2020 6f75 7465 725f 7720          outer_w 
+0002d440: 3d20 576f 726b 706c 616e 6528 292e 736c  = Workplane().sl
+0002d450: 6f74 3244 2832 2c20 3129 2e77 6972 6573  ot2D(2, 1).wires
+0002d460: 2829 2e76 616c 7328 290a 0a20 2020 2020  ().vals()..     
+0002d470: 2020 2069 6e6e 6572 5f65 3120 3d20 280a     inner_e1 = (.
+0002d480: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+0002d490: 706c 616e 6528 6f72 6967 696e 3d28 302c  plane(origin=(0,
+0002d4a0: 2030 2c20 3129 292e 6d6f 7665 546f 282d   0, 1)).moveTo(-
+0002d4b0: 302e 352c 2030 292e 6c69 6e65 546f 2830  0.5, 0).lineTo(0
+0002d4c0: 2e35 2c20 302e 3029 2e65 6467 6573 2829  .5, 0.0).edges()
+0002d4d0: 2e76 616c 7328 290a 2020 2020 2020 2020  .vals().        
+0002d4e0: 290a 2020 2020 2020 2020 696e 6e65 725f  ).        inner_
+0002d4f0: 6532 203d 2028 0a20 2020 2020 2020 2020  e2 = (.         
+0002d500: 2020 2057 6f72 6b70 6c61 6e65 286f 7269     Workplane(ori
+0002d510: 6769 6e3d 2830 2c20 302c 2031 2929 2e6d  gin=(0, 0, 1)).m
+0002d520: 6f76 6554 6f28 302c 202d 302e 3229 2e6c  oveTo(0, -0.2).l
+0002d530: 696e 6554 6f28 302c 2030 2e32 292e 6564  ineTo(0, 0.2).ed
+0002d540: 6765 7328 292e 7661 6c73 2829 0a20 2020  ges().vals().   
+0002d550: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+0002d560: 6e6e 6572 5f77 203d 2057 6f72 6b70 6c61  nner_w = Workpla
+0002d570: 6e65 286f 7269 6769 6e3d 2830 2c20 302c  ne(origin=(0, 0,
+0002d580: 2031 2929 2e65 6c6c 6970 7365 2830 2e35   1)).ellipse(0.5
+0002d590: 2c20 302e 3229 2e76 616c 7328 290a 0a20  , 0.2).vals().. 
+0002d5a0: 2020 2020 2020 2066 3120 3d20 4661 6365         f1 = Face
+0002d5b0: 2e6d 616b 654e 5369 6465 6453 7572 6661  .makeNSidedSurfa
+0002d5c0: 6365 286f 7574 6572 5f77 2c20 696e 6e65  ce(outer_w, inne
+0002d5d0: 725f 6531 202b 2069 6e6e 6572 5f65 3220  r_e1 + inner_e2 
+0002d5e0: 2b20 696e 6e65 725f 7729 0a0a 2020 2020  + inner_w)..    
+0002d5f0: 2020 2020 6173 7365 7274 2066 312e 6973      assert f1.is
+0002d600: 5661 6c69 6428 290a 2020 2020 2020 2020  Valid().        
+0002d610: 6173 7365 7274 206c 656e 2866 312e 4564  assert len(f1.Ed
+0002d620: 6765 7328 2929 203d 3d20 340a 0a20 2020  ges()) == 4..   
+0002d630: 2020 2020 2023 2069 6e6e 6572 2070 6f69       # inner poi
+0002d640: 6e74 730a 2020 2020 2020 2020 6632 203d  nts.        f2 =
+0002d650: 2046 6163 652e 6d61 6b65 4e53 6964 6564   Face.makeNSided
+0002d660: 5375 7266 6163 6528 0a20 2020 2020 2020  Surface(.       
+0002d670: 2020 2020 206f 7574 6572 5f77 2c20 5b56       outer_w, [V
+0002d680: 6563 746f 7228 2d30 2e34 2c20 302c 2031  ector(-0.4, 0, 1
+0002d690: 292e 746f 506e 7428 292c 2056 6563 746f  ).toPnt(), Vecto
+0002d6a0: 7228 302e 342c 2030 2c20 3129 5d0a 2020  r(0.4, 0, 1)].  
+0002d6b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002d6c0: 2061 7373 6572 7420 6632 2e69 7356 616c   assert f2.isVal
+0002d6d0: 6964 2829 0a20 2020 2020 2020 2061 7373  id().        ass
+0002d6e0: 6572 7420 6c65 6e28 6632 2e45 6467 6573  ert len(f2.Edges
+0002d6f0: 2829 2920 3d3d 2034 0a0a 2020 2020 2020  ()) == 4..      
+0002d700: 2020 2320 6578 6365 7074 696f 6e20 6f6e    # exception on
+0002d710: 2069 6e76 616c 6964 2063 6f6e 7374 7261   invalid constra
+0002d720: 696e 740a 2020 2020 2020 2020 7769 7468  int.        with
+0002d730: 2072 6169 7365 7328 5661 6c75 6545 7272   raises(ValueErr
+0002d740: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0002d750: 2046 6163 652e 6d61 6b65 4e53 6964 6564   Face.makeNSided
+0002d760: 5375 7266 6163 6528 6f75 7465 725f 772c  Surface(outer_w,
+0002d770: 205b 5b30 2c20 302c 2031 5d5d 290a 0a20   [[0, 0, 1]]).. 
+0002d780: 2020 2064 6566 2074 6573 745f 746f 5674     def test_toVt
+0002d790: 6b28 7365 6c66 293a 0a0a 2020 2020 2020  k(self):..      
+0002d7a0: 2020 6672 6f6d 2076 746b 6d6f 6475 6c65    from vtkmodule
+0002d7b0: 732e 7674 6b43 6f6d 6d6f 6e44 6174 614d  s.vtkCommonDataM
+0002d7c0: 6f64 656c 2069 6d70 6f72 7420 7674 6b50  odel import vtkP
+0002d7d0: 6f6c 7944 6174 610a 0a20 2020 2020 2020  olyData..       
+0002d7e0: 2066 203d 2046 6163 652e 6d61 6b65 506c   f = Face.makePl
+0002d7f0: 616e 6528 322c 2032 290a 2020 2020 2020  ane(2, 2).      
+0002d800: 2020 7674 6b20 3d20 662e 746f 5674 6b50    vtk = f.toVtkP
+0002d810: 6f6c 7944 6174 6128 6e6f 726d 616c 733d  olyData(normals=
+0002d820: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0002d830: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+0002d840: 6528 7674 6b2c 2076 746b 506f 6c79 4461  e(vtk, vtkPolyDa
+0002d850: 7461 290a 2020 2020 2020 2020 6173 7365  ta).        asse
+0002d860: 7274 2076 746b 2e47 6574 4e75 6d62 6572  rt vtk.GetNumber
+0002d870: 4f66 506f 6c79 7328 2920 3d3d 2032 0a    OfPolys() == 2.
```

### Comparing `cadquery-2.2.0b2/tests/test_cqgi.py` & `cadquery-2.3.0/tests/test_cqgi.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_examples.py` & `cadquery-2.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_hull.py` & `cadquery-2.3.0/tests/test_hull.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_importers.py` & `cadquery-2.3.0/tests/test_importers.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_jupyter.py` & `cadquery-2.3.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_selectors.py` & `cadquery-2.3.0/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_sketch.py` & `cadquery-2.3.0/tests/test_sketch.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
 
     assert (seg1.endPoint() - seg1.startPoint()).getAngle(Vector(-1, -1)) == approx(
         0, abs=1e-9
     )
 
     midpoint = (seg2.startPoint() + seg2.endPoint()) / 2
 
-    (midpoint - seg1.startPoint()).Length == approx(2)
+    assert (midpoint - seg1.startPoint()).Length == approx(2)
 
     s5 = (
         Sketch()
         .segment((0, 0), (0, 3.0), "s1")
         .arc((0.0, 0), (1.5, 1.5), (0.0, 3), "a1")
         .arc((0.0, 0), (-1.0, 1.5), (0.0, 3), "a2")
     )
```

### Comparing `cadquery-2.2.0b2/tests/test_utils.py` & `cadquery-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/test_workplanes.py` & `cadquery-2.3.0/tests/test_workplanes.py`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/1001.dxf` & `cadquery-2.3.0/tests/testdata/1001.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/MC 12x31.dxf` & `cadquery-2.3.0/tests/testdata/MC 12x31.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/OpenSans-Regular.ttf` & `cadquery-2.3.0/tests/testdata/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/gear.dxf` & `cadquery-2.3.0/tests/testdata/gear.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/genshi.dxf` & `cadquery-2.3.0/tests/testdata/genshi.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/rational_spline.dxf` & `cadquery-2.3.0/tests/testdata/rational_spline.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/red_cube_blue_cylinder.step` & `cadquery-2.3.0/tests/testdata/red_cube_blue_cylinder.step`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/spline.dxf` & `cadquery-2.3.0/tests/testdata/spline.dxf`

 * *Files identical despite different names*

### Comparing `cadquery-2.2.0b2/tests/testdata/three_layers.dxf` & `cadquery-2.3.0/tests/testdata/three_layers.dxf`

 * *Files identical despite different names*

