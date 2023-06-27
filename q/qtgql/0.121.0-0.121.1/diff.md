# Comparing `tmp/qtgql-0.121.0.tar.gz` & `tmp/qtgql-0.121.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.121.0.tar", max compression
+gzip compressed data, was "qtgql-0.121.1.tar", max compression
```

## Comparing `qtgql-0.121.0.tar` & `qtgql-0.121.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-27 04:13:28.925691 qtgql-0.121.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-27 04:13:28.925691 qtgql-0.121.0/README.md
--rw-r--r--   0        0        0     4428 2023-06-27 04:13:53.601854 qtgql-0.121.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4175 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13573 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1402 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     5371 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5200 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3482 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16797 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.121.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 07:14:40.039490 qtgql-0.121.1/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-27 07:14:40.039490 qtgql-0.121.1/README.md
+-rw-r--r--   0        0        0     4428 2023-06-27 07:15:07.385308 qtgql-0.121.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4175 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13573 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1402 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     3367 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     5371 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5200 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3482 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16797 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.121.1/PKG-INFO
```

### Comparing `qtgql-0.121.0/LICENSE` & `qtgql-0.121.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/README.md` & `qtgql-0.121.1/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/pyproject.toml` & `qtgql-0.121.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.121.0"
+version = "0.121.1"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.121.0/qtgqlcodegen/cli.py` & `qtgql-0.121.1/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/config.py` & `qtgql-0.121.1/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.121.1/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.121.1/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/core/template.py` & `qtgql-0.121.1/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/generator.py` & `qtgql-0.121.1/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.121.1/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.121.1/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/operation/template.py` & `qtgql-0.121.1/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.121.1/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.121.1/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/schema/template.py` & `qtgql-0.121.1/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(👉f_concrete.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
     }
     {% else %}
     👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
     {% endif %}
 {% elif proxy_field.type.is_model %}
 👉deserialize_concrete_field(proxy_field, setter_name)👈
+{% elif proxy_field.type.is_enum %}
+auto new_👉f_concrete.name👈= Enums::👉proxy_field.type.is_enum.map_name👈::by_name(data.value("👉proxy_field.name👈").toString());
+if (👉current👈 != new_👉f_concrete.name👈){
+👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
+}
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
 {% if proxy_field.type.is_optional %}
 else {
 👉 setter_name 👈({} 👉 setter_end 👈);
```

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.121.1/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/types.py` & `qtgql-0.121.1/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/qtgqlcodegen/utils.py` & `qtgql-0.121.1/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.0/PKG-INFO` & `qtgql-0.121.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.121.0
+Version: 0.121.1
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

