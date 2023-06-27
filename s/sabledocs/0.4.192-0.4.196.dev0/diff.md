# Comparing `tmp/sabledocs-0.4.192.tar.gz` & `tmp/sabledocs-0.4.196.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.4.192.tar", last modified: Tue Jun 27 20:50:43 2023, max compression
+gzip compressed data, was "sabledocs-0.4.196.dev0.tar", last modified: Tue Jun 27 21:34:04 2023, max compression
```

## Comparing `sabledocs-0.4.192.tar` & `sabledocs-0.4.196.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.459345 sabledocs-0.4.192/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-27 20:50:29.000000 sabledocs-0.4.192/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-27 20:50:29.000000 sabledocs-0.4.192/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-27 20:50:43.459345 sabledocs-0.4.192/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-27 20:50:29.000000 sabledocs-0.4.192/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-27 20:50:29.000000 sabledocs-0.4.192/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-06-27 20:50:43.459345 sabledocs-0.4.192/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.455345 sabledocs-0.4.192/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.455345 sabledocs-0.4.192/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.455345 sabledocs-0.4.192/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.459345 sabledocs-0.4.192/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.459345 sabledocs-0.4.192/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   261000 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-27 20:50:29.000000 sabledocs-0.4.192/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 20:50:43.455345 sabledocs-0.4.192/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-27 20:50:43.000000 sabledocs-0.4.192/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.852557 sabledocs-0.4.196.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-27 21:34:04.852557 sabledocs-0.4.196.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-27 21:34:04.852557 sabledocs-0.4.196.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.848556 sabledocs-0.4.196.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.848556 sabledocs-0.4.196.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.848556 sabledocs-0.4.196.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.852557 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5751 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.852557 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   261187 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-27 21:33:41.000000 sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:34:04.848556 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-27 21:34:04.000000 sabledocs-0.4.196.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.4.192/LICENSE` & `sabledocs-0.4.196.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/PKG-INFO` & `sabledocs-0.4.196.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.192
+Version: 0.4.196.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.192/README.md` & `sabledocs-0.4.196.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/pyproject.toml` & `sabledocs-0.4.196.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/__main__.py` & `sabledocs-0.4.196.dev0/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/lunr_search.py` & `sabledocs-0.4.196.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.4.196.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/proto_model.py` & `sabledocs-0.4.196.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/sable_config.py` & `sabledocs-0.4.196.dev0/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/base.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,22 @@
           const setPreference = () => {
             localStorage.setItem(storageKey, theme.value)
             reflectPreference()
           }
 
           const reflectPreference = () => {
             const body = document.querySelector('body');
+            const html = document.querySelector('html'); // The html element is also configured to make sure the background color is correct on mobile if the content overflows horizontally.
+
             if (theme.value === 'dark') {
                 body.className = 'dark';
+                html.className = 'dark';
             } else {
                 body.className = '';
+                html.className = '';
             }
 
             document.firstElementChild
               .setAttribute('data-theme', theme.value)
 
             document
               .querySelector('#theme-toggle')
@@ -85,54 +89,54 @@
               {{ sable_config.module_title }}
             </a>
           </p>
         </div>
 
         <div class="level-right">
           {% if sable_config.enable_lunr_search  %}
-          <form action="search.html" class="mr-2">
+          <form action="search.html" class="mr-2 has-text-centered">
             <input type="text" name="query" class="input mr-3 navbar-search-query-input" placeholder="Search">
             <input type="submit" class="button is-primary mr-5" value="Search" />
           </form>
           {% endif %}
 
-          <p class="level-item has-text-centered is-size-5 mr-5">
-            <a href="{{ sable_config.repository_url }}" class="link is-info" target="_blank">
+          <p class="level-item has-text-centered is-size-5">
+            <a href="{{ sable_config.repository_url }}" class="link is-info mr-5" target="_blank">
               {% if sable_config.repository_type | string == "RepositoryType.GITHUB" %}
               <span class="icon">
                 <i class="fa-brands fa-github"></i>
               </span>
               {% elif sable_config.repository_type | string == "RepositoryType.BITBUCKET" %}
               <span class="icon">
                 <i class="fa-brands fa-bitbucket"></i>
               </span>
               {% endif %}
               <span>Source</span>
             </a>
-          </p>
 
-          <button class="theme-toggle" id="theme-toggle" title="Toggles light & dark" aria-label="auto" aria-live="polite">
-            <svg class="sun-and-moon" aria-hidden="true" width="24" height="24" viewBox="0 0 24 24">
-              <mask class="moon" id="moon-mask">
-                <rect x="0" y="0" width="100%" height="100%" fill="white" />
-                <circle cx="24" cy="10" r="6" fill="black" />
-              </mask>
-              <circle class="sun" cx="12" cy="12" r="6" mask="url(#moon-mask)" fill="currentColor" />
-              <g class="sun-beams" stroke="currentColor">
-                <line x1="12" y1="1" x2="12" y2="3" />
-                <line x1="12" y1="21" x2="12" y2="23" />
-                <line x1="4.22" y1="4.22" x2="5.64" y2="5.64" />
-                <line x1="18.36" y1="18.36" x2="19.78" y2="19.78" />
-                <line x1="1" y1="12" x2="3" y2="12" />
-                <line x1="21" y1="12" x2="23" y2="12" />
-                <line x1="4.22" y1="19.78" x2="5.64" y2="18.36" />
-                <line x1="18.36" y1="5.64" x2="19.78" y2="4.22" />
-              </g>
-            </svg>
-          </button>
+            <button class="theme-toggle" id="theme-toggle" title="Toggles light & dark" aria-label="auto" aria-live="polite" type="button">
+              <svg class="sun-and-moon" aria-hidden="true" width="24" height="24" viewBox="0 0 24 24">
+                <mask class="moon" id="moon-mask">
+                  <rect x="0" y="0" width="100%" height="100%" fill="white" />
+                  <circle cx="24" cy="10" r="6" fill="black" />
+                </mask>
+                <circle class="sun" cx="12" cy="12" r="6" mask="url(#moon-mask)" fill="currentColor" />
+                <g class="sun-beams" stroke="currentColor">
+                  <line x1="12" y1="1" x2="12" y2="3" />
+                  <line x1="12" y1="21" x2="12" y2="23" />
+                  <line x1="4.22" y1="4.22" x2="5.64" y2="5.64" />
+                  <line x1="18.36" y1="18.36" x2="19.78" y2="19.78" />
+                  <line x1="1" y1="12" x2="3" y2="12" />
+                  <line x1="21" y1="12" x2="23" y2="12" />
+                  <line x1="4.22" y1="19.78" x2="5.64" y2="18.36" />
+                  <line x1="18.36" y1="5.64" x2="19.78" y2="4.22" />
+                </g>
+              </svg>
+            </button>
+          </p>
         </div>
       </nav>
     </div>
 
     <div class="container mb-6">{% block content %}{% endblock %}</div>
 
     <footer class="footer">
```

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/index.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/message.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/package.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/search.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/service.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files 0% similar despite different names*

```diff
@@ -7903,21 +7903,30 @@
   border-width: 0 0 0.06em 0;
   border-style: solid;
   border-color: #DDDDDD; }
 
 .navbar-search-query-input {
   width: 13em; }
 
+@media screen and (max-width: 768px) {
+  .level-right .level-item {
+    margin-top: 0.8em; } }
+
 body {
-  min-height: 100vh; }
+  min-height: 100vh;
+  padding-left: 0.7em;
+  padding-right: 0.7em; }
 
 body .subtitle,
 body .title {
   color: #181818; }
 
+html.dark {
+  background-color: #181818; }
+
 body.dark,
 body.dark .box,
 body.dark table {
   background-color: #181818;
   color: whitesmoke; }
 
 body.dark th {
```

### Comparing `sabledocs-0.4.192/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.4.196.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.192/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.4.196.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.192
+Version: 0.4.196.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.192/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.4.196.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

