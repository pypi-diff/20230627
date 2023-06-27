# Comparing `tmp/sddl_parser-0.1.0.tar.gz` & `tmp/sddl_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddl_parser-0.1.0.tar", max compression
+gzip compressed data, was "sddl_parser-0.2.0.tar", max compression
```

## Comparing `sddl_parser-0.1.0.tar` & `sddl_parser-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      398 2023-06-23 21:06:40.503242 sddl_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1493 2023-06-23 21:00:01.403378 sddl_parser-0.1.0/README.md
--rw-r--r--   0        0        0       42 2023-06-23 04:46:49.890300 sddl_parser-0.1.0/sddl_parser/__init__.py
--rw-r--r--   0        0        0      229 2023-06-23 21:09:56.417748 sddl_parser-0.1.0/sddl_parser/api.py
--rw-r--r--   0        0        0     8961 2023-06-23 20:47:39.016601 sddl_parser-0.1.0/sddl_parser/dictionary.py
--rw-r--r--   0        0        0     5447 2023-06-23 21:10:10.634227 sddl_parser-0.1.0/sddl_parser/parser.py
--rw-r--r--   0        0        0      651 2023-06-23 20:17:23.662099 sddl_parser-0.1.0/sddl_parser/types.py
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 sddl_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      398 2023-06-27 21:46:46.042420 sddl_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3741 2023-06-27 21:44:17.810516 sddl_parser-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2023-06-27 15:03:35.127501 sddl_parser-0.2.0/sddl_parser/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-27 16:21:14.512040 sddl_parser-0.2.0/sddl_parser/api.py
+-rw-r--r--   0        0        0     5151 2023-06-27 20:20:51.962626 sddl_parser-0.2.0/sddl_parser/dictionary.py
+-rw-r--r--   0        0        0     5195 2023-06-27 20:56:57.890162 sddl_parser-0.2.0/sddl_parser/parser.py
+-rw-r--r--   0        0        0    50423 2023-06-27 21:38:38.418293 sddl_parser-0.2.0/sddl_parser/rights_enums.py
+-rw-r--r--   0        0        0      796 2023-06-27 20:10:00.050365 sddl_parser-0.2.0/sddl_parser/type_enums.py
+-rw-r--r--   0        0        0     1439 2023-06-27 19:55:38.294366 sddl_parser-0.2.0/sddl_parser/types.py
+-rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 sddl_parser-0.2.0/PKG-INFO
```

### Comparing `sddl_parser-0.1.0/sddl_parser/parser.py` & `sddl_parser-0.2.0/sddl_parser/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,22 @@
 from parsy import string, regex, char_from, seq, test_char, Parser, generate
 from functools import reduce
 from operator import or_
 from typing import List, Dict, Any, Callable
 from functools import partial
 from sddl_parser.dictionary import (
     SDDL_SIDS,
-    SDDL_CMPST_RIGHTS,
     SDDL_FLAGS,
     ACE_TYPE,
     ACE_FLAGS,
     ACE_RIGHTS,
 )
 from sddl_parser.types import ACE, DACL, SDDL, SACL
 
 
-def rights_to_string(rights: int) -> List[str]:
-    rs = []
-    for g in SDDL_CMPST_RIGHTS:  # composite rights first
-        mask = ACE_RIGHTS[g][2]
-        if (rights & mask) == mask:
-            rights -= mask
-            rs.append(ACE_RIGHTS[g][0])
-    while rights > 0:  # then parse with bitmask
-        for r in ACE_RIGHTS.values():
-            if (rights & r[2]) == r[2]:
-                rights -= r[2]
-                rs.append(r[0])
-    return rs
-
-
 def parser_from_list(xs: List[str]) -> Parser:
     if not xs:
         raise ValueError("list is empty")
     return reduce(or_, map(string, xs))
 
 
 def create_parser_from_dict(
@@ -59,55 +43,56 @@
 
 
 def take_till_paren() -> Parser:
     return take_till(lambda x: x == "(" or x == ")", "not ( or )")
 
 
 def parse_sid() -> Parser:
+    return regex(r"S-1(?:-\d+)*")
+
+
+def parse_sid_field() -> Parser:
     well_known_sid = create_parser_from_dict(SDDL_SIDS)
-    specific_sid = regex(r"S-1(?:-\d+)*")
-    return well_known_sid | specific_sid
+    return well_known_sid | parse_sid()
 
 
 def parse_owner() -> Parser:
     owner_identifier = string("O:")
-    return owner_identifier >> parse_sid()
+    return owner_identifier >> parse_sid_field()
 
 
 def parse_group() -> Parser:
     group_identifier = string("G:")
-    return group_identifier >> parse_sid()
+    return group_identifier >> parse_sid_field()
 
 
 sacl_identifier = string("S:")
 dacl_identifier = string("D:")
 sddl_flags = create_parser_from_dict(SDDL_FLAGS).map(lambda x: x.split("|"))
 
-ace_types = create_parser_from_dict(ACE_TYPE, lambda xs, k: xs[k][0])
+ace_types = create_parser_from_dict(ACE_TYPE, lambda xs, k: xs[k])
 
 
 def parse_ace_flags() -> Parser:
     def flags_map(x: str) -> List[str]:
         split_by_two = map("".join, zip(*[iter(x)] * 2))
         return list(map(lambda x: ACE_FLAGS[x][0], split_by_two))
 
+    # TODO: Actually parse here instead of just grabbing till ;
     return (take_till_char(";").map(flags_map)) | string("")
 
-    # ace_flags = create_parser_from_dict(ACE_FLAGS, lambda xs, k: xs[k][0]) | string("")
-
 
 def parse_ace_rights() -> Parser:
-    def rights_map(x: str) -> List[str]:
-        split_by_two = map("".join, zip(*[iter(x)] * 2))
-        return list(map(lambda x: ACE_RIGHTS[x][0], split_by_two))
+    hex_ace_rights = regex(r"0x[0-9a-fA-F]+").map(lambda x: int(x, 16))
 
-    hex_ace_rights = (
-        regex(r"0x[0-9a-fA-F]+").map(lambda x: int(x, 16)).map(rights_to_string)
+    well_known_ace_rights = (
+        parser_from_list(list(ACE_RIGHTS.keys()))
+        .many()
+        .map(lambda xs: sum(map(lambda x: ACE_RIGHTS[x], xs)))
     )
-    well_known_ace_rights = take_till_char(";").map(rights_map)
     return hex_ace_rights | well_known_ace_rights
 
 
 # I've never not seen these empty, but they're in the spec
 object_guid = string("")
 inherit_object_guid = string("")
 
@@ -142,18 +127,18 @@
     https://learn.microsoft.com/en-us/windows/win32/secauthz/ace-strings
     Example: (A;;CCLCSWLOCRRC;;;SU)
     """
     return string("(") >> (
         seq(
             type=ace_types << char_from(";"),
             flags=parse_ace_flags() << char_from(";"),
-            rights=parse_ace_rights() << char_from(";"),
+            rights_int=parse_ace_rights() << char_from(";"),
             object_guid=object_guid << char_from(";"),
             inherit_object_guid=inherit_object_guid << char_from(";"),
-            sid=parse_sid(),
+            sid=parse_sid_field(),
             conditional_ace=parse_conditional_ace().optional(),
         )
         << string(")")
     ).combine_dict(ACE)
 
 
 dacl = seq(
@@ -163,10 +148,15 @@
 sacl = seq(
     flags=sacl_identifier >> sddl_flags, aces=parse_ace_entry().many()
 ).combine_dict(SACL)
 
 
 # https://learn.microsoft.com/en-us/windows/win32/secauthz/sid-strings?source=recommendations
 # Example: O:SYG:SYD:(A;ID;FA;;;SY)
+# TODO: Allow entries to be out of order.
+# Something like sddl_item = parse_owner() | parse_group() | dacl | sacl
+# Then sddl_entry = sddl_item.many(), then just map each type to a single object
+# Not sure how you ensure only one of each type. Maybe just post-processing,
+# but I feel like that could be done in the parser
 sddl_item = seq(
     owner=parse_owner(), group=parse_group(), dacl=dacl.optional(), sacl=sacl.optional()
 ).combine_dict(SDDL)
```

