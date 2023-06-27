# Comparing `tmp/ociedoo-0.8.0a2.tar.gz` & `tmp/ociedoo-0.8.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ociedoo-0.8.0a2.tar", max compression
+gzip compressed data, was "ociedoo-0.8.0a3.tar", max compression
```

## Comparing `ociedoo-0.8.0a2.tar` & `ociedoo-0.8.0a3.tar`

### file list

```diff
@@ -1,12 +1,26 @@
--rw-r--r--   0        0        0    34520 2019-04-24 20:34:30.919076 ociedoo-0.8.0a2/LICENSE
--rw-r--r--   0        0        0     3502 2022-10-24 21:32:42.859135 ociedoo-0.8.0a2/README.md
--rw-r--r--   0        0        0     1096 2023-06-26 09:21:59.970218 ociedoo-0.8.0a2/ociedoo/__init__.py
--rw-r--r--   0        0        0      126 2022-02-15 17:37:55.450743 ociedoo-0.8.0a2/ociedoo/__main__.py
--rw-r--r--   0        0        0     1826 2022-02-15 17:37:55.450743 ociedoo-0.8.0a2/ociedoo/check.py
--rw-r--r--   0        0        0    32817 2023-06-25 09:43:33.703960 ociedoo-0.8.0a2/ociedoo/cli.py
--rw-r--r--   0        0        0     5647 2023-06-25 10:00:11.281181 ociedoo-0.8.0a2/ociedoo/complete.py
--rw-r--r--   0        0        0      414 2023-06-25 09:43:33.703960 ociedoo-0.8.0a2/ociedoo/defaults/config
--rw-r--r--   0        0        0     9490 2023-06-26 09:21:59.970218 ociedoo-0.8.0a2/ociedoo/lib.py
--rw-r--r--   0        0        0     1332 2023-06-26 09:21:59.970218 ociedoo-0.8.0a2/pyproject.toml
--rw-r--r--   0        0        0     4606 2023-06-26 09:22:08.153716 ociedoo-0.8.0a2/setup.py
--rw-r--r--   0        0        0     4764 2023-06-26 09:22:08.155301 ociedoo-0.8.0a2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-27 13:23:15.371784 ociedoo-0.8.0a3/LICENSES/
+-rw-r--r--   0        0        0     3502 2022-10-24 21:32:42.859135 ociedoo-0.8.0a3/README.md
+-rw-r--r--   0        0        0     1076 2023-06-27 13:23:15.371784 ociedoo-0.8.0a3/ociedoo/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/__main__.py
+-rw-r--r--   0        0        0     1806 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/check.py
+-rw-r--r--   0        0        0     1101 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:05:12.252786 ociedoo-0.8.0a3/ociedoo/cli/cmd/__init__.py
+-rw-r--r--   0        0        0     1257 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/configuration.py
+-rw-r--r--   0        0        0     1419 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/copy_db.py
+-rw-r--r--   0        0        0     1323 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/drop_db.py
+-rw-r--r--   0        0        0     1566 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/list_db.py
+-rw-r--r--   0        0        0      738 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/list_module.py
+-rw-r--r--   0        0        0     2266 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/main.py
+-rw-r--r--   0        0        0     1448 2023-06-27 13:23:15.375784 ociedoo-0.8.0a3/ociedoo/cli/cmd/odooctl.py
+-rw-r--r--   0        0        0     1645 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/cmd/rename_db.py
+-rw-r--r--   0        0        0     6694 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/cmd/restore_db.py
+-rw-r--r--   0        0        0     1930 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/cmd/run.py
+-rw-r--r--   0        0        0     3145 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/cmd/set_password.py
+-rw-r--r--   0        0        0    10757 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/cmd/update_module.py
+-rw-r--r--   0        0        0     1127 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/cli/tool.py
+-rw-r--r--   0        0        0     5627 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/complete.py
+-rw-r--r--   0        0        0      532 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/defaults/config
+-rw-r--r--   0        0        0     9470 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/ociedoo/lib.py
+-rw-r--r--   0        0        0     1441 2023-06-27 13:23:15.379784 ociedoo-0.8.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4640 2023-06-27 13:23:28.283065 ociedoo-0.8.0a3/setup.py
+-rw-r--r--   0        0        0     4764 2023-06-27 13:23:28.283571 ociedoo-0.8.0a3/PKG-INFO
```

### Comparing `ociedoo-0.8.0a2/README.md` & `ociedoo-0.8.0a3/README.md`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a2/ociedoo/__init__.py` & `ociedoo-0.8.0a3/ociedoo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright 2018-2020 Coop IT Easy SCRLfs (<http://coopiteasy.be>)
-# License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
+# SPDX-FileCopyrightText: 2018 Coop IT Easy SC <https://coopiteasy.be>
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Constant shared across the module"""
 
 import os
 from pathlib import Path
 
 from prgconfig import PrgConfig
 
 __productname__ = "ociedoo"
-__version__ = "0.8.0-alpha.2"
+__version__ = "0.8.0-alpha.3"
 __license__ = "GPL-3.0-or-later"
 
 # Path for default value for config file
 PGRNAME = "ociedoo"
 DEFAULTSPATH = str(Path(__file__).parent / Path("defaults"))
 DEFAULT_CONF = str(Path(DEFAULTSPATH) / "config")
```

### Comparing `ociedoo-0.8.0a2/ociedoo/check.py` & `ociedoo-0.8.0a3/ociedoo/check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright 2018-2019 Coop IT Easy SCRLfs (<http://coopiteasy.be>)
-# License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
+# SPDX-FileCopyrightText: 2018 Coop IT Easy SC <https://coopiteasy.be>
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Checks for arguments of the CLI"""
 
 import re
 
 import click
```

### Comparing `ociedoo-0.8.0a2/ociedoo/complete.py` & `ociedoo-0.8.0a3/ociedoo/complete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright 2018-2020 Coop IT Easy SCRLfs (<http://coopiteasy.be>)
-# License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
+# SPDX-FileCopyrightText: 2018 Coop IT Easy SC <https://coopiteasy.be>
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Completion functions for CLI"""
 
 import os
 from pathlib import Path
 
 from ociedoo import config, lib
```

### Comparing `ociedoo-0.8.0a2/ociedoo/lib.py` & `ociedoo-0.8.0a3/ociedoo/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright 2018-2020 Coop IT Easy SCRLfs (<http://coopiteasy.be>)
-# License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
+# SPDX-FileCopyrightText: 2018 Coop IT Easy SC <https://coopiteasy.be>
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Small function used across the project."""
 
 import gzip
 import mimetypes
 import re
 import shlex
```

### Comparing `ociedoo-0.8.0a2/pyproject.toml` & `ociedoo-0.8.0a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+# SPDX-FileCopyrightText: 2018 Coop IT Easy SC <https://coopiteasy.be>
+#
+# SPDX-License-Identifier: CC0-1.0
+
 [tool.black]
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "ociedoo"
-version = "0.8.0-alpha.2"
+version = "0.8.0-alpha.3"
 description = "CLI tool to simplify the management of Odoo"
 authors = ["Coop IT Easy SCRLfs <remy@coopiteasy.be>"]
 maintainers = ["Rémy Taymans <remy@coopiteasy.be>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/coopiteasy/ociedoo"
 keywords = ["cli", "odoo", "coopiteasy"]
```

### Comparing `ociedoo-0.8.0a2/setup.py` & `ociedoo-0.8.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['ociedoo']
+['ociedoo', 'ociedoo.cli', 'ociedoo.cli.cmd']
 
 package_data = \
 {'': ['*'], 'ociedoo': ['defaults/*']}
 
 install_requires = \
 ['click>=7.0,<8.0',
  'passlib>=1.7.4,<2.0.0',
@@ -14,15 +14,15 @@
  'sh>=1.12,<2.0']
 
 entry_points = \
 {'console_scripts': ['ociedoo = ociedoo.cli:main']}
 
 setup_kwargs = {
     'name': 'ociedoo',
-    'version': '0.8.0a2',
+    'version': '0.8.0a3',
     'description': 'CLI tool to simplify the management of Odoo',
     'long_description': '[![pipeline status](https://gitlab.com/coopiteasy/ociedoo/badges/master/pipeline.svg)](https://gitlab.com/coopiteasy/ociedoo)\n\nociedoo\n=======\n\nociedoo is a cli collection of tools to simplify the management of odoo\non a server.\n\nSee help for more info.\n\n\nInstallation\n------------\n\nociedoo needs python version >= 3.5. So ensure `pip` points to a correct\nversion of python. To do this run:\n```shell\npip --version\n```\n\nIt should return something like:\n```\npip xx.y from /path/to/pip (python 3.5)\n```\n\nIf `pip` doesn\'t run python >=3.5, try running `pip3` which is on\ncertain distribution the `pip` for python >=3.\n\n\n### Dependencies\n\nociedoo uses external programs via the shell. Be sure they are installed\nand accessible for the current user.\n\n- psql\n- createdb\n- dropdb\n- systemctl\n\n\n### Install for a specific user\n\n\n#### Installation with pipx (recommended python >= 3.6)\n\n```shell\npipx install ociedoo\n```\n\n\n#### Installation with pipsi (recommended python < 3.5)\n\n```shell\npipsi install ociedoo\n```\n\n\n#### Install with pip\n\n```shell\npip install --user ociedoo\n```\n\n\n### Install system wide (for all users)\n\n\n#### Install with pipx (recommended python >= 3.6)\n\nFirst install pipx if not already installed:\n```shell\nsudo pip install pipx\n```\n\nThen install ociedoo:\n```shell\nsudo PIPX_HOME=/usr/local PIPX_BIN_DIR=/usr/local/bin pipx install ociedoo\n```\n\n\n#### Install with pipsi (recommended python < 3.6)\n\nFirst install pipsi, if not already installed:\n```shell\nsudo curl https://raw.githubusercontent.com/mitsuhiko/pipsi/master/get-pipsi.py | sudo python3 - --bin-dir /usr/local/bin --home /usr/local/venvs --no-modify-path\n```\n\nThen install ociedoo:\n```shell\nsudo pipsi --bin-dir /usr/local/bin --home /usr/local/venvs install ociedoo\n```\n\n\n#### Install with pip\n```shell\nsudo pip install ociedoo\n```\n\n\n### Enable bash completion\n\n\n#### Bash completion for a specific user\n\nTo enable bash completion add the following in your `.bashrc`:\n\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source ociedoo)"\nfi\n```\n\nOr if you use zsh, add this to your `.zshrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source_zsh ociedoo)"\nfi\n```\n\n\n#### Bash completion system wide (for all users)\n\nTo enable bash completion add the following in `/etc/bash.bashrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source ociedoo)"\nfi\n```\n\nOr if you use zsh, add this to your `/etc/zsh/zshrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source_zsh ociedoo)"\nfi\n```\n\n\nUpgrade\n-------\n\n\n### Upgrade for a specific user\n\n\n#### Upgrade with pipx (recommended python >= 3.6)\n\n```shell\npipx upgrade ociedoo\n```\n\n\n#### Upgrade with pipsi (recommended python < 3.5)\n\n```shell\npipsi upgrade ociedoo\n```\n\n\n#### Upgrade with pip\n\n```shell\npip install --user --upgrade ociedoo\n```\n\n\n### Upgrade system wide (for all users)\n\n\n#### Upgrade with pipx (recommended python >= 3.6)\n\n```shell\nsudo PIPX_HOME=/usr/local PIPX_BIN_DIR=/usr/local/bin pipx upgrade ociedoo\n```\n\n\n#### Upgrade with pipsi (recommended python < 3.5)\n\n```shell\nsudo pipsi --bin-dir /usr/local/bin --home /usr/local/venvs upgrade ociedoo\n```\n\n\n#### Upgrade with pip\n\n```shell\nsudo pip install --upgrade ociedoo\n```\n\nBuild and publish\n-----------------\n\nFirst do not forget to upgrade version. Then:\n\n```shell\npoetry build\npoetry publish -u coopiteasy\n',
     'author': 'Coop IT Easy SCRLfs',
     'author_email': 'remy@coopiteasy.be',
     'maintainer': 'Rémy Taymans',
     'maintainer_email': 'remy@coopiteasy.be',
     'url': 'https://gitlab.com/coopiteasy/ociedoo',
```

### Comparing `ociedoo-0.8.0a2/PKG-INFO` & `ociedoo-0.8.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ociedoo
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: CLI tool to simplify the management of Odoo
 Home-page: https://gitlab.com/coopiteasy/ociedoo
 License: GPL-3.0-or-later
 Keywords: cli,odoo,coopiteasy
 Author: Coop IT Easy SCRLfs
 Author-email: remy@coopiteasy.be
 Maintainer: Rémy Taymans
```

