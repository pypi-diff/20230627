# Comparing `tmp/batou-2.3b6.tar.gz` & `tmp/batou-2.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.3b6.tar", last modified: Fri Dec  9 13:30:50 2022, max compression
+gzip compressed data, was "batou-2.4a1.tar", last modified: Tue Jun 27 10:23:48 2023, max compression
```

## Comparing `batou-2.3b6.tar` & `batou-2.4a1.tar`

### file list

```diff
@@ -1,258 +1,264 @@
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931588 batou-2.3b6/
--rw-r--r--   0 ctheune    (501) staff       (20)    31241 2022-12-09 13:30:48.000000 batou-2.3b6/CHANGES.history.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1608 2022-12-09 13:30:48.000000 batou-2.3b6/LICENSE.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      212 2022-12-09 13:30:48.000000 batou-2.3b6/MANIFEST.in
--rw-r--r--   0 ctheune    (501) staff       (20)     3445 2022-12-09 13:30:50.931687 batou-2.3b6/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     2636 2022-12-09 13:30:48.000000 batou-2.3b6/README.md
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.897450 batou-2.3b6/doc/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.904614 batou-2.3b6/doc/source/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.905190 batou-2.3b6/doc/source/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      886 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/component.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1717 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/environment.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       48 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/templates.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       63 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/utilities.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.905331 batou-2.3b6/doc/source/cli/
--rw-r--r--   0 ctheune    (501) staff       (20)     3742 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/cli/index.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.906097 batou-2.3b6/doc/source/components/
--rw-r--r--   0 ctheune    (501) staff       (20)     1025 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/cmmi.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2941 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     5657 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/files.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4820 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/python.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3050 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/services.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.906684 batou-2.3b6/doc/source/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)      718 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/authors.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8555 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/contributing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1711 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/testing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2809 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/todo.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8196 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4799 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/upgrading.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.907554 batou-2.3b6/doc/source/user/
--rw-r--r--   0 ctheune    (501) staff       (20)    10868 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/advanced.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2565 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/install.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3848 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/installation-deb.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3798 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/installation-rpm.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2907 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/intro.txt
--rw-r--r--   0 ctheune    (501) staff       (20)    47402 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/quickstart.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899351 batou-2.3b6/examples/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.907871 batou-2.3b6/examples/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      349 2022-12-09 13:30:48.000000 batou-2.3b6/examples/api/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/api/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908018 batou-2.3b6/examples/django/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/django/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908159 batou-2.3b6/examples/errors/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/errors/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908308 batou-2.3b6/examples/errors2/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/errors2/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908458 batou-2.3b6/examples/ignores/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/ignores/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908605 batou-2.3b6/examples/largetempl/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/largetempl/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908749 batou-2.3b6/examples/package/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/package/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908889 batou-2.3b6/examples/sync_async/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/sync_async/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909031 batou-2.3b6/examples/tutorial-buildout/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909179 batou-2.3b6/examples/tutorial-component/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909320 batou-2.3b6/examples/tutorial-helloworld/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909473 batou-2.3b6/examples/tutorial-parallelize/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909621 batou-2.3b6/examples/tutorial-provision-container/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909773 batou-2.3b6/examples/tutorial-secrets/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909919 batou-2.3b6/examples/vagrant/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/vagrant/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910065 batou-2.3b6/examples/vagrant-multi/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910209 batou-2.3b6/examples/venvs/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910354 batou-2.3b6/examples/venvs/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/venvs/environments/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/venvs/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      129 2022-12-09 13:30:48.000000 batou-2.3b6/pyproject.toml
--rw-r--r--   0 ctheune    (501) staff       (20)      275 2022-12-09 13:30:48.000000 batou-2.3b6/requirements-dev.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      139 2022-12-09 13:30:50.932007 batou-2.3b6/setup.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)     2408 2022-12-09 13:30:48.000000 batou-2.3b6/setup.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899658 batou-2.3b6/src/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.913247 batou-2.3b6/src/batou/
--rw-r--r--   0 ctheune    (501) staff       (20)    19689 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      997 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/_output.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/agent.py
--rw-r--r--   0 ctheune    (501) staff       (20)      163 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/c.py
--rw-r--r--   0 ctheune    (501) staff       (20)    40142 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/component.py
--rw-r--r--   0 ctheune    (501) staff       (20)      503 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)    14278 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)    19471 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1507 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/fixtures.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11006 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/host.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914396 batou-2.3b6/src/batou/init-template/
--rw-r--r--   0 ctheune    (501) staff       (20)       44 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/.hgignore
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899884 batou-2.3b6/src/batou/init-template/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914545 batou-2.3b6/src/batou/init-template/components/example/
--rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914692 batou-2.3b6/src/batou/init-template/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       66 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      411 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/insecure-private.key
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.917533 batou-2.3b6/src/batou/lib/
--rw-r--r--   0 ctheune    (501) staff       (20)       29 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3983 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6457 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3297 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2211 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2524 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1224 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2286 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    22046 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/file.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5811 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/git.py
--rw-r--r--   0 ctheune    (501) staff       (20)      854 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/goceptnet.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1388 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/logrotate.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4541 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3647 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2814 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/package.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8150 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/python.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.918671 batou-2.3b6/src/batou/lib/resources/
--rw-r--r--   0 ctheune    (501) staff       (20)     2120 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 ctheune    (501) staff       (20)      244 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/crontab
--rw-r--r--   0 ctheune    (501) staff       (20)      548 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/init.sh
--rw-r--r--   0 ctheune    (501) staff       (20)      299 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 ctheune    (501) staff       (20)      840 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      153 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      380 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      609 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 ctheune    (501) staff       (20)      932 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/service.py
--rw-r--r--   0 ctheune    (501) staff       (20)    10273 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1172 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/svn.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921053 batou-2.3b6/src/batou/lib/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3083 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3858 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2318 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3261 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2110 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)      639 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2158 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    31505 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_file.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9642 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_git.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6165 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)      121 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)      847 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1163 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_python.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1693 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_service.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3106 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6237 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/main.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921192 batou-2.3b6/src/batou/migrate/
--rw-r--r--   0 ctheune    (501) staff       (20)     3377 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921901 batou-2.3b6/src/batou/migrate/migrations/
--rw-r--r--   0 ctheune    (501) staff       (20)      389 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1775 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 ctheune    (501) staff       (20)      874 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 ctheune    (501) staff       (20)      790 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.922152 batou-2.3b6/src/batou/migrate/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4532 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 ctheune    (501) staff       (20)    12756 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/provision.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11721 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11793 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6403 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/resources.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.922722 batou-2.3b6/src/batou/secrets/
--rw-r--r--   0 ctheune    (501) staff       (20)     3295 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3920 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/edit.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8524 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/encryption.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4353 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/manage.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.923312 batou-2.3b6/src/batou/secrets/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)       23 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3136 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2019 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5844 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2429 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/template.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926616 batou-2.3b6/src/batou/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      666 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3012 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.903141 batou-2.3b6/src/batou/tests/fixture/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926785 batou-2.3b6/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901095 batou-2.3b6/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926956 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      178 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927152 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901327 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927333 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       79 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927514 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 ctheune    (501) staff       (20)      128 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927672 batou-2.3b6/src/batou/tests/fixture/component/
--rw-r--r--   0 ctheune    (501) staff       (20)       40 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927834 batou-2.3b6/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901649 batou-2.3b6/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928017 batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 ctheune    (501) staff       (20)      973 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.902583 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928214 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      144 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928528 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 ctheune    (501) staff       (20)       88 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928787 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      110 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929019 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929240 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 ctheune    (501) staff       (20)       90 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929459 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)      191 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929678 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 ctheune    (501) staff       (20)       94 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929900 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 ctheune    (501) staff       (20)       85 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930092 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 ctheune    (501) staff       (20)       64 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930285 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)       26 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930481 batou-2.3b6/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.902910 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930669 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      346 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930854 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)      116 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.903056 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931040 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       62 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931415 batou-2.3b6/src/batou/tests/fixture/template/
--rw-r--r--   0 ctheune    (501) staff       (20)       84 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      119 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 ctheune    (501) staff       (20)    18479 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_component.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4771 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_config.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_dependencies.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1725 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9419 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_endtoend.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8674 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2305 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_exceptions.py
--rw-r--r--   0 ctheune    (501) staff       (20)      606 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_host.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1488 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_main.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1326 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_remote.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9398 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3648 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)      743 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_resources.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2602 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_template.py
--rw-r--r--   0 ctheune    (501) staff       (20)    13871 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1169 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_vfs.py
--rw-r--r--   0 ctheune    (501) staff       (20)    16103 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/version.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1009 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/vfs.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914246 batou-2.3b6/src/batou.egg-info/
--rw-r--r--   0 ctheune    (501) staff       (20)     3445 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     6667 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      361 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/requires.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249645 batou-2.4a1/
+-rw-r--r--   0 elikoga    (501) staff       (20)    31241 2023-06-27 10:23:47.000000 batou-2.4a1/CHANGES.history.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1608 2023-06-27 10:23:47.000000 batou-2.4a1/LICENSE.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      212 2023-06-27 10:23:47.000000 batou-2.4a1/MANIFEST.in
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:48.249710 batou-2.4a1/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     2636 2023-06-27 10:23:47.000000 batou-2.4a1/README.md
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.222552 batou-2.4a1/doc/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228299 batou-2.4a1/doc/source/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228745 batou-2.4a1/doc/source/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      886 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/component.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1717 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/environment.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       48 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/templates.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       63 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/utilities.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228850 batou-2.4a1/doc/source/cli/
+-rw-r--r--   0 elikoga    (501) staff       (20)     4211 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/cli/index.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.229392 batou-2.4a1/doc/source/components/
+-rw-r--r--   0 elikoga    (501) staff       (20)     1025 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/cmmi.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2941 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     5657 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/files.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4820 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/python.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3050 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/services.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.229847 batou-2.4a1/doc/source/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)      718 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/authors.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8555 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/contributing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1711 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/testing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2809 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/todo.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8488 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4799 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/upgrading.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230489 batou-2.4a1/doc/source/user/
+-rw-r--r--   0 elikoga    (501) staff       (20)    10870 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/advanced.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2565 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/install.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3848 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/installation-deb.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3798 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2907 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/intro.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)    47489 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/quickstart.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224177 batou-2.4a1/examples/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230728 batou-2.4a1/examples/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      349 2023-06-27 10:23:47.000000 batou-2.4a1/examples/api/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/api/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230831 batou-2.4a1/examples/django/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/django/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230943 batou-2.4a1/examples/durations/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/durations/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231047 batou-2.4a1/examples/errors/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/errors/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231149 batou-2.4a1/examples/errors2/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/errors2/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231257 batou-2.4a1/examples/ignores/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/ignores/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231362 batou-2.4a1/examples/largetempl/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/largetempl/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231477 batou-2.4a1/examples/package/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/package/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231582 batou-2.4a1/examples/sync_async/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/sync_async/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231687 batou-2.4a1/examples/tutorial-buildout/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231798 batou-2.4a1/examples/tutorial-component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231908 batou-2.4a1/examples/tutorial-helloworld/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232021 batou-2.4a1/examples/tutorial-parallelize/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232129 batou-2.4a1/examples/tutorial-provision-container/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232240 batou-2.4a1/examples/tutorial-secrets/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.223989 batou-2.4a1/examples/tutorial-secrets/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232360 batou-2.4a1/examples/tutorial-secrets/environments/age/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2431 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-secrets/environments/age/age_keys.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232474 batou-2.4a1/examples/vagrant/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/vagrant/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232588 batou-2.4a1/examples/vagrant-multi/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232694 batou-2.4a1/examples/venvs/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232801 batou-2.4a1/examples/venvs/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/venvs/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      129 2023-06-27 10:23:47.000000 batou-2.4a1/pyproject.toml
+-rw-r--r--   0 elikoga    (501) staff       (20)      275 2023-06-27 10:23:47.000000 batou-2.4a1/requirements-dev.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      139 2023-06-27 10:23:48.249930 batou-2.4a1/setup.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)     2187 2023-06-27 10:23:47.000000 batou-2.4a1/setup.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224422 batou-2.4a1/src/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.235088 batou-2.4a1/src/batou/
+-rw-r--r--   0 elikoga    (501) staff       (20)    21062 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      997 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/_output.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/agent.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      163 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/c.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    40510 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      795 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14630 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    20522 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1507 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/fixtures.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11006 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/host.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236056 batou-2.4a1/src/batou/init-template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       44 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/.hgignore
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224602 batou-2.4a1/src/batou/init-template/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236185 batou-2.4a1/src/batou/init-template/components/example/
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236306 batou-2.4a1/src/batou/init-template/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       66 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      411 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/insecure-private.key
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.238659 batou-2.4a1/src/batou/lib/
+-rw-r--r--   0 elikoga    (501) staff       (20)       29 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3983 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6457 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3297 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2211 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2524 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1224 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2286 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    22046 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6368 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      854 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/goceptnet.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1388 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/logrotate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4541 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3647 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2814 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/package.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8150 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/python.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.239663 batou-2.4a1/src/batou/lib/resources/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2120 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      244 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/crontab
+-rw-r--r--   0 elikoga    (501) staff       (20)      548 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/init.sh
+-rw-r--r--   0 elikoga    (501) staff       (20)      299 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      840 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      153 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      380 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      609 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 elikoga    (501) staff       (20)      932 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10273 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1172 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/svn.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.241720 batou-2.4a1/src/batou/lib/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3083 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3858 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1689 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3261 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2110 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      639 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2158 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    31505 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10383 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6165 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      121 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      847 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1165 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1693 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3106 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6247 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/main.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.241842 batou-2.4a1/src/batou/migrate/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3377 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.242578 batou-2.4a1/src/batou/migrate/migrations/
+-rw-r--r--   0 elikoga    (501) staff       (20)      389 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1775 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      874 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      790 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1282 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2400.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.242784 batou-2.4a1/src/batou/migrate/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4532 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    12756 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/provision.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11713 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11793 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6424 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/resources.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.243284 batou-2.4a1/src/batou/secrets/
+-rw-r--r--   0 elikoga    (501) staff       (20)    21705 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3872 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/edit.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    12486 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/encryption.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2695 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/manage.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.243775 batou-2.4a1/src/batou/secrets/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)       23 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1566 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2736 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2429 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/template.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246239 batou-2.4a1/src/batou/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      666 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3012 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.227122 batou-2.4a1/src/batou/tests/fixture/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246369 batou-2.4a1/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225530 batou-2.4a1/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246503 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      178 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246641 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225713 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246787 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       79 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246924 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 elikoga    (501) staff       (20)      128 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247058 batou-2.4a1/src/batou/tests/fixture/component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       40 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247196 batou-2.4a1/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225954 batou-2.4a1/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247343 batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 elikoga    (501) staff       (20)      973 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.226690 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247480 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      144 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247621 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 elikoga    (501) staff       (20)       88 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247767 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      110 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247907 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248037 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 elikoga    (501) staff       (20)       90 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248169 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)      191 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248305 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 elikoga    (501) staff       (20)       94 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248454 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 elikoga    (501) staff       (20)       85 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248597 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 elikoga    (501) staff       (20)       64 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248731 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)       26 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248860 batou-2.4a1/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.226940 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248995 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      346 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249130 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)      116 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.227053 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249262 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       62 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249513 batou-2.4a1/src/batou/tests/fixture/template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       84 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      119 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18479 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4776 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_config.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     5707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1725 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10550 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8674 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2305 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      606 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_host.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1488 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_main.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1326 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_remote.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     9398 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3648 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      743 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_resources.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2602 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_template.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14060 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1169 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_vfs.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18387 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/version.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1009 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/vfs.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.235937 batou-2.4a1/src/batou.egg-info/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     6796 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      241 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/requires.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.3b6/CHANGES.history.txt` & `batou-2.4a1/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/LICENSE.txt` & `batou-2.4a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/PKG-INFO` & `batou-2.4a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.3b6
+Version: 2.4a1
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -104,7 +105,9 @@
 * Run `./develop.sh` to create a local virtualenv with everything set up.
 * Run the test suite using: `bin/tox`
 * Build the documentation using: `cd doc; make`
 * Set up GPG for the examples with `export GNUPGHOME=<DIRECTORY OF BATOU HERE>/src/batou/secrets/tests/fixture/gnupg`
 ## Changelog
 
 See [CHANGES.md](./CHANGES.md).
+
+
```

### Comparing `batou-2.3b6/README.md` & `batou-2.4a1/README.md`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/api/component.txt` & `batou-2.4a1/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/api/environment.txt` & `batou-2.4a1/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/cli/index.txt` & `batou-2.4a1/doc/source/cli/index.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,20 @@
   usage: batou [-h] [-d] {deploy,secrets,init} ...
 
   batou v2.0b12: multi-(host|component|environment|version|platform) deployment
 
   positional arguments:
     {deploy,secrets,init}
       deploy              Deploy an environment.
-      secrets             Manage encrypted secret files. Relies on gpg being
-                          installed and configured correctly.
+      secrets             Manage encrypted secret files. Relies on age (or GPG)
+                          being installed and configured correctly.
+      migrate             Migrate the configuration to be compatible with the
+                          batou version used. Requires to commit the changes
+                          afterwards. Might show some additional upgrade steps
+                          which cannot be performed automatically.
 
   optional arguments:
     -h, --help            show this help message and exit
     -d, --debug           Enable debug mode. (default: False)
 
 
 batou deploy
@@ -46,14 +50,16 @@
                           Does not touch anything.
     -P, --predict-only    Only predict what updates would happen. Do not change
                           anything.
     -j JOBS, --jobs JOBS  Defines number of jobs running parallel to deploy. The
                           default results in a serial deployment of components.
                           Will override the environment settings for operational
                           flexibility.
+    --provision-rebuild   Rebuild provisioned resources from scratch. DANGER:
+                          this is potentially destructive.
 
 batou secrets edit
 ------------------
 
 .. code-block:: console
 
     usage: batou secrets edit [-h] [--editor EDITOR] environment
@@ -69,37 +75,37 @@
 batou secrets summary
 ---------------------
 
 Show an overview of which users have access to what encrypted secrets.
 
 .. code-block:: console
 
-    usage: batou secrets summary [-h]
+    usage: ./batou secrets summary [-h]
 
     optional arguments:
       -h, --help  show this help message and exit
 
 Example:
 
 .. code-block:: console
 
-  $ ./batou secrets summary
+    $ ./batou secrets summary
 
-  production
-     members
-      - alice@example.com
-     secret files
-      - secrets.yaml
-
-  tutorial
-     members
-      - alice@example.com
-      - bob@example.com
-     secret files
-      (none)
+    production
+      members
+        - alice@example.com
+      secret files
+        - secrets.yaml
+
+    tutorial
+      members
+        - alice@example.com
+        - bob@example.com
+      secret files
+        (none)
 
 
 batou secrets add
 -----------------
 
 .. code-block:: console
```

### Comparing `batou-2.3b6/doc/source/components/cmmi.txt` & `batou-2.4a1/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/components/downloads-vcs.txt` & `batou-2.4a1/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/components/files.txt` & `batou-2.4a1/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/components/python.txt` & `batou-2.4a1/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/components/services.txt` & `batou-2.4a1/doc/source/components/services.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/dev/authors.txt` & `batou-2.4a1/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/dev/contributing.txt` & `batou-2.4a1/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/dev/testing.txt` & `batou-2.4a1/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/dev/todo.txt` & `batou-2.4a1/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/index.txt` & `batou-2.4a1/doc/source/index.txt`

 * *Files 9% similar despite different names*

```diff
@@ -119,52 +119,52 @@
 * Use pre-defined components to manage files, python environments, supervisor, cronjobs, and more.
 * Writing your own components is easy and you can use additional Python
   package dependencies.
 
 User guide
 ----------
 
-This part of the documentation, begins with some background information about Requests, then focuses on step-by-step instructions for getting the most out of batou.
+This part of the documentation, begins with some background information about batou, then focuses on the basic parts needed on a regular basis when creating and maintaining increasingly complex deployments with batou. The last part of the narrative documentation covers selected topics in depth.
 
 .. toctree::
    :maxdepth: 2
 
    user/intro
    user/install
    user/quickstart
    user/advanced
 
-Command line
-------------
+Reference: Command line interface
+---------------------------------
 
 If you are looking for information on what commands the batou CLI provides then this is for you.
 
 .. toctree::
    :maxdepth: 2
 
    cli/index
 
 
-Components
-----------
+Reference: Component Library
+----------------------------
 
 This is the list of components that batou provides -- builtin and through the `batou_ext` package:
 
 .. toctree::
    :maxdepth: 2
 
    components/files.txt
    components/downloads-vcs.txt
    components/cmmi.txt
    components/python.txt
    components/services.txt
 
 
-API
----
+Reference: Python API
+---------------------
 
 If you are looking for information on a specific function, class or method, this part of the documentation is for you.
 
 .. toctree::
    :maxdepth: 2
 
    api/component
@@ -186,16 +186,18 @@
    dev/testing
    dev/todo
    dev/authors
 
 Support
 -------
 
-batou itself is released "as is". We hang around #batou in the Freenode IRC
-network. You can also report bugs to our `bugtracker <http://plan.flyingcircus.io/projects/batou>`_.
+batou itself is released "as is".
+You can also report bugs to our `bugtracker <https://github.com/flyingcircusio/batou/issues>`_.
+
+We also have a matrix channel: `#batou:matrix.org <https://matrix.to/#/#batou:matrix.org>`_.
 
 .. rubric:: Commercial support
 
 We will be happy to give you commercial support for batou: feature
 implementation, bug fixing, consulting, or education.
 
 To get in touch, send an email to `mail@flyingcircus.io
```

### Comparing `batou-2.3b6/doc/source/upgrading.txt` & `batou-2.4a1/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/user/advanced.txt` & `batou-2.4a1/doc/source/user/advanced.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Advanced Usage
-==============
+In-depth topics
+===============
 
 
 Writing a custom component (TODO)
 ---------------------------------
 
 Debugging batou runs
 --------------------
```

### Comparing `batou-2.3b6/doc/source/user/install.txt` & `batou-2.4a1/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/user/installation-deb.txt` & `batou-2.4a1/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/user/installation-rpm.txt` & `batou-2.4a1/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/user/intro.txt` & `batou-2.4a1/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/doc/source/user/quickstart.txt` & `batou-2.4a1/doc/source/user/quickstart.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Quickstart
-==========
+Foundations for creating and maintaining deployments
+====================================================
 
-Do you want to get started? We'll go through the steps of developing a project
+Do you want to get started? We'll go through the steps of developing a deployment
 with batou. The steps are built on top of each other, so if you have trouble
 with a specific step, it might help to review what happened earlier.
 
 Create a new project
 --------------------
 
 Deployments with batou are placed in a new directory. For this tutorial
```

### Comparing `batou-2.3b6/setup.py` & `batou-2.4a1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,18 +35,14 @@
         ]
     },
     entry_points="""
         [console_scripts]
             batou = batou.main:main
         [zc.buildout]
             requirements = batou.buildout:Requirements
-        [zest.releaser.prereleaser.after]
-            update_requirements = batou.release:update_requirements
-        [zest.releaser.postreleaser.after]
-            update_requirements = batou.release:update_requirements
         [batou.provisioners]
             fc-nixos-dev-container = batou.provision:FCDevContainer
     """,
     author="Christian Theune",
     author_email="ct@flyingcircus.io",
     license="BSD (2-clause)",
     url="https://batou.readthedocs.io/en/latest/",
```

### Comparing `batou-2.3b6/src/batou/__init__.py` & `batou-2.4a1/src/batou/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This code must not cause non-stdlib imports to support self-bootstrapping.
 import os
 import os.path
 import traceback
+from typing import List, Optional
 
 from ._output import output
 
 with open(os.path.dirname(__file__) + "/version.txt") as f:
     __version__ = f.read().strip()
 
 # Configure `remote-pdb` to be used with `breakpoint()` in Python 3.7+:
@@ -15,14 +16,16 @@
 if not os.environ.get("REMOTE_PDB_PORT", None):
     os.environ["REMOTE_PDB_PORT"] = "4444"
 
 
 class ReportingException(Exception):
     """Exceptions that support user-readable reporting."""
 
+    affected_hostname: Optional[str]
+
     def __str__(self):
         raise NotImplementedError()
 
     def report(self):
         raise NotImplementedError()
 
     def should_merge(self, other):
@@ -60,14 +63,16 @@
         new_exception.affected_hostname = "<HOSTNAME>"
         return (new_exception, hostnames)
 
 
 class FileLockedError(ReportingException):
     """A file is already locked and we do not want to block."""
 
+    filename: str
+
     @classmethod
     def from_context(cls, filename):
         self = cls()
         self.filename = filename
         return self
 
     def __str__(self):
@@ -76,14 +81,18 @@
     def report(self):
         output.error(str(self))
 
 
 class GPGCallError(ReportingException):
     """There was an error calling GPG on encrypted file."""
 
+    command: str
+    exitcode: str
+    output: str
+
     @classmethod
     def from_context(cls, command, exitcode, output):
         self = cls()
         self.command = " ".join(command)
         self.exitcode = str(exitcode)
         self.output = output.decode("ascii", errors="replace")
         return self
@@ -97,21 +106,53 @@
     def report(self):
         output.error("Error while calling GPG")
         output.tabular("command", self.command, red=True)
         output.tabular("exit code", self.exitcode)
         output.tabular("message", self.output, separator=":\n")
 
 
+class AgeCallError(ReportingException):
+    """There was an error calling age on encrypted file."""
+
+    command: str
+    exitcode: str
+    output: str
+
+    @classmethod
+    def from_context(cls, command, exitcode, output):
+        self = cls()
+        self.command = " ".join(command)
+        self.exitcode = str(exitcode)
+        self.output = output.decode("ascii", errors="replace")
+        return self
+
+    def __str__(self):
+        return (
+            f"Exitcode {self.exitcode} while calling: "
+            f"{self.command}\n{self.output}"
+        )
+
+    def report(self):
+        output.error("Error while calling age")
+        output.tabular("command", self.command, red=True)
+        output.tabular("exit code", self.exitcode)
+        output.tabular("message", self.output, separator=":\n")
+
+
 class UpdateNeeded(AssertionError):
     """A component requires an update."""
 
 
 class ConfigurationError(ReportingException):
     """Indicates that an environment could not be configured successfully."""
 
+    message: str
+    has_component: bool
+    component_root_name: Optional[str]
+
     @property
     def sort_key(self):
         return (0, self.message)
 
     @classmethod
     def from_context(cls, message, component=None):
         self = cls()
@@ -133,14 +174,20 @@
             )
         output.error(message)
 
 
 class ConversionError(ConfigurationError):
     """An override attribute could not be converted properly."""
 
+    component_breadcrumbs: str
+    conversion_name: str
+    value_repr: str
+    error_str: str
+    key: str
+
     @property
     def sort_key(self):
         return (
             1,
             self.affected_hostname,
             self.component_breadcrumbs,
             self.key,
@@ -183,14 +230,18 @@
     They basically only influence control flow during configuration and
     are manually placed to avoid double reporting.
 
     """
 
 
 class MissingOverrideAttributes(ConfigurationError):
+
+    component_breadcrumbs: str
+    attributes: List[str]
+
     @property
     def sort_key(self):
         return (3, self.affected_hostname, self.component_breadcrumbs)
 
     @classmethod
     def from_context(cls, component, attributes):
         self = cls()
@@ -208,14 +259,18 @@
         output.tabular("Attributes", ", ".join(self.attributes), red=True)
 
         # TODO point to specific line in secrets or environments
         # cfg file and show context
 
 
 class DuplicateComponent(ConfigurationError):
+    a_name: str
+    a_filename: str
+    b_filename: str
+
     @property
     def sort_key(self):
         return (2, self.a_name)
 
     @classmethod
     def from_context(cls, a, b):
         self = cls()
@@ -230,14 +285,18 @@
     def report(self):
         output.error('Duplicate component "{}"'.format(self.a_name))
         output.tabular("Occurrence", self.a_filename)
         output.tabular("Occurrence", self.b_filename)
 
 
 class DuplicateHostMapping(ConfigurationError):
+    affected_hostname: str
+    a: str
+    b: str
+
     @property
     def sort_key(self):
         return (3, self.affected_hostname, self.a, self.b)
 
     @classmethod
     def from_context(cls, hostname, a, b):
         self = cls()
@@ -310,15 +369,15 @@
 
     sort_key = (5, "unused")
 
     @classmethod
     def from_context(cls, resources):
         self = cls()
         self.unused_resources = []
-        for key in sorted(resources):
+        for key in sorted(resources.keys()):
             for component, value in resources[key].items():
                 self.unused_resources.append((key, component.name, str(value)))
         return self
 
     def __str__(self):
         return "Unused provided resources"
 
@@ -338,15 +397,15 @@
 
     sort_key = (6, "unsatisfied")
 
     @classmethod
     def from_context(cls, resources):
         self = cls()
         self.unsatisfied_resources = []
-        for key in sorted(resources):
+        for key in sorted(resources.keys()):
             self.unsatisfied_resources.append(
                 (key, [r.name for r in resources[key]])
             )
         return self
 
     def __str__(self):
         return "Unsatisfied resource requirements"
@@ -549,27 +608,29 @@
 
     sort_key = (100,)
 
     @classmethod
     def from_context(cls, roots):
         self = cls()
         self.roots_len = len(roots)
+        self.root_names = ", ".join(sorted([r.name for r in roots]))
         return self
 
     def __str__(self):
         return "There are unconfigured components remaining."
 
     def report(self):
         # TODO show this last or first, but not in the middle
         # of everything
         output.error(
-            "{} remaining unconfigured component(s)".format(self.roots_len)
+            "{} remaining unconfigured component(s): {}".format(
+                self.roots_len, self.root_names
+            )
         )
         # TODO show all incl. their host name in -vv or so
-        # output.annotate(', '.join(c.name for c in self.roots))
 
 
 class DeploymentError(ReportingException):
     """Indicates that a deployment failed.."""
 
     sort_key = (100,)
```

### Comparing `batou-2.3b6/src/batou/_output.py` & `batou-2.4a1/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/component.py` & `batou-2.4a1/src/batou/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     #: (*readonly*) The workdir attribute is set by batou when a component
     #: before a component is configured and defaults to
     #: ``<root>/work/<componentname>``. Built-in components treat all relative
     #: destination paths as relative to the work directory.
     #:
     #: During verify() and apply() batou automatically switches the current
     #: working directory to this.
-    workdir = None
+    workdir: str = None
 
     @property
     def defdir(self):
         """(*readonly*) The definition directory
            (where the ``component.py`` lives).
 
         Built-in components treat all path names of source files as relative
@@ -184,14 +184,15 @@
     #: sub-component.
     _ = None
 
     changed = False
     _prepared = False
 
     def __init__(self, namevar=None, **kw):
+        self.timer = batou.utils.Timer(self.__class__.__name__)
         # Are any keyword arguments undefined attributes?
         # This is a somewhat rough implementation as it allows overriding
         # methods
         unacceptable_args = set()
         missing_attribute = object()
         for k in kw:
             attr = getattr(self.__class__, k, missing_attribute)
@@ -320,44 +321,51 @@
     def deploy(self, predict_only=False):
         # Remember: this is a tight loop - we need to keep this code fast.
 
         # Reset changed flag here to support triggering deploy() multiple
         # times. This is mostly helpful for testing, but who knows.
         self.changed = False
         for sub_component in self.sub_components:
-            sub_component.deploy(predict_only)
+            with self.timer.step("sub"):
+                sub_component.deploy(predict_only)
             if sub_component.changed:
                 self.changed = True
 
         output.buffer("annotate", self.host.name + " > " + self._breadcrumbs)
 
         if not os.path.exists(self.workdir):
             os.makedirs(self.workdir)
         with self.chdir(self.workdir), self:
             require_update = False
             try:
-                with batou.utils.Timer("{} verify()".format(self._breadcrumbs)):
+                with self.timer.step("verify"):
                     call_with_optional_args(
                         self.verify, predicting=predict_only
                     )
             except AssertionError:
                 # avoid nested exception messages, when running `update()` in except block
                 require_update = True
 
             if require_update:
                 self.__trigger_event__(
                     "before-update", predict_only=predict_only
                 )
                 output.flush_buffer()
                 if not predict_only:
-                    self.update()
+                    with self.timer.step("update"):
+                        self.update()
                 self.changed = True
 
         output.clear_buffer()
 
+        if self.timer.above_threshold(verify=1, update=1, total=10):
+            output.annotate(
+                f"{self.host.name} > {self._breadcrumbs} [{self.timer.humanize('total', 'verify', 'update', 'sub')}]"
+            )
+
     def verify(self):
         """Verify whether this component has been deployed correctly or needs
         to be updated.
 
         Raise the :py:class:`batou.UpdateNeeded` exception if the desired
         target state is not reached. Use the :py:meth:`assert_*` methods (see
         below) to check for typical conditions and raise this exception
```

### Comparing `batou-2.3b6/src/batou/deploy.py` & `batou-2.4a1/src/batou/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
 from batou import ReportingException, SilentConfigurationError
 from batou._output import TerminalBackend, output
 
 from .environment import Environment
-from .utils import locked, notify, self_id
+from .utils import Timer, locked, notify, self_id
 
 
 class Connector(threading.Thread):
     def __init__(self, host, sem):
         self.host = host
         self.sem = sem
         self.exc_info = None
@@ -117,14 +117,16 @@
         )
         self.environment.deployment = self
 
         self.dirty = dirty
         self.predict_only = predict_only
         self.jobs = jobs
 
+        self.timer = Timer("deployment")
+
     def load(self):
         output.section("Preparing")
 
         output.step(
             "main", "Loading environment `{}`...".format(self.environment.name)
         )
         self.environment.load()
@@ -188,16 +190,17 @@
             c.start()
             yield c
 
     def connect(self):
         output.section("Connecting hosts and configuring model ...")
         # Consume the connection iterator to start all remaining connections
         # but do not wait for them to be joined.
-        self.connections = list(self._connections())
-        [c.join() for c in self.connections]
+        with self.timer.step("connect"):
+            self.connections = list(self._connections())
+            [c.join() for c in self.connections]
         all_errors = []
         all_reporting_hostnames = set()
         for c in self.connections:
             errors = pickle.loads(c.errors)
             reporting_hostname = c.host.name
             all_reporting_hostnames.add(reporting_hostname)
             all_errors.extend([(reporting_hostname, e) for e in errors])
@@ -280,47 +283,51 @@
 
     def deploy(self):
         if self.predict_only:
             output.section("Predicting deployment actions")
         else:
             output.section("Deploying")
 
-        # Pick a reference remote (the last we initialised) that will pass us
-        # the order we should be deploying components in.
-        reference_node = [
-            h for h in list(self.environment.hosts.values()) if not h.ignore
-        ][0]
-
-        self.loop = asyncio.get_event_loop()
-        self.taskpool = ThreadPoolExecutor(self.jobs)
-        self.loop.set_default_executor(self.taskpool)
-        self._launch_components(reference_node.root_dependencies())
-
-        # asyncio.Task.all_tasks was removed in Python 3.9
-        # but the replacement asyncio.all_tasks is only available
-        # for Python 3.7 and upwards
-        # confer https://docs.python.org/3/whatsnew/3.7.html
-        # and https://docs.python.org/3.9/whatsnew/3.9.html
-        if sys.version_info < (3, 7):
-            all_tasks = asyncio.Task.all_tasks
-        else:
-            all_tasks = asyncio.all_tasks
+        with self.timer.step("deploy"):
+            # Pick a reference remote (the last we initialised) that will pass us
+            # the order we should be deploying components in.
+            reference_node = [
+                h for h in list(self.environment.hosts.values()) if not h.ignore
+            ][0]
+
+            self.loop = asyncio.get_event_loop()
+            self.taskpool = ThreadPoolExecutor(self.jobs)
+            self.loop.set_default_executor(self.taskpool)
+            self._launch_components(reference_node.root_dependencies())
+
+            # asyncio.Task.all_tasks was removed in Python 3.9
+            # but the replacement asyncio.all_tasks is only available
+            # for Python 3.7 and upwards
+            # confer https://docs.python.org/3/whatsnew/3.7.html
+            # and https://docs.python.org/3.9/whatsnew/3.9.html
+            if sys.version_info < (3, 7):
+                all_tasks = asyncio.Task.all_tasks
+            else:
+                all_tasks = asyncio.all_tasks
 
-        def get_pending():
-            return {t for t in all_tasks(self.loop) if not t.done()}
+            def get_pending():
+                return {t for t in all_tasks(self.loop) if not t.done()}
 
-        pending = get_pending()
-        while pending:
-            self.loop.run_until_complete(asyncio.gather(*pending))
             pending = get_pending()
+            while pending:
+                self.loop.run_until_complete(asyncio.gather(*pending))
+                pending = get_pending()
 
     def summarize(self):
         output.section("Summary")
         for node in list(self.environment.hosts.values()):
             node.summarize()
+        output.annotate(
+            f"Deployment took {self.timer.humanize('total', 'connect', 'deploy')}"
+        )
 
     def disconnect(self):
         output.step("main", "Disconnecting from nodes ...", debug=True)
         for node in list(self.environment.hosts.values()):
             node.disconnect()
```

### Comparing `batou-2.3b6/src/batou/environment.py` & `batou-2.4a1/src/batou/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import glob
 import json
 import os
 import os.path
 import pathlib
 import sys
 from configparser import RawConfigParser
+from typing import Dict, List, Set
 
 from importlib_metadata import entry_points
 
 import batou.c
 import batou.utils
 import batou.vfs
 from batou import (
@@ -26,22 +27,23 @@
     SuperfluousComponentSection,
     SuperfluousSection,
     UnknownComponentConfigurationError,
     UnsatisfiedResources,
     UnusedResources,
 )
 from batou._output import output
-from batou.component import RootComponent
+from batou.component import ComponentDefinition, RootComponent
+from batou.provision import Provisioner
 from batou.repository import Repository
 from batou.utils import CycleError, cmd
 
 from .component import load_components_from_file
 from .host import Host, LocalHost, RemoteHost
 from .resources import Resources
-from .secrets import add_secrets_to_environment
+from .secrets import SecretProvider
 
 
 class ConfigSection(dict):
     def as_list(self, option):
         result = self[option]
         if "," in result:
             result = [x.strip() for x in result.split(",")]
@@ -52,15 +54,15 @@
             result = [result]
         return result
 
 
 class Config(object):
     def __init__(self, path):
         config = RawConfigParser()
-        config.optionxform = lambda s: s
+        config.optionxform = lambda optionstr: optionstr
         if path:  # Test support
             config.read(path)
         self.config = config
 
     def __contains__(self, section):
         return self.config.has_section(section)
 
@@ -112,39 +114,55 @@
         self,
         name,
         timeout=None,
         platform=None,
         basedir=".",
         provision_rebuild=False,
     ):
-        self.name = name
-        self.hosts = {}
+        self.name: str = name
+        self.hosts: Dict[str, Host] = {}
         self.resources = Resources()
-        self.overrides = {}
-        self.secret_data = set()
-        self.exceptions = []
+        self.overrides: Dict[str, Dict[str, str]] = {}
+        self.secret_data: Set[str] = set()
+        self.exceptions: List[Exception] = []
         self.timeout = timeout
         self.platform = platform
         self.provision_rebuild = provision_rebuild
 
-        self.hostname_mapping = {}
+        self.hostname_mapping: Dict[str, str] = {}
 
         # These are the component classes, decorated with their
         # name.
-        self.components = {}
+        self.components: Dict[str, "ComponentDefinition"] = {}
         # These are the components assigned to hosts.
-        self.root_components = []
+        self.root_components: List[RootComponent] = []
 
         self.base_dir = os.path.abspath(basedir)
         self.workdir_base = os.path.join(self.base_dir, "work")
 
         # Additional secrets files as placed in secrets/<env>-<name>
-        self.secret_files = {}
+        self.secret_files: Dict[str, str] = {}
 
-        self.provisioners = {}
+        self.provisioners: Dict[str, Provisioner] = {}
+
+    @classmethod
+    def all(cls):
+        for path in pathlib.Path("environments").glob("*/environment.cfg"):
+            yield cls(path.parent.name)
+
+    @classmethod
+    def filter(cls, names):
+        if not names:
+            return cls.all()
+        names = names.split(",")
+        names = [x.strip() for x in names]
+
+        for env in cls.all():
+            if env.name in names:
+                yield env
 
     def _environment_path(self, path="."):
         return os.path.abspath(
             os.path.join(self.base_dir, "environments", self.name, path)
         )
 
     def _ensure_environment_dir(self):
@@ -222,15 +240,16 @@
             self.target_directory = self.repository.root
 
         self.deployment_base = os.path.relpath(
             self.base_dir, self.repository.root
         )
 
     def load_secrets(self):
-        add_secrets_to_environment(self)
+        self.secret_provider = SecretProvider.from_environment(self)
+        self.secret_provider.inject_secrets()
 
     def load_environment(self, config):
         environment = config.get("environment", {})
         for key in [
             "service_user",
             "host_domain",
             "target_directory",
@@ -505,17 +524,23 @@
                 if self.resources.unsatisfied:
                     exceptions.append(
                         UnsatisfiedResources.from_context(
                             self.resources.unsatisfied_keys_and_components
                         )
                     )
 
+                cycle_start = previous_working_sets.index(retry)
+                # consider all components tried during they cycle as unconfigured
+                unconfigured = set().union(*previous_working_sets[cycle_start:])
+
                 # We did not manage to improve on our last working set, so we
                 # give up.
-                exceptions.append(NonConvergingWorkingSet.from_context(retry))
+                exceptions.append(
+                    NonConvergingWorkingSet.from_context(unconfigured)
+                )
                 break
 
             working_set = retry
 
         # We managed to converge on a working set. However, some resource were
         # provided but never used. We're rather picky here and report this as
         # an error.
```

### Comparing `batou-2.3b6/src/batou/fixtures.py` & `batou-2.4a1/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/host.py` & `batou-2.4a1/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/appenv.py` & `batou-2.4a1/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/archive.py` & `batou-2.4a1/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/buildout.py` & `batou-2.4a1/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/cmmi.py` & `batou-2.4a1/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/cron.py` & `batou-2.4a1/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/debian.py` & `batou-2.4a1/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/download.py` & `batou-2.4a1/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/file.py` & `batou-2.4a1/src/batou/lib/file.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/git.py` & `batou-2.4a1/src/batou/lib/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,33 @@
     if not os.path.isdir(path):
         ensure_path_nonexistent(path)
         os.makedirs(path)
     for file in os.listdir(path):
         ensure_path_nonexistent(os.path.join(path, file))
 
 
+def exactly_one(*args):
+    return sum(map(bool, args)) == 1
+
+
 class Clone(Component):
 
     namevar = "url"
     target = "."
     revision = None
     branch = None
+    tag = None
     vcs_update = True
     clobber = False
 
     def configure(self):
-        if (not self.revision_or_branch) or (self.revision and self.branch):
+        if not exactly_one(self.revision, self.branch, self.tag):
             raise ValueError(
-                "Clone(%s) needs exactly one of revision or branch" % self.url
+                "Clone(%s) needs exactly one of revision, branch or tag"
+                % self.url
             )
         self.target = self.map(self.target)
         self += Directory(self.target)
 
     def verify(self):
         self._force_clone = False
         if not os.path.exists(self.target):
@@ -88,18 +94,26 @@
             if self.revision and self.current_revision() != self.revision:
                 raise UpdateNeeded()
             if self.branch and (
                 self.current_branch() != self.branch
                 or self.has_incoming_changesets()
             ):
                 raise UpdateNeeded()
+            if self.tag and (
+                self.current_tag() != self.tag or self.has_incoming_changesets()
+            ):
+                raise UpdateNeeded()
 
-    @property
-    def revision_or_branch(self):
-        return self.revision or self.branch
+    def current_tag(self):
+        try:
+            with self.chdir(self.target):
+                stdout, stderr = self.cmd("LANG=C git describe --tags")
+        except RuntimeError:
+            return None
+        return stdout.strip()
 
     def current_revision(self):
         try:
             with self.chdir(self.target):
                 stdout, stderr = self.cmd("LANG=C git show -s --format=%H")
         except RuntimeError:
             return None
@@ -143,14 +157,17 @@
                 os.unlink(os.path.join(self.target, filepath))
             if not just_cloned:
                 self.cmd("git fetch")
             if self.branch:
                 self.cmd(
                     self.expand("git reset --hard origin/{{component.branch}}")
                 )
+            elif self.tag:
+                self.cmd(self.expand("git fetch --tags"))
+                self.cmd(self.expand("git reset --hard {{component.tag}}"))
             else:
                 self.cmd(self.expand("git reset --hard {{component.revision}}"))
 
             # XXX We should re-think submodule support; e.g. which revision
             # shall the submodules be updated to?
             self.cmd("git submodule update --init --recursive")
```

### Comparing `batou-2.3b6/src/batou/lib/goceptnet.py` & `batou-2.4a1/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/logrotate.py` & `batou-2.4a1/src/batou/lib/logrotate.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/mercurial.py` & `batou-2.4a1/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/mysql.py` & `batou-2.4a1/src/batou/lib/mysql.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/nagios.py` & `batou-2.4a1/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/package.py` & `batou-2.4a1/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/python.py` & `batou-2.4a1/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.4a1/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/resources/init.sh` & `batou-2.4a1/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/resources/nagios.cfg` & `batou-2.4a1/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/resources/supervisor.conf` & `batou-2.4a1/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/service.py` & `batou-2.4a1/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/supervisor.py` & `batou-2.4a1/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/svn.py` & `batou-2.4a1/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_appenv.py` & `batou-2.4a1/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_archive.py` & `batou-2.4a1/src/batou/lib/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_buildout.py` & `batou-2.4a1/src/batou/lib/tests/test_buildout.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,38 +35,14 @@
     assert b.cmd.call_count == 1
     calls = iter(x[1][0] for x in b.cmd.mock_calls)
     assert next(calls) == 'bin/buildout -t 40 -c "buildout.cfg"'
 
 
 @pytest.mark.slow
 @pytest.mark.timeout(60)
-def test_runs_buildout_successfully(root):
-    b = Buildout(
-        python="2.7",
-        version="2.13.4",
-        setuptools="44.1.1",
-        config=File(
-            "buildout.cfg",
-            source=pkg_resources.resource_filename(
-                __name__, "buildout-example.cfg"
-            ),
-        ),
-    )
-    root.component += b
-    root.component.deploy()
-    assert os.path.isdir(
-        os.path.join(root.environment.workdir_base, "mycomponent/parts")
-    )
-    assert os.path.isfile(
-        os.path.join(root.environment.workdir_base, "mycomponent/bin/py")
-    )
-
-
-@pytest.mark.slow
-@pytest.mark.timeout(60)
 def test_runs_buildout3_successfully(root, output):
     b = Buildout(
         python="3",
         version="3.0.0b1",
         setuptools="54.1.1",
         wheel="0.36.2",
         pip="21.0.1",
```

### Comparing `batou-2.3b6/src/batou/lib/tests/test_cmmi.py` & `batou-2.4a1/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_cron.py` & `batou-2.4a1/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_debian.py` & `batou-2.4a1/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_download.py` & `batou-2.4a1/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_file.py` & `batou-2.4a1/src/batou/lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_git.py` & `batou-2.4a1/src/batou/lib/tests/test_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,40 @@
             workdir=root.workdir
         )
     )
     assert "bar" == stdout.strip()
 
 
 @pytest.mark.slow
+def test_tag_does_switch_tag(root, repos_path):
+    cmd(
+        """cd {dir}; git tag -a v1.0 -m "version 1.0" """.format(dir=repos_path)
+    )
+    cmd(
+        "cd {dir}; touch bar; git add .;"
+        'git commit -m "commit branch"'.format(dir=repos_path)
+    )
+    cmd(
+        """cd {dir}; git tag -a v1.1 -m "version 1.1" """.format(dir=repos_path)
+    )
+
+    for tag in ("v1.0", "v1.1"):
+        root.component += batou.lib.git.Clone(
+            repos_path, target="clone", tag=tag
+        )
+        root.component.deploy()
+        stdout, stderr = cmd(
+            "cd {workdir}/clone; git describe --tags".format(
+                workdir=root.workdir
+            )
+        )
+        assert tag == stdout.strip()
+
+
+@pytest.mark.slow
 def test_has_changes_counts_changes_to_tracked_files(root, repos_path):
     clone = batou.lib.git.Clone(repos_path, target="clone", branch="master")
     root.component += clone
     root.component.deploy()
     assert not clone.has_changes()
     cmd("touch {}/clone/bar".format(root.workdir))
     cmd("cd {}/clone; git add bar".format(root.workdir))
```

### Comparing `batou-2.3b6/src/batou/lib/tests/test_mercurial.py` & `batou-2.4a1/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_nagios.py` & `batou-2.4a1/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_python.py` & `batou-2.4a1/src/batou/lib/tests/test_python.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     class Playground(Component):
         namevar = "version"
 
         def configure(self):
             self.venv = VirtualEnv(self.version)
             self += self.venv
 
-    playground = Playground("2.7")
+    playground = Playground("3.7")
     root.component += playground
     playground.deploy()
     root.component.sub_components.remove(playground)
 
-    playground = Playground("3")
+    playground = Playground("3.8")
     root.component += playground
     playground.deploy()
 
     out, err = playground.cmd(
         '{}/bin/python -c "import sys; print(sys.version_info[:2])"'.format(
             playground.workdir
         )
@@ -33,13 +33,13 @@
     class Playground(Component):
         namevar = "version"
 
         def configure(self):
             self.venv = VirtualEnv(self.version)
             self += self.venv
 
-    playground = Playground("2.7")
+    playground = Playground("3.7")
     root.component += playground
     playground.deploy()
     assert playground.changed
     playground.deploy()
     assert not playground.changed
```

### Comparing `batou-2.3b6/src/batou/lib/tests/test_service.py` & `batou-2.4a1/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_supervisor.py` & `batou-2.4a1/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/lib/tests/test_svn.py` & `batou-2.4a1/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/main.py` & `batou-2.4a1/src/batou/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     p.set_defaults(func=batou.deploy.main)
 
     # SECRETS
     secrets = subparsers.add_parser(
         "secrets",
         help=textwrap.dedent(
             """
-            Manage encrypted secret files. Relies on GPG being installed and
+            Manage encrypted secret files. Relies on age (or GPG) being installed and
             configured correctly. """
         ),
     )
     secrets.set_defaults(func=secrets.print_usage)
 
     sp = secrets.add_subparsers()
 
@@ -187,14 +187,15 @@
     migrate.set_defaults(func=batou.migrate.main)
 
     args = parser.parse_args(args)
 
     # Consume global arguments
     batou.output.enable_debug = args.debug
     batou.secrets.encryption.debug = args.debug
+    batou.secrets.manage.debug = args.debug
 
     # Pass over to function
     if args.func.__name__ == "print_usage":
         args.func()
         sys.exit(1)
 
     if args.func != batou.migrate.main:
@@ -204,8 +205,8 @@
     func_args = dict(args._get_kwargs())
     del func_args["func"]
     del func_args["debug"]
     try:
         return args.func(**func_args)
     except batou.FileLockedError as e:
         # Nicer error reporting for non-deployment commands.
-        print("File already locked: {}".format(e.filename))
+        print(e)
```

### Comparing `batou-2.3b6/src/batou/migrate/__init__.py` & `batou-2.4a1/src/batou/migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/migrate/migrations/2301.py` & `batou-2.4a1/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/migrate/migrations/2302.py` & `batou-2.4a1/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/migrate/migrations/2303.py` & `batou-2.4a1/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/migrate/tests/test_migrate.py` & `batou-2.4a1/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/provision.py` & `batou-2.4a1/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/remote_core.py` & `batou-2.4a1/src/batou/remote_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     output = Output(ChannelBackend(channel))
     while not channel.isclosed():
         task, args, kw = channel.receive()
         # Support slow bootstrapping
         try:
             import batou
         except ImportError:
-            batou = None
+            pass
         try:
             result = locals()[task](*args, **kw)
             channel.send(("batou-result", result))
         except Exception as e:
             # I voted for duck-typing here as we may be running in the
             # bootstrapping phase and don't have access to all classes yet.
             if hasattr(e, "report"):
```

### Comparing `batou-2.3b6/src/batou/repository.py` & `batou-2.4a1/src/batou/repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/resources.py` & `batou-2.4a1/src/batou/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict
+from typing import Set
 
 from batou.utils import flatten
 
 
 class Subscription(object):
 
     # Dirty on the subscription means: I am OK to be dirty and _not_
@@ -45,15 +46,15 @@
     # "provide before require"
 
     # {key: [(root, strict, host, reverse),
     #        (root, strict, host, reverse), ...]}
     subscribers = None
     # Keeps track of root components that have not seen changes to a key they
     # have subscribed to when they were configured earlier..
-    dirty_dependencies = None
+    dirty_dependencies: Set
 
     # {key: {root: [values]}}
     resources = None
 
     def __init__(self):
         self.resources = {}
         self.subscribers = {}
```

### Comparing `batou-2.3b6/src/batou/secrets/manage.py` & `batou-2.4a1/src/batou/secrets/edit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,129 @@
-"""Summarize status of secret files."""
-
+"""Securely edit encrypted secret files."""
+import os
 import pathlib
+import subprocess
 import sys
+import tempfile
+import traceback
+from typing import Optional
+
+from batou.environment import Environment
+
+from .encryption import debug
+
+NEW_FILE_TEMPLATE = """\
+[batou]
+secret_provider = age
+members =
+"""
+
+
+class Editor(object):
+    def __init__(
+        self,
+        editor_cmd,
+        environment: Environment,
+        edit_file: Optional[str] = None,
+    ):
+        environment.load_secrets()
+        self.editor_cmd = editor_cmd
+        self.environment = environment
+        self.edit_file = edit_file
+        self.file = self.environment.secret_provider.edit(edit_file)
+
+    def main(self):
+        with self.file:
+            self.original_cleartext = self.file.cleartext
+            self.cleartext = self.original_cleartext
+            if self.file.is_new:
+                self.original_cleartext = None
+                if self.edit_file:
+                    self.cleartext = ""
+                else:
+                    self.cleartext = NEW_FILE_TEMPLATE
 
-from batou import GPGCallError
+            self.interact()
 
-from .encryption import EncryptedConfigFile
+    def _input(self):
+        return input("> ").strip()
 
+    def interact(self):
+        cmd = "edit"
+        while cmd != "quit":
+            try:
+                self.process_cmd(cmd)
+            except Exception as e:
+                print()
+                print()
+                print(f"An error occurred: {e}")
+                print()
+                print("Your changes are still available. You can try:")
+                print("\tedit       -- opens editor with current data again")
+                print("\tencrypt    -- tries to encrypt current data again")
+                print("\tquit       -- quits and loses your changes")
+                cmd = self._input()
+            else:
+                break
+
+    def process_cmd(self, cmd):
+        if cmd == "edit":
+            self.edit()
+            self.encrypt()
+        elif cmd == "encrypt":
+            self.encrypt()
+        elif cmd == "":
+            raise ValueError("empty command")
+        else:
+            raise ValueError("unknown command `{}`".format(cmd))
 
-class UnknownEnvironmentError(ValueError):
-    """There is/are no environment(s) for this name(s)."""
+    def encrypt(self):
+        if self.cleartext == self.original_cleartext:
+            print("No changes from original cleartext. Not updating.")
+            return
+        if self.edit_file:
+            # If we're editing a specific file, we can just overwrite it.
+            with self.environment.secret_provider.config_file:
+                self.environment.secret_provider.write_file(
+                    self.file, self.cleartext.encode("utf-8")
+                )
+        else:
+            self.environment.secret_provider.write_config(
+                self.cleartext.encode("utf-8")
+            )
 
-    def __init__(self, names: list):
-        self.names = names
+    def edit(self):
+        _, suffix = os.path.splitext(self.file.path.name)
+        with tempfile.NamedTemporaryFile(
+            prefix="edit", suffix=suffix, mode="w+", encoding="utf-8"
+        ) as clearfile:
+            clearfile.write(self.cleartext)
+            clearfile.flush()
 
-    def __str__(self):
-        return f'Unknown environment(s): {", ".join(self.names)}'
+            args = [self.editor_cmd + " " + clearfile.name]
 
+            if debug:
+                print("Running editor with command: {}".format(args))
 
-class Environment(object):
-    def __init__(self, path: pathlib.Path = None, name=None):
-        if path:
-            self.path = path
-            self.name = path.parent.name
-        else:
-            self.name = name
-            self.path = pathlib.Path("environments" / name / "secrets.cfg")
+            subprocess.check_call(args, shell=True)
 
-        self.f = EncryptedConfigFile(
-            self.path, add_files_for_env=self.name, write_lock=True, quiet=True
-        )
-        self.f.__enter__()
-
-    def __del__(self):
-        try:
-            self.f.__exit__()
-        except AttributeError:
-            pass
-
-    @classmethod
-    def all(cls):
-        for path in pathlib.Path("environments").glob("*/environment.cfg"):
-            path = path.parent / "secrets.cfg"
-            yield Environment(path=path)
-
-    @classmethod
-    def by_filter(cls, filter):
-        if filter:
-            filter = filter.split(",")
-        environments = []
-        for e in cls.all():
-            if filter:
-                if e.name in filter:
-                    filter.remove(e.name)
-                else:
-                    continue
-            environments.append(e)
-        if filter:
-            raise UnknownEnvironmentError(filter)
-        return environments
-
-    def summary(self):
-        try:
-            self.f.read()
-        except Exception as e:
-            print("\t{}".format(e))
-            return
-        print("\t members")
-        members = self.f.config.get("batou", "members")
-        for m in members.value.split(","):
-            m = m.strip()
-            print("\t\t-", m)
-        if not members:
-            print("\t\t(none)")
-        print("\t secret files")
-        # Keys of self.f.files are strings, but self.path is pathlib.Path:
-        files = [f for f in self.f.files if f != str(self.path)]
-        files = [
-            f.replace("secrets/{}-".format(self.name), "", 1) for f in files
-        ]
-        for f in files:
-            print("\t\t-", f)
-        if not files:
-            print("\t\t(none)")
-        print()
-
-    def add_user(self, keyid):
-        try:
-            self.f.read()
-        except Exception as e:
-            print("\t{}".format(e))
-            return
-        members = self.f.get_members()
-        if keyid not in members:
-            members.append(keyid)
-            self.f.set_members(members)
-            try:
-                self.f.write()
-            except Exception as e:
-                print("\t{}".format(e))
-                return
-        self.summary()
-
-    def remove_user(self, keyid):
-        try:
-            self.f.read()
-        except Exception as e:
-            print("\t{}".format(e))
-            return
-        members = self.f.get_members()
-        if keyid in members:
-            members.remove(keyid)
-            self.f.set_members(members)
-            try:
-                self.f.write()
-            except Exception as e:
-                print("\t{}".format(e))
-                return
-        self.summary()
+            with open(clearfile.name, "r") as new_clearfile:
+                self.cleartext = new_clearfile.read()
 
 
-def summary(**kw):
+def main(editor, environment, edit_file: Optional[str] = None, **kw):
     """Secrets editor console script.
 
     The main focus here is to avoid having unencrypted files accidentally
     ending up in the deployment repository.
 
     """
+
     try:
-        for e in Environment.all():
-            print(e.name)
-            e.summary()
-    except GPGCallError as e:
+        editor = Editor(editor, Environment(environment), edit_file)
+        editor.main()
+    except Exception as e:
+        # only print traceback if we're in debug mode
+        if debug:
+            traceback.print_exc()
         print(e, file=sys.stderr)
-        print(e.output, file=sys.stderr)
-        return 1  # exit code
-
-
-def add_user(keyid, environments, **kw):
-    """Add a user to a given environment.
-
-    If environments is not given, a user is added
-    to all environments.
-
-    """
-    for e in Environment.by_filter(environments):
-        print(e.name)
-        e.add_user(keyid)
-        print()
-
-
-def remove_user(keyid, environments, **kw):
-    """Remove a user from a given environment.
-
-    If environments is not given, the user is removed
-    from all environments.
-
-    """
-    for e in Environment.by_filter(environments):
-        print(e.name)
-        e.remove_user(keyid)
-        print()
+        sys.exit(1)
```

### Comparing `batou-2.3b6/src/batou/secrets/tests/test_editor.py` & `batou-2.4a1/src/batou/secrets/tests/test_editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,67 @@
+import os
 import pathlib
 
 import pytest
 
+from batou.environment import Environment
 from batou.secrets.edit import Editor
-from batou.secrets.encryption import EncryptedConfigFile
 
 from .test_secrets import encrypted_file
 
 
-def test_edit(tmpdir):
-    with EncryptedConfigFile(str(tmpdir / "asdf"), write_lock=True) as sf:
-        editor = Editor(
-            "true", environment="none", edit_file=list(sf.files.keys())[0]
-        )
-        editor.cleartext = "asdf"
-        editor.edit()
-        assert editor.cleartext == "asdf"
+def test_edit_gpg(tmpdir):
+    editor = Editor(
+        "true",
+        environment=Environment(
+            "tutorial", basedir="examples/tutorial-secrets"
+        ),
+        edit_file="asdf",
+    )
+    editor.cleartext = "asdf"
+    editor.edit()
+    assert editor.cleartext == "asdf"
+
+
+def test_edit_age(tmpdir):
+    editor = Editor(
+        "true",
+        environment=Environment("age", basedir="examples/tutorial-secrets"),
+        edit_file="asdf",
+    )
+    editor.cleartext = "asdf"
+    editor.edit()
+    assert editor.cleartext == "asdf"
 
 
 def test_edit_command_loop(tmpdir, capsys):
-    with EncryptedConfigFile(str(tmpdir / "asdf"), write_lock=True) as sf:
-        editor = Editor(
-            "true", environment="none", edit_file=list(sf.files.keys())[0]
-        )
-        editor.cleartext = "asdf"
+    editor = Editor(
+        "true",
+        environment=Environment(
+            "tutorial", basedir="examples/tutorial-secrets"
+        ),
+    )
+    editor.cleartext = "asdf"
 
-        with pytest.raises(ValueError):
-            editor.process_cmd("asdf")
+    with pytest.raises(ValueError):
+        editor.process_cmd("asdf")
 
-        def broken_cmd():
-            raise RuntimeError("gpg is broken")
+    def broken_cmd():
+        raise RuntimeError("gpg is broken")
 
-        editor.edit = broken_cmd
-        editor.encrypt = broken_cmd
+    editor.edit = broken_cmd
+    editor.encrypt = broken_cmd
 
-        cmds = ["edit", "asdf", "encrypt", "quit"]
+    cmds = ["edit", "asdf", "encrypt", "quit"]
 
-        def _input():
-            return cmds.pop(0)
+    def _input():
+        return cmds.pop(0)
 
-        editor._input = _input
-        editor.interact()
+    editor._input = _input
+    editor.interact()
 
     out, err = capsys.readouterr()
     assert err == ""
     assert (
         out
         == """\
 
@@ -79,31 +96,46 @@
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 """
     )
 
 
-def test_edit_file_has_secret_prefix(tmpdir, encrypted_file):
+def test_edit_file_has_secret_prefix_gpg(tmpdir, encrypted_file):
     filename = "asdf123"
-    c = EncryptedConfigFile(encrypted_file, write_lock=True)
-    with c as _:
-        editor = Editor("true", environment="none", edit_file=filename)
-        assert editor.edit_file == pathlib.Path("environments") / "none" / (
-            f"secret-{filename}"
-        )
+    editor = Editor(
+        "true",
+        environment=Environment(
+            "tutorial", basedir="examples/tutorial-secrets"
+        ),
+        edit_file=filename,
+    )
+    assert editor.file.path.name == f"secret-{filename}.gpg"
+
+
+def test_edit_file_has_secret_prefix_age(tmpdir, encrypted_file):
+    filename = "asdf123"
+    editor = Editor(
+        "true",
+        environment=Environment("age", basedir="examples/tutorial-secrets"),
+        edit_file=filename,
+    )
+    assert editor.file.path.name == f"secret-{filename}.age"
 
 
 def test_blank_edit(tmpdir, encrypted_file):
-    c = EncryptedConfigFile(encrypted_file, write_lock=True)
-    with c as configfile:
-        editor = Editor("true", environment="none", edit_file="asdf")
-        editor.configfile = configfile
-        editor.editing = configfile.add_file(tmpdir / "asdf")
-        with editor.editing as f:
-            f.read()
-            editor.cleartext = editor.original_cleartext = f.cleartext
+    editor = Editor(
+        "true",
+        environment=Environment(
+            "tutorial", basedir="examples/tutorial-secrets"
+        ),
+        edit_file="asdf",
+    )
+    with editor.file:
+        editor.original_cleartext = None
+        editor.cleartext = ""
         editor.edit()
         assert editor.cleartext == ""
         editor.encrypt()
-        with open(tmpdir / "asdf", "rb") as f:
-            assert f.read() != b""
+    with open(editor.file.path, "rb") as f:
+        assert f.read() != b""
+    os.unlink(editor.file.path)
```

### Comparing `batou-2.3b6/src/batou/secrets/tests/test_manage.py` & `batou-2.4a1/src/batou/secrets/tests/test_manage.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 import textwrap
 
 import pytest
 
 from ..manage import UnknownEnvironmentError, add_user, remove_user, summary
 
 
-@pytest.mark.parametrize("func", (add_user, remove_user))
-def test_manage__1(monkeypatch, func):
-    """It raises an exception if called with an unknown environment."""
-    monkeypatch.chdir("examples/errors")
-    with pytest.raises(UnknownEnvironmentError) as err:
-        func("max@example.com", "foo,bar,errors")
-    assert "Unknown environment(s): foo, bar" == str(err.value)
-
-
 def test_manage__2(tmp_path, monkeypatch, capsys):
     """It allows to add/remove users."""
     shutil.copytree("examples/errors", tmp_path / "errors")
     monkeypatch.chdir(tmp_path / "errors")
 
     summary()
     out, err = capsys.readouterr()
@@ -58,13 +49,10 @@
 
 def test_manage__summary__2(capsys, monkeypatch):
     """It prints an error message on decoding problems."""
     monkeypatch.chdir("examples/errors")
     monkeypatch.setitem(os.environ, "GNUPGHOME", "")
     assert summary() == 1  # exit code
     out, err = capsys.readouterr()
-    expected = (
-        "Exitcode 2 while calling:"
-        " gpg -q --no-tty --batch --decrypt environments/errors/secrets.cfg"
-    )
-    assert out == ""
+    expected = "Exitcode 2 while calling: gpg --decrypt"
+    assert out == "errors\n"
     assert err.startswith(expected)
```

### Comparing `batou-2.3b6/src/batou/template.py` & `batou-2.4a1/src/batou/template.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/conftest.py` & `batou-2.4a1/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/ellipsis.py` & `batou-2.4a1/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_component.py` & `batou-2.4a1/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_config.py` & `batou-2.4a1/src/batou/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         batou.UnsatisfiedResources.from_context({"asdf": [c.root]}),
         batou.MissingEnvironment.from_context(env),
         batou.MissingComponent.from_context("asdf", "localhost"),
         batou.SuperfluousSection.from_context("asdf"),
         batou.SuperfluousComponentSection.from_context("asdf"),
         batou.SuperfluousSecretsSection.from_context("asdf"),
         batou.CycleErrorDetected.from_context(ValueError()),
-        batou.NonConvergingWorkingSet.from_context([c]),
+        batou.NonConvergingWorkingSet.from_context([c.root]),
         batou.DeploymentError(),
         batou.DuplicateHostMapping.from_context("host", "map1", "map2"),
         batou.RepositoryDifferentError.from_context("asdf", "bsdf"),
         batou.DuplicateHostError.from_context("localhost"),
         batou.InvalidIPAddressError.from_context("asdf"),
     ]
```

### Comparing `batou-2.3b6/src/batou/tests/test_dependencies.py` & `batou-2.4a1/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_deploy.py` & `batou-2.4a1/src/batou/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_endtoend.py` & `batou-2.4a1/src/batou/tests/test_endtoend.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 batou/2... (cpython 3...)
 ================================== Preparing ===================================
 main: Loading environment `errors`...
 main: Verifying repository ...
 main: Loading secrets ...
 
 ERROR: Error while calling GPG
-        command: gpg --decrypt environments/errors/secrets.cfg
+        command: gpg --decrypt ...environments/errors/secrets.cfg.gpg
       exit code: 2
         message:
 gpg: ...
 ...
 ERROR: Failed loading component file
            File: .../examples/errors/components/component5/component.py
       Exception: invalid syntax (component.py, line 1)
@@ -145,15 +145,15 @@
 
 ERROR: Found dependency cycle
 cycle1 depends on
         cycle2
 cycle2 depends on
         cycle1
 
-ERROR: 8 remaining unconfigured component(s)
+ERROR: 9 remaining unconfigured component(s): component1, component2, component4, crontab, cycle1, cycle2, dnsproblem, dnsproblem2, filemode
 ======================= 10 ERRORS - CONFIGURATION FAILED =======================
 ====================== DEPLOYMENT FAILED (during connect) ======================
 """
     )  # noqa: E501 line too long
 
 
 def test_example_errors_missing_environment():
@@ -186,14 +186,15 @@
 localhost: Connecting via local (1/2)
 otherhost: Connection ignored (2/2)
 ================================== Deploying ===================================
 localhost: Scheduling component component1 ...
 localhost: Skipping component fail ... (Component ignored)
 otherhost: Skipping component fail2 ... (Host ignored)
 =================================== Summary ====================================
+Deployment took total=...s, connect=...s, deploy=...s
 ============================= DEPLOYMENT FINISHED ==============================
 """
     )  # noqa: E501 line too long
 
 
 def test_example_async_sync_deployment():
     os.chdir("examples/sync_async")
@@ -263,10 +264,33 @@
 Not showing diff as it contains sensitive data,
 see ...diff for the diff.
 localhost > Hello > File('work/hello/other-secrets.yaml') > Presence('other-secrets.yaml')
 localhost > Hello > File('work/hello/other-secrets.yaml') > Content('other-secrets.yaml')
 Not showing diff as it contains sensitive data,
 see ...diff for the diff.
 =================================== Summary ====================================
+Deployment took total=...s, connect=...s, deploy=...s
 ============================= DEPLOYMENT FINISHED ==============================
 """
     )  # noqa: E501 line too long
+
+
+def test_durations_are_shown_for_components():
+    os.chdir("examples/durations")
+    out, _ = cmd("./batou deploy default")
+    assert out == Ellipsis(
+        """\
+batou/2... (cpython 3...)
+================================== Preparing ===================================
+main: Loading environment `default`...
+main: Verifying repository ...
+main: Loading secrets ...
+================== Connecting hosts and configuring model ... ==================
+localhost: Connecting via local (1/1)
+================================== Deploying ===================================
+localhost: Scheduling component takeslongtime ...
+localhost > Takeslongtime [total=...s, verify=...s, update=NaN, sub=NaN]
+=================================== Summary ====================================
+Deployment took total=...s, connect=...s, deploy=...s
+============================= DEPLOYMENT FINISHED ==============================
+"""
+    )
```

### Comparing `batou-2.3b6/src/batou/tests/test_environment.py` & `batou-2.4a1/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_exceptions.py` & `batou-2.4a1/src/batou/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_host.py` & `batou-2.4a1/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_main.py` & `batou-2.4a1/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_remote.py` & `batou-2.4a1/src/batou/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_remote_core.py` & `batou-2.4a1/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_repository.py` & `batou-2.4a1/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_resources.py` & `batou-2.4a1/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_template.py` & `batou-2.4a1/src/batou/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/tests/test_utils.py` & `batou-2.4a1/src/batou/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Address,
     CmdExecutionError,
     MultiFile,
     NetLoc,
     call_with_optional_args,
     cmd,
     flatten,
+    format_duration,
     hash,
     locked,
     notify,
     remove_nodes_without_outgoing_edges,
     resolve,
     resolve_v6,
     revert_graph,
@@ -62,44 +63,44 @@
     ov = {"foo.example.com": "::27"}
     assert "::27" == resolve_v6("foo.example.com", 80, resolve_override=ov)
 
 
 def test_resolve_v6_does_not_return_link_local_addresses(output, monkeypatch):
     output.enable_debug = True
 
-    def link_local_addrinfo(*args, **kw):
+    def link_local_addrinfo_1(*args, **kw):
         return [
             (
                 None,
                 None,
                 None,
                 None,
                 ("fe80::feaa:14ff:fe8f:94ba", 80, None, None),
             )
         ]
 
-    monkeypatch.setattr(socket, "getaddrinfo", link_local_addrinfo)
+    monkeypatch.setattr(socket, "getaddrinfo", link_local_addrinfo_1)
 
     with pytest.raises(ValueError) as err:
         resolve_v6("foo.example.com", 80)
     assert "No valid address found for `foo.example.com`." == str(err.value)
 
-    def link_local_addrinfo(*args, **kw):
+    def link_local_addrinfo_2(*args, **kw):
         return [
             (
                 None,
                 None,
                 None,
                 None,
                 ("fe80::feaa:14ff:fe8f:94ba", 80, None, None),
             ),
             (None, None, None, None, ("2a02::1", 80, None, None)),
         ]
 
-    monkeypatch.setattr(socket, "getaddrinfo", link_local_addrinfo)
+    monkeypatch.setattr(socket, "getaddrinfo", link_local_addrinfo_2)
 
     output.backend.output = ""
     assert resolve_v6("foo.example.com", 80) == "2a02::1"
 
     assert (
         """\
 resolving (v6) `foo.example.com`
@@ -464,7 +465,13 @@
     # The function expect x and it gets passed through
     assert call_with_optional_args(bar, x=4) == 4
     # The function accepts kw args and sees x
     assert call_with_optional_args(baz, x=3) == 3
     # The function accepts x but also expects y and thus breaks
     with pytest.raises(TypeError):
         call_with_optional_args(quux, x=1)
+
+
+def test_format_duration():
+    assert format_duration(1.23124) == "1.23s"
+    assert format_duration(61) == "1m1s"
+    assert format_duration(None) == "NaN"
```

### Comparing `batou-2.3b6/src/batou/tests/test_vfs.py` & `batou-2.4a1/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou/utils.py` & `batou-2.4a1/src/batou/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import itertools
 import os
 import socket
 import subprocess
 import sys
 import time
 from collections import defaultdict
+from typing import Optional
 
 import pkg_resources
 
 from batou import DeploymentError, IPAddressConfigurationError, output
 
 
 class BagOfAttributes(dict):
@@ -149,15 +150,15 @@
         output.annotate("resolving (v6) `{}`".format(host), debug=True)
         responses = socket.getaddrinfo(host, int(port), socket.AF_INET6)
         output.annotate(
             "resolved (v6) `{}` to {}".format(host, responses), debug=True
         )
         address = None
         for _, _, _, _, sockaddr in responses:
-            addr, _, _, _ = sockaddr
+            addr = sockaddr[0]
             if addr.startswith("fe80:"):
                 continue
             address = addr
             break
         if not address:
             raise ValueError("No valid address found for `{}`.".format(host))
         output.annotate(
@@ -192,15 +193,15 @@
     * 'optional' -> the listen/listen_v6 attribute will contain None if it does
        not resolve.
 
     """
 
     #: The connect address as it should be used when configuring clients.
     #: This is a :py:class:`batou.utils.NetLoc` object.
-    connect = None
+    connect: "NetLoc"
 
     # The dance with the ADDR_DEFAULT is to allow overriding the class-based
     # defaults on an environment level.
     require_v4 = True
     require_v6 = False
 
     def __init__(
@@ -247,14 +248,15 @@
         configuring servers. This is a :py:class:`batou.utils.NetLoc`
         object. It raises an :py:class:`batou.IPAddressConfigurationError`
         if used unconfigured.
         """
         if not self.require_v4:
             raise IPAddressConfigurationError.from_context(self, 4)
 
+        assert self.connect.port is not None
         if not hasattr(self, "_listen_v4"):
             try:
                 address = resolve(self.connect.host, self.connect.port)
                 self.listen = NetLoc(address, self.connect.port)
             except Exception:
                 if self.require_v4 == "optional":
                     self.listen = None
@@ -273,14 +275,15 @@
         configuring servers. This is a :py:class:`batou.utils.NetLoc`
         object. It raises an :py:class:`batou.IPAddressConfigurationError`
         if used unconfigured.
         """
         if not self.require_v6:
             raise IPAddressConfigurationError.from_context(self, 6)
 
+        assert self.connect.port is not None
         if not hasattr(self, "_listen_v6"):
             try:
                 address = resolve_v6(self.connect.host, self.connect.port)
                 self.listen_v6 = NetLoc(address, self.connect.port)
             except Exception:
                 if self.require_v6 == "optional":
                     self.listen_v6 = None
@@ -314,15 +317,15 @@
         >>> y = NetLoc('127.0.0.1', 80)
         >>> str(y)
         '127.0.0.1:80'
 
     """
 
     #: The host part of this network location. Can be a hostname or IP address.
-    host = None
+    host: str
     #: The port of this network location. Can be ``None`` or an integer.
     port = None
 
     def __init__(self, host, port=None):
         self.host = host
         self.port = port
 
@@ -431,14 +434,17 @@
         output.error(self.cmd)
         output.tabular("Return code", str(self.returncode), red=True)
         output.line("STDOUT", red=True)
         output.annotate(self.stdout)
         output.line("STDERR", red=True)
         output.annotate(self.stderr)
 
+    def __str__(self):
+        return f"Command {self.cmd} failed with return code {self.returncode}\n\nSTDOUT:\n{self.stdout}\n\nSTDERR:\n{self.stderr}"
+
 
 def cmd(
     cmd,
     silent=False,
     ignore_returncode=False,
     communicate=True,
     env=None,
@@ -478,29 +484,71 @@
     if process.returncode not in acceptable_returncodes:
         if not ignore_returncode:
             raise CmdExecutionError(cmd, process.returncode, stdout, stderr)
     return stdout, stderr
 
 
 def get_output(command, default=None):
-    stdout, stderr = cmd(command, ignore_returncode=True)
+    stdout, stderr = cmd(command, ignore_returncode=True)  # type: ignore
     return stdout or default
 
 
 class Timer(object):
-    def __init__(self, note):
-        self.duration = 0
-        self.note = note
-
-    def __enter__(self):
-        self.started = time.time()
-
-    def __exit__(self, exc1, exc2, exc3):
-        self.duration = time.time() - self.started
-        output.annotate(self.note + " took %fs" % self.duration, debug=True)
+    def __init__(self, tag=None):
+        self.durations = defaultdict(float)  # returns 0.0 for missing keys
+        self.tag = tag
+
+    class TimerContext(object):
+        def __init__(self, timer, note):
+            self.timer = timer
+            self.note = note
+
+        def __enter__(self):
+            self.start = time.time()
+
+        def __exit__(self, exc_type, exc_value, traceback):
+            delta = time.time() - self.start
+            self.timer.durations[self.note] += delta
+            output.annotate(
+                f"Timer {self.timer.tag}: {self.note} took {delta:.2f} seconds",
+                debug=True,
+            )
+            self.timer.durations[self.note] += time.time() - self.start
+
+    def step(self, note):
+        if note == "total":
+            raise ValueError("Cannot use 'total' as a step name")
+        return self.TimerContext(self, note)
+
+    def above_threshold(self, **thresholds):
+        """
+        Return true if any of the steps took longer than the given threshold.
+        "total" is a special step that is the sum of all other steps.
+        """
+
+        total = sum(self.durations.values())
+        for note, duration in self.durations.items():
+            if note in thresholds and duration > thresholds[note]:
+                return True
+        if "total" in thresholds and total > thresholds["total"]:
+            return True
+        return False
+
+    def humanize(self, *steps):
+        """
+        Given a list of steps, return a string with the time taken for each
+        step.
+        """
+        total = sum(self.durations.values())
+        durations = self.durations.copy()
+        durations["total"] = total
+
+        return ", ".join(
+            f"{note}={format_duration(durations.get(note))}" for note in steps
+        )
 
 
 def hash(path, function="sha_512"):
     h = getattr(hashlib, function)()
     with open(path, "rb") as f:
         chunk = f.read(64 * 1024)
         while chunk:
@@ -538,7 +586,32 @@
             result[k] = dict_merge(result[k], v)
         elif k in result and isinstance(result[k], list):
             result[k] = result[k][:]
             result[k].extend(v)
         else:
             result[k] = copy.deepcopy(v)
     return result
+
+
+def format_duration(duration: Optional[float]) -> str:
+    """
+    Formats a duration (in seconds) into a human readable string.
+
+    Examples:
+    ```
+    format_duration(1.23124) == "1.23s"
+    format_duration(61) == "1m1s"
+    format_duration(None) == "NaN"
+    ```
+    """
+
+    if duration is None:
+        return "NaN"
+
+    minutes, seconds = divmod(duration, 60)
+
+    if minutes:
+        output = "{}m{}s".format(int(minutes), int(seconds))
+    else:
+        output = "{:.2f}s".format(seconds)
+
+    return output
```

### Comparing `batou-2.3b6/src/batou/vfs.py` & `batou-2.4a1/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b6/src/batou.egg-info/PKG-INFO` & `batou-2.4a1/src/batou.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.3b6
+Version: 2.4a1
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -104,7 +105,9 @@
 * Run `./develop.sh` to create a local virtualenv with everything set up.
 * Run the test suite using: `bin/tox`
 * Build the documentation using: `cd doc; make`
 * Set up GPG for the examples with `export GNUPGHOME=<DIRECTORY OF BATOU HERE>/src/batou/secrets/tests/fixture/gnupg`
 ## Changelog
 
 See [CHANGES.md](./CHANGES.md).
+
+
```

### Comparing `batou-2.3b6/src/batou.egg-info/SOURCES.txt` & `batou-2.4a1/src/batou.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,28 @@
 doc/source/user/installation-deb.txt
 doc/source/user/installation-rpm.txt
 doc/source/user/intro.txt
 doc/source/user/quickstart.txt
 examples/api/index.txt
 examples/api/requirements.txt
 examples/django/requirements.txt
+examples/durations/requirements.txt
 examples/errors/requirements.txt
 examples/errors2/requirements.txt
 examples/ignores/requirements.txt
 examples/largetempl/requirements.txt
 examples/package/requirements.txt
 examples/sync_async/requirements.txt
 examples/tutorial-buildout/requirements.txt
 examples/tutorial-component/requirements.txt
 examples/tutorial-helloworld/requirements.txt
 examples/tutorial-parallelize/requirements.txt
 examples/tutorial-provision-container/requirements.txt
 examples/tutorial-secrets/requirements.txt
+examples/tutorial-secrets/environments/age/age_keys.txt
 examples/vagrant/requirements.txt
 examples/vagrant-multi/requirements.txt
 examples/venvs/requirements.txt
 examples/venvs/environments/requirements.txt
 src/batou/__init__.py
 src/batou/_output.py
 src/batou/agent.py
@@ -123,14 +125,15 @@
 src/batou/lib/tests/test_supervisor.py
 src/batou/lib/tests/test_svn.py
 src/batou/migrate/__init__.py
 src/batou/migrate/migrations/2300.py
 src/batou/migrate/migrations/2301.py
 src/batou/migrate/migrations/2302.py
 src/batou/migrate/migrations/2303.py
+src/batou/migrate/migrations/2400.py
 src/batou/migrate/migrations/__init__.py
 src/batou/migrate/tests/__init__.py
 src/batou/migrate/tests/test_migrate.py
 src/batou/secrets/__init__.py
 src/batou/secrets/edit.py
 src/batou/secrets/encryption.py
 src/batou/secrets/manage.py
```

