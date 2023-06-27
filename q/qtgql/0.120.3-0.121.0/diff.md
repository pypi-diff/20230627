# Comparing `tmp/qtgql-0.120.3.tar.gz` & `tmp/qtgql-0.121.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.120.3.tar", max compression
+gzip compressed data, was "qtgql-0.121.0.tar", max compression
```

## Comparing `qtgql-0.120.3.tar` & `qtgql-0.121.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-26 12:54:42.897055 qtgql-0.120.3/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-26 12:54:42.897055 qtgql-0.120.3/README.md
--rw-r--r--   0        0        0     4428 2023-06-26 12:55:02.589106 qtgql-0.120.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4207 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13536 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1527 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     2446 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     5405 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5200 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3482 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16797 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-26 12:54:42.909055 qtgql-0.120.3/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 04:13:28.925691 qtgql-0.121.0/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-27 04:13:28.925691 qtgql-0.121.0/README.md
+-rw-r--r--   0        0        0     4428 2023-06-27 04:13:53.601854 qtgql-0.121.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4175 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13573 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1402 2023-06-27 04:13:28.941691 qtgql-0.121.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     5371 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5200 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3482 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16797 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-27 04:13:28.945691 qtgql-0.121.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.121.0/PKG-INFO
```

### Comparing `qtgql-0.120.3/LICENSE` & `qtgql-0.121.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/README.md` & `qtgql-0.121.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/pyproject.toml` & `qtgql-0.121.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.120.3"
+version = "0.121.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/cli.py` & `qtgql-0.121.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/config.py` & `qtgql-0.121.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/core/cppref.py` & `qtgql-0.121.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.121.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/core/template.py` & `qtgql-0.121.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/generator.py` & `qtgql-0.121.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/operation/definitions.py` & `qtgql-0.121.0/qtgqlcodegen/operation/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     concrete: QtGqlFieldDefinition
     variable_uses: list[QtGqlVariableUse] = attrs.Factory(list)
 
     @cached_property
     def cached_by_args(self) -> bool:
         # if the origin implements node it's fields are cached by arguments
         # if they have ones
-        return bool(self.origin.implements_node and self.concrete.arguments)
+        return bool(self.concrete.arguments)
 
     @cached_property
     def is_root(self) -> bool:
         return self.origin.name in self.type_info.schema_type_info.root_types_names
 
     @cached_property
     def type_name(self) -> str:
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.121.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         var_name = arg.value.name.value  # type: ignore[attr-defined]
         for variable in type_info.variables:
             if var_name == variable.name:
                 ret.append(
                     QtGqlVariableUse(argument=(index, field.arguments[index]), variable=variable),
                 )
     assert len(ret) == len(arguments), "could not find all variable uses"
-    return ret
+    return sorted(ret, key=lambda v: v.argument[0])
 
 
 def _evaluate_variable_node_type(
     type_info: SchemaTypeInfo,
     node: graphql.TypeNode,
 ) -> QtGqlTypeABC:
     if nonnull := is_nonnull_node(node):
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/operation/template.py` & `qtgql-0.121.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/schema/definitions.py` & `qtgql-0.121.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.121.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/schema/template.py` & `qtgql-0.121.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro concrete_type_fields(type) -%}
 public:
 {% for f in type.unique_fields -%}
 {% set f_member_type -%}
-{% if type.implements_node and f.arguments -%}
+{% if f.arguments -%}
 std::map<👉f.arguments_type👈, 👉f.type.member_type👈>
 {% else -%}
 👉f.type.member_type👈
 {% endif -%}
 {%- endset -%}
 👉 f_member_type 👈 👉 f.private_name 👈 = 👉 f.type.default_value 👈;
 {% endfor %}
@@ -14,30 +14,30 @@
 {%for f in type.unique_fields -%}
 void 👉 f.signal_name 👈();
 {% endfor %}
 
 public:
 {%for f in type.unique_fields %}
 [[nodiscard]] const 👉 f.type.fget_type 👈 &👉 f.getter_name 👈(
-{%- if f.arguments and type.implements_node -%}👉 f.arguments_type 👈 args {% endif -%}
+{%- if f.arguments -%}👉 f.arguments_type 👈 args {% endif -%}
 ) {%- if f.type.getter_is_constable -%}const{% endif %}{
-{%- if f.arguments and type.implements_node -%}
+{%- if f.arguments -%}
 {% set f_private_name %}👉 f.private_name 👈.at(args){% endset %}
 {% else -%}
 {% set f_private_name %}👉 f.private_name 👈{% endset %}
 {% endif -%}
 {% if f.is_custom_scalar -%}
 return 👉 f_private_name 👈.to_qt();
 {% else -%}
 return 👉 f_private_name 👈;
 {% endif -%}
 }
-void 👉 f.setter_name 👈(const 👉 f.type.member_type_arg 👈 v {% if f.arguments and type.implements_node %}, 👉 f.arguments_type 👈 args {% endif %})
+void 👉 f.setter_name 👈(const 👉 f.type.member_type_arg 👈 v {% if f.arguments %}, 👉 f.arguments_type 👈 args {% endif %})
 {
-{%- if f.arguments and type.implements_node -%}
+{%- if f.arguments -%}
 {% set f_private_name %}👉 f.private_name 👈[args]{% endset %}
 {% else -%}
 {% set f_private_name %}👉 f.private_name 👈{% endset %}
 {% endif -%}
 👉 f_private_name 👈 = v;
 emit 👉 f.signal_name 👈();
 };
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,71 @@
 {%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
-{% macro update_concrete_field(proxy_field,f_concrete, fset_name, private_name, operation_pointer="operation") -%}
-{% set current -%}
-{% if not proxy_field.is_root and proxy_field.variable_uses  -%}
-inst->👉private_name👈.at(👉proxy_field.build_variables_tuple_for_field_arguments👈)
-{% else -%}
+{% macro update_concrete_field(proxy_field,f_concrete, private_name, operation_pointer="operation") -%}
+{% if proxy_field.variable_uses  -%}
+👉f_concrete.arguments_type👈 👉private_name👈_args = 👉proxy_field.build_variables_tuple_for_field_arguments👈;
+{% endif %}
+{%- set current -%}
+{% if proxy_field.variable_uses  -%}
+inst->👉private_name👈.at(👉private_name👈_args)
+{%- else -%}
 inst->👉private_name👈
-{% endif -%}
+{%- endif -%}
 {%- endset -%}
 {% set setter_end -%}
-{% if not proxy_field.is_root and proxy_field.variable_uses  -%}
-, 👉proxy_field.build_variables_tuple_for_field_arguments👈
+{% if proxy_field.variable_uses -%}
+, 👉private_name👈_args
 {% endif -%}
 {%- endset -%}
+{%- set setter_name -%}inst->👉 proxy_field.concrete.setter_name 👈{% endset -%}
 
+{%- if proxy_field.is_root and f_concrete.type.is_object_type -%}
+{#- // root fields that has no default value might not have value even if they are not optional -#}
+{% if proxy_field.variable_uses  -%}
+if (!inst->👉private_name👈.contains(👉private_name👈_args))
+{% else -%}
+if (!👉current👈)
+{% endif %}
+{
+    👉deserialize_concrete_field(proxy_field, setter_name)👈
+}
+else
+{% endif -%}
 if (!data.value("👉f_concrete.name👈").isNull()){
 {% if proxy_field.type.is_builtin_scalar -%}
 {% if proxy_field.type.is_void -%}
 /* deliberately empty */
 {% else -%}
 auto new_👉f_concrete.name👈 = data.value("👉f_concrete.name👈").👉 proxy_field.type.is_builtin_scalar.from_json_convertor 👈;
 if (👉current👈 != new_👉f_concrete.name👈){
-inst->👉fset_name👈(new_👉f_concrete.name👈 👉 setter_end 👈);
+👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
 {% endif %}
 {% elif proxy_field.type.is_custom_scalar %}
 auto new_👉proxy_field.name👈 = 👉 proxy_field.type.is_custom_scalar.type_name() 👈();
 new_👉proxy_field.name👈.deserialize(data.value("👉f_concrete.name👈"));
 if (👉current👈 != new_👉proxy_field.name👈){
-inst->👉fset_name👈(new_👉f_concrete.name👈 👉 setter_end 👈);
+👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
 {% elif proxy_field.type.is_queried_object_type %}
-{% if f_concrete.implements_node %}
-auto 👉f_concrete.name👈_data = data.value("person").toObject();
-if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
-👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
-}
-else{
-inst->👉fset_name👈(👉proxy_field.type.deserializer_name👈(data.value("👉f_concrete.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
-}
-{% endif %}
+    auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
+    {% if f_concrete.implements_node %}
+    if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
+    👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
+    }
+    else{
+    👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(👉f_concrete.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
+    }
+    {% else %}
+    👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
+    {% endif %}
 {% elif proxy_field.type.is_model %}
-{% set setter %}inst->👉 proxy_field.concrete.setter_name 👈{% endset %}
-👉deserialize_concrete_field(proxy_field, setter)👈
+👉deserialize_concrete_field(proxy_field, setter_name)👈
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
 {% if proxy_field.type.is_optional %}
 else {
-inst->👉fset_name👈({} 👉 setter_end 👈);
+👉 setter_name 👈({} 👉 setter_end 👈);
 }
 {% endif %}
 {%- endmacro %}
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -106,13 +106,13 @@
 };
 {% endif %}
 
 // Updater
 void 👉 t.updater_name 👈(👉 t.concrete.member_type_arg 👈 inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation)
 {
 {%for f in t.fields -%}
-👉update_concrete_field(f,f.concrete, fset_name=f.concrete.setter_name, private_name=f.private_name, operation_pointer="operation")👈
+👉update_concrete_field(f,f.concrete, private_name=f.private_name, operation_pointer="operation")👈
 {% endfor %}
 };
 {% endfor %}
 }
```

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.121.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/types.py` & `qtgql-0.121.0/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/qtgqlcodegen/utils.py` & `qtgql-0.121.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.3/PKG-INFO` & `qtgql-0.121.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.120.3
+Version: 0.121.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

