# Comparing `tmp/plone.distribution-1.0.0a8.tar.gz` & `tmp/plone.distribution-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0a8.tar", last modified: Sun Jun 25 22:37:54 2023, max compression
+gzip compressed data, was "plone.distribution-1.0.0a9.tar", last modified: Tue Jun 27 19:16:34 2023, max compression
```

## Comparing `plone.distribution-1.0.0a8.tar` & `plone.distribution-1.0.0a9.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.528499 plone.distribution-1.0.0a8/
--rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      540 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/.flake8
--rw-r--r--   0 ericof     (501) staff       (20)      663 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)      557 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/.meta.toml
--rw-r--r--   0 ericof     (501) staff       (20)     1740 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/.pre-commit-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)     2102 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      269 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     5109 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     9948 2023-06-25 22:37:54.528329 plone.distribution-1.0.0a8/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/constraints.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.515687 plone.distribution-1.0.0a8/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/Makefile
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.516141 plone.distribution-1.0.0a8/docs/_static/
--rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/_static/favicon.ico
--rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/_static/logo.svg
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/_static/print.css
--rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/_static/styles.css
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.516483 plone.distribution-1.0.0a8/docs/api/
--rw-r--r--   0 ericof     (501) staff       (20)      469 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/api/distribution.md
--rw-r--r--   0 ericof     (501) staff       (20)      709 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/api/index.md
--rw-r--r--   0 ericof     (501) staff       (20)      439 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/api/site.md
--rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/conf.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.516608 plone.distribution-1.0.0a8/docs/development/
--rw-r--r--   0 ericof     (501) staff       (20)       26 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/development/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/index.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.517071 plone.distribution-1.0.0a8/docs/usage/
--rw-r--r--   0 ericof     (501) staff       (20)     2560 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/usage/code-examples.md
--rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/usage/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/docs/usage/package-structure.md
--rw-r--r--   0 ericof     (501) staff       (20)      172 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      577 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)     4112 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      393 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/requirements-docs.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-25 22:37:54.528537 plone.distribution-1.0.0a8/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.511497 plone.distribution-1.0.0a8/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.517199 plone.distribution-1.0.0a8/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.519269 plone.distribution-1.0.0a8/src/plone/distribution/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.519610 plone.distribution-1.0.0a8/src/plone/distribution/api/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/api/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/api/distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     5231 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/api/site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.520191 plone.distribution-1.0.0a8/src/plone/distribution/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/admin.py
--rw-r--r--   0 ericof     (501) staff       (20)      970 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/image.py
--rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.520985 plone.distribution-1.0.0a8/src/plone/distribution/browser/static/
--rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 ericof     (501) staff       (20)   543232 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 ericof     (501) staff       (20)      812 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.521108 plone.distribution-1.0.0a8/src/plone/distribution/browser/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1431 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 ericof     (501) staff       (20)      446 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3618 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/core.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.512093 plone.distribution-1.0.0a8/src/plone/distribution/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.521654 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.522320 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/content.json
--rw-r--r--   0 ericof     (501) staff       (20)      336 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/defaultpages.json
--rw-r--r--   0 ericof     (501) staff       (20)      257 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)      613 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.522829 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.522967 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/content/
--rw-r--r--   0 ericof     (501) staff       (20)    25846 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      175 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      491 2023-06-25 22:37:53.000000 plone.distribution-1.0.0a8/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.523820 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1266 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4276 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/dist_export.py
--rw-r--r--   0 ericof     (501) staff       (20)     3054 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/dist_import.py
--rw-r--r--   0 ericof     (501) staff       (20)     2486 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)      241 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.524059 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     2290 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1371 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1334 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)      391 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/meta.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/metaconfigure.py
--rw-r--r--   0 ericof     (501) staff       (20)     4174 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/registry.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.524303 plone.distribution-1.0.0a8/src/plone/distribution/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.524633 plone.distribution-1.0.0a8/src/plone/distribution/services/auth/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      348 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.525094 plone.distribution-1.0.0a8/src/plone/distribution/services/sites/
--rw-r--r--   0 ericof     (501) staff       (20)       77 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 ericof     (501) staff       (20)      895 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/services/sites/get.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.525438 plone.distribution-1.0.0a8/src/plone/distribution/testing/
--rw-r--r--   0 ericof     (501) staff       (20)      149 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/testing/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     3123 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/testing/layer.py
--rw-r--r--   0 ericof     (501) staff       (20)     1017 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/testing/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.525790 plone.distribution-1.0.0a8/src/plone/distribution/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      914 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/utils/request.py
--rw-r--r--   0 ericof     (501) staff       (20)     4402 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone/distribution/utils/schema.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.518200 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     9948 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     4348 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      208 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.526043 plone.distribution-1.0.0a8/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.526309 plone.distribution-1.0.0a8/tests/api/
--rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/api/test_api_distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     2166 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/api/test_api_site.py
--rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.526804 plone.distribution-1.0.0a8/tests/distributions/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/distributions/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      322 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/distributions/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     1895 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/distributions/test_distributions_classic.py
--rw-r--r--   0 ericof     (501) staff       (20)     1765 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/distributions/test_distributions_default.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.527072 plone.distribution-1.0.0a8/tests/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)    12736 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/exportimport/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/exportimport/test_exportimport_helpers.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.527439 plone.distribution-1.0.0a8/tests/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/services/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      243 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/services/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/services/test_services_site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.527832 plone.distribution-1.0.0a8/tests/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/utils/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-25 22:37:54.528089 plone.distribution-1.0.0a8/tests/utils/data/
--rw-r--r--   0 ericof     (501) staff       (20)      969 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/utils/data/invalid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/utils/data/valid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1205 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/utils/test_utils_request.py
--rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tests/utils/test_utils_schema.py
--rw-r--r--   0 ericof     (501) staff       (20)     3740 2023-06-25 22:37:54.000000 plone.distribution-1.0.0a8/tox.ini
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.137769 plone.distribution-1.0.0a9/
+-rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      540 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/.flake8
+-rw-r--r--   0 ericof     (501) staff       (20)      663 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)      557 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/.meta.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     1740 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     2209 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      269 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5109 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)    10055 2023-06-27 19:16:34.137595 plone.distribution-1.0.0a9/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/constraints.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.124835 plone.distribution-1.0.0a9/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.125349 plone.distribution-1.0.0a9/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/_static/styles.css
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.125732 plone.distribution-1.0.0a9/docs/api/
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/api/distribution.md
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/api/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)      439 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/api/site.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/conf.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.125844 plone.distribution-1.0.0a9/docs/development/
+-rw-r--r--   0 ericof     (501) staff       (20)       26 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/development/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/index.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.126211 plone.distribution-1.0.0a9/docs/usage/
+-rw-r--r--   0 ericof     (501) staff       (20)     2560 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/usage/code-examples.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/usage/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/docs/usage/package-structure.md
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      577 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     4112 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-27 19:16:34.137804 plone.distribution-1.0.0a9/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.120612 plone.distribution-1.0.0a9/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.126332 plone.distribution-1.0.0a9/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.128403 plone.distribution-1.0.0a9/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.128737 plone.distribution-1.0.0a9/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5231 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.129364 plone.distribution-1.0.0a9/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.130158 plone.distribution-1.0.0a9/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   543232 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.130299 plone.distribution-1.0.0a9/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1431 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 ericof     (501) staff       (20)      446 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3618 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.121170 plone.distribution-1.0.0a9/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.130816 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.131445 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      336 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/defaultpages.json
+-rw-r--r--   0 ericof     (501) staff       (20)      257 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.131948 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.132072 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/content/
+-rw-r--r--   0 ericof     (501) staff       (20)    25846 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      491 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.132986 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1266 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4276 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/dist_export.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3054 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/dist_import.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2486 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)      241 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.133260 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     2290 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1371 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1334 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      391 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/metaconfigure.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4174 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.133502 plone.distribution-1.0.0a9/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.133878 plone.distribution-1.0.0a9/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      334 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.134398 plone.distribution-1.0.0a9/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4694 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/services/sites/get.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.134740 plone.distribution-1.0.0a9/src/plone/distribution/testing/
+-rw-r--r--   0 ericof     (501) staff       (20)      149 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/testing/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3123 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/testing/layer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1017 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/testing/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.135059 plone.distribution-1.0.0a9/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5065 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/src/plone/distribution/utils/schema.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.127315 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)    10055 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     4392 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      208 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-27 19:16:34.000000 plone.distribution-1.0.0a9/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.135297 plone.distribution-1.0.0a9/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.135560 plone.distribution-1.0.0a9/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2166 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.136048 plone.distribution-1.0.0a9/tests/distributions/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/distributions/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/distributions/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1895 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/distributions/test_distributions_classic.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1765 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/distributions/test_distributions_default.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.136307 plone.distribution-1.0.0a9/tests/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)    12736 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/exportimport/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/exportimport/test_exportimport_helpers.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.136658 plone.distribution-1.0.0a9/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/services/test_services_site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.137015 plone.distribution-1.0.0a9/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 19:16:34.137389 plone.distribution-1.0.0a9/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1328 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/data/with_default_language.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1205 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3411 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tests/utils/test_utils_schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3740 2023-06-27 19:16:33.000000 plone.distribution-1.0.0a9/tox.ini
```

### Comparing `plone.distribution-1.0.0a8/.editorconfig` & `plone.distribution-1.0.0a9/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/.flake8` & `plone.distribution-1.0.0a9/.flake8`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/.gitignore` & `plone.distribution-1.0.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/.meta.toml` & `plone.distribution-1.0.0a9/.meta.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/.pre-commit-config.yaml` & `plone.distribution-1.0.0a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/CHANGES.md` & `plone.distribution-1.0.0a9/CHANGES.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a9 (2023-06-27)
+
+
+### Bug fixes:
+
+- Allow setting default_language "default" value [@ericof] #36
+
+
 ## 1.0.0a8 (2023-06-25)
 
 
 ### New features:
 
 - Bump @rjsf/core to version 5.8.2 [@ericof] #35
```

### Comparing `plone.distribution-1.0.0a8/LICENSE` & `plone.distribution-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/Makefile` & `plone.distribution-1.0.0a9/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/PKG-INFO` & `plone.distribution-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a9 (2023-06-27)
+
+
+### Bug fixes:
+
+- Allow setting default_language "default" value [@ericof] #36
+
+
 ## 1.0.0a8 (2023-06-25)
 
 
 ### New features:
 
 - Bump @rjsf/core to version 5.8.2 [@ericof] #35
```

### Comparing `plone.distribution-1.0.0a8/README.md` & `plone.distribution-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/Makefile` & `plone.distribution-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/_static/favicon.ico` & `plone.distribution-1.0.0a9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/_static/logo.svg` & `plone.distribution-1.0.0a9/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/_static/styles.css` & `plone.distribution-1.0.0a9/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/api/index.md` & `plone.distribution-1.0.0a9/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/conf.py` & `plone.distribution-1.0.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/index.md` & `plone.distribution-1.0.0a9/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/usage/code-examples.md` & `plone.distribution-1.0.0a9/docs/usage/code-examples.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/usage/index.md` & `plone.distribution-1.0.0a9/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/docs/usage/package-structure.md` & `plone.distribution-1.0.0a9/docs/usage/package-structure.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/mx.ini` & `plone.distribution-1.0.0a9/mx.ini`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/pyproject.toml` & `plone.distribution-1.0.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/setup.py` & `plone.distribution-1.0.0a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0a8",
+    version="1.0.0a9",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0a9/src/plone/distribution/api/distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0a9/src/plone/distribution/api/site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0a9/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/core.py` & `plone.distribution-1.0.0a9/src/plone/distribution/core.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/content.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/content.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/portal.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/content/portlets.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/content/portal.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0a9/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/configure.zcml` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/dist_export.py` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/dist_export.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/dist_import.py` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/dist_import.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/helpers.py` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/serializer.py` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/serializer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/templates/export_all.pt` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/templates/export_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/exportimport/templates/import_all.pt` & `plone.distribution-1.0.0a9/src/plone/distribution/exportimport/templates/import_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/handler.py` & `plone.distribution-1.0.0a9/src/plone/distribution/handler.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0a9/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/metaconfigure.py` & `plone.distribution-1.0.0a9/src/plone/distribution/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/registry.py` & `plone.distribution-1.0.0a9/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0a9/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0a9/src/plone/distribution/services/sites/add.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0a9/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0a9/src/plone/distribution/services/sites/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from AccessControl import getSecurityManager
 from plone.distribution.api import distribution as dist_api
 from plone.distribution.api import site as site_api
+from plone.distribution.core import Distribution
 from plone.distribution.utils.request import extract_browser_language
+from plone.distribution.utils.schema import should_provide_default_language_default
 from plone.restapi.services import Service
 from Products.CMFCore.permissions import ManagePortal
 from typing import List
 from zExceptions import BadRequest
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
 
@@ -75,26 +77,29 @@
                     "description": site.description,
                     "creation_date": site.CreationDate(),
                     "needs_upgrade": _is_outdated(site),
                 }
             )
         return response
 
-    def _populate_server_defaults(self) -> dict:
+    def _populate_server_defaults(self, distribution: Distribution) -> dict:
         """Provide default values for new Plone sites."""
+        server_defaults = {}
         request = self.request
         # Sites with default id
         all_sites = self.get_sites()
         sites = [site for site in all_sites if site["id"].startswith(DEFAULT_ID)]
-        site_id = f"{DEFAULT_ID}{len(sites)}" if sites else DEFAULT_ID
-        language = extract_browser_language(request)
-        return {
-            "site_id": site_id,
-            "default_language": language,
-        }
+        server_defaults["site_id"] = (
+            f"{DEFAULT_ID}{len(sites)}" if sites else DEFAULT_ID
+        )
+        jsonschema = distribution.schema
+        uischema = distribution.uischema
+        if should_provide_default_language_default(uischema, jsonschema):
+            server_defaults["default_language"] = extract_browser_language(request)
+        return server_defaults
 
     def can_manage(self) -> bool:
         secman = getSecurityManager()
         return True if secman.checkPermission(ManagePortal, self.context) else False
 
     def reply(self) -> dict:
         base_url = f"{self.context.absolute_url()}/@sites"
@@ -114,9 +119,9 @@
                 "@id": f"{base_url}/{dist.name}",
                 "name": dist.name,
                 "title": dist.title,
                 "description": dist.description,
                 "image": f"{base_url}/@@dist-image/{dist.name}",
                 "schema": dist.schema,
                 "uischema": dist.uischema,
-                "default_values": self._populate_server_defaults(),
+                "default_values": self._populate_server_defaults(dist),
             }
```

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/testing/layer.py` & `plone.distribution-1.0.0a9/src/plone/distribution/testing/layer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/testing/testing.py` & `plone.distribution-1.0.0a9/src/plone/distribution/testing/testing.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0a9/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0a9/src/plone/distribution/utils/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,28 @@
                 {"type": "string", "enum": [tz["value"]], "title": tz["label"]}
                 for tz in _common_timezones()
             ],
         }
     return schema
 
 
+def should_provide_default_language_default(uischema: dict, jsonschema: dict) -> bool:
+    """Decide if we should add a server value for the default_language property."""
+    server_default = True
+    if "default_language" not in uischema.get("ui:order", []):
+        # Field will not be displayed in the form, so do not provide
+        # a server default
+        server_default = False
+    else:
+        language_property = jsonschema.get("properties", {}).get("default_language", {})
+        # If default_language has a 'default' attribute, do not provide a server default
+        server_default = "default" not in language_property
+    return server_default
+
+
 def enrich_uischema(uischema: dict, jsonschema: dict) -> dict:
     """Process a uischema and set default ordering (if not present)."""
     if "ui:order" not in uischema:
         # Set order to be the same as defined in the original schema creation.
         properties = [k for k in jsonschema["properties"].keys()]
         uischema["ui:order"] = properties
     return uischema
```

### Comparing `plone.distribution-1.0.0a8/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0a9/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a9 (2023-06-27)
+
+
+### Bug fixes:
+
+- Allow setting default_language "default" value [@ericof] #36
+
+
 ## 1.0.0a8 (2023-06-25)
 
 
 ### New features:
 
 - Bump @rjsf/core to version 5.8.2 [@ericof] #35
```

### Comparing `plone.distribution-1.0.0a8/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0a9/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,8 +111,9 @@
 tests/services/__init__.py
 tests/services/conftest.py
 tests/services/test_services_site.py
 tests/utils/__init__.py
 tests/utils/test_utils_request.py
 tests/utils/test_utils_schema.py
 tests/utils/data/invalid.json
-tests/utils/data/valid.json
+tests/utils/data/valid.json
+tests/utils/data/with_default_language.json
```

### Comparing `plone.distribution-1.0.0a8/tests/api/test_api_distribution.py` & `plone.distribution-1.0.0a9/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/api/test_api_site.py` & `plone.distribution-1.0.0a9/tests/api/test_api_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/distributions/test_distributions_classic.py` & `plone.distribution-1.0.0a9/tests/distributions/test_distributions_classic.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/distributions/test_distributions_default.py` & `plone.distribution-1.0.0a9/tests/distributions/test_distributions_default.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/exportimport/portal.json` & `plone.distribution-1.0.0a9/tests/exportimport/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/exportimport/test_exportimport_helpers.py` & `plone.distribution-1.0.0a9/tests/exportimport/test_exportimport_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/services/test_services_site.py` & `plone.distribution-1.0.0a9/tests/services/test_services_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/utils/data/invalid.json` & `plone.distribution-1.0.0a9/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/utils/data/valid.json` & `plone.distribution-1.0.0a9/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/utils/test_utils_request.py` & `plone.distribution-1.0.0a9/tests/utils/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a8/tests/utils/test_utils_schema.py` & `plone.distribution-1.0.0a9/tests/utils/test_utils_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 @pytest.fixture
 def data_path() -> Path:
     cur_dir = Path(__file__).parent.resolve()
     return cur_dir / "data"
 
 
 @pytest.fixture
+def language_schema(data_path):
+    return json.loads((data_path / "with_default_language.json").read_text())
+
+
+@pytest.fixture
 def valid_schema(data_path):
     return json.loads((data_path / "valid.json").read_text())
 
 
 @pytest.fixture
 def invalid_schema(data_path):
     return json.loads((data_path / "invalid.json").read_text())
@@ -80,7 +85,27 @@
 
     def test_enrich_uischema(self, app, valid_schema):
         result = self.func(valid_schema)
         assert "schema" in result
         assert "uischema" in result
         uischema = result["uischema"]
         assert "ui:order" in uischema
+
+
+class TestUtilsSchemaDefaultLanguage:
+    def process_schema(self, raw_schema):
+        schema = utils_schema.process_raw_schema(raw_schema)
+        return schema["uischema"], schema["schema"]
+
+    @property
+    def func(self):
+        return utils_schema.should_provide_default_language_default
+
+    def test_should_provide_default_language_default_true(self, app, valid_schema):
+        uischema, jsonschema = self.process_schema(valid_schema)
+        result = self.func(uischema, jsonschema)
+        assert result is True
+
+    def test_should_provide_default_language_default_false(self, app, language_schema):
+        uischema, jsonschema = self.process_schema(language_schema)
+        result = self.func(uischema, jsonschema)
+        assert result is False
```

### Comparing `plone.distribution-1.0.0a8/tox.ini` & `plone.distribution-1.0.0a9/tox.ini`

 * *Files identical despite different names*

