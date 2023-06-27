# Comparing `tmp/tuxbake-0.4.1.tar.gz` & `tmp/tuxbake-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxbake-0.4.1.tar", last modified: Tue May 30 14:47:51 2023, max compression
+gzip compressed data, was "tuxbake-0.5.0.tar", last modified: Tue Jun 27 12:16:20 2023, max compression
```

## Comparing `tuxbake-0.4.1.tar` & `tuxbake-0.5.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0       94 2023-05-30 14:47:49.328650 tuxbake-0.4.1/.gitignore
--rw-r--r--   0        0        0     2767 2023-05-30 14:47:49.328650 tuxbake-0.4.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      879 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Dockerfile.ci-debian
--rw-r--r--   0        0        0      555 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-05-30 14:47:49.328650 tuxbake-0.4.1/LICENSE
--rw-r--r--   0        0        0     1211 2023-05-30 14:47:49.328650 tuxbake-0.4.1/Makefile
--rw-r--r--   0        0        0     4869 2023-05-30 14:47:49.328650 tuxbake-0.4.1/README.md
--rw-r--r--   0        0        0      141 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/changelog
--rw-r--r--   0        0        0      700 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/control
--rw-r--r--   0        0        0      100 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/gbp.conf
--rwxr-xr-x   0        0        0      594 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/rules
--rw-r--r--   0        0        0       12 2023-05-30 14:47:49.328650 tuxbake-0.4.1/debian/source/format
--rw-r--r--   0        0        0     1051 2023-05-30 14:47:49.328650 tuxbake-0.4.1/dockerfiles/Makefile
--rw-r--r--   0        0        0     1485 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/centos-7/Dockerfile
--rw-r--r--   0        0        0     1838 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/centos-8/Dockerfile
--rw-r--r--   0        0        0     1823 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-bullseye/Dockerfile
--rw-r--r--   0        0        0     1821 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-buster/Dockerfile
--rw-r--r--   0        0        0     2259 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/debian-stretch/Dockerfile
--rw-r--r--   0        0        0     1803 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/fedora-33/Dockerfile
--rw-r--r--   0        0        0     1714 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/fedora-34/Dockerfile
--rw-r--r--   0        0        0     1535 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/opensuse-leap-15.1/Dockerfile
--rw-r--r--   0        0        0     1535 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/opensuse-leap-15.2/Dockerfile
--rw-r--r--   0        0        0     1564 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-16.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-18.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-20.04/Dockerfile
--rw-r--r--   0        0        0     1631 2023-05-30 14:47:49.329650 tuxbake-0.4.1/dockerfiles/ubuntu-22.04/Dockerfile
--rw-r--r--   0        0        0       76 2023-05-30 14:47:49.329650 tuxbake-0.4.1/examples/README.md
--rw-r--r--   0        0        0      416 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/demo.json
--rw-r--r--   0        0        0      314 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/ledge-rpb.json
--rw-r--r--   0        0        0      894 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/lkft.json
--rw-r--r--   0        0        0      495 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/lt-qcom.json
--rw-r--r--   0        0        0      387 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/oe-rpb.json
--rw-r--r--   0        0        0      409 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/oniro.json
--rw-r--r--   0        0        0      387 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/qcom-rpb-dunfell.json
--rw-r--r--   0        0        0      388 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/qcom-rpb-honister.json
--rw-r--r--   0        0        0      684 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/template.json
--rw-r--r--   0        0        0      325 2023-05-30 14:47:49.330650 tuxbake-0.4.1/examples/yocto.json
--rw-r--r--   0        0        0      437 2023-05-30 14:47:49.330650 tuxbake-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-30 14:47:49.330650 tuxbake-0.4.1/requirements-dev.txt
--rw-r--r--   0        0        0   594416 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/bitbake-environment
--rw-r--r--   0        0        0     6264 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/conftest.py
--rw-r--r--   0        0        0      204 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test.xml
--rw-r--r--   0        0        0     1369 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_argparse.py
--rw-r--r--   0        0        0      661 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_build.py
--rw-r--r--   0        0        0     5156 2023-05-30 14:47:49.332650 tuxbake-0.4.1/tests/unit/test_metadata.py
--rw-r--r--   0        0        0     9748 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tests/unit/test_models.py
--rw-r--r--   0        0        0     5723 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1409 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake.spec
--rw-r--r--   0        0        0      112 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/__main__.py
--rw-r--r--   0        0        0     2984 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/argparse.py
--rw-r--r--   0        0        0      784 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/build.py
--rw-r--r--   0        0        0      747 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/exceptions.py
--rw-r--r--   0        0        0     5014 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/helper.py
--rw-r--r--   0        0        0     1361 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata.pl
--rw-r--r--   0        0        0     7276 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata.py
--rw-r--r--   0        0        0      165 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/hardware.ini
--rw-r--r--   0        0        0      300 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/os.ini
--rw-r--r--   0        0        0       89 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/resources.ini
--rw-r--r--   0        0        0     1602 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/tools.ini
--rw-r--r--   0        0        0      190 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/metadata/uname.ini
--rw-r--r--   0        0        0    14919 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/models.py
--rw-r--r--   0        0        0     6537 2023-05-30 14:47:49.333650 tuxbake-0.4.1/tuxbake/utils.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 tuxbake-0.4.1/setup.py
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxbake-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-06-27 12:16:18.251730 tuxbake-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2767 2023-06-27 12:16:18.251730 tuxbake-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      879 2023-06-27 12:16:18.251730 tuxbake-0.5.0/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      555 2023-06-27 12:16:18.251730 tuxbake-0.5.0/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2023-06-27 12:16:18.251730 tuxbake-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1211 2023-06-27 12:16:18.252730 tuxbake-0.5.0/Makefile
+-rw-r--r--   0        0        0     4869 2023-06-27 12:16:18.252730 tuxbake-0.5.0/README.md
+-rw-r--r--   0        0        0      141 2023-06-27 12:16:18.252730 tuxbake-0.5.0/debian/changelog
+-rw-r--r--   0        0        0      700 2023-06-27 12:16:18.252730 tuxbake-0.5.0/debian/control
+-rw-r--r--   0        0        0      100 2023-06-27 12:16:18.252730 tuxbake-0.5.0/debian/gbp.conf
+-rwxr-xr-x   0        0        0      594 2023-06-27 12:16:18.252730 tuxbake-0.5.0/debian/rules
+-rw-r--r--   0        0        0       12 2023-06-27 12:16:18.252730 tuxbake-0.5.0/debian/source/format
+-rw-r--r--   0        0        0     1051 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/Makefile
+-rw-r--r--   0        0        0     1485 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/centos-7/Dockerfile
+-rw-r--r--   0        0        0     1838 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/centos-8/Dockerfile
+-rw-r--r--   0        0        0     1823 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/debian-bullseye/Dockerfile
+-rw-r--r--   0        0        0     1821 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/debian-buster/Dockerfile
+-rw-r--r--   0        0        0     2259 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/debian-stretch/Dockerfile
+-rw-r--r--   0        0        0     1803 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/fedora-33/Dockerfile
+-rw-r--r--   0        0        0     1714 2023-06-27 12:16:18.252730 tuxbake-0.5.0/dockerfiles/fedora-34/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/opensuse-leap-15.1/Dockerfile
+-rw-r--r--   0        0        0     1535 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/opensuse-leap-15.2/Dockerfile
+-rw-r--r--   0        0        0     1583 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/ubuntu-16.04/Dockerfile
+-rw-r--r--   0        0        0     1650 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/ubuntu-18.04/Dockerfile
+-rw-r--r--   0        0        0     1690 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/ubuntu-20.04/Dockerfile
+-rw-r--r--   0        0        0     1650 2023-06-27 12:16:18.253730 tuxbake-0.5.0/dockerfiles/ubuntu-22.04/Dockerfile
+-rw-r--r--   0        0        0       76 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/README.md
+-rw-r--r--   0        0        0      416 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/demo.json
+-rw-r--r--   0        0        0      314 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/ledge-rpb.json
+-rw-r--r--   0        0        0      894 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/lkft.json
+-rw-r--r--   0        0        0      495 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/lt-qcom.json
+-rw-r--r--   0        0        0      387 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/oe-rpb.json
+-rw-r--r--   0        0        0      409 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/oniro.json
+-rw-r--r--   0        0        0      387 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/qcom-rpb-dunfell.json
+-rw-r--r--   0        0        0      388 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/qcom-rpb-honister.json
+-rw-r--r--   0        0        0      684 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/template.json
+-rw-r--r--   0        0        0      325 2023-06-27 12:16:18.253730 tuxbake-0.5.0/examples/yocto.json
+-rw-r--r--   0        0        0      437 2023-06-27 12:16:18.253730 tuxbake-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-27 12:16:18.253730 tuxbake-0.5.0/requirements-dev.txt
+-rw-r--r--   0        0        0   594416 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/bitbake-environment
+-rw-r--r--   0        0        0     6264 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0      204 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test.xml
+-rw-r--r--   0        0        0     1369 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test_argparse.py
+-rw-r--r--   0        0        0      661 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test_build.py
+-rw-r--r--   0        0        0     5156 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test_metadata.py
+-rw-r--r--   0        0        0     9748 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test_models.py
+-rw-r--r--   0        0        0     5723 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1409 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake.spec
+-rw-r--r--   0        0        0      112 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/__init__.py
+-rw-r--r--   0        0        0     1909 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/__main__.py
+-rw-r--r--   0        0        0     2984 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/argparse.py
+-rw-r--r--   0        0        0      784 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/build.py
+-rw-r--r--   0        0        0      747 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/exceptions.py
+-rw-r--r--   0        0        0     5014 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/helper.py
+-rw-r--r--   0        0        0     1361 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/metadata.pl
+-rw-r--r--   0        0        0     7276 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/metadata.py
+-rw-r--r--   0        0        0      165 2023-06-27 12:16:18.255730 tuxbake-0.5.0/tuxbake/metadata/hardware.ini
+-rw-r--r--   0        0        0      300 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/metadata/os.ini
+-rw-r--r--   0        0        0       89 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/metadata/resources.ini
+-rw-r--r--   0        0        0     1602 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/metadata/tools.ini
+-rw-r--r--   0        0        0      190 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/metadata/uname.ini
+-rw-r--r--   0        0        0    14921 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/models.py
+-rw-r--r--   0        0        0     6681 2023-06-27 12:16:18.256730 tuxbake-0.5.0/tuxbake/utils.py
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 tuxbake-0.5.0/PKG-INFO
```

### Comparing `tuxbake-0.4.1/.gitlab-ci.yml` & `tuxbake-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/Dockerfile.ci-debian` & `tuxbake-0.5.0/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/Dockerfile.ci-fedora` & `tuxbake-0.5.0/Dockerfile.ci-fedora`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/LICENSE` & `tuxbake-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/Makefile` & `tuxbake-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/README.md` & `tuxbake-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/debian/control` & `tuxbake-0.5.0/debian/control`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/debian/rules` & `tuxbake-0.5.0/debian/rules`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/Makefile` & `tuxbake-0.5.0/dockerfiles/Makefile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/centos-7/Dockerfile` & `tuxbake-0.5.0/dockerfiles/centos-7/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/centos-8/Dockerfile` & `tuxbake-0.5.0/dockerfiles/centos-8/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/debian-bullseye/Dockerfile` & `tuxbake-0.5.0/dockerfiles/debian-bullseye/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/debian-buster/Dockerfile` & `tuxbake-0.5.0/dockerfiles/debian-buster/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/debian-stretch/Dockerfile` & `tuxbake-0.5.0/dockerfiles/debian-stretch/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/fedora-33/Dockerfile` & `tuxbake-0.5.0/dockerfiles/fedora-33/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/fedora-34/Dockerfile` & `tuxbake-0.5.0/dockerfiles/fedora-34/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/opensuse-leap-15.1/Dockerfile` & `tuxbake-0.5.0/dockerfiles/opensuse-leap-15.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/opensuse-leap-15.2/Dockerfile` & `tuxbake-0.5.0/dockerfiles/opensuse-leap-15.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/dockerfiles/ubuntu-16.04/Dockerfile` & `tuxbake-0.5.0/dockerfiles/ubuntu-16.04/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     jq \
     less \
     locales \
     openssh-client \
     pigz \
     python3 \
     python3-pip \
+    python3-venv \
     socat \
     sudo \
     texinfo \
     unzip \
     wget \
     xz-utils \
     xmlstarlet \
```

### Comparing `tuxbake-0.4.1/dockerfiles/ubuntu-18.04/Dockerfile` & `tuxbake-0.5.0/dockerfiles/ubuntu-20.04/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM docker.io/library/ubuntu:bionic
+FROM docker.io/library/ubuntu:focal
 
 ENV DEBIAN_FRONTEND=noninteractive
 ENV LANG=en_US.UTF-8
 ENV PKG_DEPS="\
     build-essential \
     chrpath \
     cpio \
@@ -16,28 +16,31 @@
     jq \
     less \
     locales \
     openssh-client \
     pigz \
     python3 \
     python3-pip \
+    python3-venv \
     socat \
     sudo \
     texinfo \
     unzip \
     wget \
     xz-utils \
     xmlstarlet \
     awscli \
     libssl-dev \
     libc6-dev-i386 \
     liblz4-tool \
     zstd \
-    python \
+    python2 \
     iproute2 \
+    libc6-dev-i386 \
+    gcc-multilib \
 "
 
 RUN set -e ;\
     echo 'locales locales/locales_to_be_generated multiselect C.UTF-8 UTF-8, en_US.UTF-8 UTF-8 ' | debconf-set-selections ;\
     echo 'locales locales/default_environment_locale select en_US.UTF-8' | debconf-set-selections ;\
     echo 'dash dash/sh boolean false' | debconf-set-selections ;\
     apt update -q=2 ;\
```

### Comparing `tuxbake-0.4.1/dockerfiles/ubuntu-20.04/Dockerfile` & `tuxbake-0.5.0/dockerfiles/ubuntu-22.04/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM docker.io/library/ubuntu:focal
+FROM docker.io/library/ubuntu:jammy
 
 ENV DEBIAN_FRONTEND=noninteractive
 ENV LANG=en_US.UTF-8
 ENV PKG_DEPS="\
     build-essential \
     chrpath \
     cpio \
@@ -16,14 +16,15 @@
     jq \
     less \
     locales \
     openssh-client \
     pigz \
     python3 \
     python3-pip \
+    python3-venv \
     socat \
     sudo \
     texinfo \
     unzip \
     wget \
     xz-utils \
     xmlstarlet \
```

### Comparing `tuxbake-0.4.1/dockerfiles/ubuntu-22.04/Dockerfile` & `tuxbake-0.5.0/dockerfiles/ubuntu-18.04/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM docker.io/library/ubuntu:jammy
+FROM docker.io/library/ubuntu:bionic
 
 ENV DEBIAN_FRONTEND=noninteractive
 ENV LANG=en_US.UTF-8
 ENV PKG_DEPS="\
     build-essential \
     chrpath \
     cpio \
@@ -16,27 +16,28 @@
     jq \
     less \
     locales \
     openssh-client \
     pigz \
     python3 \
     python3-pip \
+    python3-venv \
     socat \
     sudo \
     texinfo \
     unzip \
     wget \
     xz-utils \
     xmlstarlet \
     awscli \
     libssl-dev \
     libc6-dev-i386 \
     liblz4-tool \
     zstd \
-    python2 \
+    python \
     iproute2 \
 "
 
 RUN set -e ;\
     echo 'locales locales/locales_to_be_generated multiselect C.UTF-8 UTF-8, en_US.UTF-8 UTF-8 ' | debconf-set-selections ;\
     echo 'locales locales/default_environment_locale select en_US.UTF-8' | debconf-set-selections ;\
     echo 'dash dash/sh boolean false' | debconf-set-selections ;\
```

### Comparing `tuxbake-0.4.1/examples/lkft.json` & `tuxbake-0.5.0/examples/lkft.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/examples/template.json` & `tuxbake-0.5.0/examples/template.json`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/bitbake-environment` & `tuxbake-0.5.0/tests/unit/bitbake-environment`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/conftest.py` & `tuxbake-0.5.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/test_argparse.py` & `tuxbake-0.5.0/tests/unit/test_argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/test_build.py` & `tuxbake-0.5.0/tests/unit/test_build.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/test_metadata.py` & `tuxbake-0.5.0/tests/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/test_models.py` & `tuxbake-0.5.0/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tests/unit/test_utils.py` & `tuxbake-0.5.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake.spec` & `tuxbake-0.5.0/tuxbake.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxbake
-Version:   0.4.1
+Version:   0.5.0
 Release:   0%{?dist}
 Summary:   FIXME
 License:   FIXME
 URL:       FIXME
 Source0:   %{pypi_source}
```

### Comparing `tuxbake-0.4.1/tuxbake/__main__.py` & `tuxbake-0.5.0/tuxbake/__main__.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/argparse.py` & `tuxbake-0.5.0/tuxbake/argparse.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/build.py` & `tuxbake-0.5.0/tuxbake/build.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/exceptions.py` & `tuxbake-0.5.0/tuxbake/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/helper.py` & `tuxbake-0.5.0/tuxbake/helper.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/metadata.pl` & `tuxbake-0.5.0/tuxbake/metadata.pl`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/metadata.py` & `tuxbake-0.5.0/tuxbake/metadata.py`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/metadata/tools.ini` & `tuxbake-0.5.0/tuxbake/metadata/tools.ini`

 * *Files identical despite different names*

### Comparing `tuxbake-0.4.1/tuxbake/models.py` & `tuxbake-0.5.0/tuxbake/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 
     def __prepare__(self):
         os.makedirs(self.src_dir, exist_ok=True)
         os.makedirs(self.log_dir, exist_ok=True)
         debug(f"build-only flag set to: {self.build_only}")
         debug(f"sync-only flag set to: {self.sync_only}")
         if self.build_only and self.sync_only:
-            print("ERROR: Both build-only and sync-only shoun't be set.")
+            print("ERROR: Both build-only and sync-only shouldn't be set.")
         if self.build_only:
             return
         if self.sources.get("repo"):
             repo_init(self, self.src_dir, self.local_manifest, self.pinned_manifest)
         else:
             git_init(self, self.src_dir)
```

### Comparing `tuxbake-0.4.1/tuxbake/utils.py` & `tuxbake-0.5.0/tuxbake/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     cmd = "repo sync -j16".split()
     run_cmd(cmd, src_dir)
     cmd = "repo manifest -r -o pinned-manifest.xml".split()
     run_cmd(cmd, src_dir)
 
 
 def git_fetch(what_to_fetch, src_dir, dir_path):
-    cmd = f"git fetch origin --quiet {what_to_fetch}".split()
+    cmd = f"git fetch origin --quiet --recurse-submodules=no {what_to_fetch}".split()
     run_cmd(cmd, os.path.join(src_dir, dir_path))
 
 
 def git_get_sha(branch, url):
     cmd = f"git ls-remote --exit-code --quiet {url} {branch}".split()
     try:
         ret = run_cmd(cmd, None)
@@ -120,14 +120,17 @@
             cmd = f"git remote add origin {url}".split()
             run_cmd(cmd, os.path.join(src_dir, dir_path))
 
         git_fetch(sha, src_dir, dir_path)
         cmd = f"git checkout {sha}".split()
         run_cmd(cmd, os.path.join(src_dir, dir_path))
 
+        cmd = f"git submodule update --init --recursive".split()
+        run_cmd(cmd, os.path.join(src_dir, dir_path))
+
 
 def get_filtered_paths(artifacts, path):
     """
     Return resolved artifacts paths which are present relative to provided path. Rest other paths are discarded.
     """
     dir_paths = []
     if artifacts and path:
```

