# Comparing `tmp/linpg-3.6.1.tar.gz` & `tmp/linpg-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linpg-3.6.1.tar", last modified: Sat May 27 21:37:45 2023, max compression
+gzip compressed data, was "linpg-3.7.0.tar", last modified: Mon Jun 26 22:31:08 2023, max compression
```

## Comparing `linpg-3.6.1.tar` & `linpg-3.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.453575 linpg-3.6.1/
--rw-rw-rw-   0        0        0    35823 2022-10-03 22:43:03.000000 linpg-3.6.1/LICENSE
--rw-rw-rw-   0        0        0    10383 2023-05-27 21:37:45.453575 linpg-3.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     9785 2023-05-22 02:03:32.000000 linpg-3.6.1/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-27 20:11:37.000000 linpg-3.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      134 2023-05-27 21:37:45.454575 linpg-3.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.349518 linpg-3.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.418516 linpg-3.6.1/src/linpg/
--rw-rw-rw-   0        0        0     5350 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0    35823 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/LICENSE
--rw-rw-rw-   0        0        0     9785 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/README.md
--rw-rw-rw-   0        0        0    31232 2023-05-27 21:37:11.000000 linpg-3.6.1/src/linpg/__init__.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0       44 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.428521 linpg-3.6.1/src/linpg/__pyinstaller/
--rw-rw-rw-   0        0        0       90 2023-05-27 19:47:31.000000 linpg-3.6.1/src/linpg/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      984 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/__pyinstaller/hook-linpg.py
--rw-rw-rw-   0        0        0   105472 2023-05-27 21:37:11.000000 linpg-3.6.1/src/linpg/abstracts.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     2035 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/abstracts.pyi
--rw-rw-rw-   0        0        0   760832 2023-05-27 21:37:17.000000 linpg-3.6.1/src/linpg/basic.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    15860 2023-05-27 21:37:19.000000 linpg-3.6.1/src/linpg/basic.pyi
--rw-rw-rw-   0        0        0   850944 2023-05-27 21:37:15.000000 linpg-3.6.1/src/linpg/battle.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     9179 2023-05-27 21:37:16.000000 linpg-3.6.1/src/linpg/battle.pyi
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.436521 linpg-3.6.1/src/linpg/config/
--rw-rw-rw-   0        0        0   212992 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/config/__init__.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     3270 2023-05-27 21:37:14.000000 linpg-3.6.1/src/linpg/config/__init__.pyi
--rw-rw-rw-   0        0        0     2267 2023-05-23 20:46:36.000000 linpg-3.6.1/src/linpg/config/specifications.json
--rw-rw-rw-   0        0        0    24762 2023-05-23 20:46:36.000000 linpg-3.6.1/src/linpg/config/ui.json
--rw-rw-rw-   0        0        0   971264 2023-05-27 21:37:21.000000 linpg-3.6.1/src/linpg/core.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    18561 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/core.pyi
--rw-rw-rw-   0        0        0   948736 2023-05-27 21:37:17.000000 linpg-3.6.1/src/linpg/dialogue.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     7413 2023-05-27 21:37:18.000000 linpg-3.6.1/src/linpg/dialogue.pyi
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.441574 linpg-3.6.1/src/linpg/doc/
--rw-rw-rw-   0        0        0      827 2022-10-03 22:30:39.000000 linpg-3.6.1/src/linpg/doc/CN1_简介.md
--rw-rw-rw-   0        0        0     3098 2022-10-03 22:30:39.000000 linpg-3.6.1/src/linpg/doc/CN2_入门.md
--rw-rw-rw-   0        0        0     1002 2022-10-03 22:43:03.000000 linpg-3.6.1/src/linpg/doc/EN1_Introduction.md
--rw-rw-rw-   0        0        0       12 2022-10-03 22:30:39.000000 linpg-3.6.1/src/linpg/doc/Home.md
--rw-rw-rw-   0        0        0    77312 2023-05-27 21:37:11.000000 linpg-3.6.1/src/linpg/exception.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      797 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/exception.pyi
--rw-rw-rw-   0        0        0    83456 2023-05-27 21:37:11.000000 linpg-3.6.1/src/linpg/interface.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     1759 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/interface.pyi
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.451574 linpg-3.6.1/src/linpg/language/
--rw-rw-rw-   0        0        0     3157 2023-05-23 20:46:36.000000 linpg-3.6.1/src/linpg/language/English.json
--rw-rw-rw-   0        0        0     3087 2023-05-23 20:46:36.000000 linpg-3.6.1/src/linpg/language/SimplifiedChinese.json
--rw-rw-rw-   0        0        0     3087 2023-05-23 20:46:36.000000 linpg-3.6.1/src/linpg/language/TraditionalChinese.json
--rw-rw-rw-   0        0        0    91136 2023-05-27 21:37:12.000000 linpg-3.6.1/src/linpg/language/__init__.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      729 2023-05-27 21:37:14.000000 linpg-3.6.1/src/linpg/language/__init__.pyi
--rw-rw-rw-   0        0        0      119 2023-05-27 21:37:22.000000 linpg-3.6.1/src/linpg/py.typed
--rw-rw-rw-   0        0        0  1160704 2023-05-27 21:37:19.000000 linpg-3.6.1/src/linpg/ui.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    13204 2023-05-27 21:37:20.000000 linpg-3.6.1/src/linpg/ui.pyi
-drwxrwxrwx   0        0        0        0 2023-05-27 21:37:45.426521 linpg-3.6.1/src/linpg.egg-info/
--rw-rw-rw-   0        0        0    10383 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1383 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 21:37:45.000000 linpg-3.6.1/src/linpg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.764761 linpg-3.7.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-05 02:44:16.000000 linpg-3.7.0/LICENSE
+-rw-rw-rw-   0        0        0    10411 2023-06-26 22:31:08.765261 linpg-3.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9813 2023-06-26 22:11:24.000000 linpg-3.7.0/README.md
+-rw-rw-rw-   0        0        0     1293 2023-06-26 22:27:43.000000 linpg-3.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0      134 2023-06-26 22:31:08.765761 linpg-3.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.693249 linpg-3.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.746760 linpg-3.7.0/src/linpg/
+-rw-rw-rw-   0        0        0     5350 2023-06-26 22:30:56.000000 linpg-3.7.0/src/linpg/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0    35823 2023-06-26 22:30:56.000000 linpg-3.7.0/src/linpg/LICENSE
+-rw-rw-rw-   0        0        0     9813 2023-06-26 22:30:56.000000 linpg-3.7.0/src/linpg/README.md
+-rw-rw-rw-   0        0        0    30720 2023-06-26 22:30:29.000000 linpg-3.7.0/src/linpg/__init__.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0       44 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.752761 linpg-3.7.0/src/linpg/__pyinstaller/
+-rw-rw-rw-   0        0        0       90 2023-06-07 17:25:45.000000 linpg-3.7.0/src/linpg/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-06-26 22:30:56.000000 linpg-3.7.0/src/linpg/__pyinstaller/hook-linpg.py
+-rw-rw-rw-   0        0        0   107008 2023-06-26 22:30:29.000000 linpg-3.7.0/src/linpg/abstracts.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0     2035 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/abstracts.pyi
+-rw-rw-rw-   0        0        0   763392 2023-06-26 22:30:51.000000 linpg-3.7.0/src/linpg/basic.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0    15860 2023-06-26 22:30:53.000000 linpg-3.7.0/src/linpg/basic.pyi
+-rw-rw-rw-   0        0        0   913920 2023-06-26 22:30:51.000000 linpg-3.7.0/src/linpg/battle.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0     9787 2023-06-26 22:30:52.000000 linpg-3.7.0/src/linpg/battle.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.757260 linpg-3.7.0/src/linpg/config/
+-rw-rw-rw-   0        0        0   215552 2023-06-26 22:30:31.000000 linpg-3.7.0/src/linpg/config/__init__.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0     3270 2023-06-26 22:30:31.000000 linpg-3.7.0/src/linpg/config/__init__.pyi
+-rw-rw-rw-   0        0        0     2267 2023-06-26 03:45:44.000000 linpg-3.7.0/src/linpg/config/specifications.json
+-rw-rw-rw-   0        0        0    25748 2023-06-26 03:45:44.000000 linpg-3.7.0/src/linpg/config/ui.json
+-rw-rw-rw-   0        0        0   971776 2023-06-26 22:30:55.000000 linpg-3.7.0/src/linpg/core.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0    18561 2023-06-26 22:30:55.000000 linpg-3.7.0/src/linpg/core.pyi
+-rw-rw-rw-   0        0        0   928256 2023-06-26 22:30:49.000000 linpg-3.7.0/src/linpg/dialogue.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0     7417 2023-06-26 22:30:50.000000 linpg-3.7.0/src/linpg/dialogue.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.759760 linpg-3.7.0/src/linpg/doc/
+-rw-rw-rw-   0        0        0      827 2023-06-05 02:44:16.000000 linpg-3.7.0/src/linpg/doc/CN1_简介.md
+-rw-rw-rw-   0        0        0     3098 2023-06-05 02:44:16.000000 linpg-3.7.0/src/linpg/doc/CN2_入门.md
+-rw-rw-rw-   0        0        0     1002 2023-06-05 02:44:16.000000 linpg-3.7.0/src/linpg/doc/EN1_Introduction.md
+-rw-rw-rw-   0        0        0       12 2023-06-05 02:44:16.000000 linpg-3.7.0/src/linpg/doc/Home.md
+-rw-rw-rw-   0        0        0    78848 2023-06-26 22:30:29.000000 linpg-3.7.0/src/linpg/exception.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0      797 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/exception.pyi
+-rw-rw-rw-   0        0        0    84992 2023-06-26 22:30:29.000000 linpg-3.7.0/src/linpg/interface.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0     1759 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/interface.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.764261 linpg-3.7.0/src/linpg/language/
+-rw-rw-rw-   0        0        0     3229 2023-06-26 03:45:44.000000 linpg-3.7.0/src/linpg/language/English.json
+-rw-rw-rw-   0        0        0     3155 2023-06-26 03:45:44.000000 linpg-3.7.0/src/linpg/language/SimplifiedChinese.json
+-rw-rw-rw-   0        0        0     3155 2023-06-26 03:45:44.000000 linpg-3.7.0/src/linpg/language/TraditionalChinese.json
+-rw-rw-rw-   0        0        0    92672 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/language/__init__.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0      729 2023-06-26 22:30:30.000000 linpg-3.7.0/src/linpg/language/__init__.pyi
+-rw-rw-rw-   0        0        0      119 2023-06-26 22:30:56.000000 linpg-3.7.0/src/linpg/py.typed
+-rw-rw-rw-   0        0        0  1165312 2023-06-26 22:30:53.000000 linpg-3.7.0/src/linpg/ui.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0    13204 2023-06-26 22:30:54.000000 linpg-3.7.0/src/linpg/ui.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 22:31:08.751261 linpg-3.7.0/src/linpg.egg-info/
+-rw-rw-rw-   0        0        0    10411 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1383 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 22:31:08.000000 linpg-3.7.0/src/linpg.egg-info/top_level.txt
```

### Comparing `linpg-3.6.1/LICENSE` & `linpg-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/PKG-INFO` & `linpg-3.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,87 @@
 Metadata-Version: 2.1
 Name: linpg
-Version: 3.6.1
+Version: 3.7.0
 Summary: A game engine based on pygame, which aims to make game development easier.
 Author-email: Linpg Foundation <yudong9912@gmail.com>
 Project-URL: Homepage, https://github.com/LinpgFoundation/linpg
 Project-URL: Bug Tracker, https://github.com/LinpgFoundation/linpg/issues
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # :speech_balloon: Preamble / 前言
 
 ###### *"Just because c++ is the greatest language ever invented doesn't mean that writing games in c++ is easy and fun, and the same goes for pygame."*
 
-###### *"c++是有史以来最伟大的语言，但并不代表用c++写游戏是一件很轻松有趣的事情，pygame也是如此。"*
+###### *"c++是有史以来最伟大的语言，但这并不代表用c++写游戏是一件轻松而又有趣的事情，pygame也是如此。"*
 
 
 
 # :sparkles: About Linpg Engine / 关于Linpg引擎
 
-Linpg Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
+Linpg (Lin's python game) Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
 
 Linpg Engine is developed with a modular concept. It implements many features which are commonly used in game development. Simultaneously, the Linpg Engine also maintains a high level of compatibility with Pygame, making it easy for developers to migrate existing Pygame projects to Linpg Engine or use the features which Linpg Engine provides on their own Pygame projects.
 
 We always need your help to make Linpg the best it can be! No matter who you are, any contributors are welcome!
 
 Linpg引擎是Linpg基金会基于pygame库自主研发的游戏引擎，目的是为了规范化pygame游戏的开发，使得游戏代码更加整洁，易读，易扩展，易维护。
 
 Linpg引擎的开发使用了模块化的理念，并在底层实现了很多游戏开发过程中常用到的功能。Linpg引擎一直保持着与pygame高度的兼容性，使得开发者可以很容易将现有的pygame项目迁移到Linpg引擎上，或者在自己的pygame项目中使用Linpg引擎提供的功能或者工具。
 
 世上无完人，我们需要你的帮助让Linpg引擎变得更好。欢迎任何能帮助我们改进Linpg引擎的开发者！
 
 
 
+# :crystal_ball:Some awesome games developed using Linpg
+
+![](https://github.com/LinpgFoundation/A-story-of-us/raw/master/Assets/image/screenshot/dialog.png)
+
+#### [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us), a visual novel game only contains around 100 lines of code. A great starting point for anyone who is interested in Linpg.
+
+![](https://github.com/TigeiaWorkshop/GFL-LastWish/raw/master/Assets/image/screenshot/battle.png)
+
+#### [GFL-Last](https://github.com/TigeiaWorkshop/GFL-LastWish ), a turn-based strategy game that demonstrates some advanced features and the unlimited potential of the Linpg engine.
+
+
+
 # :hammer_and_wrench: Dependencies / 运行库 
 
 | Required / 必需安装 |
 | :---------- |
-| pygame      |
+| pygame-ce   |
 | numpy       |
 | PySimpleGUI |
 
 | Recommended* / 建议安装* |
 | ------------------------ |
 | pyyaml                   |
 | opencv                   |
-| tcod                     |
 
-***Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.***
+\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
 
-##### ***感谢这些库的开发者，他（她）们让使用python开发游戏不再遥远。***
+##### Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.
 
-\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
+##### 感谢这些第三方库的开发者，他（她）们让使用python开发游戏不再遥远。
 
 
 
 # :computer:Installation / 安装
 
 ### Recommend:
 
 ```
 pip install linpg
 ```
 
-We also highly suggest you download and use [https://github.com/LinpgFoundation/A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
+We also highly suggest you download and use [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
 
 ### Building From Source:
 
 First, clone this repo:
 
 ```
 git clone https://github.com/LinpgFoundation/linpg
@@ -90,63 +101,46 @@
 
 Run `builder.py`:
 
 ```
 python builder.py
 ```
 
-Enjoy!
-
+That's it, enjoy!
 
 
 # :world_map: Branches / 分支​
 
 ### master:
 
-This branch holds the current stable version. 
+The current stable version. 
 
 该分支提供了当前的稳定版本
 
 ### dev:
 
-This branch holds the latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that may cause harm to your system or projects. This version is typically recommended for experienced developers.
-
-目前可以运行的最新版本，可能在修复了部分现有的bug的同时，又带有新增的bug。 推荐开发人员使用
-
-### * in-process:
-
-**DON'T USE THIS BRANCH!** This branch contains a version that is currently unfinished.
-
-还未完成，无法运行的版本，请勿使用
-
-### * exp:
-
-**DON'T USE THIS BRANCH!**  This branch contains a version that is still in the experimental stage.
-
-实验版本，包含了部分仍在试验阶段的内容，请勿使用
-
-
+The latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that can cause harm to your system or projects. This version is typically recommended for experienced developers.
 
-*: These branches may not be available to the public.
+目前可以运行的最新版本，相对稳定，但可能包含未被发现的问题或未完善的功能。 推荐有经验的开发人员使用。
 
 
 
 # :books: How to contribute / 如何贡献代码
 
 - It would be best if you can fork the "dev" branch as your starting point. If the "dev" branch does not exist, then fork the "master" branch.
 
   你应该fork "dev"分支作为作为你的起始点。如果"dev"分支不存在，则fork "master"分支。
 
 - After you have finished your work, you should request to merge to the "dev" branch instead of the "master" branch.
 
-  所有pull request应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
+  所有PR应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
 
 - We are looking forward to seeing a pull request that contains a detailed explanation about any changes that were made.
 
-  所有pull request应该阐明所有关于改动的细节。
+  所有PR应该详细地阐明其做出的改动。
 
 
 
 # :video_game: ​Discord
 
 https://discord.gg/3wz6bs5jvu
 
@@ -181,15 +175,15 @@
 | ----------------------------------------------------------- | ------------------------------------ | ------------------ |
 | A more modular and aesthetically modern visual novel system | 更加模块化和美观现代化的视觉小说系统 | :white_check_mark: |
 | Options menu                                                | 选项菜单模块                         | :white_check_mark: |
 | Better and more complex combat system                       | 更加完善复杂的战斗系统               | :white_check_mark: |
 | Map Editor                                                  | 可用的地图编辑器                     | :white_check_mark: |
 | Dialogue Editor                                             | 可用的对话编辑器                     | :white_check_mark: |
 | Most functions work when correct input is accepted          | 大部分功能能在接受正确的输入后工作   | :hammer:         |
-| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统保持60帧       | :white_check_mark: |
+| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统达到144帧       | :white_check_mark: |
 | Video can be played at a stable 60 fps                      | 视频能稳定地以60帧播放               | :white_check_mark: |
 | Pygame native input box (English only)                      | 可用的pygame原生输入框（仅支持英文） | :white_check_mark: |
 
 ------
 
 | Linpg 4 |( On Schedule / 未来-计划中 )||
 | ------------------------------------------------------------ | -------------------------------------------------------- | ---- |
@@ -197,18 +191,17 @@
 | Rewrite using a combination of c++ and cython for better performance | 底层采用c++和cython结合的方式重写以获取更高效的性能      |      |
 | Better options menu                                          | 更好的选项菜单模块                                       |      |
 | Enemy AI systems will be partially affected by machine learning. | 敌方AI系统将部分采用machine learning的意见               |      |
 | More convenient and beautiful map editor and dialogue editor | 更加便捷美观的地图编辑器和对话编辑器                     |      |
 | More readable and standardized code                          | 更加易读规范化的代码                                     |      |
 | Most functions are able to report errors and take the most appropriate approach after accepting incorrect input | 大部分功能能在接受错误的输入后报错并采取最合适的方案运行 |      |
 | The combat system can have more varieties.                   | 战斗系统能有更多的玩法                                   |      |
-| Visual novel system and combat system can reach 144 fps      | 视觉小说系统和战斗系统达到144帧                          |      |
 | The input box will support Chinese, Japanese, and more       | 输入框支持中文，日文，以及更多                           |      |
 
 
 
 
 # :memo: License / 版权说明
 
-Please check LICENSE.
+Please check **LICENSE**.
 
-版权信息请查看LICENSE文件。
+版权信息请查看**LICENSE**文件。
```

### Comparing `linpg-3.6.1/README.md` & `linpg-3.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 # :speech_balloon: Preamble / 前言
 
 ###### *"Just because c++ is the greatest language ever invented doesn't mean that writing games in c++ is easy and fun, and the same goes for pygame."*
 
-###### *"c++是有史以来最伟大的语言，但并不代表用c++写游戏是一件很轻松有趣的事情，pygame也是如此。"*
+###### *"c++是有史以来最伟大的语言，但这并不代表用c++写游戏是一件轻松而又有趣的事情，pygame也是如此。"*
 
 
 
 # :sparkles: About Linpg Engine / 关于Linpg引擎
 
-Linpg Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
+Linpg (Lin's python game) Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
 
 Linpg Engine is developed with a modular concept. It implements many features which are commonly used in game development. Simultaneously, the Linpg Engine also maintains a high level of compatibility with Pygame, making it easy for developers to migrate existing Pygame projects to Linpg Engine or use the features which Linpg Engine provides on their own Pygame projects.
 
 We always need your help to make Linpg the best it can be! No matter who you are, any contributors are welcome!
 
 Linpg引擎是Linpg基金会基于pygame库自主研发的游戏引擎，目的是为了规范化pygame游戏的开发，使得游戏代码更加整洁，易读，易扩展，易维护。
 
 Linpg引擎的开发使用了模块化的理念，并在底层实现了很多游戏开发过程中常用到的功能。Linpg引擎一直保持着与pygame高度的兼容性，使得开发者可以很容易将现有的pygame项目迁移到Linpg引擎上，或者在自己的pygame项目中使用Linpg引擎提供的功能或者工具。
 
 世上无完人，我们需要你的帮助让Linpg引擎变得更好。欢迎任何能帮助我们改进Linpg引擎的开发者！
 
 
 
+# :crystal_ball:Some awesome games developed using Linpg
+
+![](https://github.com/LinpgFoundation/A-story-of-us/raw/master/Assets/image/screenshot/dialog.png)
+
+#### [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us), a visual novel game only contains around 100 lines of code. A great starting point for anyone who is interested in Linpg.
+
+![](https://github.com/TigeiaWorkshop/GFL-LastWish/raw/master/Assets/image/screenshot/battle.png)
+
+#### [GFL-Last](https://github.com/TigeiaWorkshop/GFL-LastWish ), a turn-based strategy game that demonstrates some advanced features and the unlimited potential of the Linpg engine.
+
+
+
 # :hammer_and_wrench: Dependencies / 运行库 
 
 | Required / 必需安装 |
 | :---------- |
-| pygame      |
+| pygame-ce   |
 | numpy       |
 | PySimpleGUI |
 
 | Recommended* / 建议安装* |
 | ------------------------ |
 | pyyaml                   |
 | opencv                   |
-| tcod                     |
 
-***Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.***
+\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
 
-##### ***感谢这些库的开发者，他（她）们让使用python开发游戏不再遥远。***
+##### Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.
 
-\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
+##### 感谢这些第三方库的开发者，他（她）们让使用python开发游戏不再遥远。
 
 
 
 # :computer:Installation / 安装
 
 ### Recommend:
 
 ```
 pip install linpg
 ```
 
-We also highly suggest you download and use [https://github.com/LinpgFoundation/A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
+We also highly suggest you download and use [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
 
 ### Building From Source:
 
 First, clone this repo:
 
 ```
 git clone https://github.com/LinpgFoundation/linpg
@@ -76,63 +87,46 @@
 
 Run `builder.py`:
 
 ```
 python builder.py
 ```
 
-Enjoy!
-
+That's it, enjoy!
 
 
 # :world_map: Branches / 分支​
 
 ### master:
 
-This branch holds the current stable version. 
+The current stable version. 
 
 该分支提供了当前的稳定版本
 
 ### dev:
 
-This branch holds the latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that may cause harm to your system or projects. This version is typically recommended for experienced developers.
-
-目前可以运行的最新版本，可能在修复了部分现有的bug的同时，又带有新增的bug。 推荐开发人员使用
-
-### * in-process:
-
-**DON'T USE THIS BRANCH!** This branch contains a version that is currently unfinished.
-
-还未完成，无法运行的版本，请勿使用
-
-### * exp:
-
-**DON'T USE THIS BRANCH!**  This branch contains a version that is still in the experimental stage.
-
-实验版本，包含了部分仍在试验阶段的内容，请勿使用
-
-
+The latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that can cause harm to your system or projects. This version is typically recommended for experienced developers.
 
-*: These branches may not be available to the public.
+目前可以运行的最新版本，相对稳定，但可能包含未被发现的问题或未完善的功能。 推荐有经验的开发人员使用。
 
 
 
 # :books: How to contribute / 如何贡献代码
 
 - It would be best if you can fork the "dev" branch as your starting point. If the "dev" branch does not exist, then fork the "master" branch.
 
   你应该fork "dev"分支作为作为你的起始点。如果"dev"分支不存在，则fork "master"分支。
 
 - After you have finished your work, you should request to merge to the "dev" branch instead of the "master" branch.
 
-  所有pull request应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
+  所有PR应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
 
 - We are looking forward to seeing a pull request that contains a detailed explanation about any changes that were made.
 
-  所有pull request应该阐明所有关于改动的细节。
+  所有PR应该详细地阐明其做出的改动。
 
 
 
 # :video_game: ​Discord
 
 https://discord.gg/3wz6bs5jvu
 
@@ -167,15 +161,15 @@
 | ----------------------------------------------------------- | ------------------------------------ | ------------------ |
 | A more modular and aesthetically modern visual novel system | 更加模块化和美观现代化的视觉小说系统 | :white_check_mark: |
 | Options menu                                                | 选项菜单模块                         | :white_check_mark: |
 | Better and more complex combat system                       | 更加完善复杂的战斗系统               | :white_check_mark: |
 | Map Editor                                                  | 可用的地图编辑器                     | :white_check_mark: |
 | Dialogue Editor                                             | 可用的对话编辑器                     | :white_check_mark: |
 | Most functions work when correct input is accepted          | 大部分功能能在接受正确的输入后工作   | :hammer:         |
-| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统保持60帧       | :white_check_mark: |
+| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统达到144帧       | :white_check_mark: |
 | Video can be played at a stable 60 fps                      | 视频能稳定地以60帧播放               | :white_check_mark: |
 | Pygame native input box (English only)                      | 可用的pygame原生输入框（仅支持英文） | :white_check_mark: |
 
 ------
 
 | Linpg 4 |( On Schedule / 未来-计划中 )||
 | ------------------------------------------------------------ | -------------------------------------------------------- | ---- |
@@ -183,18 +177,17 @@
 | Rewrite using a combination of c++ and cython for better performance | 底层采用c++和cython结合的方式重写以获取更高效的性能      |      |
 | Better options menu                                          | 更好的选项菜单模块                                       |      |
 | Enemy AI systems will be partially affected by machine learning. | 敌方AI系统将部分采用machine learning的意见               |      |
 | More convenient and beautiful map editor and dialogue editor | 更加便捷美观的地图编辑器和对话编辑器                     |      |
 | More readable and standardized code                          | 更加易读规范化的代码                                     |      |
 | Most functions are able to report errors and take the most appropriate approach after accepting incorrect input | 大部分功能能在接受错误的输入后报错并采取最合适的方案运行 |      |
 | The combat system can have more varieties.                   | 战斗系统能有更多的玩法                                   |      |
-| Visual novel system and combat system can reach 144 fps      | 视觉小说系统和战斗系统达到144帧                          |      |
 | The input box will support Chinese, Japanese, and more       | 输入框支持中文，日文，以及更多                           |      |
 
 
 
 
 # :memo: License / 版权说明
 
-Please check LICENSE.
+Please check **LICENSE**.
 
-版权信息请查看LICENSE文件。
+版权信息请查看**LICENSE**文件。
```

### Comparing `linpg-3.6.1/pyproject.toml` & `linpg-3.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,51 @@
     "setuptools>=64",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linpg"
-version = "3.6.1"
+version = "3.7.0"
 authors = [
     {name = "Linpg Foundation", email = "yudong9912@gmail.com"},
 ]
 description = "A game engine based on pygame, which aims to make game development easier."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pygame-ce",
     "numpy",
     "opencv-python",
     "pillow",
     "PySimpleGUI",
     "PyYAML",
-    "tcod",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LinpgFoundation/linpg"
 "Bug Tracker" = "https://github.com/LinpgFoundation/linpg/issues"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 # disallow_any_generics = true
 disallow_untyped_defs = true
 disallow_untyped_calls = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unreachable = true
 
 [tool.black]
 line-length = 160
-target-version = ['py310']
+target-version = ['py311']
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["*"]
```

### Comparing `linpg-3.6.1/src/linpg/CODE_OF_CONDUCT.md` & `linpg-3.7.0/src/linpg/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/LICENSE` & `linpg-3.7.0/src/linpg/LICENSE`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/README.md` & `linpg-3.7.0/src/linpg/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 # :speech_balloon: Preamble / 前言
 
 ###### *"Just because c++ is the greatest language ever invented doesn't mean that writing games in c++ is easy and fun, and the same goes for pygame."*
 
-###### *"c++是有史以来最伟大的语言，但并不代表用c++写游戏是一件很轻松有趣的事情，pygame也是如此。"*
+###### *"c++是有史以来最伟大的语言，但这并不代表用c++写游戏是一件轻松而又有趣的事情，pygame也是如此。"*
 
 
 
 # :sparkles: About Linpg Engine / 关于Linpg引擎
 
-Linpg Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
+Linpg (Lin's python game) Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
 
 Linpg Engine is developed with a modular concept. It implements many features which are commonly used in game development. Simultaneously, the Linpg Engine also maintains a high level of compatibility with Pygame, making it easy for developers to migrate existing Pygame projects to Linpg Engine or use the features which Linpg Engine provides on their own Pygame projects.
 
 We always need your help to make Linpg the best it can be! No matter who you are, any contributors are welcome!
 
 Linpg引擎是Linpg基金会基于pygame库自主研发的游戏引擎，目的是为了规范化pygame游戏的开发，使得游戏代码更加整洁，易读，易扩展，易维护。
 
 Linpg引擎的开发使用了模块化的理念，并在底层实现了很多游戏开发过程中常用到的功能。Linpg引擎一直保持着与pygame高度的兼容性，使得开发者可以很容易将现有的pygame项目迁移到Linpg引擎上，或者在自己的pygame项目中使用Linpg引擎提供的功能或者工具。
 
 世上无完人，我们需要你的帮助让Linpg引擎变得更好。欢迎任何能帮助我们改进Linpg引擎的开发者！
 
 
 
+# :crystal_ball:Some awesome games developed using Linpg
+
+![](https://github.com/LinpgFoundation/A-story-of-us/raw/master/Assets/image/screenshot/dialog.png)
+
+#### [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us), a visual novel game only contains around 100 lines of code. A great starting point for anyone who is interested in Linpg.
+
+![](https://github.com/TigeiaWorkshop/GFL-LastWish/raw/master/Assets/image/screenshot/battle.png)
+
+#### [GFL-Last](https://github.com/TigeiaWorkshop/GFL-LastWish ), a turn-based strategy game that demonstrates some advanced features and the unlimited potential of the Linpg engine.
+
+
+
 # :hammer_and_wrench: Dependencies / 运行库 
 
 | Required / 必需安装 |
 | :---------- |
-| pygame      |
+| pygame-ce   |
 | numpy       |
 | PySimpleGUI |
 
 | Recommended* / 建议安装* |
 | ------------------------ |
 | pyyaml                   |
 | opencv                   |
-| tcod                     |
 
-***Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.***
+\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
 
-##### ***感谢这些库的开发者，他（她）们让使用python开发游戏不再遥远。***
+##### Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.
 
-\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
+##### 感谢这些第三方库的开发者，他（她）们让使用python开发游戏不再遥远。
 
 
 
 # :computer:Installation / 安装
 
 ### Recommend:
 
 ```
 pip install linpg
 ```
 
-We also highly suggest you download and use [https://github.com/LinpgFoundation/A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
+We also highly suggest you download and use [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
 
 ### Building From Source:
 
 First, clone this repo:
 
 ```
 git clone https://github.com/LinpgFoundation/linpg
@@ -76,63 +87,46 @@
 
 Run `builder.py`:
 
 ```
 python builder.py
 ```
 
-Enjoy!
-
+That's it, enjoy!
 
 
 # :world_map: Branches / 分支​
 
 ### master:
 
-This branch holds the current stable version. 
+The current stable version. 
 
 该分支提供了当前的稳定版本
 
 ### dev:
 
-This branch holds the latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that may cause harm to your system or projects. This version is typically recommended for experienced developers.
-
-目前可以运行的最新版本，可能在修复了部分现有的bug的同时，又带有新增的bug。 推荐开发人员使用
-
-### * in-process:
-
-**DON'T USE THIS BRANCH!** This branch contains a version that is currently unfinished.
-
-还未完成，无法运行的版本，请勿使用
-
-### * exp:
-
-**DON'T USE THIS BRANCH!**  This branch contains a version that is still in the experimental stage.
-
-实验版本，包含了部分仍在试验阶段的内容，请勿使用
-
-
+The latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that can cause harm to your system or projects. This version is typically recommended for experienced developers.
 
-*: These branches may not be available to the public.
+目前可以运行的最新版本，相对稳定，但可能包含未被发现的问题或未完善的功能。 推荐有经验的开发人员使用。
 
 
 
 # :books: How to contribute / 如何贡献代码
 
 - It would be best if you can fork the "dev" branch as your starting point. If the "dev" branch does not exist, then fork the "master" branch.
 
   你应该fork "dev"分支作为作为你的起始点。如果"dev"分支不存在，则fork "master"分支。
 
 - After you have finished your work, you should request to merge to the "dev" branch instead of the "master" branch.
 
-  所有pull request应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
+  所有PR应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
 
 - We are looking forward to seeing a pull request that contains a detailed explanation about any changes that were made.
 
-  所有pull request应该阐明所有关于改动的细节。
+  所有PR应该详细地阐明其做出的改动。
 
 
 
 # :video_game: ​Discord
 
 https://discord.gg/3wz6bs5jvu
 
@@ -167,15 +161,15 @@
 | ----------------------------------------------------------- | ------------------------------------ | ------------------ |
 | A more modular and aesthetically modern visual novel system | 更加模块化和美观现代化的视觉小说系统 | :white_check_mark: |
 | Options menu                                                | 选项菜单模块                         | :white_check_mark: |
 | Better and more complex combat system                       | 更加完善复杂的战斗系统               | :white_check_mark: |
 | Map Editor                                                  | 可用的地图编辑器                     | :white_check_mark: |
 | Dialogue Editor                                             | 可用的对话编辑器                     | :white_check_mark: |
 | Most functions work when correct input is accepted          | 大部分功能能在接受正确的输入后工作   | :hammer:         |
-| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统保持60帧       | :white_check_mark: |
+| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统达到144帧       | :white_check_mark: |
 | Video can be played at a stable 60 fps                      | 视频能稳定地以60帧播放               | :white_check_mark: |
 | Pygame native input box (English only)                      | 可用的pygame原生输入框（仅支持英文） | :white_check_mark: |
 
 ------
 
 | Linpg 4 |( On Schedule / 未来-计划中 )||
 | ------------------------------------------------------------ | -------------------------------------------------------- | ---- |
@@ -183,18 +177,17 @@
 | Rewrite using a combination of c++ and cython for better performance | 底层采用c++和cython结合的方式重写以获取更高效的性能      |      |
 | Better options menu                                          | 更好的选项菜单模块                                       |      |
 | Enemy AI systems will be partially affected by machine learning. | 敌方AI系统将部分采用machine learning的意见               |      |
 | More convenient and beautiful map editor and dialogue editor | 更加便捷美观的地图编辑器和对话编辑器                     |      |
 | More readable and standardized code                          | 更加易读规范化的代码                                     |      |
 | Most functions are able to report errors and take the most appropriate approach after accepting incorrect input | 大部分功能能在接受错误的输入后报错并采取最合适的方案运行 |      |
 | The combat system can have more varieties.                   | 战斗系统能有更多的玩法                                   |      |
-| Visual novel system and combat system can reach 144 fps      | 视觉小说系统和战斗系统达到144帧                          |      |
 | The input box will support Chinese, Japanese, and more       | 输入框支持中文，日文，以及更多                           |      |
 
 
 
 
 # :memo: License / 版权说明
 
-Please check LICENSE.
+Please check **LICENSE**.
 
-版权信息请查看LICENSE文件。
+版权信息请查看**LICENSE**文件。
```

### Comparing `linpg-3.6.1/src/linpg/__pyinstaller/hook-linpg.py` & `linpg-3.7.0/src/linpg/__pyinstaller/hook-linpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, linpg
 
 __PATH: str = linpg.__path__[0]
 __NAME: str = "linpg"
 
-hiddenimports = ['PIL.Image', 'PIL.ImageColor', 'PIL.ImageFilter', 'PySimpleGUI', 'numpy', 'pygame', 'pygame.gfxdraw', 'tcod', 'tkinter']
+hiddenimports = ['PIL.Image', 'PIL.ImageColor', 'PIL.ImageFilter', 'PySimpleGUI', 'numpy', 'pygame', 'pygame.gfxdraw', 'tkinter']
 
 datas: list[tuple[str, str]] = []
 ignores: tuple[str, ...] = ("__pyinstaller", "__pycache__", ".git")
 
 for file_name in os.listdir(__PATH):
     # 文件夹
     if os.path.isdir(os.path.join(__PATH, file_name)):
```

### Comparing `linpg-3.6.1/src/linpg/abstracts.pyi` & `linpg-3.7.0/src/linpg/abstracts.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/basic.pyi` & `linpg-3.7.0/src/linpg/basic.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/battle.pyi` & `linpg-3.7.0/src/linpg/battle.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -142,33 +142,50 @@
     def play_sound(self, kind_of_sound: str) -> None: ...
     def move_follow(self, path: Sequence[tuple[int, int]]) -> None: ...
     def near(self, otherEntity: Position | Coordinate) -> bool: ...
     def range_target_in(self, otherEntity: Entity) -> int: ...
     def set_flip_based_on_pos(self, _pos: tuple[number, number]) -> None: ...
     def render(self, _surface: ImageSurface, pos: tuple[int, int], size: tuple[int, int], action: str | None = ..., alpha: int | None = ...) -> None: ...
 
+class _AStarPoint(Coordinate):
+    def __eq__(self, other: _AStarPoint) -> bool: ...
+
+class _AStarNode:
+    point: Incomplete
+    father: Incomplete
+    g: Incomplete
+    h: Incomplete
+    def __init__(self, point: _AStarPoint, endPoint: _AStarPoint, g: number = ...) -> None: ...
+
+class AStar:
+    @classmethod
+    def search(cls, map2d: numpy.ndarray, start_pos: tuple[int, int], end_pos: tuple[int, int]) -> list[tuple[int, int]]: ...
+
 class AbstractTileMap(Rectangle, SurfaceWithLocalPos):
     def __init__(self) -> None: ...
     def update(self, _data: dict, _block_size: int_f) -> None: ...
     @property
     def decorations(self) -> tuple[DecorationObject, ...]: ...
     @property
     def row(self) -> int: ...
     @property
     def column(self) -> int: ...
+    @property
+    def shape(self) -> tuple[int, int]: ...
+    def set_barrier_mask(self, x: int, y: int, value: int) -> None: ...
     def add_on_axis(self, index: int = ..., axis: int = ...) -> None: ...
     def remove_on_axis(self, index: int = ..., axis: int = ...) -> None: ...
     @property
     def tile_width(self) -> int: ...
     @property
     def tile_height(self) -> int: ...
     @property
     def tile_size(self) -> int: ...
     def to_dict(self) -> dict: ...
-    def is_passable(self, _x: int, _y: int) -> bool: ...
+    def is_passable(self, _x: int, _y: int, supposed: bool = ...) -> bool: ...
     def get_local_pos_in_percentage(self) -> dict[str, str]: ...
     def get_decoration(self, pos: object) -> DecorationObject | None: ...
     def add_decoration(self, _data: dict) -> None: ...
     def remove_decoration(self, decoration: DecorationObject) -> None: ...
     def count_decorations(self) -> int: ...
     def set_tile_size(self, newPerBlockWidth: int_f) -> None: ...
     def set_local_x(self, value: int_f) -> None: ...
```

### Comparing `linpg-3.6.1/src/linpg/config/__init__.pyi` & `linpg-3.7.0/src/linpg/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/config/specifications.json` & `linpg-3.7.0/src/linpg/config/specifications.json`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/config/ui.json` & `linpg-3.7.0/src/linpg/config/ui.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975163823123894%*

 * *Differences: {"'dialog_buttons'": "{'items': {2: {'text': {'src': '{Dialog.auto}'}}, 3: {'text': {'src': "*

 * *                     "'{Dialog.auto}'}}, 4: {'text': {'src': '{Dialog.skip}'}}}}",*

 * * "'dialog_editor_buttons'": "{'items': {0: {'description': '{Global.mute}'}, 1: {'description': "*

 * *                            "'{Global.save}'}, 2: {'description': '{Global.reload_file}'}, 3: "*

 * *                            "{'description': '{Editor.add}'}, 4: {'description': '{Editor.next}'}, "*

 * *                            "5: {'descri […]*

```diff
@@ -33,15 +33,15 @@
                 },
                 "name": "not_auto",
                 "scale_for_resizing_height": 1,
                 "scale_for_resizing_width": 1,
                 "src": "<NULL>",
                 "text": {
                     "color": "white",
-                    "src": "{Dialog,auto}"
+                    "src": "{Dialog.auto}"
                 },
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "80%",
                 "y": "5%"
             },
             {
@@ -54,15 +54,15 @@
                 },
                 "name": "is_auto",
                 "scale_for_resizing_height": 1,
                 "scale_for_resizing_width": 1,
                 "src": "<NULL>",
                 "text": {
                     "color": "white",
-                    "src": "{Dialog,auto}"
+                    "src": "{Dialog.auto}"
                 },
                 "type": "button",
                 "visibility": false,
                 "width": "<!button_size>",
                 "x": "80%",
                 "y": "5%"
             },
@@ -77,15 +77,15 @@
                 },
                 "name": "skip",
                 "scale_for_resizing_height": 1,
                 "scale_for_resizing_width": 1,
                 "src": "<NULL>",
                 "text": {
                     "color": "white",
-                    "src": "{Dialog,skip}"
+                    "src": "{Dialog.skip}"
                 },
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "90%",
                 "y": "5%"
             }
         ],
@@ -95,92 +95,92 @@
         "y": 0
     },
     "dialog_editor_buttons": {
         "height": "100%",
         "items": [
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Global,mute}",
+                "description": "{Global.mute}",
                 "height": "<!button_size>",
                 "name": "mute",
                 "src": "<&ui>mute.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!mute_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Global,save}",
+                "description": "{Global.save}",
                 "height": "<!button_size>",
                 "name": "save",
                 "src": "<&ui>save.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!save_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Global,reload_file}",
+                "description": "{Global.reload_file}",
                 "height": "<!button_size>",
                 "name": "reload",
                 "src": "<&ui>reload.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!reload_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Editor,add}",
+                "description": "{Editor.add}",
                 "height": "<!button_size>",
                 "name": "add",
                 "src": "<&ui>add.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!add_and_next_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Editor,next}",
+                "description": "{Editor.next}",
                 "height": "<!button_size>",
                 "name": "next",
                 "src": "<&ui>next.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!add_and_next_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Editor,previous}",
+                "description": "{Editor.previous}",
                 "height": "<!button_size>",
                 "name": "previous",
                 "src": "<&ui>previous.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!previous_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Editor,delete}",
+                "description": "{Editor.delete}",
                 "height": "<!button_size>",
                 "name": "delete",
                 "src": "<&ui>delete.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!delete_button_x>",
                 "y": "<!button_y>"
             },
             {
                 "alpha_when_not_hover": 150,
-                "description": "{Global,back_to_main_menu}",
+                "description": "{Global.back_to_main_menu}",
                 "height": "<!button_size>",
                 "name": "back",
                 "src": "<&ui>back.png",
                 "type": "button",
                 "width": "<!button_size>",
                 "x": "<!back_button_x>",
                 "y": "<!button_y>"
@@ -193,57 +193,57 @@
     },
     "exit_without_saving_progress_warning": {
         "height": "20%",
         "items": [
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{Global,warning}",
+                "src": "{Global.warning}",
                 "type": "text",
                 "x": "center",
                 "y": "10%"
             },
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{LeavingWithoutSavingWarning,about_to_exit}",
+                "src": "{LeavingWithoutSavingWarning.about_to_exit}",
                 "type": "text",
                 "x": "center",
                 "y": "30%"
             },
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{LeavingWithoutSavingWarning,progress_will_lost}",
+                "src": "{LeavingWithoutSavingWarning.progress_will_lost}",
                 "type": "text",
                 "x": "center",
                 "y": "50%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "height": "20%",
                 "name": "confirm",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,confirm}"
+                    "src": "{Global.confirm}"
                 },
                 "type": "button",
                 "width": "15%",
                 "x": "25%",
                 "y": "70%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "height": "20%",
                 "name": "cancel",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,cancel}"
+                    "src": "{Global.cancel}"
                 },
                 "type": "button",
                 "width": "15%",
                 "x": "60%",
                 "y": "70%"
             }
         ],
@@ -255,57 +255,57 @@
     },
     "leave_without_saving_progress_warning": {
         "height": "20%",
         "items": [
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{Global,warning}",
+                "src": "{Global.warning}",
                 "type": "text",
                 "x": "center",
                 "y": "10%"
             },
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{LeavingWithoutSavingWarning,about_to_leave}",
+                "src": "{LeavingWithoutSavingWarning.about_to_leave}",
                 "type": "text",
                 "x": "center",
                 "y": "30%"
             },
             {
                 "color": "white",
                 "font_size": "15%",
-                "src": "{LeavingWithoutSavingWarning,progress_will_lost}",
+                "src": "{LeavingWithoutSavingWarning.progress_will_lost}",
                 "type": "text",
                 "x": "center",
                 "y": "50%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "height": "20%",
                 "name": "confirm",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,confirm}"
+                    "src": "{Global.confirm}"
                 },
                 "type": "button",
                 "width": "15%",
                 "x": "25%",
                 "y": "70%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "height": "20%",
                 "name": "cancel",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,cancel}"
+                    "src": "{Global.cancel}"
                 },
                 "type": "button",
                 "width": "15%",
                 "x": "60%",
                 "y": "70%"
             }
         ],
@@ -317,74 +317,74 @@
     },
     "leave_without_saving_warning": {
         "height": "25%",
         "items": [
             {
                 "color": "white",
                 "font_size": "10%",
-                "src": "{Global,warning}",
+                "src": "{Global.warning}",
                 "type": "text",
                 "x": "center",
                 "y": "10%"
             },
             {
                 "color": "white",
                 "font_size": "10%",
-                "src": "{LeavingWithoutSavingWarning,leaving_without_saving_work1}",
+                "src": "{LeavingWithoutSavingWarning.leaving_without_saving_work1}",
                 "type": "text",
                 "x": "center",
                 "y": "25%"
             },
             {
                 "color": "white",
                 "font_size": "10%",
-                "src": "{LeavingWithoutSavingWarning,leaving_without_saving_work2}",
+                "src": "{LeavingWithoutSavingWarning.leaving_without_saving_work2}",
                 "type": "text",
                 "x": "center",
                 "y": "40%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "auto_resize": true,
                 "height": "15%",
                 "name": "save",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,save}"
+                    "src": "{Global.save}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": "20%",
                 "y": "70%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "auto_resize": true,
                 "height": "15%",
                 "name": "cancel",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,cancel}"
+                    "src": "{Global.cancel}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": "40%",
                 "y": "70%"
             },
             {
                 "alpha_when_not_hover": 150,
                 "auto_resize": true,
                 "height": "15%",
                 "name": "dont_save",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,dont_save}"
+                    "src": "{Global.dont_save}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": "70%",
                 "y": "70%"
             }
         ],
@@ -402,125 +402,155 @@
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "save",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,save}"
+                    "src": "{Global.save}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": "2%",
                 "y": "2%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "back",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,back}"
+                    "src": "{Global.back}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
                 "y": "2%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "delete",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,delete}"
+                    "src": "{Global.delete}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
                 "y": "2%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "reload",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Global,reload_file}"
+                    "src": "{Global.reload_file}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
                 "y": "2%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "new_row",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Editor,new_row}"
+                    "src": "{Editor.new_row}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
-                "y": "2%"
+                "y": "10%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "new_colum",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Editor,new_colum}"
+                    "src": "{Editor.new_colum}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
-                "y": "2%"
+                "y": "10%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "remove_row",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Editor,remove_row}"
+                    "src": "{Editor.remove_row}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
-                "y": "2%"
+                "y": "10%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "5%",
                 "name": "remove_colum",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Editor,remove_colum}"
+                    "src": "{Editor.remove_colum}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
-                "y": "2%"
+                "y": "10%"
+            },
+            {
+                "alpha_when_not_hover": 100,
+                "auto_resize": true,
+                "height": "5%",
+                "name": "auto_add_barriers",
+                "src": "<&ui>button.png",
+                "text": {
+                    "color": "black",
+                    "src": "{Editor.auto_add_barriers}"
+                },
+                "type": "button",
+                "width": 0,
+                "x": 0,
+                "y": "18%"
+            },
+            {
+                "alpha_when_not_hover": 100,
+                "auto_resize": true,
+                "height": "5%",
+                "name": "add_barrier",
+                "src": "<&ui>button.png",
+                "text": {
+                    "color": "black",
+                    "src": "{Editor.add_barrier}"
+                },
+                "type": "button",
+                "width": 0,
+                "x": 0,
+                "y": "18%"
             }
         ],
         "type": "container",
         "width": "100%",
         "x": 0,
         "y": 0
     },
@@ -531,30 +561,30 @@
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "3%",
                 "name": "select_tile",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Battle,tile}"
+                    "src": "{Editor.tile}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
                 "y": "3%"
             },
             {
                 "alpha_when_not_hover": 100,
                 "auto_resize": true,
                 "height": "3%",
                 "name": "select_decoration",
                 "src": "<&ui>button.png",
                 "text": {
                     "color": "black",
-                    "src": "{Battle,decoration}"
+                    "src": "{Editor.decoration}"
                 },
                 "type": "button",
                 "width": 0,
                 "x": 0,
                 "y": "3%"
             }
         ],
@@ -565,23 +595,23 @@
     },
     "option_menu": {
         "height": "75%",
         "items": [
             {
                 "color": "white",
                 "font_size": "7.5%",
-                "src": "{OptionMenu,setting}",
+                "src": "{OptionMenu.setting}",
                 "type": "text",
                 "x": "center",
                 "y": "5%"
             },
             {
                 "color": "white",
                 "font_size": "5%",
-                "src": "{OptionMenu,global_volume}",
+                "src": "{OptionMenu.global_volume}",
                 "type": "text",
                 "x": "22.5%",
                 "y": "30%"
             },
             {
                 "height": "5%",
                 "indicator": {
@@ -598,15 +628,15 @@
                 "width": "50%",
                 "x": "22.5%",
                 "y": "37.5%"
             },
             {
                 "color": "white",
                 "font_size": "5%",
-                "src": "{OptionMenu,background_music}",
+                "src": "{OptionMenu.background_music}",
                 "type": "text",
                 "x": "22.5%",
                 "y": "45%"
             },
             {
                 "height": "5%",
                 "indicator": {
@@ -623,15 +653,15 @@
                 "width": "50%",
                 "x": "22.5%",
                 "y": "52.5%"
             },
             {
                 "color": "white",
                 "font_size": "5%",
-                "src": "{OptionMenu,sound_effects}",
+                "src": "{OptionMenu.sound_effects}",
                 "type": "text",
                 "x": "22.5%",
                 "y": "60%"
             },
             {
                 "height": "5%",
                 "indicator": {
@@ -648,15 +678,15 @@
                 "width": "50%",
                 "x": "22.5%",
                 "y": "67.5%"
             },
             {
                 "color": "white",
                 "font_size": "5%",
-                "src": "{OptionMenu,environmental_sound}",
+                "src": "{OptionMenu.environmental_sound}",
                 "type": "text",
                 "x": "22.5%",
                 "y": "75%"
             },
             {
                 "height": "5%",
                 "indicator": {
@@ -673,15 +703,15 @@
                 "width": "50%",
                 "x": "22.5%",
                 "y": "82.5%"
             },
             {
                 "color": "white",
                 "font_size": "5%",
-                "src": "{OptionMenu,language}",
+                "src": "{OptionMenu.language}",
                 "type": "text",
                 "x": "22.5%",
                 "y": "20%"
             },
             {
                 "font_size": "5%",
                 "name": "lang_drop_down",
@@ -700,65 +730,65 @@
         "height": "100%",
         "items": [
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "resume",
                 "outline_thickness": 2,
-                "src": "{Global,resume}",
+                "src": "{Global.resume}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "27.5%"
             },
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "save",
                 "outline_thickness": 2,
-                "src": "{Global,save_current_progress}",
+                "src": "{Global.save_current_progress}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "35%"
             },
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "load",
                 "outline_thickness": 2,
-                "src": "{Global,load_progress}",
+                "src": "{Global.load_progress}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "42.5%"
             },
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "option_menu",
                 "outline_thickness": 2,
-                "src": "{OptionMenu,option_menu}",
+                "src": "{OptionMenu.option_menu}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "50%"
             },
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "back_to_mainMenu",
                 "outline_thickness": 2,
-                "src": "{Global,back_to_main_menu}",
+                "src": "{Global.back_to_main_menu}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "57.5%"
             },
             {
                 "color": "white",
                 "font_size": "3%",
                 "name": "exit_to_desktop",
                 "outline_thickness": 2,
-                "src": "{OptionMenu,exit_to_desktop}",
+                "src": "{OptionMenu.exit_to_desktop}",
                 "type": "text&resize_when_hovered",
                 "x": "7.5%",
                 "y": "65%"
             }
         ],
         "type": "container",
         "width": "100%",
```

### Comparing `linpg-3.6.1/src/linpg/core.pyi` & `linpg-3.7.0/src/linpg/core.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/dialogue.pyi` & `linpg-3.7.0/src/linpg/dialogue.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 class DialogContent:
     background_image: Incomplete
     background_music: Incomplete
     character_images: Incomplete
     contents: Incomplete
     narrator: Incomplete
-    last: Incomplete
+    previous: Incomplete
     next: Incomplete
     notes: Incomplete
     def __init__(self, _data: dict, _id: str) -> None: ...
     @property
     def id(self) -> str: ...
     def has_next(self) -> bool: ...
     def has_multiple_next(self) -> bool: ...
```

### Comparing `linpg-3.6.1/src/linpg/doc/CN1_简介.md` & `linpg-3.7.0/src/linpg/doc/CN1_简介.md`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/doc/CN2_入门.md` & `linpg-3.7.0/src/linpg/doc/CN2_入门.md`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/doc/EN1_Introduction.md` & `linpg-3.7.0/src/linpg/doc/EN1_Introduction.md`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/exception.pyi` & `linpg-3.7.0/src/linpg/exception.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/interface.pyi` & `linpg-3.7.0/src/linpg/interface.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/language/English.json` & `linpg-3.7.0/src/linpg/language/English.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8771929824561404%*

 * *Differences: {"'Editor'": "{'add_barrier': 'Add Barrier', 'auto_add_barriers': 'Animatedly Add Barriers', "*

 * *             "'decoration': 'Decoration', 'tile': 'Tile'}",*

 * * 'delete': "['Battle']"}*

```diff
@@ -1,33 +1,33 @@
 {
-    "Battle": {
-        "decoration": "Decoration",
-        "tile": "Tile"
-    },
     "Dialog": {
         "auto": "Auto",
         "choice": "Choice",
         "skip": "Skip"
     },
     "Editor": {
         "add": "New dialog",
+        "add_barrier": "Add Barrier",
+        "auto_add_barriers": "Animatedly Add Barriers",
         "background": "Background Image",
+        "decoration": "Decoration",
         "delete": "Delete current dialog",
         "example_project": "Example Project",
         "new_colum": "New Colum",
         "new_row": "New Row",
         "next": "Next dialog",
         "no_bgm": "No background music",
         "npc": "Npc",
         "please_enter_content": "Content",
         "please_enter_name": "Name",
         "previous": "Previous dialog",
         "remove_colum": "Remove Colum",
         "remove_npc": "Remove this npc",
-        "remove_row": "Remove Row"
+        "remove_row": "Remove Row",
+        "tile": "Tile"
     },
     "Global": {
         "back": "Back",
         "back_to_main_menu": "Back to Main Menu",
         "cancel": "Cancel",
         "confirm": "Confirm",
         "delete": "Delete",
```

### Comparing `linpg-3.6.1/src/linpg/language/SimplifiedChinese.json` & `linpg-3.7.0/src/linpg/language/SimplifiedChinese.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8771929824561404%*

 * *Differences: {"'Editor'": "{'add_barrier': '添加屏障', 'auto_add_barriers': '自动添加屏障', 'decoration': '装饰物', 'tile': "*

 * *             "'方块'}",*

 * * 'delete': "['Battle']"}*

```diff
@@ -1,33 +1,33 @@
 {
-    "Battle": {
-        "decoration": "\u88c5\u9970\u7269",
-        "tile": "\u65b9\u5757"
-    },
     "Dialog": {
         "auto": "\u81ea\u52a8",
         "choice": "\u9009\u9879",
         "skip": "\u8df3\u8fc7"
     },
     "Editor": {
         "add": "\u65b0\u589e\u5bf9\u8bdd",
+        "add_barrier": "\u6dfb\u52a0\u5c4f\u969c",
+        "auto_add_barriers": "\u81ea\u52a8\u6dfb\u52a0\u5c4f\u969c",
         "background": "\u80cc\u666f\u56fe\u7247",
+        "decoration": "\u88c5\u9970\u7269",
         "delete": "\u5220\u9664\u5f53\u524d\u5bf9\u8bdd",
         "example_project": "\u6f14\u793a\u9879\u76ee",
         "new_colum": "\u65b0\u589e\u5217",
         "new_row": "\u65b0\u589e\u884c",
         "next": "\u4e0b\u4e00\u4e2a\u5bf9\u8bdd",
         "no_bgm": "\u65e0\u80cc\u666f\u97f3\u4e50",
         "npc": "\u7acb\u7ed8",
         "please_enter_content": "\u5bf9\u8bdd\u5185\u5bb9",
         "please_enter_name": "\u89d2\u8272\u540d",
         "previous": "\u4e0a\u4e00\u4e2a\u5bf9\u8bdd",
         "remove_colum": "\u5220\u9664\u5217",
         "remove_npc": "\u79fb\u9664\u8be5\u89d2\u8272",
-        "remove_row": "\u5220\u9664\u884c"
+        "remove_row": "\u5220\u9664\u884c",
+        "tile": "\u65b9\u5757"
     },
     "Global": {
         "back": "\u8fd4\u56de",
         "back_to_main_menu": "\u8fd4\u56de\u4e3b\u83dc\u5355",
         "cancel": "\u53d6\u6d88",
         "confirm": "\u786e\u8ba4",
         "delete": " \u5220\u9664",
```

### Comparing `linpg-3.6.1/src/linpg/language/TraditionalChinese.json` & `linpg-3.7.0/src/linpg/language/TraditionalChinese.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8771929824561404%*

 * *Differences: {"'Editor'": "{'add_barrier': '添加屏障', 'auto_add_barriers': '自動添加屏障', 'decoration': '裝飾物', 'tile': "*

 * *             "'方塊'}",*

 * * 'delete': "['Battle']"}*

```diff
@@ -1,33 +1,33 @@
 {
-    "Battle": {
-        "decoration": "\u88dd\u98fe\u7269",
-        "tile": "\u65b9\u584a"
-    },
     "Dialog": {
         "auto": "\u81ea\u52d5",
         "choice": "\u9078\u9805",
         "skip": "\u8df3\u904e"
     },
     "Editor": {
         "add": "\u65b0\u589e\u5c0d\u8a71",
+        "add_barrier": "\u6dfb\u52a0\u5c4f\u969c",
+        "auto_add_barriers": "\u81ea\u52d5\u6dfb\u52a0\u5c4f\u969c",
         "background": "\u80cc\u666f\u5716\u7247",
+        "decoration": "\u88dd\u98fe\u7269",
         "delete": "\u522a\u9664\u7576\u524d\u5c0d\u8a71",
         "example_project": "\u6f14\u793a\u9805\u76ee",
         "new_colum": "\u65b0\u589e\u5217",
         "new_row": "\u65b0\u589e\u884c",
         "next": "\u4e0b\u4e00\u500b\u5c0d\u8a71",
         "no_bgm": "\u7121\u80cc\u666f\u97f3\u6a02",
         "npc": "\u7acb\u7e6a",
         "please_enter_content": "\u5c0d\u8a71\u5167\u5bb9",
         "please_enter_name": "\u89d2\u8272\u540d",
         "previous": "\u4e0a\u4e00\u500b\u5c0d\u8a71",
         "remove_colum": "\u522a\u9664\u5217",
         "remove_npc": "\u79fb\u9664\u8a72\u89d2\u8272",
-        "remove_row": "\u522a\u9664\u884c"
+        "remove_row": "\u522a\u9664\u884c",
+        "tile": "\u65b9\u584a"
     },
     "Global": {
         "back": "\u8fd4\u56de",
         "back_to_main_menu": "\u8fd4\u56de\u4e3b\u83dc\u55ae",
         "cancel": "\u53d6\u6d88",
         "confirm": "\u78ba\u8a8d",
         "delete": " \u522a\u9664",
```

### Comparing `linpg-3.6.1/src/linpg/language/__init__.pyi` & `linpg-3.7.0/src/linpg/language/__init__.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg/ui.pyi` & `linpg-3.7.0/src/linpg/ui.pyi`

 * *Files identical despite different names*

### Comparing `linpg-3.6.1/src/linpg.egg-info/PKG-INFO` & `linpg-3.7.0/src/linpg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,87 @@
 Metadata-Version: 2.1
 Name: linpg
-Version: 3.6.1
+Version: 3.7.0
 Summary: A game engine based on pygame, which aims to make game development easier.
 Author-email: Linpg Foundation <yudong9912@gmail.com>
 Project-URL: Homepage, https://github.com/LinpgFoundation/linpg
 Project-URL: Bug Tracker, https://github.com/LinpgFoundation/linpg/issues
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # :speech_balloon: Preamble / 前言
 
 ###### *"Just because c++ is the greatest language ever invented doesn't mean that writing games in c++ is easy and fun, and the same goes for pygame."*
 
-###### *"c++是有史以来最伟大的语言，但并不代表用c++写游戏是一件很轻松有趣的事情，pygame也是如此。"*
+###### *"c++是有史以来最伟大的语言，但这并不代表用c++写游戏是一件轻松而又有趣的事情，pygame也是如此。"*
 
 
 
 # :sparkles: About Linpg Engine / 关于Linpg引擎
 
-Linpg Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
+Linpg (Lin's python game) Engine is a game engine developed by Linpg Foundation, which aims to standardize the development of Pygame games and make the codes easier to read, expand and maintain.
 
 Linpg Engine is developed with a modular concept. It implements many features which are commonly used in game development. Simultaneously, the Linpg Engine also maintains a high level of compatibility with Pygame, making it easy for developers to migrate existing Pygame projects to Linpg Engine or use the features which Linpg Engine provides on their own Pygame projects.
 
 We always need your help to make Linpg the best it can be! No matter who you are, any contributors are welcome!
 
 Linpg引擎是Linpg基金会基于pygame库自主研发的游戏引擎，目的是为了规范化pygame游戏的开发，使得游戏代码更加整洁，易读，易扩展，易维护。
 
 Linpg引擎的开发使用了模块化的理念，并在底层实现了很多游戏开发过程中常用到的功能。Linpg引擎一直保持着与pygame高度的兼容性，使得开发者可以很容易将现有的pygame项目迁移到Linpg引擎上，或者在自己的pygame项目中使用Linpg引擎提供的功能或者工具。
 
 世上无完人，我们需要你的帮助让Linpg引擎变得更好。欢迎任何能帮助我们改进Linpg引擎的开发者！
 
 
 
+# :crystal_ball:Some awesome games developed using Linpg
+
+![](https://github.com/LinpgFoundation/A-story-of-us/raw/master/Assets/image/screenshot/dialog.png)
+
+#### [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us), a visual novel game only contains around 100 lines of code. A great starting point for anyone who is interested in Linpg.
+
+![](https://github.com/TigeiaWorkshop/GFL-LastWish/raw/master/Assets/image/screenshot/battle.png)
+
+#### [GFL-Last](https://github.com/TigeiaWorkshop/GFL-LastWish ), a turn-based strategy game that demonstrates some advanced features and the unlimited potential of the Linpg engine.
+
+
+
 # :hammer_and_wrench: Dependencies / 运行库 
 
 | Required / 必需安装 |
 | :---------- |
-| pygame      |
+| pygame-ce   |
 | numpy       |
 | PySimpleGUI |
 
 | Recommended* / 建议安装* |
 | ------------------------ |
 | pyyaml                   |
 | opencv                   |
-| tcod                     |
 
-***Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.***
+\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
 
-##### ***感谢这些库的开发者，他（她）们让使用python开发游戏不再遥远。***
+##### Special shout out to the developers of these libraries. They make game development using python no longer unthinkable.
 
-\* All these libraries will be installed by default as some common features cannot be enabled without these libraries.
+##### 感谢这些第三方库的开发者，他（她）们让使用python开发游戏不再遥远。
 
 
 
 # :computer:Installation / 安装
 
 ### Recommend:
 
 ```
 pip install linpg
 ```
 
-We also highly suggest you download and use [https://github.com/LinpgFoundation/A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
+We also highly suggest you download and use [A-story-of-us](https://github.com/LinpgFoundation/A-story-of-us) as your starting point.
 
 ### Building From Source:
 
 First, clone this repo:
 
 ```
 git clone https://github.com/LinpgFoundation/linpg
@@ -90,63 +101,46 @@
 
 Run `builder.py`:
 
 ```
 python builder.py
 ```
 
-Enjoy!
-
+That's it, enjoy!
 
 
 # :world_map: Branches / 分支​
 
 ### master:
 
-This branch holds the current stable version. 
+The current stable version. 
 
 该分支提供了当前的稳定版本
 
 ### dev:
 
-This branch holds the latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that may cause harm to your system or projects. This version is typically recommended for experienced developers.
-
-目前可以运行的最新版本，可能在修复了部分现有的bug的同时，又带有新增的bug。 推荐开发人员使用
-
-### * in-process:
-
-**DON'T USE THIS BRANCH!** This branch contains a version that is currently unfinished.
-
-还未完成，无法运行的版本，请勿使用
-
-### * exp:
-
-**DON'T USE THIS BRANCH!**  This branch contains a version that is still in the experimental stage.
-
-实验版本，包含了部分仍在试验阶段的内容，请勿使用
-
-
+The latest version that is available to the public. While this version may contain patches that fix identified problems, it may also have unknown or known new bugs that can cause harm to your system or projects. This version is typically recommended for experienced developers.
 
-*: These branches may not be available to the public.
+目前可以运行的最新版本，相对稳定，但可能包含未被发现的问题或未完善的功能。 推荐有经验的开发人员使用。
 
 
 
 # :books: How to contribute / 如何贡献代码
 
 - It would be best if you can fork the "dev" branch as your starting point. If the "dev" branch does not exist, then fork the "master" branch.
 
   你应该fork "dev"分支作为作为你的起始点。如果"dev"分支不存在，则fork "master"分支。
 
 - After you have finished your work, you should request to merge to the "dev" branch instead of the "master" branch.
 
-  所有pull request应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
+  所有PR应该请求merge到"dev"分支中。如果"dev"不存在，则请求merge到"master"分支。
 
 - We are looking forward to seeing a pull request that contains a detailed explanation about any changes that were made.
 
-  所有pull request应该阐明所有关于改动的细节。
+  所有PR应该详细地阐明其做出的改动。
 
 
 
 # :video_game: ​Discord
 
 https://discord.gg/3wz6bs5jvu
 
@@ -181,15 +175,15 @@
 | ----------------------------------------------------------- | ------------------------------------ | ------------------ |
 | A more modular and aesthetically modern visual novel system | 更加模块化和美观现代化的视觉小说系统 | :white_check_mark: |
 | Options menu                                                | 选项菜单模块                         | :white_check_mark: |
 | Better and more complex combat system                       | 更加完善复杂的战斗系统               | :white_check_mark: |
 | Map Editor                                                  | 可用的地图编辑器                     | :white_check_mark: |
 | Dialogue Editor                                             | 可用的对话编辑器                     | :white_check_mark: |
 | Most functions work when correct input is accepted          | 大部分功能能在接受正确的输入后工作   | :hammer:         |
-| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统保持60帧       | :white_check_mark: |
+| Visual novel system and combat system can maintain 60 fps   | 视觉小说系统和战斗系统达到144帧       | :white_check_mark: |
 | Video can be played at a stable 60 fps                      | 视频能稳定地以60帧播放               | :white_check_mark: |
 | Pygame native input box (English only)                      | 可用的pygame原生输入框（仅支持英文） | :white_check_mark: |
 
 ------
 
 | Linpg 4 |( On Schedule / 未来-计划中 )||
 | ------------------------------------------------------------ | -------------------------------------------------------- | ---- |
@@ -197,18 +191,17 @@
 | Rewrite using a combination of c++ and cython for better performance | 底层采用c++和cython结合的方式重写以获取更高效的性能      |      |
 | Better options menu                                          | 更好的选项菜单模块                                       |      |
 | Enemy AI systems will be partially affected by machine learning. | 敌方AI系统将部分采用machine learning的意见               |      |
 | More convenient and beautiful map editor and dialogue editor | 更加便捷美观的地图编辑器和对话编辑器                     |      |
 | More readable and standardized code                          | 更加易读规范化的代码                                     |      |
 | Most functions are able to report errors and take the most appropriate approach after accepting incorrect input | 大部分功能能在接受错误的输入后报错并采取最合适的方案运行 |      |
 | The combat system can have more varieties.                   | 战斗系统能有更多的玩法                                   |      |
-| Visual novel system and combat system can reach 144 fps      | 视觉小说系统和战斗系统达到144帧                          |      |
 | The input box will support Chinese, Japanese, and more       | 输入框支持中文，日文，以及更多                           |      |
 
 
 
 
 # :memo: License / 版权说明
 
-Please check LICENSE.
+Please check **LICENSE**.
 
-版权信息请查看LICENSE文件。
+版权信息请查看**LICENSE**文件。
```

### Comparing `linpg-3.6.1/src/linpg.egg-info/SOURCES.txt` & `linpg-3.7.0/src/linpg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/linpg/CODE_OF_CONDUCT.md
 src/linpg/LICENSE
 src/linpg/README.md
-src/linpg/__init__.cp310-win_amd64.pyd
+src/linpg/__init__.cp311-win_amd64.pyd
 src/linpg/__init__.pyi
-src/linpg/abstracts.cp310-win_amd64.pyd
+src/linpg/abstracts.cp311-win_amd64.pyd
 src/linpg/abstracts.pyi
-src/linpg/basic.cp310-win_amd64.pyd
+src/linpg/basic.cp311-win_amd64.pyd
 src/linpg/basic.pyi
-src/linpg/battle.cp310-win_amd64.pyd
+src/linpg/battle.cp311-win_amd64.pyd
 src/linpg/battle.pyi
-src/linpg/core.cp310-win_amd64.pyd
+src/linpg/core.cp311-win_amd64.pyd
 src/linpg/core.pyi
-src/linpg/dialogue.cp310-win_amd64.pyd
+src/linpg/dialogue.cp311-win_amd64.pyd
 src/linpg/dialogue.pyi
-src/linpg/exception.cp310-win_amd64.pyd
+src/linpg/exception.cp311-win_amd64.pyd
 src/linpg/exception.pyi
-src/linpg/interface.cp310-win_amd64.pyd
+src/linpg/interface.cp311-win_amd64.pyd
 src/linpg/interface.pyi
 src/linpg/py.typed
-src/linpg/ui.cp310-win_amd64.pyd
+src/linpg/ui.cp311-win_amd64.pyd
 src/linpg/ui.pyi
 src/linpg.egg-info/PKG-INFO
 src/linpg.egg-info/SOURCES.txt
 src/linpg.egg-info/dependency_links.txt
 src/linpg.egg-info/entry_points.txt
 src/linpg.egg-info/requires.txt
 src/linpg.egg-info/top_level.txt
 src/linpg/__pyinstaller/__init__.py
 src/linpg/__pyinstaller/hook-linpg.py
-src/linpg/config/__init__.cp310-win_amd64.pyd
+src/linpg/config/__init__.cp311-win_amd64.pyd
 src/linpg/config/__init__.pyi
 src/linpg/config/specifications.json
 src/linpg/config/ui.json
 src/linpg/doc/CN1_简介.md
 src/linpg/doc/CN2_入门.md
 src/linpg/doc/EN1_Introduction.md
 src/linpg/doc/Home.md
 src/linpg/language/English.json
 src/linpg/language/SimplifiedChinese.json
 src/linpg/language/TraditionalChinese.json
-src/linpg/language/__init__.cp310-win_amd64.pyd
+src/linpg/language/__init__.cp311-win_amd64.pyd
 src/linpg/language/__init__.pyi
```

