# Comparing `tmp/starfyre-0.6.1.tar.gz` & `tmp/starfyre-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.6.1.tar", max compression
+gzip compressed data, was "starfyre-0.6.2.tar", max compression
```

## Comparing `starfyre-0.6.1.tar` & `starfyre-0.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3215 2023-06-15 17:49:37.095611 starfyre-0.6.1/README.md
--rw-r--r--   0        0        0      454 2023-06-15 17:49:37.095611 starfyre-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1099 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/__main__.py
--rw-r--r--   0        0        0     4539 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/component.py
--rw-r--r--   0        0        0     4135 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/js/store.js
--rw-r--r--   0        0        0     8837 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/transpiler.py
--rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 starfyre-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4382 2023-06-27 20:12:52.122850 starfyre-0.6.2/README.md
+-rw-r--r--   0        0        0      454 2023-06-27 20:12:52.122850 starfyre-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      949 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/__init__.py
+-rw-r--r--   0        0        0     1637 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/__main__.py
+-rw-r--r--   0        0        0     4539 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/js/store.js
+-rw-r--r--   0        0        0     9071 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-06-27 20:12:52.122850 starfyre-0.6.2/starfyre/transpiler.py
+-rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.6.2/PKG-INFO
```

### Comparing `starfyre-0.6.1/starfyre/__init__.py` & `starfyre-0.6.2/starfyre/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 import inspect
-
 from starfyre.dom_methods import render, render_root
 from .compiler import compile
+
 from starfyre.component import Component
 from .transpiler import transpile
 
-# import js
-
-# for exports
-
-# from .component import Component
-# from .dom_methods import render
 from .parser import RootParser
 
-# from .store import create_signal
-
 
 def create_component(pyml="", css="", js="", client_side_python=""):
     if client_side_python:
         new_js = transpile(client_side_python) + js
         js = new_js
 
     local_variables = inspect.currentframe().f_back.f_back.f_locals.copy()
@@ -32,15 +24,15 @@
 
     if pyml_root is None:
         return Component("div", {}, [], {}, {}, uuid="store", js=js)
 
     return pyml_root
 
 
-# __all__ = [
-#     "render",
-#     "js",
-#     "create_component",
-#     "Component",
-#     "create_signal",
-#     "sum_as_string",
-# ]
+__all__ = [
+    "create_component",
+    "render",
+    "render_root",
+    "compile",
+    "transpile",
+    "Component",
+]
```

### Comparing `starfyre-0.6.1/starfyre/__main__.py` & `starfyre-0.6.2/starfyre/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 def write_js_file(path):
     dist_path = Path(path) / "dist"
     dist_path.mkdir(exist_ok=True)
     js_store = pkg_resources.path("starfyre.js", "store.js")
     shutil.copy(str(js_store), path + "/dist/store.js")
 
 
-
 def create_main_file(path):
     output_file_path = path + "/build/__main__.py"
     write_js_file(path)
 
-
     with open(output_file_path, "w") as f:
         f.write(
             """
 from . import app
 import os
 from pathlib import Path
 
@@ -40,16 +38,16 @@
         f.write(app)
 """
         )
 
 
 @click.command()
 @click.option("--path", default=".", help="Path to the project")
-@click.option("--dev", default=False, help="Run in development mode")
-@click.option("--build", default=False, help="Build the project")
+@click.option("--dev", default=False, help="Start the compilation and generate the build package.")
+@click.option("--build", default=False, help="Start the build package")
 def main(path, dev, build):
     if dev:
         path_ = path + "/__init__.py"
         # get absolute path
         path = os.path.abspath(path_)
         compile(path)
         create_main_file(os.path.dirname(path))
```

### Comparing `starfyre-0.6.1/starfyre/compiler.py` & `starfyre-0.6.2/starfyre/compiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.1/starfyre/component.py` & `starfyre-0.6.2/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.1/starfyre/dom_methods.py` & `starfyre-0.6.2/starfyre/dom_methods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 import re
 from functools import partial
 from uuid import uuid4
 
 from .transpiler import transpile_to_js
 
 
-# # import js
-# from pyodide import create_proxy
-
-
 from .component import Component
 
 
 def assign_event_listeners(event_listener_name, event_listener):
     # component.dom.addEventListener(event_type, create_proxy(event_listener))
     js_event_listener = transpile_to_js(event_listener)
     html = f" {event_listener_name}='{event_listener.__name__}()' "
 
     return html, js_event_listener
 
 
-# there should be two renders
-
-
-# render page and render component
 def render_helper(component: Component) -> tuple[str, str, str]:
     # Add event listeners
     def is_listener(name):
         return name.startswith("on")
 
     def is_attribute(name):
         return not is_listener(name) and name != "children"
 
     parentElement = component.parentComponent
     html = "\n"
     css = "\n"
     js = "\n"
     if parentElement is None:
-        # instead of creating an element with js
-        # we need to create a div string
-
         parentElement = Component("div", {"id": "root"}, [], {}, {}, uuid=uuid4())
         component.parentComponent = parentElement
 
-        # ??
-        # cannot use js
-        # js.document.body.appendChild(parentElement)
-
     tag = component.tag
     props = component.props
     state = component.state
     data = component.data
     event_listeners = component.event_listeners
 
     # Create DOM element
@@ -116,21 +101,14 @@
         css += new_css
         js += new_js
 
     html += f"</{tag}>\n"
 
     component.html = html
     return html, css, js
-    # // Append to parent
-    # need to apply batch updates here
-    # also create a tree of dom nodes in the first place
-    # if parentElement.contains(dom):
-    #     parentElement.replaceChild(dom, parentElement.childNodes[0])
-    # else:
-    #     parentElement.appendChild(dom)
 
 
 def render(component: Component) -> str:
     html, css, js = render_helper(component)
     final_html = f"<style>{css}</style>{html}<script>{js}</script>"
     return final_html
```

### Comparing `starfyre-0.6.1/starfyre/js/store.js` & `starfyre-0.6.2/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.1/starfyre/parser.py` & `starfyre-0.6.2/starfyre/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         if callable(value):
             functions[key] = value
 
     return functions
 
 
 class RootParser(HTMLParser):
+    # this is the grammar for the parser
+    # we need cover all the grammar rules
+
     generic_tags = ["div", "p", "b", "span", "i", "button"]
 
     def __init__(self, component_local_variables, component_global_variables, css, js):
         super().__init__()
         self.stack: list[tuple[Component, int]] = []
         self.children = []
         self.current_depth = 0
@@ -143,19 +146,24 @@
         return signal.replace("()", f"('{uuid}')")
 
     def handle_data(self, data):
         # this is doing too much
         # lexing
         # parsing
 
+
+        # this is a very minimal version of lexing
+        # we should ideally be writing a separate layer for lexing
         data = data.strip().strip("\n").strip(" ")
         # regex to find all the elements that are wrapped in {}
 
         matches = re.findall(r"{(.*?)}", data)
 
+
+        # parsing starts here
         state = {}
 
         parent_node, parent_depth = self.stack[-1]
         uuid = uuid4()
         component_signal = ""
 
         for match in matches:
```

### Comparing `starfyre-0.6.1/starfyre/transpiler.py` & `starfyre-0.6.2/starfyre/transpiler.py`

 * *Files identical despite different names*

