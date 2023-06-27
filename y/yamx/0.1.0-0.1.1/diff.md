# Comparing `tmp/yamx-0.1.0.tar.gz` & `tmp/yamx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamx-0.1.0.tar", max compression
+gzip compressed data, was "yamx-0.1.1.tar", max compression
```

## Comparing `yamx-0.1.0.tar` & `yamx-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.0/LICENSE
--rw-r--r--   0        0        0     1724 2023-05-05 14:44:31.630904 yamx-0.1.0/README.md
--rw-r--r--   0        0        0     1063 2023-05-05 14:44:31.631324 yamx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-05 14:44:31.634964 yamx-0.1.0/yamx/__init__.py
--rw-r--r--   0        0        0     1066 2023-05-05 14:44:31.635428 yamx-0.1.0/yamx/constants.py
--rw-r--r--   0        0        0      398 2023-05-05 14:44:31.635822 yamx-0.1.0/yamx/containers/__init__.py
--rw-r--r--   0        0        0     6899 2023-05-05 14:44:31.636159 yamx-0.1.0/yamx/containers/data.py
--rw-r--r--   0        0        0      105 2023-05-05 14:44:31.636361 yamx-0.1.0/yamx/containers/settings.py
--rw-r--r--   0        0        0     1532 2023-05-05 14:44:31.636595 yamx-0.1.0/yamx/extra.py
--rw-r--r--   0        0        0        0 2023-05-05 14:44:31.636670 yamx-0.1.0/yamx/jinja/__init__.py
--rw-r--r--   0        0        0     4474 2023-05-05 14:44:31.637147 yamx-0.1.0/yamx/jinja/condition.py
--rw-r--r--   0        0        0      169 2023-05-05 14:44:31.637522 yamx-0.1.0/yamx/loader/__init__.py
--rw-r--r--   0        0        0     3725 2023-05-05 14:44:31.637743 yamx-0.1.0/yamx/loader/grouper.py
--rw-r--r--   0        0        0     6208 2023-05-05 14:44:31.638079 yamx-0.1.0/yamx/loader/preprocessor.py
--rw-r--r--   0        0        0      637 2023-05-05 14:44:31.638426 yamx-0.1.0/yamx/loader/utils.py
--rw-r--r--   0        0        0      518 2023-05-05 14:44:31.639003 yamx-0.1.0/yamx/loader/validator.py
--rw-r--r--   0        0        0      244 2023-05-05 14:44:31.639417 yamx-0.1.0/yamx/representer/__init__.py
--rw-r--r--   0        0        0     9448 2023-05-05 14:44:31.639716 yamx-0.1.0/yamx/representer/common.py
--rw-r--r--   0        0        0      611 2023-05-05 14:44:31.639950 yamx-0.1.0/yamx/representer/conditional_map.py
--rw-r--r--   0        0        0      580 2023-05-05 14:44:31.640531 yamx-0.1.0/yamx/representer/conditional_seq.py
--rw-r--r--   0        0        0    18945 2023-05-05 14:44:31.641029 yamx-0.1.0/yamx/representer/rendering.py
--rw-r--r--   0        0        0     6283 2023-05-05 14:44:31.641413 yamx-0.1.0/yamx/yamx.py
--rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 yamx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1724 2023-06-27 08:17:29.427389 yamx-0.1.1/README.md
+-rw-r--r--   0        0        0     1063 2023-06-27 08:57:51.601654 yamx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-27 08:17:29.430991 yamx-0.1.1/yamx/__init__.py
+-rw-r--r--   0        0        0     1065 2023-06-27 08:34:55.316759 yamx-0.1.1/yamx/constants.py
+-rw-r--r--   0        0        0      398 2023-06-27 08:17:29.431599 yamx-0.1.1/yamx/containers/__init__.py
+-rw-r--r--   0        0        0     6993 2023-06-27 08:39:18.867870 yamx-0.1.1/yamx/containers/data.py
+-rw-r--r--   0        0        0      105 2023-06-27 08:17:29.432156 yamx-0.1.1/yamx/containers/settings.py
+-rw-r--r--   0        0        0     1532 2023-06-27 08:17:29.432409 yamx-0.1.1/yamx/extra.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:17:29.432483 yamx-0.1.1/yamx/jinja/__init__.py
+-rw-r--r--   0        0        0     4474 2023-06-27 08:17:29.432958 yamx-0.1.1/yamx/jinja/condition.py
+-rw-r--r--   0        0        0      169 2023-06-27 08:17:29.433219 yamx-0.1.1/yamx/loader/__init__.py
+-rw-r--r--   0        0        0     3725 2023-06-27 08:17:29.433444 yamx-0.1.1/yamx/loader/grouper.py
+-rw-r--r--   0        0        0     6253 2023-06-27 08:39:18.879819 yamx-0.1.1/yamx/loader/preprocessor.py
+-rw-r--r--   0        0        0      637 2023-06-27 08:17:29.433836 yamx-0.1.1/yamx/loader/utils.py
+-rw-r--r--   0        0        0      518 2023-06-27 08:17:29.434122 yamx-0.1.1/yamx/loader/validator.py
+-rw-r--r--   0        0        0      244 2023-06-27 08:17:29.434292 yamx-0.1.1/yamx/representer/__init__.py
+-rw-r--r--   0        0        0     9448 2023-06-27 08:17:29.434469 yamx-0.1.1/yamx/representer/common.py
+-rw-r--r--   0        0        0      611 2023-06-27 08:17:29.434619 yamx-0.1.1/yamx/representer/conditional_map.py
+-rw-r--r--   0        0        0      580 2023-06-27 08:17:29.434741 yamx-0.1.1/yamx/representer/conditional_seq.py
+-rw-r--r--   0        0        0    18945 2023-06-27 08:17:29.435048 yamx-0.1.1/yamx/representer/rendering.py
+-rw-r--r--   0        0        0     6271 2023-06-27 08:52:12.176499 yamx-0.1.1/yamx/yamx.py
+-rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 yamx-0.1.1/PKG-INFO
```

### Comparing `yamx-0.1.0/LICENSE` & `yamx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/README.md` & `yamx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/pyproject.toml` & `yamx-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamx"
-version = "0.1.0"
+version = "0.1.1"
 description = "YAML parser that supports jinja conditional expressions"
 
 license = "Apache-2.0"
 
 authors = [
     "Eduard Trott <eduard.trott@workday.com>"
 ]
@@ -21,15 +21,15 @@
 # Compatible Python versions
 python = ">=3.8"
 
 # Standard dependencies with semver constraints
 attrs = "^22.2.0"
 jinja2 = "^3.1.2"
 immutables= "^0.19"
-"ruamel.yaml" = "0.17.21"
+"ruamel.yaml" = "0.17.32"
 "ruamel.yaml.string" = "0.1.0"
 
 
 [tool.poetry.group.test]
 optional = true
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
```

### Comparing `yamx-0.1.0/yamx/constants.py` & `yamx-0.1.1/yamx/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 ELSE_COMMENT: Final[str] = "{% else %}"
 ENDIF_COMMENT: Final[str] = "{% endif %}"
 
 # conditional structure key constants
 CONDITIONAL_KEY_PREFIX: Final[str] = "__condition__"
 
 # conditional structure tag constants
-CONDITIONAL_TAG: Final[str] = "!conditional"
+CONDITIONAL_TAG: Final[str] = "conditional"
 
 # conditional key deduplication
 DEDUPLICATOR: Final[str] = "__deduplicator__"
 DEDUPLICATOR_UPD: Final[str] = "__deduplicator_upd__"
```

### Comparing `yamx-0.1.0/yamx/containers/data.py` & `yamx-0.1.1/yamx/containers/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, ClassVar, Optional, Tuple, Union
 
 from attr import evolve, frozen
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
+from ruamel.yaml.tag import Tag
 
 from yamx.constants import (
     CONDITIONAL_TAG,
     DEDUPLICATOR_UPD,
     YAML_MAP_TAG,
     YAML_SEQ_TAG,
     ConditionalBlockType,
@@ -55,20 +56,22 @@
         else:
             self._data[key] = value
 
 
 class ConditionalMap(CommentedMap):
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
-        self.yaml_set_tag(YAML_MAP_TAG)
+        tag = Tag(suffix=YAML_MAP_TAG)
+        self.yaml_set_ctag(tag)
 
 
 class ConditionalSeq(CommentedSeq):
     def __init__(self, *args, **kw) -> None:
-        self.yaml_set_tag(YAML_SEQ_TAG)
+        tag = Tag(suffix=YAML_SEQ_TAG)
+        self.yaml_set_ctag(tag)
         super().__init__(*args, **kw)
 
 
 @frozen
 class ConditionalBlock:
     yaml_tag: ClassVar[str] = CONDITIONAL_TAG
```

### Comparing `yamx-0.1.0/yamx/extra.py` & `yamx-0.1.1/yamx/extra.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/jinja/condition.py` & `yamx-0.1.1/yamx/jinja/condition.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/loader/grouper.py` & `yamx-0.1.1/yamx/loader/grouper.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/loader/preprocessor.py` & `yamx-0.1.1/yamx/loader/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import io
 from typing import Dict, List, Optional, Union
 
 from jinja2 import nodes
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
+from ruamel.yaml.tag import Tag
 
 from yamx.constants import CONDITIONAL_KEY_PREFIX, CONDITIONAL_TAG, ConditionalBlockType
 from yamx.containers.data import Condition
 from yamx.jinja.condition import extract_condition
 from yamx.loader.utils import get_jinja_env
 
 UNIQUE_CONDITION_CNT: int = 0
@@ -160,15 +161,15 @@
     data = CommentedMap(
         {
             "data": yaml_data,
             "typ": typ.value,
             "condition": condition and condition.raw_value,
         }
     )
-    data.yaml_set_tag(CONDITIONAL_TAG)
+    data.yaml_set_ctag(Tag(suffix=CONDITIONAL_TAG))
 
     res_yaml_data: Union[Dict[str, CommentedMap], List[CommentedMap]]
     if isinstance(yaml_data, CommentedMap):
         # create unique key to separate conditional block from other fields
         key = f"{CONDITIONAL_KEY_PREFIX}{UNIQUE_CONDITION_CNT}"
         UNIQUE_CONDITION_CNT += 1
         # abstraction level has to be created in order to encapsulate conditioned fields
```

### Comparing `yamx-0.1.0/yamx/loader/utils.py` & `yamx-0.1.1/yamx/loader/utils.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/loader/validator.py` & `yamx-0.1.1/yamx/loader/validator.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/representer/common.py` & `yamx-0.1.1/yamx/representer/common.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/representer/conditional_map.py` & `yamx-0.1.1/yamx/representer/conditional_map.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/representer/conditional_seq.py` & `yamx-0.1.1/yamx/representer/conditional_seq.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/representer/rendering.py` & `yamx-0.1.1/yamx/representer/rendering.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.0/yamx/yamx.py` & `yamx-0.1.1/yamx/yamx.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         return ConditionalData(grouped_data)
 
     def dump(self, data: ConditionalData, stream) -> None:
         self.yaml.dump(
             data._data, stream, transform=self._remove_field_names_deduplicator
         )
 
-    def resolve(self, data: ConditionalData, context: Dict[str, Any]) -> Any:
+    def resolve(self, data: str, context: Dict[str, Any]) -> Any:
         env = get_jinja_env()
         try:
             ast = env.parse(data)
         except Exception as e:
             raise Exception("Failed to parse jinja syntax while resolving.") from e
 
         missing_variables = meta.find_undeclared_variables(ast) - set(context.keys())
```

### Comparing `yamx-0.1.0/PKG-INFO` & `yamx-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamx
-Version: 0.1.0
+Version: 0.1.1
 Summary: YAML parser that supports jinja conditional expressions
 Home-page: https://github.com/maybelinot/yamx
 License: Apache-2.0
 Keywords: yaml,jinja,language
 Author: Eduard Trott
 Author-email: eduard.trott@workday.com
 Requires-Python: >=3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: immutables (>=0.19,<0.20)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: ruamel.yaml (==0.17.21)
+Requires-Dist: ruamel.yaml (==0.17.32)
 Requires-Dist: ruamel.yaml.string (==0.1.0)
 Project-URL: Repository, https://github.com/maybelinot/yamx
 Description-Content-Type: text/markdown
 
 
 
 # YAMX
```

