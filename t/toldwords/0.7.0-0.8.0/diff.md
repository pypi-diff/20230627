# Comparing `tmp/toldwords-0.7.0.tar.gz` & `tmp/toldwords-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toldwords-0.7.0.tar", max compression
+gzip compressed data, was "toldwords-0.8.0.tar", max compression
```

## Comparing `toldwords-0.7.0.tar` & `toldwords-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.7.0/README.md
--rw-r--r--   0        0        0     1990 2023-05-17 02:46:11.152718 toldwords-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      521 2023-05-17 02:43:19.968588 toldwords-0.7.0/toldwords/__init__.py
--rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.7.0/toldwords/openai.py
--rw-r--r--   0        0        0     5357 2023-05-17 02:44:00.138741 toldwords-0.7.0/toldwords/pretalx.py
--rw-r--r--   0        0        0        0 2023-04-19 02:44:37.772682 toldwords-0.7.0/toldwords/py.typed
--rw-r--r--   0        0        0      166 2023-05-04 06:45:27.125645 toldwords-0.7.0/toldwords/utils.py
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 toldwords-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.8.0/README.md
+-rw-r--r--   0        0        0     2007 2023-06-27 09:30:13.314591 toldwords-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      521 2023-06-27 09:30:18.934032 toldwords-0.8.0/toldwords/__init__.py
+-rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.8.0/toldwords/openai.py
+-rw-r--r--   0        0        0     7066 2023-06-27 09:16:27.633448 toldwords-0.8.0/toldwords/pretalx.py
+-rw-r--r--   0        0        0        0 2023-04-19 02:44:37.772682 toldwords-0.8.0/toldwords/py.typed
+-rw-r--r--   0        0        0      166 2023-05-04 06:45:27.125645 toldwords-0.8.0/toldwords/utils.py
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 toldwords-0.8.0/PKG-INFO
```

### Comparing `toldwords-0.7.0/LICENSE.txt` & `toldwords-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toldwords-0.7.0/pyproject.toml` & `toldwords-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toldwords"
-version = "0.7.0"
+version = "0.8.0"
 description = "Using ChatGPT to make keywords for the papers from COSCUP."
 authors = ["Toomore Chiang <toomore0929@gmail.com>"]
 license = 'MIT'
 readme = "README.md"
 homepage = 'https://github.com/toomore/toldwords'
 repository = 'https://github.com/toomore/toldwords'
 packages = [
@@ -25,14 +25,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 certifi = "*"
 pydantic = "^1.10.6"
+arrow = "^1.2.3"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 pylint = "^2.17.0"
 autopep8 = "^2.0.2"
 types-requests = "^2.28.11.15"
```

### Comparing `toldwords-0.7.0/toldwords/openai.py` & `toldwords-0.8.0/toldwords/openai.py`

 * *Files identical despite different names*

### Comparing `toldwords-0.7.0/toldwords/pretalx.py` & `toldwords-0.8.0/toldwords/pretalx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,77 @@
 ''' Fetch data from pretalx '''
-from typing import List, Generator, Any
-from requests import Session
+from datetime import datetime
+from typing import Any, Generator, List
+
+import arrow
 from pydantic import BaseModel, Field, parse_obj_as, validator
+from requests import Session
+
+
+def convert_datetime(value: Any) -> datetime:
+    ''' convert `action_date` to date '''
+    return arrow.get(value).naive
+
+
+class Speaker(BaseModel):
+    ''' Speaker '''
+    code: str = Field(default_factory=str)
+    name: str = Field(default_factory=str)
+    biography: str | None = Field(default_factory=str)
+    avatar: str | None = Field(default_factory=str)
+    submissions: list[str] | None = Field(default_factory=list)
+    email: str | None = Field(default_factory=str)
+    availabilities: list[dict[str, Any]] = Field(default_factory=list)
+
+
+class Slot(BaseModel):
+    ''' Slot in talk '''
+    start: datetime = Field(default_factory=datetime.now,
+                            description='Start time')
+    end: datetime = Field(default_factory=datetime.now, description='End time')
+    room: dict[str, str] = Field(default_factory=dict, description='Room name')
+    room_id: int = Field(default=0, description='Room ID')
+
+    _validate_convert_datetime = validator(
+        'start', 'end',
+        pre=True, allow_reuse=True, always=True)(convert_datetime)
 
 
 class Talk(BaseModel):
     ''' Talk '''
+    # pylint: disable=no-self-argument
     code: str = Field(default_factory=str,
                       description='A unique, alphanumeric identifier, also used in URLs')
     title: str = Field(default_factory=str,
                        description='The submission’s title')
+    track: dict[str, str] = Field(description='The track this talk belongs to')
     track_id: int = Field(default_factory=int,
                           description='ID of the track this talk belongs to')
+    submission_type: dict[str, str] | None = Field(
+        description='The submission type')
     state: str = Field(default_factory=str,
-                       description='The submission’s state, one of “submitted”, “accepted”, “rejected”, “confirmed”')
+                       description='The submission’s state, one of '
+                                   '“submitted”, “accepted”, “rejected”, “confirmed”')
     abstract: str = Field(default_factory=str,
                           description='The abstract, a short note of the submission’s content')
+    duration: int = Field(
+        default_factory=int, description='The talk’s duration in minutes, or null')
+    content_locale: str = Field(
+        default_factory=str, description='The language the submission is in, e.g. “en” or “de”')
+    slot: Slot = Field(default=Slot, description='The datetime in talk')
+    speakers: list[Speaker] = Field(
+        default_factory=list, description='A list of speaker objects')
 
+    @validator('track', pre=True)
+    def verify_track(cls, value: Any) -> dict[str, str]:
+        ''' verify track '''
+        if value is None:
+            return {'en': 'no track'}
 
-class Speaker(BaseModel):
-    ''' Speaker '''
-    code: str = Field(default_factory=str)
-    name: str = Field(default_factory=str)
-    biography: str | None = Field(default_factory=str)
-    avatar: str | None = Field(default_factory=str)
-    submissions: list[str] | None = Field(default_factory=list)
-    email: str | None = Field(default_factory=str)
-    availabilities: list[dict[str, Any]] = Field(default_factory=list)
+        return value
 
 
 class Submission(BaseModel):
     ''' Submission '''
     # pylint: disable=no-self-argument
     code: str = Field(default_factory=str,
                       description='A unique, alphanumeric identifier, also used in URLs')
@@ -41,24 +82,26 @@
     track: dict[str, str] = Field(
         description='The track this talk belongs to')
     track_id: int | None = Field(
         description='ID of the track this talk belongs to')
     submission_type: dict[str, str] | None = Field(
         description='The submission type')
     state: str = Field(
-        description='The submission’s state, one of “submitted”, “accepted”, “rejected”, “confirmed”')
+        description='The submission’s state, one of '
+                    '“submitted”, “accepted”, “rejected”, “confirmed”')
     abstract: str = Field(
         description='The abstract, a short note of the submission’s content')
     duration: int = Field(
         default_factory=int, description='The talk’s duration in minutes, or null')
     content_locale: str = Field(
         default_factory=str, description='The language the submission is in, e.g. “en” or “de”')
     notes: str = Field(default_factory=str, description='note')
     internal_notes: str | None = Field(
-        description='Notes the organisers left on the submission. Available if the requesting user has organiser permissions.')
+        description='Notes the organisers left on the submission.'
+                    'Available if the requesting user has organiser permissions.')
 
     @validator('track', pre=True)
     def verify_track(cls, value: Any) -> dict[str, str]:
         ''' verify track '''
         if value is None:
             return {'en': 'no track'}
 
@@ -71,15 +114,17 @@
                     description="The unique ID of the room object")
     name: str = Field(default_factory=str, description='The name of the room')
     description: str = Field(
         default_factory=str, description='The description of the room')
     capacity: int = Field(default_factory=int,
                           description='How many people fit in the room')
     position: int = Field(
-        default_factory=int, description='A number indicating the ordering of the room relative to other rooms, e.g. in schedule visualisations')
+        default_factory=int, description='A number indicating the ordering of '
+                                         'the room relative to other rooms, '
+                                         'e.g. in schedule visualisations')
     speaker_info: str = Field(default_factory=str)
     availabilities: list[dict[str, Any]] = Field(default_factory=list)
 
 
 class PretalxResponse(BaseModel):
     ''' PretalxResponse '''
     count: int
```

### Comparing `toldwords-0.7.0/PKG-INFO` & `toldwords-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toldwords
-Version: 0.7.0
+Version: 0.8.0
 Summary: Using ChatGPT to make keywords for the papers from COSCUP.
 Home-page: https://github.com/toomore/toldwords
 License: MIT
 Keywords: API,ChatGPT,pretalx,COSCUP,openai
 Author: Toomore Chiang
 Author-email: toomore0929@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -12,20 +12,18 @@
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: certifi
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/toomore/toldwords
 Description-Content-Type: text/markdown
 
 # toldwords
```

