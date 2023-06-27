# Comparing `tmp/sqlfluff-plugin-sparksql-upgrade-0.0.0.tar.gz` & `tmp/sqlfluff-plugin-sparksql-upgrade-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlfluff-plugin-sparksql-upgrade-0.0.0.tar", last modified: Tue Nov 15 17:44:39 2022, max compression
+gzip compressed data, was "sqlfluff-plugin-sparksql-upgrade-0.1.0.tar", last modified: Tue Jun 27 20:43:14 2023, max compression
```

## Comparing `sqlfluff-plugin-sparksql-upgrade-0.0.0.tar` & `sqlfluff-plugin-sparksql-upgrade-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 holden    (1000) holden    (1000)        0 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/
--rw-rw-r--   0 holden    (1000) holden    (1000)       47 2022-10-05 18:08:41.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/MANIFEST.in
--rw-rw-r--   0 holden    (1000) holden    (1000)      314 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/PKG-INFO
--rw-rw-r--   0 holden    (1000) holden    (1000)       38 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/setup.cfg
--rw-rw-r--   0 holden    (1000) holden    (1000)     1075 2022-11-15 17:41:56.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/setup.py
-drwxrwxr-x   0 holden    (1000) holden    (1000)        0 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/
-drwxrwxr-x   0 holden    (1000) holden    (1000)        0 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sparksql/
--rw-rw-r--   0 holden    (1000) holden    (1000)       31 2022-10-05 00:49:28.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sparksql/__init__.py
--rw-rw-r--   0 holden    (1000) holden    (1000)       60 2022-10-05 00:49:28.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sparksql/plugin_default_config.cfg
--rw-rw-r--   0 holden    (1000) holden    (1000)    15566 2022-11-09 22:21:35.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sparksql/rules.py
-drwxrwxr-x   0 holden    (1000) holden    (1000)        0 2022-11-15 17:44:39.734382 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/
--rw-rw-r--   0 holden    (1000) holden    (1000)      314 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/PKG-INFO
--rw-rw-r--   0 holden    (1000) holden    (1000)      468 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/SOURCES.txt
--rw-rw-r--   0 holden    (1000) holden    (1000)        1 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/dependency_links.txt
--rw-rw-r--   0 holden    (1000) holden    (1000)       46 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/entry_points.txt
--rw-rw-r--   0 holden    (1000) holden    (1000)       16 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/requires.txt
--rw-rw-r--   0 holden    (1000) holden    (1000)        9 2022-11-15 17:44:39.000000 sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/top_level.txt
+drwxr-xr-x   0 dpratap    (501) staff       (20)        0 2023-06-27 20:43:14.922568 sqlfluff-plugin-sparksql-upgrade-0.1.0/
+-rw-r--r--   0 dpratap    (501) staff       (20)       55 2023-06-12 17:22:17.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/MANIFEST.in
+-rw-r--r--   0 dpratap    (501) staff       (20)      338 2023-06-27 20:43:14.922422 sqlfluff-plugin-sparksql-upgrade-0.1.0/PKG-INFO
+-rw-r--r--   0 dpratap    (501) staff       (20)       38 2023-06-27 20:43:14.922613 sqlfluff-plugin-sparksql-upgrade-0.1.0/setup.cfg
+-rw-r--r--   0 dpratap    (501) staff       (20)     1144 2023-06-27 20:42:08.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/setup.py
+drwxr-xr-x   0 dpratap    (501) staff       (20)        0 2023-06-27 20:43:14.919813 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/
+drwxr-xr-x   0 dpratap    (501) staff       (20)        0 2023-06-27 20:43:14.920716 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sparksql_upgrade/
+-rw-r--r--   0 dpratap    (501) staff       (20)       31 2023-06-12 17:22:17.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sparksql_upgrade/__init__.py
+-rw-r--r--   0 dpratap    (501) staff       (20)        0 2023-06-12 17:22:17.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sparksql_upgrade/plugin_default_config.cfg
+-rw-r--r--   0 dpratap    (501) staff       (20)    20110 2023-06-12 17:22:17.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sparksql_upgrade/rules.py
+drwxr-xr-x   0 dpratap    (501) staff       (20)        0 2023-06-27 20:43:14.922228 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/
+-rw-r--r--   0 dpratap    (501) staff       (20)      338 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 dpratap    (501) staff       (20)      492 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 dpratap    (501) staff       (20)        1 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 dpratap    (501) staff       (20)       53 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 dpratap    (501) staff       (20)       16 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/requires.txt
+-rw-r--r--   0 dpratap    (501) staff       (20)       17 2023-06-27 20:43:14.000000 sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sqlfluff_plugin_sparksql_upgrade.egg-info/top_level.txt
```

### Comparing `sqlfluff-plugin-sparksql-upgrade-0.0.0/setup.py` & `sqlfluff-plugin-sparksql-upgrade-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Setup file for example plugin."""
 from setuptools import find_packages, setup
 
 # Change these names in your plugin, e.g. company name or plugin purpose.
 PLUGIN_LOGICAL_NAME = "sparksql-upgrade"
-PLUGIN_ROOT_MODULE = "sparksql"
+PLUGIN_ROOT_MODULE = "sparksql_upgrade"
 
 setup(
     name="sqlfluff-plugin-{plugin_logical_name}".format(
         plugin_logical_name=PLUGIN_LOGICAL_NAME
     ),
-    version='',
-    author='Holden Karau',
-    author_email='holden@pigscanfly.ca',
-    url='https://github.com/holdenk/spark-upgrade',
-    description='SQLFluff rules to help migrate your Spark SQL from 2.X to 3.X',
-    test_requires=[
-        'nose',
-        'coverage',
-        'unittest2'
-    ],
-    license='../LICENSE',
+    version="0.1.0",
+    author="Holden Karau",
+    author_email="holden@pigscanfly.ca",
+    url="https://github.com/holdenk/spark-upgrade",
+    description="SQLFluff rules to help migrate your Spark SQL from 2.X to 3.X",
+    long_description="SQLFluff rules to help migrate your Spark SQL from 2.X to 3.X",
+    test_requires=["nose", "coverage", "unittest2"],
+    license="../LICENSE",
     include_package_data=True,
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires="sqlfluff>=1.0.0",
     entry_points={
         "sqlfluff": [
             "{plugin_logical_name} = {plugin_root_module}.rules".format(
```

### Comparing `sqlfluff-plugin-sparksql-upgrade-0.0.0/src/sparksql/rules.py` & `sqlfluff-plugin-sparksql-upgrade-0.1.0/src/sparksql_upgrade/rules.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,47 @@
-"""An example of a custom rule implemented through the plugin system."""
+"""Custom Spark SQL upgrade rules."""
 
+import os.path
+from typing import List, Optional
+
+
+from sqlfluff.core.config import ConfigLoader
+from sqlfluff.core.parser import (
+    KeywordSegment,
+    SymbolSegment,
+    WhitespaceSegment,
+)
+from sqlfluff.core.parser.segments.raw import CodeSegment
 from sqlfluff.core.plugin import hookimpl
 from sqlfluff.core.rules import (
     BaseRule,
-    LintResult,
     LintFix,
+    LintResult,
     RuleContext,
 )
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.core.rules.doc_decorators import (
     document_configuration,
     document_fix_compatible,
     document_groups,
 )
-from sqlfluff.core.parser.segments.raw import CodeSegment
-from sqlfluff.utils.functional import sp, FunctionalContext
-from typing import List, Optional
-import os.path
-from sqlfluff.core.config import ConfigLoader
+from sqlfluff.utils.functional import FunctionalContext, sp
 
 
 @hookimpl
 def get_rules() -> List[BaseRule]:
     """Get plugin rules."""
-    return [Rule_Example_L001, Rule_SPARKSQLCAST_L001, Rule_RESERVEDROPERTIES_L002,
-            Rule_NOCHARS_L003, Rule_FORMATSTRONEINDEX_L004]
+    return [
+        Rule_SPARKSQLCAST_L001,
+        Rule_RESERVEDROPERTIES_L002,
+        Rule_NOCHARS_L003,
+        Rule_FORMATSTRONEINDEX_L004,
+        Rule_SPARKSQL_L004,
+        Rule_SPARKSQL_L005,
+    ]
 
 
 @hookimpl
 def load_default_config() -> dict:
     """Loads the default configuration for the plugin."""
     return ConfigLoader.get_global().load_config_file(
         file_dir=os.path.dirname(__file__),
@@ -74,41 +87,39 @@
     groups = ("all",)
     crawl_behaviour = SegmentSeekerCrawler({"function"})
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Check integer casts."""
         functional_context = FunctionalContext(context)
         children = functional_context.segment.children()
-        function_name_id_seg = children.first(sp.is_type("function_name")).children(
-        ).first(sp.is_type("function_name_identifier"))[0]
+        function_name_id_seg = (
+            children.first(sp.is_type("function_name"))
+            .children()
+            .first(sp.is_type("function_name_identifier"))[0]
+        )
         raw_function_name = function_name_id_seg.raw.upper().strip()
         function_name = raw_function_name.upper().strip()
         bracketed_segments = children.first(sp.is_type("bracketed"))
         bracketed = bracketed_segments[0]
 
         # Is this a cast function call
         if function_name == "CAST":
             print("Found cast function!")
-            data_type_info = bracketed.get_child(
-                "data_type").raw.upper().strip()
+            data_type_info = bracketed.get_child("data_type").raw.upper().strip()
             if data_type_info == "INT":
                 # Here we know we have a possible one
                 expr = bracketed.get_child("expression")
                 print(f"Found expr {expr} - {expr.raw}")
                 # Replace cast(X as int) with int(X) TODO
                 return LintResult(
                     anchor=context.segment,
                     fixes=[
                         LintFix.replace(
                             function_name_id_seg,
-                            [
-                                function_name_id_seg.edit(
-                                    f"int({expr.raw})"
-                                )
-                            ],
+                            [function_name_id_seg.edit(f"int({expr.raw})")],
                         ),
                         LintFix.delete(
                             bracketed,
                         ),
                     ],
                 )
 
@@ -129,41 +140,42 @@
     groups = ("all",)
     crawl_behaviour = SegmentSeekerCrawler({"function"})
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Check for invalid format strs"""
         functional_context = FunctionalContext(context)
         children = functional_context.segment.children()
-        function_name_id_seg = children.first(sp.is_type("function_name")).children(
-        ).first(sp.is_type("function_name_identifier"))[0]
+        function_name_id_seg = (
+            children.first(sp.is_type("function_name"))
+            .children()
+            .first(sp.is_type("function_name_identifier"))[0]
+        )
         raw_function_name = function_name_id_seg.raw.upper().strip()
         function_name = raw_function_name.upper().strip()
         bracketed_segments = children.first(sp.is_type("bracketed"))
         bracketed = bracketed_segments[0]
 
         # Is this a cast function call
         if function_name == "FORMAT_STRING":
             print("Found format string function!")
-            format_str_seg = bracketed.get_child("expression").get_child("quoted_literal")
+            format_str_seg = bracketed.get_child("expression").get_child(
+                "quoted_literal"
+            )
             format_str = format_str_seg.raw
             # If we don't use the bad sequence just return right away.
             if "%0$" not in format_str:
                 return None
             else:
                 # Replace %0$ with %1$
                 return LintResult(
                     anchor=context.segment,
                     fixes=[
                         LintFix.replace(
                             format_str_seg,
-                            [
-                                format_str_seg.edit(
-                                    format_str.replace("%0$", "%1$")
-                                )
-                            ],
+                            [format_str_seg.edit(format_str.replace("%0$", "%1$"))],
                         ),
                     ],
                 )
 
         return None
 
 
@@ -186,20 +198,16 @@
         if type_name.startswith("char"):
             return LintResult(
                 anchor=context.segment,
                 description=f"char type found ({type_name}) in {context} see "
                 "https://spark.apache.org/docs/3.0.0/sql-migration-guide.html for migration"
                 "advice. In Spark 2.4 on non-Hive tables these were treated as strings so "
                 "rewritting to string.",
-                fixes=[
-                    LintFix.replace(
-                        context.segment,
-                        [
-                            CodeSegment(raw="string")
-                        ])])
+                fixes=[LintFix.replace(context.segment, [CodeSegment(raw="string")])],
+            )
         else:
             return None
 
 
 @document_groups
 @document_fix_compatible
 @document_configuration
@@ -217,44 +225,54 @@
     crawl_behaviour = SegmentSeekerCrawler({"property_name_identifier"})
     reserved = {"provider", "location", "owner"}
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Check for reserved properties being configured."""
         functional_context = FunctionalContext(context)
         property_name_segment = context.segment
-        property_name = property_name_segment.raw.lower().strip().lstrip(
-            '\"').rstrip('\"').lstrip('\'').rstrip('\'')
-        print(f"Called with context {context} with \"{property_name}\"")
-        if (property_name not in self.reserved):
+        property_name = (
+            property_name_segment.raw.lower()
+            .strip()
+            .lstrip('"')
+            .rstrip('"')
+            .lstrip("'")
+            .rstrip("'")
+        )
+        print(f'Called with context {context} with "{property_name}"')
+        if property_name not in self.reserved:
             print(f"Property: {property_name} is *ok*")
             return None
         else:
             # Reserved property found, lets check and see if we are in a "CREATE" which we can fix
             # or if we are in an "ALTER" which we can not automatically fix.
             create_or_alter_segment = context.parent_stack[-2]
             print(f"{dir(create_or_alter_segment)}")
-            if (create_or_alter_segment.is_type("alter_database_statement") or
-                create_or_alter_segment.is_type("alter_table_statement")):
+            if create_or_alter_segment.is_type(
+                "alter_database_statement"
+            ) or create_or_alter_segment.is_type("alter_table_statement"):
                 return LintResult(
                     anchor=context.segment,
                     description=f"Reserved table/db property {property_name} found in alter "
-                    " statement see " +
-                    "https://spark.apache.org/docs/3.0.0/sql-migration-guide.html for migration " +
-                    " advice." +
-                    "In Spark 2.4 these alter statements were (effectively) ignored so you can " +
-                    " likely delete it, automatically " +
-                    f"rewritten to \"legacy_{property_name}\".",
+                    " statement see "
+                    "https://spark.apache.org/docs/3.0.0/sql-migration-guide.html for migration "
+                    " advice."
+                    "In Spark 2.4 these alter statements were (effectively) ignored so you can "
+                    " likely delete it, automatically "
+                    f'rewritten to "legacy_{property_name}".',
                     fixes=[
                         LintFix.replace(
                             property_name_segment,
                             [
-                                property_name_segment.get_child("quoted_identifier").edit(
-                                    f"\"legacy_{property_name}\""
-                                )
-                            ])])
+                                property_name_segment.get_child(
+                                    "quoted_identifier"
+                                ).edit(f'"legacy_{property_name}"')
+                            ],
+                        )
+                    ],
+                )
             # Ok we know it's a create statement since it is not an alter :)
             parent_segment = context.parent_stack[-1]
             # Now we want to get the segments that are "bad" (e.g. we want to delete) and that is
             # everything from this segment up until either a comma segment or a endbracket segment.
             segments_to_remove = []
             edits = []
             property_value = None
@@ -262,45 +280,49 @@
             segments_to_remove = [property_name_segment]
             for segment in siblings_post:
                 # We want to keep the end bracket so check for it before adding to the list
                 if segment.is_type("end_bracket"):
                     break
                 segments_to_remove.append(segment)
                 if segment.is_type("quoted_literal"):
-                    property_value = segment.raw.strip().lstrip('\"').rstrip('\"')
+                    property_value = segment.raw.strip().lstrip('"').rstrip('"')
                 print(f"{segment} - {segment.get_type()}")
                 # We want to drop the comma so we do the check _after_ the ops
                 if segment.is_type("comma"):
                     break
             if len(parent_segment.get_children("property_name_identifier")) == 1:
                 # If there are no other properties besides the property we are going to delete then
                 # we need to drop the entire properties part to do this correctly, but "for now"
                 # as a hack we will just edit the property name to prepend "legacy_"
                 segments_to_remove = []
                 edits = [
                     LintFix.replace(
                         property_name_segment,
                         [
                             property_name_segment.get_child("quoted_identifier").edit(
-                                f"\"legacy_{property_name}\""
+                                f'"legacy_{property_name}"'
                             )
-                        ])]
+                        ],
+                    )
+                ]
             deletes = map(lambda t: LintFix.delete(t), segments_to_remove)
             new_statement = None
             if property_name == "provider":
                 new_segment = CodeSegment(raw=f" USING {property_value}")
                 print(functional_context.parent_stack)
                 create_table_segment = functional_context.parent_stack[-2]
                 # We want to insert after the first bracketed segment containing column_definition
                 # but if there are no column definitions we instead insert after the table
                 # identifier.
-                first_bracketed_segment = create_table_segment.get_child(
-                    "bracketed")
+                first_bracketed_segment = create_table_segment.get_child("bracketed")
                 print(dir(first_bracketed_segment))
-                if "column_definition" in first_bracketed_segment.direct_descendant_type_set:
+                if (
+                    "column_definition"
+                    in first_bracketed_segment.direct_descendant_type_set
+                ):
                     new_statement = LintFix.create_after(
                         first_bracketed_segment,
                         [new_segment],
                     )
                 else:
                     new_statement = LintFix.create_after(
                         create_table_segment.get_child("table_reference"),
@@ -309,86 +331,174 @@
             elif property_name == "location":
                 create_segment = functional_context.parent_stack[-2]
                 # We want to insert after the database reference (and comment if present) or before
                 # "TBLPROPERTIES" depending.
                 if "database_reference" in create_segment.direct_descendant_type_set:
                     new_statement = LintFix.create_after(
                         create_segment.get_child("database_reference"),
-                        [CodeSegment(raw=f" LOCATION \"{property_value}\"")],
+                        [CodeSegment(raw=f' LOCATION "{property_value}"')],
                     )
                 else:
                     keywords = create_segment.get_children("keyword")
                     tbl_properties_ref = next(
-                        iter(filter(lambda s: s.raw_upper == "TBLPROPERTIES", keywords)))
+                        iter(filter(lambda s: s.raw_upper == "TBLPROPERTIES", keywords))
+                    )
                     new_statement = LintFix.create_before(
                         tbl_properties_ref,
-                        [CodeSegment(raw=f"LOCATION \"{property_value}\" ")],
+                        [CodeSegment(raw=f'LOCATION "{property_value}" ')],
                     )
             else:
                 # For "owner" property we don't have an easy work around so instead just raise
                 # a lint error.
                 return LintResult(
                     anchor=context.segment,
-                    description=f"Reserved table/db property {property_name} found see " +
-                    "https://spark.apache.org/docs/3.0.0/sql-migration-guide.html for " +
+                    description=f"Reserved table/db property {property_name} found see "
+                    "https://spark.apache.org/docs/3.0.0/sql-migration-guide.html for "
                     "migration advice.",
-                    fixes=None)
+                    fixes=None,
+                )
             fixes = list(edits) + list(deletes) + [new_statement]
             return LintResult(
                 anchor=context.segment,
                 description="Reserved table property {property_name} found.",
-                fixes=fixes)
+                fixes=fixes,
+            )
             # TODO - Make a rewrite rule.
 
 
-# These two decorators allow plugins
-# to be displayed in the sqlfluff docs
-@document_groups
-@document_fix_compatible
-@document_configuration
-class Rule_Example_L001(BaseRule):
-    """ORDER BY on these columns is forbidden!
+class Rule_SPARKSQL_L004(BaseRule):
+    """Spark 3.0 extract second field returns DecimalType
 
-    **Anti-pattern**
+    Since Spark 3.0, when using EXTRACT expression to extract the
+    second field from date/timestamp values, the result will be a
+    DecimalType(8, 6) value with 2 digits for second part, and 6 digits
+    for the fractional part with microsecond precision. e.g.
+    extract(second from to_timestamp('2019-09-20 10:10:10.1')) results
+    10.100000. In Spark version 2.4 and earlier, it returns an IntegerType
+    value and the result for the former example is 10.
+    """
 
-    Using ``ORDER BY`` one some forbidden columns.
+    groups = ("all",)
+    crawl_behaviour = SegmentSeekerCrawler({"function"})
 
-    .. code-block:: sql
+    def _eval(self, context: RuleContext) -> Optional[LintResult]:
+        functional_context = FunctionalContext(context)
+        children = functional_context.segment.children()
+        function_name_id_seg = (
+            children.first(sp.is_type("function_name"))
+            .children()
+            .first(sp.is_type("function_name_identifier"))[0]
+        )
+        raw_function_name = function_name_id_seg.raw.upper().strip()
+        function_name = raw_function_name.upper().strip()
+        bracketed_segments = children.first(sp.is_type("bracketed"))
+        bracketed = bracketed_segments[0]
 
-        SELECT *
-        FROM foo
-        ORDER BY
-            bar,
-            baz
+        if function_name == "EXTRACT":
+            print("Found extract function!")
 
-    **Best practice**
+            parent_stack_reversed = functional_context.parent_stack.reversed()
+            if (
+                parent_stack_reversed[0].get_type() == "expression" and
+                parent_stack_reversed[1].get_type() == "bracketed" and
+                parent_stack_reversed[2].get_type() == "function"
+            ):
+                if parent_stack_reversed[2].segments[0].raw.upper().strip() == "CAST":
+                    return None
 
-    Do not order by these columns.
+            date_part_into = bracketed.get_child("date_part").raw.upper().strip()
+            if date_part_into == "SECOND":
+                edits = [
+                    KeywordSegment("cast"),
+                    SymbolSegment("(", type="start_bracket"),
+                    context.segment,
+                    WhitespaceSegment(),
+                    KeywordSegment("as"),
+                    WhitespaceSegment(),
+                    KeywordSegment("int"),
+                    SymbolSegment(")", type="end_bracket"),
+                ]
+                return LintResult(
+                    anchor=context.segment,
+                    fixes=[
+                        LintFix.replace(context.segment, edits),
+                    ],
+                )
 
-    .. code-block:: sql
+        return None
 
-        SELECT *
-        FROM foo
-        ORDER BY bar
+
+class Rule_SPARKSQL_L005(BaseRule):
+    """Spark 3.0 approx_percentile only accepts int type
+
+    In Spark 3.0, the function percentile_approx and its
+    alias approx_percentile only accept integral value with
+    range in [1, 2147483647] as its 3rd argument accuracy,
+    fractional and string types are disallowed, for example,
+    percentile_approx(10.0, 0.2, 1.8D) causes AnalysisException.
+    In Spark version 2.4 and below, if accuracy is fractional or
+    string value, it is coerced to an int value, percentile_approx(10.0, 0.2, 1.8D)
+    is operated as percentile_approx(10.0, 0.2, 1) which results in 10.0.
     """
 
     groups = ("all",)
-    config_keywords = ["forbidden_columns"]
-    crawl_behaviour = SegmentSeekerCrawler({"column_reference"})
+    crawl_behaviour = SegmentSeekerCrawler({"function"})
+    # is_fix_compatible = True
+
+    def _eval(self, context: RuleContext) -> Optional[LintResult]:
+        functional_context = FunctionalContext(context)
+        children = functional_context.segment.children()
+        function_name_id_seg = (
+            children.first(sp.is_type("function_name"))
+            .children()
+            .first(sp.is_type("function_name_identifier"))[0]
+        )
+        raw_function_name = function_name_id_seg.raw.upper().strip()
+        function_name = raw_function_name.upper().strip()
+        bracketed_segments = children.first(sp.is_type("bracketed"))
+
+        if function_name == "APPROX_PERCENTILE" or function_name == "PERCENTILE_APPROX":
+            print("Found approx function!")
 
-    def __init__(self, *args, **kwargs):
-        """Overwrite __init__ to set config."""
-        super().__init__(*args, **kwargs)
-        self.forbidden_columns = [
-            col.strip() for col in self.forbidden_columns.split(",")
-        ]
-
-    def _eval(self, context: RuleContext):
-        """We should not use ORDER BY."""
-        if context.segment.is_type("orderby_clause"):
-            for seg in context.segment.segments:
-                col_name = seg.raw.lower()
-                if col_name in self.forbidden_columns:
-                    return LintResult(
-                        anchor=seg,
-                        description=f"Column `{col_name}` not allowed in ORDER BY.",
+            expression_count = 0
+            expression_segment = None
+            for segment in bracketed_segments.children().iterate_segments(
+                sp.is_type("expression")
+            ):
+                expression_count += 1
+                if expression_count == 3:
+                    expression_segment = segment
+
+            if expression_segment is not None:
+                expression_child = expression_segment.children().first()
+                if expression_child[0].type == "function":
+                    function_name_id_seg = (
+                        expression_child.children()
+                        .first(sp.is_type("function_name"))
+                        .children()
+                        .first(sp.is_type("function_name_identifier"))[0]
                     )
+                    raw_function_name = function_name_id_seg.raw.upper().strip()
+                    function_name = raw_function_name.upper().strip()
+                    print(function_name)
+                    # If we see a cast then we know this was already fixed.
+                    if function_name == "CAST":
+                        return None
+                expression_child = expression_child[0]
+                edits = [
+                    KeywordSegment("cast"),
+                    SymbolSegment("(", type="start_bracket"),
+                    expression_child,
+                    WhitespaceSegment(),
+                    KeywordSegment("as"),
+                    WhitespaceSegment(),
+                    KeywordSegment("int"),
+                    SymbolSegment(")", type="end_bracket"),
+                ]
+                return LintResult(
+                    anchor=context.segment,
+                    fixes=[
+                        LintFix.replace(expression_child, edits),
+                    ],
+                )
+
+        return None
```

