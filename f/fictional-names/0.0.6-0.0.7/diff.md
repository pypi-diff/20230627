# Comparing `tmp/fictional_names-0.0.6.tar.gz` & `tmp/fictional_names-0.0.7.tar.gz`

## Comparing `fictional_names-0.0.6.tar` & `fictional_names-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,37 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.6/LISENCE
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/dwarven.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/elven.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/giant.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/halfling.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_arab.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_erikson.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_greek.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_jordan.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_medieval.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_modern.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_norsemen.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_oriental.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_rowling.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_sapkowski.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_steampunk.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_tolkien.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/name_generator.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/orc.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/supportive_functions.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/.vscode/settings.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fictional_names-0.0.6/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fictional_names-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fictional_names-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.7/__init__.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/__init__.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/arab.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/aztec.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/chinese.py
+-rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/dwarven.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/elven.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/english.py
+-rw-r--r--   0        0        0    15039 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/erikson.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/germanic.py
+-rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/giant.py
+-rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/greek.py
+-rw-r--r--   0        0        0     9660 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/halfling.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/human.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/japanese.py
+-rw-r--r--   0        0        0    14700 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/jordan.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/martin.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/mongolian.py
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/name_generator.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/norsemen.py
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/orc.py
+-rw-r--r--   0        0        0    14194 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/roman.py
+-rw-r--r--   0        0        0    20726 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/rowling.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/sapkowski.py
+-rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/slavic.py
+-rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/steampunk.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/supportive_functions.py
+-rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/tolkien.py
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/turkish.py
+-rw-r--r--   0        0        0    15480 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/viking.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.7/src/fictional_names/.vscode/settings.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.7/LICENSE
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.7/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fictional_names-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fictional_names-0.0.7/PKG-INFO
```

### Comparing `fictional_names-0.0.6/LISENCE` & `fictional_names-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.6/src/fictional_names/.gitignore` & `fictional_names-0.0.7/src/fictional_names/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -156,8 +156,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Custom
-/tester.py
+/loop.ps1
```

### Comparing `fictional_names-0.0.6/src/fictional_names/supportive_functions.py` & `fictional_names-0.0.7/src/fictional_names/supportive_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 def generate_female_name(female_prefix, female_suffix, min=1, max=2):
     while True:
         try:
             num_prefix_syllables = randint(min, max)
             num_suffix_syllables = randint(min, max)
             if num_prefix_syllables == 0 and num_suffix_syllables == 0:
                 raise ValueError
-            
-            if (num_prefix_syllables == 1 and num_suffix_syllables == 0):
+
+            if num_prefix_syllables == 1 and num_suffix_syllables == 0:
                 name = choice(female_prefix)
                 return name.capitalize()
 
             name = ""
             for _ in range(num_prefix_syllables):
                 syllable = choice(female_prefix)
                 name += syllable
-            
+
             for _ in range(num_suffix_syllables):
                 syllable = choice(female_suffix)
                 name += syllable
-            
+
             return name.capitalize()
         except ValueError:
             continue
 
 
 def generate_male_name(male_prefix, male_suffix, min=1, max=2):
     while True:
         try:
             num_prefix_syllables = randint(min, max)
             num_suffix_syllables = randint(min, max)
             if num_prefix_syllables == 0 and num_suffix_syllables == 0:
                 raise ValueError
-            
-            if (num_prefix_syllables == 1 and num_suffix_syllables == 0):
+
+            if num_prefix_syllables == 1 and num_suffix_syllables == 0:
                 name = choice(male_prefix)
                 return name.capitalize()
 
             name = ""
             for _ in range(num_prefix_syllables):
                 syllable = choice(male_prefix)
                 name += syllable
-            
+
             for _ in range(num_suffix_syllables):
                 syllable = choice(male_suffix)
                 name += syllable
-            
+
             return name.capitalize()
         except ValueError:
             continue
 
 
 def generate_surname(surname_syllables, min=1, max=3):
     num_syllables = randint(min, max)
@@ -64,29 +64,25 @@
 
 
 def generate_surname_less(surname_prefix, surname_suffix):
     synth_surname = ""
     syllable_prefix = choice(surname_prefix)
     syllable_suffix = choice(surname_suffix)
     synth_surname += syllable_prefix + syllable_suffix
-    
+
     return synth_surname.capitalize()
 
 
-def remove_duplicates(female_names, male_names, surnames):
+def remove_duplicates(namelist):
     # Remove duplicates
-    female = list(set(female_names))
-    male = list(set(male_names))
-    surname = list(set(surnames))
+    namelist_ordered = list(set(namelist))
 
     # Sort alphabetically
-    female.sort()
-    male.sort()
-    surname.sort()
-
-    all_lists = {
-        'female': female,
-        'male': male,
-        'surname': surname
-    }
-    
-    return all_lists
+    namelist_ordered.sort()
+
+    return namelist_ordered
+
+
+# print(remove_duplicates(surnames))
+
+# for name in female_names:
+#     print("'", name.capitalize(), "'", sep='', end=', ')
```

### Comparing `fictional_names-0.0.6/pyproject.toml` & `fictional_names-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fictional_names"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="a-tsagkalidis", email="arg.tsag@gmail.com" },
 ]
 description = "A package for generating fictional names"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

