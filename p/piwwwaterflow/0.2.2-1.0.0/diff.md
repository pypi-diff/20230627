# Comparing `tmp/piwwwaterflow-0.2.2.tar.gz` & `tmp/piwwwaterflow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.2.2.tar", last modified: Thu Jun 22 13:31:25 2023, max compression
+gzip compressed data, was "piwwwaterflow-1.0.0.tar", last modified: Tue Jun 27 17:40:59 2023, max compression
```

## Comparing `piwwwaterflow-0.2.2.tar` & `piwwwaterflow-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.398343 piwwwaterflow-0.2.2/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.123536 piwwwaterflow-1.0.0/
+-rw-rw-rw-   0        0        0       33 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-06-27 17:40:59.122536 piwwwaterflow-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2021-12-09 10:59:24.000000 piwwwaterflow-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:58.994540 piwwwaterflow-1.0.0/piwwwaterflow/
+-rw-rw-rw-   0        0        0       87 2023-06-26 12:27:35.000000 piwwwaterflow-1.0.0/piwwwaterflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.048537 piwwwaterflow-1.0.0/piwwwaterflow/__pycache__/
+-rw-rw-rw-   0        0        0      266 2023-06-26 15:46:05.000000 piwwwaterflow-1.0.0/piwwwaterflow/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6756 2023-06-27 17:27:35.000000 piwwwaterflow-1.0.0/piwwwaterflow/__pycache__/webservice.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.050537 piwwwaterflow-1.0.0/piwwwaterflow/static/
+-rw-rw-rw-   0        0        0        0 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.069536 piwwwaterflow-1.0.0/piwwwaterflow/static/css/
+-rw-rw-rw-   0        0        0     1804 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/css/iepngfix.htc
+-rw-rw-rw-   0        0        0     4858 2023-06-27 16:27:54.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/css/view.css
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.113537 piwwwaterflow-1.0.0/piwwwaterflow/static/img/
+-rw-rw-rw-   0        0        0       49 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/blank.gif
+-rw-rw-rw-   0        0        0      431 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/bottom.png
+-rw-rw-rw-   0        0        0    33683 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/icon-256.png
+-rw-rw-rw-   0        0        0     2373 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/icon-32.png
+-rw-rw-rw-   0        0        0    10614 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/piwaterflow.svg
+-rw-rw-rw-   0        0        0      762 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/play.png
+-rw-rw-rw-   0        0        0       46 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/shadow.gif
+-rw-rw-rw-   0        0        0      417 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/img/top.png
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.114536 piwwwaterflow-1.0.0/piwwwaterflow/static/js/
+-rw-rw-rw-   0        0        0    11918 2023-06-27 16:55:00.000000 piwwwaterflow-1.0.0/piwwwaterflow/static/js/code.js
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.119536 piwwwaterflow-1.0.0/piwwwaterflow/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-26 07:30:22.000000 piwwwaterflow-1.0.0/piwwwaterflow/templates/__init__.py
+-rw-rw-rw-   0        0        0     4768 2023-06-27 16:17:36.000000 piwwwaterflow-1.0.0/piwwwaterflow/templates/form.html
+-rw-rw-rw-   0        0        0     6991 2023-06-27 17:28:24.000000 piwwwaterflow-1.0.0/piwwwaterflow/webservice.py
+-rw-rw-rw-   0        0        0      927 2023-06-27 17:17:36.000000 piwwwaterflow-1.0.0/piwwwaterflow/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.028536 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-06-27 17:40:58.000000 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2023-06-27 17:40:58.000000 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:40:58.000000 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-06-27 17:40:58.000000 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-27 17:40:58.000000 piwwwaterflow-1.0.0/piwwwaterflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:40:59.124537 piwwwaterflow-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1461 2023-06-27 17:37:55.000000 piwwwaterflow-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:40:59.120536 piwwwaterflow-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-19 06:41:22.000000 piwwwaterflow-1.0.0/tests/__init__.py
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-1.0.0/piwwwaterflow/static/css/iepngfix.htc`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-<public:component>
-<public:attach event="onpropertychange" onevent="doFix()" />
-
-<script type="text/javascript">
-
-// IE5.5+ PNG Alpha Fix v1.0RC4
-// (c) 2004-2005 Angus Turnbull http://www.twinhelix.com
-
-// This is licensed under the CC-GNU LGPL, version 2.1 or later.
-// For details, see: http://creativecommons.org/licenses/LGPL/2.1/
-
-
-// This must be a path to a blank image. That's all the configuration you need.
-if (typeof blankImg == 'undefined') var blankImg = 'blank.gif';
-
-
-var f = 'DXImageTransform.Microsoft.AlphaImageLoader';
-
-function filt(s, m)
-{
- if (filters[f])
- {
-  filters[f].enabled = s ? true : false;
-  if (s) with (filters[f]) { src = s; sizingMethod = m }
- }
- else if (s) style.filter = 'progid:'+f+'(src="'+s+'",sizingMethod="'+m+'")';
-}
-
-function doFix()
-{
- // Assume IE7 is OK.
- if (!/MSIE (5\.5|6\.)/.test(navigator.userAgent) ||
-  (event && !/(background|src)/.test(event.propertyName))) return;
-
- var bgImg = currentStyle.backgroundImage || style.backgroundImage;
-
- if (tagName == 'IMG')
- {
-  if ((/\.png$/i).test(src))
-  {
-   if (currentStyle.width == 'auto' && currentStyle.height == 'auto')
-    style.width = offsetWidth + 'px';
-   filt(src, 'scale');
-   src = blankImg;
-  }
-  else if (src.indexOf(blankImg) < 0) filt();
- }
- else if (bgImg && bgImg != 'none')
- {
-  if (bgImg.match(/^url[("']+(.*\.png)[)"']+$/i))
-  {
-   var s = RegExp.$1;
-   if (currentStyle.width == 'auto' && currentStyle.height == 'auto')
-    style.width = offsetWidth + 'px';
-   style.backgroundImage = 'none';
-   filt(s, 'crop');
-   // IE link fix.
-   for (var n = 0; n < childNodes.length; n++)
-    if (childNodes[n].style) childNodes[n].style.position = 'relative';
-  }
-  else filt();
- }
-}
-
-doFix();
-
-</script>
+<public:component>
+<public:attach event="onpropertychange" onevent="doFix()" />
+
+<script type="text/javascript">
+
+// IE5.5+ PNG Alpha Fix v1.0RC4
+// (c) 2004-2005 Angus Turnbull http://www.twinhelix.com
+
+// This is licensed under the CC-GNU LGPL, version 2.1 or later.
+// For details, see: http://creativecommons.org/licenses/LGPL/2.1/
+
+
+// This must be a path to a blank image. That's all the configuration you need.
+if (typeof blankImg == 'undefined') var blankImg = 'blank.gif';
+
+
+var f = 'DXImageTransform.Microsoft.AlphaImageLoader';
+
+function filt(s, m)
+{
+ if (filters[f])
+ {
+  filters[f].enabled = s ? true : false;
+  if (s) with (filters[f]) { src = s; sizingMethod = m }
+ }
+ else if (s) style.filter = 'progid:'+f+'(src="'+s+'",sizingMethod="'+m+'")';
+}
+
+function doFix()
+{
+ // Assume IE7 is OK.
+ if (!/MSIE (5\.5|6\.)/.test(navigator.userAgent) ||
+  (event && !/(background|src)/.test(event.propertyName))) return;
+
+ var bgImg = currentStyle.backgroundImage || style.backgroundImage;
+
+ if (tagName == 'IMG')
+ {
+  if ((/\.png$/i).test(src))
+  {
+   if (currentStyle.width == 'auto' && currentStyle.height == 'auto')
+    style.width = offsetWidth + 'px';
+   filt(src, 'scale');
+   src = blankImg;
+  }
+  else if (src.indexOf(blankImg) < 0) filt();
+ }
+ else if (bgImg && bgImg != 'none')
+ {
+  if (bgImg.match(/^url[("']+(.*\.png)[)"']+$/i))
+  {
+   var s = RegExp.$1;
+   if (currentStyle.width == 'auto' && currentStyle.height == 'auto')
+    style.width = offsetWidth + 'px';
+   style.backgroundImage = 'none';
+   filt(s, 'crop');
+   // IE link fix.
+   for (var n = 0; n < childNodes.length; n++)
+    if (childNodes[n].style) childNodes[n].style.position = 'relative';
+  }
+  else filt();
+ }
+}
+
+doFix();
+
+</script>
 </public:component>
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/css/view.css` & `piwwwaterflow-1.0.0/piwwwaterflow/static/css/view.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,282 +1,303 @@
-body
-{
-	background: #ffffff;
-	font-family: "Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
-	font-size: 3em;
-	margin:4px;
-	text-align:center;
-}
-
-@media (orientation: landscape) {
-body
-{
-	width:800px;
-	margin: 0 auto;
-}
-}
-
-@media (orientation: portrait) {
-body
-{
-	width:100%;
-}
-}
-
-#form_container
-{
-	margin:0 auto;
-	text-align:left;
-	width:100%;
-}
-
-textarea#log {
-    color: inherit;
-    background: #222222;
-}
-
-/**** Logo Section  *****/
-
-
-.mainheader
-{
-    background-image: linear-gradient(to bottom right, #343434 , #565656);
-    color: #EFEFEF;
-    text-shadow: 1px 1px 2px black, 0 0 25px black, 0 0 5px black;
-}
-
-div div span{
-    font-size:180%;
-    color: #222222;
-    vertical-align: middle;
-}
-
-div img {
-    display: inline-block;
-    vertical-align: middle;
-    border:none;
-}
-
-.table
-{
-  border: none;
-  font-size:100% !important;
-}
-/**** Form Section ****/
-
-td
-{
-    border:0px;
-    text-align: center;
-}
-
-.td_left
-{
-    border:0px;
-    text-align: left;
-}
-
-.copperround
-{
-    border-width: 2px;
-    border-radius: 10px;
-	border-bottom:3px solid #222222;
-	border-left:3px solid #EFDFDF;
-	border-right:3px solid #111111;
-	border-top:3px solid #DFCFCF;
-    background-image: linear-gradient(to bottom right, #332822 , #8F857F);
-}
-
-fieldset
-{
-    background-image: linear-gradient(to bottom right, #222222, #555555);
-
-    padding-block-start: 0.15em;
-    padding-inline-start: 0.15em;
-    padding-inline-end: 0.15em;
-    padding-block-end: 0.15em;
-    height: 100%;
-    padding: 0px;
-    border-width: 2px;
-    border-radius: 10px;
-    border-top:3px solid #DFDFDF;
-    border-left:3px solid #EFEFEF;
-    border-right:3px solid #111111;
-    border-bottom:3px solid #222222;
-
-}
-
-.spantime
-{
-	float:left;
-	margin:0 1% 0 0;
-	padding:0 0 0px;
-	width:39%;
-	height: 100%;
-}
-
-.spanvalve
-{
-	float:left;
-	margin:0 1% 0 0;
-	padding:0 0 0px;
-	width:24%;
-	height: 100%;
-}
-
-.spanenabled
-{
-	float:left;
-	margin:0 1% 0 0;
-	padding:0 0 0px;
-	width:9%;
-	height: 100%;
-}
-
-.form_description
-{
-	clear:both;
-	display:inline-block;
-	margin:5 0 1em;
-}
-
-.form_description label
-{
-	font-size:50%;
-	line-height:130%;
-	margin:0px 10px 2px;
-	padding: 2px 0px 0px
-}
-
-/**** Buttons ****/
-input.button_text
-{
-    color: inherit;
-    border-radius: 5px;
-	border-bottom:2px solid #222222;
-	border-left:2px solid #DFDFDF;
-	border-right:2px solid #222222;
-	border-top:2px solid #DFDFDF;
-    background-image: linear-gradient(to bottom right, #333333 , #7F7F7F);
-
-	overflow:visible;
-	padding:0 7px;
-	font-size: 30px;
-	height: 50px;
-	width: 250px;
-}
-
-input.button_text:disabled, input.button_text[disabled]
-{
-    color: #555555;
-    text-shadow: 1px 1px 2px black;
-
-    border-radius: 5px;
-	border-bottom:1px solid #555555;
-	border-left:1px solid #7F7F7F;
-	border-right:1px solid #555555;
-	border-top:1px solid #7F7F7F;
-    background-image: linear-gradient(to bottom right, #666666 , #1F1F1F);
-
-	overflow:visible;
-	padding:0 7px;
-	font-size: 30px;
-	height: 50px;
-	width: 250px;
-}
-
-
-.buttons input
-{
-	font-size:120%;
-	margin-right:5px;
-}
-
-/**** Inputs and Labels ****/
-label.description
-{
-	border:none;
-	color:#222;
-	display:block;
-	font-size:95%;
-	font-weight:700;
-	line-height:100%;
-	padding:0 0 1px;
-}
-
-input[type=radio] {
-    transform: scale(1.5);
-}
-
-label.header
-{
-	border:none;
-	font-size: 200%;
-	font-weight:500;
-	line-height:100%;
-	padding:0 0 1px;
-	color: #9f9f9f
-}
-
-label.programheader
-{
-	border:none;
-	display:block;
-	font-size:2.5vw;
-	font-weight:500;
-	line-height:100%;
-	/**padding:0.2em 0 0.2em;**/
-}
-
-
-legend.fieldsetheader
-{
-	border:none;
-	display:block;
-	font-size:2.5vw;
-	font-weight:700;
-	line-height:100%;
-	padding:0 0 1px;
-}
-
-.timeclass
-{
-    color: inherit;
-    text-shadow: 1px 1px 2px black;
-	font-size:4vh;
-	width: 100%;
-	height: 6vh;
-	margin-left:4px;
-    margin-top:2px;
-	padding: 0.2em;
-}
-
-input.number
-{
-    color: inherit;
-    text-shadow: 1px 1px 2px black;
-	font-size:4vh;
-	width: 100%;
-	height: 6vh;
-	margin-top:2px;
-    padding: 10px;
-}
-
-textarea.textarea
-{
-	background:#fff url(../../../static/img/shadow.gif) repeat-x top;
-	border-bottom:2px solid #222222;
-	border-left:2px solid #DFDFDF;
-	border-right:2px solid #222222;
-	border-top:2px solid #DFDFDF;
-	color:#333;
-	font-family:"Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
-	font-size:100%;
-	margin:0;
-	width:99%;
-}
-
-.checkstyle
-{
-    width: 50%;
-	height: 50%;
-}
+body
+{
+	background: #ffffff;
+	font-family: "Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
+	font-size: 3em;
+	margin:4px;
+	text-align:center;
+}
+
+@media (orientation: landscape) {
+body
+{
+	width:800px;
+	margin: 0 auto;
+}
+}
+
+@media (orientation: portrait) {
+body
+{
+	width:100%;
+}
+}
+
+#form_container
+{
+	margin:0 auto;
+	text-align:left;
+	width:100%;
+}
+
+textarea#log {
+    color: inherit;
+    background: #222222;
+}
+
+/**** Logo Section  *****/
+
+
+.mainheader
+{
+    background-image: linear-gradient(to bottom right, #343434 , #565656);
+    color: #EFEFEF;
+    text-shadow: 1px 1px 2px black, 0 0 25px black, 0 0 5px black;
+}
+
+@keyframes pulse {
+	0% {
+		transform: scale(0.90);
+	}
+
+	50% {
+		transform: scale(1);
+	}
+
+	100% {
+		transform: scale(0.90);
+	}
+}
+
+.logo
+{
+    display: inline-block;
+    animation: pulse 1s infinite ease-in-out;
+}
+
+
+/* div div span{
+    font-size:180%;
+    color: #222222;
+    vertical-align: middle;
+} */
+
+div img {
+    display: inline-block;
+    vertical-align: middle;
+    border:none;
+}
+
+.table
+{
+  border: none;
+  font-size:100% !important;
+}
+/**** Form Section ****/
+
+td
+{
+    border:0px;
+    text-align: center;
+}
+
+.td_left
+{
+    border:0px;
+    text-align: left;
+}
+
+.copperround
+{
+    border-width: 2px;
+    border-radius: 10px;
+	border-bottom:3px solid #222222;
+	border-left:3px solid #EFDFDF;
+	border-right:3px solid #111111;
+	border-top:3px solid #DFCFCF;
+    background-image: linear-gradient(to bottom right, #332822 , #8F857F);
+}
+
+fieldset
+{
+    background-image: linear-gradient(to bottom right, #222222, #555555);
+
+    padding-block-start: 0.15em;
+    padding-inline-start: 0.15em;
+    padding-inline-end: 0.15em;
+    padding-block-end: 0.15em;
+    height: 100%;
+    padding: 0px;
+    border-width: 2px;
+    border-radius: 10px;
+    border-top:3px solid #DFDFDF;
+    border-left:3px solid #EFEFEF;
+    border-right:3px solid #111111;
+    border-bottom:3px solid #222222;
+
+}
+
+.spantime
+{
+	float:left;
+	margin:0 1% 0 0;
+	padding:0 0 0px;
+	width:39%;
+	height: 100%;
+}
+
+.spanvalve
+{
+	float:left;
+	margin:0 1% 0 0;
+	padding:0 0 0px;
+	width:24%;
+	height: 100%;
+}
+
+.spanenabled
+{
+	float:left;
+	margin:0 1% 0 0;
+	padding:0 0 0px;
+	width:9%;
+	height: 100%;
+}
+
+.form_description
+{
+	clear:both;
+	display:inline-block;
+	margin:5 0 1em;
+}
+
+.form_description label
+{
+	font-size:50%;
+	line-height:130%;
+	margin:0px 10px 2px;
+	padding: 2px 0px 0px
+}
+
+/**** Buttons ****/
+input.button_text
+{
+    color: inherit;
+    border-radius: 5px;
+	border-bottom:2px solid #222222;
+	border-left:2px solid #DFDFDF;
+	border-right:2px solid #222222;
+	border-top:2px solid #DFDFDF;
+    background-image: linear-gradient(to bottom right, #333333 , #7F7F7F);
+
+	overflow:visible;
+	padding:0 7px;
+	font-size: 30px;
+	height: 50px;
+	width: 250px;
+}
+
+input.button_text:disabled, input.button_text[disabled]
+{
+    color: #555555;
+    text-shadow: 1px 1px 2px black;
+
+    border-radius: 5px;
+	border-bottom:1px solid #555555;
+	border-left:1px solid #7F7F7F;
+	border-right:1px solid #555555;
+	border-top:1px solid #7F7F7F;
+    background-image: linear-gradient(to bottom right, #666666 , #1F1F1F);
+
+	overflow:visible;
+	padding:0 7px;
+	font-size: 30px;
+	height: 50px;
+	width: 250px;
+}
+
+
+.buttons input
+{
+	font-size:120%;
+	margin-right:5px;
+}
+
+/**** Inputs and Labels ****/
+label.description
+{
+	border:none;
+	color:#222;
+	display:block;
+	font-size:95%;
+	font-weight:700;
+	line-height:100%;
+	padding:0 0 1px;
+}
+
+input[type=radio] {
+    transform: scale(1.5);
+}
+
+label.header
+{
+	border:none;
+	font-size: 200%;
+	font-weight:500;
+	line-height:100%;
+	padding:0 0 1px;
+	color: #9f9f9f
+}
+
+label.programheader
+{
+	border:none;
+	display:block;
+	font-size:2.5vw;
+	font-weight:500;
+	line-height:100%;
+	/**padding:0.2em 0 0.2em;**/
+}
+
+
+legend.fieldsetheader
+{
+	border:none;
+	display:block;
+	font-size:2.5vw;
+	font-weight:700;
+	line-height:100%;
+	padding:0 0 1px;
+}
+
+.timeclass
+{
+    color: inherit;
+    text-shadow: 1px 1px 2px black;
+	font-size:4vh;
+	width: 100%;
+	height: 6vh;
+	margin-left:4px;
+    margin-top:2px;
+	padding: 0.2em;
+}
+
+input.number
+{
+    color: inherit;
+    text-shadow: 1px 1px 2px black;
+	font-size:4vh;
+	width: 100%;
+	height: 6vh;
+	margin-top:2px;
+    padding: 10px;
+}
+
+textarea.textarea
+{
+	background:#fff url(../../../static/img/shadow.gif) repeat-x top;
+	border-bottom:2px solid #222222;
+	border-left:2px solid #DFDFDF;
+	border-right:2px solid #222222;
+	border-top:2px solid #DFDFDF;
+	color:#333;
+	font-family:"Lucida Grande", Tahoma, Arial, Verdana, sans-serif;
+	font-size:100%;
+	margin:0;
+	width:99%;
+}
+
+.checkstyle
+{
+    width: 50%;
+	height: 50%;
+}
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-1.0.0/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-1.0.0/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-1.0.0/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files 6% similar despite different names*

```diff
@@ -1,659 +1,664 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0a3c 7376 670a 2020 2078  "no"?>.<svg.   x
-00000040: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
-00000050: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
-00000060: 656e 7473 2f31 2e31 2f22 0a20 2020 786d  ents/1.1/".   xm
-00000070: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-00000080: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00000090: 7267 2f6e 7323 220a 2020 2078 6d6c 6e73  rg/ns#".   xmlns
-000000a0: 3a72 6466 3d22 6874 7470 3a2f 2f77 7777  :rdf="http://www
-000000b0: 2e77 332e 6f72 672f 3139 3939 2f30 322f  .w3.org/1999/02/
-000000c0: 3232 2d72 6466 2d73 796e 7461 782d 6e73  22-rdf-syntax-ns
-000000d0: 2322 0a20 2020 786d 6c6e 733a 7376 673d  #".   xmlns:svg=
-000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000000f0: 7267 2f32 3030 302f 7376 6722 0a20 2020  rg/2000/svg".   
-00000100: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00000110: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
-00000120: 6722 0a20 2020 786d 6c6e 733a 736f 6469  g".   xmlns:sodi
-00000130: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
-00000140: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
-00000150: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
-00000160: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
-00000170: 6e73 3a69 6e6b 7363 6170 653d 2268 7474  ns:inkscape="htt
-00000180: 703a 2f2f 7777 772e 696e 6b73 6361 7065  p://www.inkscape
-00000190: 2e6f 7267 2f6e 616d 6573 7061 6365 732f  .org/namespaces/
-000001a0: 696e 6b73 6361 7065 220a 2020 2077 6964  inkscape".   wid
-000001b0: 7468 3d22 3139 3537 220a 2020 2068 6569  th="1957".   hei
-000001c0: 6768 743d 2232 3530 3022 0a20 2020 7669  ght="2500".   vi
-000001d0: 6577 426f 783d 2230 2030 2032 3536 2033  ewBox="0 0 256 3
-000001e0: 3237 220a 2020 2070 7265 7365 7276 6541  27".   preserveA
-000001f0: 7370 6563 7452 6174 696f 3d22 784d 696e  spectRatio="xMin
-00000200: 594d 696e 206d 6565 7422 0a20 2020 7665  YMin meet".   ve
-00000210: 7273 696f 6e3d 2231 2e31 220a 2020 2069  rsion="1.1".   i
-00000220: 643d 2273 7667 3536 220a 2020 2073 6f64  d="svg56".   sod
-00000230: 6970 6f64 693a 646f 636e 616d 653d 2270  ipodi:docname="p
-00000240: 6977 6174 6572 666c 6f77 2e73 7667 220a  iwaterflow.svg".
-00000250: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
-00000260: 696f 6e3d 2231 2e30 2e32 2d32 2028 6538  ion="1.0.2-2 (e8
-00000270: 3663 3837 3038 3739 2c20 3230 3231 2d30  6c870879, 2021-0
-00000280: 312d 3135 2922 3e0a 2020 3c6d 6574 6164  1-15)">.  <metad
-00000290: 6174 610a 2020 2020 2069 643d 226d 6574  ata.     id="met
-000002a0: 6164 6174 6136 3222 3e0a 2020 2020 3c72  adata62">.    <r
-000002b0: 6466 3a52 4446 3e0a 2020 2020 2020 3c63  df:RDF>.      <c
-000002c0: 633a 576f 726b 0a20 2020 2020 2020 2020  c:Work.         
-000002d0: 7264 663a 6162 6f75 743d 2222 3e0a 2020  rdf:about="">.  
-000002e0: 2020 2020 2020 3c64 633a 666f 726d 6174        <dc:format
-000002f0: 3e69 6d61 6765 2f73 7667 2b78 6d6c 3c2f  >image/svg+xml</
-00000300: 6463 3a66 6f72 6d61 743e 0a20 2020 2020  dc:format>.     
-00000310: 2020 203c 6463 3a74 7970 650a 2020 2020     <dc:type.    
-00000320: 2020 2020 2020 2072 6466 3a72 6573 6f75         rdf:resou
-00000330: 7263 653d 2268 7474 703a 2f2f 7075 726c  rce="http://purl
-00000340: 2e6f 7267 2f64 632f 6463 6d69 7479 7065  .org/dc/dcmitype
-00000350: 2f53 7469 6c6c 496d 6167 6522 202f 3e0a  /StillImage" />.
-00000360: 2020 2020 2020 2020 3c64 633a 7469 746c          <dc:titl
-00000370: 6520 2f3e 0a20 2020 2020 203c 2f63 633a  e />.      </cc:
-00000380: 576f 726b 3e0a 2020 2020 3c2f 7264 663a  Work>.    </rdf:
-00000390: 5244 463e 0a20 203c 2f6d 6574 6164 6174  RDF>.  </metadat
-000003a0: 613e 0a20 203c 6465 6673 0a20 2020 2020  a>.  <defs.     
-000003b0: 6964 3d22 6465 6673 3630 2220 2f3e 0a20  id="defs60" />. 
-000003c0: 203c 736f 6469 706f 6469 3a6e 616d 6564   <sodipodi:named
-000003d0: 7669 6577 0a20 2020 2020 7061 6765 636f  view.     pageco
-000003e0: 6c6f 723d 2223 6666 6666 6666 220a 2020  lor="#ffffff".  
-000003f0: 2020 2062 6f72 6465 7263 6f6c 6f72 3d22     bordercolor="
-00000400: 2336 3636 3636 3622 0a20 2020 2020 626f  #666666".     bo
-00000410: 7264 6572 6f70 6163 6974 793d 2231 220a  rderopacity="1".
-00000420: 2020 2020 206f 626a 6563 7474 6f6c 6572       objecttoler
-00000430: 616e 6365 3d22 3130 220a 2020 2020 2067  ance="10".     g
-00000440: 7269 6474 6f6c 6572 616e 6365 3d22 3130  ridtolerance="10
-00000450: 220a 2020 2020 2067 7569 6465 746f 6c65  ".     guidetole
-00000460: 7261 6e63 653d 2231 3022 0a20 2020 2020  rance="10".     
-00000470: 696e 6b73 6361 7065 3a70 6167 656f 7061  inkscape:pageopa
-00000480: 6369 7479 3d22 3022 0a20 2020 2020 696e  city="0".     in
-00000490: 6b73 6361 7065 3a70 6167 6573 6861 646f  kscape:pageshado
-000004a0: 773d 2232 220a 2020 2020 2069 6e6b 7363  w="2".     inksc
-000004b0: 6170 653a 7769 6e64 6f77 2d77 6964 7468  ape:window-width
-000004c0: 3d22 3139 3230 220a 2020 2020 2069 6e6b  ="1920".     ink
-000004d0: 7363 6170 653a 7769 6e64 6f77 2d68 6569  scape:window-hei
-000004e0: 6768 743d 2231 3031 3722 0a20 2020 2020  ght="1017".     
-000004f0: 6964 3d22 6e61 6d65 6476 6965 7735 3822  id="namedview58"
-00000500: 0a20 2020 2020 7368 6f77 6772 6964 3d22  .     showgrid="
-00000510: 6661 6c73 6522 0a20 2020 2020 696e 6b73  false".     inks
-00000520: 6361 7065 3a73 6e61 702d 6262 6f78 3d22  cape:snap-bbox="
-00000530: 6661 6c73 6522 0a20 2020 2020 696e 6b73  false".     inks
-00000540: 6361 7065 3a7a 6f6f 6d3d 2230 2e31 3133  cape:zoom="0.113
-00000550: 3133 3730 3822 0a20 2020 2020 696e 6b73  13708".     inks
-00000560: 6361 7065 3a63 783d 222d 3138 3637 2e32  cape:cx="-1867.2
-00000570: 3737 3722 0a20 2020 2020 696e 6b73 6361  777".     inksca
-00000580: 7065 3a63 793d 2231 3035 352e 3336 3039  pe:cy="1055.3609
-00000590: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000005a0: 7769 6e64 6f77 2d78 3d22 2d38 220a 2020  window-x="-8".  
-000005b0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-000005c0: 6f77 2d79 3d22 2d38 220a 2020 2020 2069  ow-y="-8".     i
-000005d0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d6d  nkscape:window-m
-000005e0: 6178 696d 697a 6564 3d22 3122 0a20 2020  aximized="1".   
-000005f0: 2020 696e 6b73 6361 7065 3a63 7572 7265    inkscape:curre
-00000600: 6e74 2d6c 6179 6572 3d22 7376 6735 3622  nt-layer="svg56"
-00000610: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000620: 6f63 756d 656e 742d 726f 7461 7469 6f6e  ocument-rotation
-00000630: 3d22 3022 202f 3e0a 2020 3c70 6174 680a  ="0" />.  <path.
-00000640: 2020 2020 2064 3d22 6d20 3738 2e32 3033       d="m 78.203
-00000650: 3931 382c 3236 2e31 3231 3534 3420 6320  918,26.121544 c 
-00000660: 2d31 2e34 3231 3930 322c 302e 3034 3338  -1.421902,0.0438
-00000670: 3720 2d32 2e39 3533 3034 382c 302e 3536  7 -2.953048,0.56
-00000680: 3934 3439 202d 342e 3639 3036 3432 2c31  9449 -4.690642,1
-00000690: 2e39 3339 3734 202d 342e 3235 3336 3633  .93974 -4.253663
-000006a0: 2c2d 312e 3634 3033 3932 202d 382e 3338  ,-1.640392 -8.38
-000006b0: 3038 3737 2c2d 322e 3231 3037 3031 202d  0877,-2.210701 -
-000006c0: 3132 2e30 3730 3235 322c 312e 3132 3934  12.070252,1.1294
-000006d0: 3335 202d 352e 3639 3730 372c 2d30 2e37  35 -5.69707,-0.7
-000006e0: 3338 3930 3720 2d37 2e35 3438 3230 392c  38907 -7.548209,
-000006f0: 302e 3738 3632 3138 202d 382e 3935 3131  0.786218 -8.9511
-00000700: 3837 2c32 2e35 3636 3832 3120 2d31 2e32  87,2.566821 -1.2
-00000710: 3530 3732 332c 2d30 2e30 3235 3820 2d39  50723,-0.0258 -9
-00000720: 2e33 3538 3035 382c 2d31 2e32 3835 3939  .358058,-1.28599
-00000730: 3120 2d31 332e 3037 3636 382c 342e 3236  1 -13.07668,4.26
-00000740: 3035 3435 202d 392e 3334 3334 3335 2c2d  0545 -9.343435,-
-00000750: 312e 3130 3533 3520 2d31 322e 3239 3634  1.10535 -12.2964
-00000760: 3834 2c35 2e34 3935 3738 3420 2d38 2e39  84,5.495784 -8.9
-00000770: 3530 3332 362c 3131 2e36 3532 3139 3820  50326,11.652198 
-00000780: 2d31 2e39 3038 3737 322c 322e 3935 3339  -1.908772,2.9539
-00000790: 3039 202d 332e 3838 3633 362c 352e 3837  09 -3.88636,5.87
-000007a0: 3235 3439 2030 2e35 3736 3333 2c31 312e  2549 0.57633,11.
-000007b0: 3530 3531 3035 202d 312e 3537 3834 3537  505105 -1.578457
-000007c0: 2c33 2e31 3336 3237 202d 302e 3539 3935  ,3.13627 -0.5995
-000007d0: 3536 2c36 2e35 3339 3220 332e 3131 3930  56,6.5392 3.1190
-000007e0: 3636 2c31 302e 3635 3639 3532 202d 302e  66,10.656952 -0.
-000007f0: 3938 3036 3232 2c34 2e34 3130 3231 3920  980622,4.410219 
-00000800: 302e 3934 3739 3335 2c37 2e35 3230 3638  0.947935,7.52068
-00000810: 3320 342e 3430 3834 3938 2c39 2e39 3435  3 4.408498,9.945
-00000820: 3537 3220 2d30 2e36 3437 3732 362c 362e  572 -0.647726,6.
-00000830: 3033 3432 3635 2035 2e35 3333 3633 332c  034265 5.533633,
-00000840: 392e 3534 3330 3035 2037 2e33 3738 3735  9.543005 7.37875
-00000850: 312c 3130 2e37 3932 3836 3520 302e 3730  1,10.792865 0.70
-00000860: 3838 2c33 2e35 3135 3630 3920 322e 3138  88,3.515609 2.18
-00000870: 3537 3535 2c36 2e38 3334 3234 3920 392e  5755,6.834249 9.
-00000880: 3234 3533 3733 2c38 2e36 3638 3137 3920  245373,8.668179 
-00000890: 312e 3136 3437 3034 2c35 2e32 3430 3331  1.164704,5.24031
-000008a0: 3420 352e 3430 3731 3834 2c36 2e31 3435  4 5.407184,6.145
-000008b0: 3233 3420 392e 3531 3633 3334 2c37 2e32  234 9.516334,7.2
-000008c0: 3434 3536 3420 2d31 332e 3537 3938 3934  44564 -13.579894
-000008d0: 2c37 2e38 3934 3031 202d 3235 2e32 3235  ,7.89401 -25.225
-000008e0: 3231 312c 3138 2e32 3739 3134 202d 3235  211,18.27914 -25
-000008f0: 2e31 3436 3037 332c 3433 2e37 3632 3431  .146073,43.76241
-00000900: 206c 202d 312e 3938 3936 332c 332e 3534   l -1.98963,3.54
-00000910: 3833 2063 202d 3135 2e35 3731 3234 352c  83 c -15.571245,
-00000920: 392e 3436 3930 3320 2d32 392e 3538 3033  9.46903 -29.5803
-00000930: 3736 392c 3339 2e39 3034 3434 202d 372e  769,39.90444 -7.
-00000940: 3637 3239 3337 2c36 342e 3634 3139 3220  672937,64.64192 
-00000950: 312e 3433 3035 3034 2c37 2e37 3433 3437  1.430504,7.74347
-00000960: 2033 2e38 3330 3434 372c 3133 2e33 3035   3.830447,13.305
-00000970: 3439 2035 2e39 3637 3137 312c 3139 2e34  49 5.967171,19.4
-00000980: 3631 3034 2033 2e31 3935 3632 332c 3234  6104 3.195623,24
-00000990: 2e38 3034 3538 2032 342e 3035 3237 3635  .80458 24.052765
-000009a0: 2c33 362e 3431 3937 3920 3239 2e35 3534  ,36.41979 29.554
-000009b0: 3537 312c 3337 2e37 3933 3532 2038 2e30  571,37.79352 8.0
-000009c0: 3630 3838 352c 362e 3134 3030 3720 3136  60885,6.14007 16
-000009d0: 2e36 3436 3438 382c 3131 2e39 3636 3137  .646488,11.96617
-000009e0: 2032 382e 3236 3539 3939 2c31 362e 3034   28.265999,16.04
-000009f0: 3737 3920 3130 2e39 3531 3133 362c 3131  779 10.951136,11
-00000a00: 2e32 3935 3232 2032 322e 3831 3636 3636  .29522 22.816666
-00000a10: 2c31 352e 3630 3034 3920 3334 2e37 3436  ,15.60049 34.746
-00000a20: 3731 362c 3135 2e35 3933 3631 2030 2e31  716,15.59361 0.1
-00000a30: 3735 3438 2c30 2032 342e 3332 3337 332c  7548,0 24.32373,
-00000a40: 2d34 2e32 3937 3533 2033 352e 3237 3635  -4.29753 35.2765
-00000a50: 392c 2d31 352e 3539 3336 3120 3131 2e36  9,-15.59361 11.6
-00000a60: 3137 3739 2c2d 342e 3038 3136 3220 3230  1779,-4.08162 20
-00000a70: 2e32 3033 3339 2c2d 392e 3930 3737 3220  .20339,-9.90772 
-00000a80: 3238 2e32 3635 3939 2c2d 3136 2e30 3437  28.26599,-16.047
-00000a90: 3739 2035 2e35 3030 3039 2c2d 312e 3337  79 5.50009,-1.37
-00000aa0: 3337 3320 3236 2e33 3537 3233 2c2d 3132  373 26.35723,-12
-00000ab0: 2e39 3838 3934 2032 392e 3535 3238 362c  .98894 29.55286,
-00000ac0: 2d33 372e 3739 3335 3220 322e 3133 3637  -37.79352 2.1367
-00000ad0: 322c 2d36 2e31 3535 3535 2034 2e35 3336  2,-6.15555 4.536
-00000ae0: 3636 2c2d 3131 2e37 3137 3537 2035 2e39  66,-11.71757 5.9
-00000af0: 3638 3033 2c2d 3139 2e34 3631 3034 2032  6803,-19.46104 2
-00000b00: 312e 3930 3537 322c 2d32 342e 3734 3030  1.90572,-24.7400
-00000b10: 3620 372e 3839 3734 342c 2d35 352e 3137  6 7.89744,-55.17
-00000b20: 3633 3420 2d37 2e36 3732 3934 2c2d 3634  634 -7.67294,-64
-00000b30: 2e36 3435 3336 206c 202d 312e 3939 3330  .64536 l -1.9930
-00000b40: 372c 2d33 2e35 3438 3320 6320 302e 3037  7,-3.5483 c 0.07
-00000b50: 3931 2c2d 3235 2e34 3830 3639 202d 3131  91,-25.48069 -11
-00000b60: 2e35 3636 3138 2c2d 3335 2e38 3636 3638  .56618,-35.86668
-00000b70: 202d 3235 2e31 3436 3037 2c2d 3433 2e37   -25.14607,-43.7
-00000b80: 3632 3431 2034 2e31 3038 3239 2c2d 312e  6241 4.10829,-1.
-00000b90: 3039 3933 3320 382e 3335 3234 392c 2d32  09933 8.35249,-2
-00000ba0: 2e30 3034 3235 2039 2e35 3135 3437 2c2d  .00425 9.51547,-
-00000bb0: 372e 3234 3435 3634 2037 2e30 3539 3632  7.244564 7.05962
-00000bc0: 2c2d 312e 3833 3438 2038 2e35 3337 3433  ,-1.8348 8.53743
-00000bd0: 2c2d 352e 3135 3235 3720 392e 3234 3533  ,-5.15257 9.2453
-00000be0: 372c 2d38 2e36 3638 3137 3920 312e 3834  7,-8.668179 1.84
-00000bf0: 3539 382c 2d31 2e32 3439 3837 2038 2e30  598,-1.24987 8.0
-00000c00: 3236 3438 2c2d 342e 3735 3836 2037 2e33  2648,-4.7586 7.3
-00000c10: 3830 3437 2c2d 3130 2e37 3932 3836 3620  8047,-10.792866 
-00000c20: 332e 3435 3838 352c 2d32 2e34 3234 3838  3.45885,-2.42488
-00000c30: 3920 352e 3338 3832 362c 2d35 2e35 3336  9 5.38826,-5.536
-00000c40: 3231 3320 342e 3430 3637 382c 2d39 2e39  213 4.40678,-9.9
-00000c50: 3435 3537 3220 332e 3731 3934 382c 2d34  45572 3.71948,-4
-00000c60: 2e31 3137 3735 3220 342e 3639 3735 322c  .117752 4.69752,
-00000c70: 2d37 2e35 3230 3638 3220 332e 3131 3930  -7.520682 3.1190
-00000c80: 372c 2d31 302e 3635 3738 3132 2034 2e34  7,-10.657812 4.4
-00000c90: 3634 3431 2c2d 352e 3632 3931 3135 2032  6441,-5.629115 2
-00000ca0: 2e34 3833 3338 2c2d 382e 3534 3737 3536  .48338,-8.547756
-00000cb0: 2030 2e35 3737 3139 2c2d 3131 2e35 3031   0.57719,-11.501
-00000cc0: 3636 3420 332e 3334 3434 342c 2d36 2e31  664 3.34444,-6.1
-00000cd0: 3536 3431 3420 302e 3339 3331 312c 2d31  56414 0.39311,-1
-00000ce0: 322e 3735 3834 3039 202d 382e 3935 3337  2.758409 -8.9537
-00000cf0: 372c 2d31 312e 3635 3231 3938 202d 332e  7,-11.652198 -3.
-00000d00: 3731 3630 342c 2d35 2e35 3436 3533 3620  71604,-5.546536 
-00000d10: 2d31 312e 3832 3235 322c 2d34 2e32 3837  -11.82252,-4.287
-00000d20: 3231 3120 2d31 332e 3037 3636 382c 2d34  211 -13.07668,-4
-00000d30: 2e32 3631 3430 3520 2d31 2e34 3032 3132  .261405 -1.40212
-00000d40: 2c2d 312e 3737 3937 3433 202d 332e 3235  ,-1.779743 -3.25
-00000d50: 3332 362c 2d33 2e33 3034 3836 3820 2d38  326,-3.304868 -8
-00000d60: 2e39 3530 3333 2c2d 322e 3536 3539 3631  .95033,-2.565961
-00000d70: 202d 332e 3638 3933 372c 2d33 2e33 3430   -3.68937,-3.340
-00000d80: 3133 3620 2d37 2e38 3134 3837 2c2d 322e  136 -7.81487,-2.
-00000d90: 3737 3036 3837 202d 3132 2e30 3730 3235  770687 -12.07025
-00000da0: 2c2d 312e 3132 3934 3336 202d 352e 3035  ,-1.129436 -5.05
-00000db0: 3237 382c 2d33 2e39 3837 3030 3220 2d38  278,-3.987002 -8
-00000dc0: 2e33 3935 352c 2d30 2e37 3931 3337 3920  .3955,-0.791379 
-00000dd0: 2d31 322e 3231 3437 362c 302e 3431 3731  -12.21476,0.4171
-00000de0: 3935 202d 362e 3131 3737 312c 2d31 2e39  95 -6.11771,-1.9
-00000df0: 3939 3039 3320 2d37 2e35 3137 3235 2c30  99093 -7.51725,0
-00000e00: 2e37 3338 3930 3720 2d31 302e 3532 3237  .738907 -10.5227
-00000e10: 372c 312e 3835 3435 3820 2d36 2e36 3731  7,1.85458 -6.671
-00000e20: 3637 2c2d 312e 3430 3938 3539 202d 382e  67,-1.409859 -8.
-00000e30: 3639 3931 352c 312e 3635 3933 3135 202d  69915,1.659315 -
-00000e40: 3131 2e38 3936 3439 2c34 2e38 3938 3830  11.89649,4.89880
-00000e50: 3920 6c20 2d33 2e37 3231 322c 2d30 2e30  9 l -3.7212,-0.0
-00000e60: 3733 3938 2063 202d 3130 2e30 3632 3536  7398 c -10.06256
-00000e70: 2c35 2e39 3330 3138 3320 2d31 352e 3036  ,5.930183 -15.06
-00000e80: 3230 312c 3138 2e30 3035 3539 3620 2d31  201,18.005596 -1
-00000e90: 362e 3833 3430 312c 3234 2e32 3133 3632  6.83401,24.21362
-00000ea0: 3220 2d31 2e37 3732 2c2d 362e 3230 3838  2 -1.772,-6.2088
-00000eb0: 3836 202d 362e 3736 3032 372c 2d31 382e  86 -6.76027,-18.
-00000ec0: 3238 3433 202d 3136 2e38 3231 3132 2c2d  2843 -16.82112,-
-00000ed0: 3234 2e32 3133 3632 3220 6c20 2d33 2e37  24.213622 l -3.7
-00000ee0: 3230 3334 2c30 2e30 3733 3938 2063 202d  2034,0.07398 c -
-00000ef0: 332e 3230 3235 312c 2d33 2e32 3339 3439  3.20251,-3.23949
-00000f00: 3420 2d35 2e32 3239 3133 2c2d 362e 3330  4 -5.22913,-6.30
-00000f10: 3836 3638 202d 3131 2e39 3030 3739 372c  8668 -11.900797,
-00000f20: 2d34 2e38 3938 3830 3920 2d33 2e30 3036  -4.898809 -3.006
-00000f30: 3338 2c2d 312e 3131 3536 3733 202d 342e  38,-1.115673 -4.
-00000f40: 3339 3938 3936 2c2d 332e 3835 3336 3733  399896,-3.853673
-00000f50: 202d 3130 2e35 3232 3736 322c 2d31 2e38   -10.522762,-1.8
-00000f60: 3534 3538 202d 322e 3530 3636 3037 2c2d  5458 -2.506607,-
-00000f70: 302e 3739 3331 202d 342e 3831 3139 3239  0.7931 -4.811929
-00000f80: 2c2d 322e 3434 3132 3333 202d 372e 3532  ,-2.441233 -7.52
-00000f90: 3538 3434 2c2d 322e 3335 3639 3334 204c  5844,-2.356934 L
-00000fa0: 2039 2e31 3332 3030 3131 2c31 3437 2e34   9.1320011,147.4
-00000fb0: 3034 3731 220a 2020 2020 2069 643d 2270  0471".     id="p
-00000fc0: 6174 6835 3022 0a20 2020 2020 7374 796c  ath50".     styl
-00000fd0: 653d 2273 7472 6f6b 652d 7769 6474 683a  e="stroke-width:
-00000fe0: 302e 3836 3031 3935 2220 2f3e 0a20 203c  0.860195" />.  <
-00000ff0: 7061 7468 0a20 2020 2020 643d 224d 2035  path.     d="M 5
-00001000: 382e 3136 3939 3833 2c35 322e 3231 3033  8.169983,52.2103
-00001010: 3931 2043 2038 342e 3836 3639 3837 2c36  91 C 84.866987,6
-00001020: 352e 3937 3433 3637 2031 3030 2e33 3837  5.974367 100.387
-00001030: 3438 2c37 372e 3130 3837 3238 2031 3038  48,77.108728 108
-00001040: 2e38 3930 3531 2c38 362e 3539 3135 3137  .89051,86.591517
-00001050: 2031 3034 2e35 3336 322c 3130 342e 3034   104.5362,104.04
-00001060: 3430 3120 3831 2e38 3230 3137 372c 3130  401 81.820177,10
-00001070: 342e 3834 3035 3520 3733 2e35 3134 3133  4.84055 73.51413
-00001080: 372c 3130 342e 3335 3131 2063 2031 2e37  7,104.3511 c 1.7
-00001090: 3030 3630 352c 2d30 2e37 3931 3338 2033  00605,-0.79138 3
-000010a0: 2e31 3139 3932 362c 2d31 2e37 3430 3138  .119926,-1.74018
-000010b0: 2033 2e36 3233 3134 2c2d 332e 3139 3634   3.62314,-3.1964
-000010c0: 3920 2d32 2e30 3834 3235 322c 2d31 2e34  9 -2.084252,-1.4
-000010d0: 3831 3235 3420 2d39 2e34 3734 3138 352c  81254 -9.474185,
-000010e0: 2d30 2e31 3536 3535 202d 3134 2e36 3333  -0.15655 -14.633
-000010f0: 3633 332c 2d33 2e30 3534 3535 3420 312e  633,-3.054554 1.
-00001100: 3938 3138 3839 2c2d 302e 3431 3131 3720  981889,-0.41117 
-00001110: 322e 3930 3931 3739 2c2d 302e 3831 3131  2.909179,-0.8111
-00001120: 3620 332e 3833 3536 3038 2c2d 322e 3237  6 3.835608,-2.27
-00001130: 3334 3920 2d34 2e38 3733 3836 332c 2d31  349 -4.873863,-1
-00001140: 2e35 3534 3337 202d 3130 2e31 3234 3439  .55437 -10.12449
-00001150: 322c 2d32 2e38 3934 3536 202d 3133 2e32  2,-2.89456 -13.2
-00001160: 3132 3539 312c 2d35 2e34 3639 3937 3920  12591,-5.469979 
-00001170: 312e 3636 3631 3937 2c30 2e30 3230 3620  1.666197,0.0206 
-00001180: 332e 3232 3232 392c 302e 3337 3333 3220  3.22229,0.37332 
-00001190: 352e 3339 3835 3832 2c2d 312e 3133 3633  5.398582,-1.1363
-000011a0: 3220 2d34 2e33 3635 3438 382c 2d32 2e33  2 -4.365488,-2.3
-000011b0: 3532 3633 202d 392e 3032 3433 3033 2c2d  5263 -9.024303,-
-000011c0: 342e 3231 3735 3320 2d31 322e 3634 3430  4.21753 -12.6440
-000011d0: 3032 2c2d 372e 3831 3430 3120 322e 3235  02,-7.81401 2.25
-000011e0: 3731 3531 2c2d 302e 3035 3531 2034 2e36  7151,-0.0551 4.6
-000011f0: 3930 3634 322c 2d30 2e30 3232 3420 352e  90642,-0.0224 5.
-00001200: 3339 3835 3832 2c2d 302e 3835 3234 3520  398582,-0.85245 
-00001210: 2d33 2e39 3935 3630 352c 2d32 2e34 3735  -3.995605,-2.475
-00001220: 3634 202d 372e 3336 3735 3638 2c2d 352e  64 -7.367568,-5.
-00001230: 3232 3832 3633 202d 3130 2e31 3538 3034  228263 -10.15804
-00001240: 2c2d 382e 3233 3938 3035 2033 2e31 3538  ,-8.239805 3.158
-00001250: 3633 352c 302e 3338 3130 3636 2034 2e34  635,0.381066 4.4
-00001260: 3932 3739 372c 302e 3035 3333 3320 352e  92797,0.05333 5.
-00001270: 3235 3636 352c 2d30 2e34 3937 3139 3320  25665,-0.497193 
-00001280: 2d33 2e30 3231 3030 342c 2d33 2e30 3934  -3.021004,-3.094
-00001290: 3132 202d 362e 3834 3337 3039 2c2d 352e  12 -6.843709,-5.
-000012a0: 3730 3635 3331 202d 382e 3636 3634 3632  706531 -8.666462
-000012b0: 2c2d 392e 3531 3839 3135 2032 2e33 3434  ,-9.518915 2.344
-000012c0: 3839 312c 302e 3830 3835 3834 2034 2e34  891,0.808584 4.4
-000012d0: 3931 3037 372c 312e 3131 3832 3534 2036  91077,1.118254 6
-000012e0: 2e30 3337 3730 372c 2d30 2e30 3730 3533  .037707,-0.07053
-000012f0: 202d 312e 3032 3632 3132 2c2d 322e 3331   -1.026212,-2.31
-00001300: 3536 3435 202d 352e 3432 3335 3238 2c2d  5645 -5.423528,-
-00001310: 332e 3638 3136 3334 202d 372e 3935 3539  3.681634 -7.9559
-00001320: 3431 2c2d 392e 3039 3331 3139 2032 2e34  41,-9.093119 2.4
-00001330: 3639 3631 392c 302e 3233 3939 3934 2035  69619,0.239994 5
-00001340: 2e30 3838 3035 322c 302e 3533 3834 3832  .088052,0.538482
-00001350: 2035 2e36 3131 3931 312c 3020 2d31 2e31   5.611911,0 -1.1
-00001360: 3435 3738 2c2d 342e 3636 3931 3337 202d  4578,-4.669137 -
-00001370: 332e 3131 3231 3835 2c2d 372e 3239 3434  3.112185,-7.2944
-00001380: 3532 202d 352e 3034 3037 3432 2c2d 3130  52 -5.040742,-10
-00001390: 2e30 3134 3338 3720 352e 3238 3431 3737  .014387 5.284177
-000013a0: 2c2d 302e 3037 3832 3820 3133 2e32 3930  ,-0.07828 13.290
-000013b0: 3836 392c 302e 3032 3036 3420 3132 2e39  869,0.02064 12.9
-000013c0: 3238 3732 372c 2d30 2e34 3235 3739 3720  28727,-0.425797 
-000013d0: 6c20 2d33 2e32 3637 3838 2c2d 332e 3333  l -3.26788,-3.33
-000013e0: 3834 3135 2063 2035 2e31 3632 3032 392c  8415 c 5.162029,
-000013f0: 2d31 2e33 3930 3037 3520 3130 2e34 3433  -1.390075 10.443
-00001400: 3632 352c 302e 3232 3237 3920 3134 2e32  625,0.22279 14.2
-00001410: 3738 3337 332c 312e 3432 3031 3831 2031  78373,1.420181 1
-00001420: 2e37 3231 3235 2c2d 312e 3335 3832 3437  .72125,-1.358247
-00001430: 202d 302e 3033 3039 372c 2d33 2e30 3736   -0.03097,-3.076
-00001440: 3035 3620 2d32 2e31 3331 3536 332c 2d34  056 -2.131563,-4
-00001450: 2e38 3239 3939 3320 342e 3338 3639 3934  .829993 4.386994
-00001460: 2c30 2e35 3835 3739 3220 382e 3335 3037  ,0.585792 8.3507
-00001470: 3731 2c31 2e35 3933 3934 2031 312e 3933  71,1.59394 11.93
-00001480: 3433 3432 2c32 2e39 3833 3135 3520 312e  4342,2.983155 1.
-00001490: 3931 3339 3334 2c2d 312e 3732 3831 3331  913934,-1.728131
-000014a0: 202d 312e 3234 3239 3831 2c2d 332e 3435   -1.242981,-3.45
-000014b0: 3731 3233 202d 322e 3737 3036 3837 2c2d  7123 -2.770687,-
-000014c0: 352e 3138 3532 3534 2036 2e37 3737 3437  5.185254 6.77747
-000014d0: 342c 312e 3238 3531 3331 2039 2e36 3438  4,1.285131 9.648
-000014e0: 3830 342c 332e 3039 3234 2031 322e 3530  804,3.0924 12.50
-000014f0: 3230 372c 342e 3930 3133 3920 322e 3037  207,4.90139 2.07
-00001500: 3034 3839 2c2d 312e 3938 3434 3720 302e  0489,-1.98447 0.
-00001510: 3131 3837 3037 2c2d 332e 3637 3133 3131  118707,-3.671311
-00001520: 202d 312e 3237 3832 3439 2c2d 352e 3339   -1.278249,-5.39
-00001530: 3835 3833 2035 2e31 3130 3431 372c 312e  8583 5.110417,1.
-00001540: 3839 3234 3239 2037 2e37 3432 3631 332c  892429 7.742613,
-00001550: 342e 3333 3632 3432 2031 302e 3531 3333  4.336242 10.5133
-00001560: 2c36 2e37 3438 3232 3820 302e 3933 3933  ,6.748228 0.9393
-00001570: 3333 2c2d 312e 3236 3739 3237 2032 2e33  33,-1.267927 2.3
-00001580: 3837 3034 312c 2d32 2e31 3937 3739 3720  87041,-2.197797 
-00001590: 302e 3633 3931 3235 2c2d 352e 3235 3636  0.639125,-5.2566
-000015a0: 3520 332e 3632 3833 3031 2c32 2e30 3931  5 3.628301,2.091
-000015b0: 3133 3420 362e 3336 3131 342c 342e 3535  134 6.36114,4.55
-000015c0: 3535 3932 2038 2e33 3832 3539 382c 372e  5592 8.382598,7.
-000015d0: 3331 3638 3137 2032 2e32 3435 3130 382c  316817 2.245108,
-000015e0: 2d31 2e34 3239 3634 3420 312e 3333 3736  -1.429644 1.3376
-000015f0: 3032 2c2d 332e 3338 3430 3036 2031 2e33  02,-3.384006 1.3
-00001600: 3439 3634 352c 2d35 2e31 3836 3131 3420  49645,-5.186114 
-00001610: 332e 3737 3130 3933 2c33 2e30 3637 3435  3.771093,3.06745
-00001620: 3420 362e 3136 3431 3533 2c36 2e33 3331  4 6.164153,6.331
-00001630: 3839 3320 392e 3039 3331 3233 2c39 2e35  893 9.093123,9.5
-00001640: 3138 3931 3520 302e 3539 3030 392c 2d30  18915 0.59009,-0
-00001650: 2e34 3330 3039 3820 312e 3130 3632 312c  .430098 1.10621,
-00001660: 2d31 2e38 3836 3430 3820 312e 3536 3239  -1.886408 1.5629
-00001670: 372c 2d34 2e31 3930 3836 3920 382e 3939  7,-4.190869 8.99
-00001680: 3530 362c 382e 3732 3636 3735 2032 312e  506,8.726675 21.
-00001690: 3730 3631 362c 3330 2e37 3038 3935 3220  70616,30.708952 
-000016a0: 332e 3236 3730 322c 3339 2e34 3234 3433  3.26702,39.42443
-000016b0: 3820 4320 3937 2e36 3735 3238 372c 3638  8 C 97.675287,68
-000016c0: 2e36 3738 3831 3920 3738 2e39 3333 3336  .678819 78.93336
-000016d0: 332c 3539 2e32 3730 3836 3920 3538 2e31  3,59.270869 58.1
-000016e0: 3633 3936 312c 3532 2e32 3133 3833 3220  63961,52.213832 
-000016f0: 6c20 302e 3030 362c 2d30 2e30 3033 3420  l 0.006,-0.0034 
-00001700: 6d20 3134 312e 3635 3531 3539 2c30 2063  m 141.655159,0 c
-00001710: 202d 3236 2e36 3933 3534 2c31 332e 3736   -26.69354,13.76
-00001720: 3536 3535 202d 3432 2e32 3134 3034 2c32  5655 -42.21404,2
-00001730: 342e 3839 3635 3735 202d 3530 2e37 3136  4.896575 -50.716
-00001740: 322c 3334 2e33 3831 3038 3520 342e 3335  2,34.381085 4.35
-00001750: 3433 312c 3137 2e34 3532 3439 3320 3237  431,17.452493 27
-00001760: 2e30 3639 3437 2c31 382e 3234 3930 3333  .06947,18.249033
-00001770: 2033 352e 3337 3535 312c 3137 2e37 3539   35.37551,17.759
-00001780: 3538 3320 2d31 2e37 3030 3631 2c2d 302e  583 -1.70061,-0.
-00001790: 3739 3133 3820 2d33 2e31 3139 3933 2c2d  79138 -3.11993,-
-000017a0: 312e 3734 3031 3820 2d33 2e36 3232 3238  1.74018 -3.62228
-000017b0: 2c2d 332e 3139 3634 3920 322e 3038 3432  ,-3.19649 2.0842
-000017c0: 352c 2d31 2e34 3831 3235 3420 392e 3437  5,-1.481254 9.47
-000017d0: 3431 382c 2d30 2e31 3536 3535 2031 342e  418,-0.15655 14.
-000017e0: 3633 3237 372c 2d33 2e30 3534 3535 3420  63277,-3.054554 
-000017f0: 2d31 2e39 3831 3839 2c2d 302e 3431 3131  -1.98189,-0.4111
-00001800: 3720 2d32 2e39 3038 3332 2c2d 302e 3831  7 -2.90832,-0.81
-00001810: 3131 3620 2d33 2e38 3335 3631 2c2d 322e  116 -3.83561,-2.
-00001820: 3237 3334 3920 342e 3837 3437 332c 2d31  27349 4.87473,-1
-00001830: 2e35 3534 3337 2031 302e 3132 3533 362c  .55437 10.12536,
-00001840: 2d32 2e38 3934 3536 2031 332e 3231 3235  -2.89456 13.2125
-00001850: 392c 2d35 2e34 3639 3937 3920 2d31 2e36  9,-5.469979 -1.6
-00001860: 3636 3139 2c30 2e30 3230 3620 2d33 2e32  6619,0.0206 -3.2
-00001870: 3232 3239 2c30 2e33 3733 3332 202d 352e  2229,0.37332 -5.
-00001880: 3339 3835 382c 2d31 2e31 3336 3332 2034  39858,-1.13632 4
-00001890: 2e33 3636 3335 2c2d 322e 3335 3236 3320  .36635,-2.35263 
-000018a0: 392e 3032 3531 372c 2d34 2e32 3137 3533  9.02517,-4.21753
-000018b0: 2031 322e 3634 3438 362c 2d37 2e38 3134   12.64486,-7.814
-000018c0: 3031 202d 322e 3235 3830 312c 2d30 2e30  01 -2.25801,-0.0
-000018d0: 3535 3120 2d34 2e36 3931 352c 2d30 2e30  551 -4.6915,-0.0
-000018e0: 3232 3420 2d35 2e33 3938 3538 2c2d 302e  224 -5.39858,-0.
-000018f0: 3835 3234 3520 332e 3939 3536 312c 2d32  85245 3.99561,-2
-00001900: 2e34 3735 3634 2037 2e33 3637 3537 2c2d  .47564 7.36757,-
-00001910: 352e 3232 3832 3633 2031 302e 3135 3830  5.228263 10.1580
-00001920: 342c 2d38 2e32 3339 3830 3520 2d33 2e31  4,-8.239805 -3.1
-00001930: 3539 3439 2c30 2e33 3831 3036 3620 2d34  5949,0.381066 -4
-00001940: 2e34 3932 382c 302e 3035 3333 3320 2d35  .4928,0.05333 -5
-00001950: 2e32 3536 3635 2c2d 302e 3439 3731 3933  .25665,-0.497193
-00001960: 2033 2e30 3230 3135 2c2d 332e 3039 3431   3.02015,-3.0941
-00001970: 3220 362e 3834 3337 312c 2d35 2e37 3036  2 6.84371,-5.706
-00001980: 3533 3120 382e 3636 3634 362c 2d39 2e35  531 8.66646,-9.5
-00001990: 3138 3931 3520 2d32 2e33 3435 3735 2c30  18915 -2.34575,0
-000019a0: 2e38 3038 3538 3420 2d34 2e34 3931 3933  .808584 -4.49193
-000019b0: 2c31 2e31 3138 3235 3420 2d36 2e30 3338  ,1.118254 -6.038
-000019c0: 3536 2c2d 302e 3037 3035 3320 312e 3032  56,-0.07053 1.02
-000019d0: 3632 312c 2d32 2e33 3135 3634 3520 352e  621,-2.315645 5.
-000019e0: 3432 3433 382c 2d33 2e36 3831 3633 3420  42438,-3.681634 
-000019f0: 372e 3935 3539 342c 2d39 2e30 3933 3131  7.95594,-9.09311
-00001a00: 3920 2d32 2e34 3638 3736 2c30 2e32 3339  9 -2.46876,0.239
-00001a10: 3939 3420 2d35 2e30 3838 3035 2c30 2e35  994 -5.08805,0.5
-00001a20: 3338 3438 3220 2d35 2e36 3131 3931 2c30  38482 -5.61191,0
-00001a30: 2031 2e31 3438 3336 2c2d 342e 3637 3038   1.14836,-4.6708
-00001a40: 3538 2033 2e31 3134 3736 2c2d 372e 3239  58 3.11476,-7.29
-00001a50: 3631 3732 2035 2e30 3433 3332 2c2d 3130  6172 5.04332,-10
-00001a60: 2e30 3136 3130 3820 2d35 2e32 3834 3138  .016108 -5.28418
-00001a70: 2c2d 302e 3037 3832 3820 2d31 332e 3239  ,-0.07828 -13.29
-00001a80: 3038 372c 302e 3032 3036 3520 2d31 322e  087,0.02065 -12.
-00001a90: 3932 3837 332c 2d30 2e34 3235 3739 3620  92873,-0.425796 
-00001aa0: 6c20 332e 3236 3738 382c 2d33 2e33 3339  l 3.26788,-3.339
-00001ab0: 3237 3620 6320 2d35 2e31 3632 3033 2c2d  276 c -5.16203,-
-00001ac0: 312e 3338 3932 3135 202d 3130 2e34 3433  1.389215 -10.443
-00001ad0: 3632 2c30 2e32 3233 3635 3120 2d31 342e  62,0.223651 -14.
-00001ae0: 3237 3833 372c 312e 3432 3130 3432 202d  27837,1.421042 -
-00001af0: 312e 3732 3132 352c 2d31 2e33 3538 3234  1.72125,-1.35824
-00001b00: 3820 302e 3033 3031 2c2d 332e 3037 3630  8 0.0301,-3.0760
-00001b10: 3537 2032 2e31 3330 372c 2d34 2e38 3239  57 2.1307,-4.829
-00001b20: 3939 3420 2d34 2e33 3836 3133 2c30 2e35  994 -4.38613,0.5
-00001b30: 3834 3933 3320 2d38 2e33 3530 3737 2c31  84933 -8.35077,1
-00001b40: 2e35 3933 3934 3120 2d31 312e 3933 3334  .593941 -11.9334
-00001b50: 382c 322e 3938 3331 3536 202d 312e 3931  8,2.983156 -1.91
-00001b60: 3437 392c 2d31 2e37 3238 3133 3220 312e  479,-1.728132 1.
-00001b70: 3234 3239 382c 2d33 2e34 3537 3132 3320  24298,-3.457123 
-00001b80: 322e 3737 3036 392c 2d35 2e31 3835 3235  2.77069,-5.18525
-00001b90: 3420 2d36 2e37 3737 3438 2c31 2e32 3835  4 -6.77748,1.285
-00001ba0: 3133 3120 2d39 2e36 3438 3831 2c33 2e30  131 -9.64881,3.0
-00001bb0: 3932 3420 2d31 322e 3530 3239 332c 342e  924 -12.50293,4.
-00001bc0: 3930 3133 3839 202d 322e 3037 3034 392c  901389 -2.07049,
-00001bd0: 2d31 2e39 3834 3436 3920 2d30 2e31 3137  -1.984469 -0.117
-00001be0: 3835 2c2d 332e 3637 3133 3131 2031 2e32  85,-3.671311 1.2
-00001bf0: 3739 3131 2c2d 352e 3339 3835 3832 202d  7911,-5.398582 -
-00001c00: 352e 3131 3034 322c 312e 3839 3234 3239  5.11042,1.892429
-00001c10: 202d 372e 3734 3236 322c 342e 3333 3632   -7.74262,4.3362
-00001c20: 3432 202d 3130 2e35 3133 332c 362e 3734  42 -10.5133,6.74
-00001c30: 3832 3238 202d 302e 3934 3032 2c2d 312e  8228 -0.9402,-1.
-00001c40: 3236 3739 3237 202d 322e 3338 3730 342c  267927 -2.38704,
-00001c50: 2d32 2e31 3937 3739 3820 2d30 2e36 3339  -2.197798 -0.639
-00001c60: 3939 2c2d 352e 3235 3636 3520 2d33 2e36  99,-5.25665 -3.6
-00001c70: 3237 3434 2c32 2e30 3931 3133 3320 2d36  2744,2.091133 -6
-00001c80: 2e33 3630 3238 2c34 2e35 3535 3539 3120  .36028,4.555591 
-00001c90: 2d38 2e33 3831 3734 2c37 2e33 3136 3831  -8.38174,7.31681
-00001ca0: 3620 2d32 2e32 3435 312c 2d31 2e34 3239  6 -2.2451,-1.429
-00001cb0: 3634 3320 2d31 2e33 3337 362c 2d33 2e33  643 -1.3376,-3.3
-00001cc0: 3834 3836 3620 2d31 2e33 3439 3634 2c2d  84866 -1.34964,-
-00001cd0: 352e 3138 3631 3134 202d 332e 3737 3131  5.186114 -3.7711
-00001ce0: 2c33 2e30 3637 3435 3520 2d36 2e31 3634  ,3.067455 -6.164
-00001cf0: 3136 2c36 2e33 3331 3033 3320 2d39 2e30  16,6.331033 -9.0
-00001d00: 3933 3132 2c39 2e35 3138 3931 3520 2d30  9312,9.518915 -0
-00001d10: 2e35 3930 3039 2c2d 302e 3433 3030 3937  .59009,-0.430097
-00001d20: 202d 312e 3130 3632 312c 2d31 2e38 3836   -1.10621,-1.886
-00001d30: 3430 3720 2d31 2e35 3632 3937 2c2d 342e  407 -1.56297,-4.
-00001d40: 3139 3137 3239 202d 382e 3939 3530 362c  191729 -8.99506,
-00001d50: 382e 3732 3735 3336 202d 3231 2e37 3036  8.727536 -21.706
-00001d60: 3136 2c33 302e 3730 3938 3133 202d 332e  16,30.709813 -3.
-00001d70: 3236 3730 322c 3339 2e34 3235 3239 3920  26702,39.425299 
-00001d80: 3135 2e36 3833 3933 2c2d 3132 2e39 3435  15.68393,-12.945
-00001d90: 3932 3420 3334 2e34 3234 3939 2c2d 3232  924 34.42499,-22
-00001da0: 2e33 3532 3135 3420 3535 2e31 3935 3235  .352154 55.19525
-00001db0: 2c2d 3239 2e34 3039 3139 3120 6820 2d30  ,-29.409191 h -0
-00001dc0: 2e30 3033 220a 2020 2020 2066 696c 6c3d  .003".     fill=
-00001dd0: 2223 3735 6139 3238 220a 2020 2020 2069  "#75a928".     i
-00001de0: 643d 2270 6174 6835 3222 0a20 2020 2020  d="path52".     
-00001df0: 7374 796c 653d 2273 7472 6f6b 652d 7769  style="stroke-wi
-00001e00: 6474 683a 302e 3836 3031 3935 2220 2f3e  dth:0.860195" />
-00001e10: 0a20 203c 7061 7468 0a20 2020 2020 643d  .  <path.     d=
-00001e20: 226d 2031 3631 2e33 3238 3835 2c32 3239  "m 161.32885,229
-00001e30: 2e39 3235 3737 2063 2030 2e30 3932 392c  .92577 c 0.0929,
-00001e40: 3136 2e32 3836 3036 202d 3134 2e31 3439  16.28606 -14.149
-00001e50: 3335 2c32 392e 3535 3830 3120 2d33 312e  35,29.55801 -31.
-00001e60: 3831 3030 312c 3239 2e36 3433 3137 202d  81001,29.64317 -
-00001e70: 3137 2e36 3631 3532 2c30 2e30 3836 202d  17.66152,0.086 -
-00001e80: 3332 2e30 3534 3330 312c 2d31 332e 3034  32.054301,-13.04
-00001e90: 3635 3820 2d33 322e 3134 3732 3032 2c2d  658 -32.147202,-
-00001ea0: 3239 2e33 3332 3634 2061 2031 382e 3638  29.33264 a 18.68
-00001eb0: 3334 332c 3138 2e36 3833 3433 2030 2030  343,18.68343 0 0
-00001ec0: 2031 2030 2c2d 302e 3331 3035 3320 6320   1 0,-0.31053 c 
-00001ed0: 2d30 2e30 3932 392c 2d31 362e 3238 3532  -0.0929,-16.2852
-00001ee0: 3120 3134 2e31 3438 3439 322c 2d32 392e  1 14.148492,-29.
-00001ef0: 3535 3731 3520 3331 2e38 3130 3031 322c  55715 31.810012,
-00001f00: 2d32 392e 3634 3331 3720 3137 2e36 3631  -29.64317 17.661
-00001f10: 3532 2c2d 302e 3038 3620 3332 2e30 3533  52,-0.086 32.053
-00001f20: 3433 2c31 332e 3034 3635 3720 3332 2e31  43,13.04657 32.1
-00001f30: 3437 322c 3239 2e33 3332 3634 2076 2030  472,29.33264 v 0
-00001f40: 2e33 3130 3533 206d 202d 3530 2e34 3832  .31053 m -50.482
-00001f50: 3236 2c2d 3834 2e32 3338 3031 2063 2031  26,-84.23801 c 1
-00001f60: 332e 3235 3034 352c 382e 3638 3139 3420  3.25045,8.68194 
-00001f70: 3135 2e36 3339 3231 2c32 382e 3335 3937  15.63921,28.3597
-00001f80: 3620 352e 3333 3439 332c 3433 2e39 3531  6 5.33493,43.951
-00001f90: 3635 202d 3130 2e33 3034 3238 2c31 352e  65 -10.30428,15.
-00001fa0: 3539 3237 3520 2d32 392e 3339 3838 3739  59275 -29.398879
-00001fb0: 2c32 312e 3139 3630 3620 2d34 322e 3634  ,21.19606 -42.64
-00001fc0: 3933 3139 2c31 322e 3531 3439 3720 2d31  9319,12.51497 -1
-00001fd0: 332e 3235 3034 342c 2d38 2e36 3831 3935  3.25044,-8.68195
-00001fe0: 202d 3135 2e36 3338 3334 312c 2d32 382e   -15.638341,-28.
-00001ff0: 3335 3937 3620 2d35 2e33 3334 3932 382c  35976 -5.334928,
-00002000: 2d34 332e 3935 3136 3520 3130 2e33 3034  -43.95165 10.304
-00002010: 3237 332c 2d31 352e 3539 3237 3520 3239  273,-15.59275 29
-00002020: 2e33 3938 3837 362c 2d32 312e 3139 3630  .398876,-21.1960
-00002030: 3620 3432 2e36 3439 3331 372c 2d31 322e  6 42.649317,-12.
-00002040: 3531 3439 3720 6d20 3335 2e37 3633 3436  51497 m 35.76346
-00002050: 2c2d 312e 3537 3135 3820 6320 2d31 332e  ,-1.57158 c -13.
-00002060: 3234 3935 382c 382e 3638 3130 3920 2d31  24958,8.68109 -1
-00002070: 352e 3633 3833 342c 3238 2e33 3539 3736  5.63834,28.35976
-00002080: 202d 352e 3333 3439 322c 3433 2e39 3531   -5.33492,43.951
-00002090: 3635 2031 302e 3330 3432 372c 3135 2e35  65 10.30427,15.5
-000020a0: 3932 3735 2032 392e 3339 3838 372c 3231  9275 29.39887,21
-000020b0: 2e31 3936 3036 2034 322e 3634 3933 312c  .19606 42.64931,
-000020c0: 3132 2e35 3134 3131 2031 332e 3235 3034  12.51411 13.2504
-000020d0: 342c 2d38 2e36 3831 3038 2031 352e 3633  4,-8.68108 15.63
-000020e0: 3932 2c2d 3238 2e33 3538 3920 352e 3333  92,-28.3589 5.33
-000020f0: 3439 332c 2d34 332e 3935 3136 3520 4320  493,-43.95165 C 
-00002100: 3137 382e 3935 3539 362c 3134 312e 3033  178.95596,141.03
-00002110: 3834 2031 3539 2e38 3631 3335 2c31 3335  84 159.86135,135
-00002120: 2e34 3335 3120 3134 362e 3631 3030 352c  .4351 146.61005,
-00002130: 3134 342e 3131 3631 3820 4d20 3434 2e36  144.11618 M 44.6
-00002140: 3231 3931 362c 3135 392e 3838 3039 3720  21916,159.88097 
-00002150: 6320 3134 2e33 3035 3839 382c 2d33 2e38  c 14.305898,-3.8
-00002160: 3334 3735 2034 2e38 3239 3939 332c 3539  3475 4.829993,59
-00002170: 2e31 3833 3938 202d 362e 3831 3031 3632  .18398 -6.810162
-00002180: 2c35 342e 3031 3333 3520 2d31 322e 3830  ,54.01335 -12.80
-00002190: 3339 3939 2c2d 3130 2e32 3938 3235 202d  3999,-10.29825 -
-000021a0: 3136 2e39 3237 3737 322c 2d34 302e 3435  16.927772,-40.45
-000021b0: 3735 3420 362e 3831 3031 3632 2c2d 3534  754 6.810162,-54
-000021c0: 2e30 3133 3335 206d 2031 3635 2e33 3235  .01335 m 165.325
-000021d0: 3133 342c 2d30 2e37 3835 3336 2063 202d  134,-0.78536 c -
-000021e0: 3134 2e33 3037 3632 2c2d 332e 3833 3338  14.30762,-3.8338
-000021f0: 3920 2d34 2e38 3239 3939 2c35 392e 3138  9 -4.82999,59.18
-00002200: 3734 3220 362e 3831 3031 362c 3534 2e30  742 6.81016,54.0
-00002210: 3136 3739 2031 322e 3830 342c 2d31 302e  1679 12.804,-10.
-00002220: 3239 3931 3120 3136 2e39 3237 3738 2c2d  29911 16.92778,-
-00002230: 3430 2e34 3631 3834 202d 362e 3831 3031  40.46184 -6.8101
-00002240: 362c 2d35 342e 3031 3637 3920 6d20 2d34  6,-54.01679 m -4
-00002250: 382e 3630 3730 322c 2d34 362e 3932 3936  8.60702,-46.9296
-00002260: 3420 6320 3234 2e36 3838 3435 2c2d 342e  4 c 24.68845,-4.
-00002270: 3136 3835 3120 3435 2e32 3331 3632 2c31  16851 45.23162,1
-00002280: 302e 3439 3935 3320 3434 2e34 3032 3339  0.49953 44.40239
-00002290: 2c33 372e 3237 3035 3120 2d30 2e38 3132  ,37.27051 -0.812
-000022a0: 3032 2c31 302e 3236 3338 3520 2d35 332e  02,10.26385 -53.
-000022b0: 3439 3830 392c 2d33 352e 3734 3139 3520  49809,-35.74195 
-000022c0: 2d34 342e 3430 3233 392c 2d33 372e 3237  -44.40239,-37.27
-000022d0: 3035 3120 6d20 2d36 382e 3231 3334 3533  051 m -68.213453
-000022e0: 2c2d 302e 3738 3533 3620 6320 2d32 342e  ,-0.78536 c -24.
-000022f0: 3639 3031 372c 2d34 2e31 3639 3336 202d  69017,-4.16936 -
-00002300: 3435 2e32 3331 3632 2c31 302e 3530 3231  45.23162,10.5021
-00002310: 3220 2d34 342e 3430 3233 3933 2c33 372e  2 -44.402393,37.
-00002320: 3237 3133 3820 302e 3831 3230 3234 2c31  27138 0.812024,1
-00002330: 302e 3236 3239 3820 3533 2e34 3938 3935  0.26298 53.49895
-00002340: 362c 2d33 352e 3734 3238 3120 3434 2e34  6,-35.74281 44.4
-00002350: 3032 3339 332c 2d33 372e 3237 3133 3820  02393,-37.27138 
-00002360: 6d20 3335 2e34 3634 3131 332c 2d36 2e32  m 35.464113,-6.2
-00002370: 3433 3239 2063 202d 3134 2e37 3335 3134  4329 c -14.73514
-00002380: 2c2d 302e 3338 3336 3520 2d32 382e 3837  ,-0.38365 -28.87
-00002390: 3637 3432 2c31 302e 3933 3536 3520 2d32  6742,10.93565 -2
-000023a0: 382e 3931 3131 352c 3137 2e35 3031 3532  8.91115,17.50152
-000023b0: 202d 302e 3034 3034 332c 372e 3937 3734   -0.04043,7.9774
-000023c0: 3420 3131 2e36 3530 3438 2c31 362e 3134  4 11.65048,16.14
-000023d0: 3538 3520 3239 2e30 3131 382c 3136 2e33  585 29.0118,16.3
-000023e0: 3533 3136 2031 372e 3732 3836 312c 302e  5316 17.72861,0.
-000023f0: 3132 3634 3520 3239 2e30 3431 3839 2c2d  12645 29.04189,-
-00002400: 362e 3533 3833 3420 3239 2e30 3938 3637  6.53834 29.09867
-00002410: 2c2d 3134 2e37 3731 3236 2030 2e30 3635  ,-14.77126 0.065
-00002420: 342c 2d39 2e33 3237 3936 202d 3136 2e31  4,-9.32796 -16.1
-00002430: 3234 3336 2c2d 3139 2e32 3237 3934 202d  2436,-19.22794 -
-00002440: 3239 2e31 3939 3332 2c2d 3139 2e30 3834  29.19932,-19.084
-00002450: 3238 2076 2038 2e36 652d 3420 6d20 302e  28 v 8.6e-4 m 0.
-00002460: 3839 3937 372c 3136 332e 3539 3138 3320  89977,163.59183 
-00002470: 6320 3132 2e38 3437 3031 2c2d 302e 3536  c 12.84701,-0.56
-00002480: 3038 3520 3330 2e30 3835 3331 2c34 2e31  085 30.08531,4.1
-00002490: 3337 3534 2033 302e 3131 3937 322c 3130  3754 30.11972,10
-000024a0: 2e33 3731 3337 2030 2e32 3133 3333 2c36  .37137 0.21333,6
-000024b0: 2e30 3532 3333 202d 3135 2e36 3334 3034  .05233 -15.63404
-000024c0: 2c31 392e 3732 3737 3120 2d33 302e 3937  ,19.72771 -30.97
-000024d0: 3133 312c 3139 2e34 3633 3633 202d 3135  131,19.46363 -15
-000024e0: 2e38 3834 3337 2c30 2e36 3835 3537 202d  .88437,0.68557 -
-000024f0: 3331 2e34 3539 3931 362c 2d31 332e 3031  31.459916,-13.01
-00002500: 3133 3120 2d33 312e 3235 3630 352c 2d31  131 -31.25605,-1
-00002510: 372e 3735 3837 3220 2d30 2e32 3338 3237  7.75872 -0.23827
-00002520: 342c 2d36 2e39 3630 3720 3139 2e33 3430  4,-6.9607 19.340
-00002530: 3632 2c2d 3132 2e33 3935 3431 2033 322e  62,-12.39541 32.
-00002540: 3130 3736 342c 2d31 322e 3037 3632 3820  10764,-12.07628 
-00002550: 4d20 3832 2e30 3338 3636 372c 3233 312e  M 82.038667,231.
-00002560: 3738 3830 3920 6320 392e 3134 3634 352c  78809 c 9.14645,
-00002570: 3131 2e30 3139 3039 2031 332e 3331 3636  11.01909 13.3166
-00002580: 3734 2c33 302e 3337 3836 3420 352e 3638  74,30.37864 5.68
-00002590: 3333 3036 2c33 362e 3038 3630 3320 2d37  3306,36.08603 -7
-000025a0: 2e32 3231 3333 352c 342e 3335 3638 3820  .221335,4.35688 
-000025b0: 2d32 342e 3735 3831 3235 2c32 2e35 3632  -24.758125,2.562
-000025c0: 3532 202d 3337 2e32 3232 3334 372c 2d31  52 -37.222347,-1
-000025d0: 352e 3334 3431 3620 2d38 2e34 3036 3638  5.34416 -8.40668
-000025e0: 332c 2d31 352e 3032 3538 3820 2d37 2e33  3,-15.02588 -7.3
-000025f0: 3233 3639 382c 2d33 302e 3331 3538 3420  23698,-30.31584 
-00002600: 2d31 2e34 3231 3034 312c 2d33 342e 3830  -1.421041,-34.80
-00002610: 3737 3820 382e 3832 3634 3538 2c2d 352e  778 8.826458,-5.
-00002620: 3337 3632 3120 3232 2e34 3633 3938 352c  37621 22.463985,
-00002630: 312e 3838 3634 3120 3332 2e39 3630 3934  1.88641 32.96094
-00002640: 322c 3134 2e30 3635 3931 2068 202d 382e  2,14.06591 h -8.
-00002650: 3665 2d34 206d 2039 332e 3037 3330 3833  6e-4 m 93.073083
-00002660: 2c2d 332e 3439 3332 3520 6320 2d39 2e38  ,-3.49325 c -9.8
-00002670: 3936 3534 2c31 312e 3539 3131 3220 2d31  9654,11.59112 -1
-00002680: 352e 3430 3639 352c 3332 2e37 3332 3939  5.40695,32.73299
-00002690: 202d 382e 3138 3832 2c33 392e 3534 3232   -8.1882,39.5422
-000026a0: 3920 362e 3930 3330 372c 352e 3239 3032  9 6.90307,5.2902
-000026b0: 2032 352e 3433 3333 382c 342e 3535 3034   25.43338,4.5504
-000026c0: 3320 3339 2e31 3230 382c 2d31 342e 3434  3 39.1208,-14.44
-000026d0: 3138 3120 392e 3933 3836 392c 2d31 322e  181 9.93869,-12.
-000026e0: 3735 3538 3320 362e 3630 3838 382c 2d33  75583 6.60888,-3
-000026f0: 342e 3035 3835 3520 302e 3933 3135 392c  4.05855 0.93159,
-00002700: 2d33 392e 3731 3531 3920 2d38 2e34 3333  -39.71519 -8.433
-00002710: 3335 2c2d 362e 3532 3238 3620 2d32 302e  35,-6.52286 -20.
-00002720: 3534 3035 392c 312e 3832 3533 3320 2d33  54059,1.82533 -3
-00002730: 312e 3836 3431 392c 3134 2e36 3131 3237  1.86419,14.61127
-00002740: 2076 2030 2e30 3033 220a 2020 2020 2066   v 0.003".     f
-00002750: 696c 6c3d 2223 4243 3131 3432 220a 2020  ill="#BC1142".  
-00002760: 2020 2069 643d 2270 6174 6835 3422 0a20     id="path54". 
-00002770: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00002780: 2361 6130 3030 303b 7374 726f 6b65 2d77  #aa0000;stroke-w
-00002790: 6964 7468 3a30 2e38 3630 3139 3522 202f  idth:0.860195" /
-000027a0: 3e0a 2020 3c70 6174 680a 2020 2020 2073  >.  <path.     s
-000027b0: 7479 6c65 3d22 6669 6c6c 3a23 3431 3431  tyle="fill:#4141
-000027c0: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
-000027d0: 313b 7374 726f 6b65 3a23 3030 3030 3030  1;stroke:#000000
-000027e0: 3b73 7472 6f6b 652d 7769 6474 683a 372e  ;stroke-width:7.
-000027f0: 3037 3130 383b 7374 726f 6b65 2d6c 696e  07108;stroke-lin
-00002800: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00002810: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00002820: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00002830: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00002840: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00002850: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00002860: 2064 3d22 6d20 3234 322e 3536 3431 372c   d="m 242.56417,
-00002870: 3733 2e37 3734 3531 3620 6320 2d32 352e  73.774516 c -25.
-00002880: 3132 3735 352c 332e 3435 3434 3535 202d  12755,3.454455 -
-00002890: 3931 2e34 3131 3131 2c31 312e 3639 3034  91.41111,11.6904
-000028a0: 3035 202d 3533 2e38 3933 3034 2c35 332e  05 -53.89304,53.
-000028b0: 3839 3330 3534 2034 362e 3136 3130 382c  893054 46.16108,
-000028c0: 3339 2e37 3634 3235 2035 312e 3533 3131  39.76425 51.5311
-000028d0: 322c 2d32 382e 3631 3234 3031 2035 332e  2,-28.612401 53.
-000028e0: 3839 3330 342c 2d35 332e 3839 3330 3534  89304,-53.893054
-000028f0: 207a 220a 2020 2020 2069 643d 2270 6174   z".     id="pat
-00002900: 6836 3822 0a20 2020 2020 736f 6469 706f  h68".     sodipo
-00002910: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00002920: 6322 202f 3e0a 3c2f 7376 673e 0a         c" />.</svg>.
+00000030: 226e 6f22 3f3e 0d0a 3c73 7667 0d0a 2020  "no"?>..<svg..  
+00000040: 2078 6d6c 6e73 3a64 633d 2268 7474 703a   xmlns:dc="http:
+00000050: 2f2f 7075 726c 2e6f 7267 2f64 632f 656c  //purl.org/dc/el
+00000060: 656d 656e 7473 2f31 2e31 2f22 0d0a 2020  ements/1.1/"..  
+00000070: 2078 6d6c 6e73 3a63 633d 2268 7474 703a   xmlns:cc="http:
+00000080: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
+00000090: 732e 6f72 672f 6e73 2322 0d0a 2020 2078  s.org/ns#"..   x
+000000a0: 6d6c 6e73 3a72 6466 3d22 6874 7470 3a2f  mlns:rdf="http:/
+000000b0: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
+000000c0: 2f30 322f 3232 2d72 6466 2d73 796e 7461  /02/22-rdf-synta
+000000d0: 782d 6e73 2322 0d0a 2020 2078 6d6c 6e73  x-ns#"..   xmlns
+000000e0: 3a73 7667 3d22 6874 7470 3a2f 2f77 7777  :svg="http://www
+000000f0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
+00000100: 220d 0a20 2020 786d 6c6e 733d 2268 7474  "..   xmlns="htt
+00000110: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
+00000120: 3030 302f 7376 6722 0d0a 2020 2078 6d6c  000/svg"..   xml
+00000130: 6e73 3a73 6f64 6970 6f64 693d 2268 7474  ns:sodipodi="htt
+00000140: 703a 2f2f 736f 6469 706f 6469 2e73 6f75  p://sodipodi.sou
+00000150: 7263 6566 6f72 6765 2e6e 6574 2f44 5444  rceforge.net/DTD
+00000160: 2f73 6f64 6970 6f64 692d 302e 6474 6422  /sodipodi-0.dtd"
+00000170: 0d0a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ..   xmlns:inksc
+00000180: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
+00000190: 696e 6b73 6361 7065 2e6f 7267 2f6e 616d  inkscape.org/nam
+000001a0: 6573 7061 6365 732f 696e 6b73 6361 7065  espaces/inkscape
+000001b0: 220d 0a20 2020 7769 6474 683d 2231 3935  "..   width="195
+000001c0: 3722 0d0a 2020 2068 6569 6768 743d 2232  7"..   height="2
+000001d0: 3530 3022 0d0a 2020 2076 6965 7742 6f78  500"..   viewBox
+000001e0: 3d22 3020 3020 3235 3620 3332 3722 0d0a  ="0 0 256 327"..
+000001f0: 2020 2070 7265 7365 7276 6541 7370 6563     preserveAspec
+00000200: 7452 6174 696f 3d22 784d 696e 594d 696e  tRatio="xMinYMin
+00000210: 206d 6565 7422 0d0a 2020 2076 6572 7369   meet"..   versi
+00000220: 6f6e 3d22 312e 3122 0d0a 2020 2069 643d  on="1.1"..   id=
+00000230: 2273 7667 3536 220d 0a20 2020 736f 6469  "svg56"..   sodi
+00000240: 706f 6469 3a64 6f63 6e61 6d65 3d22 7069  podi:docname="pi
+00000250: 7761 7465 7266 6c6f 772e 7376 6722 0d0a  waterflow.svg"..
+00000260: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
+00000270: 696f 6e3d 2231 2e30 2e32 2d32 2028 6538  ion="1.0.2-2 (e8
+00000280: 3663 3837 3038 3739 2c20 3230 3231 2d30  6c870879, 2021-0
+00000290: 312d 3135 2922 3e0d 0a20 203c 6d65 7461  1-15)">..  <meta
+000002a0: 6461 7461 0d0a 2020 2020 2069 643d 226d  data..     id="m
+000002b0: 6574 6164 6174 6136 3222 3e0d 0a20 2020  etadata62">..   
+000002c0: 203c 7264 663a 5244 463e 0d0a 2020 2020   <rdf:RDF>..    
+000002d0: 2020 3c63 633a 576f 726b 0d0a 2020 2020    <cc:Work..    
+000002e0: 2020 2020 2072 6466 3a61 626f 7574 3d22       rdf:about="
+000002f0: 223e 0d0a 2020 2020 2020 2020 3c64 633a  ">..        <dc:
+00000300: 666f 726d 6174 3e69 6d61 6765 2f73 7667  format>image/svg
+00000310: 2b78 6d6c 3c2f 6463 3a66 6f72 6d61 743e  +xml</dc:format>
+00000320: 0d0a 2020 2020 2020 2020 3c64 633a 7479  ..        <dc:ty
+00000330: 7065 0d0a 2020 2020 2020 2020 2020 2072  pe..           r
+00000340: 6466 3a72 6573 6f75 7263 653d 2268 7474  df:resource="htt
+00000350: 703a 2f2f 7075 726c 2e6f 7267 2f64 632f  p://purl.org/dc/
+00000360: 6463 6d69 7479 7065 2f53 7469 6c6c 496d  dcmitype/StillIm
+00000370: 6167 6522 202f 3e0d 0a20 2020 2020 2020  age" />..       
+00000380: 203c 6463 3a74 6974 6c65 202f 3e0d 0a20   <dc:title />.. 
+00000390: 2020 2020 203c 2f63 633a 576f 726b 3e0d       </cc:Work>.
+000003a0: 0a20 2020 203c 2f72 6466 3a52 4446 3e0d  .    </rdf:RDF>.
+000003b0: 0a20 203c 2f6d 6574 6164 6174 613e 0d0a  .  </metadata>..
+000003c0: 2020 3c64 6566 730d 0a20 2020 2020 6964    <defs..     id
+000003d0: 3d22 6465 6673 3630 2220 2f3e 0d0a 2020  ="defs60" />..  
+000003e0: 3c73 6f64 6970 6f64 693a 6e61 6d65 6476  <sodipodi:namedv
+000003f0: 6965 770d 0a20 2020 2020 7061 6765 636f  iew..     pageco
+00000400: 6c6f 723d 2223 6666 6666 6666 220d 0a20  lor="#ffffff".. 
+00000410: 2020 2020 626f 7264 6572 636f 6c6f 723d      bordercolor=
+00000420: 2223 3636 3636 3636 220d 0a20 2020 2020  "#666666"..     
+00000430: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
+00000440: 220d 0a20 2020 2020 6f62 6a65 6374 746f  "..     objectto
+00000450: 6c65 7261 6e63 653d 2231 3022 0d0a 2020  lerance="10"..  
+00000460: 2020 2067 7269 6474 6f6c 6572 616e 6365     gridtolerance
+00000470: 3d22 3130 220d 0a20 2020 2020 6775 6964  ="10"..     guid
+00000480: 6574 6f6c 6572 616e 6365 3d22 3130 220d  etolerance="10".
+00000490: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
+000004a0: 6167 656f 7061 6369 7479 3d22 3022 0d0a  ageopacity="0"..
+000004b0: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
+000004c0: 6765 7368 6164 6f77 3d22 3222 0d0a 2020  geshadow="2"..  
+000004d0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+000004e0: 6f77 2d77 6964 7468 3d22 3139 3230 220d  ow-width="1920".
+000004f0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
+00000500: 696e 646f 772d 6865 6967 6874 3d22 3130  indow-height="10
+00000510: 3137 220d 0a20 2020 2020 6964 3d22 6e61  17"..     id="na
+00000520: 6d65 6476 6965 7735 3822 0d0a 2020 2020  medview58"..    
+00000530: 2073 686f 7767 7269 643d 2266 616c 7365   showgrid="false
+00000540: 220d 0a20 2020 2020 696e 6b73 6361 7065  "..     inkscape
+00000550: 3a73 6e61 702d 6262 6f78 3d22 6661 6c73  :snap-bbox="fals
+00000560: 6522 0d0a 2020 2020 2069 6e6b 7363 6170  e"..     inkscap
+00000570: 653a 7a6f 6f6d 3d22 302e 3131 3331 3337  e:zoom="0.113137
+00000580: 3038 220d 0a20 2020 2020 696e 6b73 6361  08"..     inksca
+00000590: 7065 3a63 783d 222d 3138 3637 2e32 3737  pe:cx="-1867.277
+000005a0: 3722 0d0a 2020 2020 2069 6e6b 7363 6170  7"..     inkscap
+000005b0: 653a 6379 3d22 3130 3535 2e33 3630 3922  e:cy="1055.3609"
+000005c0: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
+000005d0: 7769 6e64 6f77 2d78 3d22 2d38 220d 0a20  window-x="-8".. 
+000005e0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+000005f0: 646f 772d 793d 222d 3822 0d0a 2020 2020  dow-y="-8"..    
+00000600: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000610: 2d6d 6178 696d 697a 6564 3d22 3122 0d0a  -maximized="1"..
+00000620: 2020 2020 2069 6e6b 7363 6170 653a 6375       inkscape:cu
+00000630: 7272 656e 742d 6c61 7965 723d 2273 7667  rrent-layer="svg
+00000640: 3536 220d 0a20 2020 2020 696e 6b73 6361  56"..     inksca
+00000650: 7065 3a64 6f63 756d 656e 742d 726f 7461  pe:document-rota
+00000660: 7469 6f6e 3d22 3022 202f 3e0d 0a20 203c  tion="0" />..  <
+00000670: 7061 7468 0d0a 2020 2020 2064 3d22 6d20  path..     d="m 
+00000680: 3738 2e32 3033 3931 382c 3236 2e31 3231  78.203918,26.121
+00000690: 3534 3420 6320 2d31 2e34 3231 3930 322c  544 c -1.421902,
+000006a0: 302e 3034 3338 3720 2d32 2e39 3533 3034  0.04387 -2.95304
+000006b0: 382c 302e 3536 3934 3439 202d 342e 3639  8,0.569449 -4.69
+000006c0: 3036 3432 2c31 2e39 3339 3734 202d 342e  0642,1.93974 -4.
+000006d0: 3235 3336 3633 2c2d 312e 3634 3033 3932  253663,-1.640392
+000006e0: 202d 382e 3338 3038 3737 2c2d 322e 3231   -8.380877,-2.21
+000006f0: 3037 3031 202d 3132 2e30 3730 3235 322c  0701 -12.070252,
+00000700: 312e 3132 3934 3335 202d 352e 3639 3730  1.129435 -5.6970
+00000710: 372c 2d30 2e37 3338 3930 3720 2d37 2e35  7,-0.738907 -7.5
+00000720: 3438 3230 392c 302e 3738 3632 3138 202d  48209,0.786218 -
+00000730: 382e 3935 3131 3837 2c32 2e35 3636 3832  8.951187,2.56682
+00000740: 3120 2d31 2e32 3530 3732 332c 2d30 2e30  1 -1.250723,-0.0
+00000750: 3235 3820 2d39 2e33 3538 3035 382c 2d31  258 -9.358058,-1
+00000760: 2e32 3835 3939 3120 2d31 332e 3037 3636  .285991 -13.0766
+00000770: 382c 342e 3236 3035 3435 202d 392e 3334  8,4.260545 -9.34
+00000780: 3334 3335 2c2d 312e 3130 3533 3520 2d31  3435,-1.10535 -1
+00000790: 322e 3239 3634 3834 2c35 2e34 3935 3738  2.296484,5.49578
+000007a0: 3420 2d38 2e39 3530 3332 362c 3131 2e36  4 -8.950326,11.6
+000007b0: 3532 3139 3820 2d31 2e39 3038 3737 322c  52198 -1.908772,
+000007c0: 322e 3935 3339 3039 202d 332e 3838 3633  2.953909 -3.8863
+000007d0: 362c 352e 3837 3235 3439 2030 2e35 3736  6,5.872549 0.576
+000007e0: 3333 2c31 312e 3530 3531 3035 202d 312e  33,11.505105 -1.
+000007f0: 3537 3834 3537 2c33 2e31 3336 3237 202d  578457,3.13627 -
+00000800: 302e 3539 3935 3536 2c36 2e35 3339 3220  0.599556,6.5392 
+00000810: 332e 3131 3930 3636 2c31 302e 3635 3639  3.119066,10.6569
+00000820: 3532 202d 302e 3938 3036 3232 2c34 2e34  52 -0.980622,4.4
+00000830: 3130 3231 3920 302e 3934 3739 3335 2c37  10219 0.947935,7
+00000840: 2e35 3230 3638 3320 342e 3430 3834 3938  .520683 4.408498
+00000850: 2c39 2e39 3435 3537 3220 2d30 2e36 3437  ,9.945572 -0.647
+00000860: 3732 362c 362e 3033 3432 3635 2035 2e35  726,6.034265 5.5
+00000870: 3333 3633 332c 392e 3534 3330 3035 2037  33633,9.543005 7
+00000880: 2e33 3738 3735 312c 3130 2e37 3932 3836  .378751,10.79286
+00000890: 3520 302e 3730 3838 2c33 2e35 3135 3630  5 0.7088,3.51560
+000008a0: 3920 322e 3138 3537 3535 2c36 2e38 3334  9 2.185755,6.834
+000008b0: 3234 3920 392e 3234 3533 3733 2c38 2e36  249 9.245373,8.6
+000008c0: 3638 3137 3920 312e 3136 3437 3034 2c35  68179 1.164704,5
+000008d0: 2e32 3430 3331 3420 352e 3430 3731 3834  .240314 5.407184
+000008e0: 2c36 2e31 3435 3233 3420 392e 3531 3633  ,6.145234 9.5163
+000008f0: 3334 2c37 2e32 3434 3536 3420 2d31 332e  34,7.244564 -13.
+00000900: 3537 3938 3934 2c37 2e38 3934 3031 202d  579894,7.89401 -
+00000910: 3235 2e32 3235 3231 312c 3138 2e32 3739  25.225211,18.279
+00000920: 3134 202d 3235 2e31 3436 3037 332c 3433  14 -25.146073,43
+00000930: 2e37 3632 3431 206c 202d 312e 3938 3936  .76241 l -1.9896
+00000940: 332c 332e 3534 3833 2063 202d 3135 2e35  3,3.5483 c -15.5
+00000950: 3731 3234 352c 392e 3436 3930 3320 2d32  71245,9.46903 -2
+00000960: 392e 3538 3033 3736 392c 3339 2e39 3034  9.5803769,39.904
+00000970: 3434 202d 372e 3637 3239 3337 2c36 342e  44 -7.672937,64.
+00000980: 3634 3139 3220 312e 3433 3035 3034 2c37  64192 1.430504,7
+00000990: 2e37 3433 3437 2033 2e38 3330 3434 372c  .74347 3.830447,
+000009a0: 3133 2e33 3035 3439 2035 2e39 3637 3137  13.30549 5.96717
+000009b0: 312c 3139 2e34 3631 3034 2033 2e31 3935  1,19.46104 3.195
+000009c0: 3632 332c 3234 2e38 3034 3538 2032 342e  623,24.80458 24.
+000009d0: 3035 3237 3635 2c33 362e 3431 3937 3920  052765,36.41979 
+000009e0: 3239 2e35 3534 3537 312c 3337 2e37 3933  29.554571,37.793
+000009f0: 3532 2038 2e30 3630 3838 352c 362e 3134  52 8.060885,6.14
+00000a00: 3030 3720 3136 2e36 3436 3438 382c 3131  007 16.646488,11
+00000a10: 2e39 3636 3137 2032 382e 3236 3539 3939  .96617 28.265999
+00000a20: 2c31 362e 3034 3737 3920 3130 2e39 3531  ,16.04779 10.951
+00000a30: 3133 362c 3131 2e32 3935 3232 2032 322e  136,11.29522 22.
+00000a40: 3831 3636 3636 2c31 352e 3630 3034 3920  816666,15.60049 
+00000a50: 3334 2e37 3436 3731 362c 3135 2e35 3933  34.746716,15.593
+00000a60: 3631 2030 2e31 3735 3438 2c30 2032 342e  61 0.17548,0 24.
+00000a70: 3332 3337 332c 2d34 2e32 3937 3533 2033  32373,-4.29753 3
+00000a80: 352e 3237 3635 392c 2d31 352e 3539 3336  5.27659,-15.5936
+00000a90: 3120 3131 2e36 3137 3739 2c2d 342e 3038  1 11.61779,-4.08
+00000aa0: 3136 3220 3230 2e32 3033 3339 2c2d 392e  162 20.20339,-9.
+00000ab0: 3930 3737 3220 3238 2e32 3635 3939 2c2d  90772 28.26599,-
+00000ac0: 3136 2e30 3437 3739 2035 2e35 3030 3039  16.04779 5.50009
+00000ad0: 2c2d 312e 3337 3337 3320 3236 2e33 3537  ,-1.37373 26.357
+00000ae0: 3233 2c2d 3132 2e39 3838 3934 2032 392e  23,-12.98894 29.
+00000af0: 3535 3238 362c 2d33 372e 3739 3335 3220  55286,-37.79352 
+00000b00: 322e 3133 3637 322c 2d36 2e31 3535 3535  2.13672,-6.15555
+00000b10: 2034 2e35 3336 3636 2c2d 3131 2e37 3137   4.53666,-11.717
+00000b20: 3537 2035 2e39 3638 3033 2c2d 3139 2e34  57 5.96803,-19.4
+00000b30: 3631 3034 2032 312e 3930 3537 322c 2d32  6104 21.90572,-2
+00000b40: 342e 3734 3030 3620 372e 3839 3734 342c  4.74006 7.89744,
+00000b50: 2d35 352e 3137 3633 3420 2d37 2e36 3732  -55.17634 -7.672
+00000b60: 3934 2c2d 3634 2e36 3435 3336 206c 202d  94,-64.64536 l -
+00000b70: 312e 3939 3330 372c 2d33 2e35 3438 3320  1.99307,-3.5483 
+00000b80: 6320 302e 3037 3931 2c2d 3235 2e34 3830  c 0.0791,-25.480
+00000b90: 3639 202d 3131 2e35 3636 3138 2c2d 3335  69 -11.56618,-35
+00000ba0: 2e38 3636 3638 202d 3235 2e31 3436 3037  .86668 -25.14607
+00000bb0: 2c2d 3433 2e37 3632 3431 2034 2e31 3038  ,-43.76241 4.108
+00000bc0: 3239 2c2d 312e 3039 3933 3320 382e 3335  29,-1.09933 8.35
+00000bd0: 3234 392c 2d32 2e30 3034 3235 2039 2e35  249,-2.00425 9.5
+00000be0: 3135 3437 2c2d 372e 3234 3435 3634 2037  1547,-7.244564 7
+00000bf0: 2e30 3539 3632 2c2d 312e 3833 3438 2038  .05962,-1.8348 8
+00000c00: 2e35 3337 3433 2c2d 352e 3135 3235 3720  .53743,-5.15257 
+00000c10: 392e 3234 3533 372c 2d38 2e36 3638 3137  9.24537,-8.66817
+00000c20: 3920 312e 3834 3539 382c 2d31 2e32 3439  9 1.84598,-1.249
+00000c30: 3837 2038 2e30 3236 3438 2c2d 342e 3735  87 8.02648,-4.75
+00000c40: 3836 2037 2e33 3830 3437 2c2d 3130 2e37  86 7.38047,-10.7
+00000c50: 3932 3836 3620 332e 3435 3838 352c 2d32  92866 3.45885,-2
+00000c60: 2e34 3234 3838 3920 352e 3338 3832 362c  .424889 5.38826,
+00000c70: 2d35 2e35 3336 3231 3320 342e 3430 3637  -5.536213 4.4067
+00000c80: 382c 2d39 2e39 3435 3537 3220 332e 3731  8,-9.945572 3.71
+00000c90: 3934 382c 2d34 2e31 3137 3735 3220 342e  948,-4.117752 4.
+00000ca0: 3639 3735 322c 2d37 2e35 3230 3638 3220  69752,-7.520682 
+00000cb0: 332e 3131 3930 372c 2d31 302e 3635 3738  3.11907,-10.6578
+00000cc0: 3132 2034 2e34 3634 3431 2c2d 352e 3632  12 4.46441,-5.62
+00000cd0: 3931 3135 2032 2e34 3833 3338 2c2d 382e  9115 2.48338,-8.
+00000ce0: 3534 3737 3536 2030 2e35 3737 3139 2c2d  547756 0.57719,-
+00000cf0: 3131 2e35 3031 3636 3420 332e 3334 3434  11.501664 3.3444
+00000d00: 342c 2d36 2e31 3536 3431 3420 302e 3339  4,-6.156414 0.39
+00000d10: 3331 312c 2d31 322e 3735 3834 3039 202d  311,-12.758409 -
+00000d20: 382e 3935 3337 372c 2d31 312e 3635 3231  8.95377,-11.6521
+00000d30: 3938 202d 332e 3731 3630 342c 2d35 2e35  98 -3.71604,-5.5
+00000d40: 3436 3533 3620 2d31 312e 3832 3235 322c  46536 -11.82252,
+00000d50: 2d34 2e32 3837 3231 3120 2d31 332e 3037  -4.287211 -13.07
+00000d60: 3636 382c 2d34 2e32 3631 3430 3520 2d31  668,-4.261405 -1
+00000d70: 2e34 3032 3132 2c2d 312e 3737 3937 3433  .40212,-1.779743
+00000d80: 202d 332e 3235 3332 362c 2d33 2e33 3034   -3.25326,-3.304
+00000d90: 3836 3820 2d38 2e39 3530 3333 2c2d 322e  868 -8.95033,-2.
+00000da0: 3536 3539 3631 202d 332e 3638 3933 372c  565961 -3.68937,
+00000db0: 2d33 2e33 3430 3133 3620 2d37 2e38 3134  -3.340136 -7.814
+00000dc0: 3837 2c2d 322e 3737 3036 3837 202d 3132  87,-2.770687 -12
+00000dd0: 2e30 3730 3235 2c2d 312e 3132 3934 3336  .07025,-1.129436
+00000de0: 202d 352e 3035 3237 382c 2d33 2e39 3837   -5.05278,-3.987
+00000df0: 3030 3220 2d38 2e33 3935 352c 2d30 2e37  002 -8.3955,-0.7
+00000e00: 3931 3337 3920 2d31 322e 3231 3437 362c  91379 -12.21476,
+00000e10: 302e 3431 3731 3935 202d 362e 3131 3737  0.417195 -6.1177
+00000e20: 312c 2d31 2e39 3939 3039 3320 2d37 2e35  1,-1.999093 -7.5
+00000e30: 3137 3235 2c30 2e37 3338 3930 3720 2d31  1725,0.738907 -1
+00000e40: 302e 3532 3237 372c 312e 3835 3435 3820  0.52277,1.85458 
+00000e50: 2d36 2e36 3731 3637 2c2d 312e 3430 3938  -6.67167,-1.4098
+00000e60: 3539 202d 382e 3639 3931 352c 312e 3635  59 -8.69915,1.65
+00000e70: 3933 3135 202d 3131 2e38 3936 3439 2c34  9315 -11.89649,4
+00000e80: 2e38 3938 3830 3920 6c20 2d33 2e37 3231  .898809 l -3.721
+00000e90: 322c 2d30 2e30 3733 3938 2063 202d 3130  2,-0.07398 c -10
+00000ea0: 2e30 3632 3536 2c35 2e39 3330 3138 3320  .06256,5.930183 
+00000eb0: 2d31 352e 3036 3230 312c 3138 2e30 3035  -15.06201,18.005
+00000ec0: 3539 3620 2d31 362e 3833 3430 312c 3234  596 -16.83401,24
+00000ed0: 2e32 3133 3632 3220 2d31 2e37 3732 2c2d  .213622 -1.772,-
+00000ee0: 362e 3230 3838 3836 202d 362e 3736 3032  6.208886 -6.7602
+00000ef0: 372c 2d31 382e 3238 3433 202d 3136 2e38  7,-18.2843 -16.8
+00000f00: 3231 3132 2c2d 3234 2e32 3133 3632 3220  2112,-24.213622 
+00000f10: 6c20 2d33 2e37 3230 3334 2c30 2e30 3733  l -3.72034,0.073
+00000f20: 3938 2063 202d 332e 3230 3235 312c 2d33  98 c -3.20251,-3
+00000f30: 2e32 3339 3439 3420 2d35 2e32 3239 3133  .239494 -5.22913
+00000f40: 2c2d 362e 3330 3836 3638 202d 3131 2e39  ,-6.308668 -11.9
+00000f50: 3030 3739 372c 2d34 2e38 3938 3830 3920  00797,-4.898809 
+00000f60: 2d33 2e30 3036 3338 2c2d 312e 3131 3536  -3.00638,-1.1156
+00000f70: 3733 202d 342e 3339 3938 3936 2c2d 332e  73 -4.399896,-3.
+00000f80: 3835 3336 3733 202d 3130 2e35 3232 3736  853673 -10.52276
+00000f90: 322c 2d31 2e38 3534 3538 202d 322e 3530  2,-1.85458 -2.50
+00000fa0: 3636 3037 2c2d 302e 3739 3331 202d 342e  6607,-0.7931 -4.
+00000fb0: 3831 3139 3239 2c2d 322e 3434 3132 3333  811929,-2.441233
+00000fc0: 202d 372e 3532 3538 3434 2c2d 322e 3335   -7.525844,-2.35
+00000fd0: 3639 3334 204c 2039 2e31 3332 3030 3131  6934 L 9.1320011
+00000fe0: 2c31 3437 2e34 3034 3731 220d 0a20 2020  ,147.40471"..   
+00000ff0: 2020 6964 3d22 7061 7468 3530 220d 0a20    id="path50".. 
+00001000: 2020 2020 7374 796c 653d 2273 7472 6f6b      style="strok
+00001010: 652d 7769 6474 683a 302e 3836 3031 3935  e-width:0.860195
+00001020: 2220 2f3e 0d0a 2020 3c70 6174 680d 0a20  " />..  <path.. 
+00001030: 2020 2020 643d 224d 2035 382e 3136 3939      d="M 58.1699
+00001040: 3833 2c35 322e 3231 3033 3931 2043 2038  83,52.210391 C 8
+00001050: 342e 3836 3639 3837 2c36 352e 3937 3433  4.866987,65.9743
+00001060: 3637 2031 3030 2e33 3837 3438 2c37 372e  67 100.38748,77.
+00001070: 3130 3837 3238 2031 3038 2e38 3930 3531  108728 108.89051
+00001080: 2c38 362e 3539 3135 3137 2031 3034 2e35  ,86.591517 104.5
+00001090: 3336 322c 3130 342e 3034 3430 3120 3831  362,104.04401 81
+000010a0: 2e38 3230 3137 372c 3130 342e 3834 3035  .820177,104.8405
+000010b0: 3520 3733 2e35 3134 3133 372c 3130 342e  5 73.514137,104.
+000010c0: 3335 3131 2063 2031 2e37 3030 3630 352c  3511 c 1.700605,
+000010d0: 2d30 2e37 3931 3338 2033 2e31 3139 3932  -0.79138 3.11992
+000010e0: 362c 2d31 2e37 3430 3138 2033 2e36 3233  6,-1.74018 3.623
+000010f0: 3134 2c2d 332e 3139 3634 3920 2d32 2e30  14,-3.19649 -2.0
+00001100: 3834 3235 322c 2d31 2e34 3831 3235 3420  84252,-1.481254 
+00001110: 2d39 2e34 3734 3138 352c 2d30 2e31 3536  -9.474185,-0.156
+00001120: 3535 202d 3134 2e36 3333 3633 332c 2d33  55 -14.633633,-3
+00001130: 2e30 3534 3535 3420 312e 3938 3138 3839  .054554 1.981889
+00001140: 2c2d 302e 3431 3131 3720 322e 3930 3931  ,-0.41117 2.9091
+00001150: 3739 2c2d 302e 3831 3131 3620 332e 3833  79,-0.81116 3.83
+00001160: 3536 3038 2c2d 322e 3237 3334 3920 2d34  5608,-2.27349 -4
+00001170: 2e38 3733 3836 332c 2d31 2e35 3534 3337  .873863,-1.55437
+00001180: 202d 3130 2e31 3234 3439 322c 2d32 2e38   -10.124492,-2.8
+00001190: 3934 3536 202d 3133 2e32 3132 3539 312c  9456 -13.212591,
+000011a0: 2d35 2e34 3639 3937 3920 312e 3636 3631  -5.469979 1.6661
+000011b0: 3937 2c30 2e30 3230 3620 332e 3232 3232  97,0.0206 3.2222
+000011c0: 392c 302e 3337 3333 3220 352e 3339 3835  9,0.37332 5.3985
+000011d0: 3832 2c2d 312e 3133 3633 3220 2d34 2e33  82,-1.13632 -4.3
+000011e0: 3635 3438 382c 2d32 2e33 3532 3633 202d  65488,-2.35263 -
+000011f0: 392e 3032 3433 3033 2c2d 342e 3231 3735  9.024303,-4.2175
+00001200: 3320 2d31 322e 3634 3430 3032 2c2d 372e  3 -12.644002,-7.
+00001210: 3831 3430 3120 322e 3235 3731 3531 2c2d  81401 2.257151,-
+00001220: 302e 3035 3531 2034 2e36 3930 3634 322c  0.0551 4.690642,
+00001230: 2d30 2e30 3232 3420 352e 3339 3835 3832  -0.0224 5.398582
+00001240: 2c2d 302e 3835 3234 3520 2d33 2e39 3935  ,-0.85245 -3.995
+00001250: 3630 352c 2d32 2e34 3735 3634 202d 372e  605,-2.47564 -7.
+00001260: 3336 3735 3638 2c2d 352e 3232 3832 3633  367568,-5.228263
+00001270: 202d 3130 2e31 3538 3034 2c2d 382e 3233   -10.15804,-8.23
+00001280: 3938 3035 2033 2e31 3538 3633 352c 302e  9805 3.158635,0.
+00001290: 3338 3130 3636 2034 2e34 3932 3739 372c  381066 4.492797,
+000012a0: 302e 3035 3333 3320 352e 3235 3636 352c  0.05333 5.25665,
+000012b0: 2d30 2e34 3937 3139 3320 2d33 2e30 3231  -0.497193 -3.021
+000012c0: 3030 342c 2d33 2e30 3934 3132 202d 362e  004,-3.09412 -6.
+000012d0: 3834 3337 3039 2c2d 352e 3730 3635 3331  843709,-5.706531
+000012e0: 202d 382e 3636 3634 3632 2c2d 392e 3531   -8.666462,-9.51
+000012f0: 3839 3135 2032 2e33 3434 3839 312c 302e  8915 2.344891,0.
+00001300: 3830 3835 3834 2034 2e34 3931 3037 372c  808584 4.491077,
+00001310: 312e 3131 3832 3534 2036 2e30 3337 3730  1.118254 6.03770
+00001320: 372c 2d30 2e30 3730 3533 202d 312e 3032  7,-0.07053 -1.02
+00001330: 3632 3132 2c2d 322e 3331 3536 3435 202d  6212,-2.315645 -
+00001340: 352e 3432 3335 3238 2c2d 332e 3638 3136  5.423528,-3.6816
+00001350: 3334 202d 372e 3935 3539 3431 2c2d 392e  34 -7.955941,-9.
+00001360: 3039 3331 3139 2032 2e34 3639 3631 392c  093119 2.469619,
+00001370: 302e 3233 3939 3934 2035 2e30 3838 3035  0.239994 5.08805
+00001380: 322c 302e 3533 3834 3832 2035 2e36 3131  2,0.538482 5.611
+00001390: 3931 312c 3020 2d31 2e31 3435 3738 2c2d  911,0 -1.14578,-
+000013a0: 342e 3636 3931 3337 202d 332e 3131 3231  4.669137 -3.1121
+000013b0: 3835 2c2d 372e 3239 3434 3532 202d 352e  85,-7.294452 -5.
+000013c0: 3034 3037 3432 2c2d 3130 2e30 3134 3338  040742,-10.01438
+000013d0: 3720 352e 3238 3431 3737 2c2d 302e 3037  7 5.284177,-0.07
+000013e0: 3832 3820 3133 2e32 3930 3836 392c 302e  828 13.290869,0.
+000013f0: 3032 3036 3420 3132 2e39 3238 3732 372c  02064 12.928727,
+00001400: 2d30 2e34 3235 3739 3720 6c20 2d33 2e32  -0.425797 l -3.2
+00001410: 3637 3838 2c2d 332e 3333 3834 3135 2063  6788,-3.338415 c
+00001420: 2035 2e31 3632 3032 392c 2d31 2e33 3930   5.162029,-1.390
+00001430: 3037 3520 3130 2e34 3433 3632 352c 302e  075 10.443625,0.
+00001440: 3232 3237 3920 3134 2e32 3738 3337 332c  22279 14.278373,
+00001450: 312e 3432 3031 3831 2031 2e37 3231 3235  1.420181 1.72125
+00001460: 2c2d 312e 3335 3832 3437 202d 302e 3033  ,-1.358247 -0.03
+00001470: 3039 372c 2d33 2e30 3736 3035 3620 2d32  097,-3.076056 -2
+00001480: 2e31 3331 3536 332c 2d34 2e38 3239 3939  .131563,-4.82999
+00001490: 3320 342e 3338 3639 3934 2c30 2e35 3835  3 4.386994,0.585
+000014a0: 3739 3220 382e 3335 3037 3731 2c31 2e35  792 8.350771,1.5
+000014b0: 3933 3934 2031 312e 3933 3433 3432 2c32  9394 11.934342,2
+000014c0: 2e39 3833 3135 3520 312e 3931 3339 3334  .983155 1.913934
+000014d0: 2c2d 312e 3732 3831 3331 202d 312e 3234  ,-1.728131 -1.24
+000014e0: 3239 3831 2c2d 332e 3435 3731 3233 202d  2981,-3.457123 -
+000014f0: 322e 3737 3036 3837 2c2d 352e 3138 3532  2.770687,-5.1852
+00001500: 3534 2036 2e37 3737 3437 342c 312e 3238  54 6.777474,1.28
+00001510: 3531 3331 2039 2e36 3438 3830 342c 332e  5131 9.648804,3.
+00001520: 3039 3234 2031 322e 3530 3230 372c 342e  0924 12.50207,4.
+00001530: 3930 3133 3920 322e 3037 3034 3839 2c2d  90139 2.070489,-
+00001540: 312e 3938 3434 3720 302e 3131 3837 3037  1.98447 0.118707
+00001550: 2c2d 332e 3637 3133 3131 202d 312e 3237  ,-3.671311 -1.27
+00001560: 3832 3439 2c2d 352e 3339 3835 3833 2035  8249,-5.398583 5
+00001570: 2e31 3130 3431 372c 312e 3839 3234 3239  .110417,1.892429
+00001580: 2037 2e37 3432 3631 332c 342e 3333 3632   7.742613,4.3362
+00001590: 3432 2031 302e 3531 3333 2c36 2e37 3438  42 10.5133,6.748
+000015a0: 3232 3820 302e 3933 3933 3333 2c2d 312e  228 0.939333,-1.
+000015b0: 3236 3739 3237 2032 2e33 3837 3034 312c  267927 2.387041,
+000015c0: 2d32 2e31 3937 3739 3720 302e 3633 3931  -2.197797 0.6391
+000015d0: 3235 2c2d 352e 3235 3636 3520 332e 3632  25,-5.25665 3.62
+000015e0: 3833 3031 2c32 2e30 3931 3133 3420 362e  8301,2.091134 6.
+000015f0: 3336 3131 342c 342e 3535 3535 3932 2038  36114,4.555592 8
+00001600: 2e33 3832 3539 382c 372e 3331 3638 3137  .382598,7.316817
+00001610: 2032 2e32 3435 3130 382c 2d31 2e34 3239   2.245108,-1.429
+00001620: 3634 3420 312e 3333 3736 3032 2c2d 332e  644 1.337602,-3.
+00001630: 3338 3430 3036 2031 2e33 3439 3634 352c  384006 1.349645,
+00001640: 2d35 2e31 3836 3131 3420 332e 3737 3130  -5.186114 3.7710
+00001650: 3933 2c33 2e30 3637 3435 3420 362e 3136  93,3.067454 6.16
+00001660: 3431 3533 2c36 2e33 3331 3839 3320 392e  4153,6.331893 9.
+00001670: 3039 3331 3233 2c39 2e35 3138 3931 3520  093123,9.518915 
+00001680: 302e 3539 3030 392c 2d30 2e34 3330 3039  0.59009,-0.43009
+00001690: 3820 312e 3130 3632 312c 2d31 2e38 3836  8 1.10621,-1.886
+000016a0: 3430 3820 312e 3536 3239 372c 2d34 2e31  408 1.56297,-4.1
+000016b0: 3930 3836 3920 382e 3939 3530 362c 382e  90869 8.99506,8.
+000016c0: 3732 3636 3735 2032 312e 3730 3631 362c  726675 21.70616,
+000016d0: 3330 2e37 3038 3935 3220 332e 3236 3730  30.708952 3.2670
+000016e0: 322c 3339 2e34 3234 3433 3820 4320 3937  2,39.424438 C 97
+000016f0: 2e36 3735 3238 372c 3638 2e36 3738 3831  .675287,68.67881
+00001700: 3920 3738 2e39 3333 3336 332c 3539 2e32  9 78.933363,59.2
+00001710: 3730 3836 3920 3538 2e31 3633 3936 312c  70869 58.163961,
+00001720: 3532 2e32 3133 3833 3220 6c20 302e 3030  52.213832 l 0.00
+00001730: 362c 2d30 2e30 3033 3420 6d20 3134 312e  6,-0.0034 m 141.
+00001740: 3635 3531 3539 2c30 2063 202d 3236 2e36  655159,0 c -26.6
+00001750: 3933 3534 2c31 332e 3736 3536 3535 202d  9354,13.765655 -
+00001760: 3432 2e32 3134 3034 2c32 342e 3839 3635  42.21404,24.8965
+00001770: 3735 202d 3530 2e37 3136 322c 3334 2e33  75 -50.7162,34.3
+00001780: 3831 3038 3520 342e 3335 3433 312c 3137  81085 4.35431,17
+00001790: 2e34 3532 3439 3320 3237 2e30 3639 3437  .452493 27.06947
+000017a0: 2c31 382e 3234 3930 3333 2033 352e 3337  ,18.249033 35.37
+000017b0: 3535 312c 3137 2e37 3539 3538 3320 2d31  551,17.759583 -1
+000017c0: 2e37 3030 3631 2c2d 302e 3739 3133 3820  .70061,-0.79138 
+000017d0: 2d33 2e31 3139 3933 2c2d 312e 3734 3031  -3.11993,-1.7401
+000017e0: 3820 2d33 2e36 3232 3238 2c2d 332e 3139  8 -3.62228,-3.19
+000017f0: 3634 3920 322e 3038 3432 352c 2d31 2e34  649 2.08425,-1.4
+00001800: 3831 3235 3420 392e 3437 3431 382c 2d30  81254 9.47418,-0
+00001810: 2e31 3536 3535 2031 342e 3633 3237 372c  .15655 14.63277,
+00001820: 2d33 2e30 3534 3535 3420 2d31 2e39 3831  -3.054554 -1.981
+00001830: 3839 2c2d 302e 3431 3131 3720 2d32 2e39  89,-0.41117 -2.9
+00001840: 3038 3332 2c2d 302e 3831 3131 3620 2d33  0832,-0.81116 -3
+00001850: 2e38 3335 3631 2c2d 322e 3237 3334 3920  .83561,-2.27349 
+00001860: 342e 3837 3437 332c 2d31 2e35 3534 3337  4.87473,-1.55437
+00001870: 2031 302e 3132 3533 362c 2d32 2e38 3934   10.12536,-2.894
+00001880: 3536 2031 332e 3231 3235 392c 2d35 2e34  56 13.21259,-5.4
+00001890: 3639 3937 3920 2d31 2e36 3636 3139 2c30  69979 -1.66619,0
+000018a0: 2e30 3230 3620 2d33 2e32 3232 3239 2c30  .0206 -3.22229,0
+000018b0: 2e33 3733 3332 202d 352e 3339 3835 382c  .37332 -5.39858,
+000018c0: 2d31 2e31 3336 3332 2034 2e33 3636 3335  -1.13632 4.36635
+000018d0: 2c2d 322e 3335 3236 3320 392e 3032 3531  ,-2.35263 9.0251
+000018e0: 372c 2d34 2e32 3137 3533 2031 322e 3634  7,-4.21753 12.64
+000018f0: 3438 362c 2d37 2e38 3134 3031 202d 322e  486,-7.81401 -2.
+00001900: 3235 3830 312c 2d30 2e30 3535 3120 2d34  25801,-0.0551 -4
+00001910: 2e36 3931 352c 2d30 2e30 3232 3420 2d35  .6915,-0.0224 -5
+00001920: 2e33 3938 3538 2c2d 302e 3835 3234 3520  .39858,-0.85245 
+00001930: 332e 3939 3536 312c 2d32 2e34 3735 3634  3.99561,-2.47564
+00001940: 2037 2e33 3637 3537 2c2d 352e 3232 3832   7.36757,-5.2282
+00001950: 3633 2031 302e 3135 3830 342c 2d38 2e32  63 10.15804,-8.2
+00001960: 3339 3830 3520 2d33 2e31 3539 3439 2c30  39805 -3.15949,0
+00001970: 2e33 3831 3036 3620 2d34 2e34 3932 382c  .381066 -4.4928,
+00001980: 302e 3035 3333 3320 2d35 2e32 3536 3635  0.05333 -5.25665
+00001990: 2c2d 302e 3439 3731 3933 2033 2e30 3230  ,-0.497193 3.020
+000019a0: 3135 2c2d 332e 3039 3431 3220 362e 3834  15,-3.09412 6.84
+000019b0: 3337 312c 2d35 2e37 3036 3533 3120 382e  371,-5.706531 8.
+000019c0: 3636 3634 362c 2d39 2e35 3138 3931 3520  66646,-9.518915 
+000019d0: 2d32 2e33 3435 3735 2c30 2e38 3038 3538  -2.34575,0.80858
+000019e0: 3420 2d34 2e34 3931 3933 2c31 2e31 3138  4 -4.49193,1.118
+000019f0: 3235 3420 2d36 2e30 3338 3536 2c2d 302e  254 -6.03856,-0.
+00001a00: 3037 3035 3320 312e 3032 3632 312c 2d32  07053 1.02621,-2
+00001a10: 2e33 3135 3634 3520 352e 3432 3433 382c  .315645 5.42438,
+00001a20: 2d33 2e36 3831 3633 3420 372e 3935 3539  -3.681634 7.9559
+00001a30: 342c 2d39 2e30 3933 3131 3920 2d32 2e34  4,-9.093119 -2.4
+00001a40: 3638 3736 2c30 2e32 3339 3939 3420 2d35  6876,0.239994 -5
+00001a50: 2e30 3838 3035 2c30 2e35 3338 3438 3220  .08805,0.538482 
+00001a60: 2d35 2e36 3131 3931 2c30 2031 2e31 3438  -5.61191,0 1.148
+00001a70: 3336 2c2d 342e 3637 3038 3538 2033 2e31  36,-4.670858 3.1
+00001a80: 3134 3736 2c2d 372e 3239 3631 3732 2035  1476,-7.296172 5
+00001a90: 2e30 3433 3332 2c2d 3130 2e30 3136 3130  .04332,-10.01610
+00001aa0: 3820 2d35 2e32 3834 3138 2c2d 302e 3037  8 -5.28418,-0.07
+00001ab0: 3832 3820 2d31 332e 3239 3038 372c 302e  828 -13.29087,0.
+00001ac0: 3032 3036 3520 2d31 322e 3932 3837 332c  02065 -12.92873,
+00001ad0: 2d30 2e34 3235 3739 3620 6c20 332e 3236  -0.425796 l 3.26
+00001ae0: 3738 382c 2d33 2e33 3339 3237 3620 6320  788,-3.339276 c 
+00001af0: 2d35 2e31 3632 3033 2c2d 312e 3338 3932  -5.16203,-1.3892
+00001b00: 3135 202d 3130 2e34 3433 3632 2c30 2e32  15 -10.44362,0.2
+00001b10: 3233 3635 3120 2d31 342e 3237 3833 372c  23651 -14.27837,
+00001b20: 312e 3432 3130 3432 202d 312e 3732 3132  1.421042 -1.7212
+00001b30: 352c 2d31 2e33 3538 3234 3820 302e 3033  5,-1.358248 0.03
+00001b40: 3031 2c2d 332e 3037 3630 3537 2032 2e31  01,-3.076057 2.1
+00001b50: 3330 372c 2d34 2e38 3239 3939 3420 2d34  307,-4.829994 -4
+00001b60: 2e33 3836 3133 2c30 2e35 3834 3933 3320  .38613,0.584933 
+00001b70: 2d38 2e33 3530 3737 2c31 2e35 3933 3934  -8.35077,1.59394
+00001b80: 3120 2d31 312e 3933 3334 382c 322e 3938  1 -11.93348,2.98
+00001b90: 3331 3536 202d 312e 3931 3437 392c 2d31  3156 -1.91479,-1
+00001ba0: 2e37 3238 3133 3220 312e 3234 3239 382c  .728132 1.24298,
+00001bb0: 2d33 2e34 3537 3132 3320 322e 3737 3036  -3.457123 2.7706
+00001bc0: 392c 2d35 2e31 3835 3235 3420 2d36 2e37  9,-5.185254 -6.7
+00001bd0: 3737 3438 2c31 2e32 3835 3133 3120 2d39  7748,1.285131 -9
+00001be0: 2e36 3438 3831 2c33 2e30 3932 3420 2d31  .64881,3.0924 -1
+00001bf0: 322e 3530 3239 332c 342e 3930 3133 3839  2.50293,4.901389
+00001c00: 202d 322e 3037 3034 392c 2d31 2e39 3834   -2.07049,-1.984
+00001c10: 3436 3920 2d30 2e31 3137 3835 2c2d 332e  469 -0.11785,-3.
+00001c20: 3637 3133 3131 2031 2e32 3739 3131 2c2d  671311 1.27911,-
+00001c30: 352e 3339 3835 3832 202d 352e 3131 3034  5.398582 -5.1104
+00001c40: 322c 312e 3839 3234 3239 202d 372e 3734  2,1.892429 -7.74
+00001c50: 3236 322c 342e 3333 3632 3432 202d 3130  262,4.336242 -10
+00001c60: 2e35 3133 332c 362e 3734 3832 3238 202d  .5133,6.748228 -
+00001c70: 302e 3934 3032 2c2d 312e 3236 3739 3237  0.9402,-1.267927
+00001c80: 202d 322e 3338 3730 342c 2d32 2e31 3937   -2.38704,-2.197
+00001c90: 3739 3820 2d30 2e36 3339 3939 2c2d 352e  798 -0.63999,-5.
+00001ca0: 3235 3636 3520 2d33 2e36 3237 3434 2c32  25665 -3.62744,2
+00001cb0: 2e30 3931 3133 3320 2d36 2e33 3630 3238  .091133 -6.36028
+00001cc0: 2c34 2e35 3535 3539 3120 2d38 2e33 3831  ,4.555591 -8.381
+00001cd0: 3734 2c37 2e33 3136 3831 3620 2d32 2e32  74,7.316816 -2.2
+00001ce0: 3435 312c 2d31 2e34 3239 3634 3320 2d31  451,-1.429643 -1
+00001cf0: 2e33 3337 362c 2d33 2e33 3834 3836 3620  .3376,-3.384866 
+00001d00: 2d31 2e33 3439 3634 2c2d 352e 3138 3631  -1.34964,-5.1861
+00001d10: 3134 202d 332e 3737 3131 2c33 2e30 3637  14 -3.7711,3.067
+00001d20: 3435 3520 2d36 2e31 3634 3136 2c36 2e33  455 -6.16416,6.3
+00001d30: 3331 3033 3320 2d39 2e30 3933 3132 2c39  31033 -9.09312,9
+00001d40: 2e35 3138 3931 3520 2d30 2e35 3930 3039  .518915 -0.59009
+00001d50: 2c2d 302e 3433 3030 3937 202d 312e 3130  ,-0.430097 -1.10
+00001d60: 3632 312c 2d31 2e38 3836 3430 3720 2d31  621,-1.886407 -1
+00001d70: 2e35 3632 3937 2c2d 342e 3139 3137 3239  .56297,-4.191729
+00001d80: 202d 382e 3939 3530 362c 382e 3732 3735   -8.99506,8.7275
+00001d90: 3336 202d 3231 2e37 3036 3136 2c33 302e  36 -21.70616,30.
+00001da0: 3730 3938 3133 202d 332e 3236 3730 322c  709813 -3.26702,
+00001db0: 3339 2e34 3235 3239 3920 3135 2e36 3833  39.425299 15.683
+00001dc0: 3933 2c2d 3132 2e39 3435 3932 3420 3334  93,-12.945924 34
+00001dd0: 2e34 3234 3939 2c2d 3232 2e33 3532 3135  .42499,-22.35215
+00001de0: 3420 3535 2e31 3935 3235 2c2d 3239 2e34  4 55.19525,-29.4
+00001df0: 3039 3139 3120 6820 2d30 2e30 3033 220d  09191 h -0.003".
+00001e00: 0a20 2020 2020 6669 6c6c 3d22 2337 3561  .     fill="#75a
+00001e10: 3932 3822 0d0a 2020 2020 2069 643d 2270  928"..     id="p
+00001e20: 6174 6835 3222 0d0a 2020 2020 2073 7479  ath52"..     sty
+00001e30: 6c65 3d22 7374 726f 6b65 2d77 6964 7468  le="stroke-width
+00001e40: 3a30 2e38 3630 3139 3522 202f 3e0d 0a20  :0.860195" />.. 
+00001e50: 203c 7061 7468 0d0a 2020 2020 2064 3d22   <path..     d="
+00001e60: 6d20 3136 312e 3332 3838 352c 3232 392e  m 161.32885,229.
+00001e70: 3932 3537 3720 6320 302e 3039 3239 2c31  92577 c 0.0929,1
+00001e80: 362e 3238 3630 3620 2d31 342e 3134 3933  6.28606 -14.1493
+00001e90: 352c 3239 2e35 3538 3031 202d 3331 2e38  5,29.55801 -31.8
+00001ea0: 3130 3031 2c32 392e 3634 3331 3720 2d31  1001,29.64317 -1
+00001eb0: 372e 3636 3135 322c 302e 3038 3620 2d33  7.66152,0.086 -3
+00001ec0: 322e 3035 3433 3031 2c2d 3133 2e30 3436  2.054301,-13.046
+00001ed0: 3538 202d 3332 2e31 3437 3230 322c 2d32  58 -32.147202,-2
+00001ee0: 392e 3333 3236 3420 6120 3138 2e36 3833  9.33264 a 18.683
+00001ef0: 3433 2c31 382e 3638 3334 3320 3020 3020  43,18.68343 0 0 
+00001f00: 3120 302c 2d30 2e33 3130 3533 2063 202d  1 0,-0.31053 c -
+00001f10: 302e 3039 3239 2c2d 3136 2e32 3835 3231  0.0929,-16.28521
+00001f20: 2031 342e 3134 3834 3932 2c2d 3239 2e35   14.148492,-29.5
+00001f30: 3537 3135 2033 312e 3831 3030 3132 2c2d  5715 31.810012,-
+00001f40: 3239 2e36 3433 3137 2031 372e 3636 3135  29.64317 17.6615
+00001f50: 322c 2d30 2e30 3836 2033 322e 3035 3334  2,-0.086 32.0534
+00001f60: 332c 3133 2e30 3436 3537 2033 322e 3134  3,13.04657 32.14
+00001f70: 3732 2c32 392e 3333 3236 3420 7620 302e  72,29.33264 v 0.
+00001f80: 3331 3035 3320 6d20 2d35 302e 3438 3232  31053 m -50.4822
+00001f90: 362c 2d38 342e 3233 3830 3120 6320 3133  6,-84.23801 c 13
+00001fa0: 2e32 3530 3435 2c38 2e36 3831 3934 2031  .25045,8.68194 1
+00001fb0: 352e 3633 3932 312c 3238 2e33 3539 3736  5.63921,28.35976
+00001fc0: 2035 2e33 3334 3933 2c34 332e 3935 3136   5.33493,43.9516
+00001fd0: 3520 2d31 302e 3330 3432 382c 3135 2e35  5 -10.30428,15.5
+00001fe0: 3932 3735 202d 3239 2e33 3938 3837 392c  9275 -29.398879,
+00001ff0: 3231 2e31 3936 3036 202d 3432 2e36 3439  21.19606 -42.649
+00002000: 3331 392c 3132 2e35 3134 3937 202d 3133  319,12.51497 -13
+00002010: 2e32 3530 3434 2c2d 382e 3638 3139 3520  .25044,-8.68195 
+00002020: 2d31 352e 3633 3833 3431 2c2d 3238 2e33  -15.638341,-28.3
+00002030: 3539 3736 202d 352e 3333 3439 3238 2c2d  5976 -5.334928,-
+00002040: 3433 2e39 3531 3635 2031 302e 3330 3432  43.95165 10.3042
+00002050: 3733 2c2d 3135 2e35 3932 3735 2032 392e  73,-15.59275 29.
+00002060: 3339 3838 3736 2c2d 3231 2e31 3936 3036  398876,-21.19606
+00002070: 2034 322e 3634 3933 3137 2c2d 3132 2e35   42.649317,-12.5
+00002080: 3134 3937 206d 2033 352e 3736 3334 362c  1497 m 35.76346,
+00002090: 2d31 2e35 3731 3538 2063 202d 3133 2e32  -1.57158 c -13.2
+000020a0: 3439 3538 2c38 2e36 3831 3039 202d 3135  4958,8.68109 -15
+000020b0: 2e36 3338 3334 2c32 382e 3335 3937 3620  .63834,28.35976 
+000020c0: 2d35 2e33 3334 3932 2c34 332e 3935 3136  -5.33492,43.9516
+000020d0: 3520 3130 2e33 3034 3237 2c31 352e 3539  5 10.30427,15.59
+000020e0: 3237 3520 3239 2e33 3938 3837 2c32 312e  275 29.39887,21.
+000020f0: 3139 3630 3620 3432 2e36 3439 3331 2c31  19606 42.64931,1
+00002100: 322e 3531 3431 3120 3133 2e32 3530 3434  2.51411 13.25044
+00002110: 2c2d 382e 3638 3130 3820 3135 2e36 3339  ,-8.68108 15.639
+00002120: 322c 2d32 382e 3335 3839 2035 2e33 3334  2,-28.3589 5.334
+00002130: 3933 2c2d 3433 2e39 3531 3635 2043 2031  93,-43.95165 C 1
+00002140: 3738 2e39 3535 3936 2c31 3431 2e30 3338  78.95596,141.038
+00002150: 3420 3135 392e 3836 3133 352c 3133 352e  4 159.86135,135.
+00002160: 3433 3531 2031 3436 2e36 3130 3035 2c31  4351 146.61005,1
+00002170: 3434 2e31 3136 3138 204d 2034 342e 3632  44.11618 M 44.62
+00002180: 3139 3136 2c31 3539 2e38 3830 3937 2063  1916,159.88097 c
+00002190: 2031 342e 3330 3538 3938 2c2d 332e 3833   14.305898,-3.83
+000021a0: 3437 3520 342e 3832 3939 3933 2c35 392e  475 4.829993,59.
+000021b0: 3138 3339 3820 2d36 2e38 3130 3136 322c  18398 -6.810162,
+000021c0: 3534 2e30 3133 3335 202d 3132 2e38 3033  54.01335 -12.803
+000021d0: 3939 392c 2d31 302e 3239 3832 3520 2d31  999,-10.29825 -1
+000021e0: 362e 3932 3737 3732 2c2d 3430 2e34 3537  6.927772,-40.457
+000021f0: 3534 2036 2e38 3130 3136 322c 2d35 342e  54 6.810162,-54.
+00002200: 3031 3333 3520 6d20 3136 352e 3332 3531  01335 m 165.3251
+00002210: 3334 2c2d 302e 3738 3533 3620 6320 2d31  34,-0.78536 c -1
+00002220: 342e 3330 3736 322c 2d33 2e38 3333 3839  4.30762,-3.83389
+00002230: 202d 342e 3832 3939 392c 3539 2e31 3837   -4.82999,59.187
+00002240: 3432 2036 2e38 3130 3136 2c35 342e 3031  42 6.81016,54.01
+00002250: 3637 3920 3132 2e38 3034 2c2d 3130 2e32  679 12.804,-10.2
+00002260: 3939 3131 2031 362e 3932 3737 382c 2d34  9911 16.92778,-4
+00002270: 302e 3436 3138 3420 2d36 2e38 3130 3136  0.46184 -6.81016
+00002280: 2c2d 3534 2e30 3136 3739 206d 202d 3438  ,-54.01679 m -48
+00002290: 2e36 3037 3032 2c2d 3436 2e39 3239 3634  .60702,-46.92964
+000022a0: 2063 2032 342e 3638 3834 352c 2d34 2e31   c 24.68845,-4.1
+000022b0: 3638 3531 2034 352e 3233 3136 322c 3130  6851 45.23162,10
+000022c0: 2e34 3939 3533 2034 342e 3430 3233 392c  .49953 44.40239,
+000022d0: 3337 2e32 3730 3531 202d 302e 3831 3230  37.27051 -0.8120
+000022e0: 322c 3130 2e32 3633 3835 202d 3533 2e34  2,10.26385 -53.4
+000022f0: 3938 3039 2c2d 3335 2e37 3431 3935 202d  9809,-35.74195 -
+00002300: 3434 2e34 3032 3339 2c2d 3337 2e32 3730  44.40239,-37.270
+00002310: 3531 206d 202d 3638 2e32 3133 3435 332c  51 m -68.213453,
+00002320: 2d30 2e37 3835 3336 2063 202d 3234 2e36  -0.78536 c -24.6
+00002330: 3930 3137 2c2d 342e 3136 3933 3620 2d34  9017,-4.16936 -4
+00002340: 352e 3233 3136 322c 3130 2e35 3032 3132  5.23162,10.50212
+00002350: 202d 3434 2e34 3032 3339 332c 3337 2e32   -44.402393,37.2
+00002360: 3731 3338 2030 2e38 3132 3032 342c 3130  7138 0.812024,10
+00002370: 2e32 3632 3938 2035 332e 3439 3839 3536  .26298 53.498956
+00002380: 2c2d 3335 2e37 3432 3831 2034 342e 3430  ,-35.74281 44.40
+00002390: 3233 3933 2c2d 3337 2e32 3731 3338 206d  2393,-37.27138 m
+000023a0: 2033 352e 3436 3431 3133 2c2d 362e 3234   35.464113,-6.24
+000023b0: 3332 3920 6320 2d31 342e 3733 3531 342c  329 c -14.73514,
+000023c0: 2d30 2e33 3833 3635 202d 3238 2e38 3736  -0.38365 -28.876
+000023d0: 3734 322c 3130 2e39 3335 3635 202d 3238  742,10.93565 -28
+000023e0: 2e39 3131 3135 2c31 372e 3530 3135 3220  .91115,17.50152 
+000023f0: 2d30 2e30 3430 3433 2c37 2e39 3737 3434  -0.04043,7.97744
+00002400: 2031 312e 3635 3034 382c 3136 2e31 3435   11.65048,16.145
+00002410: 3835 2032 392e 3031 3138 2c31 362e 3335  85 29.0118,16.35
+00002420: 3331 3620 3137 2e37 3238 3631 2c30 2e31  316 17.72861,0.1
+00002430: 3236 3435 2032 392e 3034 3138 392c 2d36  2645 29.04189,-6
+00002440: 2e35 3338 3334 2032 392e 3039 3836 372c  .53834 29.09867,
+00002450: 2d31 342e 3737 3132 3620 302e 3036 3534  -14.77126 0.0654
+00002460: 2c2d 392e 3332 3739 3620 2d31 362e 3132  ,-9.32796 -16.12
+00002470: 3433 362c 2d31 392e 3232 3739 3420 2d32  436,-19.22794 -2
+00002480: 392e 3139 3933 322c 2d31 392e 3038 3432  9.19932,-19.0842
+00002490: 3820 7620 382e 3665 2d34 206d 2030 2e38  8 v 8.6e-4 m 0.8
+000024a0: 3939 3737 2c31 3633 2e35 3931 3833 2063  9977,163.59183 c
+000024b0: 2031 322e 3834 3730 312c 2d30 2e35 3630   12.84701,-0.560
+000024c0: 3835 2033 302e 3038 3533 312c 342e 3133  85 30.08531,4.13
+000024d0: 3735 3420 3330 2e31 3139 3732 2c31 302e  754 30.11972,10.
+000024e0: 3337 3133 3720 302e 3231 3333 332c 362e  37137 0.21333,6.
+000024f0: 3035 3233 3320 2d31 352e 3633 3430 342c  05233 -15.63404,
+00002500: 3139 2e37 3237 3731 202d 3330 2e39 3731  19.72771 -30.971
+00002510: 3331 2c31 392e 3436 3336 3320 2d31 352e  31,19.46363 -15.
+00002520: 3838 3433 372c 302e 3638 3535 3720 2d33  88437,0.68557 -3
+00002530: 312e 3435 3939 3136 2c2d 3133 2e30 3131  1.459916,-13.011
+00002540: 3331 202d 3331 2e32 3536 3035 2c2d 3137  31 -31.25605,-17
+00002550: 2e37 3538 3732 202d 302e 3233 3832 3734  .75872 -0.238274
+00002560: 2c2d 362e 3936 3037 2031 392e 3334 3036  ,-6.9607 19.3406
+00002570: 322c 2d31 322e 3339 3534 3120 3332 2e31  2,-12.39541 32.1
+00002580: 3037 3634 2c2d 3132 2e30 3736 3238 204d  0764,-12.07628 M
+00002590: 2038 322e 3033 3836 3637 2c32 3331 2e37   82.038667,231.7
+000025a0: 3838 3039 2063 2039 2e31 3436 3435 2c31  8809 c 9.14645,1
+000025b0: 312e 3031 3930 3920 3133 2e33 3136 3637  1.01909 13.31667
+000025c0: 342c 3330 2e33 3738 3634 2035 2e36 3833  4,30.37864 5.683
+000025d0: 3330 362c 3336 2e30 3836 3033 202d 372e  306,36.08603 -7.
+000025e0: 3232 3133 3335 2c34 2e33 3536 3838 202d  221335,4.35688 -
+000025f0: 3234 2e37 3538 3132 352c 322e 3536 3235  24.758125,2.5625
+00002600: 3220 2d33 372e 3232 3233 3437 2c2d 3135  2 -37.222347,-15
+00002610: 2e33 3434 3136 202d 382e 3430 3636 3833  .34416 -8.406683
+00002620: 2c2d 3135 2e30 3235 3838 202d 372e 3332  ,-15.02588 -7.32
+00002630: 3336 3938 2c2d 3330 2e33 3135 3834 202d  3698,-30.31584 -
+00002640: 312e 3432 3130 3431 2c2d 3334 2e38 3037  1.421041,-34.807
+00002650: 3738 2038 2e38 3236 3435 382c 2d35 2e33  78 8.826458,-5.3
+00002660: 3736 3231 2032 322e 3436 3339 3835 2c31  7621 22.463985,1
+00002670: 2e38 3836 3431 2033 322e 3936 3039 3432  .88641 32.960942
+00002680: 2c31 342e 3036 3539 3120 6820 2d38 2e36  ,14.06591 h -8.6
+00002690: 652d 3420 6d20 3933 2e30 3733 3038 332c  e-4 m 93.073083,
+000026a0: 2d33 2e34 3933 3235 2063 202d 392e 3839  -3.49325 c -9.89
+000026b0: 3635 342c 3131 2e35 3931 3132 202d 3135  654,11.59112 -15
+000026c0: 2e34 3036 3935 2c33 322e 3733 3239 3920  .40695,32.73299 
+000026d0: 2d38 2e31 3838 322c 3339 2e35 3432 3239  -8.1882,39.54229
+000026e0: 2036 2e39 3033 3037 2c35 2e32 3930 3220   6.90307,5.2902 
+000026f0: 3235 2e34 3333 3338 2c34 2e35 3530 3433  25.43338,4.55043
+00002700: 2033 392e 3132 3038 2c2d 3134 2e34 3431   39.1208,-14.441
+00002710: 3831 2039 2e39 3338 3639 2c2d 3132 2e37  81 9.93869,-12.7
+00002720: 3535 3833 2036 2e36 3038 3838 2c2d 3334  5583 6.60888,-34
+00002730: 2e30 3538 3535 2030 2e39 3331 3539 2c2d  .05855 0.93159,-
+00002740: 3339 2e37 3135 3139 202d 382e 3433 3333  39.71519 -8.4333
+00002750: 352c 2d36 2e35 3232 3836 202d 3230 2e35  5,-6.52286 -20.5
+00002760: 3430 3539 2c31 2e38 3235 3333 202d 3331  4059,1.82533 -31
+00002770: 2e38 3634 3139 2c31 342e 3631 3132 3720  .86419,14.61127 
+00002780: 7620 302e 3030 3322 0d0a 2020 2020 2066  v 0.003"..     f
+00002790: 696c 6c3d 2223 4243 3131 3432 220d 0a20  ill="#BC1142".. 
+000027a0: 2020 2020 6964 3d22 7061 7468 3534 220d      id="path54".
+000027b0: 0a20 2020 2020 7374 796c 653d 2266 696c  .     style="fil
+000027c0: 6c3a 2361 6130 3030 303b 7374 726f 6b65  l:#aa0000;stroke
+000027d0: 2d77 6964 7468 3a30 2e38 3630 3139 3522  -width:0.860195"
+000027e0: 202f 3e0d 0a20 203c 7061 7468 0d0a 2020   />..  <path..  
+000027f0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00002800: 3431 3431 6666 3b66 696c 6c2d 6f70 6163  4141ff;fill-opac
+00002810: 6974 793a 313b 7374 726f 6b65 3a23 3030  ity:1;stroke:#00
+00002820: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+00002830: 683a 372e 3037 3130 383b 7374 726f 6b65  h:7.07108;stroke
+00002840: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00002850: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00002860: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00002870: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00002880: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00002890: 726f 6b65 2d6f 7061 6369 7479 3a31 220d  roke-opacity:1".
+000028a0: 0a20 2020 2020 643d 226d 2032 3432 2e35  .     d="m 242.5
+000028b0: 3634 3137 2c37 332e 3737 3435 3136 2063  6417,73.774516 c
+000028c0: 202d 3235 2e31 3237 3535 2c33 2e34 3534   -25.12755,3.454
+000028d0: 3435 3520 2d39 312e 3431 3131 312c 3131  455 -91.41111,11
+000028e0: 2e36 3930 3430 3520 2d35 332e 3839 3330  .690405 -53.8930
+000028f0: 342c 3533 2e38 3933 3035 3420 3436 2e31  4,53.893054 46.1
+00002900: 3631 3038 2c33 392e 3736 3432 3520 3531  6108,39.76425 51
+00002910: 2e35 3331 3132 2c2d 3238 2e36 3132 3430  .53112,-28.61240
+00002920: 3120 3533 2e38 3933 3034 2c2d 3533 2e38  1 53.89304,-53.8
+00002930: 3933 3035 3420 7a22 0d0a 2020 2020 2069  93054 z"..     i
+00002940: 643d 2270 6174 6836 3822 0d0a 2020 2020  d="path68"..    
+00002950: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00002960: 7065 733d 2263 6363 2220 2f3e 0d0a 3c2f  pes="ccc" />..</
+00002970: 7376 673e 0d0a                           svg>..
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/img/play.png` & `piwwwaterflow-1.0.0/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/static/js/code.js` & `piwwwaterflow-1.0.0/piwwwaterflow/static/js/code.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,306 +1,309 @@
-var forceTriggersEnabled = true
-
-function _setEnableForceTriggers(enable) {
-    forceTriggersEnabled = enable
-}
-
-function getProgramName(index) {
-    return document.getElementById('program' + (index + 1) + 'trigger').textContent
-}
-
-function getValveName(index) {
-    return document.getElementById('valve' + (index + 1) + 'trigger').textContent
-}
-
-function _resetForceTriggers() {
-    document.getElementById('program1trigger').style.color = 'inherit';
-    document.getElementById('program2trigger').style.color = 'inherit';
-    document.getElementById('valve1trigger').style.color = 'inherit';
-    document.getElementById('valve2trigger').style.color = 'inherit';
-}
-
-function _activateForceTrigger(controlname) {
-    control = document.getElementById(controlname);
-    control.style.color = '#22FF22'
-}
-
-const inputs = document.querySelectorAll("input");
-
-function saveCurrentValues() {
-    for (const el of inputs) {
-        if (el.type == 'checkbox')
-            el.oldValue = el.checked;
-        else
-            el.oldValue = el.value;
-    }
-}
-
-function refreshSaveButton(e) {
-    var anychanged = false;
-    for (const el of inputs) {
-        if (el.type == 'checkbox') {
-            if (el.oldValue !== el.checked) {
-                el.changed = true
-                anychanged = true;
-            } else {
-                el.changed = false
-            }
-        } else {
-            if (el.oldValue !== el.value) {
-                el.changed = true
-                anychanged = true;
-            } else {
-                el.changed = false
-            }
-        }
-    }
-    document.getElementById("saveForm").disabled = !anychanged;
-}
-
-document.addEventListener("change", refreshSaveButton);
-
-function _datestringFromDate(dateobject) {
-    date = ("0" + dateobject.getDate()).slice(-2);
-    month = ("0" + (dateobject.getMonth() + 1)).slice(-2);
-    hours = ("0" + (dateobject.getHours())).slice(-2);
-    minutes = ("0" + (dateobject.getMinutes())).slice(-2);
-    seconds = ("0" + (dateobject.getSeconds())).slice(-2);
-    formattedDate = dateobject.getFullYear() + "-" + month + "-" + date + " " + hours + ":" + minutes + ":" + seconds;
-    return formattedDate
-}
-String.prototype.replaceAt = function(index, sourcelength, replacement) {
-    return this.substr(0, index) + replacement + this.substr(index + sourcelength);
-}
-
-function _readableDay(original, start, end, formattedNow, formattedTomorrow) {
-    if (original.slice(start, end) == formattedNow) {
-        return original.replaceAt(start, 10, 'Today')
-    } else {
-        if (original.slice(start, end) == formattedTomorrow) {
-            return original.replaceAt(start, 10, 'Tomorrow')
-        } else {
-            return original
-        }
-    }
-}
-
-update(true);
-
-setInterval("update(false);", 30000);
-
-function update(first_time) {
-    let requestservice = new XMLHttpRequest();
-    // Add timestamp to avoid caching
-    requestservice.open('GET', '/service?' + (new Date()).getTime());
-    requestservice.responseType = 'json';
-    requestservice.onload = function() {
-        var versionlabel = document.getElementById('version');
-        frontend = requestservice.response.version_frontend
-        backend = requestservice.response.version_backend
-        versionlabel.textContent = `PiWaterflow ${frontend} (Backend ${backend})`
-
-        // Status line update
-        now = new Date()
-        formattedNow = _datestringFromDate(now).slice(0, 10)
-        tomorrow = new Date(now.getTime())
-        tomorrow.setDate(now.getDate() + 1)
-        formattedTomorrow = _datestringFromDate(tomorrow).slice(0, 10)
-
-        lastlooptime = new Date(requestservice.response.lastlooptime)
-
-        formattedLastLoopDate = _datestringFromDate(lastlooptime)
-
-        // Remove date info, if its today... and keep only time info
-        if (formattedLastLoopDate.slice(0, 10) == formattedNow)
-            formattedLastLoopDate = formattedLastLoopDate.slice(11, )
-
-        lapseseconds = Math.trunc((now - lastlooptime) / 1000)
-
-        var statuscontrol = document.getElementById('status');
-        if (lapseseconds > 10 * 60) {
-            statuscontrol.innerHTML = "Status: Waterflow loop NOT running! (since " + formattedLastLoopDate + " ... " + lapseseconds + " seconds ago)"
-            statuscontrol.style.color = '#FF2222'
-        } else {
-            statuscontrol.innerHTML = "Status: Waterflow loop running OK. (" + formattedLastLoopDate + " ... " + lapseseconds + " seconds ago)"
-            statuscontrol.style.color = 'inherited'
-        }
-
-        // Log textarea update
-        logtextarea = document.getElementById("log");
-        atbottom = ((logtextarea.scrollHeight - logtextarea.scrollTop) <= logtextarea.clientHeight);
-
-        var newlines = "";
-        var lines = requestservice.response.log.split('\n');
-
-        for (var i = 0; i < lines.length; i++) {
-            if (lines[i].slice(20, 24) == 'Next') {
-                newstring = _readableDay(lines[i], 34, 44, formattedNow, formattedTomorrow)
-                newstring = _readableDay(newstring, 0, 10, formattedNow, formattedTomorrow)
-            } else {
-                newstring = _readableDay(lines[i], 0, 10, formattedNow, formattedTomorrow)
-            }
-            newlines += newstring + '\n'
-        }
-
-        logtextarea.value = newlines;
-        if (atbottom)
-            logtextarea.scrollTop = logtextarea.scrollHeight;
-
-        // Stop button update
-        if (requestservice.response.stop == false)
-            document.getElementById('stop').disabled = false
-        else
-            document.getElementById('stop').disabled = true
-
-        // Force triggers update
-        _resetForceTriggers();
-        var forcedObj = requestservice.response.forced;
-        if (forcedObj != null) {
-            _setEnableForceTriggers(false);
-
-            if (forcedObj.type == 'program') {
-                if (forcedObj.value == 0)
-                    _activateForceTrigger("program1trigger");
-                else
-                    _activateForceTrigger("program2trigger");
-            } else {
-                if (forcedObj.value == 0)
-                    _activateForceTrigger("valve1trigger");
-                else
-                    _activateForceTrigger("valve2trigger");
-            }
-        } else {
-            _setEnableForceTriggers(true)
-        }
-
-        // Controls update
-        var configObj = requestservice.response.config;
-        if (configObj != null) {
-            time1 = document.getElementById("time1");
-            if (!time1.changed)
-                time1.value = configObj.programs[0].start_time;
-            valve11 = document.getElementById("valve11");
-            if (!valve11.changed)
-                valve11.value = configObj.programs[0].valves[0].time
-            valve12 = document.getElementById("valve12");
-            if (!valve12.changed)
-                valve12.value = configObj.programs[0].valves[1].time
-            prog1enabled = document.getElementById("prog1enabled");
-            if (!prog1enabled.changed)
-                prog1enabled.checked = configObj.programs[0].enabled;
-
-            time1 = document.getElementById("time2");
-            if (!time1.changed)
-                time1.value = configObj.programs[1].start_time;
-            valve21 = document.getElementById("valve21");
-            if (!valve21.changed)
-                valve21.value = configObj.programs[1].valves[0].time
-            valve22 = document.getElementById("valve22");
-            if (!valve22.changed)
-                valve22.value = configObj.programs[1].valves[1].time
-            prog2enabled = document.getElementById("prog2enabled");
-            if (!prog2enabled.changed)
-                prog2enabled.checked = configObj.programs[1].enabled;
-
-            if (first_time) { // Get this value from the closure (parameter in update function)
-                // Set names of programs and valves
-                document.getElementById('program1trigger').textContent = configObj.programs[0].name;
-                document.getElementById('program2trigger').textContent = configObj.programs[1].name;
-                document.getElementById('valve1trigger').textContent = configObj.programs[0].valves[0].name;
-                document.getElementById('valve2trigger').textContent = configObj.programs[0].valves[1].name;
-
-                saveCurrentValues();
-                refreshSaveButton();
-            }
-        }
-    };
-    requestservice.send();
-}
-
-function forceProgram(control, program_forced) {
-    if (forceTriggersEnabled && confirm("Are you sure you want to force program?.")) {
-        let requestservice = new XMLHttpRequest();
-        requestservice.open('POST', '/force');
-        requestservice.responseType = 'text';
-        requestservice.onload = function() {
-            if (requestservice.response == 'true') {
-                control.style.color = '#22FF22'
-                _setEnableForceTriggers(false)
-            }
-        }
-        var data = new FormData();
-        data.append('type', 'program');
-        data.append('value', program_forced);
-
-        requestservice.send(data);
-    } else {
-        control.checked = false
-    }
-}
-
-function forceValve(control, valve_forced) {
-    if (forceTriggersEnabled && confirm("Are you sure you want to force valve?.")) {
-        let requestservice = new XMLHttpRequest();
-        requestservice.open('POST', '/force');
-        requestservice.responseType = 'text';
-        requestservice.onload = function() {
-            if (requestservice.response == 'true') {
-                control.style.color = '#22FF22'
-                _setEnableForceTriggers(false)
-            }
-        }
-        var data = new FormData();
-        data.append('type', 'valve');
-        data.append('value', valve_forced);
-
-        requestservice.send(data);
-    } else {
-        control.checked = false
-    }
-}
-
-function stopWaterflow(button) {
-    let requestservice = new XMLHttpRequest();
-    requestservice.open('POST', '/stop');
-    requestservice.send();
-    button.disabled = true;
-}
-
-function save(button) {
-    let requestservice = new XMLHttpRequest();
-    requestservice.open('POST', '/save');
-    requestservice.responseType = 'text';
-    requestservice.onload = function() {
-        if (requestservice.response == 'true') {
-            saveCurrentValues();
-            refreshSaveButton();
-            button.disabled = true;
-        }
-    }
-    var data = new FormData();
-    data.append('save', JSON.stringify(
-        [{
-            'name': getProgramName(0),
-            'time': document.getElementById("time1").value,
-            'valves': [{
-                'name': getValveName(0),
-                'time': parseInt(document.getElementById("valve11").value)
-            }, {
-                'name': getValveName(1),
-                'time': parseInt(document.getElementById("valve12").value)
-            }, ],
-            'enabled': document.getElementById("prog1enabled").checked
-        }, {
-            'name': getProgramName(1),
-            'time': document.getElementById("time2").value,
-            'valves': [{
-                'name': getValveName(0),
-                'time': parseInt(document.getElementById("valve21").value)
-            }, {
-                'name': getValveName(1),
-                'time': parseInt(document.getElementById("valve22").value)
-            }, ],
-            'enabled': document.getElementById("prog2enabled").checked
-        }]));
-    requestservice.send(data);
+var forceTriggersEnabled = true
+
+function _setEnableForceTriggers(enable) {
+    forceTriggersEnabled = enable
+}
+
+function getProgramName(index) {
+    return document.getElementById('program' + (index + 1) + 'trigger').textContent
+}
+
+function getValveName(index) {
+    return document.getElementById('valve' + (index + 1) + 'trigger').textContent
+}
+
+function _resetForceTriggers() {
+    document.getElementById('program1trigger').style.color = 'inherit';
+    document.getElementById('program2trigger').style.color = 'inherit';
+    document.getElementById('valve1trigger').style.color = 'inherit';
+    document.getElementById('valve2trigger').style.color = 'inherit';
+}
+
+function _activateForceTrigger(controlname) {
+    control = document.getElementById(controlname);
+    control.style.color = '#22FF22'
+}
+
+const inputs = document.querySelectorAll("input");
+
+function saveCurrentValues() {
+    for (const el of inputs) {
+        if (el.type == 'checkbox')
+            el.oldValue = el.checked;
+        else
+            el.oldValue = el.value;
+    }
+}
+
+function refreshSaveButton(e) {
+    var anychanged = false;
+    for (const el of inputs) {
+        if (el.type == 'checkbox') {
+            if (el.oldValue !== el.checked) {
+                el.changed = true
+                anychanged = true;
+            } else {
+                el.changed = false
+            }
+        } else {
+            if (el.oldValue !== el.value) {
+                el.changed = true
+                anychanged = true;
+            } else {
+                el.changed = false
+            }
+        }
+    }
+    document.getElementById("saveForm").disabled = !anychanged;
+}
+
+document.addEventListener("change", refreshSaveButton);
+
+function _datestringFromDate(dateobject) {
+    date = ("0" + dateobject.getDate()).slice(-2);
+    month = ("0" + (dateobject.getMonth() + 1)).slice(-2);
+    hours = ("0" + (dateobject.getHours())).slice(-2);
+    minutes = ("0" + (dateobject.getMinutes())).slice(-2);
+    seconds = ("0" + (dateobject.getSeconds())).slice(-2);
+    formattedDate = dateobject.getFullYear() + "-" + month + "-" + date + " " + hours + ":" + minutes + ":" + seconds;
+    return formattedDate
+}
+String.prototype.replaceAt = function(index, sourcelength, replacement) {
+    return this.substr(0, index) + replacement + this.substr(index + sourcelength);
+}
+
+function _readableDay(original, start, end, formattedNow, formattedTomorrow) {
+    if (original.slice(start, end) == formattedNow) {
+        return original.replaceAt(start, 10, 'Today')
+    } else {
+        if (original.slice(start, end) == formattedTomorrow) {
+            return original.replaceAt(start, 10, 'Tomorrow')
+        } else {
+            return original
+        }
+    }
+}
+
+update(true);
+
+setInterval("update(false);", 30000);
+
+function update(first_time) {
+    let requestservice = new XMLHttpRequest();
+    // Add timestamp to avoid caching
+    requestservice.open('GET', '/service?' + (new Date()).getTime());
+    requestservice.responseType = 'json';
+    requestservice.onload = function() {
+        if (requestservice.status == 401) {
+            document.location.reload()
+        }
+        var versionlabel = document.getElementById('version');
+        frontend = requestservice.response.version_frontend
+        backend = requestservice.response.version_backend
+        versionlabel.textContent = `PiWaterflow ${frontend} (Backend ${backend})`
+
+        // Status line update
+        now = new Date()
+        formattedNow = _datestringFromDate(now).slice(0, 10)
+        tomorrow = new Date(now.getTime())
+        tomorrow.setDate(now.getDate() + 1)
+        formattedTomorrow = _datestringFromDate(tomorrow).slice(0, 10)
+
+        lastlooptime = new Date(requestservice.response.lastlooptime)
+
+        formattedLastLoopDate = _datestringFromDate(lastlooptime)
+
+        // Remove date info, if its today... and keep only time info
+        if (formattedLastLoopDate.slice(0, 10) == formattedNow)
+            formattedLastLoopDate = formattedLastLoopDate.slice(11, )
+
+        lapseseconds = Math.trunc((now - lastlooptime) / 1000)
+
+        var statuscontrol = document.getElementById('status');
+        if (lapseseconds > 10 * 60) {
+            statuscontrol.innerHTML = "Status: Waterflow loop NOT running! (since " + formattedLastLoopDate + " ... " + lapseseconds + " seconds ago)"
+            statuscontrol.style.color = '#FF2222'
+        } else {
+            statuscontrol.innerHTML = "Status: Waterflow loop running OK. (" + formattedLastLoopDate + " ... " + lapseseconds + " seconds ago)"
+            statuscontrol.style.color = 'inherited'
+        }
+
+        // Log textarea update
+        logtextarea = document.getElementById("log");
+        atbottom = ((logtextarea.scrollHeight - logtextarea.scrollTop) <= logtextarea.clientHeight);
+
+        var newlines = "";
+        var lines = requestservice.response.log.split('\n');
+
+        for (var i = 0; i < lines.length; i++) {
+            if (lines[i].slice(20, 24) == 'Next') {
+                newstring = _readableDay(lines[i], 34, 44, formattedNow, formattedTomorrow)
+                newstring = _readableDay(newstring, 0, 10, formattedNow, formattedTomorrow)
+            } else {
+                newstring = _readableDay(lines[i], 0, 10, formattedNow, formattedTomorrow)
+            }
+            newlines += newstring + '\n'
+        }
+
+        logtextarea.value = newlines;
+        if (atbottom)
+            logtextarea.scrollTop = logtextarea.scrollHeight;
+
+        // Stop button update
+        if (requestservice.response.stop == false)
+            document.getElementById('stop').disabled = false
+        else
+            document.getElementById('stop').disabled = true
+
+        // Force triggers update
+        _resetForceTriggers();
+        var forcedObj = requestservice.response.forced;
+        if (forcedObj != null) {
+            _setEnableForceTriggers(false);
+
+            if (forcedObj.type == 'program') {
+                if (forcedObj.value == 0)
+                    _activateForceTrigger("program1trigger");
+                else
+                    _activateForceTrigger("program2trigger");
+            } else {
+                if (forcedObj.value == 0)
+                    _activateForceTrigger("valve1trigger");
+                else
+                    _activateForceTrigger("valve2trigger");
+            }
+        } else {
+            _setEnableForceTriggers(true)
+        }
+
+        // Controls update
+        var configObj = requestservice.response.config;
+        if (configObj != null) {
+            time1 = document.getElementById("time1");
+            if (!time1.changed)
+                time1.value = configObj.programs[0].start_time;
+            valve11 = document.getElementById("valve11");
+            if (!valve11.changed)
+                valve11.value = configObj.programs[0].valves[0].time
+            valve12 = document.getElementById("valve12");
+            if (!valve12.changed)
+                valve12.value = configObj.programs[0].valves[1].time
+            prog1enabled = document.getElementById("prog1enabled");
+            if (!prog1enabled.changed)
+                prog1enabled.checked = configObj.programs[0].enabled;
+
+            time1 = document.getElementById("time2");
+            if (!time1.changed)
+                time1.value = configObj.programs[1].start_time;
+            valve21 = document.getElementById("valve21");
+            if (!valve21.changed)
+                valve21.value = configObj.programs[1].valves[0].time
+            valve22 = document.getElementById("valve22");
+            if (!valve22.changed)
+                valve22.value = configObj.programs[1].valves[1].time
+            prog2enabled = document.getElementById("prog2enabled");
+            if (!prog2enabled.changed)
+                prog2enabled.checked = configObj.programs[1].enabled;
+
+            if (first_time) { // Get this value from the closure (parameter in update function)
+                // Set names of programs and valves
+                document.getElementById('program1trigger').textContent = configObj.programs[0].name;
+                document.getElementById('program2trigger').textContent = configObj.programs[1].name;
+                document.getElementById('valve1trigger').textContent = configObj.programs[0].valves[0].name;
+                document.getElementById('valve2trigger').textContent = configObj.programs[0].valves[1].name;
+
+                saveCurrentValues();
+                refreshSaveButton();
+            }
+        }
+    };
+    requestservice.send();
+}
+
+function forceProgram(control, program_forced) {
+    if (forceTriggersEnabled && confirm("Are you sure you want to force program?.")) {
+        let requestservice = new XMLHttpRequest();
+        requestservice.open('POST', '/force');
+        requestservice.responseType = 'text';
+        requestservice.onload = function() {
+            if (requestservice.response == 'true') {
+                control.style.color = '#22FF22'
+                _setEnableForceTriggers(false)
+            }
+        }
+        var data = new FormData();
+        data.append('type', 'program');
+        data.append('value', program_forced);
+
+        requestservice.send(data);
+    } else {
+        control.checked = false
+    }
+}
+
+function forceValve(control, valve_forced) {
+    if (forceTriggersEnabled && confirm("Are you sure you want to force valve?.")) {
+        let requestservice = new XMLHttpRequest();
+        requestservice.open('POST', '/force');
+        requestservice.responseType = 'text';
+        requestservice.onload = function() {
+            if (requestservice.response == 'true') {
+                control.style.color = '#22FF22'
+                _setEnableForceTriggers(false)
+            }
+        }
+        var data = new FormData();
+        data.append('type', 'valve');
+        data.append('value', valve_forced);
+
+        requestservice.send(data);
+    } else {
+        control.checked = false
+    }
+}
+
+function stopWaterflow(button) {
+    let requestservice = new XMLHttpRequest();
+    requestservice.open('POST', '/stop');
+    requestservice.send();
+    button.disabled = true;
+}
+
+function save(button) {
+    let requestservice = new XMLHttpRequest();
+    requestservice.open('POST', '/save');
+    requestservice.responseType = 'text';
+    requestservice.onload = function() {
+        if (requestservice.response == 'true') {
+            saveCurrentValues();
+            refreshSaveButton();
+            button.disabled = true;
+        }
+    }
+    var data = new FormData();
+    data.append('save', JSON.stringify(
+        [{
+            'name': getProgramName(0),
+            'time': document.getElementById("time1").value,
+            'valves': [{
+                'name': getValveName(0),
+                'time': parseInt(document.getElementById("valve11").value)
+            }, {
+                'name': getValveName(1),
+                'time': parseInt(document.getElementById("valve12").value)
+            }, ],
+            'enabled': document.getElementById("prog1enabled").checked
+        }, {
+            'name': getProgramName(1),
+            'time': document.getElementById("time2").value,
+            'valves': [{
+                'name': getValveName(0),
+                'time': parseInt(document.getElementById("valve21").value)
+            }, {
+                'name': getValveName(1),
+                'time': parseInt(document.getElementById("valve22").value)
+            }, ],
+            'enabled': document.getElementById("prog2enabled").checked
+        }]));
+    requestservice.send(data);
 }
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/webservice.py` & `piwwwaterflow-1.0.0/piwwwaterflow/webservice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,176 @@
-""" Webservice to control and manage the piwaterflow loop """
-from datetime import datetime
-import json
-from flask import Flask, render_template, request, make_response, Response
-from flask_compress import Compress
-from importlib_metadata import version, PackageNotFoundError
-
-from piwaterflow import Waterflow
-from log_mgr import Logger, LoggerMode
-from revproxy_auth import RevProxyAuth
-
-
-class PiWWWaterflowService:
-    """Class for the web service... its an interface to the real functionality in piwaterflow package.
-    """
-    def __init__(self,  template_folder, static_folder):
-
-        self.logger = Logger(self.class_name(), log_file_name='piwwwaterflow', mode=LoggerMode.BOTH, dry_run=False)
-        self.logger.info("Launching piwwwaterflow...")
-
-        self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
-
-        self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
-
-        self.app.add_url_rule('/', 'waterflow', self.waterflow_endpoint, methods=['GET', 'POST'])
-
-        self.app.add_url_rule('/service', 'service', self.on_service_request, methods=['GET'])
-        self.app.add_url_rule('/force', 'force', self.on_force, methods=['GET', 'POST'])
-        self.app.add_url_rule('/stop', 'stop', self.on_stop, methods=['GET', 'POST'])
-        self.app.add_url_rule('/save', 'save', self.on_save, methods=['POST'])
-
-        Compress(self.app)
-
-    @classmethod
-    def class_name(cls):
-        """ class name """
-        return "piwwwaterflow"
-
-    def get_app(self):
-        """ Returns WSGI app
-        Returns:
-            WSGI app:
-        """
-        return self.app
-
-    def run(self):
-        """ Run function """
-        self.app.run()
-
-    def waterflow_endpoint(self):
-        """ Main endpoint that returns the main page for piwaterflow
-        Returns:
-            response: The main html content
-        """
-        return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
-
-    def on_service_request(self) -> dict:
-        """ Gets all the information from the waterflow service
-        Args:
-            data (dict):'first_time': This value is only bypassed to the caller
-        Returns:
-            dict:Dictionary with all the information about the status of the waterflow system
-        """
-        self.logger.info('Service requested...')
-
-        waterflow = Waterflow()
-
-        try:
-            ver_backend = version('piwaterflow')
-            ver_frontend = version('piwwwwaterflow')
-        except PackageNotFoundError:
-            ver_backend = '?.?.?'
-            ver_frontend = '?.?.?'
-
-        responsedict = None
-
-        try:
-            responsedict = {'log': waterflow.get_log(),
-                            'forced': waterflow.get_forced_info(),
-                            'stop': waterflow.stop_requested(),
-                            'config': self._filter_public_config(waterflow.config.get_dict_copy()),
-                            'lastlooptime': waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
-                            'version_backend': ver_backend,
-                            'version_frontend': ver_frontend
-                            }
-            # Change to string so that javascript can manage with it
-            for program in responsedict['config']['programs']:
-                program['start_time'] = program['start_time'].strftime('%H:%M')
-        except Exception as ex:
-            self.logger.error('Error calculating service request: %s', ex)
-            raise RuntimeError(f'Exception on service request: {ex}') from ex
-
-        return make_response(json.dumps(responsedict), 200)
-
-    def on_force(self):
-        """ On force action request
-        Args:
-            data (dict): 'type': Must be 'valve' or 'program'
-                         'value': Must be the index of the program or value to be forced
-        """
-        waterflow = Waterflow()
-
-        if request.method == 'POST':
-            type_force = request.form.get('type')
-            value_force = request.form.get('value')
-            self.logger.info('Force requested: %s = %s', type_force, value_force)
-
-            waterflow.force(type_force, value_force)
-            return make_response('Force scheduled: %s = %s', type_force, value_force, 200)
-        else:
-            forced_data = waterflow.get_forced_info()
-            return make_response(json.dumps(forced_data), 200)
-
-    def on_stop(self):
-        """ Event to stop current operation """
-        waterflow = Waterflow()
-
-        if request.method == 'POST':
-            self.logger.info('Stop requested...')
-            waterflow.stop()
-            return "true"
-        else:
-            stop_requested = waterflow.stop_requested()
-            return make_response(json.dumps(stop_requested), 200)
-
-    def on_save(self):
-        """ Event to save the changes in the watering system schedulling
-        Args:
-            data (dict): Information about the required schedulling
-        Returns:
-            bool: If everything went ok
-        """
-        waterflow = Waterflow()
-
-        self.logger.info("Saving programs...")
-        data = json.loads(request.form.get('save'))
-        parsed_config = waterflow.config.get_dict_copy()
-        for program, update in zip(parsed_config['programs'], data):
-            self._change_program(program, update)
-
-        waterflow.update_config(programs=parsed_config['programs'])
-        return "true"
-
-    def _filter_public_config(self, config):
-        del config['influxdbconn']
-        return config
-
-    def _change_program(self, program, new_program):
-        inputbox_text = new_program['time']
-        time1 = datetime.strptime(inputbox_text, '%H:%M')
-        new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
-        program['start_time'] = new_datetime
-        program['valves'][0] = new_program['valves'][0]
-        program['valves'][1] = new_program['valves'][1]
-        program['enabled'] = new_program['enabled']
+""" Webservice to control and manage the piwaterflow loop """
+from datetime import datetime
+import os
+import re
+import json
+from pathlib import Path
+from flask import Flask, render_template, request, make_response
+from flask_compress import Compress
+
+from piwaterflow import Waterflow
+from log_mgr import Logger, LoggerMode
+from revproxy_auth import RevProxyAuth
+
+
+class PiWWWaterflowService:
+    """Class for the web service... its an interface to the real functionality in piwaterflow package.
+    """
+    def __init__(self,  template_folder, static_folder):
+
+        self.logger = Logger(self.class_name(), log_file_name='piwwwaterflow', mode=LoggerMode.BOTH, dry_run=False)
+        self.logger.info("Launching piwwwaterflow...")
+
+        self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
+
+        self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
+
+        self.app.add_url_rule('/', 'waterflow', self.waterflow_endpoint, methods=['GET', 'POST'])
+
+        self.app.add_url_rule('/service', 'service', self.on_service_request, methods=['GET'])
+        self.app.add_url_rule('/force', 'force', self.on_force, methods=['GET', 'POST'])
+        self.app.add_url_rule('/stop', 'stop', self.on_stop, methods=['GET', 'POST'])
+        self.app.add_url_rule('/save', 'save', self.on_save, methods=['POST'])
+
+        Compress(self.app)
+
+    @classmethod
+    def class_name(cls):
+        """ class name """
+        return "piwwwaterflow"
+
+    def get_app(self):
+        """ Returns WSGI app
+        Returns:
+            WSGI app:
+        """
+        return self.app
+
+    def run(self):
+        """ Run function """
+        self.app.run()
+
+    def waterflow_endpoint(self):
+        """ Main endpoint that returns the main page for piwaterflow
+        Returns:
+            response: The main html content
+        """
+        return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
+
+    def on_service_request(self) -> dict:
+        """ Gets all the information from the waterflow service
+        Args:
+            data (dict):'first_time': This value is only bypassed to the caller
+        Returns:
+            dict:Dictionary with all the information about the status of the waterflow system
+        """
+        self.logger.info('Service requested...')
+
+        if not self.revproxy_auth.session_token_valid(request):
+            self.logger.info('Credentials not valid. Expired?.')
+            return make_response("Credentials not valid. Expired?.", 401)
+
+        waterflow = Waterflow()
+
+        try:
+            ver_backend = waterflow.get_version()
+            ver_frontend = self.get_version()
+        except Exception as ex:
+            self.logger.info('Versions could not be found: %s', ex)
+
+            ver_backend = '?.?.?'
+            ver_frontend = '?.?.?'
+
+        responsedict = None
+
+        try:
+            responsedict = {'log': waterflow.get_log(),
+                            'forced': waterflow.get_forced_info(),
+                            'stop': waterflow.stop_requested(),
+                            'config': self._filter_public_config(waterflow.config.get_dict_copy()),
+                            'lastlooptime': waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
+                            'version_backend': ver_backend,
+                            'version_frontend': ver_frontend
+                            }
+            # Change to string so that javascript can manage with it
+            for program in responsedict['config']['programs']:
+                program['start_time'] = program['start_time'].strftime('%H:%M')
+        except Exception as ex:
+            self.logger.error('Error calculating service request: %s', ex)
+            raise RuntimeError(f'Exception on service request: {ex}') from ex
+
+        return make_response(json.dumps(responsedict), 200)
+
+    def on_force(self):
+        """ On force action request
+        Args:
+            data (dict): 'type': Must be 'valve' or 'program'
+                         'value': Must be the index of the program or value to be forced
+        """
+        waterflow = Waterflow()
+
+        if request.method == 'POST':
+            type_force = request.form.get('type')
+            value_force = request.form.get('value')
+            self.logger.info('Force requested: %s = %s', type_force, value_force)
+
+            waterflow.force(type_force, value_force)
+            return make_response('Force scheduled: %s = %s', type_force, value_force, 200)
+        else:
+            forced_data = waterflow.get_forced_info()
+            return make_response(json.dumps(forced_data), 200)
+
+    def on_stop(self):
+        """ Event to stop current operation """
+        waterflow = Waterflow()
+
+        if request.method == 'POST':
+            self.logger.info('Stop requested...')
+            waterflow.stop()
+            return "true"
+        else:
+            stop_requested = waterflow.stop_requested()
+            return make_response(json.dumps(stop_requested), 200)
+
+    def on_save(self):
+        """ Event to save the changes in the watering system schedulling
+        Args:
+            data (dict): Information about the required schedulling
+        Returns:
+            bool: If everything went ok
+        """
+        waterflow = Waterflow()
+
+        self.logger.info("Saving programs...")
+        data = json.loads(request.form.get('save'))
+        parsed_config = waterflow.config.get_dict_copy()
+        for program, update in zip(parsed_config['programs'], data):
+            self._change_program(program, update)
+
+        waterflow.update_config(programs=parsed_config['programs'])
+        return "true"
+
+    def _filter_public_config(self, config):
+        del config['influxdbconn']
+        return config
+
+    def _change_program(self, program, new_program):
+        inputbox_text = new_program['time']
+        time1 = datetime.strptime(inputbox_text, '%H:%M')
+        new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
+        program['start_time'] = new_datetime
+        program['valves'][0] = new_program['valves'][0]
+        program['valves'][1] = new_program['valves'][1]
+        program['enabled'] = new_program['enabled']
+
+    @classmethod
+    def get_version(cls) -> str:
+        """ Gets version string from the init file
+        Returns:
+            str: Version string
+        """
+        version_file = os.path.join(Path(__file__).parent.resolve(), '__init__.py')
+        with open(version_file, 'r',  encoding="utf-8") as initfile_lines:
+            content = initfile_lines.read()
+            version = re.search(r'__version__ = ["|\'](.*?)["|\']', content).group(1)
+            return version
+        raise RuntimeError(f'Unable to find version string in {version_file}.')
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow/wsgi.py` & `piwwwaterflow-1.0.0/piwwwaterflow/wsgi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-""" WSGI entry point """
-from pathlib import Path
-import os
-
-from piwwwaterflow import PiWWWaterflowService
-
-def _create_service():
-    """ Instantiation of the webservice
-    Returns:
-       Webservice class instantiated
-    """
-    templates_path = os.path.join(Path(__file__).parent.resolve(), 'templates')
-    static_path = os.path.join(Path(__file__).parent.resolve(), 'static')
-    return PiWWWaterflowService(template_folder=templates_path, static_folder=static_path)
-
-def create_app():
-    """ Creates a WSGI standard callable function
-    Returns:
-        WSGI app provided by the PiWWWaterflowService/Flask
-    """
-    wtf_service = _create_service()
-    return wtf_service.get_app()
-
-# __main__ used for standalone execution (debugging). For WSGI call, the "wsgi:create_app()" function should be called
-if __name__ == '__main__':
-    service = create_app()
-    service.run()
+""" WSGI entry point """
+from pathlib import Path
+import os
+
+from piwwwaterflow import PiWWWaterflowService
+
+def _create_service():
+    """ Instantiation of the webservice
+    Returns:
+       Webservice class instantiated
+    """
+    templates_path = os.path.join(Path(__file__).parent.resolve(), 'templates')
+    static_path = os.path.join(Path(__file__).parent.resolve(), 'static')
+    return PiWWWaterflowService(template_folder=templates_path, static_folder=static_path)
+
+def create_app():
+    """ Creates a WSGI standard callable function
+    Returns:
+        WSGI app provided by the PiWWWaterflowService/Flask
+    """
+    wtf_service = _create_service()
+    return wtf_service.get_app()
+
+# __main__ used for standalone execution (debugging). For WSGI call, the "wsgi:create_app()" function should be called
+if __name__ == '__main__':
+    service = create_app()
+    service.run(host="0.0.0.0")
```

### Comparing `piwwwaterflow-0.2.2/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-1.0.0/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 piwwwaterflow/webservice.py
 piwwwaterflow/wsgi.py
 piwwwaterflow.egg-info/PKG-INFO
 piwwwaterflow.egg-info/SOURCES.txt
 piwwwaterflow.egg-info/dependency_links.txt
 piwwwaterflow.egg-info/requires.txt
 piwwwaterflow.egg-info/top_level.txt
+piwwwaterflow/__pycache__/__init__.cpython-38.pyc
+piwwwaterflow/__pycache__/webservice.cpython-38.pyc
 piwwwaterflow/static/__init__.py
 piwwwaterflow/static/css/iepngfix.htc
 piwwwaterflow/static/css/view.css
 piwwwaterflow/static/img/blank.gif
 piwwwaterflow/static/img/bottom.png
 piwwwaterflow/static/img/icon-256.png
 piwwwaterflow/static/img/icon-32.png
```

### Comparing `piwwwaterflow-0.2.2/setup.py` & `piwwwaterflow-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-""" Pypi stup """
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="piwwwaterflow",
-    version="0.2.2",
-    author="Ismael Raya",
-    author_email="phornee@gmail.com",
-    description="Raspberry Pi Waterflow resilient system",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Phornee/piwwwaterflow",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Topic :: Home Automation",
-    ],
-    install_requires=[
-        'Flask>=1.1.2',
-        'flask-compress>=1.9.0',
-        'importlib-metadata>=4.5.0',
-        'piwaterflow>=0.6.0',
-        'revproxy_auth>=0.1.7'
-    ],
-    python_requires='>=3.6',
+""" Pypi stup """
+import os
+import re
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+def get_version():
+    """ Gets version string from the init file
+    Returns:
+        str: Version string
+    """
+    version_file = os.path.join('piwwwaterflow', '__init__.py')
+    with open(version_file, 'r',  encoding="utf-8") as initfile_lines:
+        version = re.search(r'__version__ = ["|\'](.*?)["|\']', initfile_lines.read()).group(1)
+        return version
+    raise RuntimeError(f'Unable to find version string in {version_file}.')
+
+setuptools.setup(
+    name="piwwwaterflow",
+    version=get_version(),
+    author="Ismael Raya",
+    author_email="phornee@gmail.com",
+    description="Raspberry Pi Waterflow resilient system",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Phornee/piwwwaterflow",
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Home Automation",
+    ],
+    install_requires=[
+        'Flask>=1.1.2',
+        'flask-compress>=1.9.0',
+        'importlib-metadata>=4.5.0',
+        'piwaterflow>=1.0.0',
+        'revproxy_auth>=0.1.8'
+    ],
+    python_requires='>=3.6',
 )
```

