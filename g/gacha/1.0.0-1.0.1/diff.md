# Comparing `tmp/gacha-1.0.0.tar.gz` & `tmp/gacha-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gacha-1.0.0.tar", max compression
+gzip compressed data, was "gacha-1.0.1.tar", max compression
```

## Comparing `gacha-1.0.0.tar` & `gacha-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2023-06-26 05:56:26.396065 gacha-1.0.0/LICENSE
--rw-r--r--   0        0        0      832 2023-06-26 07:29:28.252893 gacha-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2695 2023-06-26 07:29:40.913640 gacha-1.0.0/README.md
--rw-r--r--   0        0        0       95 2023-06-26 07:19:12.693042 gacha-1.0.0/src/gacha/__init__.py
--rw-r--r--   0        0        0     1580 2023-06-26 07:28:02.679171 gacha-1.0.0/src/gacha/banners.py
--rw-r--r--   0        0        0     1214 2023-06-26 07:27:55.422026 gacha-1.0.0/src/gacha/characters.py
--rw-r--r--   0        0        0     5197 2023-06-26 07:26:50.665553 gacha-1.0.0/src/gacha/engines.py
--rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 gacha-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-26 05:56:26.396065 gacha-1.0.1/LICENSE
+-rw-r--r--   0        0        0      833 2023-06-27 10:02:01.364486 gacha-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2695 2023-06-26 07:29:40.913640 gacha-1.0.1/README.md
+-rw-r--r--   0        0        0       95 2023-06-26 07:19:12.693042 gacha-1.0.1/src/gacha/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-27 09:59:13.401010 gacha-1.0.1/src/gacha/banners.py
+-rw-r--r--   0        0        0     1198 2023-06-27 09:53:07.487422 gacha-1.0.1/src/gacha/characters.py
+-rw-r--r--   0        0        0     5289 2023-06-27 10:01:21.549869 gacha-1.0.1/src/gacha/engines.py
+-rw-r--r--   0        0        0     3374 1970-01-01 00:00:00.000000 gacha-1.0.1/PKG-INFO
```

### Comparing `gacha-1.0.0/LICENSE` & `gacha-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gacha-1.0.0/pyproject.toml` & `gacha-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gacha"
-version = "1.0.0"
-description = "✨ Gacha"
+version = "1.0.1"
+description = "🔮 Gacha"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/gacha"
 repository = "https://github.com/elaresai/gacha"
 classifiers = [
```

### Comparing `gacha-1.0.0/README.md` & `gacha-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gacha-1.0.0/src/gacha/banners.py` & `gacha-1.0.1/src/gacha/banners.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,29 @@
     * `fallback` - Fallback of the banner
     * `name` - Name of the banner
     * `description` - Description of the banner
 
     # 🔎 Examples
     ```
     from gacha import Character, Banner
-    ...
+
     Banner(
         "Wanderlust_Invocation",
         characters=[
             Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean"),
             Character(0.003, name="Qiqi", description="https://genshin-impact.fandom.com/wiki/Qiqi"),
             Character(0.003, name="Tighnari", description="https://genshin-impact.fandom.com/wiki/Tighnari"),
             Character(0.003, name="Keqing", description="https://genshin-impact.fandom.com/wiki/Keqing"),
             Character(0.003, name="Mona", description="https://genshin-impact.fandom.com/wiki/Mona"),
             Character(0.003, name="Dehya", description="https://genshin-impact.fandom.com/wiki/Dehya"),
             Character(0.003, name="Diluc", description="https://genshin-impact.fandom.com/wiki/Diluc"),
-            ...
         ],
         name="Wanderlust_Invocation",
         description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation"
     )
-    ...
     ```
     """
 
     fallback: str
 
     characters: Optional[Sequence[Character]] = None
```

### Comparing `gacha-1.0.0/src/gacha/characters.py` & `gacha-1.0.1/src/gacha/characters.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,22 @@
     * `weight` - Relative weight of the character
     * `name` - Name of the character
     * `description` - Description of the character
 
     # 🔎 Examples
     ```
     from gacha import Character
-    ...
+
     Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean")
     Character(0.003, name="Qiqi", description="https://genshin-impact.fandom.com/wiki/Qiqi")
     Character(0.003, name="Tighnari", description="https://genshin-impact.fandom.com/wiki/Tighnari")
     Character(0.003, name="Keqing", description="https://genshin-impact.fandom.com/wiki/Keqing")
     Character(0.003, name="Mona", description="https://genshin-impact.fandom.com/wiki/Mona")
     Character(0.003, name="Dehya", description="https://genshin-impact.fandom.com/wiki/Dehya")
     Character(0.003, name="Diluc", description="https://genshin-impact.fandom.com/wiki/Diluc")
-    ...
     ```
     """
 
     weight: float
 
     name: Optional[str] = None
     description: Optional[str] = None
```

### Comparing `gacha-1.0.0/src/gacha/engines.py` & `gacha-1.0.1/src/gacha/engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,21 @@
     )
     ...
     ```
     """
 
     banners: Optional[Sequence[Banner]] = None
 
-    def roll(self, fallback: str) -> Character:
+    def roll(self, fallback: str, count: int = 1) -> list[Character]:
         """*roll*
 
         # Arguments
 
         * `fallback` - Fallback of the banner
+        * `count` - Count of the rolls
 
         # 🔎 Examples
         ```
         from gacha import Engine, Banner, Character
 
         engine = Engine(
             [
@@ -125,36 +126,38 @@
                             description="https://genshin-impact.fandom.com/wiki/Dehya",
                         ),
                         Character(
                             0.003,
                             name="Diluc",
                             description="https://genshin-impact.fandom.com/wiki/Diluc",
                         ),
-                        ...,
                     ],
                     name="Wanderlust_Invocation",
                     description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation",
                 ),
             ]
         )
 
         character = engine.roll()
 
         print(character.name)  # Jean
         print(character.description)  # https://genshin-impact.fandom.com/wiki/Jean
-
         ```
         """
+        k = count
+
         for banner in self.banners:
             if banner.fallback != fallback:
                 continue
 
             population = []
             weights = []
 
             for character in banner.characters:
                 weight = character.weight * MULTIPLIER
 
                 population.append(character)
                 weights.append(weight)
 
-            return choices(population, weights=weights)
+            return choices(population, weights=weights, k=k)
+
+        raise ValueError(fallback)
```

### Comparing `gacha-1.0.0/PKG-INFO` & `gacha-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gacha
-Version: 1.0.0
-Summary: ✨ Gacha
+Version: 1.0.1
+Summary: 🔮 Gacha
 Home-page: https://github.com/elaresai/gacha
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
 Requires-Python: >=3.8.0,<3.12
```

