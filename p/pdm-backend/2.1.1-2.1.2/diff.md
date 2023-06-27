# Comparing `tmp/pdm_backend-2.1.1.tar.gz` & `tmp/pdm_backend-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.1.1.tar", last modified: Mon Jun 26 01:32:02 2023, max compression
+gzip compressed data, was "pdm_backend-2.1.2.tar", last modified: Tue Jun 27 01:24:02 2023, max compression
```

## Comparing `pdm_backend-2.1.1.tar` & `pdm_backend-2.1.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1067 2023-06-26 01:31:40.666484 pdm_backend-2.1.1/LICENSE
--rw-r--r--   0        0        0     1725 2023-06-26 01:31:40.666484 pdm_backend-2.1.1/README.md
--rw-r--r--   0        0        0     2271 2023-06-26 01:32:02.454833 pdm_backend-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3282 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      661 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9606 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5115 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     7928 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    38937 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16469 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16315 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    19827 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0       70 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    11948 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9872 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/config.py
--rw-r--r--   0        0        0     4063 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      452 2023-06-26 01:31:40.670484 pdm_backend-2.1.1/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4429 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6364 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     4894 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10129 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0      759 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14958 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3604 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     7080 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    11706 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0      747 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/conftest.py
--rw-r--r--   0        0        0      856 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-license/src/foo_module.py
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-version/README.md
-lrwxr-xr-x   0        0        0        0 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      639 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rwxr-xr-x   0        0        0       32 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/scripts/my_script.sh
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.674484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    18382 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_api.py
--rw-r--r--   0        0        0     5324 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_metadata.py
--rw-r--r--   0        0        0      311 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/test_wheel.py
--rw-r--r--   0        0        0      598 2023-06-26 01:31:40.678484 pdm_backend-2.1.1/tests/testutils.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1725 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/README.md
+-rw-r--r--   0        0        0     2271 2023-06-27 01:24:02.945014 pdm_backend-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3282 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-06-27 01:23:49.776665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      661 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9606 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5115 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     7928 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    38937 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16469 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16315 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    19827 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       70 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    11948 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9872 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     4063 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6364 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     4894 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10129 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0      759 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14958 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3050 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     7661 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    11894 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      856 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.780665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      639 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rwxr-xr-x   0        0        0       32 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/scripts/my_script.sh
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0    18382 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_metadata.py
+-rw-r--r--   0        0        0      311 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/test_wheel.py
+-rw-r--r--   0        0        0      598 2023-06-27 01:23:49.784665 pdm_backend-2.1.2/tests/testutils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.1.2/PKG-INFO
```

### Comparing `pdm_backend-2.1.1/LICENSE` & `pdm_backend-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/README.md` & `pdm_backend-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/pyproject.toml` & `pdm_backend-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.1.1"
+version = "2.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
```

### Comparing `pdm_backend-2.1.1/src/pdm/backend/__init__.py` & `pdm_backend-2.1.2/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/__about__.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.1.2/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/base.py` & `pdm_backend-2.1.2/src/pdm/backend/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/config.py` & `pdm_backend-2.1.2/src/pdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/editable.py` & `pdm_backend-2.1.2/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/hooks/base.py` & `pdm_backend-2.1.2/src/pdm/backend/hooks/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.1.2/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.1.2/src/pdm/backend/hooks/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.1.2/src/pdm/backend/hooks/version/scm.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/intree.py` & `pdm_backend-2.1.2/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.1.2/src/pdm/backend/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/sdist.py` & `pdm_backend-2.1.2/src/pdm/backend/sdist.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,31 +7,15 @@
 from pathlib import Path
 from posixpath import join as pjoin
 from typing import Iterable
 
 from pdm.backend._vendor.packaging.utils import canonicalize_name
 from pdm.backend.base import Builder
 from pdm.backend.hooks import Context
-from pdm.backend.utils import safe_version, to_filename
-
-
-def normalize_file_permissions(st_mode: int) -> int:
-    """
-    Normalizes the permission bits in the st_mode field from stat to 644/755
-
-    Popular VCSs only track whether a file is executable or not. The exact
-    permissions can vary on systems with different umasks. Normalising
-    to 644 (non executable) or 755 (executable) makes builds more reproducible.
-    """
-    # Set 644 permissions, leaving higher bits of st_mode unchanged
-    new_mode = (st_mode | 0o644) & ~0o133
-    if st_mode & 0o100:
-        new_mode |= 0o111  # Executable: 644 -> 755
-
-    return new_mode
+from pdm.backend.utils import normalize_file_permissions, safe_version, to_filename
 
 
 def clean_tarinfo(tar_info: tarfile.TarInfo) -> tarfile.TarInfo:
     """
     Clean metadata from a TarInfo object to make it more reproducible.
 
         - Set uid & gid to 0
```

### Comparing `pdm_backend-2.1.1/src/pdm/backend/structures.py` & `pdm_backend-2.1.2/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/src/pdm/backend/utils.py` & `pdm_backend-2.1.2/src/pdm/backend/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,7 +215,22 @@
     """Import a module from a given path."""
     spec = importlib.util.spec_from_file_location(module_name, src_path)
     if spec is None:
         raise ValueError(f"Could not import module {module_name} from {src_path}")
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)  # type: ignore
     return module
+
+
+def normalize_file_permissions(st_mode: int) -> int:
+    """
+    Normalizes the permission bits in the st_mode field from stat to 644/755
+    Popular VCSs only track whether a file is executable or not. The exact
+    permissions can vary on systems with different umasks. Normalising
+    to 644 (non executable) or 755 (executable) makes builds more reproducible.
+    """
+    # Set 644 permissions, leaving higher bits of st_mode unchanged
+    new_mode = (st_mode | 0o644) & ~0o133
+    if st_mode & 0o100:
+        new_mode |= 0o111  # Executable: 644 -> 755
+
+    return new_mode
```

### Comparing `pdm_backend-2.1.1/src/pdm/backend/wheel.py` & `pdm_backend-2.1.2/src/pdm/backend/wheel.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pdm.backend.base import Builder
 from pdm.backend.hooks import Context
 from pdm.backend.hooks.setuptools import SetuptoolsBuildHook
 from pdm.backend.utils import (
     expand_vars,
     get_abi_tag,
     get_platform,
+    normalize_file_permissions,
     safe_version,
     to_filename,
 )
 
 SCHEME_NAMES = frozenset(
     ["purelib", "platlib", "include", "platinclude", "scripts", "data"]
 )
@@ -146,24 +147,29 @@
                     )
                     yield self.scheme_path(name, relpath), child
 
     def build_artifact(
         self, context: Context, files: Iterable[tuple[str, Path]]
     ) -> Path:
         records: list[RecordEntry] = []
-        with tempfile.NamedTemporaryFile(suffix=".whl", delete=False) as fp:
+        fd, temp_name = tempfile.mkstemp(suffix=".whl")
+        st_mode = os.stat(temp_name).st_mode
+        new_mode = normalize_file_permissions(st_mode)
+        os.chmod(temp_name, new_mode)
+
+        with os.fdopen(fd, "w+b") as fp:
             with zipfile.ZipFile(fp, "w", compression=zipfile.ZIP_DEFLATED) as zf:
                 for rel_path, full_path in files:
                     records.append(self._add_file_to_zip(zf, rel_path, full_path))
                 self._write_record(zf, records)
 
         target = context.dist_dir / f"{self.name_version}-{self.tag}.whl"
         if target.exists():
             target.unlink()
-        shutil.move(fp.name, target)
+        shutil.move(temp_name, target)
         return target
 
     @property
     def name_version(self) -> str:
         name = to_filename(canonicalize_name(self.config.metadata["name"]))
         version = to_filename(safe_version(self.config.metadata["version"]))
         return f"{name}-{version}"
@@ -231,35 +237,34 @@
         return dist_info
 
     def _add_file_to_zip(
         self, zf: zipfile.ZipFile, rel_path: str, full_path: Path
     ) -> RecordEntry:
         self._show_add_file(rel_path, full_path)
         zi = zipfile.ZipInfo(rel_path, ZIPINFO_DATE_TIME)
-        st_mode = os.stat(full_path).st_mode
-        zi.external_attr = (st_mode & 0xFFFF) << 16  # Unix attributes
+        st_mode = full_path.stat().st_mode
+        new_mode = normalize_file_permissions(st_mode)
+        zi.external_attr = (new_mode & 0xFFFF) << 16  # Unix attributes
 
         if stat.S_ISDIR(st_mode):
             zi.external_attr |= 0x10  # MS-DOS directory flag
 
         with full_path.open("rb") as src:
             hash_digest = self._write_zip_info(zf, zi, src)
         size = zi.file_size
         return RecordEntry(rel_path, f"sha256={hash_digest}", str(size))
 
     @staticmethod
     def _write_zip_info(
         zf: zipfile.ZipFile, zi: zipfile.ZipInfo, src: IO[bytes]
     ) -> str:
         hashsum = hashlib.sha256()
-        for buf in iter(lambda: src.read(2**16), b""):
-            hashsum.update(buf)
-
-        src.seek(0)
-        zf.writestr(zi, src.read(), compress_type=zipfile.ZIP_DEFLATED)
+        data = src.read()
+        hashsum.update(data)
+        zf.writestr(zi, data, compress_type=zipfile.ZIP_DEFLATED)
         return urlsafe_b64encode(hashsum.digest()).decode("ascii").rstrip("=")
 
     def _write_record(self, zf: zipfile.ZipFile, records: list[RecordEntry]) -> None:
         zi = zipfile.ZipInfo(f"{self.dist_info_name}/RECORD", ZIPINFO_DATE_TIME)
         buffer = io.BytesIO()
         text_buffer = io.TextIOWrapper(buffer, encoding="utf-8", newline="")
```

### Comparing `pdm_backend-2.1.1/tests/conftest.py` & `pdm_backend-2.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.1.2/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.1.2/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.1.2/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.1.2/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/test_api.py` & `pdm_backend-2.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/test_file_finder.py` & `pdm_backend-2.1.2/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/test_hooks.py` & `pdm_backend-2.1.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/test_metadata.py` & `pdm_backend-2.1.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/test_wheel.py` & `pdm_backend-2.1.2/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/tests/testutils.py` & `pdm_backend-2.1.2/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.1.1/PKG-INFO` & `pdm_backend-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.1.1
+Version: 2.1.2
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging PEP 517 build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.1.1 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.1.2 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging PEP 517 build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

