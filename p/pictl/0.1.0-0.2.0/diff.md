# Comparing `tmp/pictl-0.1.0.tar.gz` & `tmp/pictl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictl-0.1.0.tar", max compression
+gzip compressed data, was "pictl-0.2.0.tar", max compression
```

## Comparing `pictl-0.1.0.tar` & `pictl-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-06-03 13:02:39.998029 pictl-0.1.0/LICENSE
--rw-r--r--   0        0        0     2524 2023-06-13 13:29:39.030421 pictl-0.1.0/README.md
--rw-r--r--   0        0        0      375 2023-06-05 04:51:32.185620 pictl-0.1.0/pictl/__init__.py
--rw-r--r--   0        0        0       77 2023-06-05 04:48:36.217133 pictl-0.1.0/pictl/cli/__init__.py
--rw-r--r--   0        0        0     2509 2023-06-13 13:26:40.481800 pictl-0.1.0/pictl/cli/main.py
--rw-r--r--   0        0        0       81 2023-06-04 06:47:00.665547 pictl-0.1.0/pictl/config/__init__.py
--rw-r--r--   0        0        0     5737 2023-06-13 08:17:30.305473 pictl-0.1.0/pictl/config/config.py
--rw-r--r--   0        0        0       90 2023-06-04 12:42:32.939767 pictl-0.1.0/pictl/pic/__init__.py
--rw-r--r--   0        0        0      788 2023-06-13 13:19:05.300217 pictl-0.1.0/pictl/pic/pic.py
--rw-r--r--   0        0        0      128 2023-06-04 13:12:45.748457 pictl-0.1.0/pictl/upload/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-13 13:22:46.704987 pictl-0.1.0/pictl/upload/upload.py
--rw-r--r--   0        0        0      151 2023-06-04 13:38:46.000398 pictl-0.1.0/pictl/utils/__init__.py
--rw-r--r--   0        0        0      958 2023-06-04 13:22:52.114022 pictl-0.1.0/pictl/utils/utils.py
--rw-r--r--   0        0        0      555 2023-06-13 13:33:09.259152 pictl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 pictl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 06:25:56.664657 pictl-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3651 2023-06-27 06:25:56.664657 pictl-0.2.0/README.md
+-rw-r--r--   0        0        0      375 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/cli/__init__.py
+-rw-r--r--   0        0        0     2979 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/cli/main.py
+-rw-r--r--   0        0        0      133 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/__init__.py
+-rw-r--r--   0        0        0     4308 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/config.py
+-rw-r--r--   0        0        0     1400 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/regions.py
+-rw-r--r--   0        0        0       90 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/pic/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/pic/pic.py
+-rw-r--r--   0        0        0      128 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/upload/__init__.py
+-rw-r--r--   0        0        0     1763 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/upload/upload.py
+-rw-r--r--   0        0        0      271 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/utils/__init__.py
+-rw-r--r--   0        0        0     1473 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/utils/utils.py
+-rw-r--r--   0        0        0      558 2023-06-27 06:25:56.664657 pictl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 pictl-0.2.0/PKG-INFO
```

### Comparing `pictl-0.1.0/LICENSE` & `pictl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pictl-0.1.0/README.md` & `pictl-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # pictl
 
 A command line tool for Image Compression and Upload (ex. S3-type)
 
+![PyPI](https://img.shields.io/pypi/v/pictl)
+![GitHub](https://img.shields.io/github/license/zhonger/pictl)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/zhonger/pictl)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pictl)
+
+![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/zhonger/pictl)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/zhonger/pictl/python-publish.yml)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pictl)
+
+Engligh | [中文简体](https://lisz.me/tech/project/pictl.html)
+
 ## Why a new project
 
 When I publish blog articles, it's quite inefficient for me to prepare images.
 
 Although there exist many good enough tools, like [uPic](https://github.com/gee1k/uPic), [PicGo](https://github.com/Molunerfinn/PicGo), and so on, they still cannot meet my need completely.
 
 For me, these points are very necessary:
@@ -53,33 +64,64 @@
 
 ```bash
 pip3 install pictl
 ```
 
 ### Brew
 
+(~~**PS**: It will support in the next version.~~ Now it's supported in MacOS. Linux is not available yet.)
+
 ```bash
 brew tap zhonger/pictl
 brew install pictl
 ```
 
 ## Usage
 
 ### Config
 
-The config file for PICTL is named `.pictlrc` with `toml` format. The global config file is located at `~/.pictlrc`. The local config file is located at `./.pictlrc`. If there is a local config file, it will be used firstly. If the necessary settings cannot be found in the local config file, the settings in the global config file will be used instead.
+The config file for PICTL is named `.pictlrc` with `toml` format. The config file is located at `~/.pictlrc`.
+
+Until now PICTL supports:
+
+| Name | `type` in config |
+| :--: | :--: |
+| Cloudflare R2 | `R2` |
+| AWS S3 | `S3` |
+| Tencent COS | `COS(Tencent)` |
 
 #### Manually
 
 ```bash
 [basic]
 length = 6
+ntype = "random"
 algorithm = "sha1"
 
-[upload]
-endpoint = "https://s3.amazonaws.com"
-key = "qwqewqwqeqweqwe"
-secret = "dadfadaeqweqeqe"
+[blog]
+type = "S3"
+endpoint = "https://s3.ap-northeast-1.amazonaws.com"
+bucket = "blog"
+region = "ap-northeast-1"
+prefix = "blog"
+key = "this-is-a-long-key-for-s3"
+secret = "this-is-a-long-secret-for-s3"
 url = "https://i.lisz.me"
 ```
 
 ### Interactive way
+
+```bash
+╰─$ pictl config
+Usage: pictl config [OPTIONS] COMMAND [ARGS]...
+
+  Operations for the config file `~/.pictlrc`.
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  add     Add configs to the config file.
+  delete  Delete config group from the config file.
+  info    Check the configs.
+  init    Initialize config file with default configs
+```
```

### Comparing `pictl-0.1.0/pictl/cli/main.py` & `pictl-0.2.0/pictl/cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,42 +29,58 @@
     is_flag=True,
 )
 def cli():
     """A command line tool for image processing and uploading (ex. S3-type).
 
     \b
     Now it supports:
-      - transformation from other image types to `webp` image as well as 
+      - transformation from other image types to `webp` image as well as
         image compression.
       - image file uploading to AWS S3 or Cloudflare R2.
     """
 
 
 @click.group()
 def config():
     """Operations for the config file `~/.pictlrc`."""
 
 
 @config.command()
 def info():
     """Check the configs."""
-    rprint(Config().read())
+    try:
+        c = Config()
+        settings = c.read()
+        rprint(settings)
+    except FileNotFoundError:
+        rprint(f"{c.rc} doesn't exsit. Please check it.")
 
 
 @config.command()
 def add():
     """Add configs to the config file."""
-    Config().add()
+    try:
+        c = Config()
+        c.read()
+        c.add()
+    except FileNotFoundError:
+        c.init()
+        c.add()
 
 
 @config.command()
 @click.option("-g", "--group", help="The specified group name.")
 def delete(group: str = None):
     """Delete config group from the config file."""
-    Config().delete(group)
+    try:
+        c = Config()
+        c.read()
+        c.delete(group)
+    except FileNotFoundError:
+        rprint(f"{c.rc} doesn't exsit. Please check it.")
 
 
 @config.command()
 def init():
     """Initialize config file with default configs."""
     Config().init()
 
@@ -82,20 +98,21 @@
     output = pcom(filename)
     if output is not None:
         pup(output, group)
 
 
 @click.command()
 @click.argument("filename")
-def compress(filename):
+@click.option("-o", "--output", help="The output filename.")
+def compress(filename, output: str = None):
     """Compress any image into `webp` image.
 
     FILENAME is the name of the file to compress.
     """
-    pcom(filename)
+    pcom(filename, output)
 
 
 @click.command()
 @click.argument("filename")
 @click.argument("group")
 def upload(filename: str, group: str):
     """Upload the file to remote storage.
```

### Comparing `pictl-0.1.0/pictl/pic/pic.py` & `pictl-0.2.0/pictl/pic/pic.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,33 @@
 from PIL import Image
 from rich import print as rprint
 
 from pictl.config import Config
 from pictl.utils import get_name
 
 
-def compress(filename: str):
+def compress(fi: str, fo: str = None):
     """Compress any image into `webp` image.
 
-    FILENAME is the name of the file to compress.
+    FI is the name of the input file.
+    FO is the name of the output file.
     """
-    settings = Config().read()
-    optimize = settings["basic"].get("optimize", True)
-    quality = settings["basic"].get("quality", 75)
     try:
-        imgfile = Image.open(filename).convert("RGB")
-        filename = f"{get_name(filename)}.webp"
+        settings = Config().read()
+        optimize = settings["basic"].get("optimize", True)
+        quality = settings["basic"].get("quality", 75)
+    except FileNotFoundError:
+        optimize = True
+        quality = 75
+
+    try:
+        imgfile = Image.open(fi).convert("RGB")
+        if fo:
+            filename = f"{fo}.webp"
+        else:
+            filename = f"{get_name(fi)}.webp"
         imgfile.save(filename, "webp", optimize=optimize, quality=quality)
         rprint(f"The output file is {filename}")
         return filename
     except FileNotFoundError:
-        rprint(f"{filename} doesn't exsit. Please check it again.")
+        rprint(f"{fi} doesn't exsit. Please check it again.")
         return None
```

### Comparing `pictl-0.1.0/pictl/upload/upload.py` & `pictl-0.2.0/pictl/upload/upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Upload module"""
 
 import boto3
 from rich import print as rprint
 
 from pictl.config import Config
-
+from pictl.utils import get_content_type, get_object_key
 
 
 def upload(filename: str, group: str) -> None:
     """Upload the file to remote storage.
 
     \b
     FILENAME is the name of the file to upload.
@@ -22,28 +22,34 @@
             groups.remove("basic")
         rprint(f"Please choose one group from below:\n  {groups}")
     else:
         upload_s3(settings, filename, group)
 
 
 def upload_s3(settings: dict, filename: str, group: str):
-    s3 = boto3.resource(
-        "s3",
-        endpoint_url=settings[group]["endpoint"],
-        aws_access_key_id=settings[group]["key"],
-        aws_secret_access_key=settings[group]["secret"],
-    )
+    resource = {
+        "endpoint_url": settings[group]["endpoint"],
+        "aws_access_key_id": settings[group]["key"],
+        "aws_secret_access_key": settings[group]["secret"],
+        "region_name": settings[group]["region"],
+    }
+    s3 = boto3.resource("s3", **resource)
     with open(filename, "rb") as data:
-        s3.Bucket(settings[group]["prefix"]).put_object(Key=filename, Body=data)
+        content_type = get_content_type(filename)
+        key = get_object_key(filename, settings[group]["prefix"])
+        s3.Bucket(settings[group]["bucket"]).put_object(
+            Key=key,
+            Body=data,
+            ContentType=content_type,
+        )
         get_link(settings, filename, group)
 
 
 def get_link(settings: dict, filename: str, group: str):
-    if settings[group]["prefix"] == "":
-        url = f'{settings[group]["url"]}/{filename}'
-    else:
-        url = f'{settings[group]["url"]}/{settings[group]["prefix"]}/{filename}'
-    rprint(
+    key = get_object_key(filename, settings[group]["prefix"])
+    url = f'{settings[group]["url"]}/{key}'
+    filename = filename.split("/")[-1]
+    print(
         f"Direct URL: {url}\n"
         f"Markdown: ![{filename}]({url})\n"
         f'HTML Code: <img src="{url}" alt="{filename}" />\n'
     )
```

### Comparing `pictl-0.1.0/pictl/utils/utils.py` & `pictl-0.2.0/pictl/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Tools module"""
 
 import hashlib
+import mimetypes
 import random
 import string
 
 from pictl.config import Config
 
 
 def get_name(filename: str):
-    settings = Config().read()
-    ntype = settings["basic"].get("ntype", None)
-    length = settings["basic"].get("length", 8)
-    algorithm = settings["basic"].get("algorithm", "sha1")
+    try:
+        settings = Config().read()
+        ntype = settings["basic"].get("ntype", None)
+        length = settings["basic"].get("length", 6)
+        algorithm = settings["basic"].get("algorithm", "sha1")
+    except FileNotFoundError:
+        ntype = None
+        length = 6
+        algorithm = "sha1"
     if ntype == "random":
         name = get_random_name(length)
     elif ntype == "hash":
         name = get_hash_name(filename, algorithm, length)
     else:
         name = filename.split(".")[0]
     return name
@@ -31,7 +37,21 @@
 
 
 def get_hash_name(filename: str, algorithm: str = "sha1", length: int = 8):
     with open(filename, "rb") as f:
         value = hashlib.new(algorithm, f.read()).hexdigest()
         name = value[:length].upper()
     return name
+
+
+def get_content_type(filename: str):
+    mimetypes.types_map[".webp"]="image/webp"
+    if mimetypes.guess_type(filename)[0]:
+        return mimetypes.guess_type(filename)[0]
+    return "binary/octet-stream"
+
+
+def get_object_key(filename: str, prefix: str):
+    filename = filename.split("/")[-1]
+    if prefix:
+        return f"{prefix}/{filename}"
+    return f"{filename}"
```

### Comparing `pictl-0.1.0/pyproject.toml` & `pictl-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pictl"
-version = "0.1.0"
+version = "0.2.0"
 description = "A command line tool for image processing and uploading (ex. S3-type)"
 authors = ["zhonger <zhonger@live.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Pillow = "^9.3.0"
-rtoml = "^0.9.0"
 inquirer = "^3.1.3"
 rich = "^13.4.1"
 click = "^8.1.3"
 boto3 = "^1.26.146"
+tomlkit = "^0.11.8"
 
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pictl-0.1.0/PKG-INFO` & `pictl-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 Metadata-Version: 2.1
 Name: pictl
-Version: 0.1.0
+Version: 0.2.0
 Summary: A command line tool for image processing and uploading (ex. S3-type)
 License: MIT
 Author: zhonger
 Author-email: zhonger@live.cn
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
 Requires-Dist: boto3 (>=1.26.146,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
-Requires-Dist: rtoml (>=0.9.0,<0.10.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # pictl
 
 A command line tool for Image Compression and Upload (ex. S3-type)
 
+![PyPI](https://img.shields.io/pypi/v/pictl)
+![GitHub](https://img.shields.io/github/license/zhonger/pictl)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/zhonger/pictl)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pictl)
+
+![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/zhonger/pictl)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/zhonger/pictl/python-publish.yml)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pictl)
+
+Engligh | [中文简体](https://lisz.me/tech/project/pictl.html)
+
 ## Why a new project
 
 When I publish blog articles, it's quite inefficient for me to prepare images.
 
 Although there exist many good enough tools, like [uPic](https://github.com/gee1k/uPic), [PicGo](https://github.com/Molunerfinn/PicGo), and so on, they still cannot meet my need completely.
 
 For me, these points are very necessary:
@@ -73,34 +84,65 @@
 
 ```bash
 pip3 install pictl
 ```
 
 ### Brew
 
+(~~**PS**: It will support in the next version.~~ Now it's supported in MacOS. Linux is not available yet.)
+
 ```bash
 brew tap zhonger/pictl
 brew install pictl
 ```
 
 ## Usage
 
 ### Config
 
-The config file for PICTL is named `.pictlrc` with `toml` format. The global config file is located at `~/.pictlrc`. The local config file is located at `./.pictlrc`. If there is a local config file, it will be used firstly. If the necessary settings cannot be found in the local config file, the settings in the global config file will be used instead.
+The config file for PICTL is named `.pictlrc` with `toml` format. The config file is located at `~/.pictlrc`.
+
+Until now PICTL supports:
+
+| Name | `type` in config |
+| :--: | :--: |
+| Cloudflare R2 | `R2` |
+| AWS S3 | `S3` |
+| Tencent COS | `COS(Tencent)` |
 
 #### Manually
 
 ```bash
 [basic]
 length = 6
+ntype = "random"
 algorithm = "sha1"
 
-[upload]
-endpoint = "https://s3.amazonaws.com"
-key = "qwqewqwqeqweqwe"
-secret = "dadfadaeqweqeqe"
+[blog]
+type = "S3"
+endpoint = "https://s3.ap-northeast-1.amazonaws.com"
+bucket = "blog"
+region = "ap-northeast-1"
+prefix = "blog"
+key = "this-is-a-long-key-for-s3"
+secret = "this-is-a-long-secret-for-s3"
 url = "https://i.lisz.me"
 ```
 
 ### Interactive way
 
+```bash
+╰─$ pictl config
+Usage: pictl config [OPTIONS] COMMAND [ARGS]...
+
+  Operations for the config file `~/.pictlrc`.
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  add     Add configs to the config file.
+  delete  Delete config group from the config file.
+  info    Check the configs.
+  init    Initialize config file with default configs
+```
+
```

