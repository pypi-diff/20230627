# Comparing `tmp/cmdy-0.5.4.tar.gz` & `tmp/cmdy-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdy-0.5.4.tar", max compression
+gzip compressed data, was "cmdy-0.5.5.tar", max compression
```

## Comparing `cmdy-0.5.4.tar` & `cmdy-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-04-05 17:34:03.465765 cmdy-0.5.4/LICENSE
--rw-r--r--   0        0        0    15593 2023-04-05 17:34:03.465765 cmdy-0.5.4/README.md
--rw-r--r--   0        0        0      123 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/__init__.py
--rw-r--r--   0        0        0     9117 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy.py
--rw-r--r--   0        0        0     1939 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_bakeable.py
--rw-r--r--   0        0        0      899 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_defaults.py
--rw-r--r--   0        0        0     2666 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_exceptions.py
--rw-r--r--   0        0        0     9032 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugin.py
--rw-r--r--   0        0        0      485 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/__init__.py
--rw-r--r--   0        0        0     4355 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/fg.py
--rw-r--r--   0        0        0     4309 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/iter.py
--rw-r--r--   0        0        0     5076 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/pipe.py
--rw-r--r--   0        0        0     4975 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/redirect.py
--rw-r--r--   0        0        0     5157 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_plugins/value.py
--rw-r--r--   0        0        0     4934 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_result.py
--rw-r--r--   0        0        0    17349 2023-04-05 17:34:03.465765 cmdy-0.5.4/cmdy/cmdy_utils.py
--rw-r--r--   0        0        0     1174 2023-04-05 17:34:03.465765 cmdy-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    17352 1970-01-01 00:00:00.000000 cmdy-0.5.4/setup.py
--rw-r--r--   0        0        0    16509 1970-01-01 00:00:00.000000 cmdy-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 03:20:13.092855 cmdy-0.5.5/LICENSE
+-rw-r--r--   0        0        0    15593 2023-06-27 03:20:13.092855 cmdy-0.5.5/README.md
+-rw-r--r--   0        0        0      123 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/__init__.py
+-rw-r--r--   0        0        0     9117 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy.py
+-rw-r--r--   0        0        0     1939 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_bakeable.py
+-rw-r--r--   0        0        0      899 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_defaults.py
+-rw-r--r--   0        0        0     2666 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_exceptions.py
+-rw-r--r--   0        0        0     9032 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugin.py
+-rw-r--r--   0        0        0      485 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/__init__.py
+-rw-r--r--   0        0        0     4355 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/fg.py
+-rw-r--r--   0        0        0     4309 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/iter.py
+-rw-r--r--   0        0        0     5076 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/pipe.py
+-rw-r--r--   0        0        0     4975 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/redirect.py
+-rw-r--r--   0        0        0     5157 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_plugins/value.py
+-rw-r--r--   0        0        0     4934 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_result.py
+-rw-r--r--   0        0        0    17349 2023-06-27 03:20:13.092855 cmdy-0.5.5/cmdy/cmdy_utils.py
+-rw-r--r--   0        0        0     1174 2023-06-27 03:20:13.092855 cmdy-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    17352 1970-01-01 00:00:00.000000 cmdy-0.5.5/setup.py
+-rw-r--r--   0        0        0    16509 1970-01-01 00:00:00.000000 cmdy-0.5.5/PKG-INFO
```

### Comparing `cmdy-0.5.4/LICENSE` & `cmdy-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/README.md` & `cmdy-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy.py` & `cmdy-0.5.5/cmdy/cmdy.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_bakeable.py` & `cmdy-0.5.5/cmdy/cmdy_bakeable.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_defaults.py` & `cmdy-0.5.5/cmdy/cmdy_defaults.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_exceptions.py` & `cmdy-0.5.5/cmdy/cmdy_exceptions.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugin.py` & `cmdy-0.5.5/cmdy/cmdy_plugin.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugins/fg.py` & `cmdy-0.5.5/cmdy/cmdy_plugins/fg.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugins/iter.py` & `cmdy-0.5.5/cmdy/cmdy_plugins/iter.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugins/pipe.py` & `cmdy-0.5.5/cmdy/cmdy_plugins/pipe.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugins/redirect.py` & `cmdy-0.5.5/cmdy/cmdy_plugins/redirect.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_plugins/value.py` & `cmdy-0.5.5/cmdy/cmdy_plugins/value.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_result.py` & `cmdy-0.5.5/cmdy/cmdy_result.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/cmdy/cmdy_utils.py` & `cmdy-0.5.5/cmdy/cmdy_utils.py`

 * *Files identical despite different names*

### Comparing `cmdy-0.5.4/pyproject.toml` & `cmdy-0.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "cmdy"
-version = "0.5.4"
+version = "0.5.5"
 description = "Shell language to run command in python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/cmdy"
 repository = "https://github.com/pwwang/cmdy"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.7"
-python-simpleconf = {version = "^0.5", extras = ["toml"]}
+python-simpleconf = {version = "^0.6", extras = ["toml"]}
 varname = [
     {version = "^0.10", python = "<3.8"},
     {version = "^0.11", python = "^3.8"},
 ]
 curio = "^1.6"
 ## required by python-simpleconf
 # diot = "^0.1"
```

### Comparing `cmdy-0.5.4/setup.py` & `cmdy-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['cmdy', 'cmdy.cmdy_plugins']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['curio>=1.6,<2.0', 'python-simpleconf[toml]>=0.5,<0.6']
+['curio>=1.6,<2.0', 'python-simpleconf[toml]>=0.6,<0.7']
 
 extras_require = \
 {':python_version < "3.8"': ['varname>=0.10,<0.11'],
  ':python_version >= "3.8" and python_version < "4.0"': ['varname>=0.11,<0.12']}
 
 setup_kwargs = {
     'name': 'cmdy',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'Shell language to run command in python',
     'long_description': '# cmdy\n"Shell language" to run command in python\n\n[![pypi][1]][2] [![tag][3]][4] [![travis][5]][6] [![codacy quality][7]][8] [![codacy quality][9]][8] ![pyver][10]\n\n## Installation\n```shell\npip install cmdy\n```\n\n## Usage\n\nSee [Demo](./demo.ipynb)\n\n### Basic usage\n```python\nfrom cmdy import ls\nprint(ls())\n```\n\n```python\nfor line in ls().iter():\n    print(\'Got:\', line, end=\'\')\n```\n\n#### With non-keyword arguments\n```python\nfrom cmdy import tar\nprint(tar("cvf", "/tmp/test.tar", "./cmdy"))\n```\n\n#### With keyword arguments\n```python\nfrom cmdy import curl\ncurl("http://duckduckgo.com/", o="/tmp/page.html", silent=True)\n# curl http://duckduckgo.com/ -o /tmp/page.html --silent\n```\n\n#### Order keyword arguments\n```python\ncurl("http://duckduckgo.com/", "-o", "/tmp/page.html", "--silent")\n# or\n\nfrom diot import OrderedDiot\nkwargs = OrderedDiot()\nkwargs.silent = True\nkwargs.o = \'/tmp/page.html\'\ncurl("http://duckduckgo.com/", kwargs)\n# You can also use collections.OrderedDict\n```\n\n#### Prefix and separator for keyword arguments\n```python\nfrom cmdy import bedtools, bcftools\nbedtools.intersect(wa=True, wb=True,\n                   a=\'query.bed\', b=[\'d1.bed\', \'d2.bed\', \'d3.bed\'],\n                   names=[\'d1\', \'d2\', \'d3\'], sorted=True,\n                   _prefix=\'-\').h().strcmd\n# \'bedtools intersect -wa -wb -a query.bed \\\n# -b d1.bed d2.bed d3.bed -names d1 d2 d3 -sorted\'\n```\n\n```python\n# default prefix is auto\nbcftools.query(_=[\'a.vcf\', \'b.vcf\'], H=True,\n               format=\'%CHROM\\t%POS\\t%REF\\t%ALT\\n\').h().strcmd\n\n# "bcftools query -H --format \'%CHROM\\t%POS\\t%REF\\t%ALT\\n\' a.vcf b.vcf"\n\nls(l=True, block_size=\'KB\', _sep=\'auto\').h().cmd\n[\'ls\', \'-l\', \'--block-size=KB\']\n```\n\n#### Mixed combinations of prefices and separators in one command\n```python\nfrom cmdy import java\n# Note this is just an example for old verion picard.\n# Picard is changing it\'s style\n\npicard = java(jar=\'picard.jar\', _prefix=\'\', _sep=\'=\', _sub=True)\nc = picard.SortSam(I=\'input.bam\', O=\'sorted.bam\',\n               SORTED_ORDER=\'coordinate\',\n               _prefix=\'\', _sep=\'=\', _deform=None).h\nprint(c.cmd)\n\n# same as the above\njava({\'jar\': \'picard.jar\', \'_prefix\': \'-\', \'_sep\': \' \'},\n     \'SortSam\', I=\'input.bam\', O=\'sorted.bam\',\n     SORTED_ORDER=\'coordinate\', _prefix=\'\', _sep=\'=\', _deform=None).h().cmd\n\n# _deform prevents SORTED_ORDER to be deformed to SORTED-ORDER\n\n# [\'java\', \'jar=picard.jar\',\n#  \'SortSam\', \'I=input.bam\', \'O=sorted.bam\', \'SORTED_ORDER=coordinate\']\n```\n\n#### Subcommands\n\n```python\nfrom cmdy import git\ngit.branch(v=True).fg\n# <CmdyResult: [\'git\', \'branch\', \'-v\']>\n```\n\n```python\n# What if I have separate arguments for main and sub-command?\ngit(git_dir=\'.\', _sub=True).branch(v=True).h\n# <CmdyHolding: [\'git\', \'--git-dir\', \'.\', \'branch\', \'-v\']>\n```\n\n#### Duplicated keys for list arguments:\n```python\nfrom cmdy import sort\nprint(sort(k=[\'1,1\', \'2,2\'], t=\'_\', _=\'./.editorconfig\', _dupkey=True))\n# sort -k 1,1 -k 2,2 ./.editorconfig\n```\n\n### Return code and exception\n```python\nfrom cmdy import x\nx()\n```\n\n```python console\nTraceback (most recent call last):\n  File "<ipython-input-16-092cc5b72e61>", line 2, in <module>\n    x()\n/path/.../to/cmdy/__init__.py", line 146, in __call__\n    ready_cfgargs, ready_popenargs, _will())\n/path/.../to/cmdy/__init__.py", line 201, in __new__\n    result = holding.run()\n/path/.../to/cmdy/__init__.py", line 854, in run\n    return orig_run(self, wait)\n/path/.../to/cmdy/__init__.py", line 717, in run\n    return orig_run(self, wait)\n/path/.../to/cmdy/__init__.py", line 327, in run\n    ret = CmdyResult(self._run(), self)\n/path/.../to/cmdy/__init__.py", line 271, in _run\n    raise CmdyExecNotFoundError(str(fnfe)) from None\ncmdy.cmdy_util.CmdyExecNotFoundError: [Errno 2] No such file or directory: \'x\': \'x\'\n```\n\n```python\nfrom cmdy import ls\nls(\'non-existing-file\')\n```\n\n```python console\n\nTraceback (most recent call last):\n  File "<ipython-input-17-132683fc2227>", line 2, in <module>\n    ls(\'non-existing-file\')\n/path/.../to/cmdy/__init__.py", line 146, in __call__\n    ready_cfgargs, ready_popenargs, _will())\n/path/.../to/cmdy/__init__.py", line 204, in __new__\n    return result.wait()\n/path/.../to/cmdy/__init__.py", line 407, in wait\n    raise CmdyReturnCodeError(self)\ncmdy.cmdy_util.CmdyReturnCodeError: Unexpected RETURN CODE 2, expecting: [0]\n\n  [   PID] 167164\n\n  [   CMD] [\'ls non-existing-file\']\n\n  [STDOUT]\n\n  [STDERR] ls: cannot access non-existing-file: No such file or directory\n```\n\n#### Don\'t raise exception but store the return code\n```python\nfrom cmdy import ls\nresult = ls(\'non-existing-file\', _raise=False)\nresult.rc # 2\n```\n\n#### Tolerance on return code\n```python\nfrom cmdy import ls\n# or _okcode=[0,2]\nls(\'non-existing-file\', _okcode=\'0,2\').rc # 2\n```\n\n### Timeouts\n```python\nfrom cmdy import sleep\nsleep(3, _timeout=1)\n```\n\n```python console\nTraceback (most recent call last):\n  File "<ipython-input-20-47b0ec7af55f>", line 2, in <module>\n    sleep(3, _timeout=1)\n/path/.../to/cmdy/__init__.py", line 146, in __call__\n    ready_cfgargs, ready_popenargs, _will())\n/path/.../to/cmdy/__init__.py", line 204, in __new__\n    return result.wait()\n/path/.../to/cmdy/__init__.py", line 404, in wait\n    ) from None\ncmdy.cmdy_util.CmdyTimeoutError: Timeout after 1 seconds.\n```\n\n### Redirections\n```python\nfrom cmdy import cat\ncat(\'./pytest.ini\').redirect > \'/tmp/pytest.ini\'\nprint(cat(\'/tmp/pytest.ini\'))\n```\n\n#### Appending\n```python\n# r short for redirect\ncat(\'./pytest.ini\').r >> \'/tmp/pytest.ini\'\nprint(cat(\'/tmp/pytest.ini\')) # content doubled\n```\n\n#### Redirecting to a file handler\n```python\nwith open(\'/tmp/pytest.ini\', \'w\') as f\n    cat(\'./pytest.ini\').r > f\n\nprint(cat(\'/tmp/pytest.ini\'))\n```\n\n#### STDIN, STDOUT and/or STDERR redirections\n```python\nfrom cmdy import STDIN, STDOUT, STDERR, DEVNULL\n\nc = cat().r(STDIN) < \'/tmp/pytest.ini\'\nprint(c)\n```\n\n```python\n# Mixed\nc = cat().r(STDIN, STDOUT) ^ \'/tmp/pytest.ini\' > DEVNULL\n# we can\'t fetch result from a redirected pipe\nprint(c.stdout)\n\n# Why not \'<\' for STDIN?\n# Because the priority of the operator is not in sequential order.\n# We can use < for STDIN, but we need to ensure it runs first\nc = (cat().r(STDIN, STDOUT) < \'/tmp/pytest.ini\') > DEVNULL\nprint(c.stdout)\n\n# A simple rule for multiple redirections to always use ">" in the last place\n```\n\n```python\n# Redirect stderr to stdout\nfrom cmdy import bash\nc = bash(c="cat 1>&2").r(STDIN, STDERR) ^ \'/tmp/pytest.ini\' > STDOUT\nprint(c.stdout)\n```\n\n```python\n# Redirect the world\nc = bash(c="cat 1>&2").r(STDIN, STDOUT, STDERR) ^ \'/tmp/pytest.ini\' ^ DEVNULL > STDOUT\nprint(c.stdout) # None\nprint(c.stderr) # None\n```\n\n### Pipings\n```python\nfrom cmdy import grep\nc = ls().p | grep(\'README\')\nprint(c)\n# README.md\n# README.rst\n```\n\n```python\n# p short for pipe\nc = ls().p | grep(\'README\').p | grep(\'md\')\nprint(c) # README.md\nprint(c.piped_strcmds) # [\'ls\', \'grep README\', \'grep md\']\n```\n\n```python\nfrom cmdy import _CMDY_EVENT\n# !!! Pipings should be consumed immediately!\n# !!! DO NOT do this\nls().p\nls() # <- Will not run as expected\n# All commands will be locked as holding until pipings are consumed\n_CMDY_EVENT.clear()\nprint(ls()) # runs\n\n# See Advanced/Holdings if you want to hold a piping command for a while\n```\n\n### Running command in foreground\n```python\nls().fg\n```\n\n```python\nfrom cmdy import tail\ntail(\'/tmp/pytest.ini\', f=True, _timeout=3).fg\n# This mimics the `tail -f` program\n# You will see the content comes out one after another\n# and then program hangs for 3s\n```\n\nYou can also write an `echo-like` program easily. See \'[echo.py](./echo.py)\'\n\n### Iterating on output\n```python\nfor line in ls().iter():\n    print(line, end=\'\')\n```\n\n#### Iterating on stderr\n```python\nfor line in bash(c="cat /tmp/pytest.ini 1>&2").iter(STDERR):\n    print(line, end=\'\')\n```\n\n#### Getting live output\n```python\n# Like we did for `tail -f` program\n# This time, we can do something with each output line\n\n# Let\'s use a thread to write content to a file\n# And we try to get the live contents using cmdy\nimport time\nfrom threading import Thread\ndef live_write(file, n):\n\n    with open(file, \'w\', buffering=1) as f:\n        # Let\'s write something every half second\n        for i in range(n):\n            f.write(str(i) + \'\\n\')\n            time.sleep(.5)\n\ntest_file = \'/tmp/tail-f.txt\'\nThread(target=live_write, args=(test_file, 10)).start()\n\nfrom cmdy import tail\n\ntail_iter = tail(f=True, _=test_file).iter()\n\nfor line in tail_iter:\n    # Do whatever you want with the line\n    print(\'We got:\', line, end=\'\')\n    if line.strip() == \'8\':\n        break\n\n# make sure thread ends\ntime.sleep(2)\n```\n\n```python\n# What about timeout?\n\n# Of course you can use a timer to check inside the loop\n# You can also set a timeout for each fetch\n\n# Terminate after 10 queries\n\nThread(target=live_write, args=(test_file, 10)).start()\n\nfrom cmdy import tail\n\ntail_iter = tail(f=True, _=test_file).iter()\n\nfor i in range(10):\n    print(\'We got:\', tail_iter.next(timeout=1), end=\'\')\n```\n\n### Advanced\n#### Baking the `cmdy` object\n\nSometimes, you may want to run the same program a couple of times, with the same set of arguments or configurations, and you don\'t want to type those arguments every time, then you can bake the Cmdy object with that same arguments or configurations.\n\nFor example, if you want to run ls as ls -l all the time:\n\n```python\nfrom cmdy import ls\nll = ls._(l=True)\nprint(ll().h.cmd) # [\'ls\', \'-l\']\nprint(ll(a=True).h.cmd) # [\'ls\', \'-l\', \'-a\']\n# I don\'t want the l flag for some commands occasionally\nprint(ll(l=False).h.cmd) # [\'ls\']\n\n# Bake a baked command\nlla = ll._(a=True)\nprint(lla().h.cmd) # [\'ls\', \'-l\', \'-a\']\n```\n\n```python\n# I know git is always gonna run with subcommand\ngit = git._(_sub=True)\n# don\'t bother to pass _sub=True every time\nprint(git(git_dir=\'.\').branch(v=True).h)\n# <CmdyHolding: [\'git\', \'--git-dir\', \'.\', \'branch\', \'-v\']>\nprint(git().status().h)\n# <CmdyHolding: [\'git\', \'status\']>\n```\n\n```python\n# What if I have a subcommand call bake?\nfrom cmdy import git, CmdyActionError\n\nprint(git.branch().h.cmd) # [\'git\', \'branch\']\nprint(type(git._())) # <class \'cmdy.Cmdy\'>\n\n# run the git with _sub\nprint(git(_sub=True).bake().h.cmd) # [\'git\', \'bake\']\n```\n\n#### Baking the whole module\n```python\nimport cmdy\n# run version of the whole world\nsh = cmdy(version=True)\n# anything under sh directly will be supposed to have subcommand\nfrom sh import git, gcc\nprint(git().h)\n# <CmdyHolding: [\'git\', \'--version\']>\nprint(gcc().h)\n# <CmdyHolding: [\'gcc\', \'--version\']>\n```\n\nNote that module baking is deep copying, except the exception classes and some utils. This means, you would expect following behavior:\n\n```python\nimport cmdy\nfrom cmdy import CmdyHolding, CmdyExecNotFoundError\n\nsh = cmdy()\n\nc = sh.echo().h\nprint(type(c)) # <class \'cmdy.CmdyHolding\'>\nprint(isinstance(c, CmdyHolding)) # False\nprint(isinstance(c, sh.CmdyHolding)) # True\n\ntry:\n    sh.notexisting()\nexcept CmdyExecNotFoundError:\n    # we can catch it, as CmdyExecNotFoundError is sh.CmdyExecNotFoundError\n    print(\'Catched!\')\n```\n\n#### Holding objects\n\nYou may have noticed that we have a couple of examples above with a final call .h or .h(), which is holding the command from running.\n\nYou can do that, too, if you have multiple operations\n\n```python\nprint(ls().h) # <CmdyHolding: [\'ls\']>\n\n# however, you cannot hold after some actions\nls().r.h\n# CmdyActionError: Should be called in the first place: .h() or .hold()\n```\n\nOnce a command is on hold (by .h, .hold, .h() or .hold())\n\nYou have to explictly call run() to set the command running\n\n```python\nfrom time import time\ntic = time()\nc = sleep(2).h\nprint(f\'Time elapsed: {time() - tic:.3f} s\')\n# Time elapsed: 0.022 s\n\n# not running even with fg\nc.fg\nprint(f\'Time elapsed: {time() - tic:.3f} s\')\n# Time elapsed: 0.034 s\nc.run()\nprint(f\'Time elapsed: {time() - tic:.3f} s\')\n# Time elapsed: 2.043 s\n```\n\n#### Reuse of command\n```python\n# After you set a command running,\n# you can retrieve the holding object,\n# and reuse it\nfrom cmdy import ls\nc = ls().fg\n# nothing will be produced\nc.holding.reset().r > DEVNULL\n```\n\n#### Async mode\n```python\nimport curio\nfrom cmdy import ls\na = ls().a # async command is never blocking!\n\nasync def main():\n    async for line in a:\n        print(line, end=\'\')\n\ncurio.run(main())\n```\n\n#### Extending `cmdy`\n\nAll those actions for holding/result objects were implemented internally as plugins. You can right your own plugins, too.\n\nA plugin has to be defined as a class and then instantiated.\n\n**There are 5 APIs for developing a plugin for `cmdy`**\n\n- `cmdy._plugin_factory.register`: A decorator for the plugin class\n- `cmdy._plugin_factory.hold_then`: A decorator to decorate methods in the plugin class, which define actions after a holding object. Arguments:\n  - `alias`: The alias of this action (e.g. `r/redir` for `redirect`)\n  - `final`: Whether this is a final action, meaning no other actions should be followed\n  - `prop`: Whether this action can be called as a property\n  - `hold_right`: Should I put right following action on hold? This is useful when we have connectors which then can set the command running. (e.g `>` for redirect and `|` for pipe)\n- `cmdy._plugin_factory.run_then`: A decorator to decorate methods in the plugin class, which define actions after a sync result object. Arguments are similar as `cmdy._plugin_factory.hold_then` except that `prop` and `hold_right` are not avaialbe.\n- `async_run_then.add_method`: A decorator to decorate methods in the plugin class, which add methods to the `CmdyHolding`, `CmdyResult` or `CmdyAsyncResult` class. `cls` is the only argument that specifies which class we are hacking.\n- `async_run_then.add_property`: Property version of `cmdy_plugin_add_method`\n\n**Notes on name conflicts:**\n\nIf we need to add the methods to multiple classes in the plugin with the same name, you can define a different name with extra underscore suffix(es).\n\n**Notes on module baking:**\n\n- Always use the baked module to get those classes\n    ```pytho\n    import cmdy\n    cmdy2 = cmdy()\n\n    @cmdy2._plugin_factory.register\n    class MyPlugin:\n        ...\n    ```\n- Plugin enable and disable only take effect within the same module. For example:\n\n    ```python\n    import cmdy\n    sh = cmdy()\n    # only affects cmdy not sh\n    sh._plugins.fg.disable()\n    # to disable this plugin for sh as well:\n    sh._plugins.fg.disable()\n    ```\n\n```python\n# An example to define a plugin\nimport cmdy\n\n@cmdy._plugin_factory.register\nclass MyPlugin:\n    @cmdy._plugin_factory.add_method(cmdy.CmdyHolding)\n    def say_hello(self):\n        return \'Hello world!\'\n\n    @cmdy._plugin_factory.hold_then(\'hello\')\n    def helloworld(self):\n        print(self.say_hello())\n        # keep chaining\n        return self\n\nmyplugin = MyPlugin()\n\n# command will never run,\n# because we didn\'t do self.run() in helloworld(self)\nls().helloworld()  # prints Hello world!\n# property calls enabled by default\nls().helloworld  # prints Hello world!\n# we have alias\nls().hello  # prints Hello world!\n\n```\n\n[1]: https://img.shields.io/pypi/v/cmdy?style=flat-square\n[2]: https://pypi.org/project/cmdy/\n[3]: https://img.shields.io/github/tag/pwwang/cmdy?style=flat-square\n[4]: https://github.com/pwwang/cmdy\n[5]: https://img.shields.io/travis/pwwang/cmdy?style=flat-square\n[6]: https://travis-ci.org/pwwang/cmdy\n[7]: https://img.shields.io/codacy/grade/fa12f06d39404f98b94c19e83865fd4e?style=flat-square\n[8]: https://app.codacy.com/project/pwwang/cmdy/dashboard\n[9]: https://img.shields.io/codacy/coverage/fa12f06d39404f98b94c19e83865fd4e?style=flat-square\n[10]: https://img.shields.io/pypi/pyversions/cmdy?style=flat-square\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/cmdy',
```

### Comparing `cmdy-0.5.4/PKG-INFO` & `cmdy-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cmdy
-Version: 0.5.4
+Version: 0.5.5
 Summary: Shell language to run command in python
 Home-page: https://github.com/pwwang/cmdy
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: curio (>=1.6,<2.0)
-Requires-Dist: python-simpleconf[toml] (>=0.5,<0.6)
+Requires-Dist: python-simpleconf[toml] (>=0.6,<0.7)
 Requires-Dist: varname (>=0.10,<0.11) ; python_version < "3.8"
 Requires-Dist: varname (>=0.11,<0.12) ; python_version >= "3.8" and python_version < "4.0"
 Project-URL: Repository, https://github.com/pwwang/cmdy
 Description-Content-Type: text/markdown
 
 # cmdy
 "Shell language" to run command in python
```

