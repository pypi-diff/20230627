# Comparing `tmp/symcirc-0.0.8-py3-none-any.whl.zip` & `tmp/symcirc-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12773 bytes, number of entries: 11
+Zip file size: 12796 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat       96 b- defN 22-Apr-21 09:44 symcirc/__init__.py
--rw-rw-rw-  2.0 fat    22127 b- defN 22-Aug-26 11:19 symcirc/analysis.py
+-rw-rw-rw-  2.0 fat    22208 b- defN 22-Aug-30 08:35 symcirc/analysis.py
 -rw-rw-rw-  2.0 fat     7557 b- defN 22-Jun-30 09:54 symcirc/component.py
 -rw-rw-rw-  2.0 fat     6072 b- defN 22-Aug-25 09:29 symcirc/laplace.py
--rw-rw-rw-  2.0 fat    17640 b- defN 22-Aug-26 11:25 symcirc/parse.py
+-rw-rw-rw-  2.0 fat    17720 b- defN 22-Aug-30 08:30 symcirc/parse.py
 -rw-rw-rw-  2.0 fat      839 b- defN 22-Jun-27 15:56 symcirc/utils.py
--rw-rw-rw-  2.0 fat     1088 b- defN 22-Aug-26 11:28 symcirc-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1043 b- defN 22-Aug-26 11:28 symcirc-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-26 11:28 symcirc-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 22-Aug-26 11:28 symcirc-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      834 b- defN 22-Aug-26 11:28 symcirc-0.0.8.dist-info/RECORD
-11 files, 57396 bytes uncompressed, 11381 bytes compressed:  80.2%
+-rw-rw-rw-  2.0 fat     1088 b- defN 22-Aug-30 08:36 symcirc-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1043 b- defN 22-Aug-30 08:36 symcirc-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-30 08:36 symcirc-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 22-Aug-30 08:36 symcirc-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      834 b- defN 22-Aug-30 08:36 symcirc-0.0.9.dist-info/RECORD
+11 files, 57557 bytes uncompressed, 11404 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: symcirc/parse.py
 Comment: 
 
 Filename: symcirc/utils.py
 Comment: 
 
-Filename: symcirc-0.0.8.dist-info/LICENSE
+Filename: symcirc-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: symcirc-0.0.8.dist-info/METADATA
+Filename: symcirc-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: symcirc-0.0.8.dist-info/WHEEL
+Filename: symcirc-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: symcirc-0.0.8.dist-info/top_level.txt
+Filename: symcirc-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: symcirc-0.0.8.dist-info/RECORD
+Filename: symcirc-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## symcirc/analysis.py

```diff
@@ -65,14 +65,16 @@
 
           :return dict ret: in format {"v(id1)" : value, "i(id2)" : value, ...}
         """
         ret = {}
         for key in self.components:
             if self.components[key].type == "k":
                 pass
+            elif self.components[key].name[-3:] == "_IC":
+                pass
             else:
                 name = self.components[key].name
                 val = self.component_values(name)
                 ret.update(val)
         return ret
 
     def node_voltages(self):
```

## symcirc/parse.py

```diff
@@ -343,15 +343,15 @@
                     init_cond, _ = convert_units(words[4][3:])
                     c = Capacitor(name, variant, node1, node2, sym_value=sym_value, init_cond=init_cond, value=value)
                 except IndexError:
                     #print("No initial condition set for {}".format(name))
                     init_cond = 0
                     c = Capacitor(name, variant, node1, node2, sym_value=sym_value, value=value)
                 if tran:
-                    ic = CurrentSource(name + "_IC", "i", node2, node1, sym_value=init_cond*sym_value, dc_value=init_cond*value)
+                    ic = CurrentSource(name + "_IC", "i", node2, node1, sym_value=init_cond*sym_value, dc_value=init_cond*value, ac_value=0, tran_value=init_cond*value)
                     independent_sources.append(ic)
                     components[ic.name] = ic
                 basic_components.append(c)
 
 
             elif name[0] in ["l", "L"]:
                 variant = "l"
@@ -364,15 +364,15 @@
                     init_cond, _ = convert_units(words[4][3:])
                     c = Inductor(name, variant, node1, node2, sym_value=sym_value, init_cond=init_cond, value=value)
                 except IndexError:
                     #print("No initial condition set for {}".format(name))
                     init_cond = 0
                     c = Inductor(name, variant, node1, node2, sym_value=sym_value, value=value)
                 if tran:
-                    ic = CurrentSource(name + "_IC", "i", node1, node2, sym_value=init_cond*sym_value, dc_value=init_cond*value)
+                    ic = CurrentSource(name + "_IC", "i", node1, node2, sym_value=init_cond*sym_value, dc_value=init_cond*value, ac_value=0, tran_value=init_cond*value)
                     independent_sources.append(ic)
                     components[ic.name] = ic
                 basic_components.append(c)
 
             elif name[0] in ["a", "A"]:
                 variant = "a"
                 sym_value = sympy.Symbol(name, real=True)
```

## Comparing `symcirc-0.0.8.dist-info/LICENSE` & `symcirc-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `symcirc-0.0.8.dist-info/METADATA` & `symcirc-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symcirc
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for symbolic electronic circuit analysis
 Home-page: https://github.com/MatyasVasek/SymCirc
 Author: Matyas Vasek
 Author-email: matyas.vasek@gmail.com
 License: MIT license
 Project-URL: Bug Tracker, https://github.com/MatyasVasek/SymCirc/issues
 Platform: UNKNOWN
```

## Comparing `symcirc-0.0.8.dist-info/RECORD` & `symcirc-0.0.9.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 symcirc/__init__.py,sha256=6cg1X9GcKPlNU6op1wowcj9fUS7dCKd-dQj1HqWhnu8,96
-symcirc/analysis.py,sha256=Kb9PKlG8zC-v5Cgi8JQ0PEzQJc-UHpA6MPQow4X9BYE,22127
+symcirc/analysis.py,sha256=pubaY3xCu7GFdtqfT_2645w6NgwRvzB1orvDi88hrIA,22208
 symcirc/component.py,sha256=2GCOvb5tVFd6rIoxTAmK28wX6fOreQEg3zxud-GJ914,7557
 symcirc/laplace.py,sha256=w60lVfU6F9Vmn-8ejEEt1SNIqIzycGOE6inj3hp-Dqs,6072
-symcirc/parse.py,sha256=iyp8YAfP0f2B1fBD288na4CGPL2AXZMlaRWW25B5b0Y,17640
+symcirc/parse.py,sha256=fF8eHEnpavdvxm7pmesAxrT4-hoLDsOOb5MQiFwcdy8,17720
 symcirc/utils.py,sha256=cknOhZAToXaJk85IV_nH0llOobR12v4PqICiUBbUUp4,839
-symcirc-0.0.8.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
-symcirc-0.0.8.dist-info/METADATA,sha256=jurXUCHECxmrC74gQOLcHU8OwvnveCwPgmA_uDMlyxA,1043
-symcirc-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-symcirc-0.0.8.dist-info/top_level.txt,sha256=9OnmgAf4G3r0me_isCye9UkVPJfWuECjpB7ehnWhWBo,8
-symcirc-0.0.8.dist-info/RECORD,,
+symcirc-0.0.9.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
+symcirc-0.0.9.dist-info/METADATA,sha256=vNZUC4XRt763sD8J7GILTvQjeIZ6L3RKa09MBYRwPdE,1043
+symcirc-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+symcirc-0.0.9.dist-info/top_level.txt,sha256=9OnmgAf4G3r0me_isCye9UkVPJfWuECjpB7ehnWhWBo,8
+symcirc-0.0.9.dist-info/RECORD,,
```

