# Comparing `tmp/qtgql-0.121.1.tar.gz` & `tmp/qtgql-0.122.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.121.1.tar", max compression
+gzip compressed data, was "qtgql-0.122.0.tar", max compression
```

## Comparing `qtgql-0.121.1.tar` & `qtgql-0.122.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-27 07:14:40.039490 qtgql-0.121.1/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-27 07:14:40.039490 qtgql-0.121.1/README.md
--rw-r--r--   0        0        0     4428 2023-06-27 07:15:07.385308 qtgql-0.121.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4175 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13573 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-27 07:14:40.051491 qtgql-0.121.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1402 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     3367 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     5371 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5200 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3482 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16797 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-27 07:14:40.055491 qtgql-0.121.1/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.121.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 12:33:59.107303 qtgql-0.122.0/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-27 12:33:59.107303 qtgql-0.122.0/README.md
+-rw-r--r--   0        0        0     4428 2023-06-27 12:34:16.175650 qtgql-0.122.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4175 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13573 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1395 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     3367 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     5371 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5200 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3480 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16819 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.122.0/PKG-INFO
```

### Comparing `qtgql-0.121.1/LICENSE` & `qtgql-0.122.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/README.md` & `qtgql-0.122.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/pyproject.toml` & `qtgql-0.122.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.121.1"
+version = "0.122.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.121.1/qtgqlcodegen/cli.py` & `qtgql-0.122.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/config.py` & `qtgql-0.122.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/core/cppref.py` & `qtgql-0.122.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.122.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/core/template.py` & `qtgql-0.122.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/generator.py` & `qtgql-0.122.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/operation/definitions.py` & `qtgql-0.122.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.122.0/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/operation/template.py` & `qtgql-0.122.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/schema/definitions.py` & `qtgql-0.122.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.122.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/schema/template.py` & `qtgql-0.122.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 {% endif -%}
 {% if f.is_custom_scalar -%}
 return 👉 f_private_name 👈.to_qt();
 {% else -%}
 return 👉 f_private_name 👈;
 {% endif -%}
 }
-void 👉 f.setter_name 👈(const 👉 f.type.member_type_arg 👈 v {% if f.arguments %}, 👉 f.arguments_type 👈 args {% endif %})
+void 👉 f.setter_name 👈(👉 f.type.member_type_arg 👈 v{% if f.arguments %}, 👉 f.arguments_type 👈 args {% endif %})
 {
 {%- if f.arguments -%}
 {% set f_private_name %}👉 f.private_name 👈[args]{% endset %}
 {% else -%}
 {% set f_private_name %}👉 f.private_name 👈{% endset %}
 {% endif -%}
 👉 f_private_name 👈 = v;
```

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.122.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,46 @@
     GraphQLEnum_MACRO(👉enum.name👈)
 };
 
 {% endfor %}
 };
 {% endif %}
 
+// ---------- INPUT OBJECTS ----------
+{% for type in context.input_objects -%}
+/*
+ * 👉 type.docstring 👈
+ */
+struct 👉type.name👈{
+
+public:
+{# // this is doubtfully needed, but std::map requires comparison for ordering. #}
+bool operator<(const 👉type.name👈& other) const {
+    {% for f in type.fields -%}
+    if(👉f.name👈 < other.👉f.name👈){
+        return true;
+    }
+    {% endfor -%}
+    return false;
+}
+{% for f in type.fields -%}
+std::optional<👉f.type.member_type👈> 👉f.name👈 = {};
+{% endfor %}
+[[nodiscard]] QJsonObject to_json() const{
+    auto ret = QJsonObject();
+    {% for f in type.fields %}{% set attr_name %}👉f.name👈{% endset %}
+    if (👉attr_name👈.has_value()){
+        ret.insert("👉f.name👈", 👉f.json_repr(attr_name)👈);
+    }
+    {% endfor %}
+    return ret;
+}
+};
+{% endfor %}
+
 // ---------- Interfaces ----------
 {% for interface in context.interfaces -%}
 class 👉 interface.name 👈 {% for base in interface.bases %} {%if loop.first %}: {% endif %} public 👉 base.name 👈 {% if not loop.last %}, {% endif %}{% endfor %}{
 Q_OBJECT
 
 👉 concrete_type_fields(interface) 👈
 
@@ -53,15 +85,16 @@
         return cache;
 }
 {% endif %}
 };
 {% endfor %}
 
 // ---------- Object Types ----------
-{% for type in context.types -%} {# forward references -#}
+{# forward references -#}
+{% for type in context.types -%}
 class 👉 type.name 👈;
 {% endfor %}
 
 {% for type in context.types %}
 {%- set base_class -%}{% if type. implements_node %}NodeInterfaceABC{% else %}ObjectTypeABC{% endif %}{%- endset -%}
 class 👉 type.name 👈 {% for base in type.bases %}{%if loop.first%}: {% endif %} public 👉 base.name 👈 {% if not loop.last %}, {% endif %}{% endfor %}{
 Q_OBJECT
@@ -88,38 +121,8 @@
     }
     return {};
 }
 {% endif %}
 };
 {% endfor %}
 
-// ---------- INPUT OBJECTS ----------
-
-{% for type in context.input_objects %}
-/*
- * 👉 type.docstring 👈
- */
-struct 👉type.name👈: QObject{
-Q_OBJECT
-
-public:
-{% for f in type.fields %}
-std::optional<👉f.type.member_type👈> 👉f.name👈 = {};
-{% endfor -%}
-👉type.name👈(QObject* parent, {% for f in type.fields %} std::optional<👉f.type.member_type👈> &👉f.name👈{% if not loop.last %},{% endif %} {% endfor %}): QObject::QObject(parent){
-    {% for f in type.fields -%}
-    👉f.name👈 = 👉f.name👈;
-    {% endfor %}
-};
-QJsonObject to_json() const{
-    auto ret = QJsonObject();
-    {% for f in type.fields %}{% set attr_name %}👉f.name👈{% endset %}
-    if (👉attr_name👈.has_value()){
-    ret.insert("👉f.name👈", 👉f.json_repr(attr_name)👈);
-    }
-    {% endfor %}
-    return ret;
-}
-};
-{% endfor %}
-
 }
```

### Comparing `qtgql-0.121.1/qtgqlcodegen/types.py` & `qtgql-0.122.0/qtgqlcodegen/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     @property
     def member_type_arg(self) -> str:
         """
 
         :return: The C++ member_type if it was passed in argument to somewhere.
         """
-        return self.member_type
+        return f"const {self.member_type} &"
 
     @property
     def fget_type(self) -> str:
         """
 
         :return: type for the proxy object, usually this would be the member type though for custom scalars
         there is `to_qt` that has different type.
@@ -312,16 +312,17 @@
     def member_type(self) -> str:
         if self.is_root:
             return self.type_name()  # root types are singletons
         return f"std::shared_ptr<{self.type_name()}>"
 
     @property
     def member_type_arg(self) -> str:
-        pointer_type = "*" if self.is_root else "&"
-        return f"{self.member_type} {pointer_type}"
+        if self.is_root:
+            return f"{self.member_type} *"
+        return f"const {self.member_type} &"
 
     def __attrs_post_init__(self):
         # inject this object type to the interface.
         # later the interface would use this list to know who he might resolve to.
         for base in self.interfaces_raw:
             if not base.implementations.get(self.name):
                 base.implementations[self.name] = self
```

### Comparing `qtgql-0.121.1/qtgqlcodegen/utils.py` & `qtgql-0.122.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.121.1/PKG-INFO` & `qtgql-0.122.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.121.1
+Version: 0.122.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

