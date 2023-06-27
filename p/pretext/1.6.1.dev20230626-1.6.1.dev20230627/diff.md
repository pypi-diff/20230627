# Comparing `tmp/pretext-1.6.1.dev20230626.tar.gz` & `tmp/pretext-1.6.1.dev20230627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230626.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230627.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230626.tar` & `pretext-1.6.1.dev20230627.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/README.md
--rw-r--r--   0        0        0     1909 2023-06-26 06:23:45.943116 pretext-1.6.1.dev20230626/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/build.py
--rw-r--r--   0        0        0    25561 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-26 06:23:50.823120 pretext-1.6.1.dev20230626/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/core/resources.py
--rw-r--r--   0        0        0  1041184 2023-06-26 06:23:50.823120 pretext-1.6.1.dev20230626/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/generate.py
--rw-r--r--   0        0        0    31778 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/project.py
--rw-r--r--   0        0        0      739 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-06-26 06:23:50.871120 pretext-1.6.1.dev20230626/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-06-26 06:23:50.871120 pretext-1.6.1.dev20230626/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-06-26 06:23:50.879120 pretext-1.6.1.dev20230626/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-26 06:23:50.891120 pretext-1.6.1.dev20230626/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-06-26 06:23:50.875120 pretext-1.6.1.dev20230626/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    19529 2023-06-26 06:23:06.503070 pretext-1.6.1.dev20230626/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-06-26 06:23:45.943116 pretext-1.6.1.dev20230626/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230626/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/README.md
+-rw-r--r--   0        0        0     1909 2023-06-27 06:16:29.860806 pretext-1.6.1.dev20230627/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/build.py
+-rw-r--r--   0        0        0    25736 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172492 2023-06-27 06:16:35.016815 pretext-1.6.1.dev20230627/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/core/resources.py
+-rw-r--r--   0        0        0  1041222 2023-06-27 06:16:35.016815 pretext-1.6.1.dev20230627/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-06-27 06:15:55.672754 pretext-1.6.1.dev20230627/pretext/generate.py
+-rw-r--r--   0        0        0    29108 2023-06-27 06:15:55.676754 pretext-1.6.1.dev20230627/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-06-27 06:15:55.676754 pretext-1.6.1.dev20230627/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-06-27 06:16:35.068815 pretext-1.6.1.dev20230627/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-06-27 06:16:35.072815 pretext-1.6.1.dev20230627/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-06-27 06:16:35.076815 pretext-1.6.1.dev20230627/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-27 06:16:35.092815 pretext-1.6.1.dev20230627/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-06-27 06:16:35.076815 pretext-1.6.1.dev20230627/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-06-27 06:15:55.676754 pretext-1.6.1.dev20230627/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-06-27 06:16:29.860806 pretext-1.6.1.dev20230627/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230627/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230626/LICENSE` & `pretext-1.6.1.dev20230627/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/README.md` & `pretext-1.6.1.dev20230627/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/__init__.py` & `pretext-1.6.1.dev20230627/pretext/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '5db618b98d63ba4169c1f2f606f6ffcb1b8f8b4a'
+CORE_COMMIT = '3af9f7123aab845bc4dbc4dc6a3607c3b7980030'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230626/pretext/build.py` & `pretext-1.6.1.dev20230627/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/cli.py` & `pretext-1.6.1.dev20230627/pretext/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -669,16 +669,23 @@
 
 # pretext deploy
 @main.command(
     short_help="Deploys Git-managed project to GitHub Pages.",
     context_settings=CONTEXT_SETTINGS,
 )
 @click.argument("target_name", metavar="target", required=False)
+@click.option(
+    "-s",
+    "--site",
+    required=False,
+    default="site",
+    help="Relative path to a directory containing html for a landing page.",
+)
 @click.option("-u", "--update_source", is_flag=True, required=False)
-def deploy(target_name: str, update_source: bool) -> None:
+def deploy(target_name: str, site: str, update_source: bool) -> None:
     """
     Automatically deploys most recent build of [TARGET] to GitHub Pages,
     making it available to the general public.
     Requires that your project is under Git version control
     properly configured with GitHub and GitHub Pages. Deployed
     files will live in `docs` subdirectory of project.
     """
@@ -690,8 +697,8 @@
         log.critical("Target could not be found in project.ptx manifest.")
         # only list targets with html format.
         log.critical(
             f"Possible html targets to deploy are: {project.target_names('html')}"
         )
         log.critical("Exiting without completing task.")
         return
-    project.deploy(target_name, update_source)
+    project.deploy(target_name, site, update_source)
```

### Comparing `pretext-1.6.1.dev20230626/pretext/codechat.py` & `pretext-1.6.1.dev20230627/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230627/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/core/pretext.py` & `pretext-1.6.1.dev20230627/pretext/core/pretext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1112,14 +1112,15 @@
     # This should work for 2.17 and beyond.
     try:
         params_for_version_determination = dict(
             problemSeed=1,
             displayMode='PTX',
             courseID=courseID,
             userID=userID,
+            course_password=course_password,
             outputformat='raw'
         )
         version_determination_json = requests.get(url=ww_domain_path, params=params_for_version_determination).json()
         ww_version = ""
         if "ww_version" in version_determination_json:
             ww_version = version_determination_json["ww_version"]
             ww_version_match = re.search(
@@ -1475,15 +1476,15 @@
             if image_extension == ".tgz":
                 ptx_image = ptx_image_name
             else:
                 ptx_image = ptx_image_name + image_extension
             if ww_image_scheme:
                 image_url = ww_image_url
             else:
-                image_url = ww_domain + "/" + ww_image_full_path
+                image_url = urllib.parse.urljoin(ww_domain, ww_image_full_path)
             # modify PTX problem source to include local versions
             if generated_dir:
                 if "xmlns:pi=" not in response_text:
                     response_text = response_text.replace(
                         "<webwork>",
                         '<webwork xmlns:pi="http://pretextbook.org/2020/pretext/internal">',
                     )
```

### Comparing `pretext-1.6.1.dev20230626/pretext/core/resources.py` & `pretext-1.6.1.dev20230627/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/core/resources.zip` & `pretext-1.6.1.dev20230627/pretext/core/resources.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1041184 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-26 06:23 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-26 06:23 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-26 06:23 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-26 06:23 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 06:23 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-26 06:23 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 06:23 pretext/__init__.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-26 06:23 pretext/pretext
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-26 06:23 pretext/README.md
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-26 06:23 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-26 06:23 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-26 06:23 pretext/module-test.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-26 06:23 pretext/braille_format.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-26 06:23 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   612399 b- defN 23-Jun-26 06:23 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-26 06:23 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-26 06:23 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-26 06:23 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-26 06:23 xsl/README.md
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-26 06:23 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-26 06:23 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-26 06:23 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-26 06:23 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-26 06:23 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx   109017 b- defN 23-Jun-26 06:23 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-26 06:23 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-26 06:23 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-26 06:23 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-26 06:23 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-26 06:23 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-26 06:23 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-26 06:23 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-26 06:23 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-26 06:23 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-26 06:23 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-26 06:23 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-26 06:23 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-26 06:23 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-26 06:23 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-26 06:23 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-26 06:23 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-26 06:23 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-26 06:23 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-26 06:23 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-26 06:23 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-26 06:23 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-26 06:23 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-26 06:23 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-26 06:23 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-26 06:23 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-26 06:23 xsl/entities.ent
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-26 06:23 xsl/pretext-json-manifest.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-26 06:23 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-26 06:23 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-26 06:23 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-26 06:23 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-26 06:23 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-26 06:23 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-26 06:23 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-26 06:23 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-26 06:23 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-26 06:23 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-26 06:23 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-26 06:23 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-26 06:23 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-26 06:23 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-26 06:23 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-26 06:23 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jun-26 06:23 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-26 06:23 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jun-26 06:23 xsl/localizations/README.md
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-26 06:23 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-26 06:23 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-26 06:23 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-26 06:23 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-26 06:23 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    20427 b- defN 23-Jun-26 06:23 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-26 06:23 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-26 06:23 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-26 06:23 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    15850 b- defN 23-Jun-26 06:23 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-26 06:23 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-26 06:23 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-26 06:23 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-26 06:23 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-26 06:23 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-26 06:23 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-26 06:23 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-26 06:23 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-26 06:23 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-26 06:23 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-26 06:23 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-26 06:23 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-26 06:23 schema/README.md
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-26 06:23 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-26 06:23 schema/pretext.rng
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-26 06:23 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-26 06:23 schema/pretext.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-26 06:23 schema/build.sh
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-26 06:23 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-26 06:23 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-26 06:23 schema/pretext.xsd
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-26 06:23 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-26 06:23 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-26 06:23 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-26 06:23 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-26 06:23 css/README.md
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-26 06:23 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-26 06:23 css/style_oscarlevin.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-26 06:23 css/mathbook-content.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-26 06:23 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-26 06:23 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-26 06:23 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_green_blue.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-26 06:23 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-26 06:23 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-26 06:23 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-26 06:23 css/kindle.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-26 06:23 css/style_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-26 06:23 css/pretext_add_on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-26 06:23 css/setcolors.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-26 06:23 css/style_soundwriting.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-26 06:23 css/colors_blue_green.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-26 06:23 css/colors_brown_gold.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-26 06:23 css/mathbook-3.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-26 06:23 css/mathbook-add-on.css
-142 files, 4834916 bytes uncompressed, 1023610 bytes compressed:  78.8%
+Zip file size: 1041222 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-27 06:16 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-27 06:16 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-27 06:16 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-27 06:16 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 06:16 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-27 06:16 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 06:16 pretext/__init__.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-27 06:16 pretext/pretext
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-27 06:16 pretext/README.md
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-27 06:16 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172492 b- defN 23-Jun-27 06:16 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-27 06:16 pretext/module-test.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-27 06:16 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-27 06:16 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   612399 b- defN 23-Jun-27 06:16 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-27 06:16 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jun-27 06:16 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-27 06:16 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-27 06:16 xsl/README.md
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-27 06:16 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-27 06:16 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-27 06:16 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-27 06:16 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-27 06:16 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-27 06:16 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-27 06:16 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-27 06:16 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-27 06:16 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-27 06:16 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-27 06:16 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-27 06:16 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-27 06:16 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-27 06:16 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-27 06:16 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-27 06:16 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-27 06:16 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-27 06:16 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-27 06:16 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-27 06:16 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-27 06:16 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-27 06:16 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-27 06:16 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-27 06:16 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-27 06:16 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-27 06:16 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-27 06:16 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-27 06:16 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-27 06:16 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-27 06:16 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-27 06:16 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-27 06:16 xsl/entities.ent
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-27 06:16 xsl/pretext-json-manifest.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-27 06:16 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-27 06:16 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-27 06:16 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-27 06:16 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-27 06:16 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-27 06:16 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-27 06:16 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-27 06:16 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-27 06:16 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-27 06:16 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-27 06:16 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-27 06:16 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-27 06:16 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-27 06:16 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-27 06:16 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-27 06:16 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jun-27 06:16 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-27 06:16 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jun-27 06:16 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-27 06:16 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-27 06:16 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-27 06:16 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-27 06:16 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-27 06:16 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    20465 b- defN 23-Jun-27 06:16 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-27 06:16 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-27 06:16 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-27 06:16 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    15850 b- defN 23-Jun-27 06:16 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-27 06:16 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-27 06:16 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-27 06:16 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-27 06:16 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-27 06:16 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-27 06:16 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-27 06:16 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-27 06:16 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-27 06:16 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-27 06:16 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-27 06:16 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-27 06:16 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-27 06:16 schema/README.md
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-27 06:16 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-27 06:16 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-27 06:16 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-27 06:16 schema/pretext.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-27 06:16 schema/build.sh
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-27 06:16 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-27 06:16 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-27 06:16 schema/pretext.xsd
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-27 06:16 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-27 06:16 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-27 06:16 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-27 06:16 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-27 06:16 css/README.md
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-27 06:16 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-27 06:16 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-27 06:16 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-27 06:16 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-27 06:16 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-27 06:16 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-27 06:16 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-27 06:16 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-27 06:16 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-27 06:16 css/kindle.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-27 06:16 css/style_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-27 06:16 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-27 06:16 css/setcolors.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-27 06:16 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-27 06:16 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-27 06:16 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-27 06:16 css/mathbook-3.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-27 06:16 css/mathbook-add-on.css
+142 files, 4835031 bytes uncompressed, 1023648 bytes compressed:  78.8%
```

#### pretext/pretext.py

```diff
@@ -1112,14 +1112,15 @@
     # This should work for 2.17 and beyond.
     try:
         params_for_version_determination = dict(
             problemSeed=1,
             displayMode='PTX',
             courseID=courseID,
             userID=userID,
+            course_password=course_password,
             outputformat='raw'
         )
         version_determination_json = requests.get(url=ww_domain_path, params=params_for_version_determination).json()
         ww_version = ""
         if "ww_version" in version_determination_json:
             ww_version = version_determination_json["ww_version"]
             ww_version_match = re.search(
@@ -1475,15 +1476,15 @@
             if image_extension == ".tgz":
                 ptx_image = ptx_image_name
             else:
                 ptx_image = ptx_image_name + image_extension
             if ww_image_scheme:
                 image_url = ww_image_url
             else:
-                image_url = ww_domain + "/" + ww_image_full_path
+                image_url = urllib.parse.urljoin(ww_domain, ww_image_full_path)
             # modify PTX problem source to include local versions
             if generated_dir:
                 if "xmlns:pi=" not in response_text:
                     response_text = response_text.replace(
                         "<webwork>",
                         '<webwork xmlns:pi="http://pretextbook.org/2020/pretext/internal">',
                     )
```

#### xsl/publisher-variables.xsl

##### xsl/publisher-variables.xsl

```diff
@@ -3118,15 +3118,15 @@
     </latex>
     <webwork>
       <pi:pub-attribute name="server" default="https://webwork-ptx.aimath.org" freeform="yes"/>
       <pi:pub-attribute name="course" default="anonymous" freeform="yes"/>
       <pi:pub-attribute name="coursepassword" default="anonymous" freeform="yes"/>
       <pi:pub-attribute name="user" default="anonymous" freeform="yes"/>
       <pi:pub-attribute name="userpassword" default="anonymous" freeform="yes"/>
-      <pi:pub-attribute name="task-reveal" default="" options="all"/>
+      <pi:pub-attribute name="task-reveal" default="all" options="preceding-correct"/>
     </webwork>
     <revealjs>
       <appearance>
         <pi:pub-attribute name="theme" default="simple" freeform="yes"/>
       </appearance>
       <controls>
         <pi:pub-attribute name="backarrows" default="faded" options="hidden visible"/>
```

#### xsl/localizations/ku-CKB.xml

##### xsl/localizations/ku-CKB.xml

```diff
@@ -251,15 +251,15 @@
   <!-- an overlay window with the search results.  "Search Results"      -->
   <!-- is like a heading.  It renders like "Search Results: algorithm".  -->
   <!-- When a reader uses a term that produces no results (perhaps they  -->
   <!-- misspell the search term) then they get a message to that effect. -->
   <!-- Capitalize "Search Results" - used as a heading, no punctuation   -->
   <localization string-id="search-results-heading">ئەنجامی گەڕان</localization>
   <!-- Short phrase, no punctuation -->
-  <localization string-id="no-search-results"/>
+  <localization string-id="no-search-results">ەنجامی-گەڕانەکان-نیە</localization>
   <!-- Parts of memos and letters -->
   <localization string-id="to">بۆ</localization>
   <localization string-id="from">لە</localization>
   <localization string-id="subject">بابەت</localization>
   <localization string-id="date">بەروار</localization>
   <localization string-id="copy">cc</localization>
   <localization string-id="enclosure">پیچانەوە</localization>
```

### Comparing `pretext-1.6.1.dev20230626/pretext/generate.py` & `pretext-1.6.1.dev20230627/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/project.py` & `pretext-1.6.1.dev20230627/pretext/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from . import build as builder
 from . import ASSETS
 from pathlib import Path
 import sys
 from .config.xml_overlay import ShadowXmlDocument
 from typing import Dict, List, Optional, Tuple
 import hashlib
+import subprocess
 
 log = logging.getLogger("ptxlogger")
 
 asset_table_type = Dict[Tuple[str, str], bytes]
 
 
 class Target:
@@ -128,14 +129,20 @@
 
     def output_filename(self) -> Optional[str]:
         if self.xml_element().find("output-filename") is None:
             return None
         else:
             return self.require_tag_text("output-filename").strip()
 
+    def deploy_dir(self) -> Optional[str]:
+        if self.xml_element().find("deploy-dir") is None:
+            return None
+        else:
+            return self.require_tag_text("deploy-dir").strip()
+
     def port(self) -> int:
         view_ele = self.xml_element().find("view")
         if view_ele is not None and (port := view_ele.get("port")) is not None:
             return int(port)
         else:
             return 8000
 
@@ -198,15 +205,15 @@
                     assert isinstance(node, _Element)
                     # First see if the node has an xml:id, or if it is a child of a node with an xml:id (but we haven't already made this key)
                     if (
                         (id := node.xpath("@xml:id") or node.xpath("parent::*/@xml:id"))
                         and isinstance(id, List)
                         and (asset, id[0]) not in asset_hash_dict
                     ):
-                        assert isinstance(id, _Element)
+                        assert isinstance(id[0], str)
                         asset_hash_dict[(asset, id[0])] = hashlib.sha256(
                             ET.tostring(node)
                         ).digest()
                     # otherwise collect all non-id'd nodes into a single hash
                     else:
                         h_no_id.update(ET.tostring(node))
                 asset_hash_dict[(asset, "")] = h_no_id.digest()
@@ -265,16 +272,18 @@
     def targets(self) -> List[Target]:
         t = self.xml_element().xpath("targets/target")
         assert isinstance(
             t, List
         ), "Project file error: expected list of targets in targets/target tags."
         ret: List[Target] = []
         for target_element in t:
-            assert isinstance(t, _Element), "Project file error: target must be a tag."
-            t.append(
+            assert isinstance(
+                target_element, _Element
+            ), "Project file error: target must be a tag."
+            ret.append(
                 Target(xml_element=target_element, project_path=self.__project_path)
             )
         return ret
 
     def target_names(self, *args: str) -> List[str]:
         # Optional arguments are formats: returns list of targets that have that format.
         names = []
@@ -586,156 +595,82 @@
                 target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
         # Delete temporary directories left behind by core:
         core.release_temporary_directories()
 
-    def deploy(self, target_name: str, update_source: bool) -> None:
+    def deploy_targets(self) -> List[Target]:
+        return [target for target in self.targets() if target.deploy_dir() is not None]
+
+    def deploy(self, target_name: str, site: str, update_source: bool) -> None:
+        # Before doing any work, we check that git is installed.
         try:
-            import git
-            import ghp_import
-        except ImportError:
+            subprocess.run(["git", "--version"], capture_output=True)
+            log.debug("Git is installed.")
+        except Exception as e:
             log.error(
                 "Git must be installed to use this feature, but couldn't be found."
             )
-            log.error("Visit https://github.com/git-guides/install-git for assistance.")
+            log.debug(f"Error: {e}")
             return
-        target = self.target(target_name)
-        if target is None:
-            log.error(f"Target `{target_name}` not found.")
-            return
-        if target.format() != "html":  # redundant for CLI
-            log.error("Only HTML format targets are supported.")
-            return
-        try:
-            repo = git.Repo(self.__project_path)
-        except git.exc.InvalidGitRepositoryError:  # type: ignore
-            log.info("Initializing project with Git.")
-            repo = git.Repo.init(self.__project_path)
-            try:
-                repo.config_reader().get_value("user", "name")
-                repo.config_reader().get_value("user", "email")
-            except Exception:
-                log.info("Setting up name/email configuration for Git...")
-                name = input("Type a name to use with Git: ")
-                email = input("Type your GitHub email to use with Git: ")
-                with repo.config_writer() as w:
-                    w.set_value("user", "name", name)
-                    w.set_value("user", "email", email)
-            repo.git.add(all=True)
-            repo.git.commit(message="Initial commit")
-            repo.active_branch.rename("main")
-            log.info("Successfully initialized new Git repository!")
-            log.info("")
-        log.info(
-            f"Preparing to deploy from active `{repo.active_branch.name}` git branch."
-        )
-        log.info("")
-        if repo.bare or repo.is_dirty() or len(repo.untracked_files) > 0:
-            log.info("Changes to project source since last commit detected.")
-            if update_source:
-                log.info("Add/committing these changes to local Git repository.")
-                log.info("")
-                repo.git.add(all=True)
-                repo.git.commit(message="Update to PreTeXt project source.")
-            else:
-                log.error("Either add and commit these changes with Git, or run")
+        # Determine what set of targets to deploy.  If a target name is specified, deploy on that target.  If there are `deploy-dir` specified in the project manifest, also deploy the contents of the `site` folder, if present.
+        if len(self.deploy_targets()) == 0:
+            target = self.target(target_name)
+            if target is None:
+                log.error(f"Target `{target_name}` not found.")
+                return
+            if target.format() != "html":  # redundant for CLI
+                log.error("Only HTML format targets are supported.")
+                return
+            if not target.output_dir().exists():
+                log.error(
+                    f"No build for `{target.name()}` was found in the directory `{target.output_dir()}`."
+                )
                 log.error(
-                    "`pretext deploy -u` to have these changes updated automatically."
+                    f"Try running `pretext view {target.name()} -b` to build and preview your project first."
                 )
                 return
-        if not target.output_dir().exists():
-            log.error(
-                f"No build for `{target.name()}` was found in the directory `{target.output_dir()}`."
-            )
-            log.error(
-                f"Try running `pretext view {target.name()} -b` to build and preview your project first."
-            )
-            return
-        log.info(f"Using latest build located in `{target.output_dir()}`.")
-        log.info("")
-        try:
-            origin = repo.remotes.origin
-        except AttributeError:
-            log.warning("Remote GitHub repository is not yet configured.")
-            log.info("")
-            log.info(
-                "And if you haven't already, create a remote GitHub repository for this project at:"
-            )
-            log.info("    https://github.com/new")
-            log.info('(Do NOT check any "initialize" options.)')
-            log.info(
-                'On the next page, copy the URL in the "Quick Setup" section (use HTTPS unless you have SSH setup already).'
-            )
-            log.info("")
-            repourl = input("Paste url here: ").strip()
-            repo.create_remote("origin", url=repourl)
-            origin = repo.remotes.origin
-            log.info(
-                "\nFor information about authentication options for github, see: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github\n"
-            )
-        log.info("Committing your latest build to the `gh-pages` branch.")
-        log.info("")
-        ghp_import.ghp_import(
-            target.output_dir(),
-            mesg=f"Latest build of target {target.name()}.",
-            nojekyll=True,
-        )
-        log.info(f"Attempting to connect to remote repository at `{origin.url}`...")
-        # log.info("(Your SSH password may be required.)")
-        log.info("")
-        try:
-            repo_user, repo_name = utils.parse_git_remote(origin.url)
-            repo_url = f"https://github.com/{repo_user}/{repo_name}/"
-            # Set pages_url depending on whether project is base pages for the user or a separate repo
-            if "github.io" in repo_name:
-                pages_url = f"https://{repo_name}"
-            else:
-                pages_url = f"https://{repo_user}.github.io/{repo_name}/"
-        except Exception:
-            log.error(f"Unable to parse GitHub URL from {origin.url}")
-            log.error("Deploy unsuccessful")
-            return
-        try:
-            origin.push(refspec=f"{repo.active_branch.name}:{repo.active_branch.name}")
-            origin.push(refspec="gh-pages:gh-pages")
-        except git.exc.GitCommandError:  # type: ignore
-            log.warning(
-                f"There was an issue connecting to GitHub repository located at {repo_url}"
-            )
-            log.info("")
-            log.info(
-                "If you haven't already, configure SSH with GitHub by following instructions at:"
-            )
-            log.info(
-                "    https://docs.github.com/en/authentication/connecting-to-github-with-ssh"
-            )
-            log.info("Then try to deploy again.")
-            log.info("")
-            log.info(f"If `{origin.url}` doesn't match your GitHub repository,")
-            log.info(
-                "use `git remote remove origin` on the command line then try to deploy again."
-            )
+            log.info(f"Using latest build located in `{target.output_dir()}`.")
             log.info("")
-            log.error("Deploy was unsuccessful.")
+            utils.publish_to_ghpages(target.output_dir(), update_source)
             return
-        log.info("")
-        log.info("Latest build successfully pushed to GitHub!")
-        log.info("")
-        log.info("To enable GitHub Pages, visit")
-        log.info(f"    {repo_url}settings/pages")
-        log.info("selecting the `gh-pages` branch with the `/ (root)` folder.")
-        log.info("")
-        log.info("Visit")
-        log.info(f"    {repo_url}actions/")
-        log.info("to check on the status of your GitHub Pages deployment.")
-        log.info("")
-        log.info("Your built project will soon be available to the public at:")
-        log.info(f"    {pages_url}")
+        else:  # we now deploy multiple targets and the site directory
+            site_dir = (self.__project_path / site).resolve()
+            if not site_dir.exists():
+                log.error(f"Site directory `{site_dir}` not found.")
+                log.info(
+                    f"You have `deploy-dir` elements in your project.ptx file, which requires you to maintain at least a simple landing page in the folder `{site_dir}`. Either create this folder or remove the `deploy-dir` elements from your project.ptx file.\n"
+                )
+                return
+            with tempfile.TemporaryDirectory() as temp_dir:
+                shutil.copytree(
+                    (self.__project_path / site).resolve(),
+                    Path(temp_dir),
+                    dirs_exist_ok=True,
+                )
+                for target in self.deploy_targets():
+                    if not target.output_dir().exists():
+                        log.warning(
+                            f"No build for `{target.name()}` was found in the directory `{target.output_dir()}`. Try running `pretext build {target.name()}` to build this component first."
+                        )
+                        log.info("Skipping this target for now.")
+                    else:
+                        deploy_dir = target.deploy_dir()
+                        assert isinstance(deploy_dir, str)
+                        shutil.copytree(
+                            target.output_dir(),
+                            (Path(temp_dir) / deploy_dir).resolve(),
+                            dirs_exist_ok=True,
+                        )
+                        log.info(
+                            f"Deploying `{target.name()}` to `{target.deploy_dir()}`."
+                        )
+                utils.publish_to_ghpages(Path(temp_dir), update_source)
+        return
 
     def xml_source_is_valid(self, target_name: str) -> bool:
         target = self.target(target_name)
         if target is None:
             return False
         return utils.xml_syntax_is_valid(target.source())
```

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230627/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230627/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230627/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-26 06:23 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-26 06:23 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-26 06:23 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-26 06:23 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-26 06:23 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-26 06:23 assets/frog.jpg
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-26 06:23 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-26 06:23 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-26 06:23 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-26 06:23 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-27 06:16 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-27 06:15 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-27 06:16 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-27 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-27 06:16 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-27 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-27 06:15 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-27 06:15 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-27 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-27 06:15 publication/publication.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230627/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-26 06:23 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-26 06:23 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-26 06:23 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-26 06:23 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-26 06:23 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-26 06:23 source/main.ptx
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-26 06:23 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-27 06:16 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-27 06:15 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-27 06:16 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-27 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-27 06:16 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-27 06:15 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-27 06:15 publication/publication.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230627/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-26 06:23 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-26 06:23 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-26 06:23 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-26 06:23 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-26 06:23 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-26 06:23 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-26 06:23 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-26 06:23 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-26 06:23 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-26 06:23 source/ch-empty.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-26 06:23 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-26 06:23 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-26 06:23 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-26 06:23 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-26 06:23 source/sec-features.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-26 06:23 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-26 06:23 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-26 06:23 source/ch-features.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-26 06:23 source/docinfo.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-26 06:23 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-26 06:23 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-26 06:23 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-26 06:23 source/backmatter.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-26 06:23 source/images/cflag.asy
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-26 06:23 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-26 06:23 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-26 06:23 source/images/tikz.tex
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-26 06:23 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-27 06:16 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-27 06:15 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-27 06:16 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-27 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-27 06:16 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-27 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-27 06:15 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-27 06:15 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-27 06:15 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-27 06:15 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-27 06:15 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-27 06:15 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-27 06:15 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-27 06:15 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-27 06:15 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-27 06:15 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-27 06:15 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-27 06:15 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-27 06:15 source/docinfo.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-27 06:15 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-27 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-27 06:15 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-27 06:15 source/backmatter.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-27 06:15 source/images/cflag.asy
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-27 06:15 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-27 06:15 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-27 06:15 source/images/tikz.tex
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-27 06:15 publication/publication.ptx
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230627/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230627/pretext/templates/resources/hello.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-26 06:23 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-26 06:23 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-26 06:23 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-26 06:23 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-26 06:23 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-26 06:23 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-26 06:23 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-27 06:15 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-27 06:15 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-27 06:16 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-27 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-27 06:16 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-27 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-27 06:15 publication/publication.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230627/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230626/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230627/pretext/templates/resources/slideshow.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 06:23 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-26 06:23 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-26 06:23 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-26 06:23 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-26 06:23 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-26 06:23 xsl/slides.xsl
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-26 06:23 source/main.ptx
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-26 06:23 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:16 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 06:15 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-27 06:15 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-27 06:16 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-27 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-27 06:16 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-27 06:15 xsl/slides.xsl
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-27 06:15 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-27 06:15 publication/publication.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230626/pretext/utils.py` & `pretext-1.6.1.dev20230627/pretext/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import shutil
 from pathlib import Path
 import platform
 import re
 import socketserver
 import socket
 import subprocess
-import sys
 import logging
 import logging.handlers
 import threading
 import watchdog.events
 import watchdog.observers
 import time
 import webbrowser
@@ -499,15 +498,15 @@
     Checks to see if anything (errors etc.) is in the memory handler.  If it is, reports that there are errors before the handler gets flushed.  Otherwise, adds a single blank line.
     """
     if len(mh.buffer) > 0:
         print("\n----------------------------------------------------")
         log.info("While running pretext, the following errors occurred:\n")
         mh.flush()
         print("----------------------------------------------------")
-        sys.exit(1)
+        # sys.exit("Exit due to errors.")
     else:
         print("")
 
 
 def format_docstring_as_help_str(string: str) -> str:
     """
     Formats a docstring so that it is suitable to pass in as a help string
@@ -528,7 +527,136 @@
     git@github.com:PreTeXtBook/pretext-cli.git or
     https://github.com/PreTeXtBook/pretext-cli.git or
     https://github.com/PreTeXtBook/pretext-cli
     return a list with the username (PreTeXtBook) and reponame (pretext-cli).
     """
     repo_info = list(filter(None, re.split(r"\/|\:|\.git$", string)))
     return repo_info[-2:]
+
+
+def publish_to_ghpages(directory: Path, update_source: bool) -> None:
+    """
+    Publish the current project to GitHub pages.
+    """
+    # Some git setup. Try to import git and ghp_import to make sure git is installed.  These need to be done here, because if git is not installed, then this will break, and not everyone will need deploy functionality.
+    try:
+        import git
+        import ghp_import
+    except ImportError:
+        log.error("Git must be installed to use this feature, but couldn't be found.")
+        log.error("Visit https://github.com/git-guides/install-git for assistance.")
+        return
+
+    try:
+        repo = git.Repo(project_path())
+    except git.exc.InvalidGitRepositoryError:  # type: ignore
+        log.info("Initializing project with Git.")
+        repo = git.Repo.init(project_path())
+        try:
+            repo.config_reader().get_value("user", "name")
+            repo.config_reader().get_value("user", "email")
+        except Exception:
+            log.info("Setting up name/email configuration for Git...")
+            name = input("Type a name to use with Git: ")
+            email = input("Type your GitHub email to use with Git: ")
+            with repo.config_writer() as w:
+                w.set_value("user", "name", name)
+                w.set_value("user", "email", email)
+        repo.git.add(all=True)
+        repo.git.commit(message="Initial commit")
+        repo.active_branch.rename("main")
+        log.info("Successfully initialized new Git repository!")
+        log.info("")
+    log.info(f"Preparing to deploy from active `{repo.active_branch.name}` git branch.")
+    log.info("")
+    if repo.bare or repo.is_dirty() or len(repo.untracked_files) > 0:
+        log.info("Changes to project source since last commit detected.")
+        if update_source:
+            log.info("Add/committing these changes to local Git repository.")
+            log.info("")
+            repo.git.add(all=True)
+            repo.git.commit(message="Update to PreTeXt project source.")
+        else:
+            log.error("Either add and commit these changes with Git, or run")
+            log.error(
+                "`pretext deploy -u` to have these changes updated automatically."
+            )
+            return
+
+    try:
+        origin = repo.remotes.origin
+    except AttributeError:
+        log.warning("Remote GitHub repository is not yet configured.")
+        log.info("")
+        log.info(
+            "And if you haven't already, create a remote GitHub repository for this project at:"
+        )
+        log.info("    https://github.com/new")
+        log.info('(Do NOT check any "initialize" options.)')
+        log.info(
+            'On the next page, copy the URL in the "Quick Setup" section (use HTTPS unless you have SSH setup already).'
+        )
+        log.info("")
+        repourl = input("Paste url here: ").strip()
+        repo.create_remote("origin", url=repourl)
+        origin = repo.remotes.origin
+        log.info(
+            "\nFor information about authentication options for github, see: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github\n"
+        )
+    log.info("Committing your latest build to the `gh-pages` branch.")
+    log.info("")
+    ghp_import.ghp_import(
+        directory,
+        mesg="Latest build deployed.",
+        nojekyll=False,
+    )
+    log.info(f"Attempting to connect to remote repository at `{origin.url}`...")
+    # log.info("(Your SSH password may be required.)")
+    log.info("")
+    try:
+        repo_user, repo_name = parse_git_remote(origin.url)
+        repo_url = f"https://github.com/{repo_user}/{repo_name}/"
+        # Set pages_url depending on whether project is base pages for the user or a separate repo
+        if "github.io" in repo_name:
+            pages_url = f"https://{repo_name}"
+        else:
+            pages_url = f"https://{repo_user}.github.io/{repo_name}/"
+    except Exception:
+        log.error(f"Unable to parse GitHub URL from {origin.url}")
+        log.error("Deploy unsuccessful")
+        return
+    try:
+        origin.push(refspec=f"{repo.active_branch.name}:{repo.active_branch.name}")
+        origin.push(refspec="gh-pages:gh-pages")
+    except git.exc.GitCommandError:  # type: ignore
+        log.warning(
+            f"There was an issue connecting to GitHub repository located at {repo_url}"
+        )
+        log.info("")
+        log.info(
+            "If you haven't already, configure SSH with GitHub by following instructions at:"
+        )
+        log.info(
+            "    https://docs.github.com/en/authentication/connecting-to-github-with-ssh"
+        )
+        log.info("Then try to deploy again.")
+        log.info("")
+        log.info(f"If `{origin.url}` doesn't match your GitHub repository,")
+        log.info(
+            "use `git remote remove origin` on the command line then try to deploy again."
+        )
+        log.info("")
+        log.error("Deploy was unsuccessful.")
+        return
+    log.info("")
+    log.info("Latest build successfully pushed to GitHub!")
+    log.info("")
+    log.info("To enable GitHub Pages, visit")
+    log.info(f"    {repo_url}settings/pages")
+    log.info("selecting the `gh-pages` branch with the `/ (root)` folder.")
+    log.info("")
+    log.info("Visit")
+    log.info(f"    {repo_url}actions/")
+    log.info("to check on the status of your GitHub Pages deployment.")
+    log.info("")
+    log.info("Your built project will soon be available to the public at:")
+    log.info(f"    {pages_url}")
```

### Comparing `pretext-1.6.1.dev20230626/pyproject.toml` & `pretext-1.6.1.dev20230627/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230626"
+version = "1.6.1.dev20230627"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230626/PKG-INFO` & `pretext-1.6.1.dev20230627/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230626
+Version: 1.6.1.dev20230627
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

