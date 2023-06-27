# Comparing `tmp/wmwpy-0.4.1b0.tar.gz` & `tmp/wmwpy-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.4.1b0.tar", last modified: Tue May 30 21:22:02 2023, max compression
+gzip compressed data, was "wmwpy-0.5.0b0.tar", last modified: Tue Jun 27 19:38:42 2023, max compression
```

## Comparing `wmwpy-0.4.1b0.tar` & `wmwpy-0.5.0b0.tar`

### file list

```diff
@@ -1,57 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.043078 wmwpy-0.4.1b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.043078 wmwpy-0.4.1b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Font/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/gif.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.051078 wmwpy-0.4.1b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.055078 wmwpy-0.4.1b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/classes/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-30 21:21:48.000000 wmwpy-0.4.1b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:22:02.047078 wmwpy-0.4.1b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49356 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 21:22:02.000000 wmwpy-0.4.1b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49376 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.953100 wmwpy-0.5.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.953100 wmwpy-0.5.0b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.957100 wmwpy-0.5.0b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/Font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.957100 wmwpy-0.5.0b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33465 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.957100 wmwpy-0.5.0b0/src/wmwpy/classes/objectpack/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/objectpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/objectpack/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/objectpack/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40969 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/texturesettings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.957100 wmwpy-0.5.0b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/src/wmwpy/object_packs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/object_packs/WMW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/object_packs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/src/wmwpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.961100 wmwpy-0.5.0b0/src/wmwpy/utils/file_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/file_types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/file_types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/file_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23358 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/imageprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-27 19:38:28.000000 wmwpy-0.5.0b0/src/wmwpy/utils/waltex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:38:42.957100 wmwpy-0.5.0b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49376 2023-06-27 19:38:42.000000 wmwpy-0.5.0b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-27 19:38:42.000000 wmwpy-0.5.0b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:38:42.000000 wmwpy-0.5.0b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 19:38:42.000000 wmwpy-0.5.0b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 19:38:42.000000 wmwpy-0.5.0b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.4.1b0/LICENSE` & `wmwpy-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/PKG-INFO` & `wmwpy-0.5.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.4.1b0
+Version: 0.5.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1017,15 +1017,15 @@
  ```
 py -m build
  ```
 
 # Building docs
  To build the docs, make sure sphinx is installed
  ```
-pip install -U sphinx
+pip install -r doc-build/requirements.txt
  ```
 
  You then need to run
  ```
 sphinx-build -b html doc-build docs
  ```
```

### Comparing `wmwpy-0.4.1b0/README.md` & `wmwpy-0.5.0b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
  ```
 py -m build
  ```
 
 # Building docs
  To build the docs, make sure sphinx is installed
  ```
-pip install -U sphinx
+pip install -r doc-build/requirements.txt
  ```
 
  You then need to run
  ```
 sphinx-build -b html doc-build docs
  ```
```

### Comparing `wmwpy-0.4.1b0/pyproject.toml` & `wmwpy-0.5.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 ]
 dependencies = [
   "lxml",
   "numpy",
   "Pillow",
   "natsort",
   "filetype",
-  "tk",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/wmw-modding/wmwpy"
 "Bug Tracker" = "https://github.com/wmw-modding/wmwpy/issues"
 "Documentation" = "https://wmw-modding.github.io/wmwpy/"
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/file_types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/XMLTools.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/XMLTools.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import natsort
 import typing
 import fnmatch
 import logging
 
 from .path import joinPath
 # from . import Waltex
-# from . import ImageUtils
+# from . import Imageutils
 # from ..classes import sprite
 # from ..classes import Object
 
 __all__ = ['Filesystem', 'File', 'Folder', 'FileBase']
 
 
 FILE_READERS = []
@@ -378,14 +378,15 @@
             this._rawcontent = data.read()
             if isinstance(this._rawcontent, str):
                 this._rawcontent = this._rawcontent.encode()
         else:
             this._rawcontent = bytes(data)
         
         this.content = None
+        this.reader = Reader()
         
         if this._datatype == 'raw':
             this._getdata()
         
     def _getdata(this):
         """Get data from file path
         """
@@ -443,34 +444,45 @@
         if this._datatype == 'path':
             return os.path.splitext(this._rawcontent)[1::]
         else:
             this._extension
     @extension.setter
     def extension(this, value):
         this._extension = value
+    
+    def setReader(this, extension = None, mime = None, **kwargs):
+        this.reader = Reader()
+        
+        for r in FILE_READERS:
+            # print(r)
+            if r.check(mime, extension, this.rawdata, filesystem = this.filesystem, **kwargs):
+                this.reader = r
+                return r
+        
+        for r in FILE_READERS:
+            # print(r)
+            if r.check(this.mime, this.extension, this.rawdata, filesystem = this.filesystem, **kwargs):
+                this.reader = r
+                return r
         
-    def read(this, **kwargs):
+        return this.reader
+    
+    def read(this, mime = None, extension = None, **kwargs):
         """Read file.
 
         Returns:
             Any: Object for file.
         """
         
         if this._datatype == 'path':
             this._getdata()
         
         this.rawdata.seek(0)
         
-        reader = Reader()
-        
-        for r in FILE_READERS:
-            # print(r)
-            if r.check(this.mime, this.extension, this.rawdata, filesystem = this.filesystem, **kwargs):
-                reader = r
-                break
+        reader = this.setReader(mime = mime, extension = extension, **kwargs)
         
         this.content = reader.read(this.mime, this.extension, this.rawdata, **kwargs)
         
         # if this.mime == 'image/waltex':
         #     this.content = Waltex(this.rawcontent.getvalue())
         #     this.image = this.content.image
         
@@ -488,18 +500,18 @@
         #             print(f)
                     
         #             content = this.content.read(f)
         #             this.root.add(f, content, replace = True)
                 
         # elif this.mime.startswith('text/'):
         #     if this.extension == 'imagelist':
-        #         this.content = ImageUtils.Imagelist(this.rawcontent.getvalue(), this.root, **kwargs)
+        #         this.content = Imageutils.Imagelist(this.rawcontent.getvalue(), this.root, **kwargs)
         #         # I need to make Imagelist() accept a Folder or Filesystem, and raw file data.
         #         # raise NotImplementedError('Imagelist reading is currently not implemented yet.')
-        #         # this.content = ImageUtils.Imagelist()
+        #         # this.content = Imageutils.Imagelist()
         #     else:
         #         this.content = this.rawcontent.read().decode(encoding=kwargs['encoding'])
         
         this.rawdata.seek(0)
         
         return this.content
     
@@ -527,26 +539,29 @@
             path (str): Path to check.
 
         Returns:
             bool: Does path exist?
         """
         return this.parent.exists(path)
     
-    def write(this, data : bytes) -> int:
+    def write(this, data : bytes, extension = None, mime = None,) -> int:
         """Write data to file.
 
         Args:
             data (bytes): New data.
 
         Returns:
             int: bytes written.
         """
         this.rawdata.truncate(0)
         this.rawdata.seek(0)
-        return this.rawdata.write(data)
+        
+        this.setReader(extension = extension, mime = mime)
+        
+        return this.rawdata.write(this.reader.save(data))
     
     def listdir(this, recursive = False, search = r'*'):
         """Returns a list of files and subfolders in path.
 
         Args:
             path (str, optional): Path to folder to list. Defaults to '/'.
             recursive (bool, optional): Whether to include subfolders. Defaults to False.
@@ -730,21 +745,26 @@
         """
         if 'endoding' in kwargs:
             encoding = kwargs['encoding']
         else:
             encoding = 'utf-8'
         
         return rawdata.getvalue().decode(encoding=encoding)
+    
+    def save(this, data : bytes | io.BytesIO) -> bytes:
+        if isinstance(data, io.BytesIO):
+            return data.getvalue()
+        return data
 
 def register_reader(reader : Reader):
     """
     Add reader for file type.
-    reader must inherit from `Utils.filesystem.Reader` class.
+    reader must inherit from `utils.filesystem.Reader` class.
 
     Args:
         reader (Reader): Inherited `Reader` class.
     """
     
     if isinstance(reader, Reader):
         FILE_READERS.append(reader)
     else:
-        raise TypeError('reader must inherit from `Utils.filesystem.Reader`')
+        raise TypeError('reader must inherit from `utils.filesystem.Reader`')
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/gif.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/gif.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/path.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/path.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/rotate.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/rotate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/textures.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/texture.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,141 @@
-import os
-from lxml import etree
+from .texturesettings import TextureSettings
+from ..gameobject import GameObject
+from ..utils.filesystem import File, Filesystem, Folder
+from ..utils.textures import getHDFile
+from ..utils.waltex import Waltex
+
 
-from .waltex import WaltexImage, Waltex
 from PIL import Image
 
-from .path import joinPath
-from .XMLTools import findTag
-from .filesystem import Filesystem, Folder, File
-from ..gameobject import GameObject
 
-_cachedWaltextImages = {}
+import io
+import os
+
 
 class Texture(GameObject):
     def __init__(
         this,
         image : Image.Image | Waltex | File,
-        HD : bool = False,
-        TabHD : bool = False,
+        filesystem : Filesystem | Folder = None,
+        gamepath : str = None,
+        assets : str = '/assets',
+        baseassets : str = '/',
+        HD = False,
+        TabHD = False,
     ) -> None:
         """Texture for image.
-
         Args:
             image (Image.Image | Waltex | File): Image object. Can be PIL.Image.Image, Waltex image, or file.
-            HD (bool, optional): Use HD images. Defaults to False.
-            TabHD (bool, optional): Use TabHD images. Defaults to False.
-
+            filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
+            gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+            assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`.
+            HD (bool, optional): Use HD image. Defaults to False.
+            TabHD (bool, optional): Use TabHD image. Defaults to False.
         Raises:
             TypeError: image must be PIL.Image.Image, Waltex, or filesystem.File.
         """
-        this._image = image
-        
-        if isinstance(this._image, File):
-            this._image = this._image.read()
-        
-        if isinstance(this._image, Waltex):
-            this.image = this._image.image
-        elif isinstance(this._image, Image.Image):
-            this.image = this._image
+        super().__init__(filesystem, gamepath, assets, baseassets)
+
+        this._file = image
+        this.HD = HD
+        this.TabHD = TabHD
+
+        if isinstance(this._file, (File, str)):
+            if isinstance(this._file, str):
+                this.filename = this._file
+            else:
+                this.filename = this._file.path
+
+            this._file = getHDFile(
+                this._file,
+                HD = this.HD,
+                TabHD = this.TabHD,
+                filesystem = this.filesystem,
+                gamepath = this.gamepath,
+                assets = this.assets,
+                baseassets = this.baseassets,
+            )
+        else:
+            this.filename = ''
+
+        if isinstance(this._file, str):
+            this._file = this.filesystem.get(this._file)
+
+        if isinstance(this._file, Waltex):
+            this.image = this._file.image
+        elif isinstance(this._file, Image.Image):
+            this.image = this._file
+        elif isinstance(this._file, File):
+            this.image = this._file.read()
+            if isinstance(this.image, Waltex):
+                this.image = this.image.image
+        elif isinstance(this._file, str):
+            this._file = this.filesystem.get(this._file)
+            this.image = this._file.read()
         else:
             raise TypeError('image must be PIL.Image.Image, Waltex, or filesystem.File.')
         
+        this._textureSettings = TextureSettings(
+            filesystem = this.filesystem,
+            gamepath = this.gamepath,
+            assets = this.assets,
+            baseassets = this.baseassets,
+        )
+
+        this.textureSettings = this._textureSettings.get(this.filename)
+
+        # if not this.textureSettings.premultiplyAlpha:
+        #     this.image = this.image.convert('RGBa')
+
     @property
-    def size(this):
+    def size(this) -> tuple[int,int]:
+        """The size of the image.
+        Returns:
+            tuple[int,int]: (width,height)
+        """
         return this.image.size
 
-class HDFile(GameObject):
-    def __init__(
-        this,
-        file : str | File,
-        HD : bool = True,
-        TabHD : bool = False, 
-        filesystem: Filesystem | Folder = None,
-        gamepath: str = None,
-        assets: str = '/assets',
-        baseassets: str = '/',
-    ) -> None:
-        super().__init__(filesystem, gamepath, assets, baseassets)
-        
-        if isinstance(file, File):
-            this.file = file.path
-        elif isinstance(file, str):
-            this.file = file
+    def save(this, filename : str = None) -> File:
+        """Save the image to the filesystem.
+        Args:
+            filename (str, optional): Path to save the image to. Defaults to None.
+        Returns:
+            File: wmwpy File object.
+        """
+        if filename == None:
+            filename = this.filename
         else:
-            raise TypeError('file must be a File or str')
+            this.filename = filename
 
-        this.HD = HD
-        this.TabHD = TabHD
+        fileio = io.BytesIO()
+
+        this.image.save(fileio, format = os.path.splitext(filename)[1][1:].upper())
+
+        file = this.filesystem.add(filename, fileio, replace = True)
+
+        return file
     
-    @property
-    def filename(this) -> str:
-        name, extension = os.path.splitext(this.file)
+    def show(self, *args, **kwargs):
+        """Calls the PIL.Image.Image.show() method.
         
-        if this.TabHD:
-            filename = f'{name}-TabHD{extension}'
-            if this.filesystem == None:
-                return filename
-
-            if this.filesystem.exists(filename):
-                return filename
+        ---
+        #### Description copied from the PIL library
         
-        if this.HD:
-            filename = f'{name}-HD{extension}'
-            if this.filesystem == None:
-                return filename
+        Displays this image. This method is mainly intended for debugging purposes.
 
-            if this.filesystem.exists(filename):
-                return filename
-        
-        return this.file
+        This method calls PIL.ImageShow.show internally. You can use
+        PIL.ImageShow.register to override its default behavior.
 
-def getHDFile(
-    file : str,
-    HD = True,
-    TabHD = False,
-    filesystem : Filesystem = None,
-    gamepath : str = None,
-    assets : str = '/assets',
-    baseassets : str = '/',
-) -> str:
-    """Get HD filename.
-
-    Args:
-        file (str): Filename. Must be a string.
-        HD (bool, optional): 
-
-    Returns:
-        str: HD filename.
-    """
-    return HDFile(
-        file = file,
-        HD = HD,
-        TabHD = TabHD,
-        filesystem = filesystem,
-        gamepath = gamepath,
-        assets = assets,
-        baseassets = baseassets,
-    ).filename
-            
-def getTexture(
-    path : str,
-    textureSettings : dict,
-    size : tuple,
-    cache = True
-) -> Image.Image:
-    """Get image.
-
-    Args:
-        path (str): Path to Image.
-        textureSettings (dict): Texture settings.
-        size (tuple[width,height]): Size of image.
-        cache (bool, optional): Whether to cache waltex images. Defaults to True.
-
-    Returns:
-        Image.Image: PIL Image.
-    """
-    type = os.path.splitext(path)[1][1:]
-    image = None
-    if type == 'waltex':
-        if cache:
-            try:
-                image = _cachedWaltextImages[path].copy()
-            except:
-                pass
-        if image == None:
-            image = Waltex(
-                path
-            ).image
-            if cache:
-                _cachedWaltextImages[path] = image.copy()
-    else:
-        image = Image.open(path).convert('RGBA')
-        
-    return image
-    
-def getTextueSettings(gamepath : str, assets : str, textureSettings : str, name : str, ) -> dict:
-    """Get the texture settings of a texture.
-    
-    Really needs an update, as now I can reliably get the path to the file using the `baseassets` property in the `Game` object.
+        The image is first saved to a temporary file. By default, it will be in PNG format.
 
-    Args:
-        gamepath (str): Path to game
-        assets (str): Relative path from the gamepath to the assets folder.
-        textureSettings (str): Path to `TextureSettings.xml` file
-        name (str): Name of image to look for.
-
-    Returns:
-        dict: The texture settings as a dict.
-    """
-    fullpath = joinPath(gamepath, assets, textureSettings)
-    xml = etree.parse(fullpath).getroot()
-    
-    Texture = etree.ElementBase()
-    for i in xml:
-        if not i.tag is etree.Comment:
-            if i.tag == 'Texture' and i.get('name') == name:
-                Texture = i
-                break
-            
-    attributes = {
-        'colorspace': 'RGBA4444',
-        'premultiplyAlpha': False,
-        'dePremultiplyAlpha': False,
-    }
-    
-    values = Texture.attrib
-    
-    for key in values:
-        attributes[key] = values[key]
-    
-    return attributes
+        On Unix, the image is then opened using the **display**, **eog** or **xv** utility, depending on which one can be found.
+
+        On macOS, the image is opened with the native Preview application.
+
+        On Windows, the image is opened with the standard PNG display utility.
+
+        Args:
+            title (str | None, optional): Optional title to use for the image window, where possible.. Defaults to None.
+        """
+        return self.image.show(*args, **kwargs)
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.5.0b0/src/wmwpy/utils/waltex.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 class Waltex():
     format = 'waltex'
     format_description = "Walaber image file"
 
     def __init__(
         this,
         file : str | bytes,
-        byte_order : str = 'little'
+        byte_order : str = 'little',
     ) -> None:
         """Waltex image
 
         Args:
             file (str | bytes): Waltex file. Can be path to file, contents of file as bytes, or file-like object.
             byte_order (str, optional): 'little' or 'big'. Defaults to 'little'.
 
@@ -105,29 +105,33 @@
         """
         
         this._colorspecs = [
             {
                 'order': 'rgba',
                 'bpp': [8,8,8,8],
                 'spec': 'rgba8888',
+                'byte_order': 'big',
             },
             {
                 'order': 'rgb',
                 'bpp': [5,6,5],
                 'spec': 'rgb565',
+                'byte_order': 'little',
             },
             {
                 'order': 'rgba',
                 'bpp': [5,5,5,1],
                 'spec': 'rgba5551',
+                'byte_order': 'little',
             },
             {
                 'order': 'rgba',
                 'bpp': [4,4,4,4],
                 'spec': 'rgba4444',
+                'byte_order': 'little',
             },
         ]
         
         if isinstance(file, (str)):
             with open(file, 'rb') as f:
                 rawdata = f.read()
                 
@@ -142,15 +146,15 @@
             raise TypeError(f"file has to be a 'str', 'bytes' or file-like object.")
         
         this._byte_order = byte_order
         
         this.file = file
         this.rawdata = io.BytesIO(rawdata)
         
-        this.read(byte_order=this._byte_order)
+        this.read()
     
     def read(this, byte_order : str = None) -> Image.Image:
         """Read the waltex image.
 
         Args:
             byte_order (str, optional): The byte order. Can be 'little' or 'big'. Defaults to None.
 
@@ -164,21 +168,24 @@
             
         this.format = int(header[5])
         this.colorspec = this._colorspecs[this.format]
         this.version = int(header[4])
         size = (int.from_bytes(header[6:8], byteorder='little'), int.from_bytes(header[8:10], byteorder='little'))
         this.image = Image.new('RGBA', size)
         
+        if not byte_order:
+            this._byte_order = this.colorspec['byte_order']
+        
         try:
             this.image = Image.open(this.rawdata)
-            if byte_order == 'little':
+            if this._byte_order == 'little':
                 A, B, G, R = this.image.split()
                 this.image = Image.merge('RGBA', (R,G,B,A))
         except:
-            this.image = WaltexImage(this.rawdata, byte_order = byte_order)
+            this.image = WaltexImage(this.rawdata, byte_order = this._byte_order)
         
         this.image.format = _WaltexImageFile.format
         this.image.format_description = _WaltexImageFile.format_description
         return this.image
     
     @property
     def size(this):
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/__init__.py` & `wmwpy-0.5.0b0/src/wmwpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-__version__ = "0.4.1-beta"
+__version__ = "0.5.0-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
 import logging
 
-from .game import Game
-from . import Utils
+from . import utils
 from . import classes
 from . import Font
 from .classes import widget
 from .gametemplate import GAMES
-from .Utils import filesystem
+from .utils import filesystem
+from .game import Game
 
-__all__ = ['load', 'Game', 'Utils', 'classes', 'GAMES', 'filesystem']
+__all__ = ['load', 'Game', 'utils', 'classes', 'GAMES', 'filesystem']
 
 def load(
     gamepath : str,
     platform : typing.Literal['android', 'ios'] = 'android',
     game : str = 'WMW',
     assets : str = None,
     db : str = None,
@@ -25,20 +25,20 @@
     load_callback : typing.Callable[[int, str, int], typing.Any] = None,
 ) -> Game:
     """load game
 
     Args:
         gamepath (str): Folder to extracted game.
         platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
-        game (str, optional): Which game is being loaded. A full list of games is in the `gametemplate.GAMES` variable. Defaults to 'WMW'. 
+        game (str, optional): Which game is being loaded. A full list of games is in `gametemplate.GAMES`. Defaults to 'WMW'. 
         assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
         db (str, optional): Relative path to database file from assets folder. Defaults to '/Data/water.db'.
-        profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`
-        baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
-        hook (Callable[[int, str, int], Any], optional): Hook for loading assets, useful for guis. The function gets called with the paramaters `(progress : int, current : str, max : int)`. Defaults to None.
+        profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`.
+        baseassets (str, optional): Base assets path within the assets folder, e.g. '/perry/' in wmp. Defaults to '/'.
+        load_callback (Callable[[int, str, int], Any], optional): A callback function to be ran while loading the game. Defaults to `None`.
     """
     
     game = game.upper()
     platform = platform.lower()
     
     platforms = {
         'android': {
@@ -57,16 +57,7 @@
         gamepath = gamepath,
         assets = assets,
         db = db,
         profile = profile,
         load_callback = load_callback,
         baseassets = baseassets,
     )
-    # except:
-    #     return Game(
-    #         gamepath = gamepath,
-    #         assets = assets,
-    #         db = db,
-    #         profile = profile,
-    #         load_callback = load_callback,
-    #         baseassets = baseassets,
-    #     )
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/Widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import lxml
 from lxml import etree
 from PIL import Image
-from ..Utils.waltex import WaltexImage
+from ..utils.waltex import WaltexImage
 from .widget import Widget
 
 class Widgets():
     def __init__(this, element : etree.Element, gamePath : str, screenSize = (), texturePath : str = None, baseLayoutFile : str = None) -> None:
         this.element = element
         
         this.attributes = this.element.attrib
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/curves.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/imagelist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from ..Utils.textures import getHDFile, getTextueSettings, getTexture
-from ..Utils.filesystem import *
-from ..Utils import joinPath, Texture
+from .texture import Texture
+from ..utils.textures import getHDFile, HDFile
+from ..utils.filesystem import *
+from ..utils.path import joinPath
 from ..gameobject import GameObject
 
 import numpy
 import PIL.Image
 from lxml import etree
 from copy import deepcopy
 
@@ -34,65 +35,83 @@
         """Get imagelist from file
         
         Args:
             file (str | bytes | File, optional): File to read. Defaults to None.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
-            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`.
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
+            save_images (bool, optional): Save images in filesystem. Note: this may take more time to load the imagelist. Defaults to False.
         
         Raises:
             FileNotFoundError: Filesystem is not usable and no gamepath.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
         
         this.HD = HD
         this.TabHD = TabHD
         
         if isinstance(file, str):
-            file = getHDFile(
+            this.filename = file
+            newFile = HDFile(
                 file,
                 HD = this.HD,
                 TabHD = this.TabHD,
                 filesystem = this.filesystem,
                 gamepath = this.gamepath,
                 assets = this.assets,
                 baseassets = this.baseassets,
             )
+
+            file = newFile.filename
+            this.HD = newFile.HD
+            this.TabHD = newFile.TabHD
         elif isinstance(file, File):
-            file = getHDFile(
+            this.filename = file.path
+            newFile = HDFile(
                 file.path,
                 HD = this.HD,
                 TabHD = this.TabHD,
                 filesystem = this.filesystem,
                 gamepath = this.gamepath,
                 assets = this.assets,
                 baseassets = this.baseassets,
             )
+
+            file = newFile.filename
+            this.HD = newFile.HD
+            this.TabHD = newFile.TabHD
+        else:
+            this.filename = ''
         
         if isinstance(file, str):
             file = this.filesystem.get(file)
         
         this.file = super().get_file(file, template = this.TEMPLATE)
 
+        if isinstance(this.file, io.BytesIO):
+            this.file.seek(0)
+        
         this.xml : etree.ElementBase = etree.parse(this.file).getroot()
         
         this.pages : list[Imagelist.Page] = []
         this.format = this.Format.IMAGELIST
-        this.filename = ''
 
         # this.images = {}
 
         this.read(save_images = save_images)
     
     def read(this, save_images : bool = False):
         """Read the imagelist xml.
+
+        Args:
+            save_images (bool, optional): Save images in filesystem. Note: this may take more time to load the imagelist. Defaults to False.
         """
         this.format = this.Format.IMAGELIST
         
         for element in this.xml:
             if element is etree.Comment:
                 continue
             
@@ -115,20 +134,30 @@
                 HD = this.HD,
                 TabHD = this.TabHD,
                 save_images = save_images,
             )
             
             this.pages.append(page)
     
+    def update(this, gap : tuple[int,int] = (1,1), auto_fit = False):
+        """Update the atlas image.
+
+        Args:
+            gap (tuple[int,int], optional): The gap between images. Defaults to (1,1).
+            auto_fit (bool, optional): Auto minimize the atlas image size while keeping all the sprites in the image. Defaults to False.
+        """
+        for page in this.pages:
+            page.update(gap = gap, auto_fit = auto_fit)
+    
     def export(
         this,
         path : str = None,
-        exportImage : bool = False,
-        imageFormat : str = 'webp',
-        removeImageFiles : bool = False,
+        exportImage : bool = True,
+        format : str = 'webp',
+        removeImageFiles : bool = True,
     ):
         """Export the xml of the imagelist.
 
         Args:
             path (str, optional): Path to the file in the filesystem to write to. If `None`, it will not save to a file, only report the output. Defaults to None.
             exportImage (bool, optional): Whether to also export the atlas image(s). If there are multiple pages, it'll append `_split_#` to the end of the filenames. Defaults to False.
             imageFormat (str, optional): What format to export the images as. Defaults to 'webp'.
@@ -142,59 +171,72 @@
         """
         if path == None:
             if this.filename:
                 path = this.filename
         else:
             this.filename = path
         
+        # if path != None:
+        #     path = getHDFile(
+        #         path,
+        #         HD = this.HD,
+        #         TabHD = this.TabHD,
+        #     )
+        
         if removeImageFiles:
             this.removeImageFiles()
         
         if path != None:
             if exportImage:
                 if this.format == this.Format.PAGES:
                     index = 0
                     for page in this.pages:
                         index += 1
                         
                         filename = os.path.splitext(path)[0]
-                        filename = f'{filename}_split_{str(index)}.{imageFormat}'
+                        filename = f'{filename}_split_{str(index)}.{format}'
                         
                         page.file = filename
-                        page.exportAtlas(filename = getHDFile(filename, this.HD, this.TabHD), format = imageFormat)
+                        page.exportAtlas(filename = filename, format = format)
                         
                 else:
                     page = this.pages[0]
                     
                     filename = os.path.splitext(path)[0]
-                    filename = f'{filename}.{imageFormat}'
+                    filename = f'{filename}.{format}'
                     
                     page.file = filename
-                    page.exportAtlas(filename = getHDFile(filename, this.HD, this.TabHD), format = imageFormat)
+                    page.exportAtlas(filename = filename, format = format)
         
         if this.format == this.Format.IMAGELIST:
             page = this.pages[0]
-            xml = page.getXML(type = this.format)
+            xml = page.getXML(format = this.format)
         else:
             xml = etree.Element('Imagelist')
             for page in this.pages:
-                xml.append(page.getXML(type = this.format))
+                xml.append(page.getXML(format = this.format))
             
-        output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
+        xmloutput = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
         
         if path != None:
+            path = getHDFile(path, HD = this.HD, TabHD = this.TabHD)
+            
             if (file := this.filesystem.get(path)) != None:
                 if isinstance(file, Folder):
                     raise TypeError(f'Path {path} is not a file.')
                 
-                file.write(output)
+                file.write(xmloutput)
                 
             else:
-                file = this.filesystem.add(path, output)
+                file = this.filesystem.add(path, xmloutput)
         
+        output = {
+            'xml' : xmloutput,
+            'images' : [a.atlas for a in this.pages]
+        }
         
         return output
     
     def combinePages(this):
         """Combine all the pages in this Imagelist into 1 Page
         """
         if this.format == this.Format.IMAGELIST:
@@ -214,15 +256,46 @@
                 
         main.id = None
         main.exportAtlas()
         
         this.format = this.Format.IMAGELIST
         
         this.pages = [main]
-                
+    
+    def add(
+        this,
+        name : str,
+        image : PIL.Image.Image,
+        properties : dict = {},
+        page : int | str = 0,
+        replace = False
+    ):
+        """Add image to imagelist.
+
+        Args:
+            name (str): Name of image file used in-game.
+            image (PIL.Image.Image): Image to use.
+            properties (dict, optional): Additional properties for image. Defaults to {}.
+            replace (bool, optional): Whether to replace existing image if there is a conflict. Defaults to False.
+
+        Raises:
+            NameError: Image already exists.
+        
+        Returns:
+            Imagelist.Page.Image: Resulting imagelist image.
+        """
+        page : Imagelist.Page = this.getPage(page)
+        
+        if page != None:
+            return page.add(
+                name = name,
+                image = image,
+                properties = properties,
+                replace = replace,
+            )
     
     def get(this, name : str):
         """Get image from imagelist.
 
         Args:
             name (str): Name of image.
 
@@ -240,14 +313,34 @@
     
     def removeImageFiles(this):
         """Remove all image files in imagelist from filesystem.
         """
         for page in this.pages:
             page.removeImageFiles()
     
+    def getPage(this, id : int | str = 0) -> 'Imagelist.Page':
+        """Get the page with this id / index.
+
+        Args:
+            id (int | str, optional): The id or index of the page. Defaults to 0.
+
+        Raises:
+            TypeError: id must be int or str
+
+        Returns:
+            Imagelist.Page: The page that has the id or index.
+        """
+        if isinstance(id, (int, float)):
+            id = int(id)
+            return this.pages[id]
+        elif isinstance(id, str):
+            return [p for p in this.pages if p.id == id][0]
+        else:
+            raise TypeError('id must be int or str')
+    
     class Page(GameObject):
         def __init__(
             this,
             element : etree.ElementBase,
             filesystem: Filesystem | Folder = None,
             gamepath: str = None,
             assets: str = '/assets',
@@ -259,14 +352,15 @@
 
             Args:
                 element (etree.Element): lxml elment
                 filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
                 gamepath (str, optional): Gamepath used if filesystem is not specified. Defaults to None.
                 assets (str, optional): Assets path relative to gamepath. Only used if filesystem is not specified. Defaults to '/assets'.
                 HD (bool, optional): Use HD graphics. Defaults to False.
+                save_images (bool, optional): Save images in filesystem. Note: this may take more time to load the imagelist. Defaults to False.
             """
             super().__init__(filesystem, gamepath, assets)
             
             this.HD = HD
             this.TabHD = TabHD
             
             this.xml : etree.ElementBase = element
@@ -275,14 +369,17 @@
             this.images : list[Imagelist.Page.Image] = []
             this.properties : dict[str,str] = {}
             
             this.read(save_images = save_images)
         
         def read(this, save_images : bool = False):
             """Read xml.
+            
+            Args:
+                save_images (bool, optional): Save images in filesystem. Note: this may take more time to load the imagelist. Defaults to False.
             """
             this.properties = deepcopy(this.xml.attrib)
     
             # if this.gamepath:
             #     this.fullAtlasPath = joinPath(this.gamepath, this.assets, this.file)
                 # print(this.fullAtlasPath)
     
@@ -299,15 +396,15 @@
             if 'imgSize' in this.properties:
                 return tuple([int(v) for v in this.properties['imgSize'].split()])
             else:
                 return (1,1)
         @imgSize.setter
         def imgSize(this, size : tuple | list | str):
             if isinstance(size, (list, tuple)):
-                this.properties['imgSize'] = ''.join([str(a) for a in size])
+                this.properties['imgSize'] = ' '.join([str(a) for a in size])
             elif isinstance(size, str):
                 this.properties['imgSize'] = size
             else:
                 raise TypeError('size must be a tuple, list, or str')
     
         @property
         def textureBasePath(this) -> str:
@@ -322,29 +419,22 @@
                 this.textureBasePath = joinPath(this.filesystem.baseassets, '/Textures/')
                 return this.textureBasePath
         @textureBasePath.setter
         def textureBasePath(this, path):
             this.properties['textureBasePath'] = path
         
         @property
-        def file(this):
+        def file(this) -> str:
             """The path to the atlas file to use in this ImageList
 
             Returns:
                 str: Path to atlas file.
             """
             if 'file' in this.properties:
-                return getHDFile(
-                    this.properties['file'],
-                    HD = this.HD,
-                    TabHD = this.TabHD,
-                    filesystem = this.filesystem,
-                    assets = this.assets,
-                    baseassets = this.baseassets,
-                )
+                return this.properties['file']
             else:
                 return ''
         @file.setter
         def file(this, path):
             this.properties['file'] = path
         
         @property
@@ -365,24 +455,30 @@
             else:
                 this.properties['id'] = str(value)
     
         def getAtlas(this):
             """Get atlas image.
             """
             if this.file in ['', None]:
-                image = Texture(PIL.Image.new('RGBA', this.imgSize))
-                this.atlas = image.image.copy()
-                
-            elif this.filesystem.exists(this.file):
-                file = this.filesystem.get(this.file)
-                image = Texture(file.read())
-                this.atlas = image.image.copy()
+                this.atlas = Texture(PIL.Image.new('RGBA', this.imgSize)).image
+            else:
+                this.atlas = Texture(
+                    this.file,
+                    HD = this.HD,
+                    TabHD = this.TabHD,
+                    filesystem = this.filesystem,
+                    gamepath = this.gamepath,
+                    assets = this.assets,
+                    baseassets = this.baseassets,
+                ).image
     
         def getImages(this, save_images = False):
             """Get images from xml.
+            Args:
+                save_images (bool, optional): Save images in filesystem. Note: this may take more time to load the imagelist. Defaults to False.
             """
             for element in this.xml:
                 if element is etree.Comment:
                     continue
                 
                 if element.tag == 'Image':
                     image = this.Image(
@@ -407,113 +503,144 @@
                 if image.name == name:
                     return image
         
         def add(this,
                 name : str,
                 image : PIL.Image.Image,
                 properties : dict = {},
-                replace = False
-            ):
+                replace = False,
+            ) -> 'Imagelist.Page.Image':
             """Add image to imagelist.
 
             Args:
                 name (str): Name of image file used in-game.
                 image (PIL.Image.Image): Image to use.
                 properties (dict, optional): Additional properties for image. Defaults to {}.
                 replace (bool, optional): Whether to replace existing image if there is a conflict. Defaults to False.
 
             Raises:
                 NameError: Image already exists.
+            
+            Returns:
+                Imagelist.Page.Image: Resulting imagelist image.
             """
             if name in this.images:
                 # print(f'Warning: "{name}" already in imagelist.')
                 if not replace:
                     raise NameError(f'Image "{name}" already exists.')
             properties['name'] = name
             properties['rect'] = ' '.join([str(_) for _ in (0,0) + image.size])
             
             texture = this.Image(
                 image,
-                properties
+                properties,
+                textureBasePath = this.textureBasePath,
+                filesystem = this.filesystem,
+                gamepath = this.gamepath,
+                assets = this.assets,
+                save_image = True,
             )
             this.images.append(texture)
             
             this._getRects()
+            
+            return texture
         
-        def exportAtlas(this, filename = None, gap : tuple = (1,1), format : str = 'webp', ):
+        def update(this, gap : tuple[int,int] = (1,1), auto_fit = False):
+            """Update the atlas image.
+
+            Args:
+                gap (tuple[int,int], optional): The gap between images. Defaults to (1,1).
+                auto_fit (bool, optional): Auto minimize the atlas image size while keeping all the sprites in the image. Defaults to False.
+            """
+            for image in this.images:
+                image.getImage()
+            
+            this._getRects(gap = gap, auto_fit = auto_fit)
+            this._updateAtlas()
+            
+            return this.atlas
+        
+        def exportAtlas(this, filename = None, gap : tuple = (1,1), auto_fit = False, format : str = 'webp', ):
             """Export the atlas image into the Filesystem. This function recreates the imagelist, so you need to also export the xml using `getXML()`.
 
             Args:
                 gap (tuple, optional): Gap between each image. Defaults to (1,1).
                 filename (str, optional): Filename of image. Defaults to `file` property.
+                auto_fit (bool, optional): Auto minimize the atlas image size while keeping all the sprites in the image. Defaults to False.
                 format (str, optional): Format to save image as. Defaults to 'webp'.
 
             Returns:
                 PIL.Image.Image: PIL Image.
             """
-            this._getRects(gap = gap)
-            this._updateAtlas()
+            this.update(gap = gap, auto_fit = auto_fit)
             file = io.BytesIO()
             
-            this.atlas.save(file, format=format)
+            this.atlas.save(file, format=format, lossless = True, exact = True)
             
             if filename == None:
                 filename = f'{os.path.splitext(this.file)[0]}.{format}'
             
             this.file = filename
             
+            filename = getHDFile(filename, this.HD, this.TabHD)
+            
             if this.filesystem.exists(filename):
                 this.filesystem.get(filename).rawdata = file
             else:
                 this.filesystem.add(filename, file.getvalue())
             
             return this.atlas
         
-        def getXML(this, filename = None, type : int = 1):
+        def getXML(this, filename = None, format : int = 1):
             """Generates the xml for the page / imagelist.
 
             Args:
                 filename (str, optional): Name of image. Defaults to file property.
-                type (int, optional): Type of file. 0 for `Page`, 1 for `Imagelist`. Defaults to 1.
+                format (int, optional): Format of file. 0 for `Imagelist`, 1 for `Page`. Defaults to 1.
 
             Returns:
                 lxml.etree.Element: lxml Element.
             """
             if filename != None:
                 this.file = filename
             
-            tag = 'Page' if type else 'Imagelist'
+            tag = 'Page' if format else 'ImageList'
+            
+            this.imgSize = this.atlas.size
+            
             
             xml : etree.ElementBase = etree.Element(tag, **this.properties)
             
             for image in this.images:
                 xml.append(image.getXML())
             
             this.xml = xml
             return this.xml
         
         def removeImageFiles(this):
             """Remove all image files from filesystem.
             """
-            for name in this.images:
-                this.images.removeFile()
+            for image in this.images:
+                image.removeFile()
             
         
-        def _getRects(this, gap : tuple = (1,1)):
+        def _getRects(this, gap : tuple = (1,1), auto_fit = False):
             """Update the rect for all images.
 
             Args:
                 gap (tuple, optional): Gap between images. Defaults to (1,1).
+                auto_fit (bool, optional): Auto minimize the atlas image size while keeping all the sprites in the image. Defaults to False.
             """
+
             x, y = gap
             maxheight = maxwidth = 0
             row = column = 0
             
             for image in this.images:
-                image = this.images[image]
                 image.rect = (x,y) + image.size
                 
                 if x > maxwidth:
                     maxwidth = x
                 
                 x += image.size[0] + gap[0]
                 
@@ -530,61 +657,77 @@
                     x += image.size[0] + gap[0]
                 
                 if image.size[1] > maxheight:
                     maxheight = image.size[1]
             
             y += maxheight + gap[1]
             
-            if y > this.imgSize[1]:
+            if auto_fit:
+                this.imgSize = (maxwidth,y)
+            elif y > this.imgSize[1]:
                 this.imgSize = (this.imgSize[0], y)
             
                 
-        def _updateAtlas(this):
+        def _updateAtlas(this) -> PIL.Image.Image:
+            """Update the atlas image.
+
+            Returns:
+                PIL.Image.Image: PIL Image.
+            """
             atlas : PIL.Image.Image = PIL.Image.new('RGBA', this.imgSize)
             
             for image in this.images:
-                image = this.images[image]
                 image.atlas = atlas
                 atlas.paste(image.image, image.rect[0:2])
             
             this.atlas = atlas
+            
+            # this.atlas = Texture(
+            #     atlas,
+            #     filesystem = this.filesystem,
+            #     gamepath = this.gamepath,
+            #     assets = this.assets,
+            #     baseassets = this.baseassets,
+            #     HD = this.HD,
+            #     TabHD = this.TabHD,
+            # )
             return this.atlas
     
         class Image(GameObject):
             def __init__(
                 this,
                 atlas : PIL.Image.Image,
                 properties : dict,
                 textureBasePath = '/Textures',
                 filesystem: Filesystem | Folder = None,
                 gamepath: str = None,
                 assets: str = '/assets',
+                baseassets : str = '/',
                 save_image : bool = False,
             ) -> None:
                 """Image for Imagelist
 
                 Args:
                     atlas (PIL.Image.Image): Atlas file containing all images
                     properties (dict): Properties for Image.
                     filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
                     gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
                     assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+                    baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+                    save_image (bool, optional): Save the current image in the filesystem on load. Defaults to False.
                 """
-                super().__init__(filesystem, gamepath, assets)
+                super().__init__(filesystem, gamepath, assets, baseassets)
 
                 this.atlas = atlas
                 this.properties = deepcopy(properties)
                 this.textureBasePath : str = textureBasePath
-
-                this.image = PIL.Image.new('RGBA', this.size)
-
                 this.rawdata = io.BytesIO()
-                
+
                 this._image = None
-                
+
                 if save_image:
                     this.getImage()
             
             @property
             def size(this) -> tuple[int,int]:
                 """The size of the image.
 
@@ -654,15 +797,15 @@
                 elif isinstance(value, str):
                     this.properties['rect'] = value
                 else:
                     raise TypeError('value must be tuple, list or str')
             
             @property
             def name(this) -> str:
-                """The name of the iamge
+                """The name of the image
 
                 Returns:
                     str: image name
                 """
                 if 'name' in this.properties:
                     return this.properties['name']
                 else:
@@ -670,14 +813,19 @@
                     return this.name
             @name.setter
             def name(this, name : str):
                 this.properties['name'] = str(name)
             
             @property
             def image(this):
+                """The resulting PIL Image.
+
+                Returns:
+                    PIL.Image.Image: PIL Image.
+                """
                 if this._image == None:
                     this.getImage()
                 
                 return this._image.copy()
             
             @image.setter
             def image(this, image : PIL.Image.Image):
@@ -691,26 +839,45 @@
                 """
                 this._image = this.atlas.crop(numpy.add(this.rect, (0,0) + this.rect[0:2]))
                 this._image = this._image.resize(this.size)
                 
                 this._image.save(this.rawdata, format = os.path.splitext(this.name)[1][1::].upper())
                 return this._image
 
-            def show(this):
-                """Show image with default image viewer.
+            def show(this, *args, **kwargs):
+                """Calls the PIL.Image.Image.show() method.
+                
+                ---
+                #### Description copied from the PIL library
+                
+                Displays this image. This method is mainly intended for debugging purposes.
+
+                This method calls PIL.ImageShow.show internally. You can use
+                PIL.ImageShow.register to override its default behavior.
+
+                The image is first saved to a temporary file. By default, it will be in PNG format.
+
+                On Unix, the image is then opened using the **display**, **eog** or **xv** utility, depending on which one can be found.
+
+                On macOS, the image is opened with the native Preview application.
+
+                On Windows, the image is opened with the standard PNG display utility.
+
+                Args:
+                    title (str | None, optional): Optional title to use for the image window, where possible.. Defaults to None.
                 """
-                this.image.show()
+                this.image.show(*args, **kwargs)
             
-            def getXML(this):
+            def getXML(this, tag = 'Image'):
                 """Get xml for image.
 
                 Returns:
                     lxml.etree.Element: lxml element
                 """
-                xml : etree.ElementBase = etree.Element('Image', **this.properties)
+                xml : etree.ElementBase = etree.Element(tag, **this.properties)
                 
                 return xml
             
             def removeFile(this):
                 """Remove file from filesystem.
                 """
                 return this.filesystem.remove(this.filename)
@@ -725,17 +892,26 @@
                 this.image.save(this.rawdata, os.path.splitext(this.name)[1][1::])
                 this.filesystem.add(
                     this.name,
                     content = this.rawdata.getvalue(),
                     replace = replace,
                 )
             
-            
             @property
             def filename(this) -> str:
                 """Image filepath in the Filesystem
 
                 Returns:
                     str: Full filepath in the Filesystem
                 """
-                return this.filesystem.get(this.name).path
+                file = this.filesystem.get(this.name)
+                if file != None:
+                    return file.path
+                
+                return this.name
+            
+            def __str__(self) -> str:
+                return etree.tostring(self.getXML()).decode()
+
+            def __repr__(self) -> str:
+                return etree.tostring(self.getXML(f'{self.__class__.__module__}.{self.__class__.__qualname__}')).decode()
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/layout.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..gameobject import GameObject
-from ..Utils.filesystem import *
+from ..utils.filesystem import *
 from .widget import get_widget
 
 class Layout(GameObject):
     def __init__(
         this,
         file  : str | bytes | File = None,
         filesystem: Filesystem | Folder = None,
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/level.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/level.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,33 @@
 if LOADED_ImageTk:
     try:
         from PIL import ImageTk
     except:
         LOADED_ImageTk = False
 
 
-from ..Utils.filesystem import *
-from ..Utils.logging_utils import log_exception
+from ..utils.filesystem import *
+from ..utils.logging_utils import log_exception
 from .object import Object
 from ..gameobject import GameObject
+from .objectpack.pack import ObjectPack
 
 class Level(GameObject):
+    """
+    The Level object.
+    
+    Attributes:
+        HD (bool): Using HD graphics
+        TabHD (bool): Using TabHD graphics.
+        object_pack (ObjectPack): The ObjectPack that is being used for all the objects.
+        objects (list[Object]): List of Objects currently in this level.
+        properties (dict[str,str]:) All the Level properties.
+        challenges (list[Level.Challenge]): List of WMW2 challenges in this level.
+        room (tuple[float,float]): The room element in WMW levels. I have no idea what this does, but it still should be kept, even though it doesn't actually do anything.
+    """
     XML_TEMPLATE = b"""<?xml version="1.0"?>
     <Objects>
     </Objects>
     """
     
     IMAGE_TEMPLATE = Image.new('P', (90,127), 'white').quantize(colors=256)
     IMAGE_FORMAT = 'PNG'
@@ -37,14 +50,15 @@
         gamepath : str = None,
         assets : str = '/assets',
         baseassets : str = '/',
         load_callback : typing.Callable[[int, str, int], typing.Any] = None,
         ignore_errors : bool = False,
         HD : bool = False,
         TabHD : bool = False,
+        object_pack : ObjectPack = None
     ) -> None:
         """Load level
 
         Args:
             xml (str | bytes | File): XML file for level.
             image (str | bytes | File): Image file for level.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
@@ -88,14 +102,16 @@
             this.image = this.IMAGE_TEMPLATE.copy()
         else:
             this.image = Image.open(this.image_file).quantize(colors=256)
         
         this.HD = HD
         this.TabHD = TabHD
         
+        this.object_pack = object_pack
+        
         this.objects : list[Object] = []
         this.properties : dict[str,str] = {}
         this.challenges : list[Level.Challenge] = []
         this.room = (0,0)
         
         this.read(load_callback = load_callback, ignore_errors = ignore_errors)
         
@@ -210,14 +226,15 @@
                         this.filesystem.get(properties['Filename']), # get file because `Object` does not take filepath
                         filesystem = this.filesystem,
                         properties = properties,
                         pos = pos,
                         name = name,
                         HD = this.HD,
                         TabHD = this.TabHD,
+                        object_pack = this.object_pack,
                     )
                     
                     obj.id = id
                     
                     this.objects.append(obj)
                     
                     id += 1
@@ -355,26 +372,27 @@
     ):
         """Add object to level.
 
         Args:
             filename (str | Object): Filename for object. If it's a wmwpy.classes.Object class, then it will use that instead.
             properties (dict, optional): Object properties. Defaults to {}.
             pos (tuple[x,y], optional): Position of object in level. Defaults to (0,0).
-            name (str, optional): Name of object. May get renamed if object with name alread exists. Defaults to 'Obj'.
+            name (str, optional): Name of object. May get renamed if object with name already exists. Defaults to 'Obj'.
 
         Returns:
             Object: wmwpy Object.
         """
         if not isinstance(filename, Object):
             filename = Object(
                 filename,
                 filesystem = this.filesystem,
                 properties = properties,
                 pos = pos,
                 name = name,
+                object_pack = this.object_pack,
             )
         else:
             filename.name = name
             filename.pos = pos
             filename.setProperty(properties)
         
         obj = filename
@@ -465,15 +483,15 @@
             """
             if not isinstance(this.xml, etree._Element):
                 return
             
             this.id = this.xml.get('id', '')
             
             for element in this.xml:
-                # so I can acess the attributes in vscode
+                # so I can access the attributes in vscode
                 element : etree.ElementBase
                 
                 if element is etree.Comment:
                     continue
                 
                 requirement = copy.deepcopy(element.attrib)
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/object.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,67 @@
+from __future__ import annotations
+import typing
 import lxml
 from lxml import etree
 import io
 import os
 from copy import deepcopy
 from PIL import Image, ImageDraw
 import numpy
 import math
-import typing
 
 LOADED_ImageTk = True
 if LOADED_ImageTk:
     try:
         from PIL import ImageTk
     except:
         LOADED_ImageTk = False
 
 from ..gameobject import GameObject
 from .sprite import Sprite
-from ..Utils.filesystem import *
-from ..Utils.rotate import rotate
-from ..Utils.gif import save_transparent_gif
+from ..utils.filesystem import *
+from ..utils.rotate import rotate
+from ..utils.gif import save_transparent_gif
+if typing.TYPE_CHECKING:
+    from .objectpack import ObjectPack
 
-from ..Utils.XMLTools import strbool
+from ..utils.XMLTools import strbool
 class Object(GameObject):
+    """wmwpy Object.
+    
+    Attributes:
+        HD (bool): Using HD images.
+        TabHD (bool): Using TabHD images.
+        sprites (list[Sprite]): List of sprites.
+        shapes (list[Shape]): List of Shapes.
+        UVs (list[tuple[int,int]]): List of UVs (on the balloon object).
+        VertIndices (list[int]): List of VertIndices (on the balloon object).
+        defaultProperties (dict[str,str]): Dictionary of the object default properties (the ones in the object .hs files).
+        properties (dict[str,str]): Dictionary of the object properties (the ones in the level xml).
+        name (str): The object name.
+        id (int): The object id.
+        frame (int): The current animation frame.
+        object_pack (ObjectPack): The game Object Pack.
+        scale (float): The image scale.
+    """
+    
     def __init__(
         this,
         file : str | bytes | File,
         filesystem : Filesystem | Folder = None,
         gamepath : str = None,
         assets : str = '/assets',
         baseassets : str = '/',
         properties : dict = {},
         pos : tuple | str = (0,0),
         name : str = 'Obj',
         scale : int = 50,
         HD : bool = False,
         TabHD : bool = False,
+        object_pack : ObjectPack = None,
     ) -> None:
         """Get game object. Game object is `.hs` file.
 
         Args:
             file (str | bytes | File): Object file.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
@@ -47,21 +69,22 @@
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
             properties (dict, optional): Object properties that override default properties. Defaults to {}.
             pos (tuple | str, optional): Position of object. Defaults to (0,0).
             name (str, optional): Name of object. Defaults to 'Obj'.
             scale (int, optional): The image scale. Defaults to 10.
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
+            object_pack (ObjectPack, optional): The game Object Pack to use in this object. If None, it will not try to use any object types. Defaults to None.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
         
         this.file = super().get_file(file)
         
-        this._properties = deepcopy(properties)
+        this._level_properties = deepcopy(properties)
         if isinstance(pos, str):
             this.pos = tuple([float(a) for a in pos.split()])
         else:
             this.pos = tuple(pos)
         
         this.HD = HD
         this.TabHD = TabHD
@@ -74,28 +97,38 @@
         this.defaultProperties = {}
         this.properties = {}
         this.name = name
         this.size = (0,0)
         this.id = 0
         this.frame = 0
         
+        this.object_pack = object_pack
+        
         this._background : list[Sprite] = []
         this._foreground : list[Sprite] = []
         this._PhotoImage : dict[str, 'ImageTk.PhotoImage'] = {}
         
         this._offset = [0,0]
         this.scale = scale
         
         this.readXML()
         
+        this._properties = deepcopy(this.properties)
+        this.SAFE_MODE = False
+        
         if isinstance(file, File):
             this.filename = file.path
             
     @property
-    def frame(this):
+    def frame(this) -> int:
+        """The current animation frame.
+
+        Returns:
+            int: Current frame.
+        """
         return this._frame
     @frame.setter
     def frame(this, value : int):
         this._frame = value
         for sprite in this.sprites:
             sprite.frame = value
     
@@ -136,23 +169,66 @@
         min = numpy.array([math.floor(v.min()) for v in rects])
         max = numpy.array([math.ceil(v.max()) for v in rects])
         
         
         this.size = max - min
         this._offset = [a.mean() for a in numpy.array([min,max]).swapaxes(0,1)]
         
+        
+        
         return this._offset
     
+    
+    @property
+    def SAFE_MODE(this) -> bool:
+        """Safe mode allows the properties to be modified without carrying onto the level xml.
+
+        Returns:
+            bool: The current state.
+        """
+        if not hasattr(this, '_SAFE_MODE'):
+            this._SAFE_MODE = False
+        
+        this.SAFE_MODE = this._SAFE_MODE
+        return this._SAFE_MODE
+    
+    @SAFE_MODE.setter
+    def SAFE_MODE(this, mode : bool):
+        if not isinstance(mode, bool):
+            raise TypeError('mode must be True or False')
+        
+        if mode:
+            if not hasattr(this, '_SAFE_MODE') or not this.SAFE_MODE:
+                this._properties = deepcopy(this.properties)
+        else:
+            if not hasattr(this, '_SAFE_MODE') or this.SAFE_MODE:
+                this.properties = deepcopy(this._properties)
+        
+        for sprite in this.sprites:
+            sprite.SAFE_MODE = mode
+        
+        
+    @property
+    def Type(this):
+        if this.object_pack != None:
+            return this.object_pack.get_type(this.type, this)
+    
     @property
     def background(this) -> Image.Image:
         """The background image of this Object
 
         Returns:
             PIL.Image.Image: PIL Image
         """
+        this.SAFE_MODE = True
+        
+        type = this.Type
+        if type != None:
+            type.ready_sprites()
+        
         this.getOffset()
         
         image = Image.new('RGBA', tuple(this.size * this.scale), (0,0,0,0))
         
         for sprite in this._background:
             size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
             pos = this.truePos(
@@ -167,14 +243,15 @@
             
             image.alpha_composite(
                 sprite.image,
                 tuple([round(x) for x in pos]),
             )
         image = this.rotateImage(image)
         
+        this.SAFE_MODE = False
         return image
     
     @property
     def background_PhotoImage(this) -> 'ImageTk.PhotoImage':
         """Tkinter PhotoImage of this Object
 
         Returns:
@@ -190,14 +267,20 @@
     @property
     def foreground(this) -> Image.Image:
         """The foreground of the Object image
 
         Returns:
             PIL.Image.Image: PIL Image
         """
+        this.SAFE_MODE = True
+        
+        type = this.Type
+        if type != None:
+            type.ready_sprites()
+        
         this.getOffset()
         image = Image.new('RGBA', tuple(this.size * this.scale), (0,0,0,0))
         
         for sprite in this._foreground:
             size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
             pos = this.truePos(
                 sprite.pos,
@@ -211,19 +294,20 @@
             
             image.alpha_composite(
                 sprite.image,
                 tuple([round(x) for x in pos]),
             )
         image = this.rotateImage(image)
         
+        this.SAFE_MODE = False
         return image
     
     @property
     def foreground_PhotoImage(this) -> 'ImageTk.PhotoImage':
-        """Foregound Tkinter PhotoImage
+        """Foreground Tkinter PhotoImage
 
         Returns:
             ImageTk.PhotoImage: Tkinter PhotoImage
         """
         if LOADED_ImageTk:
             this._PhotoImage['foreground'] = ImageTk.PhotoImage(this.foreground)
         else:
@@ -418,17 +502,20 @@
                     
             else:
                 this.filesystem.add(path, output)
         
         return output
     
     def updateProperties(this):
-        """Update properties. Deletes any properties that are the same as defaultProperties.
+        """Update properties. Deletes any properties that are the same as defaultProperties, unless specified by the object type in the ObjectPack.
         """
-        properties = list(this.properties.keys())
+        type = this.Type
+        
+        if type != None:
+            type.ready_properties()
         
         # for property in properties:
         #     if property in this.defaultProperties:
         #         if this.properties[property] == this.defaultProperties[property]:
         #             del this.properties[property]
         
         # if this.type != None:
@@ -466,15 +553,15 @@
         
         this.getProperties()
         
         return xml
     
     @property
     def filename(this) -> str | None:
-        """Object filename based on the `Filename` proprty
+        """Object filename based on the `Filename` property
         """
         if 'Filename' in this.properties:
             return this.properties['Filename']
         else:
             return None
     @filename.setter
     def filename(this, value : str):
@@ -507,23 +594,28 @@
     def _getSprites(this, xml : etree.ElementBase):
         for element in xml:
             if element is etree.Comment:
                 continue
             
             if element.tag == 'Sprite':
                 attributes = element.attrib
-                sprite = Sprite(
-                    file = this.filesystem.get(attributes['filename']),
-                    filesystem = this.filesystem,
-                    properties = attributes,
-                    scale = this.scale,
-                    HD = this.HD,
-                    TabHD = this.TabHD,
-                )
-                this.sprites.append(sprite)
+                
+                file = this.filesystem.get(attributes['filename'])
+                
+                if isinstance(file, File):
+                
+                    sprite = Sprite(
+                        file = file,
+                        filesystem = this.filesystem,
+                        properties = attributes,
+                        scale = this.scale,
+                        HD = this.HD,
+                        TabHD = this.TabHD,
+                    )
+                    this.sprites.append(sprite)
     
     def _getUVs(this, xml : etree.ElementBase):
         for element in xml:
             if element is etree.Comment:
                 continue
             if element.tag == 'UV':
                 pos = element.get('pos')
@@ -534,18 +626,25 @@
             if element is etree.Comment:
                 continue
             if element.tag == 'Vert':
                 index = element.get('index')
                 this.VertIndices.append(int(index))
     
     def getProperties(this):
-        for prop in this.defaultProperties:
-            this.properties[prop] = this.defaultProperties[prop]
-        for prop in this._properties:
-            this.properties[prop] = this._properties[prop]
+        """Get the object properties.
+
+        Returns:
+            dict[str,str]: The properties dictionary.
+        """
+        
+        # for prop in this.defaultProperties:
+        #     if prop not in this.properties:
+        #         this.properties[prop] = this.defaultProperties[prop]
+        for prop in this._level_properties:
+            this.properties[prop] = this._level_properties[prop]
         return this.properties
     
     def _getDefaultProperties(this, xml : etree.ElementBase):
         for element in xml:
             if element is etree.Comment:
                 continue
             if element.tag == 'Property':
@@ -654,28 +753,50 @@
         Returns:
             PIL.Image.Image: The resulting PIL Image object.
         """
         if filename == None:
             filename = this.name if this.name not in ['', None] else this.type if this.type not in ['', None] else os.path.basename(this.filename)
             filename = os.path.splitext(filename)[0] + '.gif'
             
-            print(f'{filename = }')
+            # print(f'{filename = }')
         
         animation = this.getAnimation(
             duration = duration,
             fps = fps,
         )
         
         return save_transparent_gif(
             animation['frames'],
             durations = animation['frame_duration'],
             save_file = filename,
         )
+    
+    def copy(this) -> Object:
+        """Creates a copy of this object (aka, get the object again).
+
+        Returns:
+            Object: New Object.
+        """
+        return Object(
+            this.file,
+            filesystem = this.filesystem,
+            properties = this.properties,
+            pos = this.pos,
+            name = this.name,
+            scale = this.scale,
+            HD = this.HD,
+            TabHD = this.TabHD,
+        )
 
 class Shape(GameObject):
+    """Shape object for wmwpy Object.
+
+    Attributes:
+        points (list[tuple[float,float]]): List of shape points.
+    """
     def __init__(this, xml : etree.ElementBase = None) -> None:
         """Shape for Object
 
         Args:
             xml (etree.Element, optional): lxml Element. Defaults to None.
         """
         this.points : list[tuple[float,float]] = []
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/sprite.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/sprite.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,100 +10,167 @@
 if LOADED_ImageTk:
     try:
         from PIL import ImageTk
     except:
         LOADED_ImageTk = False
 
 from .imagelist import Imagelist
-from ..Utils.filesystem import *
-from ..Utils.gif import save_transparent_gif
-from ..Utils.XMLTools import strbool
+from ..utils.filesystem import *
+from ..utils.gif import save_transparent_gif
+from ..utils.XMLTools import strbool
+from ..utils import path
 from ..gameobject import GameObject
+from .texture import Texture
 
 class Sprite(GameObject):
+    """wmwpy Sprite.
+    
+    Attributes:
+        HD (bool): Using HD images.
+        TabHD (bool): Using TabHD images.
+        properties (dict[str,str]): Sprite properties.
+        animations (list[Sprite.Animation]): List of animations.
+        scale (float): The image scale.
+    """
+    
+    TEMPLATE = b"""<?xml version="1.0"?>
+<Sprite>
+</Sprite>
+"""
+    
     def __init__(
         this,
-        file : str | bytes | File,
+        file : str | bytes | File = None,
         filesystem: Filesystem | Folder = None,
         gamepath: str = None, assets: str = '/assets',
         baseassets : str = '/',
         properties : dict = {},
-        scale : int = 50,
+        scale : float = 50,
         HD : bool = False,
         TabHD : bool = False,
     ) -> None:
         """Game sprite.
 
         Args:
-            this (_type_): _description_
             file (str | bytes | File): Sprite file.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
             properties (dict, optional): Sprite properties. Defaults to {}.
             scale (int, optional): Sprite image scale. Defaults to 10.
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
-        this.file = super().get_file(file)
         
+        this.file = super().get_file(file, template = this.TEMPLATE)
+
         this.xml : etree.ElementBase = etree.parse(this.file).getroot()
         
         this.HD = HD
         this.TabHD = TabHD
         
         this.properties = deepcopy(properties)
+        this._properties = deepcopy(this.properties)
         this.animations : list[Sprite.Animation] = []
         
+        this.SAFE_MODE = False
+        
         this.scale = scale
         
         this.readXML()
         this.animation = 0
     
     def setAnimation(this, animation : str | int):
         """Set the current animation for the Sprite
 
         Args:
             animation (str | int): Animation name or index.
         """
         this.animation = animation
     
     @property
+    def SAFE_MODE(this) -> bool:
+        """A "safe mode" where you can modify the properties without them being added to the output xml.
+
+        Returns:
+            bool: The current state.
+        """
+        if not hasattr(this, '_SAFE_MODE'):
+            this._SAFE_MODE = False
+        
+        return this._SAFE_MODE
+    @SAFE_MODE.setter
+    def SAFE_MODE(this, mode : bool):
+        if not isinstance(mode, bool):
+            raise TypeError('mode must be True or False')
+        
+        if mode:
+            if not this.SAFE_MODE:
+                this._properties = deepcopy(this.properties)
+                this._image = None
+        else:
+            if this.SAFE_MODE:
+                this.properties = deepcopy(this._properties)
+                this._image = None
+        
+        for animation in this.animations:
+            animation.SAFE_MODE = mode
+        
+        this._SAFE_MODE = mode
+    
+    @property
     def image(this) -> Image.Image:
         """Image of sprite
 
         Returns:
             PIL.Image.Image: PIL Image
         """
+        if this.SAFE_MODE:
+            if hasattr(this, '_image'):
+                if isinstance(this._image, Image.Image):
+                    return this._image.copy()
+        
         image = this.animation.image.copy()
         gridSize = numpy.array(this.gridSize)
+        
+        # print(f'{gridSize = }')
+        # print(f'{this.scale = }')
+        
         size = gridSize * this.scale
         size = [abs(round(x)) for x in size]
         image = image.resize(size)
         
         image = image.rotate(this.angle, Image.BILINEAR, expand=True)
         
+        this._image = image
         return image
+    @image.setter
+    def image(this, image : Image.Image):
+        if isinstance(image, Image.Image):
+            this._image = image
+        else:
+            raise TypeError('image must be instance of PIL.Image.Image')
     
     @property
     def animation(this) -> 'Sprite.Animation':
         """Returns the current animation
 
         Returns:
             Sprite.Animation: A Sprite.Animation class
         """
         return this._currentAnimation
     @animation.setter
     def animation(this, animation : str | int):
         if isinstance(animation, (int, float)):
             animation = int(animation)
-            this._currentAnimation = this.animations[animation]
+            if animation < len(this.animations):
+                this._currentAnimation = this.animations[animation]
         elif isinstance(animation, str):
             for a in this.animations:
                 if a.name == animation:
                     this._currentAnimation = a
                     break
         elif isinstance(animation, this.Animation):
             this._currentAnimation = animation
@@ -144,37 +211,43 @@
     @filename.setter
     def filename(this, value):
         this.properties['filename'] = value
         
     def readXML(this):
         """Read Sprite XML
         """
+        if this.file == None:
+            return
+        
         this.animations = []
         for element in this.xml:
-            if (not element is etree.Comment) or element.tag == 'Animation':
+            if element is etree.Comment:
+                continue
+            
+            if element.tag == 'Animation':
                 animation = this.Animation(
                     element,
                     this.filesystem,
                     HD = this.HD,
                     TabHD = this.TabHD,
                 )
                 
                 this.animations.append(animation)
     
-    def export(this, path : str = None):
+    def export(this, path : str = None) -> bytes:
         """Export the Sprite XML file
 
         Args:
             path (str, optional): Path to export into the filesystem. Defaults to the original filename.
 
         Raises:
             TypeError: Path is not a file.
 
         Returns:
-            str: Contents of saved file.
+            bytes: Contents of saved file.
         """
         xml : etree.ElementBase = etree.Element('Sprite')
         
         for animation in this.animations:
             xml.append(animation.getXML())
         
         this.xml = xml
@@ -318,17 +391,31 @@
         this.animation.saveGIF(
             filename = filename,
             duration = duration,
             fps = fps,
         )
 
     class Animation(GameObject):
+        """Animation object for wmwpy Sprite.
+        
+        Attributes:
+            HD (bool): Using HD images.
+            TabHD (bool): Using TabHD images.
+            properties (dict[str,str]): The animation properties.
+            frames (list[Sprite.Animation.Frame]): List of frames.
+            frame (int): The current animation frame.
+        
+        """
+        TEMPLATE = """<Animation>
+</Animation>
+"""
+        
         def __init__(
             this,
-            xml : str | etree.ElementBase,
+            xml : str | etree.ElementBase = None,
             filesystem: Filesystem | Folder = None,
             gamepath: str = None,
             assets: str = '/assets',
             baseassets: str = '/',
             HD : bool = False,
             TabHD : bool = False,
         ) -> None:
@@ -342,48 +429,80 @@
                 baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
                 HD (bool, optional): Use HD images. Defaults to False.
                 TabHD (bool, optional): Use TabHD images. Defaults to False.
             """
             super().__init__(filesystem, gamepath, assets, baseassets)
             
             if isinstance(xml, str):
-                this.xml : etree.ElementBase = etree.parse(xml).getroot()
-            else:
+                this.xml : etree.ElementBase = etree.XML(xml).getroot()
+            elif isinstance(xml, etree._Element):
                 this.xml = xml
+            elif xml == None:
+                this.xml = etree.XML(this.TEMPLATE)
             
             this.HD = HD
             this.TabHD = TabHD
             
             this.properties = {}
-            this.name = ''
-            this.textureBasePath = '/Textures/'
-            this.atlas : Imagelist = None
-            this.fps = 30
-            this.playbackMode = 'ONCE'
-            this.loopCount = 1
             
             this._PhotoImage = None
             
             this.frames : list[Sprite.Animation.Frame] = []
             this.frame = 0
             
             this.readXML()
+            
+            this.SAFE_MODE = False
+        
+        
+        @property
+        def SAFE_MODE(this) -> bool:
+            """A "safe mode" where you can modify the properties without them being added to the output xml.
+
+            Returns:
+                bool: The current state.
+            """
+            if not hasattr(this, '_SAFE_MODE'):
+                this._SAFE_MODE = False
+            
+            return this._SAFE_MODE
+        @SAFE_MODE.setter
+        def SAFE_MODE(this, mode : bool):
+            if not isinstance(mode, bool):
+                raise TypeError('mode must be True or False')
+            
+            if mode:
+                if not this.SAFE_MODE:
+                    this._properties = deepcopy(this.properties)
+            else:
+                if this.SAFE_MODE:
+                    this.properties = deepcopy(this._properties)
+            
+            for frame in this.frames:
+                frame.SAFE_MODE = mode
+            
+            this._SAFE_MODE = mode
         
         @property
         def image(this) -> Image.Image:
             """Current Animation image
 
             Returns:
                 PIL.Image.Image: PIL Image
             """
             
             return this.frames[this.frame].image
         
         @property
         def frame(this) -> int:
+            """Current animation frame.
+
+            Returns:
+                int: Current animation frame index.
+            """
             return this._frame
         @frame.setter
         def frame(this, value : int):
             if len(this.frames) > 0:
                 this._frame = int(value) % len(this.frames)
             else:
                 this._frame = 0
@@ -406,38 +525,176 @@
             this.getFrames()
         
         def getAttributes(this):
             """Get all the attributes of this Animation
             """
             this.properties = this.xml.attrib
             
+        
+        @property
+        def name(this) -> str:
+            """Name of this animation.
+
+            Returns:
+                str: The name of this animation.
+            """
             if 'name' in this.properties:
-                this.name = this.properties['name']
+                return this.properties['name']
+            else:
+                return ''
+        @name.setter
+        def name(this, value : str):
+            if not isinstance(value, str):
+                raise TypeError('name must be str')
+            
+            this.properties['name'] = value
+        
+        @property
+        def textureBasePath(this) -> str:
+            """The textureBasePath where all textures are stored.
+
+            Returns:
+                str: textureBasePath.
+            """
             if 'textureBasePath' in this.properties:
-                this.textureBasePath = this.properties['textureBasePath']
+                return this.properties['textureBasePath']
+            else:
+                if this.filesystem == None:
+                    return '/Textures/'
+                
+                this.textureBasePath = path.joinPath(this.filesystem.baseassets, '/Textures/')
+                return this.textureBasePath
+        @textureBasePath.setter
+        def textureBasePath(this, path):
+            if isinstance(path, Folder):
+                path = path.path
+            if not isinstance(path, str):
+                raise TypeError('path must be str')
+            
+            this.properties['textureBasePath'] = path
+        
+        @property
+        def atlasPath(this) -> str:
+            """The path to the atlas.
+
+            Returns:
+                str: The path to the atlas file.
+            """
+            if 'atlas' in this.properties:
+                return this.properties['atlas']
+            else:
+                return None
+        @atlasPath.setter
+        def atlasPath(this, path):
+            this.atlas = path
+        
+        @property
+        def atlas(this) -> Imagelist:
+            if hasattr(this, '_atlas') and isinstance(this._atlas, Imagelist):
+                this.properties['atlas'] = this._atlas.filename
+                return this._atlas
+            
             if 'atlas' in this.properties:
-                this.atlasPath = this.properties['atlas']
-                this.atlas = Imagelist(
+                this._atlas = Imagelist(
+                    this.filesystem.get(this.properties['atlas']),
+                    this.filesystem,
+                    HD = this.HD,
+                    TabHD = this.TabHD,
+                )
+            else:
+                this._atlas = None
+            
+            return this._atlas
+        @atlas.setter
+        def atlas(this, path):
+            if isinstance(path, str):
+                this._atlas = Imagelist(
                     this.filesystem.get(this.properties['atlas']),
                     this.filesystem,
-                    HD=this.HD,
+                    HD = this.HD,
+                    TabHD = this.TabHD,
+                )
+            elif isinstance(path, Imagelist):
+                this._atlas = path
+            else:
+                raise TypeError('atlas must be str or Imagelist')
+        
+        @property
+        def texture(this) -> Texture:
+            """The texture for this animation. Sometimes used instead of an atlas.
+
+            Returns:
+                Texture: The Texture.
+            """
+            if hasattr(this, '_texture') and isinstance(this._texture, Texture):
+                this.properties['texture'] = this._texture.filename
+                return this._texture
+            
+            if 'texture' in this.properties:
+                this._texture = Texture(
+                    this.properties['texture'],
+                    filesystem = this.filesystem,
+                    gamepath = this.gamepath,
+                    assets = this.assets,
+                    baseassets = this.baseassets,
+                    HD = this.HD,
                     TabHD = this.TabHD,
                 )
                 
-                # this.atlasHD = Imagelist(
-                #     this.filesystem.get(this.properties['atlas']),
-                #     this.filesystem,
-                #     HD=True
-                # )
+            else:
+                this._texture = None
+
+            return this._texture
+        @texture.setter
+        def texture(this, path):
+            if isinstance(path, str):
+                this.properties['texture'] = path
+            elif isinstance(path, File):
+                this.properties['texture'] = path.path
+            elif isinstance(path, Texture):
+                this.properties['texture'] = path.filename
+                this._texture = path
+            else:
+                raise TypeError('texture must be a path, File, or Texture object')
+            
                 
+        
+        @property
+        def playbackMode(this) -> str:
+            """The playback mode.
+
+            Returns:
+                str: The current playback mode.
+            """
             if 'playbackMode' in this.properties:
-                this.playbackMode = this.properties['playbackMode']
+                return this.properties['playbackMode']
+            else:
+                return 'ONCE'
+        @playbackMode.setter
+        def playbackMode(this, mode):
+            if not isinstance(mode, str):
+                raise TypeError('playbackMode must be str')
+        
+        @property
+        def loopCount(this) -> int:
+            """The loopCount for this Animation.
+            
+            Returns:
+                int: The loopCount.
+            """        
             if 'loopCount' in this.properties:
-                this.loopCount = int(this.properties['loopCount'])
+                return int(this.properties['loopCount'])
+            else:
+                return 0
+        @loopCount.setter
+        def loopCount(this, count):
+            if not isinstance(count, (str, int, float)):
+                raise TypeError('loopCount must be str or int')
             
+            this.properties['loopCount'] = str(count)
             
         def getFrames(this) -> list['Sprite.Animation.Frame']:
             """Get a list of all the Animation `Frame`s
 
             Returns:
                 list[Sprite.Animation.Frame]: List of all the Frames in this Animation.
             """
@@ -445,16 +702,20 @@
             
             if this.xml == None:
                 return None
             for f in this.xml:
                 if (not f is etree.Comment) and f.tag == 'Frame':
                     this.frames.append(this.Frame(
                         f.attrib,
-                        this.atlas,
-                        this.textureBasePath
+                        this.atlas if this.atlas != None else this.texture,
+                        this.textureBasePath,
+                        filesystem = this.filesystem,
+                        gamepath = this.gamepath,
+                        assets = this.assets,
+                        baseassets = this.baseassets,
                     ))
             
             return this.frames
 
         def updateProperties(this):
             """Update the Sprite properties
             """
@@ -485,15 +746,20 @@
             for frame in this.frames:
                 xml.append(frame.getXML())
             
             this.xml = xml
             return this.xml
         
         @property
-        def fps(this):
+        def fps(this) -> float:
+            """The Animation fps.
+
+            Returns:
+                float: The Animation fps.
+            """
             if 'fps' in this.properties:
                 return float(this.properties['fps'])
             else:
                 this.fps = 30
                 return this.fps
         @fps.setter
         def fps(this, value : int | float | str):
@@ -581,97 +847,267 @@
 
             Returns:
                 PIL.Image.Image: The resulting PIL Image object.
             """
             if filename == None:
                 filename = this.name
                 filename = os.path.splitext(filename)[0] + '.gif'
-                
-                print(f'{filename = }')
             
             animation = this.getAnimation(
                 duration = duration,
                 fps = fps,
             )
             
             return save_transparent_gif(
                 animation['frames'],
                 durations = animation['frame_duration'],
                 save_file = filename,
             )
         
         # Frame
-        class Frame():
-            _offset = (0,0)
-            _scale = (1,1)
-            _angleDeg = 0
-            _repeat = 1
+        class Frame(GameObject):
+            """The Frame for Animations.
+
+            Attributes:
+                atlas (Imagelist): The atlas for this Frame.
+                textureBasePath (str): The textureBasePath for this Frame.
+                properties (dict[str,str]): The frame properties.
+            """
+            
             def __init__(
                 this,
-                properties : dict,
+                properties : dict = {},
                 atlas : Imagelist = None,
                 textureBasePath : str = None,
+                filesystem : Filesystem | Folder = None,
+                gamepath : str = None,
+                assets : str = '/assets',
+                baseassets : str = '/',
             ) -> None:
                 """Frame for Sprite.Animation.
 
                 Args:
-                    this (_type_): _description_
                     properties (dict): Image properties.
                     atlas (Imagelist, optional): Image atlas for Image. Defaults to None.
                     textureBasePath (str, optional): Directory to put image in. Defaults to None.
+                    filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
+                    gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+                    assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+                    baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `
                 """
+                super().__init__(filesystem, gamepath, assets, baseassets)
+                
                 this.atlas = atlas
-                this.textueBasePath = textureBasePath
+                this.textureBasePath = textureBasePath
                 this.properties = properties
                 
-                this.name = ''
-                this.offset = this._offset
-                this.scale = this._scale
-                this.angleDeg = this._angleDeg
-                this.repeat = this._repeat
+                this.color_filter : tuple[int,int,int,int] = []
                 
+                this.getImage()
                 
+                this.SAFE_MODE = False
+            
+            
+            @property
+            def SAFE_MODE(this) -> bool:
+                """A "safe mode" where you can modify the properties without them being added to the output xml.
+
+                Returns:
+                    bool: The current state.
+                """
+                if not hasattr(this, '_SAFE_MODE'):
+                    this._SAFE_MODE = False
                 
-                this.getData()
-                this.getImage()
+                return this._SAFE_MODE
+            @SAFE_MODE.setter
+            def SAFE_MODE(this, mode : bool):
+                if not isinstance(mode, bool):
+                    raise TypeError('mode must be True or False')
+                
+                if mode:
+                    if not this.SAFE_MODE:
+                        this._properties = deepcopy(this.properties)
+                        this._color_filters = deepcopy(this.color_filter)
+                else:
+                    if this.SAFE_MODE:
+                        this.properties = deepcopy(this._properties)
+                        this.color_filter = deepcopy(this._color_filters)
+                
+                this._SAFE_MODE = mode
             
-            def getData(this):
-                """Get the Frame data
+            @property
+            def name(this) -> str:
+                """The name of this frame.
+
+                Returns:
+                    str: The name of this frame.
                 """
                 if 'name' in this.properties:
-                    this.name = this.properties['name']
+                    return this.properties['name']
+                else:
+                    return ''
+            @name.setter
+            def name(this, name : str):
+                this.properties['name'] = str(name)
+            
+            @property
+            def offset(this) -> tuple[float,float]:
+                """The frame offset.
+
+                Returns:
+                    tuple[float,float]: (x,y)
+                """
                 if 'offset' in this.properties:
-                    this.offset = tuple([float(x) for x in this.properties['offset'].split()])
+                    return tuple([float(x) for x in this.properties['offset'].split()])
+                else:
+                    return (0,0)
+            @offset.setter
+            def offset(this, offset : tuple[float,float]):
+                if isinstance(offset, (tuple, list)):
+                    this.properties['offset'] = ' '.join([str(x) for x in offset])
+                elif isinstance(offset, (int, float)):
+                    this.properties['offset'] = ' '.join([str(offset), str(offset)])
+                elif isinstance(offset, str):
+                    this.properties['offset'] = offset
+                else:
+                    raise TypeError('offset must be tuple, float or str')
+            
+            @property
+            def scale(this) -> tuple[float, float]:
+                """The frame scale.
+
+                Returns:
+                    tuple[float, float]: (x,y)
+                """
                 if 'scale' in this.properties:
-                    this.scale = tuple([float(x) for x in this.properties['scale'].split()])
+                    return tuple([float(x) for x in this.properties['scale'].split()])
+                else:
+                    return (1, 1)
+            @scale.setter
+            def scale(this, scale : tuple[float,float]):
+                if isinstance(scale, (tuple, list)):
+                    this.properties['scale'] = ' '.join([str(x) for x in scale])
+                elif isinstance(scale, (int, float)):
+                    this.properties['scale'] = ' '.join([str(scale), str(scale)])
+                elif isinstance(scale, str):
+                    this.properties['scale'] = scale
+                else:
+                    raise TypeError('scale must be tuple, float or str')
+            
+            @property
+            def angleDeg(this) -> float:
+                """The frame rotation angle.
+
+                Returns:
+                    float: Angle in degrees.
+                """
                 if 'angleDeg' in this.properties:
-                    this.angleDeg = float(this.properties['angleDeg'])
+                    return float(this.properties['angleDeg'])
+                else:
+                    return 0
+            @angleDeg.setter
+            def angleDeg(this, angle : float):
+                if isinstance(angle, (int, float, str)):
+                    this.properties['angleDeg'] = str(angle)
+                else:
+                    raise TypeError('angle must be float')
+            
+            @property
+            def repeat(this) -> int:
+                """The amount of times to repeat this frame in the animation.
+
+                Returns:
+                    int: The amount of times to repeat.
+                """
                 if 'repeat' in this.properties:
                     this.repeat = int(this.properties['repeat'])
+                else:
+                    return 0
+            @repeat.setter
+            def repeat(this, num : int):
+                if isinstance(num, (int, float, str)):
+                    this.properties['angleDeg'] = str(int(float(num)))
+                else:
+                    raise TypeError('angle must be int')
                 
             def getImage(this):
-                this._image = this.atlas.get(this.name)
+                """Get the image. The image is stored in Frame._image.
+                """
+                if isinstance(this.atlas, Imagelist):
+                    this._image = this.atlas.get(this.name)
+                elif this.texture != None:
+                    this._image = this.texture
+                
+            
+            @property
+            def texture(this) -> Texture:
+                """The frame Texture instead of atlas.
+
+                Returns:
+                    Texture: The Texture object.
+                """
+                if isinstance(this.atlas, Texture):
+                    return this.atlas
+                else:
+                    return None
+            
             
             @property
             def image(this) -> Image.Image:
                 """Image of this Image
 
                 Returns:
                     PIL.Image.Image: PIL Image
                 """
-                if this._image:
+                this.getImage()
+                
+                if hasattr(this._image, 'image'):
                     image = this._image.image.copy()
-                    image = image.resize(tuple([round(_) for _ in (numpy.array(this._image.size) * numpy.array(this.scale))]))
-                    image = image.rotate(this.angleDeg, expand = True)
+                elif isinstance(this._image, Image.Image):
+                    image = this._image.copy()
                 else:
                     image = Image.new('RGBA', (1,1), (0,0,0,0))
+                
+                image = image.resize(tuple([round(_) for _ in (numpy.array(this._image.size) * numpy.array(this.scale))]))
+                image = image.rotate(this.angleDeg, expand = True)
+                
+                # for color in this.color_filters:
+                # if len(this.color_filter) >= 3:
+                #     try:
+                #         image = imageprocessing.recolor_image(
+                #             image,
+                #             this.color_filter
+                #         )
+                #     except:
+                #         pass
+                    # image.show()
+                
+                
                 return image
             @image.setter
-            def image(this, image : Image.Image):
-                this._image = image
+            def image(this, image : str):
+                if isinstance(image, Texture):
+                    this.atlas = image
+                elif isinstance(this.atlas, Texture):
+                    if isinstance(image, str):
+                        this.atlas = Texture(
+                            image = image,
+                            filesystem = this.filesystem,
+                            gamepath = this.gamepath,
+                            assets = this.assets,
+                            baseassets = this.baseassets,
+                            HD = this.atlas.HD,
+                            TabHD = this.atlas.TabHD,
+                        )
+                elif isinstance(this.atlas, Imagelist):
+                    if isinstance(image, str):
+                        this.name = image
+                
+                this.getImage()
+                
             
             def updateProperties(this):
                 """Update Image properties
                 """
                 def updateProperty(property : str, value, default):
                     if value == default:
                         if property in this.properties:
@@ -710,30 +1146,30 @@
 
                 Returns:
                     etree.Element: XML of this Frame
                 """
                 this.updateProperties()
                 return etree.Element('Frame', **this.properties)
             
-            def show(this, title: str | None = None):
+            def show(this, *args, **kwargs):
                 """Calls the PIL.Image.Image.show() method.
                 
                 ---
                 #### Description copied from the PIL library
                 
                 Displays this image. This method is mainly intended for debugging purposes.
 
                 This method calls PIL.ImageShow.show internally. You can use
-                PIL.ImageShow.register to override its default behaviour.
+                PIL.ImageShow.register to override its default behavior.
 
                 The image is first saved to a temporary file. By default, it will be in PNG format.
 
                 On Unix, the image is then opened using the **display**, **eog** or **xv** utility, depending on which one can be found.
 
                 On macOS, the image is opened with the native Preview application.
 
                 On Windows, the image is opened with the standard PNG display utility.
 
                 Args:
                     title (str | None, optional): Optional title to use for the image window, where possible.. Defaults to None.
                 """
-                return this.image.show(title = title)
+                return this.image.show(*args, **kwargs)
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy/classes/widget/widget.py` & `wmwpy-0.5.0b0/src/wmwpy/classes/widget/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # main widget class
-from ...Utils.filesystem import Filesystem, Folder
+from ...utils.filesystem import Filesystem, Folder
 from ...gameobject import GameObject
 
 
 from PIL import Image
 from lxml import etree
 
 WIDGETS : dict[str, 'Widget'] = {}
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/game.py` & `wmwpy-0.5.0b0/src/wmwpy/game.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import os
 import typing
 import logging
 
-from .Utils.filesystem import *
-from .Utils import Texture
-from .Utils import path
+from .utils.filesystem import *
+from .classes.texture import Texture
+from .utils.path import joinPath
 from .classes import *
 
+from . import object_packs
+
 class Game():
+    """The wmwpy Game object.
+
+    Attributes:
+        gamepath (str): The path to the game directory on disk.
+        assets (str): The relative path from the game directory to the assets folder (e.g. '/assets').
+        baseassets (str): The base assets path inside the assets folder, e.g. '/Perry' in WMP.
+        db (str): The path to the database file.
+        profile (str): The path to the profile in WMW2.
+        platform (Literal['android','ios']): The platform this extracted game is on.
+        object_pack (ObjectPack): The ObjectPack for this game.
+    
+    """
+    
     _DB = '/Data/water.db'
     _BASEASSETS = '/'
     _PROFILE = None
     
     game = 'WMW'
     
     def __init__(
         this,
-        gamepath : str, assets : str = '/assets',
+        gamepath : str,
+        assets : str = '/assets',
         db : str = '/Data/water.db',
         profile : str = None,
         baseassets : str = '/',
         platform : typing.Literal['android', 'ios'] = 'android',
         load_callback : typing.Callable[[int, str, int], typing.Any] = None,
     ) -> None:
         """load game
@@ -28,31 +44,37 @@
         Args:
             gamepath (str): Folder to extracted game.
             assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
             db (str, optional): Relative path to database file from assets folder. Defaults to '/Data/water.db'.
             profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
             platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
-            load_callbac (Callable[[int, str, int], Any], optional): (Callable[[int, str, int], Any], optional): A callback function to be ran while loading the game. Defaults to None.
+            load_callback (Callable[[int, str, int], Any], optional): A callback function to be ran while loading the game. Defaults to None.
         """
         if gamepath == None:
             return
         
         this.gamepath = os.path.abspath(gamepath)
         # print(f'{gamepath = }\n{this.gamepath = }')
         this.assets = assets
         this.db = db or this._DB
         this.profile = profile or this._PROFILE
         this.baseassets = baseassets or this._BASEASSETS
         this.platform = platform
         
+        this.object_pack = object_packs.get_object_pack(this.game)
         
         this.updateFilesystem(load_callback = load_callback)
         
     def updateFilesystem(this, load_callback : typing.Callable[[int, str, int], typing.Any] = None):
+        """Update the current filesystem.
+
+        Args:
+            load_callback (Callable[[int, str, int], typing.Any], optional): A callback to be ran while loading the filesystem. Defaults to None.
+        """
         this.filesystem = Filesystem(this.gamepath, this.assets)
         this.filesystem.getAssets(load_callback = load_callback)
     
     def dump(
         this,
         folder = None,
         callback : typing.Callable[[int, str, int], typing.Any] = None,
@@ -69,25 +91,36 @@
         this,
         xmlPath : str = None,
         imagePath : str = None,
         load_callback : typing.Callable[[int, str, int], typing.Any] = None,
         ignore_errors : bool = False,
         HD = False,
         TabHD = False,
+        object_pack : object_packs.ObjectPack = None,
     ):
-        """
-        Load level
+        """Load Level
 
         Args:
+            this (_type_): _description_
             xmlPath (str, optional): Path to xml file. Defaults to None.
             imagePath (str, optional): Path to image file. Defaults to None.
+            load_callback (Callable[[int, str, int], typing.Any], optional): A callback function to be called while loading the level. Defaults to None.
+            ignore_errors (bool, optional): Whether to ignore errors while loading the level. Defaults to False.
+            HD (bool, optional): Use HD images. Defaults to False.
+            TabHD (bool, optional): Use TabHD images. Defaults to False.
+            object_pack (classes.objectpack.pack.ObjectPack, optional): The object pack to use. Defaults to the game object pack.
+
+        Returns:
+            classes.level.Level: wmwpy Level object.
         """
         logging.debug(f'Game: xml input: {xmlPath}')
         
-        levels = this.filesystem.get(path.joinPath(this.baseassets, '/Levels'))
+        levels = this.filesystem.get(joinPath(this.baseassets, '/Levels'))
+        if levels == None:
+            levels = this.filesystem
         
         if isinstance(xmlPath, File):
             xml = xmlPath
             
             logging.debug(f'Game: xml path: {xmlPath.path}')
             
         else:
@@ -113,59 +146,71 @@
             if imagePath:
                 image = levels.get(imagePath)
         
         logging.debug(f'Game: xml after: {xml}')
         if isinstance(xml, File):
             logging.debug(f'Game: xml path: {xml.path}')
         
+        if object_pack == None:
+            object_pack = this.object_pack
+        
         level = Level(
             xml = xml,
             image = image,
             filesystem = this.filesystem,
             load_callback = load_callback,
             ignore_errors = ignore_errors,
             HD = HD,
             TabHD = TabHD,
+            object_pack = object_pack,
         )
         if isinstance(xmlPath, File):
             level.filename = xmlPath.path
         else:
             level.filename = xmlPath
         
         return level
     
     def Object(
         this,
         object : str,
         HD : bool = False,
         TabHD : bool = False,
+        object_pack = None,
         **kwargs
     ):
         """
         Load object
 
         Args:
             object (str): Path to `.hs` object file.
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
+            object_pack (classes.objectpack.pack.ObjectPack, optional): The object pack to use. Defaults to the game object pack.
 
         Returns:
             classes.object.Object: Where's My Water? object.
         """
         
-        objects = this.filesystem.get(path.joinPath(this.baseassets, '/Objects'))
+        objects = this.filesystem.get(joinPath(this.baseassets, '/Objects'))
+        if objects == None:
+            objects = this.filesystem
         
         if not isinstance(object, File):
             object = objects.get(object)
         
+        if object_pack == None:
+            object_pack = this.object_pack
+        
         obj = Object(
             object,
             filesystem = this.filesystem,
             HD = HD,
             TabHD = TabHD,
+            object_pack = object_pack,
             **kwargs
         )
         if isinstance(object, File):
             obj.filename = object.path
         else:
             obj.filename = object
             
@@ -182,35 +227,39 @@
         """
         Load imagelist
 
         Args:
             imagelist (str): Path to `.imagelist` file. Defaults to None
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
+            save_images (bool, optional): Whether to save all the images in the filesystem. Note: it can take longer to load if this is True. Defaults to False.
 
         Returns:
             classes.imagelist.Imagelist: Imagelist object.
         """
         
-        textures = this.filesystem.get(path.joinPath(this.baseassets, '/Textures'))
+        textures = this.filesystem.get(joinPath(this.baseassets, '/Textures'))
+        if textures == None:
+            textures = this.filesystem
         
         if not isinstance(imagelist, File):
+            if isinstance(imagelist, str):
+                split = os.path.splitext(imagelist)
+                if split[1] == '':
+                    imagelist = ''.join([split[0], '.imagelist'])
+                
             imagelist = textures.get(imagelist)
         
         imagelistObject = Imagelist(
             imagelist,
             filesystem = this.filesystem,
             HD = HD,
             TabHD = TabHD,
             save_images = save_images,
         )
-        if isinstance(imagelist, File):
-            imagelistObject.filename = imagelist.path
-        else:
-            imagelistObject.filename = imagelist
         
         return imagelistObject
     
     def Sprite(
         this,
         sprite : str,
         HD = False,
@@ -225,15 +274,17 @@
             HD (bool, optional): Use HD images. Defaults to False.
             TabHD (bool, optional): Use TabHD images. Defaults to False.
 
         Returns:
             classes.sprite.Sprite: Sprite object.
         """
         
-        sprites = this.filesystem.get(path.joinPath(this.baseassets, '/Sprites'))
+        sprites = this.filesystem.get(joinPath(this.baseassets, '/Sprites'))
+        if sprites == None:
+            sprites = this.filesystem
         
         if not isinstance(sprite, File):
             sprite = sprites.get(sprite)
         
         spriteObject = Sprite(
             sprite,
             filesystem = this.filesystem,
@@ -246,39 +297,111 @@
         else:
             spriteObject.filename = sprite.path
         
         return spriteObject
     
     def Texture(
         this,
-        texture : str,
+        texture : str | File,
+        HD = False,
+        TabHD = False,
     ):
         """
         Get image texture. Doesn't matter if it's a `.waltex` image or not.
 
         Args:
             texture (str): Path to image file.
+            HD (bool, optional): Use HD image. Defaults to False.
+            TabHD (bool, optional): Use TabHD image. Defaults to False.
 
         Returns:
-            Utils.textures.Texture: Texture object.
+            utils.textures.Texture: Texture object.
         """
         
-        textures = this.filesystem.get(path.joinPath(this.baseassets, '/Textures'))
+        textures = this.filesystem.get(joinPath(this.baseassets, '/Textures'))
+        if textures == None:
+            textures = this.filesystem
         
-        if not isinstance(texture, File):
+        if isinstance(texture, str):
             texture = textures.get(texture)
         
         return Texture(
-            texture
+            texture,
+            filesystem = this.filesystem,
+            HD = HD,
+            TabHD = TabHD,
         )
     
     def Layout(this, layout : str):
         raise NotImplementedError('load layout is not implemented yet.')
     
-    def FileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
+    def Location(this, location : str) -> Location:
+        """Load Location in `WMW2`
+
+        Args:
+            location (str): The path to the location xml file.
+
+        Returns:
+            Location: wmwpy Location object.
+        """
+        locations = this.filesystem.get(joinPath(this.baseassets, '/Locations'))
+        if locations == None:
+            locations = this.filesystem
+        
+        if isinstance(location, str):
+            location = locations.get(location)
+        
+        return Location(
+            location,
+            filesystem = this.filesystem,
+            gamepath = this.gamepath,
+            assets = this.assets,
+            baseassets = this.baseassets,
+        )
+        
+    
+    def Database(this, path : str = None) -> Database:
+        """Load the game database.
+
+        Args:
+            path (str, optional): Path to the database file. Defaults to `Game.db`.
+
+        Returns:
+            Database: Game Database object.
+        """
+        if path == None:
+            path = this.db
+        
+        file = this.filesystem.get(path)
+        
+        return Database(file)
+
+    def TextureSettings(this, path : str = None):
+        if path == None:
+            file = this.filesystem.get(joinPath(this.baseassets, '/Data/textureSettings.xml'))
+        elif isinstance(path, str):
+            file = this.filesystem.get(path)
+        elif isinstance(path, File):
+            file = path
+        else:
+            file = this.filesystem.get(joinPath(this.baseassets, '/Data/textureSettings.xml'))
+
+        return TextureSettings(
+            file,
+            filesystem = this.filesystem,
+            assets = this.assets,
+            gamepath = this.gamepath,
+            baseassets = this.baseassets,
+        )
+    
+    def FileManifest(
+        this,
+        writeFile : bool = True,
+        filename : str = '/FileManifest.txt',
+    ):
         """Generate the `FileManifest.txt` file needed for some games, such as WMM. This just generates a text file with the paths to every file in the `assets` folder (which includes the `FileManifest.txt` file).
 
         Args:
             writeFile (bool, optional): Write the manifest to the `FileManifest.txt` file. Defaults to True.
             filename (str, optional): Filename for FileManifest.txt. Defaults to 'filename'.
 
         Returns:
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/gameobject.py` & `wmwpy-0.5.0b0/src/wmwpy/gameobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .Utils.filesystem import *
+from .utils.filesystem import *
 
 import io
 import typing
 import numpy
 import math
 
 class GameObject():
@@ -15,15 +15,15 @@
     ) -> None:
         """Load filesystem
 
         Args:
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
-            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`.
         """
         this.gamepath = gamepath
         this.assets = assets
         if this.assets == None:
             this.assets = '/assets'
         this.baseassets = baseassets
         
@@ -50,15 +50,15 @@
         this,
         file : bytes | File | io.BytesIO | str,
         template : str | io.BytesIO = None,
     ) -> io.BytesIO | str:
         """Get file
 
         Args:
-            file (bytes | wmwpy.Utils.filesystem.File | io.BytesIO | str): Content of file. Can be bytes, wmwpy File, str (contents of file) or file-like object.
+            file (bytes | wmwpy.utils.filesystem.File | io.BytesIO | str): Content of file. Can be bytes, wmwpy File, str (contents of file) or file-like object.
             template (str | io.BytesIO, optional): Fallback for file if file == None. Defaults to ''
 
         Raises:
             TypeError: File can only be 'str', 'bytes', or file-like object.
 
         Returns:
             io.BytesIO | str: New file object or str.
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy/gametemplate.py` & `wmwpy-0.5.0b0/src/wmwpy/gametemplate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.4.1b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.5.0b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.4.1b0
+Version: 0.5.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1017,15 +1017,15 @@
  ```
 py -m build
  ```
 
 # Building docs
  To build the docs, make sure sphinx is installed
  ```
-pip install -U sphinx
+pip install -r doc-build/requirements.txt
  ```
 
  You then need to run
  ```
 sphinx-build -b html doc-build docs
  ```
```

### Comparing `wmwpy-0.4.1b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.5.0b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,40 +7,51 @@
 src/wmwpy/gametemplate.py
 src/wmwpy.egg-info/PKG-INFO
 src/wmwpy.egg-info/SOURCES.txt
 src/wmwpy.egg-info/dependency_links.txt
 src/wmwpy.egg-info/requires.txt
 src/wmwpy.egg-info/top_level.txt
 src/wmwpy/Font/__init__.py
-src/wmwpy/Utils/XMLTools.py
-src/wmwpy/Utils/__init__.py
-src/wmwpy/Utils/filesystem.py
-src/wmwpy/Utils/gif.py
-src/wmwpy/Utils/logging_utils.py
-src/wmwpy/Utils/path.py
-src/wmwpy/Utils/rotate.py
-src/wmwpy/Utils/textures.py
-src/wmwpy/Utils/waltex.py
-src/wmwpy/Utils/Types/Documents.py
-src/wmwpy/Utils/Types/Images.py
-src/wmwpy/Utils/Types/__init__.py
 src/wmwpy/classes/Widgets.py
 src/wmwpy/classes/__init__.py
 src/wmwpy/classes/curves.py
+src/wmwpy/classes/database.py
 src/wmwpy/classes/imagelist.py
 src/wmwpy/classes/layout.py
 src/wmwpy/classes/level.py
+src/wmwpy/classes/location.py
 src/wmwpy/classes/object.py
 src/wmwpy/classes/sprite.py
+src/wmwpy/classes/texture.py
+src/wmwpy/classes/texturesettings.py
+src/wmwpy/classes/objectpack/__init__.py
+src/wmwpy/classes/objectpack/pack.py
+src/wmwpy/classes/objectpack/type.py
 src/wmwpy/classes/widget/WT_CANVAS.py
 src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
 src/wmwpy/classes/widget/WT_GROUP.py
 src/wmwpy/classes/widget/WT_ICON_LIST.py
 src/wmwpy/classes/widget/WT_LABEL.py
 src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
 src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
 src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
 src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
 src/wmwpy/classes/widget/WT_SLIDER.py
 src/wmwpy/classes/widget/WT_TOGGLE.py
 src/wmwpy/classes/widget/__init__.py
-src/wmwpy/classes/widget/widget.py
+src/wmwpy/classes/widget/widget.py
+src/wmwpy/object_packs/WMW.py
+src/wmwpy/object_packs/__init__.py
+src/wmwpy/utils/XMLTools.py
+src/wmwpy/utils/__init__.py
+src/wmwpy/utils/color.py
+src/wmwpy/utils/filesystem.py
+src/wmwpy/utils/gif.py
+src/wmwpy/utils/imageprocessing.py
+src/wmwpy/utils/logging_utils.py
+src/wmwpy/utils/path.py
+src/wmwpy/utils/rotate.py
+src/wmwpy/utils/textures.py
+src/wmwpy/utils/waltex.py
+src/wmwpy/utils/file_types/Documents.py
+src/wmwpy/utils/file_types/Images.py
+src/wmwpy/utils/file_types/__init__.py
```

