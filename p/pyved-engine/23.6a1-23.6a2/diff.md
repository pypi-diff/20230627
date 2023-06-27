# Comparing `tmp/pyved-engine-23.6a1.tar.gz` & `tmp/pyved-engine-23.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-engine-23.6a1.tar", last modified: Fri Jun 16 12:06:45 2023, max compression
+gzip compressed data, was "pyved-engine-23.6a2.tar", last modified: Tue Jun 27 14:15:25 2023, max compression
```

## Comparing `pyved-engine-23.6a1.tar` & `pyved-engine-23.6a2.tar`

### file list

```diff
@@ -1,131 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.278943 pyved-engine-23.6a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.282943 pyved-engine-23.6a1/src/pyved_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/Singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/_BaseGameState.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/_ecs_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.282943 pyved-engine-23.6a1/src/pyved_engine/compo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/compo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/compo/gfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/compo/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)    40142 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/compo/packed_capello_ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/compo/vscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.282943 pyved-engine-23.6a1/src/pyved_engine/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/core/Injector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/core/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.286943 pyved-engine-23.6a1/src/pyved_engine/foundation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/foundation/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/foundation/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/foundation/pbackends.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/legacyevent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.286943 pyved-engine-23.6a1/src/pyved_engine/looparts/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.286943 pyved-engine-23.6a1/src/pyved_engine/looparts/ai/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/ai/FSA_classes_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/ai/NorrecBrain.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/ai/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.286943 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/animobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/pathfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/rpgmenu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.290943 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/BaseGuiElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Button2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/DispCenteredPopup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/DispPopup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/TextBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/WidgetBo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/WidgetContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.290943 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/
--rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/IsometricMapViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/IsometricMapViewer0.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/extras.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/isosm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.290943 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/frects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21229 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/rogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/rpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/sysconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tabletop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/terrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.294944 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24970 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.294944 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.294944 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/wang_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/ztilemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/pal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/state_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/tankui.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/src/pyved_engine/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.282943 pyved-engine-23.6a1/src/pyved_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 12:06:45.000000 pyved-engine-23.6a1/src/pyved_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:06:45.298944 pyved-engine-23.6a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 12:06:35.000000 pyved-engine-23.6a1/tests/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.654746 pyved-engine-23.6a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.658746 pyved-engine-23.6a2/src/pyved_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/Singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/_BaseGameState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/_ecs_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/_pyv_implem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.658746 pyved-engine-23.6a2/src/pyved_engine/compo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/compo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/compo/gfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/compo/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40142 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/compo/packed_capello_ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/compo/vscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.658746 pyved-engine-23.6a2/src/pyved_engine/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/core/Injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/core_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.658746 pyved-engine-23.6a2/src/pyved_engine/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/foundation/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/foundation/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/foundation/pbackends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/legacyevent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.662746 pyved-engine-23.6a2/src/pyved_engine/looparts/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.662746 pyved-engine-23.6a2/src/pyved_engine/looparts/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/ai/FSA_classes_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/ai/NorrecBrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.662746 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/animobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/pathfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/rpgmenu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.666746 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/BaseGuiElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Button2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/DispCenteredPopup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/DispPopup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/TextBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/WidgetBo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/WidgetContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.666746 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/
+-rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/IsometricMapViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/IsometricMapViewer0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/isosm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.666746 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/frects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21229 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/rpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/sysconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tabletop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/terrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.666746 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24970 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/wang_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/ztilemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/pal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/state_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/tankui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/src/pyved_engine/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.658746 pyved-engine-23.6a2/src/pyved_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 14:15:25.000000 pyved-engine-23.6a2/src/pyved_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:15:25.670746 pyved-engine-23.6a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 14:15:16.000000 pyved-engine-23.6a2/tests/test_engine.py
```

### Comparing `pyved-engine-23.6a1/LICENSE` & `pyved-engine-23.6a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/PKG-INFO` & `pyved-engine-23.6a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved-engine
-Version: 23.6a1
+Version: 23.6a2
 Summary: Custom game engine built upon python/pygame
 Home-page: https://github.com/gaudiatech/pyved-engine
 Author: moonb3ndr et al.
 Author-email: thomas.iw@kata.games
 License: LGPL3
 Keywords: Python,Pygame,Game Engine
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyved-engine Version: 23.6a1 Summary: Custom game
+Metadata-Version: 2.1 Name: pyved-engine Version: 23.6a2 Summary: Custom game
 engine built upon python/pygame Home-page: https://github.com/gaudiatech/pyved-
 engine Author: moonb3ndr et al. Author-email: thomas.iw@kata.games License:
 LGPL3 Keywords: Python,Pygame,Game Engine Description-Content-Type: text/
 markdown License-File: LICENSE [https://gaudia-tech.com/shared/pyved-engine-
 logo.png]
                               join_us_on_Discord
                              [join_us_on_Discord]
```

### Comparing `pyved-engine-23.6a1/README.md` & `pyved-engine-23.6a2/README.md`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/setup.py` & `pyved-engine-23.6a2/setup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/Singleton.py` & `pyved-engine-23.6a2/src/pyved_engine/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/_BaseGameState.py` & `pyved-engine-23.6a2/src/pyved_engine/_BaseGameState.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/__init__.py` & `pyved-engine-23.6a2/src/pyved_engine/_pyv_implem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,368 +1,245 @@
-"""
-+-----------------------------------------------------+
-| KENGI [K]atagames [ENGI]ne                          |
-| Motto ~ Never slow down the innovation              |
-|                                                     |
-| Main author: wkta-tom (github.com/wkta)             |
-|                                                     |
-| an open-source project funded by GAUDIA TECH INC.   |
-| https://github.com/gaudiatech/kengi                 |
-+-----------------------------------------------------+
-
- * defines a subset of the pygame library (chosen functions & objects)
-  and creates a wrapper around it
-
- * allows for a swift implementation of two essential design patterns:
-   Mediator and Model-View-Contoller
-
- * provides easy access to data structures useful in game development:
-   stacks, matrices, trees, graphs, finite state machines, cellular automata
-
- * provides algorithms that may be tricky to code but are super-useful:
-   A-star, Minimax, a FOV algorithm for a 2D grid based world,
-
- * is extensible: kengi is capable of receiving custom events and custom
-  extensions, for example a custom GUI manager, an isometric engine, or
-  antything similar, without requiring any architectural change
-
- * can run along with the KataSDK but can also be detached, to run independently
-
- * does not know ANYTHING about whether your code runs in a web browser or not,
-  although the engine can be hacked to allow such a possibility
-
- * incentivizes you, the creator, to write clean readable easy-to-refactor &
-  easy-to-reuse code!
-"""
-import time
-from abc import ABCMeta, abstractmethod
-
-from ._ecs_pattern import entity, component, EntityManager, System, SystemManager
-
-from . import _hub as hub
-from . import pal
-from . import state_management as _state_sm
-from . import struct
-from . import tankui
-from ._BaseGameState import BaseGameState
+from . import _hub
+from . import events
+from . import state_management as _st_management_module
+from . import vars
 from .__version__ import ENGI_VERSION as _VER_CST
-from ._hub import Injector
-from .compo import gfx
 from .compo import vscreen
-from .compo.modes import GameModeMger, BaseGameMode
-from .compo.vscreen import flip, proj_to_vscreen
-from .core import events
-from .core.events import Emitter, EvListener, EngineEvTypes, game_events_enum
-from .foundation import defs
-from .foundation.defs import STD_SCR_SIZE, KengiEv, Singleton
-from .foundation.interfaces import PygameIface
-from .state_management import declare_game_states
-from .util import underscore_format, camel_case_format
-
-
-_active_state = False
-_gameticker = None
-one_plus_init = False
-_stored_kbackend = None
-pbackend_name = ''  # can be modified from elsewhere
-
-
-class Objectifier:
-    def __init__(self, **entries):
-        self.__dict__.update(entries)
+from .compo.vscreen import flip as _flip_screen
 
+# We avoid polluting the "pyv.*" namespace also we make it very clear what is the list of
+# functions that are made available when typing "import pyved_engine as pyv"
 
-def _show_ver_infos():
-    print(f'KENGI - ver {_VER_CST}, built on top of ')
-
-
-def is_ready():
-    global one_plus_init
-    return one_plus_init
-
-
-def bootstrap_e(print_ver_info=True):
-    """
-    ensure the engine is ready to be used
-    :param print_ver_info: bool
-    :return:
-    """
-    global one_plus_init, _gameticker, _stored_kbackend, pbackend_name, pygame
-    if one_plus_init:
-        return
-    del pygame
-    one_plus_init = True
-    if print_ver_info:
-        # skip the msg, (if running KENGI along with katasdk, the sdk has already printed out ver. infos)
-        _show_ver_infos()
-
-    # --> init newest event system! in nov22
-    # from here and later,
-    # we know that kengi_inj has been updated, so we can build a primal backend
-    from .foundation.pbackends import build_primalbackend
-    _stored_kbackend = build_primalbackend(pbackend_name)  # by default: local ctx
-    events.EvManager.instance().a_event_source = _stored_kbackend
-
-    # TODO quick fix this part!
-    # event.create_manager()
-    # _gameticker = event.GameTicker()
-
-    # dry import
-    vscreen.cached_pygame_mod = hub.pygame
-
-
-def screen_param(gfx_mode_code, paintev=None, screen_dim=None):
-    global _active_state, config
+__all__ = [  # the full PYV INTERFACE/API SPECIFICATION
+    'bootstrap_e',
+    'close_game',
+    'draw_circle',
+    'draw_polygon',
+    'draw_rect',
+    'get_ev_manager',
+    'get_game_ctrl',
+    'get_surface',
+    'get_ready_flag',
+    'get_version',
+    'init',
+    'preload_assets',
+]
+
+
+# private variables
+_ready_flag = False  # if set to True, means that bootstrap_e has been called at least once
+_init_flag = False  # if set to True, means the display is active right now
+_pyv_backend = None
+_ref_pygame = None
+_joystick = None
+_existing_game_ctrl = None
+
+
+# -------------------------------
+#  private functions AND classes
+# -------------------------------
+def _screen_param(gfx_mode_code, paintev=None, screen_dim=None):
+    global _init_flag
+    if isinstance(gfx_mode_code, int) and -1 < gfx_mode_code <= 3:
+        if gfx_mode_code == 0 and screen_dim is None:
+            ValueError(f'graphic mode 0 required an extra valid screen_dim argument(provided by user: {screen_dim})')
+
+        # from here, we know that the gfx_mode_code is 100% valid
+        conventionw, conventionh = vars.disp_size
+        if gfx_mode_code != 0:
+            adhoc_upscaling = gfx_mode_code
+            taille_surf_dessin = int(conventionw / gfx_mode_code), int(conventionh / gfx_mode_code)
+        else:
+            adhoc_upscaling = 1
+            taille_surf_dessin = screen_dim
+            print(adhoc_upscaling, taille_surf_dessin)
+        # ---------------------------------
+        #  legacy code, not modified in july22. It's complex but
+        # it works so dont modify unless you really know what you're doing ;)
+        # ---------------------------------
+        if vscreen.stored_upscaling is None:  # stored_upscaling isnt relevant <= webctx
+            _active_state = True
+            pygame_surf_dessin = _hub.pygame.display.set_mode(taille_surf_dessin)
+            vscreen.set_virtual_screen(pygame_surf_dessin)
+        else:
 
-    if not isinstance(gfx_mode_code, int) and (1 <= gfx_mode_code <= 3):
+            pygame_surf_dessin = _hub.pygame.surface.Surface(taille_surf_dessin)
+            vscreen.set_virtual_screen(pygame_surf_dessin)
+            vscreen.set_upscaling(adhoc_upscaling)
+            if paintev:
+                paintev.screen = pygame_surf_dessin
+            if _init_flag:
+                return
+            _init_flag = True
+
+            if gfx_mode_code:
+                pgscreen = _hub.pygame.display.set_mode(vars.disp_size)
+            else:
+                pgscreen = _hub.pygame.display.set_mode(taille_surf_dessin)
+            vscreen.set_realpygame_screen(pgscreen)
+    else:
         e_msg = f'graphic mode requested({gfx_mode_code}: {type(gfx_mode_code)}) isnt a valid one! Expected type: int'
         raise ValueError(e_msg)
 
-    # from here, we know that the gfx_mode_code is 100% valid
-    conventionw, conventionh = STD_SCR_SIZE
-    if gfx_mode_code != 0:
-        adhoc_upscaling = gfx_mode_code
-        taille_surf_dessin = int(conventionw / gfx_mode_code), int(conventionh / gfx_mode_code)
-    else:
-        if screen_dim is None:
-            raise ValueError(f'graphic mode 0 required a valid screen_dim arg (provided by user: {screen_dim})')
-        adhoc_upscaling = 1
-        taille_surf_dessin = screen_dim
-
-    config.SCR_SIZE = taille_surf_dessin
-    config.UPSCALING = adhoc_upscaling
-
-    # ---------------------------------
-    #  legacy code, not modified in july22. It's complex but
-    # it works so dont modify unless you really know what you're doing ;)
-    # ---------------------------------
-    if vscreen.stored_upscaling is None:  # stored_upscaling isnt relevant <= webctx
-        _active_state = True
-        pygame_surf_dessin = hub.pygame.display.set_mode(taille_surf_dessin)
-        vscreen.set_virtual_screen(pygame_surf_dessin)
-    else:
-
-        pygame_surf_dessin = hub.pygame.surface.Surface(taille_surf_dessin)
-        vscreen.set_virtual_screen(pygame_surf_dessin)
-        vscreen.set_upscaling(adhoc_upscaling)
-        if paintev:
-            paintev.screen = pygame_surf_dessin
-        if _active_state:
-            return
-        _active_state = True
-
-        if gfx_mode_code:
-            pgscreen = hub.pygame.display.set_mode(STD_SCR_SIZE)
-        else:
-            pgscreen = hub.pygame.display.set_mode(taille_surf_dessin)
-        vscreen.set_realpygame_screen(pgscreen)
-
-
-
-_joy = None
-
-
-def get_surface():
-    global _active_state
-    if not is_ready():
-        raise Exception('calling kengi.get_surface() while the engine isnt ready! (no previous bootstrap op.)')
-    if not _active_state:
-        raise Exception('kengi.init has not been called yet')
-    return vscreen.screen
-
-
-# TODO repair this part, so it fits kengi v22.11.3+
 
-# def declare_states(gsdefinition, assoc_gscode_cls, mod_glvars=None):
-#     global _multistate_flag, state_stack, _stack_based_ctrl
-#     _multistate_flag = True
-#     state_stack = struct.Stack()
-#     _stack_based_ctrl = event.StackBasedGameCtrl(
-#         _gameticker, gsdefinition, mod_glvars, assoc_gscode_cls
-#     )
+def _show_ver_infos():
+    print(f'KENGI - ver {_VER_CST}, built on top of ')
 
 
 class _MyGameCtrl(events.EvListener):
-    MAXFPS = 75
 
     def __init__(self):
         super().__init__()
-        self._clock = hub.kengi_inj['pygame'].time.Clock()
+        self._clock = vars.game_ticker
         self.gameover = False
 
     def on_gameover(self, ev):
         self.gameover = True
 
     def loop(self):
-        if state_management.multistate_flag:  # force this, otherwise the 1st state enter method isnt called
-            self.pev(events.EngineEvTypes.Gamestart)
+        # if state_management.multistate_flag:  # force this, otherwise the 1st state enter method isnt called
+        #     self.pev(events.EngineEvTypes.Gamestart)
 
         while not self.gameover:
             self.pev(events.EngineEvTypes.Update)
-            self.pev(events.EngineEvTypes.Paint, screen=vscreen.screen)
+            self.pev(events.EngineEvTypes.Paint, screen=vars.screen)
             self._manager.update()
-            flip()
-            self._clock.tick(self.MAXFPS)
+            _flip_screen()
+            self._clock.tick(vars.max_fps)
 
 
-def get_game_ctrl():
-    return _MyGameCtrl()
+# --------------------------
+#  public functions
+# --------------------------
+def bootstrap_e(print_version=True):
+    global _ready_flag, _pyv_backend
+    if not _ready_flag:
+        _ready_flag = True
+        if print_version:
+            # skip the msg, (if running KENGI along with katasdk, the sdk has already printed out ver. infos)
+            _show_ver_infos()
+        # --> init newest event system! in nov22
+        # from here and later,
+        # we know that kengi_inj has been updated, so we can build a primal backend
+        from .foundation.pbackends import build_primalbackend
+        _pyv_backend = build_primalbackend(vars.backend_name)  # by default: local ctx
+        events.EvManager.instance().a_event_source = _pyv_backend
+        # TODO quick fix this part!
+        # event.create_manager()
+        # _gameticker = event.GameTicker()
+        # dry import
+        vscreen.cached_pygame_mod = _hub.pygame
+
+
+def draw_circle(surface, color_arg, position2d, radius, width=0):
+    _ref_pygame.draw.circle(surface, color_arg, position2d, radius, width)
 
 
-def get_ev_manager():  # saves some time
-    return events.EvManager.instance()
+def draw_polygon(surface, color_arg, point_li, width=0):
+    _ref_pygame.draw.polygon(surface, color_arg, point_li, width)
 
 
-class GameTpl(metaclass=ABCMeta):
-    """
-    the "no name" game template class. It allows to define your game in a quick way,
-    by redefining one or several methods: enter, update, exit
-    """
-    INFO_STOP_MSG = 'kengi.GameTpl->the loop() call has ended.'
-    ERR_LOCK_MSG = 'kengi.GameTpl.loop called while SAFETY_LOCK is on!'
-    SAFETY_LOCK = False  # can be set to True from outside, if you don't want a game to call .loop()
-    MAXFPS = 75
+def draw_rect(surface, color_arg, rect_obj, width=0):
+    _ref_pygame.draw.rect(surface, color_arg, rect_obj, width)
 
-    def __init__(self):
-        self._manager = None
-        self.gameover = False
-        self.clock = hub.kengi_inj['pygame'].time.Clock()
-        self.nxt_game = 'niobepolis'
-
-    @abstractmethod
-    def init_video(self):
-        raise NotImplementedError
-
-    def setup_ev_manager(self):
-        self._manager.setup()
-
-    def enter(self, vms=None):
-        """
-        Careful if you redefine this:
-        one *HAS TO* bind the ev manager to self._manager and call .setup, somehow
-        """
-        self._manager = events.EvManager.instance()
-        self.init_video()
-        self.setup_ev_manager()
-
-        # gamestart event HAS TO be pushed so the game rly starts...
-        self._manager.post(EngineEvTypes.Gamestart)
-
-    def update(self, infot):
-        self._manager.post(EngineEvTypes.Update, curr_t=infot)
-        self._manager.post(EngineEvTypes.Paint, screen=vscreen.screen)
-        self._manager.update()
-        pyg = hub.kengi_inj['pygame']
-        pk = pyg.key.get_pressed()
-        if pk[pyg.K_ESCAPE] or self.gameover:
-            return 2, self.nxt_game
-        flip()
-        self.clock.tick(self.MAXFPS)
-
-    def exit(self, vms=None):
-        quit()
-
-    def loop(self):
-        """
-        its forbidden to call .loop() in the web ctx, but its convenient in the local ctx
-        if one wants to test a program without using the Kata VM
-        :return:
-        """
-        # lock mechanism, for extra safety so we never call .loop() in the web ctx
-        if self.SAFETY_LOCK:
-            raise ValueError(self.ERR_LOCK_MSG)
-
-        # use enter, update, exit to handle the global "run game logic"
-        self.enter()
-
-        while not self.gameover:
-            infot = time.time()
-            self.update(infot)
-        self.exit()
-        print(self.INFO_STOP_MSG)
-
-
-# ----------------------------
-#  init & quit
-# ----------------------------
-class _Config:
-    MAXFPS = 45
-    SCR_SIZE = (None, None)
-    UPSCALING = None  # not defined, yet
 
+def init(gfc_mode=1, caption=None, maxfps=60, screen_dim=None):
+    global _joystick, _ref_pygame, _existing_game_ctrl
+    bootstrap_e()
 
-config = _Config
+    _ref_pygame = _hub.kengi_inj['pygame']
+    _ref_pygame.init()
+    _ref_pygame.mixer.init()  # activate sounds
 
+    vars.game_ticker = _ref_pygame.time.Clock()
+    vars.max_fps = maxfps
 
-def init(gfc_mode=1, caption=None, maxfps=60, screen_dim=None):
-    global _gameticker, _joy, config
-    bootstrap_e()
-    config.MAXFPS = int(maxfps)
-    pygm = hub.pygame
-    pygm.init()
-    pygm.mixer.init()
+    _existing_game_ctrl = _MyGameCtrl()
 
-    jc = _stored_kbackend.joystick_count()
+    jc = _pyv_backend.joystick_count()
     if jc > 0:
         # ------ init the joystick ------
-        _joy = _stored_kbackend.joystick_init(0)
-        name = _stored_kbackend.joystick_info(0)
+        _joystick = _pyv_backend.joystick_init(0)
+        name = _pyv_backend.joystick_info(0)
         print(name + ' detected')
         # numaxes = _joy.get_numaxes()
         # numballs = _joy.get_numballs()
         # numbuttons = _joy.get_numbuttons()
         # numhats = _joy.get_numhats()
         # print(numaxes, numballs, numbuttons, numhats)
 
-    screen_param(gfc_mode, screen_dim=screen_dim)
+    _screen_param(gfc_mode, screen_dim=screen_dim)
     if caption is None:
         caption = f'untitled demo, uses KENGI ver {_VER_CST}'
-    pygm.display.set_caption(caption)
+    _ref_pygame.display.set_caption(caption)
 
 
-def quit():  # we keep the "quit" name bc of pygame
-    global _active_state
-    if _active_state:
-        if _state_sm.multistate_flag:
-            _state_sm.multistate_flag = False
-            _state_sm.stack_based_ctrl.turn_off()
-            _state_sm.stack_based_ctrl = None
-        if hub.kengi_inj.is_loaded('ascii') and hub.ascii.is_ready():
-            hub.ascii.reset()
+def get_ev_manager():
+    return events.EvManager.instance()
 
-        events.EvManager.instance().hard_reset()
-        vscreen.init2_done = False
-        pyg = get_injector()['pygame']
-        pyg.mixer.quit()
-        pyg.quit()
-        _active_state = False
 
+def get_game_ctrl():
+    global _existing_game_ctrl
+    if _existing_game_ctrl is None:
+        raise Exception('get_game_ctrl called, while engine is not init.')
+    return _existing_game_ctrl
 
-# ----------------------------
-#  Related to lazy import
-# ----------------------------
-pygame = PygameIface()
 
+def get_ready_flag():
+    global _ready_flag
+    return _ready_flag
 
-def get_injector():
-    return hub.kengi_inj
 
+def get_surface():
+    global _init_flag
+    if not get_ready_flag():
+        raise Exception('calling kengi.get_surface() while the engine isnt ready! (no previous bootstrap op.)')
+    if not _init_flag:
+        raise Exception('kengi.init has not been called yet')
+    return vars.screen
 
-def plugin_bind(plugin_name, pypath):
-    hub.kengi_inj.register(plugin_name, pypath)
 
+def get_version():
+    return _VER_CST
 
-def bulk_plugin_bind(darg: dict):
+
+def preload_assets(adhoc_dict: dict, prefix_asset_folder=None):
     """
-    :param darg: association extension(plug-in) name to a pypath
+    expected to find the (mandatory) key 'images',
+    also we may find the (optionnal) key 'sounds'
+    :param prefix_asset_folder:
+    :param adhoc_dict:
     :return:
     """
-    for pname, ppath in darg.items():
-        plugin_bind(ppath, ppath)
+    for gfx_elt in adhoc_dict['images']:
+        filepath = gfx_elt if (prefix_asset_folder is None) else prefix_asset_folder + gfx_elt
+        vars.images[gfx_elt.split('.')[0]] = _ref_pygame.image.load(filepath)
+
+    if 'sounds' in adhoc_dict:
+        for snd_elt in adhoc_dict['sounds']:
+            filepath = snd_elt if (prefix_asset_folder is None) else prefix_asset_folder + snd_elt
+            vars.sounds[snd_elt.split('.')[0]] = _ref_pygame.mixer.Sound(filepath)
+
+
+def close_game():
+    global _init_flag, _existing_game_ctrl
+    vars.screen = None
+
+    vars.images.clear()
+    vars.sounds.clear()
+    _existing_game_ctrl = None
+
+    if _init_flag:
+        _init_flag = False
+
+        if _st_management_module.multistate_flag:
+            _st_management_module.multistate_flag = False
+            _st_management_module.stack_based_ctrl.turn_off()
+            _st_management_module.stack_based_ctrl = None
 
+        if _hub.kengi_inj.is_loaded('ascii') and _hub.ascii.is_ready():
+            _hub.ascii.reset()
 
-def __getattr__(attr_name):
-    if attr_name in ('ver', 'vernum'):
-        return _VER_CST
-    if is_ready():
-        return getattr(hub, attr_name)
-    raise AttributeError(f"kengi cannot lazy load, it hasnt bootstrap yet! (user request: {attr_name})")
+        events.EvManager.instance().hard_reset()
+        vscreen.init2_done = False
+        _hub.pygame.mixer.quit()
+        _hub.pygame.quit()
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/__version__.py` & `pyved-engine-23.6a2/src/pyved_engine/__version__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 VYEAR_2DIG = 23  # remember to use only 2 digits
 VMONTH = 6
 _idx = 1  # 1 =alpha, 2 =beta, 3 =release candidate, 0 =legit release
-VRANK = 1
+VRANK = 2
 
 """
 We target this standard format:
 - Alpha release     yy.MMaN
 - Beta release      yy.MMbN
 - Release candidate yy.MMrcN
 - Final release     yy.MM
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/_ecs_pattern.py` & `pyved-engine-23.6a2/src/pyved_engine/_ecs_pattern.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/_hub.py` & `pyved-engine-23.6a2/src/pyved_engine/_hub.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/compo/gfx.py` & `pyved-engine-23.6a2/src/pyved_engine/compo/gfx.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/compo/modes.py` & `pyved-engine-23.6a2/src/pyved_engine/compo/modes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/compo/packed_capello_ft.py` & `pyved-engine-23.6a2/src/pyved_engine/compo/packed_capello_ft.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/compo/vscreen.py` & `pyved-engine-23.6a2/src/pyved_engine/compo/vscreen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..foundation import defs
+from .. import vars
 
 
 _vsurface = None
 _vsurface_required = True
 
 cached_pygame_mod = None  # init from outside when one calls kengi.bootstrap_e
 special_flip = 0  # flag, set it to 1 when using web ctx
-screen = None
 stored_upscaling = 1
 defacto_upscaling = None
 
 # hopefully i will be able to simplify this:
 ctx_emuvram = None
 canvas_emuvram = None
 canvas_rendering = None
@@ -31,17 +31,17 @@
     if _vsurface_required:
         # TODO
         pass
 
     if not special_flip:  # flag can be off if the extra blit/transform has to disabled (web ctx)
         realscreen = cached_pygame_mod.display.get_surface()
         if 1 == stored_upscaling:
-            realscreen.blit(screen, (0, 0))
+            realscreen.blit(vars.screen, (0, 0))
         else:
-            cached_pygame_mod.transform.scale(screen, defs.STD_SCR_SIZE, realscreen)
+            cached_pygame_mod.transform.scale(vars.screen, defs.STD_SCR_SIZE, realscreen)
 
     cached_pygame_mod.display.update()
 
 
 # ------------------------------------
 #   old code
 # ------------------------------------
@@ -69,20 +69,16 @@
     if real_pygamescreen:
         print('warning: set_realpygame_scneen called a 2nd time. Ignoring request')
         return
     real_pygamescreen = ref_surf
 
 
 def set_virtual_screen(ref_surface):
-    global screen, screen_rank, defacto_upscaling
-    screen = ref_surface
-    w = screen.get_size()[0]
+    global screen_rank, defacto_upscaling
+    vars.screen = ref_surface
+    w = vars.screen.get_size()[0]
     defacto_upscaling = 960/w
     screen_rank += 1
 
 
-def get_screen():
-    return screen
-
-
 def proj_to_vscreen(org_screen_pos):
     return conv_to_vscreen(*org_screen_pos)
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/core/Injector.py` & `pyved-engine-23.6a2/src/pyved_engine/core/Injector.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/core/events.py` & `pyved-engine-23.6a2/src/pyved_engine/core/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,21 +152,21 @@
 
         names = list()
         self._known_ev_types = EngineEvTypes.content.copy()
 
         for evname, eid in EngineEvTypes.content.items():
             names.append(to_snakecase(evname))
 
-        if given_extra_penum is not None:
+        if given_extra_penum is None:
+            self._cached_extra_penum = None
+        else:
             self._cached_extra_penum = given_extra_penum
             self._known_ev_types.update(given_extra_penum.content)
             for evname, eid in given_extra_penum.content.items():
                 names.append(to_snakecase(evname))
-        else:
-            self._cached_extra_penum = None
 
         # force a {refresh regexp} op!
         self._refresh_regexp(names)
 
         for ename_cc, etype in self._known_ev_types.items():
             self._etype_to_sncname[etype] = to_snakecase(ename_cc)
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/foundation/defs.py` & `pyved-engine-23.6a2/src/pyved_engine/foundation/defs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/foundation/interfaces.py` & `pyved-engine-23.6a2/src/pyved_engine/foundation/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/foundation/pbackends.py` & `pyved-engine-23.6a2/src/pyved_engine/foundation/pbackends.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/legacyevent.py` & `pyved-engine-23.6a2/src/pyved_engine/legacyevent.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/ai/FSA_classes_base.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/ai/FSA_classes_base.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/ai/NorrecBrain.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/ai/NorrecBrain.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/ai/tests.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/ai/tests.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/anim.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/anim.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/ascii.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/ascii.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/console.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/console.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/animobs.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/animobs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/dialogue.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/dialogue.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/pathfinding.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/pathfinding.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/demolib/rpgmenu.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/demolib/rpgmenu.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/BaseGuiElement.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/BaseGuiElement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from abc import ABCMeta, abstractmethod
-from ...compo.vscreen import get_screen
+from ... import vars
 
 
 ANCHOR_LEFT, ANCHOR_RIGHT, ANCHOR_CENTER = range(34151, 34151+3)
 
 
 class BaseGuiElement(metaclass=ABCMeta):
     """
     Base cls for any Gui element class
     """
     free_gui_id = 821798
 
     def __init__(self):
         self._id = self.__class__.free_gui_id
         self.__class__.free_gui_id -= 1
-
         self._parent = None
-
-        self._scrref = get_screen()
-
+        self._scrref = vars.screen
         self._debug = 0
         self._abs_pos = [0, 0]
         self._dim = [None, None]
         self._anchor_type = ANCHOR_LEFT
         self._debug = False
 
         # not all widgets can be de-activated
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Button.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Button.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Button2.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Button2.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/DispCenteredPopup.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/DispCenteredPopup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/DispPopup.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/DispPopup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Label.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Label.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/TextBlock.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/TextBlock.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/Trigger.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/Trigger.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/WidgetBo.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/WidgetBo.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/WidgetContainer.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/WidgetContainer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/__init__.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/base.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/base.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/gui/text.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/gui/text.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/IsometricMapViewer.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/IsometricMapViewer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/IsometricMapViewer0.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/IsometricMapViewer0.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/extras.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/extras.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/isometric/model.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/isometric/model.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/__init__.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/frects.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/frects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ... import _hub
-from ...compo import vscreen as core
+from ... import vars
 
 
 ANCHOR_UPPERLEFT = (0, 0)
 ANCHOR_UPPERRIGHT = (2, 0)
 ANCHOR_CENTER = (1, 1)
 ANCHOR_LOWERLEFT = (0, 2)
 ANCHOR_LOWERRIGHT = (2, 2)
@@ -27,11 +27,11 @@
 
     def get_rect(self):
         if self.parent:
             prect = self.parent.get_rect()
             x0 = prect.left + (prect.w // 2) * self.anchor[0]
             y0 = prect.top + (prect.h // 2) * self.anchor[1]
         else:
-            sw, sh = core.get_screen().get_size()
+            sw, sh = vars.screen.get_size()
             x0 = (sw // 2) * self.anchor[0]
             y0 = (sh // 2) * self.anchor[1]
         return pygame.Rect(self.dx + x0, self.dy + y0, self.w, self.h)
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/general.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import weakref
 
 from . import frects
 from . import image
 from .image import TEXT_COLOR, truncline, render_text
 from ... import _hub
+from ... import vars
 from ...compo import vscreen
 
 
 pygame = _hub.pygame
 
 
 class KeyObject(object):
@@ -54,15 +55,15 @@
         self.l = l
         self.r = r
         self.transparent = transparent
 
     def render(self, dest, scr=None):
         """Draw this decorative border at dest on screen."""
         if scr is None:
-            scr = vscreen.get_screen()
+            scr = vars.screen
 
         # We're gonna draw a decorative border to surround the provided area.
         if self.border == None:
             self.border = image.Image(self.border_name, self.border_width, self.border_width)
         if self.tex_name and not self.tex:
             self.tex = image.Image(self.tex_name, self.tex_width, self.tex_width)
             if self.transparent:
@@ -220,15 +221,15 @@
 ANIMFONT = None
 MEDIUMFONT = None
 ALTTEXTFONT = None  # Use this instead of MEDIUMFONT when you want to shake things up a bit.
 POSTERS = list()
 
 my_state = GameState()
 # fix: add ref to screen
-my_state.screen = vscreen.get_screen()
+my_state.screen = vars.screen
 
 # The FPS the rules runs at.
 FPS = 30
 
 # Use a timer to control FPS.
 TIMEREVENT = pygame.USEREVENT
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/image.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import weakref
 from itertools import chain
-
+from ... import vars
 from ... import _hub
-from ...compo import vscreen as core
 
 
 DEFAULT_COLOR_KEY = (255, 0, 255)
 TEXT_COLOR = (240, 240, 50)
 pygame = _hub.pygame
 # Keep a list of already-loaded images, to save memory when multiple objects
 # need to use the same image file.
@@ -83,15 +82,15 @@
 
 
 def draw_text(font, text, rect, color=TEXT_COLOR, justify=-1, antialias=True, dest_surface=None):
     # Draw some text to the screen with the provided options.
     if dest_surface:
         dsu = dest_surface
     else:
-        dsu = core.get_screen()
+        dsu = vars.screen
 
     # myimage = render. ...
     render_text(font, text, rect.width, color, justify, antialias, dsuu=dsu, moff=rect.topleft)
     return
 
     if justify == 0:
         myrect = myimage.get_rect(midtop=rect.midtop)
@@ -115,15 +114,15 @@
                 self.bitmap = pygame.image.load(fname).convert_alpha()
                 self.bitmap.set_colorkey(color_key, flags)
         else:
             self.bitmap = pygame.Surface((frame_width, frame_height))
             self.bitmap.fill(color_key)
             self.bitmap.set_colorkey(color_key, flags)
 
-        self.scrref = core.get_screen()
+        self.scrref = vars.screen
 
         self.fname = fname
         self.flags = flags
         self.transparent = transparent
         self.color_key = color_key
         if transparent:
             alpha = int(transparent)
@@ -172,15 +171,15 @@
 
     def render_c(self, dest=(0, 0), frame=0, dest_surface=None ):
         # As above, but the dest coordinates point to the center of the image.
         area = self._get_frame_area(frame)
 
         dest_c = self.get_rect(frame)
         dest_c.center = dest
-        dest_surface = dest_surface or core.get_screen()  # new way to retrieve the surface used for display
+        dest_surface = dest_surface or vars.screen  # new way to retrieve the surface used for display
 
         dest_surface.blit(self.bitmap, dest_c, area)
 
     def get_subsurface(self, frame):
         # Return one of the frames as a pygame subsurface.
         area = self._get_frame_area(frame)
         return self.bitmap.subsurface(area)
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/polarbear/widgets.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/polarbear/widgets.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/rogue.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/rogue.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/rpg.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/rpg.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/sysconsole.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/sysconsole.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tabletop.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tabletop.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/terrain.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/terrain.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/data.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/data.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/misc.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/misc.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/__init__.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/common_types.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/common_types.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/layer.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parser.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/layer.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/properties.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/properties.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_map.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_object.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tileset.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/wang_set.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/json/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/layer.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/properties.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/properties.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_map.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_object.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tileset.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/wang_set.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/parsers/tmx/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_map.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_object.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/tileset.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/util.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/util.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/wang_set.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/pytiled_parser/world.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/pytiled_parser/world.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/looparts/tmx/ztilemap.py` & `pyved-engine-23.6a2/src/pyved_engine/looparts/tmx/ztilemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # game settings
 # Ensure no partial squares with these values
 WINDOW_WIDTH = 1024  # 16 * 64 or 32 * 32 or 64 * 16
 WINDOW_HEIGHT = 768  # 16 * 48 or 32 * 24 or 64 * 12
 TILESIZE = 64
 BLACK = (0, 0, 0)
 
-kengi = katasdk.kengi
+kengi = katasdk.pyv
 pygame = kengi.pygame
 TileLayerCls = pytiled_parser.layer.TileLayer
 ObjLayerCls = pytiled_parser.layer.ObjectLayer
 
 
 # By default, the collide method uses the default rect of the player.
 # We create this custom method to compare the player's 'hit_rect' instead.
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine/pal.py` & `pyved-engine-23.6a2/src/pyved_engine/pal.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/state_management.py` & `pyved-engine-23.6a2/src/pyved_engine/state_management.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/struct.py` & `pyved-engine-23.6a2/src/pyved_engine/struct.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/tankui.py` & `pyved-engine-23.6a2/src/pyved_engine/tankui.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine/util.py` & `pyved-engine-23.6a2/src/pyved_engine/util.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.6a1/src/pyved_engine.egg-info/PKG-INFO` & `pyved-engine-23.6a2/src/pyved_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyved-engine
-Version: 23.6a1
+Version: 23.6a2
 Summary: Custom game engine built upon python/pygame
 Home-page: https://github.com/gaudiatech/pyved-engine
 Author: moonb3ndr et al.
 Author-email: thomas.iw@kata.games
 License: LGPL3
 Keywords: Python,Pygame,Game Engine
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyved-engine Version: 23.6a1 Summary: Custom game
+Metadata-Version: 2.1 Name: pyved-engine Version: 23.6a2 Summary: Custom game
 engine built upon python/pygame Home-page: https://github.com/gaudiatech/pyved-
 engine Author: moonb3ndr et al. Author-email: thomas.iw@kata.games License:
 LGPL3 Keywords: Python,Pygame,Game Engine Description-Content-Type: text/
 markdown License-File: LICENSE [https://gaudia-tech.com/shared/pyved-engine-
 logo.png]
                               join_us_on_Discord
                              [join_us_on_Discord]
```

### Comparing `pyved-engine-23.6a1/src/pyved_engine.egg-info/SOURCES.txt` & `pyved-engine-23.6a2/src/pyved_engine.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 setup.py
 src/pyved_engine/Singleton.py
 src/pyved_engine/_BaseGameState.py
 src/pyved_engine/__init__.py
 src/pyved_engine/__version__.py
 src/pyved_engine/_ecs_pattern.py
 src/pyved_engine/_hub.py
+src/pyved_engine/_pyv_implem.py
+src/pyved_engine/core_classes.py
 src/pyved_engine/legacyevent.py
 src/pyved_engine/pal.py
 src/pyved_engine/state_management.py
 src/pyved_engine/struct.py
 src/pyved_engine/tankui.py
 src/pyved_engine/util.py
+src/pyved_engine/vars.py
 src/pyved_engine.egg-info/PKG-INFO
 src/pyved_engine.egg-info/SOURCES.txt
 src/pyved_engine.egg-info/dependency_links.txt
 src/pyved_engine.egg-info/entry_points.txt
 src/pyved_engine.egg-info/requires.txt
 src/pyved_engine.egg-info/top_level.txt
 src/pyved_engine/compo/__init__.py
```

### Comparing `pyved-engine-23.6a1/tests/test_engine.py` & `pyved-engine-23.6a2/tests/test_engine.py`

 * *Files identical despite different names*

