# Comparing `tmp/telebot_components-0.8.3.tar.gz` & `tmp/telebot_components-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.3.tar", max compression
+gzip compressed data, was "telebot_components-0.8.4.tar", max compression
```

## Comparing `telebot_components-0.8.3.tar` & `telebot_components-0.8.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-04-24 09:52:01.104767 telebot_components-0.8.3/LICENSE
--rw-r--r--   0        0        0     2258 2023-04-24 09:52:01.104767 telebot_components-0.8.3/README.md
--rw-r--r--   0        0        0     1573 2023-04-24 09:52:51.494265 telebot_components-0.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.108767 telebot_components-0.8.3/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-04-24 09:52:01.108767 telebot_components-0.8.3/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-04-24 09:52:01.108767 telebot_components-0.8.3/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-04-24 09:52:01.108767 telebot_components-0.8.3/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.108767 telebot_components-0.8.3/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/constants/times.py
--rw-r--r--   0        0        0    50254 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8255 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    29347 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/field.py
--rw-r--r--   0        0        0    14757 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    11976 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9306 2023-04-24 09:52:01.112768 telebot_components-0.8.3/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8066 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8134 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5136 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-04-24 09:52:01.116768 telebot_components-0.8.3/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-27 09:35:12.676991 telebot_components-0.8.4/LICENSE
+-rw-r--r--   0        0        0     2258 2023-06-27 09:35:12.676991 telebot_components-0.8.4/README.md
+-rw-r--r--   0        0        0     1619 2023-06-27 09:35:28.941136 telebot_components-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    50254 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8255 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.676991 telebot_components-0.8.4/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    31714 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/field.py
+-rw-r--r--   0        0        0    18987 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    11976 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9342 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8298 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8134 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5136 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-06-27 09:35:12.680991 telebot_components-0.8.4/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.4/PKG-INFO
```

### Comparing `telebot_components-0.8.3/LICENSE` & `telebot_components-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/README.md` & `telebot_components-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/pyproject.toml` & `telebot_components-0.8.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.3"
+version = "0.8.4"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
+
 [tool.poetry.group.dev.dependencies]
 pyproject-flake8 = "^6.0.0.post1"
 coverage = "^7.2.3"
 
-
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = true
 style="semver"
 
 [tool.poetry.dependencies]
@@ -42,16 +42,16 @@
 black = "^22.3.0"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
 mypy = "^0.960"
 
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = 'black'
```

### Comparing `telebot_components-0.8.3/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.4/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.4/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/constants/emoji.py` & `telebot_components-0.8.4/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/feedback/__init__.py` & `telebot_components-0.8.4/telebot_components/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.4/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.4/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.4/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.4/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/form/field.py` & `telebot_components-0.8.4/telebot_components/form/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
 import copy
+import dataclasses
 import datetime
 import logging
 from dataclasses import dataclass
 from dataclasses import field as dataclass_field
 from dataclasses import fields as dataclass_fields
 from datetime import date, time, tzinfo
 from enum import Enum
 from hashlib import md5
 from typing import (
+    Any,
     Callable,
     ClassVar,
     Dict,
     Generic,
     Optional,
     Type,
     TypeVar,
@@ -32,14 +34,15 @@
     calendar_keyboard,
 )
 from telebot_components.stores.language import (
     AnyText,
     Language,
     MaybeLanguage,
     any_text_to_str,
+    is_any_text,
 )
 
 logger = logging.getLogger(__name__)
 
 FieldValueT = TypeVar("FieldValueT")
 
 
@@ -86,32 +89,65 @@
 
     @classmethod
     def form_end(cls) -> "NextFieldGetter":
         return NextFieldGetter(lambda u, v: None, possible_next_field_names=[None])
 
 
 @dataclass
+class FormFieldResultFormattingOpts(Generic[FieldValueT]):
+    """Options specifying how to format field's result to HTML (e.g. telegram message)"""
+
+    descr: str  # used for telegram message formatting
+    is_multiline: bool = False
+    value_formatter: Optional[
+        Callable[[FieldValueT, MaybeLanguage], str]
+    ] = None  # if not specified, field's default formatter is used
+
+
+@dataclass
+class FormFieldResultExportOpts(Generic[FieldValueT]):
+    """Options specifying how to format field's result to generic record"""
+
+    column: Any  # usually an enum specifying airtable or Google Sheets column
+
+    value_mapping: Optional[dict[FieldValueT, Any]] = None
+    unmapped_value_default: Optional[Any] = None
+
+    value_processor: Optional[Callable[[FieldValueT], Any]] = None
+
+    def __post_init__(self) -> None:
+        if (self.value_mapping is not None) and (self.value_processor is not None):
+            raise ValueError("Value mapping and value processor are mutually exclusive")
+
+
+@dataclass
 class MessageProcessingResult(Generic[FieldValueT]):
     response_to_user: Optional[str]
     parsed_value: Optional[FieldValueT]
     no_form_state_mutation: bool
 
 
+FormFieldT = TypeVar("FormFieldT")
+
+
 @dataclass
 class FormField(Generic[FieldValueT]):
     name: str
     required: bool
     query_message: AnyText
 
     # should contain 1 '{}' for field value
     echo_result_template: Optional[AnyText] = dataclass_field(default=None, kw_only=True)
 
     # None (default) means sequential form flow
     next_field_getter: Optional[NextFieldGetter[FieldValueT]] = dataclass_field(default=None, kw_only=True)
 
+    result_formatting_opts: Optional[FormFieldResultFormattingOpts] = dataclass_field(default=None, kw_only=True)
+    export_opts: Optional[FormFieldResultExportOpts] = dataclass_field(default=None, kw_only=True)
+
     def __post_init__(self):
         pass  # future-proof
 
     def get_next_field_getter(self) -> NextFieldGetter[FieldValueT]:
         if self.next_field_getter is None:
             raise RuntimeError(
                 f"{self}: next field getter wasn't properly initialized; "
@@ -146,14 +182,15 @@
                 no_form_state_mutation=False,
             )
 
     async def get_query_message(self, user: tg.User) -> AnyText:
         return self.query_message
 
     def value_to_str(self, value: FieldValueT, language: MaybeLanguage) -> str:
+        """Fields can override this to specify the default human-readable formatting of the field value."""
         return str(value)
 
     def get_result_message(self, value: FieldValueT, language: MaybeLanguage) -> Optional[str]:
         if self.echo_result_template is None:
             return None
         else:
             return any_text_to_str(self.echo_result_template, language).format(self.value_to_str(value, language))
@@ -181,14 +218,26 @@
         return res
 
     def custom_texts(self) -> list[AnyText]:
         """If subclasses add their own field-related texts (custom error messages,
         button captions or anything else, they must list them here)"""
         return []
 
+    def with_output_opts(
+        self: FormFieldT,
+        formatting: Optional[FormFieldResultFormattingOpts] = None,
+        export: Optional[FormFieldResultExportOpts] = None,
+    ) -> FormFieldT:
+        """Typed version of dataclasses.replace"""
+        return dataclasses.replace(
+            self,
+            result_formatting_opts=formatting,
+            export_opts=export,
+        )
+
 
 @dataclass
 class PlainTextField(FormField[str]):
     empty_text_error_msg: AnyText
 
     def parse(self, message: tg.Message) -> str:
         text = message.text_content
@@ -217,14 +266,17 @@
         try:
             text = message.text_content.strip()
             numbers = text.split()
             return [int(n) for n in numbers]
         except Exception:
             raise BadFieldValueError(self.not_an_integer_list_error_msg)
 
+    def value_to_str(self, value: list[int], lang: MaybeLanguage) -> str:
+        return ", ".join(str(i) for i in value)
+
 
 @dataclass
 class DateField(FormField[date]):
     timezone: tzinfo
     bad_date_format_error_msg: AnyText
     # if specified, the date is checked to be in the future
     cant_be_in_the_past_error_msg: Optional[AnyText] = None
@@ -249,25 +301,31 @@
 
     def custom_texts(self) -> list[AnyText]:
         if self.cant_be_in_the_past_error_msg is not None:
             return [self.cant_be_in_the_past_error_msg]
         else:
             return []
 
+    def value_to_str(self, value: date, lang: MaybeLanguage) -> str:
+        return value.strftime("%d.%m.%Y")
+
 
 @dataclass
 class TimeField(FormField[time]):
     bad_time_format_msg: AnyText
 
     def parse(self, message: tg.Message) -> time:
         try:
             return time.fromisoformat(message.text_content)
         except ValueError as e:
             raise BadFieldValueError(self.bad_time_format_msg)
 
+    def value_to_str(self, value: time, lang: MaybeLanguage) -> str:
+        return value.isoformat(timespec="minutes")
+
 
 TelegramAttachment = Union[list[tg.PhotoSize], tg.Video, tg.Animation, tg.Audio, tg.Document]
 
 
 _users_uploading_media_group: set[int] = set()
 _media_group_attachments_stash: dict[str, list[TelegramAttachment]] = dict()
 
@@ -421,17 +479,14 @@
 class SingleSelectField(_EnumDefinedFieldMixin, FormField[Enum]):
     invalid_enum_value_error_msg: AnyText
     menu_row_width: int = 2
 
     def custom_value_type(self) -> Type:
         return self.EnumClass
 
-    def value_to_str(self, value: Enum, language: MaybeLanguage) -> str:
-        return any_text_to_str(value.value, language)
-
     def parse_enum(self, text: str) -> Optional[Enum]:
         for enum in self.EnumClass:
             if isinstance(enum.value, str):
                 if text == enum.value:
                     return enum
             elif isinstance(enum.value, dict):
                 for _, lang_text in enum.value.items():
@@ -449,14 +504,20 @@
     def parse(self, message: tg.Message) -> Enum:
         parsed_enum = self.parse_enum(message.text_content)
         if parsed_enum is None:
             raise BadFieldValueError(self.invalid_enum_value_error_msg)
         else:
             return parsed_enum
 
+    def value_to_str(self, value: Enum, lang: MaybeLanguage) -> str:
+        if not is_any_text(value.value):
+            return any_text_to_str(value.value, lang)
+        else:
+            return str(value.value)
+
 
 EnumField = SingleSelectField  # backward compatibility
 
 
 INLINE_FIELD_CALLBACK_DATA = CallbackData("fieldname", "payload", prefix="inline_field")
 
 
@@ -704,7 +765,10 @@
 
     def get_reply_markup(self, language: MaybeLanguage, current_value: Optional[date] = None) -> tg.ReplyMarkup:
         return self._calendar_keyboard(
             year=current_value.year if current_value else None,
             month=current_value.month if current_value else None,
             selected_value=current_value,
         )
+
+    def value_to_str(self, value: date, lang: MaybeLanguage) -> str:
+        return value.strftime("%d.%m.%Y")
```

### Comparing `telebot_components-0.8.3/telebot_components/form/form.py` & `telebot_components-0.8.4/telebot_components/form/form.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import copy
+import functools
+import operator
 from collections import defaultdict
 from dataclasses import dataclass
 from itertools import chain, zip_longest
 from types import GenericAlias
 from typing import (  # type: ignore
     Any,
+    Collection,
     Mapping,
     Optional,
     Type,
     _TypedDictMeta,
+    cast,
     get_args,
 )
 
-from telebot_components.form.field import FormField, NextFieldGetter
+from telebot_components.form.field import (
+    FormField,
+    FormFieldResultFormattingOpts,
+    NextFieldGetter,
+)
+from telebot_components.stores.language import MaybeLanguage
 
-FieldNameT = Optional[str]
+FieldName = Optional[str]
 
 
 class Form:
     """Container for collection of fields linked together via get_next_field_getter() attribute. Does not modify passed
     objects, creates private copies.
 
     If allow_cyclic param is False (default), performs topological sort to validate form acyclicity and can print
     it's graph structure in ASCII with print_graph method.
     """
 
-    def __init__(self, fields: list[FormField], start_field: Optional[FormField] = None, allow_cyclic: bool = False):
+    def __init__(
+        self, fields: Collection[FormField], start_field: Optional[FormField] = None, allow_cyclic: bool = False
+    ):
         if not fields:
             raise ValueError("Fields list can't be empty")
 
+        self.allow_cyclic = allow_cyclic
+
         # copying fields to avoid modifying user's objects
         self.fields = [copy.deepcopy(f) for f in fields]
         if start_field is None:
-            start_field = fields[0]
+            start_field = next(iter(fields))
         self.start_field = copy.deepcopy(start_field)
 
         # if any field has the next field getter omitted, use default sequential connection
         for field, next_field in zip_longest(self.fields, self.fields[1:]):
             if field.next_field_getter is None:
                 if isinstance(next_field, FormField):
                     field.next_field_getter = NextFieldGetter.by_name(next_field.name)
@@ -46,23 +59,23 @@
         # validating field name uniqueness
         field_names = [f.name for f in self.fields]
         for fn in field_names:
             if field_names.count(fn) > 1:
                 raise ValueError(f"All fields must have unique names, but there is at least one duplicate: {fn}!")
 
         # binding next field getters so that they can look up next form field by its name
-        fields_by_name = {f.name: f for f in self.fields}
+        self.fields_by_name = {f.name: f for f in self.fields}
         for f in self.fields:
-            f.get_next_field_getter().fields_by_name = fields_by_name
+            f.get_next_field_getter().fields_by_name = self.fields_by_name
 
         # validating that field graph is connected and that the start field has no incoming edges
         reachable_field_names = set(
             chain.from_iterable(f.get_next_field_getter().possible_next_field_names for f in self.fields)
         )
-        if not allow_cyclic and self.start_field.name in reachable_field_names:
+        if not self.allow_cyclic and self.start_field.name in reachable_field_names:
             raise ValueError(
                 f"Form configuration error: start field '{self.start_field.name}' is reachable from other field(s)"
             )
         reachable_field_names.add(self.start_field.name)
         if None not in reachable_field_names:
             raise ValueError("Endless form: no field has None (form end) as a possible next field")
         reachable_field_names.remove(None)
@@ -76,42 +89,64 @@
             unknown_reachable_field_names = reachable_field_names.difference(field_names)
             if unknown_reachable_field_names:
                 raise ValueError(
                     "Form configuration error: some fields list non-existing fields as reachable:"
                     + ", ".join([str(n) for n in unknown_reachable_field_names])
                 )
 
-        # topological sort to validate acyclicity + for nice rendering
-        if not allow_cyclic:
-            next_field_names: dict[FieldNameT, set[FieldNameT]] = {
-                f.name: set(f.get_next_field_getter().possible_next_field_names) for f in self.fields
-            }
-            prev_field_names: dict[FieldNameT, set[FieldNameT]] = defaultdict(set)
-            for field_name, nexts in next_field_names.items():
-                for next in nexts:
-                    prev_field_names[next].add(field_name)
+        # pre-calculating some generic graph-related stuff
+        self.next_field_names: dict[FieldName, set[FieldName]] = {
+            f.name: set(f.get_next_field_getter().possible_next_field_names) for f in self.fields
+        }
+        self.prev_field_names: dict[FieldName, set[FieldName]] = defaultdict(set)
+        for field_name, nexts in self.next_field_names.items():
+            for next_ in nexts:
+                self.prev_field_names[next_].add(field_name)
+
+        # calculating global requiredness for fields
+        if not self.allow_cyclic:
+
+            def paths_from(from_field: FieldName) -> list[list[FieldName]]:
+                if from_field is None:
+                    return [[]]
+                paths: list[list[FieldName]] = []
+                for step in self.next_field_names[from_field]:
+                    paths.extend([[from_field, *subpath] for subpath in paths_from(step)])
+                return paths
 
-            topologically_sorted: list[Optional[str]] = []
-            vertices_without_incoming_edges: set[Optional[str]] = {self.start_field.name}
+            path_fields = [set(p) for p in paths_from(self.start_field.name)]
+            self.globally_required_fields: Optional[set[FieldName]] = functools.reduce(operator.and_, path_fields)
+        else:
+            self.globally_required_fields = None
+
+        # topological sort to validate acyclicity + for nice rendering
+        if not self.allow_cyclic:
+            next_field_names = self.next_field_names.copy()
+            prev_field_names = self.prev_field_names.copy()
+            topologically_sorted: list[str] = []
+            # NOTE: this is semantically set, but we use list for predictability
+            vertices_without_incoming_edges: list[Optional[str]] = [self.start_field.name]
             while vertices_without_incoming_edges:
-                from_ = vertices_without_incoming_edges.pop()
-                topologically_sorted.append(from_)
-                tos = next_field_names.get(from_)
+                vertices_without_incoming_edges.sort()
+                from_ = vertices_without_incoming_edges.pop(0)
+                if from_ is not None:
+                    topologically_sorted.append(from_)
+                tos = self.next_field_names.get(from_)
                 if tos is None:
                     continue
                 tos = tos.copy()
                 for to in tos:
                     next_field_names[from_].remove(to)
                     prev_field_names[to].remove(from_)
                     if not prev_field_names[to]:
-                        vertices_without_incoming_edges.add(to)
+                        vertices_without_incoming_edges.append(to)
 
             if any(next_field_names.values()):
                 raise ValueError("Form graph has at least one cycle")
-            self.topologically_sorted_field_names: Optional[list[FieldNameT]] = topologically_sorted
+            self.topologically_sorted_field_names: Optional[list[str]] = topologically_sorted
         else:
             self.topologically_sorted_field_names = None
 
     @staticmethod
     def _field_value_type(field: FormField) -> Any:
         custom_value_type = field.custom_value_type()
         if custom_value_type is not None:
@@ -156,40 +191,91 @@
                     + (" (Optional reflects the fact that the field is not required)" if not field.required else "")
                 )
 
     def generate_result_type(self) -> str:
         indent = " " * 4
         lines = ["class MyFormResultT(TypedDict):", indent + '"""Generated by Form.generate_result_type() method"""']
         fields = self.fields.copy()
+        fields.sort(key=lambda ff: ff.name)  # first, alphabetical sort
         if self.topologically_sorted_field_names is not None:
+            # then, if possible, topological
             fields.sort(key=lambda ff: self.topologically_sorted_field_names.index(ff.name))  # type: ignore
         for field in fields:
             field_type_str = self._field_value_type_to_string(self._field_value_type(field))
             if not field.required:
                 field_type_str = f"Optional[{field_type_str}]"
+            if self.globally_required_fields is not None and field.name not in self.globally_required_fields:
+                field_type_str = f"NotRequired[{field_type_str}]"
             lines.append(indent + f"{field.name}: {field_type_str}")
         return "\n".join(lines)
 
-    def print_graph(self):
+    def result_to_html(self, result: Mapping[str, Any], lang: MaybeLanguage) -> str:
+        for f in self.fields:
+            if f.result_formatting_opts is None:
+                raise ValueError(
+                    f"Can't convert result to telegram message, field {f.name!r} does not have formatting opts"
+                )
+
+        lines: list[str] = []
+        field_names = self.topologically_sorted_field_names or sorted([f.name for f in self.fields])
+        for field_name in field_names:
+            field = self.fields_by_name[field_name]
+            formatting_opts = cast(FormFieldResultFormattingOpts, field.result_formatting_opts)
+            field_descr = formatting_opts.descr
+            if field_name not in result:
+                if self.globally_required_fields is not None and field_name in self.globally_required_fields:
+                    raise ValueError(f"Globally required field {field_name!r} not found in result")
+                else:
+                    continue
+            field_value = result[field_name]
+            field_value_formatter = formatting_opts.value_formatter or field.value_to_str
+            if field_value is not None:
+                lines.append(
+                    format_named_value(
+                        field_descr,
+                        field_value_formatter(field_value, lang),
+                        single_line=not formatting_opts.is_multiline,
+                    )
+                )
+        return "\n".join(lines)
+
+    def result_to_export(self, result: Mapping[str, Any]) -> dict[Any, Any]:
+        exported: dict[Any, Any] = dict()
+        for name, value in result.items():
+            field = self.fields_by_name[name]
+            if field.export_opts is None:
+                continue
+            if field.export_opts.value_mapping is not None:
+                value_for_export = field.export_opts.value_mapping[value]
+            elif field.export_opts.value_processor is not None:
+                value_for_export = field.export_opts.value_processor(value)
+            else:
+                value_for_export = value
+            exported[field.export_opts.column] = value_for_export
+        return exported
+
+    # VVVVVV messy shitty terminal visualization code VVVVVV
+
+    def format_graph(self) -> str:
         if self.topologically_sorted_field_names is None:
             raise ValueError("print_graph method only available for acyclic form graphs")
         DEFAULT_FORM_END_PRINT = "END"
         form_end_print_name = DEFAULT_FORM_END_PRINT
         idx = 0
         while form_end_print_name in self.topologically_sorted_field_names:
             idx += 1
             form_end_print_name = f"{DEFAULT_FORM_END_PRINT} ({idx})"
 
-        def to_print(name: FieldNameT) -> str:
+        def to_print(name: FieldName) -> str:
             if isinstance(name, str):
                 return name
             else:
                 return form_end_print_name
 
-        vertex_names = [to_print(fn) for fn in self.topologically_sorted_field_names]
+        vertex_names = self.topologically_sorted_field_names + [form_end_print_name]
         max_vertex_name_len = max([len(v) for v in vertex_names]) + 2
 
         edges: set[tuple[str, str]] = set()
         for f in self.fields:
             for next_field_name in f.get_next_field_getter().possible_next_field_names:
                 edges.add((to_print(f.name), to_print(next_field_name)))
 
@@ -234,15 +320,18 @@
             arc_canvas = CharCanvas()
             arc_margin = 1 + 2 * arc_idx
             arc_canvas.insert_string(0, 0, ("─" * arc_margin) + "┐")
             arc_canvas.insert_string(1, arc_margin, "|" * (arc_end_i - arc_start_i - 1), vertical=True)
             arc_canvas.insert_string(arc_end_i - arc_start_i, 0, ("─" * arc_margin) + "┘")
             canvas.overlay(arc_canvas, arc_start_i, max_vertex_name_len + 3, front=False)
 
-        canvas.print()
+        return canvas.format()
+
+    def print_graph(self) -> None:
+        print(self.format_graph())
 
 
 @dataclass
 class VertexBox:
     name: str
     name_print_len: int
     n_arcs_out: int
@@ -331,21 +420,31 @@
         for i_local, row in enumerate(other._array):
             for j_local, char in enumerate(row):
                 self.insert_char(i_top + i_local, j_left + j_local, char, front)
 
     def join_down(self, other: "CharCanvas", j_left: int, front: bool = True):
         self.overlay(other, self.height, j_left, front)
 
+    def format(self):
+        return "\n".join("".join(row) for row in self._array)
+
     def print(self):
-        for row in self._array:
-            print("".join(row))
+        print(self.format())
 
 
 def pad_to_len(string: str, length: int) -> str:
     add_to_right = True
     while len(string) < length:
         if add_to_right:
             string = string + " "
         else:
             string = " " + string
         add_to_right = not add_to_right
     return string
+
+
+def format_named_value(name: str, value: str, single_line: bool = True) -> str:
+    sep = ": " if single_line else "\n"
+    result = f"<b>{name}</b>{sep}{value}"
+    if not single_line:
+        result += "\n"
+    return result
```

### Comparing `telebot_components-0.8.3/telebot_components/form/handler.py` & `telebot_components-0.8.4/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.4/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/menu/menu.py` & `telebot_components-0.8.4/telebot_components/menu/menu.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.4/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.4/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/stores/banned_users.py` & `telebot_components-0.8.4/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/stores/category.py` & `telebot_components-0.8.4/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.4/telebot_components/stores/forum_topics.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                             success = await self.bot.edit_forum_topic(
                                 chat_id=self.admin_chat_id,
                                 message_thread_id=existing_message_thread_id,
                                 name=topic_spec.name,
                                 icon_custom_emoji_id=topic_spec.icon_custom_emoji_id,
                             )
                         except ApiHTTPException as e:
-                            if "TOPIC_NOT_MODIFIED" in e.error_description:
+                            if e.error_description is not None and "TOPIC_NOT_MODIFIED" in e.error_description:
                                 success = True
                             else:
                                 self.logger.exception("Unexpected error syncing topic")
 
                         if success:
                             self.logger.info(f"Forum topic OK: {topic_spec}")
                             await asyncio.sleep(5)
```

### Comparing `telebot_components-0.8.3/telebot_components/stores/generic.py` & `telebot_components-0.8.4/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/stores/language.py` & `telebot_components-0.8.4/telebot_components/stores/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Optional, Union
+from typing import Any, Optional, TypeGuard, Union
 
 from telebot import AsyncTeleBot, types
 from telebot.callback_data import CallbackData
 
 from telebot_components.constants import times
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.generic import KeyValueStore
@@ -39,35 +39,47 @@
 
 
 MaybeLanguage = Optional[Language]  # None = multilang mode is off, using regular strings
 
 
 MultilangText = dict[Language, str]
 
+AnyText = Union[str, MultilangText]
 
-def validate_multilang_text(t: Any, languages: list[Language]) -> MultilangText:
+
+def is_multilang_text(t: Any) -> TypeGuard[MultilangText]:
     if not isinstance(t, dict):
-        raise TypeError(f"Language -> str dictionary expected, found {type(t).__name__}: {t}")
+        return False
+    for key, value in t.items():
+        if not isinstance(key, Language):
+            return False
+        if not isinstance(value, str):
+            return False
+    return True
+
+
+def is_any_text(t: Any) -> TypeGuard[AnyText]:
+    return is_multilang_text(t) or isinstance(t, str)
+
+
+def validate_multilang_text(t: Any, languages: list[Language]) -> MultilangText:
+    if not is_multilang_text(t):
+        raise TypeError(f"Not a multilang text: {t}")
     for language in languages:
         if language not in t:
             raise ValueError(f"Multilang text misses localisation to '{language}': {t}")
-        if not isinstance(t[language], str):
-            raise ValueError(f"Non-string text for language {language}: {t[language]!r}")
     return t
 
 
 def vaildate_singlelang_text(t: Any) -> str:
     if not isinstance(t, str):
         raise TypeError(f"Single language text must be a string, found {type(t).__name__}: {t}")
     return t
 
 
-AnyText = Union[str, MultilangText]
-
-
 def any_text_to_str(t: AnyText, language: MaybeLanguage) -> str:
     if language is None:
         if isinstance(t, str):
             return t
         else:
             raise ValueError("MultilangText requires a valid Language for localisation")
     else:
```

### Comparing `telebot_components-0.8.3/telebot_components/stores/user_group.py` & `telebot_components-0.8.4/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/stores/utils.py` & `telebot_components-0.8.4/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/utils/__init__.py` & `telebot_components-0.8.4/telebot_components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/utils/airtable.py` & `telebot_components-0.8.4/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/utils/alerts.py` & `telebot_components-0.8.4/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/telebot_components/utils/strings.py` & `telebot_components-0.8.4/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.3/PKG-INFO` & `telebot_components-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.3
+Version: 0.8.4
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

