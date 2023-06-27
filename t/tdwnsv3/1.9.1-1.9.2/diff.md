# Comparing `tmp/tdwnsv3-1.9.1.tar.gz` & `tmp/tdwnsv3-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdwnsv3-1.9.1.tar", last modified: Fri Jun 23 13:10:49 2023, max compression
+gzip compressed data, was "tdwnsv3-1.9.2.tar", last modified: Tue Jun 27 12:15:56 2023, max compression
```

## Comparing `tdwnsv3-1.9.1.tar` & `tdwnsv3-1.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 13:10:48.966000 tdwnsv3-1.9.1/
--rw-rw----   0 root         (0) everybody  (9997)     1070 2023-02-20 13:15:55.000000 tdwnsv3-1.9.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     8287 2023-06-23 13:10:48.946000 tdwnsv3-1.9.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     7313 2023-06-23 13:07:26.000000 tdwnsv3-1.9.1/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-23 13:10:48.966000 tdwnsv3-1.9.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1364 2023-06-23 13:08:12.000000 tdwnsv3-1.9.1/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 13:10:48.754000 tdwnsv3-1.9.1/tdwnsv3/
--rw-rw----   0 root         (0) everybody  (9997)     1317 2023-06-23 13:01:50.000000 tdwnsv3-1.9.1/tdwnsv3/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-04-18 16:36:08.000000 tdwnsv3-1.9.1/tdwnsv3/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     2273 2023-02-20 13:15:56.000000 tdwnsv3-1.9.1/tdwnsv3/ciphersuite.py
--rw-rw----   0 root         (0) everybody  (9997)    14899 2023-02-20 13:15:56.000000 tdwnsv3-1.9.1/tdwnsv3/fav.py
--rw-rw----   0 root         (0) everybody  (9997)     8838 2023-03-08 02:19:44.000000 tdwnsv3-1.9.1/tdwnsv3/html_prettier.py
--rw-rw----   0 root         (0) everybody  (9997)     2079 2023-02-21 12:22:35.000000 tdwnsv3-1.9.1/tdwnsv3/javascript.py
--rw-rw----   0 root         (0) everybody  (9997)     2962 2023-02-20 13:15:56.000000 tdwnsv3-1.9.1/tdwnsv3/sec_server.py
--rw-rw----   0 root         (0) everybody  (9997)    10411 2023-04-09 10:15:10.000000 tdwnsv3-1.9.1/tdwnsv3/style.py
--rw-rw----   0 root         (0) everybody  (9997)    20400 2023-04-18 16:36:08.000000 tdwnsv3-1.9.1/tdwnsv3/tdwnsv3.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 13:10:48.930000 tdwnsv3-1.9.1/tdwnsv3.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     8287 2023-06-23 13:10:47.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      397 2023-06-23 13:10:48.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-23 13:10:47.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-23 13:10:47.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-23 13:10:47.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-23 13:10:47.000000 tdwnsv3-1.9.1/tdwnsv3.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:56.127000 tdwnsv3-1.9.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1070 2023-02-20 13:15:55.000000 tdwnsv3-1.9.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     8283 2023-06-27 12:15:56.039000 tdwnsv3-1.9.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     7309 2023-06-27 12:14:03.000000 tdwnsv3-1.9.2/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-27 12:15:56.127000 tdwnsv3-1.9.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1364 2023-06-27 12:11:46.000000 tdwnsv3-1.9.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:55.711000 tdwnsv3-1.9.2/tdwnsv3/
+-rw-rw----   0 root         (0) everybody  (9997)     1317 2023-06-27 12:11:26.000000 tdwnsv3-1.9.2/tdwnsv3/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-04-18 16:36:08.000000 tdwnsv3-1.9.2/tdwnsv3/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2273 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/ciphersuite.py
+-rw-rw----   0 root         (0) everybody  (9997)    14899 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/fav.py
+-rw-rw----   0 root         (0) everybody  (9997)     9381 2023-06-26 20:14:20.000000 tdwnsv3-1.9.2/tdwnsv3/html_prettier.py
+-rw-rw----   0 root         (0) everybody  (9997)     2079 2023-02-21 12:22:35.000000 tdwnsv3-1.9.2/tdwnsv3/javascript.py
+-rw-rw----   0 root         (0) everybody  (9997)     2962 2023-02-20 13:15:56.000000 tdwnsv3-1.9.2/tdwnsv3/sec_server.py
+-rw-rw----   0 root         (0) everybody  (9997)    13343 2023-06-27 07:33:54.000000 tdwnsv3-1.9.2/tdwnsv3/style.py
+-rw-rw----   0 root         (0) everybody  (9997)    20403 2023-06-27 07:38:01.000000 tdwnsv3-1.9.2/tdwnsv3/tdwnsv3.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 12:15:56.019000 tdwnsv3-1.9.2/tdwnsv3.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     8283 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      397 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-27 12:15:54.000000 tdwnsv3-1.9.2/tdwnsv3.egg-info/top_level.txt
```

### Comparing `tdwnsv3-1.9.1/LICENSE` & `tdwnsv3-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.1/PKG-INFO` & `tdwnsv3-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdwnsv3
-Version: 1.9.1
+Version: 1.9.2
 Summary: Simple local-files server with security on top!
 Home-page: https://github.com/Simatwa/tdwnsv3
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT
@@ -17,29 +17,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">tdwnsv3</h1>
 
-<div align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
+<p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
 
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.1&color=yellow&logo=pypi" alt="pypi"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 
 <a href="#"><img src="https://visitor-badge.glitch.me/badge?page_id=Simatwa.tdwnsv3&left_color=red&right_color=lime&left_text=Counts" alt="Visitors"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 
-</div>
+</p>
 
 
 
 > Access your files on the web.
```

### Comparing `tdwnsv3-1.9.1/README.md` & `tdwnsv3-1.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <h1 align="center">tdwnsv3</h1>
-<div align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.1&color=yellow&logo=pypi" alt="pypi"/></a>
+<p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 <a href="#"><img src="https://visitor-badge.glitch.me/badge?page_id=Simatwa.tdwnsv3&left_color=red&right_color=lime&left_text=Counts" alt="Visitors"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
-</div>
+</p>
 
 > Access your files on the web.
 
 ![Web interface sample](https://github.com/Simatwa/tdwnsv3/raw/main/assets/web_interface_example.gif)
 
 ## [Independencies](https://github.com/Simatwa/tdwnsv3/raw/main/requirements.txt)
```

### Comparing `tdwnsv3-1.9.1/setup.py` & `tdwnsv3-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 __info__ = "Simple local-files server with security on top!"
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __author__ = "Smartwa Caleb"
 __email__ = "smartwacaleb@gmail.com"
 __repo__ = "https://github.com/Simatwa/tdwnsv3"
 
 
 def get_file(nm: str) -> list:
     with open(nm, encoding="utf-8") as fp:
```

### Comparing `tdwnsv3-1.9.1/tdwnsv3/__init__.py` & `tdwnsv3-1.9.2/tdwnsv3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __info__ = "Simple local-files server with security on top!"
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __author__ = "Smartwa Caleb"
 __email__ = "smartwacaleb@gmail.com"
 __repo__ = "https://github.com/Simatwa/tdwnsv3"
 
 __all__ = [
     "tdwnsv3",
     "app",
```

### Comparing `tdwnsv3-1.9.1/tdwnsv3/ciphersuite.py` & `tdwnsv3-1.9.2/tdwnsv3/ciphersuite.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.1/tdwnsv3/fav.py` & `tdwnsv3-1.9.2/tdwnsv3/fav.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.1/tdwnsv3/html_prettier.py` & `tdwnsv3-1.9.2/tdwnsv3/html_prettier.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,28 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import os, urllib, html
 
 
+def make_navigator(dir, home_dir):
+    # dir = "DCIM/Bugjaege/hello"
+    resp = f'<a class="listed_dir" href="/{home_dir}/home">Home</a>'
+    splitted = dir.split("/")
+    for x in range(len(splitted)):
+        if len(splitted) == 1 or not bool(splitted[x].strip()):
+            break
+        url = os.path.join(*["/" + home_dir] + splitted[: x + 1])
+        resp = resp + "/" + f'<a class="listed_dir" href="{url}/">{splitted[x]}</a>'
+    return resp
+
+
+# out = make_navigator("","files")
+# print(out)
 def prettify(
     contents: list, path: str, dir: str, args: object, config: dict, encryptor: object
 ) -> str:
     r = []
     enc = "utf-8"
     static = config["static"]
     fmtlink = lambda uri: encryptor.handle_cipher(
@@ -56,15 +70,15 @@
     r.append(
         '<meta content="width=width-device, initial-scale=1.0" name="viewport"></meta>'
         f'<link rel="icon" type="image/x-icon" href="/{static}/favicon.ico"></link>'
         f'<link rel="stylesheet" href="/{static}/style/style.css"></link>'
         f'<script type="text/javascript" src="/{static}/javascript/script.js"></script>'
     )
     r.append("<title>Directory %s</title></head>" % dir)
-    r.append("<body><h1>%s</h1><hr/>" % title)
+    r.append("<body><p class='nav'>%s</p;><hr/>" % make_navigator(dir, config["home"]))
 
     preload = "none"
     if args.preload:
         preload = "metadata"
     for name in contents:
         fullname = os.path.join(path, name)
         displayname = linkname = name
```

### Comparing `tdwnsv3-1.9.1/tdwnsv3/javascript.py` & `tdwnsv3-1.9.2/tdwnsv3/javascript.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.1/tdwnsv3/sec_server.py` & `tdwnsv3-1.9.2/tdwnsv3/sec_server.py`

 * *Files identical despite different names*

### Comparing `tdwnsv3-1.9.1/tdwnsv3/style.py` & `tdwnsv3-1.9.2/tdwnsv3/style.py`

 * *Files 14% similar despite different names*

```diff
@@ -448,14 +448,205 @@
     padding: 10px;
     color: #666;
     text-align: center;
     font-size: 14px;
     border-top: 1px solid #ddd;
 }
 """
+data3 = """
+
+body{
+    background-color: #f2f2f2;
+    font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+    text-align:center;
+    
+}
+
+h3{
+ background-color:red;
+ color:lime;
+ padding:5px;
+ margin-left: 30%;
+ margin-right: 30%;
+ border-radius:2px;
+}
+
+p.nav{
+    position:sticky;
+    top:0;
+    margin-left:0;
+    margin-right:0;
+    padding:20px;
+    background-color:#fff;
+    clear:both;
+    font-size:1.6rem;
+    border-bottom: 1px solid #ddd;
+}
+
+.header{
+    color: #222;
+    text-decoration: none;
+}
+
+a{
+    text-decoration:none;
+}
+
+a.listed_dir{
+ background-color:blue;
+ padding:5px;
+ border-radius:10px;
+ color:lightgreen;
+ font-size:20px;
+}
+
+div.folders{
+    background-color: #fff;
+    padding: 10px;
+    border: 1px solid #ddd;
+}
+
+button{
+    background-color: lightgreen;
+    margin: 5px;
+    font-size: 14px;
+    border: 1px solid #ddd;
+    padding: 8px 16px;
+    border-radius: 4px;
+}
+
+.dir{
+    color: #222;
+    font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+    font-weight: bold;
+}
+
+a.dir{
+  color : black;
+}
+
+a.file{
+  color:darkgreen;
+  
+}
+
+/*button > a.dir:hover*/
+button:hover, a.dir:hover{
+    background-color:yellow;
+    color:red;
+    }
+
+#cp{
+    background-color: #fff;
+    width: 60%;
+    font-size: 16px;
+    border-radius: 20px;
+    font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+    padding: 10px;
+    color: #222;
+    border: 1px solid #ddd;
+    /* display:none; */
+}
+
+input#cp{
+    text-align: center;
+    padding: 10px;
+    height: 0.2cm;
+}
+
+input#cp:focus{
+   height:0.8cm;
+   border:1px solid blue;
+ }
+
+.vida,.pic,.aud{
+    display: inline-block;
+    margin: 5px;
+    max-width: 320px;
+}
+
+p.doc{
+    display: inline-block;
+    color: #222;
+    font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+    max-width: 340px;
+}
+
+/*
+.vida{
+    max-width:320px;
+
+} */
+
+video{
+    border:none;
+    background-color: 000;
+    border-radius: 4px;
+    width: 100%;
+    height: auto;
+}
+
+img, video{
+    max-width:100%;
+    height: auto;
+    
+}
+
+audio{
+    height: 50px;
+    width:100%;
+}
+
+.aud{
+    background-color: #fff;
+    color: #222;
+    padding: 10px;
+    margin-top: 10px;
+    border: 1px solid #ddd;
+    min-width:300px;
+    max-width:300px;
+}
+
+li.doc{
+    display: inline-block;
+    color: #222;
+    background-color: #fff;
+    padding: 10px;
+    border-radius: 4px;
+    margin: 7px;
+    font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
+}
+
+.but{
+    background-color: #fff;
+    padding: 4px;
+    border-radius: 8px;
+}
+
+marquee{
+    margin:5px;
+    font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;
+    font-size:14px;
+    color:#222;
+}
+
+footer{
+  /*  position: fixed; */
+    bottom: 0;
+    width: 100%;
+    background-color: #f2f2f2;
+    padding: 10px;
+    color: #666;
+    text-align: center;
+    font-size: 14px;
+    border-top: 1px solid #ddd;
+    /*margin-top:100vh;*/
+}
+"""
 
 
 class style_handler:
     def __init__(self, log: object, args: object):
         self.val = args.theme
         self.fnm = args.css
         self.log = log
@@ -521,9 +712,10 @@
                 fp = self.open_file()
                 if fp[0]:
                     return fp[1]
             css1 = {
                 1: data,
                 2: data1,
                 3: data2,
+                4: data3,
             }
             return css1[self.val]
```

### Comparing `tdwnsv3-1.9.1/tdwnsv3/tdwnsv3.py` & `tdwnsv3-1.9.2/tdwnsv3/tdwnsv3.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,17 +98,17 @@
         default=45,
     )
     parser.add_argument(
         "-th",
         "--theme",
         help="Theme for displaying contents",
         type=int,
-        choices=[1, 2, 3],
-        metavar="[1-3]",
-        default=3,
+        choices=[1, 2, 3, 4],
+        metavar="[1-4]",
+        default=4,
     )
     parser.add_argument("-cs", "--css", help="Customize webpage with the CSS in path")
     parser.add_argument(
         "-upp",
         "--upload-path",
         help="Path for saving uploaded files",
     )
```

### Comparing `tdwnsv3-1.9.1/tdwnsv3.egg-info/PKG-INFO` & `tdwnsv3-1.9.2/tdwnsv3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdwnsv3
-Version: 1.9.1
+Version: 1.9.2
 Summary: Simple local-files server with security on top!
 Home-page: https://github.com/Simatwa/tdwnsv3
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: MIT
@@ -17,29 +17,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">tdwnsv3</h1>
 
-<div align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
+<p align="center"><a href="https://github.com/Simatwa/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Github&message=Passing&logo=github&color=green" alt="Github"/></a>
 
-<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.1&color=yellow&logo=pypi" alt="pypi"/></a>
+<a href="https://pypi.org/project/tdwnsv3"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.9.2&color=yellow&logo=pypi" alt="pypi"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=lime&logo=Coverage" alt="Coverage"/></a>
 
 <a href="https://wakatime.com/badge/github/Simatwa/svinf3"><img src="https://wakatime.com/badge/github/Simatwa/svinf3.svg" alt="wakatime"/></a>
 
 <a href="https://pepy.tech/project/tdwnsv3"><img src="https://static.pepy.tech/badge/tdwnsv3" alt="Downloads"/></a>
 
 <a href="#"><img src="https://visitor-badge.glitch.me/badge?page_id=Simatwa.tdwnsv3&left_color=red&right_color=lime&left_text=Counts" alt="Visitors"/></a>
 
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 
-</div>
+</p>
 
 
 
 > Access your files on the web.
```

