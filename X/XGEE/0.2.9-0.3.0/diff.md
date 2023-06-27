# Comparing `tmp/XGEE-0.2.9.tar.gz` & `tmp/XGEE-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XGEE-0.2.9.tar", last modified: Sat Jan 14 18:02:18 2023, max compression
+gzip compressed data, was "XGEE-0.3.0.tar", last modified: Tue Jun 27 10:09:50 2023, max compression
```

## Comparing `XGEE-0.2.9.tar` & `XGEE-0.3.0.tar`

### file list

```diff
@@ -1,1047 +1,1054 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.448884 XGEE-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-01-14 18:02:09.000000 XGEE-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2992 2023-01-14 18:02:18.447884 XGEE-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-01-14 18:02:09.000000 XGEE-0.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.164865 XGEE-0.2.9/XGEE.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2992 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    42145 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-14 18:02:18.000000 XGEE-0.2.9/XGEE.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-14 18:02:18.448884 XGEE-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-01-14 18:02:09.000000 XGEE-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.165865 XGEE-0.2.9/xgee/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-01-14 18:02:09.000000 XGEE-0.2.9/xgee/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-01-14 18:02:09.000000 XGEE-0.2.9/xgee/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.166865 XGEE-0.2.9/xgee/core/
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/.git
--rw-r--r--   0 root         (0) root         (0)      358 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/.gitmodules
--rw-r--r--   0 root         (0) root         (0)     1078 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.168865 XGEE-0.2.9/xgee/core/contrib/
--rw-r--r--   0 root         (0) root         (0)   183390 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/bluebird.js
--rw-r--r--   0 root         (0) root         (0)    81530 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/bluebird.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.168865 XGEE-0.2.9/xgee/core/contrib/font-awesome/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.173866 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/
--rw-r--r--   0 root         (0) root         (0)    73117 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/all.css
--rw-r--r--   0 root         (0) root         (0)    58935 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/all.min.css
--rw-r--r--   0 root         (0) root         (0)      732 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/brands.css
--rw-r--r--   0 root         (0) root         (0)      675 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/brands.min.css
--rw-r--r--   0 root         (0) root         (0)    71482 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/fontawesome.css
--rw-r--r--   0 root         (0) root         (0)    57503 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/fontawesome.min.css
--rw-r--r--   0 root         (0) root         (0)      734 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/regular.css
--rw-r--r--   0 root         (0) root         (0)      677 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/regular.min.css
--rw-r--r--   0 root         (0) root         (0)      727 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/solid.css
--rw-r--r--   0 root         (0) root         (0)      669 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/solid.min.css
--rw-r--r--   0 root         (0) root         (0)     8077 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/svg-with-js.css
--rw-r--r--   0 root         (0) root         (0)     6359 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/svg-with-js.min.css
--rw-r--r--   0 root         (0) root         (0)    41312 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/v4-shims.css
--rw-r--r--   0 root         (0) root         (0)    26702 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/css/v4-shims.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.183866 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/
--rw-r--r--   0 root         (0) root         (0)  1248390 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/all.js
--rw-r--r--   0 root         (0) root         (0)  1182553 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/all.min.js
--rw-r--r--   0 root         (0) root         (0)   445294 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/brands.js
--rw-r--r--   0 root         (0) root         (0)   438090 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/brands.min.js
--rw-r--r--   0 root         (0) root         (0)    33929 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/conflict-detection.js
--rw-r--r--   0 root         (0) root         (0)    13502 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/conflict-detection.min.js
--rw-r--r--   0 root         (0) root         (0)    79139 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/fontawesome.js
--rw-r--r--   0 root         (0) root         (0)    37191 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/fontawesome.min.js
--rw-r--r--   0 root         (0) root         (0)   107110 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/regular.js
--rw-r--r--   0 root         (0) root         (0)   103386 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/regular.min.js
--rw-r--r--   0 root         (0) root         (0)   617405 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/solid.js
--rw-r--r--   0 root         (0) root         (0)   604447 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/solid.min.js
--rw-r--r--   0 root         (0) root         (0)    17459 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/v4-shims.js
--rw-r--r--   0 root         (0) root         (0)    15055 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/js/v4-shims.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.191867 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/
--rw-r--r--   0 root         (0) root         (0)   134878 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 root         (0) root         (0)   729325 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 root         (0) root         (0)   134572 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 root         (0) root         (0)    90872 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 root         (0) root         (0)    77444 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 root         (0) root         (0)    34390 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 root         (0) root         (0)   144322 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 root         (0) root         (0)    34092 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 root         (0) root         (0)    16800 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 root         (0) root         (0)    13596 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 root         (0) root         (0)   204866 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 root         (0) root         (0)   910710 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 root         (0) root         (0)   204580 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 root         (0) root         (0)   104252 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 root         (0) root         (0)    80328 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.195867 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.196867 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/
--rw-r--r--   0 root         (0) root         (0)     3528 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.eot
--rw-r--r--   0 root         (0) root         (0)     3320 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
--rw-r--r--   0 root         (0) root         (0)     2180 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1680 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
--rw-r--r--   0 root         (0) root         (0)     7278 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.css
--rw-r--r--   0 root         (0) root         (0)    91213 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.js
--rw-r--r--   0 root         (0) root         (0)     5991 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
--rw-r--r--   0 root         (0) root         (0)    14532 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
--rw-r--r--   0 root         (0) root         (0)    27807 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
--rw-r--r--   0 root         (0) root         (0)   131140 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
--rw-r--r--   0 root         (0) root         (0)    22405 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.js
--rw-r--r--   0 root         (0) root         (0)     5855 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.197867 XGEE-0.2.9/xgee/core/contrib/jquery/
--rw-r--r--   0 root         (0) root         (0)     1097 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    86927 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery/jquery-3.3.1.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.198867 XGEE-0.2.9/xgee/core/contrib/jquery-ui/
--rw-r--r--   0 root         (0) root         (0)     1817 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.200868 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/
--rw-r--r--   0 root         (0) root         (0)     7006 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7074 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4676 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7013 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4632 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 root         (0) root         (0)     6313 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 root         (0) root         (0)    32076 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/jquery-ui.min.css
--rw-r--r--   0 root         (0) root         (0)   253669 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/jquery-ui/jquery-ui.min.js
--rw-r--r--   0 root         (0) root         (0)    13780 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/notify.min.js
--rw-r--r--   0 root         (0) root         (0)      290 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/notifyjs-LICENSE
--rw-r--r--   0 root         (0) root         (0)     1139 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/underscore-LICENSE
--rw-r--r--   0 root         (0) root         (0)    18069 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/contrib/underscore-min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.203868 XGEE-0.2.9/xgee/core/css/
--rw-r--r--   0 root         (0) root         (0)      329 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/UIComponents.canvasSearch.css
--rw-r--r--   0 root         (0) root         (0)     1099 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/app.css
--rw-r--r--   0 root         (0) root         (0)      337 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/canvas.css
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/contextmenu.css
--rw-r--r--   0 root         (0) root         (0)       94 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/layout.css
--rw-r--r--   0 root         (0) root         (0)     4230 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/notes.css
--rw-r--r--   0 root         (0) root         (0)     1974 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/palette.css
--rw-r--r--   0 root         (0) root         (0)     7091 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/css/uiControls.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.207868 XGEE-0.2.9/xgee/core/img/
--rw-r--r--   0 root         (0) root         (0)     2989 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/edit.svg
--rw-r--r--   0 root         (0) root         (0)     3645 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/eye.svg
--rw-r--r--   0 root         (0) root         (0)     5763 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/globe.svg
--rw-r--r--   0 root         (0) root         (0)     3577 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/graph-view-oaam-allocations.svg
--rw-r--r--   0 root         (0) root         (0)     4433 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/graph-view-oaam-functions.svg
--rw-r--r--   0 root         (0) root         (0)     3096 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/graph-view-oaam-hardware.svg
--rw-r--r--   0 root         (0) root         (0)     2830 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/redo.svg
--rw-r--r--   0 root         (0) root         (0)     3529 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tool-domain-status-down.svg
--rw-r--r--   0 root         (0) root         (0)     3152 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tool-domain-status-error.svg
--rw-r--r--   0 root         (0) root         (0)     4286 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tool-domain-status-up-down.svg
--rw-r--r--   0 root         (0) root         (0)     3535 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tool-domain-status-up.svg
--rw-r--r--   0 root         (0) root         (0)     2803 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tool-domain-status.svg
--rw-r--r--   0 root         (0) root         (0)     3449 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/tree.svg
--rw-r--r--   0 root         (0) root         (0)     2788 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/undo.svg
--rw-r--r--   0 root         (0) root         (0)     3010 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/img/view-editor.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.209868 XGEE-0.2.9/xgee/core/js/
--rw-r--r--   0 root         (0) root         (0)     3240 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/DomainStatistics.js
--rw-r--r--   0 root         (0) root         (0)    12997 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/app.js
--rw-r--r--   0 root         (0) root         (0)     5020 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/commands.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.209868 XGEE-0.2.9/xgee/core/js/connectors/
--rw-r--r--   0 root         (0) root         (0)     9049 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/connectors/connectors.graph.js
--rw-r--r--   0 root         (0) root         (0)     4190 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/connectors/connectors.selection.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.209868 XGEE-0.2.9/xgee/core/js/grids/
--rw-r--r--   0 root         (0) root         (0)      415 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/grids/points_grid.svg
--rw-r--r--   0 root         (0) root         (0)     3582 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/ports.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.210868 XGEE-0.2.9/xgee/core/js/ui/
--rw-r--r--   0 root         (0) root         (0)     4761 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/ui/DomainStatusTool.js
--rw-r--r--   0 root         (0) root         (0)     1437 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/ui/ui.colorProvider.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.211868 XGEE-0.2.9/xgee/core/js/workspace/
--rw-r--r--   0 root         (0) root         (0)     3669 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/workspace/workspace.jobs.js
--rw-r--r--   0 root         (0) root         (0)    18830 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/js/workspace/workspace.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.213868 XGEE-0.2.9/xgee/core/jsa/
--rw-r--r--   0 root         (0) root         (0)       52 2023-01-14 18:02:13.000000 XGEE-0.2.9/xgee/core/jsa/.git
--rw-r--r--   0 root         (0) root         (0)     1865 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1291 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.218869 XGEE-0.2.9/xgee/core/jsa/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.224869 XGEE-0.2.9/xgee/core/jsa/img/black/
--rw-r--r--   0 root         (0) root         (0)     2092 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/bubble-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2083 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/bubble.svg
--rw-r--r--   0 root         (0) root         (0)     2214 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/close.svg
--rw-r--r--   0 root         (0) root         (0)     2097 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/folder.svg
--rw-r--r--   0 root         (0) root         (0)     2072 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/home.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     2201 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/maximize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2192 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2880 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/menu-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2862 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/menu.svg
--rw-r--r--   0 root         (0) root         (0)     2075 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/minimize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2066 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     2326 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/redo.svg
--rw-r--r--   0 root         (0) root         (0)     2374 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/settings.svg
--rw-r--r--   0 root         (0) root         (0)     2378 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/undo.svg
--rw-r--r--   0 root         (0) root         (0)     2343 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/view-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/black/view.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/close.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     3731 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/loading.svg
--rw-r--r--   0 root         (0) root         (0)     2443 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2437 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     3173 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/resize-ne.svg
--rw-r--r--   0 root         (0) root         (0)     3172 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/resize-nw.svg
--rw-r--r--   0 root         (0) root         (0)     3173 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/resize-se.svg
--rw-r--r--   0 root         (0) root         (0)     3113 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/resize-sw.svg
--rw-r--r--   0 root         (0) root         (0)     3639 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/restore.svg
--rw-r--r--   0 root         (0) root         (0)     2637 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/tool-default.svg
--rw-r--r--   0 root         (0) root         (0)     2693 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/view-close.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.229869 XGEE-0.2.9/xgee/core/jsa/img/white/
--rw-r--r--   0 root         (0) root         (0)     2083 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/bubble-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2074 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/bubble.svg
--rw-r--r--   0 root         (0) root         (0)     2205 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/close.svg
--rw-r--r--   0 root         (0) root         (0)     2097 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/folder.svg
--rw-r--r--   0 root         (0) root         (0)     2063 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/home.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     2192 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/maximize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2183 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2871 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/menu-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2853 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/menu.svg
--rw-r--r--   0 root         (0) root         (0)     2066 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/minimize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2057 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     2317 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/redo.svg
--rw-r--r--   0 root         (0) root         (0)     2365 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/settings.svg
--rw-r--r--   0 root         (0) root         (0)     2369 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/undo.svg
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/view-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2325 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/img/white/view.svg
--rw-r--r--   0 root         (0) root         (0)    46194 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/jsapplication.css
--rw-r--r--   0 root         (0) root         (0)   357646 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/jsapplication.js
--rw-r--r--   0 root         (0) root         (0)    15308 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/jsa/jsapplicationPlugins.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.230869 XGEE-0.2.9/xgee/core/mxgraph/
--rw-r--r--   0 root         (0) root         (0)    10487 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.230869 XGEE-0.2.9/xgee/core/mxgraph/css/
--rw-r--r--   0 root         (0) root         (0)     4325 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/css/common.css
--rw-r--r--   0 root         (0) root         (0)      486 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/css/explorer.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.236870 XGEE-0.2.9/xgee/core/mxgraph/images/
--rw-r--r--   0 root         (0) root         (0)      137 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/button.gif
--rw-r--r--   0 root         (0) root         (0)       70 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/close.gif
--rw-r--r--   0 root         (0) root         (0)      877 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/collapsed.gif
--rw-r--r--   0 root         (0) root         (0)      907 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/error.gif
--rw-r--r--   0 root         (0) root         (0)      878 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/expanded.gif
--rw-r--r--   0 root         (0) root         (0)      843 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/maximize.gif
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/minimize.gif
--rw-r--r--   0 root         (0) root         (0)      845 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/normalize.gif
--rw-r--r--   0 root         (0) root         (0)       55 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/point.gif
--rw-r--r--   0 root         (0) root         (0)       74 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/resize.gif
--rw-r--r--   0 root         (0) root         (0)      146 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/separator.gif
--rw-r--r--   0 root         (0) root         (0)       56 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/submenu.gif
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/transparent.gif
--rw-r--r--   0 root         (0) root         (0)      276 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/warning.gif
--rw-r--r--   0 root         (0) root         (0)      425 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/warning.png
--rw-r--r--   0 root         (0) root         (0)      275 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/window-title.gif
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/images/window.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.236870 XGEE-0.2.9/xgee/core/mxgraph/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.238870 XGEE-0.2.9/xgee/core/mxgraph/js/editor/
--rw-r--r--   0 root         (0) root         (0)     3232 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultKeyHandler.js
--rw-r--r--   0 root         (0) root         (0)     9716 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultPopupMenu.js
--rw-r--r--   0 root         (0) root         (0)    14610 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultToolbar.js
--rw-r--r--   0 root         (0) root         (0)    74993 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxEditor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.243870 XGEE-0.2.9/xgee/core/mxgraph/js/handler/
--rw-r--r--   0 root         (0) root         (0)     7282 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellHighlight.js
--rw-r--r--   0 root         (0) root         (0)     9337 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellMarker.js
--rw-r--r--   0 root         (0) root         (0)     2992 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellTracker.js
--rw-r--r--   0 root         (0) root         (0)    62381 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxConnectionHandler.js
--rw-r--r--   0 root         (0) root         (0)    13695 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxConstraintHandler.js
--rw-r--r--   0 root         (0) root         (0)    63081 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxEdgeHandler.js
--rw-r--r--   0 root         (0) root         (0)     9925 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxEdgeSegmentHandler.js
--rw-r--r--   0 root         (0) root         (0)     5944 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxElbowEdgeHandler.js
--rw-r--r--   0 root         (0) root         (0)    39448 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxGraphHandler.js
--rw-r--r--   0 root         (0) root         (0)     7701 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxHandle.js
--rw-r--r--   0 root         (0) root         (0)    10128 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxKeyHandler.js
--rw-r--r--   0 root         (0) root         (0)    11402 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxPanningHandler.js
--rw-r--r--   0 root         (0) root         (0)     5293 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxPopupMenuHandler.js
--rw-r--r--   0 root         (0) root         (0)     9837 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxRubberband.js
--rw-r--r--   0 root         (0) root         (0)     6478 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxSelectionCellsHandler.js
--rw-r--r--   0 root         (0) root         (0)     7419 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxTooltipHandler.js
--rw-r--r--   0 root         (0) root         (0)    52962 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxVertexHandler.js
--rw-r--r--   0 root         (0) root         (0)    12044 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/index.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.249871 XGEE-0.2.9/xgee/core/mxgraph/js/io/
--rw-r--r--   0 root         (0) root         (0)     4531 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCellCodec.js
--rw-r--r--   0 root         (0) root         (0)     4207 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxChildChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)    13541 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCodec.js
--rw-r--r--   0 root         (0) root         (0)     2690 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCodecRegistry.js
--rw-r--r--   0 root         (0) root         (0)     1986 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
--rw-r--r--   0 root         (0) root         (0)     1226 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultPopupMenuCodec.js
--rw-r--r--   0 root         (0) root         (0)     9221 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultToolbarCodec.js
--rw-r--r--   0 root         (0) root         (0)     6163 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxEditorCodec.js
--rw-r--r--   0 root         (0) root         (0)     1798 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGenericChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)      621 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGraphCodec.js
--rw-r--r--   0 root         (0) root         (0)     5022 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGraphViewCodec.js
--rw-r--r--   0 root         (0) root         (0)     1705 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxModelCodec.js
--rw-r--r--   0 root         (0) root         (0)    30213 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxObjectCodec.js
--rw-r--r--   0 root         (0) root         (0)     1598 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxRootChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)     4651 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxStylesheetCodec.js
--rw-r--r--   0 root         (0) root         (0)      818 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/io/mxTerminalChangeCodec.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.252871 XGEE-0.2.9/xgee/core/mxgraph/js/layout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.252871 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.254871 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/
--rw-r--r--   0 root         (0) root         (0)     4029 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
--rw-r--r--   0 root         (0) root         (0)     3852 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
--rw-r--r--   0 root         (0) root         (0)    20322 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
--rw-r--r--   0 root         (0) root         (0)     4915 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
--rw-r--r--   0 root         (0) root         (0)    23605 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
--rw-r--r--   0 root         (0) root         (0)    20146 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
--rw-r--r--   0 root         (0) root         (0)    22708 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.256871 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/
--rw-r--r--   0 root         (0) root         (0)    43070 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
--rw-r--r--   0 root         (0) root         (0)      726 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
--rw-r--r--   0 root         (0) root         (0)    16867 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
--rw-r--r--   0 root         (0) root         (0)     3123 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
--rw-r--r--   0 root         (0) root         (0)     2816 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
--rw-r--r--   0 root         (0) root         (0)     4343 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCircleLayout.js
--rw-r--r--   0 root         (0) root         (0)    22959 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCompactTreeLayout.js
--rw-r--r--   0 root         (0) root         (0)     2496 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCompositeLayout.js
--rw-r--r--   0 root         (0) root         (0)     3158 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxEdgeLabelLayout.js
--rw-r--r--   0 root         (0) root         (0)    14338 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxFastOrganicLayout.js
--rw-r--r--   0 root         (0) root         (0)    14251 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxGraphLayout.js
--rw-r--r--   0 root         (0) root         (0)     4851 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxParallelEdgeLayout.js
--rw-r--r--   0 root         (0) root         (0)     5537 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxPartitionLayout.js
--rw-r--r--   0 root         (0) root         (0)     8037 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxRadialTreeLayout.js
--rw-r--r--   0 root         (0) root         (0)    12740 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxStackLayout.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.257871 XGEE-0.2.9/xgee/core/mxgraph/js/model/
--rw-r--r--   0 root         (0) root         (0)    15954 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/model/mxCell.js
--rw-r--r--   0 root         (0) root         (0)     2933 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/model/mxCellPath.js
--rw-r--r--   0 root         (0) root         (0)    12721 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/model/mxGeometry.js
--rw-r--r--   0 root         (0) root         (0)    62665 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/model/mxGraphModel.js
--rw-r--r--   0 root         (0) root         (0)    28988 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/mxClient.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.263872 XGEE-0.2.9/xgee/core/mxgraph/js/shape/
--rw-r--r--   0 root         (0) root         (0)     2117 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxActor.js
--rw-r--r--   0 root         (0) root         (0)     3316 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxArrow.js
--rw-r--r--   0 root         (0) root         (0)    11601 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxArrowConnector.js
--rw-r--r--   0 root         (0) root         (0)     1506 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxCloud.js
--rw-r--r--   0 root         (0) root         (0)     4196 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxConnector.js
--rw-r--r--   0 root         (0) root         (0)     2694 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxCylinder.js
--rw-r--r--   0 root         (0) root         (0)     2823 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxDoubleEllipse.js
--rw-r--r--   0 root         (0) root         (0)     1159 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxEllipse.js
--rw-r--r--   0 root         (0) root         (0)      802 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxHexagon.js
--rw-r--r--   0 root         (0) root         (0)     6341 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxImageShape.js
--rw-r--r--   0 root         (0) root         (0)     6800 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxLabel.js
--rw-r--r--   0 root         (0) root         (0)     1139 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxLine.js
--rw-r--r--   0 root         (0) root         (0)     5400 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxMarker.js
--rw-r--r--   0 root         (0) root         (0)     2485 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxPolyline.js
--rw-r--r--   0 root         (0) root         (0)     3068 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxRectangleShape.js
--rw-r--r--   0 root         (0) root         (0)     1597 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxRhombus.js
--rw-r--r--   0 root         (0) root         (0)    38952 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxShape.js
--rw-r--r--   0 root         (0) root         (0)    26031 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxStencil.js
--rw-r--r--   0 root         (0) root         (0)     1053 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxStencilRegistry.js
--rw-r--r--   0 root         (0) root         (0)     9507 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxSwimlane.js
--rw-r--r--   0 root         (0) root         (0)    37084 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxText.js
--rw-r--r--   0 root         (0) root         (0)      828 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxTriangle.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.274872 XGEE-0.2.9/xgee/core/mxgraph/js/util/
--rw-r--r--   0 root         (0) root         (0)    11723 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAbstractCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)     1895 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAnimation.js
--rw-r--r--   0 root         (0) root         (0)     4430 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAutoSaveManager.js
--rw-r--r--   0 root         (0) root         (0)     5354 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxClipboard.js
--rw-r--r--   0 root         (0) root         (0)    63826 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxConstants.js
--rw-r--r--   0 root         (0) root         (0)     2236 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDictionary.js
--rw-r--r--   0 root         (0) root         (0)     3205 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDivResizer.js
--rw-r--r--   0 root         (0) root         (0)    16885 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDragSource.js
--rw-r--r--   0 root         (0) root         (0)     4460 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEffects.js
--rw-r--r--   0 root         (0) root         (0)    27401 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEvent.js
--rw-r--r--   0 root         (0) root         (0)     1941 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEventObject.js
--rw-r--r--   0 root         (0) root         (0)     3778 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEventSource.js
--rw-r--r--   0 root         (0) root         (0)     4041 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxForm.js
--rw-r--r--   0 root         (0) root         (0)    10378 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxGuide.js
--rw-r--r--   0 root         (0) root         (0)      670 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImage.js
--rw-r--r--   0 root         (0) root         (0)     3380 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImageBundle.js
--rw-r--r--   0 root         (0) root         (0)     3798 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImageExport.js
--rw-r--r--   0 root         (0) root         (0)     8228 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxLog.js
--rw-r--r--   0 root         (0) root         (0)     5691 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxMorphing.js
--rw-r--r--   0 root         (0) root         (0)     4481 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxMouseEvent.js
--rw-r--r--   0 root         (0) root         (0)     1485 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxObjectIdentity.js
--rw-r--r--   0 root         (0) root         (0)     5082 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPanningManager.js
--rw-r--r--   0 root         (0) root         (0)     1039 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPoint.js
--rw-r--r--   0 root         (0) root         (0)    14045 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPopupMenu.js
--rw-r--r--   0 root         (0) root         (0)     3693 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxRectangle.js
--rw-r--r--   0 root         (0) root         (0)    11080 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxResources.js
--rw-r--r--   0 root         (0) root         (0)    45946 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxSvgCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    12132 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxToolbar.js
--rw-r--r--   0 root         (0) root         (0)     5793 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUndoManager.js
--rw-r--r--   0 root         (0) root         (0)     4535 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUndoableEdit.js
--rw-r--r--   0 root         (0) root         (0)     2768 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUrlConverter.js
--rw-r--r--   0 root         (0) root         (0)   106481 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUtils.js
--rw-r--r--   0 root         (0) root         (0)    26243 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxVmlCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    27971 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxWindow.js
--rw-r--r--   0 root         (0) root         (0)    28763 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxXmlCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    10820 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/util/mxXmlRequest.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.281873 XGEE-0.2.9/xgee/core/mxgraph/js/view/
--rw-r--r--   0 root         (0) root         (0)    35624 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellEditor.js
--rw-r--r--   0 root         (0) root         (0)     6245 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellOverlay.js
--rw-r--r--   0 root         (0) root         (0)    44101 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellRenderer.js
--rw-r--r--   0 root         (0) root         (0)     9726 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellState.js
--rw-r--r--   0 root         (0) root         (0)     4286 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellStatePreview.js
--rw-r--r--   0 root         (0) root         (0)     1649 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxConnectionConstraint.js
--rw-r--r--   0 root         (0) root         (0)    42452 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxEdgeStyle.js
--rw-r--r--   0 root         (0) root         (0)   333205 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraph.js
--rw-r--r--   0 root         (0) root         (0)     9127 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraphSelectionModel.js
--rw-r--r--   0 root         (0) root         (0)    74549 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraphView.js
--rw-r--r--   0 root         (0) root         (0)    10941 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxLayoutManager.js
--rw-r--r--   0 root         (0) root         (0)     7440 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxMultiplicity.js
--rw-r--r--   0 root         (0) root         (0)    19683 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxOutline.js
--rw-r--r--   0 root         (0) root         (0)    20530 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxPerimeter.js
--rw-r--r--   0 root         (0) root         (0)    32135 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxPrintPreview.js
--rw-r--r--   0 root         (0) root         (0)     2022 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxStyleRegistry.js
--rw-r--r--   0 root         (0) root         (0)     6753 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxStylesheet.js
--rw-r--r--   0 root         (0) root         (0)     9336 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxSwimlaneManager.js
--rw-r--r--   0 root         (0) root         (0)     2955 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/js/view/mxTemporaryCellStates.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.283873 XGEE-0.2.9/xgee/core/mxgraph/resources/
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/editor.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/editor_de.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/editor_zh.txt
--rw-r--r--   0 root         (0) root         (0)      340 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/graph.txt
--rw-r--r--   0 root         (0) root         (0)      375 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/graph_de.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/mxgraph/resources/graph_zh.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.154864 XGEE-0.2.9/xgee/core/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.284873 XGEE-0.2.9/xgee/core/plugins/autostart/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.285873 XGEE-0.2.9/xgee/core/plugins/autostart/js/
--rw-r--r--   0 root         (0) root         (0)      593 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/autostart/js/AppStartupEvent.js
--rw-r--r--   0 root         (0) root         (0)      823 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/autostart/js/AppStartupObserver.js
--rw-r--r--   0 root         (0) root         (0)     1138 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/autostart/js/Autostarter.js
--rw-r--r--   0 root         (0) root         (0)     3186 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/autostart/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.285873 XGEE-0.2.9/xgee/core/plugins/clipboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.287873 XGEE-0.2.9/xgee/core/plugins/clipboard/js/
--rw-r--r--   0 root         (0) root         (0)      969 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/AppClipboard.js
--rw-r--r--   0 root         (0) root         (0)     1279 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/Clipboard.js
--rw-r--r--   0 root         (0) root         (0)     6598 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardAPI.js
--rw-r--r--   0 root         (0) root         (0)      308 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardEvaluator.js
--rw-r--r--   0 root         (0) root         (0)      618 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js
--rw-r--r--   0 root         (0) root         (0)     3342 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardManager.js
--rw-r--r--   0 root         (0) root         (0)     3665 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js
--rw-r--r--   0 root         (0) root         (0)     4999 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/clipboard/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.288873 XGEE-0.2.9/xgee/core/plugins/contextMenu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.290873 XGEE-0.2.9/xgee/core/plugins/contextMenu/js/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu/js/ContextMenu.js
--rw-r--r--   0 root         (0) root         (0)     1768 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu/js/util.js
--rw-r--r--   0 root         (0) root         (0)     2762 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.288873 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.288873 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/css/
--rw-r--r--   0 root         (0) root         (0)      399 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/css/contextMenu.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.288873 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/js/
--rw-r--r--   0 root         (0) root         (0)      361 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/js/Filter.js
--rw-r--r--   0 root         (0) root         (0)    13387 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.289873 XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.289873 XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/js/
--rw-r--r--   0 root         (0) root         (0)     4740 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/js/util.js
--rw-r--r--   0 root         (0) root         (0)     4218 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.291874 XGEE-0.2.9/xgee/core/plugins/ecore/
--rw-r--r--   0 root         (0) root         (0)    11515 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/LICENSE
--rw-r--r--   0 root         (0) root         (0)    93760 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/ecore.xmi.js
--rw-r--r--   0 root         (0) root         (0)      456 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.294874 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/
--rw-r--r--   0 root         (0) root         (0)       57 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/.gitignore
--rw-r--r--   0 root         (0) root         (0)      145 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/.travis.yml
--rw-r--r--   0 root         (0) root         (0)      366 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/AUTHORS
--rw-r--r--   0 root         (0) root         (0)      280 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     2011 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8381 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.297874 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/
--rw-r--r--   0 root         (0) root         (0)   181013 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml
--rw-r--r--   0 root         (0) root         (0)      790 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/example.js
--rw-r--r--   0 root         (0) root         (0)     1539 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js
--rw-r--r--   0 root         (0) root         (0)      164 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/hello-world.js
--rw-r--r--   0 root         (0) root         (0)      181 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/not-pretty.xml
--rw-r--r--   0 root         (0) root         (0)     1506 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js
--rw-r--r--   0 root         (0) root         (0)    99650 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml
--rw-r--r--   0 root         (0) root         (0)      138 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/test.html
--rw-r--r--   0 root         (0) root         (0)    51402 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/test.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.297874 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/lib/
--rw-r--r--   0 root         (0) root         (0)    43541 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/lib/sax.js
--rw-r--r--   0 root         (0) root         (0)    85352 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/package-lock.json
--rw-r--r--   0 root         (0) root         (0)      655 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.314875 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/
--rw-r--r--   0 root         (0) root         (0)      763 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js
--rw-r--r--   0 root         (0) root         (0)     2426 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js
--rw-r--r--   0 root         (0) root         (0)      719 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js
--rw-r--r--   0 root         (0) root         (0)     1478 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/bom.js
--rw-r--r--   0 root         (0) root         (0)     1047 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js
--rw-r--r--   0 root         (0) root         (0)     1557 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/case.js
--rw-r--r--   0 root         (0) root         (0)      389 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-chunked.js
--rw-r--r--   0 root         (0) root         (0)      363 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-end-split.js
--rw-r--r--   0 root         (0) root         (0)      782 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js
--rw-r--r--   0 root         (0) root         (0)      514 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js
--rw-r--r--   0 root         (0) root         (0)      362 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata.js
--rw-r--r--   0 root         (0) root         (0)      247 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cyrillic.js
--rw-r--r--   0 root         (0) root         (0)      383 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/duplicate-attribute.js
--rw-r--r--   0 root         (0) root         (0)      343 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/emoji.js
--rw-r--r--   0 root         (0) root         (0)      130 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/end_empty_stream.js
--rw-r--r--   0 root         (0) root         (0)      368 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/entities.js
--rw-r--r--   0 root         (0) root         (0)      372 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/entity-mega.js
--rw-r--r--   0 root         (0) root         (0)      238 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/entity-nan.js
--rw-r--r--   0 root         (0) root         (0)      329 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/flush.js
--rw-r--r--   0 root         (0) root         (0)     1311 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/index.js
--rw-r--r--   0 root         (0) root         (0)     1912 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js
--rw-r--r--   0 root         (0) root         (0)      691 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js
--rw-r--r--   0 root         (0) root         (0)      336 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-35.js
--rw-r--r--   0 root         (0) root         (0)      398 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-47.js
--rw-r--r--   0 root         (0) root         (0)     1155 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js
--rw-r--r--   0 root         (0) root         (0)      467 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-84.js
--rw-r--r--   0 root         (0) root         (0)     1196 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js
--rw-r--r--   0 root         (0) root         (0)      240 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/not-string.js
--rw-r--r--   0 root         (0) root         (0)     1300 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js
--rw-r--r--   0 root         (0) root         (0)      952 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js
--rw-r--r--   0 root         (0) root         (0)      637 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js
--rw-r--r--   0 root         (0) root         (0)     1035 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/script.js
--rw-r--r--   0 root         (0) root         (0)     1072 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js
--rw-r--r--   0 root         (0) root         (0)      904 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js
--rw-r--r--   0 root         (0) root         (0)      217 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/stand-alone-comment.js
--rw-r--r--   0 root         (0) root         (0)      755 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js
--rw-r--r--   0 root         (0) root         (0)      288 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/trailing-attribute-no-value.js
--rw-r--r--   0 root         (0) root         (0)      407 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/trailing-non-whitespace.js
--rw-r--r--   0 root         (0) root         (0)      387 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/unclosed-root.js
--rw-r--r--   0 root         (0) root         (0)      727 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js
--rw-r--r--   0 root         (0) root         (0)     1009 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js
--rw-r--r--   0 root         (0) root         (0)     1846 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js
--rw-r--r--   0 root         (0) root         (0)      429 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xml_entities.js
--rw-r--r--   0 root         (0) root         (0)      465 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-as-tag-name.js
--rw-r--r--   0 root         (0) root         (0)     1668 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js
--rw-r--r--   0 root         (0) root         (0)     5497 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js
--rw-r--r--   0 root         (0) root         (0)     5577 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js
--rw-r--r--   0 root         (0) root         (0)     1805 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js
--rw-r--r--   0 root         (0) root         (0)      947 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js
--rw-r--r--   0 root         (0) root         (0)     1070 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js
--rw-r--r--   0 root         (0) root         (0)      871 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js
--rw-r--r--   0 root         (0) root         (0)      509 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix.js
--rw-r--r--   0 root         (0) root         (0)     1096 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.128863 XGEE-0.2.9/xgee/core/plugins/ecoreDebuggerUi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.314875 XGEE-0.2.9/xgee/core/plugins/ecoreDebuggerUi/js/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreDebuggerUi/js/ecoreDebuggerUiController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.316875 XGEE-0.2.9/xgee/core/plugins/ecoreSync/
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-14 18:02:14.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/.git
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.322876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/changes/
--rw-r--r--   0 root         (0) root         (0)    10675 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/changes/esChanges.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.322876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/
--rw-r--r--   0 root         (0) root         (0)     5919 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/esDebugging.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.323876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/lib/
--rw-r--r--   0 root         (0) root         (0)     4918 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/lib/libesync.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.325876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/
--rw-r--r--   0 root         (0) root         (0)     1484 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esDomain.js
--rw-r--r--   0 root         (0) root         (0)      378 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esErrors.js
--rw-r--r--   0 root         (0) root         (0)     3129 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esLookup.js
--rw-r--r--   0 root         (0) root         (0)    13249 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esMetaSync.js
--rw-r--r--   0 root         (0) root         (0)    20548 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js
--rw-r--r--   0 root         (0) root         (0)     1570 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js
--rw-r--r--   0 root         (0) root         (0)     1901 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/ecoreSync.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.325876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/interfaces/
--rw-r--r--   0 root         (0) root         (0)     2956 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/interfaces/esInstance.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.327876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/
--rw-r--r--   0 root         (0) root         (0)    10832 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js
--rw-r--r--   0 root         (0) root         (0)     9168 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js
--rw-r--r--   0 root         (0) root         (0)     9420 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js
--rw-r--r--   0 root         (0) root         (0)     2183 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js
--rw-r--r--   0 root         (0) root         (0)     1834 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.329876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/
--rw-r--r--   0 root         (0) root         (0)    20117 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js
--rw-r--r--   0 root         (0) root         (0)     1851 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueries.js
--rw-r--r--   0 root         (0) root         (0)    36223 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js
--rw-r--r--   0 root         (0) root         (0)    25761 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js
--rw-r--r--   0 root         (0) root         (0)     2491 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js
--rw-r--r--   0 root         (0) root         (0)     4045 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.330876 XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/
--rw-r--r--   0 root         (0) root         (0)      966 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/auxiliaries.js
--rw-r--r--   0 root         (0) root         (0)       50 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/esLogging.js
--rw-r--r--   0 root         (0) root         (0)    14957 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/esUtils.js
--rw-r--r--   0 root         (0) root         (0)     1194 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/uuid.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.316875 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.316875 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/css/
--rw-r--r--   0 root         (0) root         (0)     5694 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.321875 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/
--rw-r--r--   0 root         (0) root         (0)     3076 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg
--rw-r--r--   0 root         (0) root         (0)     2651 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg
--rw-r--r--   0 root         (0) root         (0)     4500 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg
--rw-r--r--   0 root         (0) root         (0)     4471 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg
--rw-r--r--   0 root         (0) root         (0)     2553 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg
--rw-r--r--   0 root         (0) root         (0)     3529 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg
--rw-r--r--   0 root         (0) root         (0)     3500 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg
--rw-r--r--   0 root         (0) root         (0)     5270 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg
--rw-r--r--   0 root         (0) root         (0)     5138 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg
--rw-r--r--   0 root         (0) root         (0)     2381 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.322876 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/
--rw-r--r--   0 root         (0) root         (0)     8088 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js
--rw-r--r--   0 root         (0) root         (0)     5394 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js
--rw-r--r--   0 root         (0) root         (0)    48201 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js
--rw-r--r--   0 root         (0) root         (0)      760 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.330876 XGEE-0.2.9/xgee/core/plugins/editor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.132863 XGEE-0.2.9/xgee/core/plugins/editor/controllers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.333876 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/
--rw-r--r--   0 root         (0) root         (0)      970 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/AnchorController.js
--rw-r--r--   0 root         (0) root         (0)      972 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/ContainerController.js
--rw-r--r--   0 root         (0) root         (0)     2337 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/EdgeController.js
--rw-r--r--   0 root         (0) root         (0)    15589 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/GraphController.js
--rw-r--r--   0 root         (0) root         (0)     7060 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js
--rw-r--r--   0 root         (0) root         (0)      275 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/GraphObjectController.js
--rw-r--r--   0 root         (0) root         (0)      976 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/LabelController.js
--rw-r--r--   0 root         (0) root         (0)      978 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/QueryController.js
--rw-r--r--   0 root         (0) root         (0)     5353 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/VertexController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.334876 XGEE-0.2.9/xgee/core/plugins/editor/controllers/palette/
--rw-r--r--   0 root         (0) root         (0)     1245 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/controllers/palette/PaletteController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.334876 XGEE-0.2.9/xgee/core/plugins/editor/css/
--rw-r--r--   0 root         (0) root         (0)      547 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/css/loading.css
--rw-r--r--   0 root         (0) root         (0)      115 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/css/xgeeJsaIntegration.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.335876 XGEE-0.2.9/xgee/core/plugins/editor/extensions/
--rw-r--r--   0 root         (0) root         (0)     2473 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.335876 XGEE-0.2.9/xgee/core/plugins/editor/graph/
--rw-r--r--   0 root         (0) root         (0)     1383 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/graph/GraphResourceProvider.js
--rw-r--r--   0 root         (0) root         (0)     6693 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/graph/mxGraphIntegration.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.336876 XGEE-0.2.9/xgee/core/plugins/editor/interactions/
--rw-r--r--   0 root         (0) root         (0)     3785 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/interactions/DropReception.js
--rw-r--r--   0 root         (0) root         (0)     1042 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/interactions/GraphInteraction.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.337876 XGEE-0.2.9/xgee/core/plugins/editor/lib/
--rw-r--r--   0 root         (0) root         (0)    10080 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/lib/libapi.js
--rw-r--r--   0 root         (0) root         (0)     9750 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/lib/libaux.js
--rw-r--r--   0 root         (0) root         (0)    20059 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/lib/libjsa.js
--rw-r--r--   0 root         (0) root         (0)     1194 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/lib/uuid.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.338877 XGEE-0.2.9/xgee/core/plugins/editor/model/
--rw-r--r--   0 root         (0) root         (0)      339 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/PresentationModel.js
--rw-r--r--   0 root         (0) root         (0)    83708 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/editorModel.ecore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.352877 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Anchor.js
--rw-r--r--   0 root         (0) root         (0)     3246 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/AnchorManager.js
--rw-r--r--   0 root         (0) root         (0)      449 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/AnchorType.js
--rw-r--r--   0 root         (0) root         (0)     2305 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Container.js
--rw-r--r--   0 root         (0) root         (0)     1896 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerManager.js
--rw-r--r--   0 root         (0) root         (0)      608 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerProvider.js
--rw-r--r--   0 root         (0) root         (0)     1760 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerType.js
--rw-r--r--   0 root         (0) root         (0)     1037 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/DeletableObject.js
--rw-r--r--   0 root         (0) root         (0)      266 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EObjectOwner.js
--rw-r--r--   0 root         (0) root         (0)    10305 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Edge.js
--rw-r--r--   0 root         (0) root         (0)     1264 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EdgeContainer.js
--rw-r--r--   0 root         (0) root         (0)     6994 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EdgeManager.js
--rw-r--r--   0 root         (0) root         (0)      383 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EdgeType.js
--rw-r--r--   0 root         (0) root         (0)      566 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EventProvider.js
--rw-r--r--   0 root         (0) root         (0)      346 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/FloatingLabel.js
--rw-r--r--   0 root         (0) root         (0)     1013 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphEvent.js
--rw-r--r--   0 root         (0) root         (0)    27515 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js
--rw-r--r--   0 root         (0) root         (0)     6623 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModel.js
--rw-r--r--   0 root         (0) root         (0)    12643 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModelFactory.js
--rw-r--r--   0 root         (0) root         (0)     4145 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModelManager.js
--rw-r--r--   0 root         (0) root         (0)      553 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphObject.js
--rw-r--r--   0 root         (0) root         (0)     2097 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphObjectManager.js
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphObjectType.js
--rw-r--r--   0 root         (0) root         (0)     2200 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Label.js
--rw-r--r--   0 root         (0) root         (0)     1990 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelManager.js
--rw-r--r--   0 root         (0) root         (0)      478 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelProvider.js
--rw-r--r--   0 root         (0) root         (0)     2061 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelSegment.js
--rw-r--r--   0 root         (0) root         (0)     6090 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js
--rw-r--r--   0 root         (0) root         (0)      419 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelSegmentType.js
--rw-r--r--   0 root         (0) root         (0)      386 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelType.js
--rw-r--r--   0 root         (0) root         (0)      932 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LocatableObject.js
--rw-r--r--   0 root         (0) root         (0)      615 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/NestedLabel.js
--rw-r--r--   0 root         (0) root         (0)      464 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/RoutableObject.js
--rw-r--r--   0 root         (0) root         (0)     1527 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/SizableObject.js
--rw-r--r--   0 root         (0) root         (0)     2346 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertex.js
--rw-r--r--   0 root         (0) root         (0)     7913 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertexManager.js
--rw-r--r--   0 root         (0) root         (0)     1684 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertexType.js
--rw-r--r--   0 root         (0) root         (0)      546 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/TransactionObject.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/TypedObject.js
--rw-r--r--   0 root         (0) root         (0)     3517 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Vertex.js
--rw-r--r--   0 root         (0) root         (0)    12233 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexContainer.js
--rw-r--r--   0 root         (0) root         (0)    12045 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexManager.js
--rw-r--r--   0 root         (0) root         (0)     1682 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexType.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.353878 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/DragAndDropTool.js
--rw-r--r--   0 root         (0) root         (0)    15745 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js
--rw-r--r--   0 root         (0) root         (0)     3656 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/GraphTool.js
--rw-r--r--   0 root         (0) root         (0)     8885 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/PaletteModel.js
--rw-r--r--   0 root         (0) root         (0)     3844 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/SelectionTool.js
--rw-r--r--   0 root         (0) root         (0)     8885 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/model/palette/ToolGenerator.js
--rw-r--r--   0 root         (0) root         (0)     5667 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.354878 XGEE-0.2.9/xgee/core/plugins/editor/queries/
--rw-r--r--   0 root         (0) root         (0)     6432 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/queries/Query.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.356878 XGEE-0.2.9/xgee/core/plugins/editor/view/
--rw-r--r--   0 root         (0) root         (0)    55157 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/view/GraphView.js
--rw-r--r--   0 root         (0) root         (0)     1725 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/view/GraphViewMenu.js
--rw-r--r--   0 root         (0) root         (0)    22370 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/view/GraphViewPort.js
--rw-r--r--   0 root         (0) root         (0)     3483 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/view/PaletteView.js
--rw-r--r--   0 root         (0) root         (0)     5888 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/editor/view/ScreenshotExport.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.356878 XGEE-0.2.9/xgee/core/plugins/eoq.actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.356878 XGEE-0.2.9/xgee/core/plugins/eoq.actions/css/
--rw-r--r--   0 root         (0) root         (0)     2193 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eoq.actions/css/ActionsUi.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.357878 XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/
--rw-r--r--   0 root         (0) root         (0)     5233 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsController.js
--rw-r--r--   0 root         (0) root         (0)    14088 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsCore.js
--rw-r--r--   0 root         (0) root         (0)    23053 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsUi.js
--rw-r--r--   0 root         (0) root         (0)     1541 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eoq.actions/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.360878 XGEE-0.2.9/xgee/core/plugins/eoq1/
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/.git
--rw-r--r--   0 root         (0) root         (0)     1160 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1077 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/README.md
--rw-r--r--   0 root         (0) root         (0)    11898 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/commandparser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.361878 XGEE-0.2.9/xgee/core/plugins/eoq1/domains/
--rw-r--r--   0 root         (0) root         (0)     5897 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/domains/bufferingdomain.js
--rw-r--r--   0 root         (0) root         (0)      879 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/domains/domain.js
--rw-r--r--   0 root         (0) root         (0)     4364 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/domains/httppostdomain.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.361878 XGEE-0.2.9/xgee/core/plugins/eoq1/model/
--rw-r--r--   0 root         (0) root         (0)    37451 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/model/model.js
--rw-r--r--   0 root         (0) root         (0)      468 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/package.json
--rw-r--r--   0 root         (0) root         (0)      504 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/plugin.js
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/queryparser.js
--rw-r--r--   0 root         (0) root         (0)    11900 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/resultparser.js
--rw-r--r--   0 root         (0) root         (0)    12168 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq1/valueparser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.363878 XGEE-0.2.9/xgee/core/plugins/eoq2/
--rw-r--r--   0 root         (0) root         (0)       64 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/.git
--rw-r--r--   0 root         (0) root         (0)     1160 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      925 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.364878 XGEE-0.2.9/xgee/core/plugins/eoq2/action/
--rw-r--r--   0 root         (0) root         (0)      579 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/action/call.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.364878 XGEE-0.2.9/xgee/core/plugins/eoq2/command/
--rw-r--r--   0 root         (0) root         (0)    12287 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/command/command.js
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/command/result.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.364878 XGEE-0.2.9/xgee/core/plugins/eoq2/domain/
--rw-r--r--   0 root         (0) root         (0)      983 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/domain/domain.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.365878 XGEE-0.2.9/xgee/core/plugins/eoq2/domain/remote/
--rw-r--r--   0 root         (0) root         (0)     2267 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js
--rw-r--r--   0 root         (0) root         (0)     5812 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js
--rw-r--r--   0 root         (0) root         (0)     4806 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/eoq2.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.365878 XGEE-0.2.9/xgee/core/plugins/eoq2/event/
--rw-r--r--   0 root         (0) root         (0)     3879 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/event/event.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.366878 XGEE-0.2.9/xgee/core/plugins/eoq2/frame/
--rw-r--r--   0 root         (0) root         (0)      567 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/frame/frame.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.366878 XGEE-0.2.9/xgee/core/plugins/eoq2/legacy/
--rw-r--r--   0 root         (0) root         (0)    14240 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/legacy/legacy.js
--rw-r--r--   0 root         (0) root         (0)      440 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/package.json
--rw-r--r--   0 root         (0) root         (0)     2472 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.366878 XGEE-0.2.9/xgee/core/plugins/eoq2/query/
--rw-r--r--   0 root         (0) root         (0)    14393 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/query/query.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.367879 XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/
--rw-r--r--   0 root         (0) root         (0)      837 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/jsonserializer.js
--rw-r--r--   0 root         (0) root         (0)      725 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/serializer.js
--rw-r--r--   0 root         (0) root         (0)    40363 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/textserializer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.368879 XGEE-0.2.9/xgee/core/plugins/eoq2/util/
--rw-r--r--   0 root         (0) root         (0)     2823 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/core/plugins/eoq2/util/logger.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.369879 XGEE-0.2.9/xgee/core/plugins/eventBroker/
--rw-r--r--   0 root         (0) root         (0)      506 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eventBroker/BasicEvent.js
--rw-r--r--   0 root         (0) root         (0)      506 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eventBroker/QueryDebugEvent.js
--rw-r--r--   0 root         (0) root         (0)      694 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eventBroker/SelectionChangedEvent.js
--rw-r--r--   0 root         (0) root         (0)     3823 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/eventBroker/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.369879 XGEE-0.2.9/xgee/core/plugins/iconProvider/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.370879 XGEE-0.2.9/xgee/core/plugins/iconProvider/js/
--rw-r--r--   0 root         (0) root         (0)      387 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/iconProvider/js/IconProvider.js
--rw-r--r--   0 root         (0) root         (0)     2394 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/iconProvider/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.370879 XGEE-0.2.9/xgee/core/plugins/keyHandler/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.371879 XGEE-0.2.9/xgee/core/plugins/keyHandler/js/
--rw-r--r--   0 root         (0) root         (0)     1493 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/keyHandler/js/KeyHandler.js
--rw-r--r--   0 root         (0) root         (0)      391 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/keyHandler/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.370879 XGEE-0.2.9/xgee/core/plugins/keyHandler.ecore/
--rw-r--r--   0 root         (0) root         (0)      720 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/keyHandler.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.371879 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.374879 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.376879 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/
--rw-r--r--   0 root         (0) root         (0)     3528 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot
--rw-r--r--   0 root         (0) root         (0)     3320 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
--rw-r--r--   0 root         (0) root         (0)     2180 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1680 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
--rw-r--r--   0 root         (0) root         (0)     7278 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css
--rw-r--r--   0 root         (0) root         (0)    91213 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js
--rw-r--r--   0 root         (0) root         (0)     5991 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
--rw-r--r--   0 root         (0) root         (0)    14532 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
--rw-r--r--   0 root         (0) root         (0)    27807 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
--rw-r--r--   0 root         (0) root         (0)   131140 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
--rw-r--r--   0 root         (0) root         (0)    22405 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js
--rw-r--r--   0 root         (0) root         (0)     5855 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js
--rw-r--r--   0 root         (0) root         (0)      669 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.376879 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.388880 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/
--rw-r--r--   0 root         (0) root         (0)      554 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif
--rw-r--r--   0 root         (0) root         (0)      123 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAttribute.gif
--rw-r--r--   0 root         (0) root         (0)      206 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EClass.gif
--rw-r--r--   0 root         (0) root         (0)      199 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EDataType.gif
--rw-r--r--   0 root         (0) root         (0)      131 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnum.gif
--rw-r--r--   0 root         (0) root         (0)      109 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnumLiteral.gif
--rw-r--r--   0 root         (0) root         (0)      211 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EFactory.gif
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericElementType.gif
--rw-r--r--   0 root         (0) root         (0)      108 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericException.gif
--rw-r--r--   0 root         (0) root         (0)      139 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericSuperType.gif
--rw-r--r--   0 root         (0) root         (0)       99 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericType.gif
--rw-r--r--   0 root         (0) root         (0)      139 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericTypeArgument.gif
--rw-r--r--   0 root         (0) root         (0)      111 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericWildcard.gif
--rw-r--r--   0 root         (0) root         (0)      323 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EObject.gif
--rw-r--r--   0 root         (0) root         (0)       62 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceN.gif
--rw-r--r--   0 root         (0) root         (0)       71 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToM.gif
--rw-r--r--   0 root         (0) root         (0)       81 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      131 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)       58 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOne.gif
--rw-r--r--   0 root         (0) root         (0)       68 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToN.gif
--rw-r--r--   0 root         (0) root         (0)       79 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      128 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)       70 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZero.gif
--rw-r--r--   0 root         (0) root         (0)       78 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToN.gif
--rw-r--r--   0 root         (0) root         (0)       77 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToOne.gif
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      133 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)      141 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOperation.gif
--rw-r--r--   0 root         (0) root         (0)      207 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EPackage.gif
--rw-r--r--   0 root         (0) root         (0)      911 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif
--rw-r--r--   0 root         (0) root         (0)      183 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EReference.gif
--rw-r--r--   0 root         (0) root         (0)      213 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EStringToStringMapEntry.gif
--rw-r--r--   0 root         (0) root         (0)      211 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/ETypeParameter.gif
--rw-r--r--   0 root         (0) root         (0)      554 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif
--rw-r--r--   0 root         (0) root         (0)      206 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eClassifiers.gif
--rw-r--r--   0 root         (0) root         (0)      141 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eOperations.gif
--rw-r--r--   0 root         (0) root         (0)      207 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eSubpackages.gif
--rw-r--r--   0 root         (0) root         (0)      211 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eTypeParameters.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.388880 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/js/
--rw-r--r--   0 root         (0) root         (0)      577 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js
--rw-r--r--   0 root         (0) root         (0)    29666 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.376879 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView.eoq/
--rw-r--r--   0 root         (0) root         (0)    16933 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.390880 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   128443 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js
--rw-r--r--   0 root         (0) root         (0)   162267 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map
--rw-r--r--   0 root         (0) root         (0)      562 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.392880 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/
--rw-r--r--   0 root         (0) root         (0)     5513 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif
--rw-r--r--   0 root         (0) root         (0)     5510 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif
--rw-r--r--   0 root         (0) root         (0)     3234 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif
--rw-r--r--   0 root         (0) root         (0)    24749 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css
--rw-r--r--   0 root         (0) root         (0)     4818 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less
--rw-r--r--   0 root         (0) root         (0)      852 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif
--rw-r--r--   0 root         (0) root         (0)      852 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.393880 XGEE-0.2.9/xgee/core/plugins/propertiesView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.399881 XGEE-0.2.9/xgee/core/plugins/propertiesView/css/
--rw-r--r--   0 root         (0) root         (0)      961 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/css/PropertiesView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.400881 XGEE-0.2.9/xgee/core/plugins/propertiesView/doc/
--rw-r--r--   0 root         (0) root         (0)    38735 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.401881 XGEE-0.2.9/xgee/core/plugins/propertiesView/js/
--rw-r--r--   0 root         (0) root         (0)     1641 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js
--rw-r--r--   0 root         (0) root         (0)      298 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/js/PropertiesBubble.js
--rw-r--r--   0 root         (0) root         (0)      779 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     7532 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/js/PropertiesViewController.js
--rw-r--r--   0 root         (0) root         (0)     1795 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.393880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.398881 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/js/
--rw-r--r--   0 root         (0) root         (0)    10124 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     1682 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1173 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.393880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.394880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/
--rw-r--r--   0 root         (0) root         (0)     7014 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     1163 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js
--rw-r--r--   0 root         (0) root         (0)     2739 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)      878 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.395880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.395880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/css/
--rw-r--r--   0 root         (0) root         (0)      458 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/css/EcoreEditorsPropertiesPane.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.396880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/js/
--rw-r--r--   0 root         (0) root         (0)     1565 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     2170 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1297 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.396880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.396880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/css/
--rw-r--r--   0 root         (0) root         (0)      458 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/css/EcoreModifyPropertiesPane.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.397880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/js/
--rw-r--r--   0 root         (0) root         (0)     2571 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     2157 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1287 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.397880 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.398881 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/js/
--rw-r--r--   0 root         (0) root         (0)     1281 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js
--rw-r--r--   0 root         (0) root         (0)     1263 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.399881 XGEE-0.2.9/xgee/core/plugins/propertiesView.info/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.399881 XGEE-0.2.9/xgee/core/plugins/propertiesView.info/js/
--rw-r--r--   0 root         (0) root         (0)     3609 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)      984 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/propertiesView.info/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.401881 XGEE-0.2.9/xgee/core/plugins/tool.goToView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.402881 XGEE-0.2.9/xgee/core/plugins/tool.goToView/css/
--rw-r--r--   0 root         (0) root         (0)      126 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.goToView/css/GoToViewTool.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.402881 XGEE-0.2.9/xgee/core/plugins/tool.goToView/img/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.402881 XGEE-0.2.9/xgee/core/plugins/tool.goToView/js/
--rw-r--r--   0 root         (0) root         (0)     2805 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.goToView/js/GoToViewTool.js
--rw-r--r--   0 root         (0) root         (0)     1018 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1262 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.goToView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.403881 XGEE-0.2.9/xgee/core/plugins/tool.notes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.403881 XGEE-0.2.9/xgee/core/plugins/tool.notes/css/
--rw-r--r--   0 root         (0) root         (0)     4415 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/css/NotesTool.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.405881 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-error.svg
--rw-r--r--   0 root         (0) root         (0)     2197 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-info.svg
--rw-r--r--   0 root         (0) root         (0)     2085 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-success.svg
--rw-r--r--   0 root         (0) root         (0)     3188 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-warning.svg
--rw-r--r--   0 root         (0) root         (0)     2173 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/img/tool-notes.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.405881 XGEE-0.2.9/xgee/core/plugins/tool.notes/js/
--rw-r--r--   0 root         (0) root         (0)     6924 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/js/NotesTool.js
--rw-r--r--   0 root         (0) root         (0)      940 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/js/NotesToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1076 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tool.notes/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.406881 XGEE-0.2.9/xgee/core/plugins/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.406881 XGEE-0.2.9/xgee/core/plugins/tools/js/
--rw-r--r--   0 root         (0) root         (0)      364 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tools/js/ToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tools/js/ToolsController.js
--rw-r--r--   0 root         (0) root         (0)     1268 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/tools/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.407881 XGEE-0.2.9/xgee/core/plugins/view.dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.412881 XGEE-0.2.9/xgee/core/plugins/view.dashboard/css/
--rw-r--r--   0 root         (0) root         (0)      149 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard/css/DashboardView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.412881 XGEE-0.2.9/xgee/core/plugins/view.dashboard/img/
--rw-r--r--   0 root         (0) root         (0)     2146 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard/img/view-dashboard.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.413882 XGEE-0.2.9/xgee/core/plugins/view.dashboard/js/
--rw-r--r--   0 root         (0) root         (0)      479 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard/js/DashProvider.js
--rw-r--r--   0 root         (0) root         (0)     3522 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     2285 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.407881 XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.407881 XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/js/
--rw-r--r--   0 root         (0) root         (0)     1123 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js
--rw-r--r--   0 root         (0) root         (0)     1659 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.408881 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.408881 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/css/
--rw-r--r--   0 root         (0) root         (0)     1506 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.410881 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/
--rw-r--r--   0 root         (0) root         (0)     3787 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg
--rw-r--r--   0 root         (0) root         (0)     2220 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg
--rw-r--r--   0 root         (0) root         (0)     2936 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg
--rw-r--r--   0 root         (0) root         (0)     3277 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg
--rw-r--r--   0 root         (0) root         (0)     2181 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg
--rw-r--r--   0 root         (0) root         (0)     2403 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg
--rw-r--r--   0 root         (0) root         (0)     2522 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.411882 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/
--rw-r--r--   0 root         (0) root         (0)    24067 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js
--rw-r--r--   0 root         (0) root         (0)     5322 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js
--rw-r--r--   0 root         (0) root         (0)     2123 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js
--rw-r--r--   0 root         (0) root         (0)     2212 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.413882 XGEE-0.2.9/xgee/core/plugins/view.workspace/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.413882 XGEE-0.2.9/xgee/core/plugins/view.workspace/css/
--rw-r--r--   0 root         (0) root         (0)      176 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.workspace/css/WorkspaceView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.414882 XGEE-0.2.9/xgee/core/plugins/view.workspace/img/
--rw-r--r--   0 root         (0) root         (0)     2511 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.workspace/img/view-workspace.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.414882 XGEE-0.2.9/xgee/core/plugins/view.workspace/js/
--rw-r--r--   0 root         (0) root         (0)     2417 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     1766 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/view.workspace/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.414882 XGEE-0.2.9/xgee/core/plugins/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.415882 XGEE-0.2.9/xgee/core/plugins/views/js/
--rw-r--r--   0 root         (0) root         (0)      435 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/views/js/ViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     1886 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/views/js/ViewsController.js
--rw-r--r--   0 root         (0) root         (0)     1423 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/views/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.415882 XGEE-0.2.9/xgee/core/plugins/viewsMenu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.416882 XGEE-0.2.9/xgee/core/plugins/viewsMenu/js/
--rw-r--r--   0 root         (0) root         (0)     5303 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js
--rw-r--r--   0 root         (0) root         (0)     1290 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/viewsMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.416882 XGEE-0.2.9/xgee/core/plugins/viewsTabbar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.416882 XGEE-0.2.9/xgee/core/plugins/viewsTabbar/css/
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css
--rw-r--r--   0 root         (0) root         (0)     1919 2023-01-14 18:02:12.000000 XGEE-0.2.9/xgee/core/plugins/viewsTabbar/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.417882 XGEE-0.2.9/xgee/eoqserver/
--rw-r--r--   0 root         (0) root         (0)    13048 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/eoqserver/PyEoq2WebServer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-14 18:02:15.000000 XGEE-0.2.9/xgee/eoqserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.418882 XGEE-0.2.9/xgee/eoqserver/eoq1/
--rw-r--r--   0 root         (0) root         (0)      182 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.419882 XGEE-0.2.9/xgee/eoqserver/eoq1/actions/
--rw-r--r--   0 root         (0) root         (0)      119 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/actions/actionutils.py
--rw-r--r--   0 root         (0) root         (0)    29323 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/actions/externalactionhandler.py
--rw-r--r--   0 root         (0) root         (0)     9347 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/commandparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.422882 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/
--rw-r--r--   0 root         (0) root         (0)      283 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72154 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/localdomain.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/remotehttpdomain.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.422882 XGEE-0.2.9/xgee/eoqserver/eoq1/error/
--rw-r--r--   0 root         (0) root         (0)      248 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/error/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/error/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.423882 XGEE-0.2.9/xgee/eoqserver/eoq1/model/
--rw-r--r--   0 root         (0) root         (0)     7459 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64472 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/model/model.py
--rw-r--r--   0 root         (0) root         (0)    22749 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/queryparser.py
--rw-r--r--   0 root         (0) root         (0)     8387 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/resultparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.424882 XGEE-0.2.9/xgee/eoqserver/eoq1/utils/
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25693 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/utils/csvconnector.py
--rw-r--r--   0 root         (0) root         (0)    10694 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq1/valueparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.424882 XGEE-0.2.9/xgee/eoqserver/eoq2/
--rw-r--r--   0 root         (0) root         (0)      117 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.426882 XGEE-0.2.9/xgee/eoqserver/eoq2/action/
--rw-r--r--   0 root         (0) root         (0)      142 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/__init__.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/action.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/call.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/callhandler.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/callmanager.py
--rw-r--r--   0 root         (0) root         (0)     8117 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.427883 XGEE-0.2.9/xgee/eoqserver/eoq2/action/externalpy/
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/externalpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24055 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/action/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.429883 XGEE-0.2.9/xgee/eoqserver/eoq2/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9319 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/command/command.py
--rw-r--r--   0 root         (0) root         (0)    64224 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/command/commandrunner.py
--rw-r--r--   0 root         (0) root         (0)    43028 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/command/diff.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/command/result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.430883 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/
--rw-r--r--   0 root         (0) root         (0)       60 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.430883 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/local/
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/local/__init__.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.431883 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/
--rw-r--r--   0 root         (0) root         (0)       86 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.432883 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/remote/
--rw-r--r--   0 root         (0) root         (0)       30 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/remote/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6884 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.433883 XGEE-0.2.9/xgee/eoqserver/eoq2/event/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/event/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.434883 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/
--rw-r--r--   0 root         (0) root         (0)      127 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/domainframehandler.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/frame.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/framehandler.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/frame/multiversionframehandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.435883 XGEE-0.2.9/xgee/eoqserver/eoq2/legacy/
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12199 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/legacy/legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.436883 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/
--rw-r--r--   0 root         (0) root         (0)       99 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/mdb.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/mdbaccessor.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/nocodec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.439883 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/
--rw-r--r--   0 root         (0) root         (0)      213 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.440883 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/
--rw-r--r--   0 root         (0) root         (0)      867 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py
--rw-r--r--   0 root         (0) root         (0)    36345 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
--rw-r--r--   0 root         (0) root         (0)     3823 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
--rw-r--r--   0 root         (0) root         (0)    80843 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.441883 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5277 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.441883 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/valuecodec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.442884 XGEE-0.2.9/xgee/eoqserver/eoq2/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12347 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/query/query.py
--rw-r--r--   0 root         (0) root         (0)    38368 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/query/queryrunner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.444884 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/
--rw-r--r--   0 root         (0) root         (0)      204 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/jsonserializer.py
--rw-r--r--   0 root         (0) root         (0)     6755 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/jsserializer.py
--rw-r--r--   0 root         (0) root         (0)     5871 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/pyserializer.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/serializer.py
--rw-r--r--   0 root         (0) root         (0)    35630 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/textserializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.447884 XGEE-0.2.9/xgee/eoqserver/eoq2/util/
--rw-r--r--   0 root         (0) root         (0)      118 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/backup.py
--rw-r--r--   0 root         (0) root         (0)     4033 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/benchmark.py
--rw-r--r--   0 root         (0) root         (0)    13851 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/csvconnector.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/error.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/logger.py
--rw-r--r--   0 root         (0) root         (0)     2634 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/model.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-01-14 18:02:17.000000 XGEE-0.2.9/xgee/eoqserver/eoq2/util/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:02:18.447884 XGEE-0.2.9/xgee/meta/
--rw-rw-rw-   0 root         (0) root         (0)     7875 2023-01-14 18:02:09.000000 XGEE-0.2.9/xgee/meta/layout.ecore
--rw-rw-rw-   0 root         (0) root         (0)    10705 2023-01-14 18:02:09.000000 XGEE-0.2.9/xgee/xgee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.387591 XGEE-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-06-27 10:09:43.000000 XGEE-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-27 10:09:50.387591 XGEE-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-06-27 10:09:43.000000 XGEE-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.226595 XGEE-0.3.0/XGEE.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43015 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-27 10:09:50.000000 XGEE-0.3.0/XGEE.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 10:09:50.387591 XGEE-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-06-27 10:09:43.000000 XGEE-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.226595 XGEE-0.3.0/xgee/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 10:09:43.000000 XGEE-0.3.0/xgee/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-27 10:09:43.000000 XGEE-0.3.0/xgee/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.227595 XGEE-0.3.0/xgee/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/.git
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.209596 XGEE-0.3.0/xgee/core/dep/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.228595 XGEE-0.3.0/xgee/core/dep/bluebird/
+-rw-r--r--   0 root         (0) root         (0)   183390 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/bluebird/bluebird.js
+-rw-r--r--   0 root         (0) root         (0)    81530 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/bluebird/bluebird.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.228595 XGEE-0.3.0/xgee/core/dep/font-awesome/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.231595 XGEE-0.3.0/xgee/core/dep/font-awesome/css/
+-rw-r--r--   0 root         (0) root         (0)    73117 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/all.css
+-rw-r--r--   0 root         (0) root         (0)    58935 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/all.min.css
+-rw-r--r--   0 root         (0) root         (0)      732 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/brands.css
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/brands.min.css
+-rw-r--r--   0 root         (0) root         (0)    71482 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/fontawesome.css
+-rw-r--r--   0 root         (0) root         (0)    57503 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/fontawesome.min.css
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/regular.css
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/regular.min.css
+-rw-r--r--   0 root         (0) root         (0)      727 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/solid.css
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/solid.min.css
+-rw-r--r--   0 root         (0) root         (0)     8077 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/svg-with-js.css
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/svg-with-js.min.css
+-rw-r--r--   0 root         (0) root         (0)    41312 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/v4-shims.css
+-rw-r--r--   0 root         (0) root         (0)    26702 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/css/v4-shims.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.237595 XGEE-0.3.0/xgee/core/dep/font-awesome/js/
+-rw-r--r--   0 root         (0) root         (0)  1248390 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/all.js
+-rw-r--r--   0 root         (0) root         (0)  1182553 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/all.min.js
+-rw-r--r--   0 root         (0) root         (0)   445294 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/brands.js
+-rw-r--r--   0 root         (0) root         (0)   438090 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/brands.min.js
+-rw-r--r--   0 root         (0) root         (0)    33929 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/conflict-detection.js
+-rw-r--r--   0 root         (0) root         (0)    13502 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/conflict-detection.min.js
+-rw-r--r--   0 root         (0) root         (0)    79139 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/fontawesome.js
+-rw-r--r--   0 root         (0) root         (0)    37191 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/fontawesome.min.js
+-rw-r--r--   0 root         (0) root         (0)   107110 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/regular.js
+-rw-r--r--   0 root         (0) root         (0)   103386 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/regular.min.js
+-rw-r--r--   0 root         (0) root         (0)   617405 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/solid.js
+-rw-r--r--   0 root         (0) root         (0)   604447 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/solid.min.js
+-rw-r--r--   0 root         (0) root         (0)    17459 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/v4-shims.js
+-rw-r--r--   0 root         (0) root         (0)    15055 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/js/v4-shims.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.242595 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/
+-rw-r--r--   0 root         (0) root         (0)   134878 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 root         (0) root         (0)   729325 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 root         (0) root         (0)   134572 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 root         (0) root         (0)    90872 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 root         (0) root         (0)    77444 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 root         (0) root         (0)    34390 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 root         (0) root         (0)   144322 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 root         (0) root         (0)    34092 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 root         (0) root         (0)    16800 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 root         (0) root         (0)    13596 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 root         (0) root         (0)   204866 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 root         (0) root         (0)   910710 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 root         (0) root         (0)   204580 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 root         (0) root         (0)   104252 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 root         (0) root         (0)    80328 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.243595 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.244595 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css
+-rw-r--r--   0 root         (0) root         (0)    91213 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
+-rw-r--r--   0 root         (0) root         (0)    14532 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
+-rw-r--r--   0 root         (0) root         (0)    27807 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
+-rw-r--r--   0 root         (0) root         (0)   131140 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    22405 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js
+-rw-r--r--   0 root         (0) root         (0)     5855 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.244595 XGEE-0.3.0/xgee/core/dep/jquery/
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    86927 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery/jquery-3.3.1.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.245595 XGEE-0.3.0/xgee/core/dep/jquery-ui/
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.246595 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7074 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4676 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     6313 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 root         (0) root         (0)    32076 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/jquery-ui.min.css
+-rw-r--r--   0 root         (0) root         (0)   253669 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/jquery-ui/jquery-ui.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.248595 XGEE-0.3.0/xgee/core/dep/jsa/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-27 10:09:46.000000 XGEE-0.3.0/xgee/core/dep/jsa/.git
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.251595 XGEE-0.3.0/xgee/core/dep/jsa/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.254594 XGEE-0.3.0/xgee/core/dep/jsa/img/black/
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/bubble-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/bubble.svg
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/close.svg
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/folder.svg
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/home.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/maximize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/menu-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/menu.svg
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/minimize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/settings.svg
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     2343 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/view-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/black/view.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/close.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/loading.svg
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     3173 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/resize-ne.svg
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/resize-nw.svg
+-rw-r--r--   0 root         (0) root         (0)     3173 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/resize-se.svg
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/resize-sw.svg
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/restore.svg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/tool-default.svg
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/view-close.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.257594 XGEE-0.3.0/xgee/core/dep/jsa/img/white/
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/bubble-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/bubble.svg
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/close.svg
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/folder.svg
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/home.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/maximize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/menu-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/menu.svg
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/minimize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/settings.svg
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/view-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/img/white/view.svg
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/jsapplication.css
+-rw-r--r--   0 root         (0) root         (0)   357922 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/jsapplication.js
+-rw-r--r--   0 root         (0) root         (0)    15308 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/jsapplicationPlugins.js
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/package.json
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/dep/jsa/webpack.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.257594 XGEE-0.3.0/xgee/core/dep/mxgraph/
+-rw-r--r--   0 root         (0) root         (0)    10487 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.258594 XGEE-0.3.0/xgee/core/dep/mxgraph/css/
+-rw-r--r--   0 root         (0) root         (0)     4325 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/css/common.css
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/css/explorer.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.261594 XGEE-0.3.0/xgee/core/dep/mxgraph/images/
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/button.gif
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/close.gif
+-rw-r--r--   0 root         (0) root         (0)      877 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/collapsed.gif
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/error.gif
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/expanded.gif
+-rw-r--r--   0 root         (0) root         (0)      843 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/maximize.gif
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/minimize.gif
+-rw-r--r--   0 root         (0) root         (0)      845 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/normalize.gif
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/point.gif
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/resize.gif
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/separator.gif
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/submenu.gif
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/transparent.gif
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/warning.gif
+-rw-r--r--   0 root         (0) root         (0)      425 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/warning.png
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/window-title.gif
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/images/window.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.261594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.262594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/
+-rw-r--r--   0 root         (0) root         (0)     3232 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9716 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js
+-rw-r--r--   0 root         (0) root         (0)    14610 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js
+-rw-r--r--   0 root         (0) root         (0)    74993 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxEditor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.265594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/
+-rw-r--r--   0 root         (0) root         (0)     7282 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js
+-rw-r--r--   0 root         (0) root         (0)    62381 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js
+-rw-r--r--   0 root         (0) root         (0)    13695 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js
+-rw-r--r--   0 root         (0) root         (0)    63081 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9925 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js
+-rw-r--r--   0 root         (0) root         (0)     5944 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js
+-rw-r--r--   0 root         (0) root         (0)    39448 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js
+-rw-r--r--   0 root         (0) root         (0)     7701 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxHandle.js
+-rw-r--r--   0 root         (0) root         (0)    10128 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)    11402 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js
+-rw-r--r--   0 root         (0) root         (0)     5293 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9837 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxRubberband.js
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js
+-rw-r--r--   0 root         (0) root         (0)     7419 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js
+-rw-r--r--   0 root         (0) root         (0)    52962 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js
+-rw-r--r--   0 root         (0) root         (0)    12044 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/index.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.268594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/
+-rw-r--r--   0 root         (0) root         (0)     4531 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCellCodec.js
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)    13541 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCodec.js
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js
+-rw-r--r--   0 root         (0) root         (0)     9221 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js
+-rw-r--r--   0 root         (0) root         (0)     6163 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxModelCodec.js
+-rw-r--r--   0 root         (0) root         (0)    30213 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js
+-rw-r--r--   0 root         (0) root         (0)      818 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.270594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.270594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.271594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
+-rw-r--r--   0 root         (0) root         (0)    20322 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
+-rw-r--r--   0 root         (0) root         (0)    23605 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
+-rw-r--r--   0 root         (0) root         (0)    20146 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
+-rw-r--r--   0 root         (0) root         (0)    22708 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.272594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/
+-rw-r--r--   0 root         (0) root         (0)    43070 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
+-rw-r--r--   0 root         (0) root         (0)     4343 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js
+-rw-r--r--   0 root         (0) root         (0)    22959 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js
+-rw-r--r--   0 root         (0) root         (0)    14338 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js
+-rw-r--r--   0 root         (0) root         (0)    14251 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js
+-rw-r--r--   0 root         (0) root         (0)     8037 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js
+-rw-r--r--   0 root         (0) root         (0)    12740 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.273594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/
+-rw-r--r--   0 root         (0) root         (0)    15954 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxCell.js
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxCellPath.js
+-rw-r--r--   0 root         (0) root         (0)    12721 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxGeometry.js
+-rw-r--r--   0 root         (0) root         (0)    62665 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxGraphModel.js
+-rw-r--r--   0 root         (0) root         (0)    28988 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/mxClient.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.277594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxActor.js
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxArrow.js
+-rw-r--r--   0 root         (0) root         (0)    11601 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxCloud.js
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxConnector.js
+-rw-r--r--   0 root         (0) root         (0)     2694 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxCylinder.js
+-rw-r--r--   0 root         (0) root         (0)     2823 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxEllipse.js
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxHexagon.js
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxImageShape.js
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxLabel.js
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxLine.js
+-rw-r--r--   0 root         (0) root         (0)     5400 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxMarker.js
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxPolyline.js
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxRhombus.js
+-rw-r--r--   0 root         (0) root         (0)    38952 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxShape.js
+-rw-r--r--   0 root         (0) root         (0)    26031 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxStencil.js
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     9507 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js
+-rw-r--r--   0 root         (0) root         (0)    37084 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxText.js
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxTriangle.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.284594 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/
+-rw-r--r--   0 root         (0) root         (0)    11723 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAnimation.js
+-rw-r--r--   0 root         (0) root         (0)     4430 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxClipboard.js
+-rw-r--r--   0 root         (0) root         (0)    63826 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxConstants.js
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDictionary.js
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDivResizer.js
+-rw-r--r--   0 root         (0) root         (0)    16885 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDragSource.js
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEffects.js
+-rw-r--r--   0 root         (0) root         (0)    27401 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEvent.js
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEventObject.js
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEventSource.js
+-rw-r--r--   0 root         (0) root         (0)     4041 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxForm.js
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxGuide.js
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImage.js
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImageBundle.js
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImageExport.js
+-rw-r--r--   0 root         (0) root         (0)     8228 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxLog.js
+-rw-r--r--   0 root         (0) root         (0)     5691 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxMorphing.js
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js
+-rw-r--r--   0 root         (0) root         (0)     5082 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPanningManager.js
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPoint.js
+-rw-r--r--   0 root         (0) root         (0)    14045 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js
+-rw-r--r--   0 root         (0) root         (0)     3693 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxRectangle.js
+-rw-r--r--   0 root         (0) root         (0)    11080 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxResources.js
+-rw-r--r--   0 root         (0) root         (0)    45946 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    12132 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxToolbar.js
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUndoManager.js
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js
+-rw-r--r--   0 root         (0) root         (0)   106481 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUtils.js
+-rw-r--r--   0 root         (0) root         (0)    26243 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    27971 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxWindow.js
+-rw-r--r--   0 root         (0) root         (0)    28763 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    10820 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.288593 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/
+-rw-r--r--   0 root         (0) root         (0)    35624 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellEditor.js
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js
+-rw-r--r--   0 root         (0) root         (0)    44101 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js
+-rw-r--r--   0 root         (0) root         (0)     9726 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellState.js
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js
+-rw-r--r--   0 root         (0) root         (0)    42452 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js
+-rw-r--r--   0 root         (0) root         (0)   333205 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraph.js
+-rw-r--r--   0 root         (0) root         (0)     9127 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js
+-rw-r--r--   0 root         (0) root         (0)    74549 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraphView.js
+-rw-r--r--   0 root         (0) root         (0)    10941 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js
+-rw-r--r--   0 root         (0) root         (0)     7440 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js
+-rw-r--r--   0 root         (0) root         (0)    19683 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxOutline.js
+-rw-r--r--   0 root         (0) root         (0)    20530 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxPerimeter.js
+-rw-r--r--   0 root         (0) root         (0)    32135 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxStylesheet.js
+-rw-r--r--   0 root         (0) root         (0)     9336 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.289593 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/editor.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/editor_de.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/editor_zh.txt
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/graph.txt
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/graph_de.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/mxgraph/resources/graph_zh.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.290593 XGEE-0.3.0/xgee/core/dep/notifyjs/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/notifyjs/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13780 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/notifyjs/notify.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.290593 XGEE-0.3.0/xgee/core/dep/underscore/
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/underscore/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    18069 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/dep/underscore/underscore-min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.221595 XGEE-0.3.0/xgee/core/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.290593 XGEE-0.3.0/xgee/core/plugins/autostart/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.291593 XGEE-0.3.0/xgee/core/plugins/autostart/js/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/autostart/js/AppStartupEvent.js
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/autostart/js/AppStartupObserver.js
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/autostart/js/Autostarter.js
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/autostart/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.291593 XGEE-0.3.0/xgee/core/plugins/clipboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.292593 XGEE-0.3.0/xgee/core/plugins/clipboard/js/
+-rw-r--r--   0 root         (0) root         (0)      969 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/AppClipboard.js
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/Clipboard.js
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardAPI.js
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)      618 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardManager.js
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/clipboard/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.292593 XGEE-0.3.0/xgee/core/plugins/contextMenu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.294593 XGEE-0.3.0/xgee/core/plugins/contextMenu/js/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu/js/ContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu/js/util.js
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.293593 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.293593 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/css/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/css/contextMenu.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.293593 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/js/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/js/Filter.js
+-rw-r--r--   0 root         (0) root         (0)    13387 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.293593 XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.293593 XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/js/
+-rw-r--r--   0 root         (0) root         (0)     4740 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/js/util.js
+-rw-r--r--   0 root         (0) root         (0)     4218 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.294593 XGEE-0.3.0/xgee/core/plugins/ecore/
+-rw-r--r--   0 root         (0) root         (0)    11515 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    93760 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/ecore.xmi.js
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.296593 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)      366 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8381 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.298593 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/
+-rw-r--r--   0 root         (0) root         (0)   181013 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/example.js
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/hello-world.js
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/not-pretty.xml
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js
+-rw-r--r--   0 root         (0) root         (0)    99650 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/test.html
+-rw-r--r--   0 root         (0) root         (0)    51402 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/test.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.298593 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/lib/
+-rw-r--r--   0 root         (0) root         (0)    43541 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/lib/sax.js
+-rw-r--r--   0 root         (0) root         (0)    85352 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.307593 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/bom.js
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/case.js
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-chunked.js
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-end-split.js
+-rw-r--r--   0 root         (0) root         (0)      782 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata.js
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cyrillic.js
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/duplicate-attribute.js
+-rw-r--r--   0 root         (0) root         (0)      343 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/emoji.js
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/end_empty_stream.js
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/entities.js
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/entity-mega.js
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/entity-nan.js
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/flush.js
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/index.js
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-35.js
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-47.js
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js
+-rw-r--r--   0 root         (0) root         (0)      467 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-84.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/not-string.js
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/script.js
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js
+-rw-r--r--   0 root         (0) root         (0)      904 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/stand-alone-comment.js
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/trailing-attribute-no-value.js
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/trailing-non-whitespace.js
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/unclosed-root.js
+-rw-r--r--   0 root         (0) root         (0)      727 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js
+-rw-r--r--   0 root         (0) root         (0)      429 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xml_entities.js
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-as-tag-name.js
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js
+-rw-r--r--   0 root         (0) root         (0)     5577 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js
+-rw-r--r--   0 root         (0) root         (0)      509 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix.js
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.211596 XGEE-0.3.0/xgee/core/plugins/ecoreDebuggerUi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.308593 XGEE-0.3.0/xgee/core/plugins/ecoreDebuggerUi/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreDebuggerUi/js/ecoreDebuggerUiController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.308593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-27 10:09:47.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/.git
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.312593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/changes/
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/changes/esChanges.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.312593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/esDebugging.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.312593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/lib/
+-rw-r--r--   0 root         (0) root         (0)     4918 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/lib/libesync.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.313593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esDomain.js
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esErrors.js
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esLookup.js
+-rw-r--r--   0 root         (0) root         (0)    13249 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esMetaSync.js
+-rw-r--r--   0 root         (0) root         (0)    20548 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/ecoreSync.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.314593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/interfaces/esInstance.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.315593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/
+-rw-r--r--   0 root         (0) root         (0)    10832 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js
+-rw-r--r--   0 root         (0) root         (0)     9168 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js
+-rw-r--r--   0 root         (0) root         (0)     9420 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.316593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/
+-rw-r--r--   0 root         (0) root         (0)    20117 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueries.js
+-rw-r--r--   0 root         (0) root         (0)    36223 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)    26527 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.316593 XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/auxiliaries.js
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/esLogging.js
+-rw-r--r--   0 root         (0) root         (0)    14957 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/esUtils.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/uuid.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.308593 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.309593 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/css/
+-rw-r--r--   0 root         (0) root         (0)     5694 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.311593 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg
+-rw-r--r--   0 root         (0) root         (0)     5270 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.312593 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/
+-rw-r--r--   0 root         (0) root         (0)     8088 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js
+-rw-r--r--   0 root         (0) root         (0)    48201 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.317593 XGEE-0.3.0/xgee/core/plugins/editor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.213596 XGEE-0.3.0/xgee/core/plugins/editor/controllers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.318593 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/
+-rw-r--r--   0 root         (0) root         (0)      970 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/AnchorController.js
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/ContainerController.js
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/EdgeController.js
+-rw-r--r--   0 root         (0) root         (0)    15589 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/GraphController.js
+-rw-r--r--   0 root         (0) root         (0)     7060 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/GraphObjectController.js
+-rw-r--r--   0 root         (0) root         (0)      976 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/LabelController.js
+-rw-r--r--   0 root         (0) root         (0)      978 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/QueryController.js
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/VertexController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.318593 XGEE-0.3.0/xgee/core/plugins/editor/controllers/palette/
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/controllers/palette/PaletteController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.319593 XGEE-0.3.0/xgee/core/plugins/editor/css/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/css/loading.css
+-rw-r--r--   0 root         (0) root         (0)      115 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/css/xgeeJsaIntegration.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.319593 XGEE-0.3.0/xgee/core/plugins/editor/extensions/
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.319593 XGEE-0.3.0/xgee/core/plugins/editor/graph/
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/graph/GraphResourceProvider.js
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/graph/mxGraphIntegration.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.320592 XGEE-0.3.0/xgee/core/plugins/editor/interactions/
+-rw-r--r--   0 root         (0) root         (0)     3785 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/interactions/DropReception.js
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/interactions/GraphInteraction.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.320592 XGEE-0.3.0/xgee/core/plugins/editor/lib/
+-rw-r--r--   0 root         (0) root         (0)    10080 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/lib/libapi.js
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/lib/libaux.js
+-rw-r--r--   0 root         (0) root         (0)    20059 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/lib/libjsa.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/lib/uuid.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.321592 XGEE-0.3.0/xgee/core/plugins/editor/model/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/PresentationModel.js
+-rw-r--r--   0 root         (0) root         (0)    83708 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/editorModel.ecore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.328592 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Anchor.js
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/AnchorManager.js
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/AnchorType.js
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Container.js
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerManager.js
+-rw-r--r--   0 root         (0) root         (0)      608 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerType.js
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/DeletableObject.js
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EObjectOwner.js
+-rw-r--r--   0 root         (0) root         (0)    10305 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Edge.js
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EdgeContainer.js
+-rw-r--r--   0 root         (0) root         (0)     6994 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EdgeManager.js
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EdgeType.js
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EventProvider.js
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/FloatingLabel.js
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphEvent.js
+-rw-r--r--   0 root         (0) root         (0)    27960 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js
+-rw-r--r--   0 root         (0) root         (0)     6623 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModel.js
+-rw-r--r--   0 root         (0) root         (0)    12643 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModelFactory.js
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModelManager.js
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphObject.js
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphObjectManager.js
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphObjectType.js
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Label.js
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelManager.js
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelSegment.js
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelSegmentType.js
+-rw-r--r--   0 root         (0) root         (0)      386 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelType.js
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LocatableObject.js
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/NestedLabel.js
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/RoutableObject.js
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/SizableObject.js
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertex.js
+-rw-r--r--   0 root         (0) root         (0)     7913 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertexManager.js
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertexType.js
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/TransactionObject.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/TypedObject.js
+-rw-r--r--   0 root         (0) root         (0)     3517 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Vertex.js
+-rw-r--r--   0 root         (0) root         (0)    12233 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexContainer.js
+-rw-r--r--   0 root         (0) root         (0)    12045 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexManager.js
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexType.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.330592 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/DragAndDropTool.js
+-rw-r--r--   0 root         (0) root         (0)    16081 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/GraphTool.js
+-rw-r--r--   0 root         (0) root         (0)     8885 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/PaletteModel.js
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/SelectionTool.js
+-rw-r--r--   0 root         (0) root         (0)     8885 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/model/palette/ToolGenerator.js
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.330592 XGEE-0.3.0/xgee/core/plugins/editor/queries/
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/queries/Query.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.331592 XGEE-0.3.0/xgee/core/plugins/editor/view/
+-rw-r--r--   0 root         (0) root         (0)    55157 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/view/GraphView.js
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/view/GraphViewMenu.js
+-rw-r--r--   0 root         (0) root         (0)    22370 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/view/GraphViewPort.js
+-rw-r--r--   0 root         (0) root         (0)     3483 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/view/PaletteView.js
+-rw-r--r--   0 root         (0) root         (0)     5888 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/editor/view/ScreenshotExport.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.331592 XGEE-0.3.0/xgee/core/plugins/eoq.actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.331592 XGEE-0.3.0/xgee/core/plugins/eoq.actions/css/
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eoq.actions/css/ActionsUi.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.332592 XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsController.js
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsCore.js
+-rw-r--r--   0 root         (0) root         (0)    23053 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsUi.js
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eoq.actions/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.333592 XGEE-0.3.0/xgee/core/plugins/eoq1/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-27 10:09:47.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/.git
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/README.md
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/commandparser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.334592 XGEE-0.3.0/xgee/core/plugins/eoq1/domains/
+-rw-r--r--   0 root         (0) root         (0)     5897 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/domains/bufferingdomain.js
+-rw-r--r--   0 root         (0) root         (0)      879 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/domains/domain.js
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/domains/httppostdomain.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.334592 XGEE-0.3.0/xgee/core/plugins/eoq1/model/
+-rw-r--r--   0 root         (0) root         (0)    37451 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/model/model.js
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/package.json
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/plugin.js
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/queryparser.js
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/resultparser.js
+-rw-r--r--   0 root         (0) root         (0)    12168 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq1/valueparser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.335592 XGEE-0.3.0/xgee/core/plugins/eoq2/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/.git
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.335592 XGEE-0.3.0/xgee/core/plugins/eoq2/action/
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/action/call.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.336592 XGEE-0.3.0/xgee/core/plugins/eoq2/command/
+-rw-r--r--   0 root         (0) root         (0)    12287 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/command/command.js
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/command/result.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.336592 XGEE-0.3.0/xgee/core/plugins/eoq2/domain/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/domain/domain.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.336592 XGEE-0.3.0/xgee/core/plugins/eoq2/domain/remote/
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js
+-rw-r--r--   0 root         (0) root         (0)     5812 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/eoq2.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.336592 XGEE-0.3.0/xgee/core/plugins/eoq2/event/
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/event/event.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.337592 XGEE-0.3.0/xgee/core/plugins/eoq2/frame/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/frame/frame.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.337592 XGEE-0.3.0/xgee/core/plugins/eoq2/legacy/
+-rw-r--r--   0 root         (0) root         (0)    14240 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/legacy/legacy.js
+-rw-r--r--   0 root         (0) root         (0)      440 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/package.json
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.337592 XGEE-0.3.0/xgee/core/plugins/eoq2/query/
+-rw-r--r--   0 root         (0) root         (0)    14393 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/query/query.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.337592 XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/jsonserializer.js
+-rw-r--r--   0 root         (0) root         (0)      725 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/serializer.js
+-rw-r--r--   0 root         (0) root         (0)    40363 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/textserializer.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.338592 XGEE-0.3.0/xgee/core/plugins/eoq2/util/
+-rw-r--r--   0 root         (0) root         (0)     2823 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/core/plugins/eoq2/util/logger.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.338592 XGEE-0.3.0/xgee/core/plugins/eventBroker/
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eventBroker/BasicEvent.js
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eventBroker/QueryDebugEvent.js
+-rw-r--r--   0 root         (0) root         (0)      694 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eventBroker/SelectionChangedEvent.js
+-rw-r--r--   0 root         (0) root         (0)     3823 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/eventBroker/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.339592 XGEE-0.3.0/xgee/core/plugins/iconProvider/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.339592 XGEE-0.3.0/xgee/core/plugins/iconProvider/js/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/iconProvider/js/IconProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/iconProvider/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.339592 XGEE-0.3.0/xgee/core/plugins/keyHandler/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.339592 XGEE-0.3.0/xgee/core/plugins/keyHandler/js/
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/keyHandler/js/KeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/keyHandler/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.339592 XGEE-0.3.0/xgee/core/plugins/keyHandler.ecore/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/keyHandler.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.340592 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.341592 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.342592 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css
+-rw-r--r--   0 root         (0) root         (0)    91213 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
+-rw-r--r--   0 root         (0) root         (0)    14532 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
+-rw-r--r--   0 root         (0) root         (0)    27807 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
+-rw-r--r--   0 root         (0) root         (0)   131140 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    22405 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js
+-rw-r--r--   0 root         (0) root         (0)     5855 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.342592 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.349592 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/
+-rw-r--r--   0 root         (0) root         (0)      554 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif
+-rw-r--r--   0 root         (0) root         (0)      123 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAttribute.gif
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EClass.gif
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EDataType.gif
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnum.gif
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnumLiteral.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EFactory.gif
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericElementType.gif
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericException.gif
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericSuperType.gif
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericType.gif
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericTypeArgument.gif
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericWildcard.gif
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EObject.gif
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceN.gif
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToM.gif
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOne.gif
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToN.gif
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZero.gif
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToN.gif
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToOne.gif
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOperation.gif
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EPackage.gif
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EReference.gif
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EStringToStringMapEntry.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/ETypeParameter.gif
+-rw-r--r--   0 root         (0) root         (0)      554 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eClassifiers.gif
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eOperations.gif
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eSubpackages.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eTypeParameters.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.349592 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/js/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js
+-rw-r--r--   0 root         (0) root         (0)    29729 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.342592 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView.eoq/
+-rw-r--r--   0 root         (0) root         (0)    16933 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.350592 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   128443 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js
+-rw-r--r--   0 root         (0) root         (0)   162267 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.351592 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif
+-rw-r--r--   0 root         (0) root         (0)     5510 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif
+-rw-r--r--   0 root         (0) root         (0)    24749 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less
+-rw-r--r--   0 root         (0) root         (0)      852 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif
+-rw-r--r--   0 root         (0) root         (0)      852 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.352592 XGEE-0.3.0/xgee/core/plugins/propertiesView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.355592 XGEE-0.3.0/xgee/core/plugins/propertiesView/css/
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/css/PropertiesView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.355592 XGEE-0.3.0/xgee/core/plugins/propertiesView/doc/
+-rw-r--r--   0 root         (0) root         (0)    38735 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.356592 XGEE-0.3.0/xgee/core/plugins/propertiesView/js/
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js
+-rw-r--r--   0 root         (0) root         (0)      298 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/js/PropertiesBubble.js
+-rw-r--r--   0 root         (0) root         (0)      779 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     7532 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/js/PropertiesViewController.js
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.352592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.355592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/js/
+-rw-r--r--   0 root         (0) root         (0)    10124 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.352592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.352592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/
+-rw-r--r--   0 root         (0) root         (0)     7014 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.353592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.353592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/css/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/css/EcoreEditorsPropertiesPane.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.353592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/js/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.353592 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.354591 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/css/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/css/EcoreModifyPropertiesPane.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.354591 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/js/
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.354591 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.354591 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/js/
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.355592 XGEE-0.3.0/xgee/core/plugins/propertiesView.info/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.355592 XGEE-0.3.0/xgee/core/plugins/propertiesView.info/js/
+-rw-r--r--   0 root         (0) root         (0)     3609 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/propertiesView.info/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.356592 XGEE-0.3.0/xgee/core/plugins/tool.goToView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.356592 XGEE-0.3.0/xgee/core/plugins/tool.goToView/css/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.goToView/css/GoToViewTool.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.357591 XGEE-0.3.0/xgee/core/plugins/tool.goToView/img/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.357591 XGEE-0.3.0/xgee/core/plugins/tool.goToView/js/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.goToView/js/GoToViewTool.js
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.goToView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.357591 XGEE-0.3.0/xgee/core/plugins/tool.notes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.357591 XGEE-0.3.0/xgee/core/plugins/tool.notes/css/
+-rw-r--r--   0 root         (0) root         (0)     4415 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/css/NotesTool.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.358591 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-error.svg
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-info.svg
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-success.svg
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-warning.svg
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/img/tool-notes.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.359591 XGEE-0.3.0/xgee/core/plugins/tool.notes/js/
+-rw-r--r--   0 root         (0) root         (0)     6924 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/js/NotesTool.js
+-rw-r--r--   0 root         (0) root         (0)      940 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/js/NotesToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tool.notes/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.359591 XGEE-0.3.0/xgee/core/plugins/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.359591 XGEE-0.3.0/xgee/core/plugins/tools/js/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tools/js/ToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tools/js/ToolsController.js
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/tools/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.359591 XGEE-0.3.0/xgee/core/plugins/view.dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.362591 XGEE-0.3.0/xgee/core/plugins/view.dashboard/css/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard/css/DashboardView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.362591 XGEE-0.3.0/xgee/core/plugins/view.dashboard/img/
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard/img/view-dashboard.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.362591 XGEE-0.3.0/xgee/core/plugins/view.dashboard/js/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard/js/DashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.359591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.360591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/js/
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.360591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.360591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/css/
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.361591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.362591 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/
+-rw-r--r--   0 root         (0) root         (0)    24067 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.362591 XGEE-0.3.0/xgee/core/plugins/view.workspace/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/view.workspace/css/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.workspace/css/WorkspaceView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/view.workspace/img/
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.workspace/img/view-workspace.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/view.workspace/js/
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/view.workspace/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/views/js/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/views/js/ViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/views/js/ViewsController.js
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/views/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.363591 XGEE-0.3.0/xgee/core/plugins/viewsMenu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.364591 XGEE-0.3.0/xgee/core/plugins/viewsMenu/js/
+-rw-r--r--   0 root         (0) root         (0)     5303 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/viewsMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.364591 XGEE-0.3.0/xgee/core/plugins/viewsTabbar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.364591 XGEE-0.3.0/xgee/core/plugins/viewsTabbar/css/
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/plugins/viewsTabbar/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.221595 XGEE-0.3.0/xgee/core/res/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.365591 XGEE-0.3.0/xgee/core/res/css/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/UIComponents.canvasSearch.css
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/app.css
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/canvas.css
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/contextmenu.css
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/layout.css
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/notes.css
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/palette.css
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/css/uiControls.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.368591 XGEE-0.3.0/xgee/core/res/img/
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/edit.svg
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/eye.svg
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/globe.svg
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-allocations.svg
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-functions.svg
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-hardware.svg
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tool-domain-status-down.svg
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tool-domain-status-error.svg
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tool-domain-status-up-down.svg
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tool-domain-status-up.svg
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tool-domain-status.svg
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/tree.svg
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/img/view-editor.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.369591 XGEE-0.3.0/xgee/core/res/js/
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/DomainStatistics.js
+-rw-r--r--   0 root         (0) root         (0)    12997 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/app.js
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/commands.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.369591 XGEE-0.3.0/xgee/core/res/js/connectors/
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/connectors/connectors.graph.js
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/connectors/connectors.selection.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.369591 XGEE-0.3.0/xgee/core/res/js/grids/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/grids/points_grid.svg
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/ports.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.370591 XGEE-0.3.0/xgee/core/res/js/ui/
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/ui/DomainStatusTool.js
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/ui/ui.colorProvider.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.370591 XGEE-0.3.0/xgee/core/res/js/workspace/
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/workspace/workspace.jobs.js
+-rw-r--r--   0 root         (0) root         (0)    18830 2023-06-27 10:09:45.000000 XGEE-0.3.0/xgee/core/res/js/workspace/workspace.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.370591 XGEE-0.3.0/xgee/eoqserver/
+-rw-r--r--   0 root         (0) root         (0)    13048 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/eoqserver/PyEoq2WebServer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 10:09:48.000000 XGEE-0.3.0/xgee/eoqserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.371591 XGEE-0.3.0/xgee/eoqserver/eoq1/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.372591 XGEE-0.3.0/xgee/eoqserver/eoq1/actions/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/actions/actionutils.py
+-rw-r--r--   0 root         (0) root         (0)    29323 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/actions/externalactionhandler.py
+-rw-r--r--   0 root         (0) root         (0)     9347 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/commandparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.373591 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72154 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/localdomain.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/remotehttpdomain.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.373591 XGEE-0.3.0/xgee/eoqserver/eoq1/error/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/error/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/error/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.374591 XGEE-0.3.0/xgee/eoqserver/eoq1/model/
+-rw-r--r--   0 root         (0) root         (0)     7459 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64472 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    22749 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/queryparser.py
+-rw-r--r--   0 root         (0) root         (0)     8387 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/resultparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.374591 XGEE-0.3.0/xgee/eoqserver/eoq1/utils/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25693 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/utils/csvconnector.py
+-rw-r--r--   0 root         (0) root         (0)    10694 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq1/valueparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.374591 XGEE-0.3.0/xgee/eoqserver/eoq2/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.375591 XGEE-0.3.0/xgee/eoqserver/eoq2/action/
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/action.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/call.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/callhandler.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/callmanager.py
+-rw-r--r--   0 root         (0) root         (0)     8117 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.376591 XGEE-0.3.0/xgee/eoqserver/eoq2/action/externalpy/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/externalpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24055 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/action/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.377591 XGEE-0.3.0/xgee/eoqserver/eoq2/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/command/command.py
+-rw-r--r--   0 root         (0) root         (0)    64224 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/command/commandrunner.py
+-rw-r--r--   0 root         (0) root         (0)    43028 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/command/diff.py
+-rw-r--r--   0 root         (0) root         (0)      854 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/command/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.377591 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.378591 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/local/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/local/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.378591 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.379591 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/remote/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/remote/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.379591 XGEE-0.3.0/xgee/eoqserver/eoq2/event/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/event/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.380591 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/domainframehandler.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/frame.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/framehandler.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/frame/multiversionframehandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.380591 XGEE-0.3.0/xgee/eoqserver/eoq2/legacy/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/legacy/legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.381591 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/mdb.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/mdbaccessor.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/nocodec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.382591 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.383591 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py
+-rw-r--r--   0 root         (0) root         (0)    36345 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
+-rw-r--r--   0 root         (0) root         (0)     3823 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
+-rw-r--r--   0 root         (0) root         (0)    80843 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.383591 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.384591 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/valuecodec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.384591 XGEE-0.3.0/xgee/eoqserver/eoq2/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12347 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    38368 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/query/queryrunner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.385591 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/jsonserializer.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/jsserializer.py
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/pyserializer.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/serializer.py
+-rw-r--r--   0 root         (0) root         (0)    35630 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/textserializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.387591 XGEE-0.3.0/xgee/eoqserver/eoq2/util/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/backup.py
+-rw-r--r--   0 root         (0) root         (0)     4033 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    13851 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/csvconnector.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/error.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/model.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-06-27 10:09:49.000000 XGEE-0.3.0/xgee/eoqserver/eoq2/util/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 10:09:50.387591 XGEE-0.3.0/xgee/meta/
+-rw-rw-rw-   0 root         (0) root         (0)     7875 2023-06-27 10:09:43.000000 XGEE-0.3.0/xgee/meta/layout.ecore
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-06-27 10:09:43.000000 XGEE-0.3.0/xgee/xgee.py
```

### Comparing `XGEE-0.2.9/LICENSE` & `XGEE-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/PKG-INFO` & `XGEE-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XGEE
-Version: 0.2.9
+Version: 0.3.0
 Summary: eXtensible Graphical EMOF Editor - a framework for graphical editing single page web-applications
 Home-page: https://gitlab.com/xgee/py/xgee
 Author: Matthias Brunner
 Author-email: matthias.brunner@ils.uni-stuttgart.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XGEE-0.2.9/README.md` & `XGEE-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/XGEE.egg-info/PKG-INFO` & `XGEE-0.3.0/XGEE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XGEE
-Version: 0.2.9
+Version: 0.3.0
 Summary: eXtensible Graphical EMOF Editor - a framework for graphical editing single page web-applications
 Home-page: https://gitlab.com/xgee/py/xgee
 Author: Matthias Brunner
 Author-email: matthias.brunner@ils.uni-stuttgart.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XGEE-0.2.9/XGEE.egg-info/SOURCES.txt` & `XGEE-0.3.0/XGEE.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,346 +10,315 @@
 xgee/__init__.py
 xgee/__main__.py
 xgee/xgee.py
 xgee/core/.git
 xgee/core/.gitmodules
 xgee/core/LICENSE
 xgee/core/README.md
-xgee/core/contrib/bluebird.js
-xgee/core/contrib/bluebird.min.js
-xgee/core/contrib/notify.min.js
-xgee/core/contrib/notifyjs-LICENSE
-xgee/core/contrib/underscore-LICENSE
-xgee/core/contrib/underscore-min.js
-xgee/core/contrib/font-awesome/LICENSE.txt
-xgee/core/contrib/font-awesome/css/all.css
-xgee/core/contrib/font-awesome/css/all.min.css
-xgee/core/contrib/font-awesome/css/brands.css
-xgee/core/contrib/font-awesome/css/brands.min.css
-xgee/core/contrib/font-awesome/css/fontawesome.css
-xgee/core/contrib/font-awesome/css/fontawesome.min.css
-xgee/core/contrib/font-awesome/css/regular.css
-xgee/core/contrib/font-awesome/css/regular.min.css
-xgee/core/contrib/font-awesome/css/solid.css
-xgee/core/contrib/font-awesome/css/solid.min.css
-xgee/core/contrib/font-awesome/css/svg-with-js.css
-xgee/core/contrib/font-awesome/css/svg-with-js.min.css
-xgee/core/contrib/font-awesome/css/v4-shims.css
-xgee/core/contrib/font-awesome/css/v4-shims.min.css
-xgee/core/contrib/font-awesome/js/all.js
-xgee/core/contrib/font-awesome/js/all.min.js
-xgee/core/contrib/font-awesome/js/brands.js
-xgee/core/contrib/font-awesome/js/brands.min.js
-xgee/core/contrib/font-awesome/js/conflict-detection.js
-xgee/core/contrib/font-awesome/js/conflict-detection.min.js
-xgee/core/contrib/font-awesome/js/fontawesome.js
-xgee/core/contrib/font-awesome/js/fontawesome.min.js
-xgee/core/contrib/font-awesome/js/regular.js
-xgee/core/contrib/font-awesome/js/regular.min.js
-xgee/core/contrib/font-awesome/js/solid.js
-xgee/core/contrib/font-awesome/js/solid.min.js
-xgee/core/contrib/font-awesome/js/v4-shims.js
-xgee/core/contrib/font-awesome/js/v4-shims.min.js
-xgee/core/contrib/font-awesome/webfonts/fa-brands-400.eot
-xgee/core/contrib/font-awesome/webfonts/fa-brands-400.svg
-xgee/core/contrib/font-awesome/webfonts/fa-brands-400.ttf
-xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff
-xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff2
-xgee/core/contrib/font-awesome/webfonts/fa-regular-400.eot
-xgee/core/contrib/font-awesome/webfonts/fa-regular-400.svg
-xgee/core/contrib/font-awesome/webfonts/fa-regular-400.ttf
-xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff
-xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff2
-xgee/core/contrib/font-awesome/webfonts/fa-solid-900.eot
-xgee/core/contrib/font-awesome/webfonts/fa-solid-900.svg
-xgee/core/contrib/font-awesome/webfonts/fa-solid-900.ttf
-xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff
-xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff2
-xgee/core/contrib/jQuery-contextMenu-2.8/LICENSE
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.css
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.js
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.js
-xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.min.js
-xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.eot
-xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
-xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff
-xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
-xgee/core/contrib/jquery/LICENSE.txt
-xgee/core/contrib/jquery/jquery-3.3.1.min.js
-xgee/core/contrib/jquery-ui/LICENSE.txt
-xgee/core/contrib/jquery-ui/jquery-ui.min.css
-xgee/core/contrib/jquery-ui/jquery-ui.min.js
-xgee/core/contrib/jquery-ui/images/ui-icons_444444_256x240.png
-xgee/core/contrib/jquery-ui/images/ui-icons_555555_256x240.png
-xgee/core/contrib/jquery-ui/images/ui-icons_777620_256x240.png
-xgee/core/contrib/jquery-ui/images/ui-icons_777777_256x240.png
-xgee/core/contrib/jquery-ui/images/ui-icons_cc0000_256x240.png
-xgee/core/contrib/jquery-ui/images/ui-icons_ffffff_256x240.png
-xgee/core/css/UIComponents.canvasSearch.css
-xgee/core/css/app.css
-xgee/core/css/canvas.css
-xgee/core/css/contextmenu.css
-xgee/core/css/layout.css
-xgee/core/css/notes.css
-xgee/core/css/palette.css
-xgee/core/css/uiControls.css
-xgee/core/img/edit.svg
-xgee/core/img/eye.svg
-xgee/core/img/globe.svg
-xgee/core/img/graph-view-oaam-allocations.svg
-xgee/core/img/graph-view-oaam-functions.svg
-xgee/core/img/graph-view-oaam-hardware.svg
-xgee/core/img/redo.svg
-xgee/core/img/tool-domain-status-down.svg
-xgee/core/img/tool-domain-status-error.svg
-xgee/core/img/tool-domain-status-up-down.svg
-xgee/core/img/tool-domain-status-up.svg
-xgee/core/img/tool-domain-status.svg
-xgee/core/img/tree.svg
-xgee/core/img/undo.svg
-xgee/core/img/view-editor.svg
-xgee/core/js/DomainStatistics.js
-xgee/core/js/app.js
-xgee/core/js/commands.js
-xgee/core/js/ports.js
-xgee/core/js/connectors/connectors.graph.js
-xgee/core/js/connectors/connectors.selection.js
-xgee/core/js/grids/points_grid.svg
-xgee/core/js/ui/DomainStatusTool.js
-xgee/core/js/ui/ui.colorProvider.js
-xgee/core/js/workspace/workspace.jobs.js
-xgee/core/js/workspace/workspace.js
-xgee/core/jsa/.git
-xgee/core/jsa/CHANGELOG.md
-xgee/core/jsa/LICENSE
-xgee/core/jsa/README.md
-xgee/core/jsa/jsapplication.css
-xgee/core/jsa/jsapplication.js
-xgee/core/jsa/jsapplicationPlugins.js
-xgee/core/jsa/img/close-hover.svg
-xgee/core/jsa/img/close.svg
-xgee/core/jsa/img/jsa.svg
-xgee/core/jsa/img/loading.svg
-xgee/core/jsa/img/maximize.svg
-xgee/core/jsa/img/minimize.svg
-xgee/core/jsa/img/resize-ne.svg
-xgee/core/jsa/img/resize-nw.svg
-xgee/core/jsa/img/resize-se.svg
-xgee/core/jsa/img/resize-sw.svg
-xgee/core/jsa/img/restore.svg
-xgee/core/jsa/img/tool-default.svg
-xgee/core/jsa/img/view-close.svg
-xgee/core/jsa/img/black/bubble-hover.svg
-xgee/core/jsa/img/black/bubble.svg
-xgee/core/jsa/img/black/close-hover.svg
-xgee/core/jsa/img/black/close.svg
-xgee/core/jsa/img/black/folder.svg
-xgee/core/jsa/img/black/home.svg
-xgee/core/jsa/img/black/jsa.svg
-xgee/core/jsa/img/black/maximize-hover.svg
-xgee/core/jsa/img/black/maximize.svg
-xgee/core/jsa/img/black/menu-hover.svg
-xgee/core/jsa/img/black/menu.svg
-xgee/core/jsa/img/black/minimize-hover.svg
-xgee/core/jsa/img/black/minimize.svg
-xgee/core/jsa/img/black/redo.svg
-xgee/core/jsa/img/black/settings.svg
-xgee/core/jsa/img/black/undo.svg
-xgee/core/jsa/img/black/view-hover.svg
-xgee/core/jsa/img/black/view.svg
-xgee/core/jsa/img/white/bubble-hover.svg
-xgee/core/jsa/img/white/bubble.svg
-xgee/core/jsa/img/white/close-hover.svg
-xgee/core/jsa/img/white/close.svg
-xgee/core/jsa/img/white/folder.svg
-xgee/core/jsa/img/white/home.svg
-xgee/core/jsa/img/white/jsa.svg
-xgee/core/jsa/img/white/maximize-hover.svg
-xgee/core/jsa/img/white/maximize.svg
-xgee/core/jsa/img/white/menu-hover.svg
-xgee/core/jsa/img/white/menu.svg
-xgee/core/jsa/img/white/minimize-hover.svg
-xgee/core/jsa/img/white/minimize.svg
-xgee/core/jsa/img/white/redo.svg
-xgee/core/jsa/img/white/settings.svg
-xgee/core/jsa/img/white/undo.svg
-xgee/core/jsa/img/white/view-hover.svg
-xgee/core/jsa/img/white/view.svg
-xgee/core/mxgraph/LICENSE
-xgee/core/mxgraph/css/common.css
-xgee/core/mxgraph/css/explorer.css
-xgee/core/mxgraph/images/button.gif
-xgee/core/mxgraph/images/close.gif
-xgee/core/mxgraph/images/collapsed.gif
-xgee/core/mxgraph/images/error.gif
-xgee/core/mxgraph/images/expanded.gif
-xgee/core/mxgraph/images/maximize.gif
-xgee/core/mxgraph/images/minimize.gif
-xgee/core/mxgraph/images/normalize.gif
-xgee/core/mxgraph/images/point.gif
-xgee/core/mxgraph/images/resize.gif
-xgee/core/mxgraph/images/separator.gif
-xgee/core/mxgraph/images/submenu.gif
-xgee/core/mxgraph/images/transparent.gif
-xgee/core/mxgraph/images/warning.gif
-xgee/core/mxgraph/images/warning.png
-xgee/core/mxgraph/images/window-title.gif
-xgee/core/mxgraph/images/window.gif
-xgee/core/mxgraph/js/index.txt
-xgee/core/mxgraph/js/mxClient.js
-xgee/core/mxgraph/js/editor/mxDefaultKeyHandler.js
-xgee/core/mxgraph/js/editor/mxDefaultPopupMenu.js
-xgee/core/mxgraph/js/editor/mxDefaultToolbar.js
-xgee/core/mxgraph/js/editor/mxEditor.js
-xgee/core/mxgraph/js/handler/mxCellHighlight.js
-xgee/core/mxgraph/js/handler/mxCellMarker.js
-xgee/core/mxgraph/js/handler/mxCellTracker.js
-xgee/core/mxgraph/js/handler/mxConnectionHandler.js
-xgee/core/mxgraph/js/handler/mxConstraintHandler.js
-xgee/core/mxgraph/js/handler/mxEdgeHandler.js
-xgee/core/mxgraph/js/handler/mxEdgeSegmentHandler.js
-xgee/core/mxgraph/js/handler/mxElbowEdgeHandler.js
-xgee/core/mxgraph/js/handler/mxGraphHandler.js
-xgee/core/mxgraph/js/handler/mxHandle.js
-xgee/core/mxgraph/js/handler/mxKeyHandler.js
-xgee/core/mxgraph/js/handler/mxPanningHandler.js
-xgee/core/mxgraph/js/handler/mxPopupMenuHandler.js
-xgee/core/mxgraph/js/handler/mxRubberband.js
-xgee/core/mxgraph/js/handler/mxSelectionCellsHandler.js
-xgee/core/mxgraph/js/handler/mxTooltipHandler.js
-xgee/core/mxgraph/js/handler/mxVertexHandler.js
-xgee/core/mxgraph/js/io/mxCellCodec.js
-xgee/core/mxgraph/js/io/mxChildChangeCodec.js
-xgee/core/mxgraph/js/io/mxCodec.js
-xgee/core/mxgraph/js/io/mxCodecRegistry.js
-xgee/core/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
-xgee/core/mxgraph/js/io/mxDefaultPopupMenuCodec.js
-xgee/core/mxgraph/js/io/mxDefaultToolbarCodec.js
-xgee/core/mxgraph/js/io/mxEditorCodec.js
-xgee/core/mxgraph/js/io/mxGenericChangeCodec.js
-xgee/core/mxgraph/js/io/mxGraphCodec.js
-xgee/core/mxgraph/js/io/mxGraphViewCodec.js
-xgee/core/mxgraph/js/io/mxModelCodec.js
-xgee/core/mxgraph/js/io/mxObjectCodec.js
-xgee/core/mxgraph/js/io/mxRootChangeCodec.js
-xgee/core/mxgraph/js/io/mxStylesheetCodec.js
-xgee/core/mxgraph/js/io/mxTerminalChangeCodec.js
-xgee/core/mxgraph/js/layout/mxCircleLayout.js
-xgee/core/mxgraph/js/layout/mxCompactTreeLayout.js
-xgee/core/mxgraph/js/layout/mxCompositeLayout.js
-xgee/core/mxgraph/js/layout/mxEdgeLabelLayout.js
-xgee/core/mxgraph/js/layout/mxFastOrganicLayout.js
-xgee/core/mxgraph/js/layout/mxGraphLayout.js
-xgee/core/mxgraph/js/layout/mxParallelEdgeLayout.js
-xgee/core/mxgraph/js/layout/mxPartitionLayout.js
-xgee/core/mxgraph/js/layout/mxRadialTreeLayout.js
-xgee/core/mxgraph/js/layout/mxStackLayout.js
-xgee/core/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
-xgee/core/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
-xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
-xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
-xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
-xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
-xgee/core/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
-xgee/core/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
-xgee/core/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
-xgee/core/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
-xgee/core/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
-xgee/core/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
-xgee/core/mxgraph/js/model/mxCell.js
-xgee/core/mxgraph/js/model/mxCellPath.js
-xgee/core/mxgraph/js/model/mxGeometry.js
-xgee/core/mxgraph/js/model/mxGraphModel.js
-xgee/core/mxgraph/js/shape/mxActor.js
-xgee/core/mxgraph/js/shape/mxArrow.js
-xgee/core/mxgraph/js/shape/mxArrowConnector.js
-xgee/core/mxgraph/js/shape/mxCloud.js
-xgee/core/mxgraph/js/shape/mxConnector.js
-xgee/core/mxgraph/js/shape/mxCylinder.js
-xgee/core/mxgraph/js/shape/mxDoubleEllipse.js
-xgee/core/mxgraph/js/shape/mxEllipse.js
-xgee/core/mxgraph/js/shape/mxHexagon.js
-xgee/core/mxgraph/js/shape/mxImageShape.js
-xgee/core/mxgraph/js/shape/mxLabel.js
-xgee/core/mxgraph/js/shape/mxLine.js
-xgee/core/mxgraph/js/shape/mxMarker.js
-xgee/core/mxgraph/js/shape/mxPolyline.js
-xgee/core/mxgraph/js/shape/mxRectangleShape.js
-xgee/core/mxgraph/js/shape/mxRhombus.js
-xgee/core/mxgraph/js/shape/mxShape.js
-xgee/core/mxgraph/js/shape/mxStencil.js
-xgee/core/mxgraph/js/shape/mxStencilRegistry.js
-xgee/core/mxgraph/js/shape/mxSwimlane.js
-xgee/core/mxgraph/js/shape/mxText.js
-xgee/core/mxgraph/js/shape/mxTriangle.js
-xgee/core/mxgraph/js/util/mxAbstractCanvas2D.js
-xgee/core/mxgraph/js/util/mxAnimation.js
-xgee/core/mxgraph/js/util/mxAutoSaveManager.js
-xgee/core/mxgraph/js/util/mxClipboard.js
-xgee/core/mxgraph/js/util/mxConstants.js
-xgee/core/mxgraph/js/util/mxDictionary.js
-xgee/core/mxgraph/js/util/mxDivResizer.js
-xgee/core/mxgraph/js/util/mxDragSource.js
-xgee/core/mxgraph/js/util/mxEffects.js
-xgee/core/mxgraph/js/util/mxEvent.js
-xgee/core/mxgraph/js/util/mxEventObject.js
-xgee/core/mxgraph/js/util/mxEventSource.js
-xgee/core/mxgraph/js/util/mxForm.js
-xgee/core/mxgraph/js/util/mxGuide.js
-xgee/core/mxgraph/js/util/mxImage.js
-xgee/core/mxgraph/js/util/mxImageBundle.js
-xgee/core/mxgraph/js/util/mxImageExport.js
-xgee/core/mxgraph/js/util/mxLog.js
-xgee/core/mxgraph/js/util/mxMorphing.js
-xgee/core/mxgraph/js/util/mxMouseEvent.js
-xgee/core/mxgraph/js/util/mxObjectIdentity.js
-xgee/core/mxgraph/js/util/mxPanningManager.js
-xgee/core/mxgraph/js/util/mxPoint.js
-xgee/core/mxgraph/js/util/mxPopupMenu.js
-xgee/core/mxgraph/js/util/mxRectangle.js
-xgee/core/mxgraph/js/util/mxResources.js
-xgee/core/mxgraph/js/util/mxSvgCanvas2D.js
-xgee/core/mxgraph/js/util/mxToolbar.js
-xgee/core/mxgraph/js/util/mxUndoManager.js
-xgee/core/mxgraph/js/util/mxUndoableEdit.js
-xgee/core/mxgraph/js/util/mxUrlConverter.js
-xgee/core/mxgraph/js/util/mxUtils.js
-xgee/core/mxgraph/js/util/mxVmlCanvas2D.js
-xgee/core/mxgraph/js/util/mxWindow.js
-xgee/core/mxgraph/js/util/mxXmlCanvas2D.js
-xgee/core/mxgraph/js/util/mxXmlRequest.js
-xgee/core/mxgraph/js/view/mxCellEditor.js
-xgee/core/mxgraph/js/view/mxCellOverlay.js
-xgee/core/mxgraph/js/view/mxCellRenderer.js
-xgee/core/mxgraph/js/view/mxCellState.js
-xgee/core/mxgraph/js/view/mxCellStatePreview.js
-xgee/core/mxgraph/js/view/mxConnectionConstraint.js
-xgee/core/mxgraph/js/view/mxEdgeStyle.js
-xgee/core/mxgraph/js/view/mxGraph.js
-xgee/core/mxgraph/js/view/mxGraphSelectionModel.js
-xgee/core/mxgraph/js/view/mxGraphView.js
-xgee/core/mxgraph/js/view/mxLayoutManager.js
-xgee/core/mxgraph/js/view/mxMultiplicity.js
-xgee/core/mxgraph/js/view/mxOutline.js
-xgee/core/mxgraph/js/view/mxPerimeter.js
-xgee/core/mxgraph/js/view/mxPrintPreview.js
-xgee/core/mxgraph/js/view/mxStyleRegistry.js
-xgee/core/mxgraph/js/view/mxStylesheet.js
-xgee/core/mxgraph/js/view/mxSwimlaneManager.js
-xgee/core/mxgraph/js/view/mxTemporaryCellStates.js
-xgee/core/mxgraph/resources/editor.txt
-xgee/core/mxgraph/resources/editor_de.txt
-xgee/core/mxgraph/resources/editor_zh.txt
-xgee/core/mxgraph/resources/graph.txt
-xgee/core/mxgraph/resources/graph_de.txt
-xgee/core/mxgraph/resources/graph_zh.txt
+xgee/core/dep/bluebird/bluebird.js
+xgee/core/dep/bluebird/bluebird.min.js
+xgee/core/dep/font-awesome/LICENSE.txt
+xgee/core/dep/font-awesome/css/all.css
+xgee/core/dep/font-awesome/css/all.min.css
+xgee/core/dep/font-awesome/css/brands.css
+xgee/core/dep/font-awesome/css/brands.min.css
+xgee/core/dep/font-awesome/css/fontawesome.css
+xgee/core/dep/font-awesome/css/fontawesome.min.css
+xgee/core/dep/font-awesome/css/regular.css
+xgee/core/dep/font-awesome/css/regular.min.css
+xgee/core/dep/font-awesome/css/solid.css
+xgee/core/dep/font-awesome/css/solid.min.css
+xgee/core/dep/font-awesome/css/svg-with-js.css
+xgee/core/dep/font-awesome/css/svg-with-js.min.css
+xgee/core/dep/font-awesome/css/v4-shims.css
+xgee/core/dep/font-awesome/css/v4-shims.min.css
+xgee/core/dep/font-awesome/js/all.js
+xgee/core/dep/font-awesome/js/all.min.js
+xgee/core/dep/font-awesome/js/brands.js
+xgee/core/dep/font-awesome/js/brands.min.js
+xgee/core/dep/font-awesome/js/conflict-detection.js
+xgee/core/dep/font-awesome/js/conflict-detection.min.js
+xgee/core/dep/font-awesome/js/fontawesome.js
+xgee/core/dep/font-awesome/js/fontawesome.min.js
+xgee/core/dep/font-awesome/js/regular.js
+xgee/core/dep/font-awesome/js/regular.min.js
+xgee/core/dep/font-awesome/js/solid.js
+xgee/core/dep/font-awesome/js/solid.min.js
+xgee/core/dep/font-awesome/js/v4-shims.js
+xgee/core/dep/font-awesome/js/v4-shims.min.js
+xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot
+xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg
+xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf
+xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff
+xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2
+xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot
+xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg
+xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf
+xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff
+xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2
+xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot
+xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg
+xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf
+xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff
+xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2
+xgee/core/dep/jQuery-contextMenu-2.8/LICENSE
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js
+xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js
+xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot
+xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
+xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff
+xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
+xgee/core/dep/jquery/LICENSE.txt
+xgee/core/dep/jquery/jquery-3.3.1.min.js
+xgee/core/dep/jquery-ui/LICENSE.txt
+xgee/core/dep/jquery-ui/jquery-ui.min.css
+xgee/core/dep/jquery-ui/jquery-ui.min.js
+xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png
+xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png
+xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png
+xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png
+xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png
+xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png
+xgee/core/dep/jsa/.git
+xgee/core/dep/jsa/.gitignore
+xgee/core/dep/jsa/CHANGELOG.md
+xgee/core/dep/jsa/LICENSE
+xgee/core/dep/jsa/README.md
+xgee/core/dep/jsa/jsapplication.css
+xgee/core/dep/jsa/jsapplication.js
+xgee/core/dep/jsa/jsapplicationPlugins.js
+xgee/core/dep/jsa/package.json
+xgee/core/dep/jsa/webpack.config.js
+xgee/core/dep/jsa/img/close-hover.svg
+xgee/core/dep/jsa/img/close.svg
+xgee/core/dep/jsa/img/jsa.svg
+xgee/core/dep/jsa/img/loading.svg
+xgee/core/dep/jsa/img/maximize.svg
+xgee/core/dep/jsa/img/minimize.svg
+xgee/core/dep/jsa/img/resize-ne.svg
+xgee/core/dep/jsa/img/resize-nw.svg
+xgee/core/dep/jsa/img/resize-se.svg
+xgee/core/dep/jsa/img/resize-sw.svg
+xgee/core/dep/jsa/img/restore.svg
+xgee/core/dep/jsa/img/tool-default.svg
+xgee/core/dep/jsa/img/view-close.svg
+xgee/core/dep/jsa/img/black/bubble-hover.svg
+xgee/core/dep/jsa/img/black/bubble.svg
+xgee/core/dep/jsa/img/black/close-hover.svg
+xgee/core/dep/jsa/img/black/close.svg
+xgee/core/dep/jsa/img/black/folder.svg
+xgee/core/dep/jsa/img/black/home.svg
+xgee/core/dep/jsa/img/black/jsa.svg
+xgee/core/dep/jsa/img/black/maximize-hover.svg
+xgee/core/dep/jsa/img/black/maximize.svg
+xgee/core/dep/jsa/img/black/menu-hover.svg
+xgee/core/dep/jsa/img/black/menu.svg
+xgee/core/dep/jsa/img/black/minimize-hover.svg
+xgee/core/dep/jsa/img/black/minimize.svg
+xgee/core/dep/jsa/img/black/redo.svg
+xgee/core/dep/jsa/img/black/settings.svg
+xgee/core/dep/jsa/img/black/undo.svg
+xgee/core/dep/jsa/img/black/view-hover.svg
+xgee/core/dep/jsa/img/black/view.svg
+xgee/core/dep/jsa/img/white/bubble-hover.svg
+xgee/core/dep/jsa/img/white/bubble.svg
+xgee/core/dep/jsa/img/white/close-hover.svg
+xgee/core/dep/jsa/img/white/close.svg
+xgee/core/dep/jsa/img/white/folder.svg
+xgee/core/dep/jsa/img/white/home.svg
+xgee/core/dep/jsa/img/white/jsa.svg
+xgee/core/dep/jsa/img/white/maximize-hover.svg
+xgee/core/dep/jsa/img/white/maximize.svg
+xgee/core/dep/jsa/img/white/menu-hover.svg
+xgee/core/dep/jsa/img/white/menu.svg
+xgee/core/dep/jsa/img/white/minimize-hover.svg
+xgee/core/dep/jsa/img/white/minimize.svg
+xgee/core/dep/jsa/img/white/redo.svg
+xgee/core/dep/jsa/img/white/settings.svg
+xgee/core/dep/jsa/img/white/undo.svg
+xgee/core/dep/jsa/img/white/view-hover.svg
+xgee/core/dep/jsa/img/white/view.svg
+xgee/core/dep/mxgraph/LICENSE
+xgee/core/dep/mxgraph/css/common.css
+xgee/core/dep/mxgraph/css/explorer.css
+xgee/core/dep/mxgraph/images/button.gif
+xgee/core/dep/mxgraph/images/close.gif
+xgee/core/dep/mxgraph/images/collapsed.gif
+xgee/core/dep/mxgraph/images/error.gif
+xgee/core/dep/mxgraph/images/expanded.gif
+xgee/core/dep/mxgraph/images/maximize.gif
+xgee/core/dep/mxgraph/images/minimize.gif
+xgee/core/dep/mxgraph/images/normalize.gif
+xgee/core/dep/mxgraph/images/point.gif
+xgee/core/dep/mxgraph/images/resize.gif
+xgee/core/dep/mxgraph/images/separator.gif
+xgee/core/dep/mxgraph/images/submenu.gif
+xgee/core/dep/mxgraph/images/transparent.gif
+xgee/core/dep/mxgraph/images/warning.gif
+xgee/core/dep/mxgraph/images/warning.png
+xgee/core/dep/mxgraph/images/window-title.gif
+xgee/core/dep/mxgraph/images/window.gif
+xgee/core/dep/mxgraph/js/index.txt
+xgee/core/dep/mxgraph/js/mxClient.js
+xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js
+xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js
+xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js
+xgee/core/dep/mxgraph/js/editor/mxEditor.js
+xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js
+xgee/core/dep/mxgraph/js/handler/mxCellMarker.js
+xgee/core/dep/mxgraph/js/handler/mxCellTracker.js
+xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js
+xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js
+xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js
+xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js
+xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js
+xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js
+xgee/core/dep/mxgraph/js/handler/mxHandle.js
+xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js
+xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js
+xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js
+xgee/core/dep/mxgraph/js/handler/mxRubberband.js
+xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js
+xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js
+xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js
+xgee/core/dep/mxgraph/js/io/mxCellCodec.js
+xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js
+xgee/core/dep/mxgraph/js/io/mxCodec.js
+xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js
+xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
+xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js
+xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js
+xgee/core/dep/mxgraph/js/io/mxEditorCodec.js
+xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js
+xgee/core/dep/mxgraph/js/io/mxGraphCodec.js
+xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js
+xgee/core/dep/mxgraph/js/io/mxModelCodec.js
+xgee/core/dep/mxgraph/js/io/mxObjectCodec.js
+xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js
+xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js
+xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js
+xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js
+xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js
+xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js
+xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js
+xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js
+xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js
+xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js
+xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js
+xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js
+xgee/core/dep/mxgraph/js/layout/mxStackLayout.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
+xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
+xgee/core/dep/mxgraph/js/model/mxCell.js
+xgee/core/dep/mxgraph/js/model/mxCellPath.js
+xgee/core/dep/mxgraph/js/model/mxGeometry.js
+xgee/core/dep/mxgraph/js/model/mxGraphModel.js
+xgee/core/dep/mxgraph/js/shape/mxActor.js
+xgee/core/dep/mxgraph/js/shape/mxArrow.js
+xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js
+xgee/core/dep/mxgraph/js/shape/mxCloud.js
+xgee/core/dep/mxgraph/js/shape/mxConnector.js
+xgee/core/dep/mxgraph/js/shape/mxCylinder.js
+xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js
+xgee/core/dep/mxgraph/js/shape/mxEllipse.js
+xgee/core/dep/mxgraph/js/shape/mxHexagon.js
+xgee/core/dep/mxgraph/js/shape/mxImageShape.js
+xgee/core/dep/mxgraph/js/shape/mxLabel.js
+xgee/core/dep/mxgraph/js/shape/mxLine.js
+xgee/core/dep/mxgraph/js/shape/mxMarker.js
+xgee/core/dep/mxgraph/js/shape/mxPolyline.js
+xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js
+xgee/core/dep/mxgraph/js/shape/mxRhombus.js
+xgee/core/dep/mxgraph/js/shape/mxShape.js
+xgee/core/dep/mxgraph/js/shape/mxStencil.js
+xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js
+xgee/core/dep/mxgraph/js/shape/mxSwimlane.js
+xgee/core/dep/mxgraph/js/shape/mxText.js
+xgee/core/dep/mxgraph/js/shape/mxTriangle.js
+xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js
+xgee/core/dep/mxgraph/js/util/mxAnimation.js
+xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js
+xgee/core/dep/mxgraph/js/util/mxClipboard.js
+xgee/core/dep/mxgraph/js/util/mxConstants.js
+xgee/core/dep/mxgraph/js/util/mxDictionary.js
+xgee/core/dep/mxgraph/js/util/mxDivResizer.js
+xgee/core/dep/mxgraph/js/util/mxDragSource.js
+xgee/core/dep/mxgraph/js/util/mxEffects.js
+xgee/core/dep/mxgraph/js/util/mxEvent.js
+xgee/core/dep/mxgraph/js/util/mxEventObject.js
+xgee/core/dep/mxgraph/js/util/mxEventSource.js
+xgee/core/dep/mxgraph/js/util/mxForm.js
+xgee/core/dep/mxgraph/js/util/mxGuide.js
+xgee/core/dep/mxgraph/js/util/mxImage.js
+xgee/core/dep/mxgraph/js/util/mxImageBundle.js
+xgee/core/dep/mxgraph/js/util/mxImageExport.js
+xgee/core/dep/mxgraph/js/util/mxLog.js
+xgee/core/dep/mxgraph/js/util/mxMorphing.js
+xgee/core/dep/mxgraph/js/util/mxMouseEvent.js
+xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js
+xgee/core/dep/mxgraph/js/util/mxPanningManager.js
+xgee/core/dep/mxgraph/js/util/mxPoint.js
+xgee/core/dep/mxgraph/js/util/mxPopupMenu.js
+xgee/core/dep/mxgraph/js/util/mxRectangle.js
+xgee/core/dep/mxgraph/js/util/mxResources.js
+xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js
+xgee/core/dep/mxgraph/js/util/mxToolbar.js
+xgee/core/dep/mxgraph/js/util/mxUndoManager.js
+xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js
+xgee/core/dep/mxgraph/js/util/mxUrlConverter.js
+xgee/core/dep/mxgraph/js/util/mxUtils.js
+xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js
+xgee/core/dep/mxgraph/js/util/mxWindow.js
+xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js
+xgee/core/dep/mxgraph/js/util/mxXmlRequest.js
+xgee/core/dep/mxgraph/js/view/mxCellEditor.js
+xgee/core/dep/mxgraph/js/view/mxCellOverlay.js
+xgee/core/dep/mxgraph/js/view/mxCellRenderer.js
+xgee/core/dep/mxgraph/js/view/mxCellState.js
+xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js
+xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js
+xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js
+xgee/core/dep/mxgraph/js/view/mxGraph.js
+xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js
+xgee/core/dep/mxgraph/js/view/mxGraphView.js
+xgee/core/dep/mxgraph/js/view/mxLayoutManager.js
+xgee/core/dep/mxgraph/js/view/mxMultiplicity.js
+xgee/core/dep/mxgraph/js/view/mxOutline.js
+xgee/core/dep/mxgraph/js/view/mxPerimeter.js
+xgee/core/dep/mxgraph/js/view/mxPrintPreview.js
+xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js
+xgee/core/dep/mxgraph/js/view/mxStylesheet.js
+xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js
+xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js
+xgee/core/dep/mxgraph/resources/editor.txt
+xgee/core/dep/mxgraph/resources/editor_de.txt
+xgee/core/dep/mxgraph/resources/editor_zh.txt
+xgee/core/dep/mxgraph/resources/graph.txt
+xgee/core/dep/mxgraph/resources/graph_de.txt
+xgee/core/dep/mxgraph/resources/graph_zh.txt
+xgee/core/dep/notifyjs/LICENSE
+xgee/core/dep/notifyjs/notify.min.js
+xgee/core/dep/underscore/LICENSE
+xgee/core/dep/underscore/underscore-min.js
 xgee/core/plugins/autostart/plugin.js
 xgee/core/plugins/autostart/js/AppStartupEvent.js
 xgee/core/plugins/autostart/js/AppStartupObserver.js
 xgee/core/plugins/autostart/js/Autostarter.js
 xgee/core/plugins/clipboard/plugin.js
 xgee/core/plugins/clipboard/js/AppClipboard.js
 xgee/core/plugins/clipboard/js/Clipboard.js
@@ -751,14 +720,48 @@
 xgee/core/plugins/views/plugin.js
 xgee/core/plugins/views/js/ViewProvider.js
 xgee/core/plugins/views/js/ViewsController.js
 xgee/core/plugins/viewsMenu/plugin.js
 xgee/core/plugins/viewsMenu/js/ViewsMenuController.js
 xgee/core/plugins/viewsTabbar/plugin.js
 xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css
+xgee/core/res/css/UIComponents.canvasSearch.css
+xgee/core/res/css/app.css
+xgee/core/res/css/canvas.css
+xgee/core/res/css/contextmenu.css
+xgee/core/res/css/layout.css
+xgee/core/res/css/notes.css
+xgee/core/res/css/palette.css
+xgee/core/res/css/uiControls.css
+xgee/core/res/img/edit.svg
+xgee/core/res/img/eye.svg
+xgee/core/res/img/globe.svg
+xgee/core/res/img/graph-view-oaam-allocations.svg
+xgee/core/res/img/graph-view-oaam-functions.svg
+xgee/core/res/img/graph-view-oaam-hardware.svg
+xgee/core/res/img/redo.svg
+xgee/core/res/img/tool-domain-status-down.svg
+xgee/core/res/img/tool-domain-status-error.svg
+xgee/core/res/img/tool-domain-status-up-down.svg
+xgee/core/res/img/tool-domain-status-up.svg
+xgee/core/res/img/tool-domain-status.svg
+xgee/core/res/img/tree.svg
+xgee/core/res/img/undo.svg
+xgee/core/res/img/view-editor.svg
+xgee/core/res/js/DomainStatistics.js
+xgee/core/res/js/app.js
+xgee/core/res/js/commands.js
+xgee/core/res/js/ports.js
+xgee/core/res/js/connectors/connectors.graph.js
+xgee/core/res/js/connectors/connectors.selection.js
+xgee/core/res/js/grids/points_grid.svg
+xgee/core/res/js/ui/DomainStatusTool.js
+xgee/core/res/js/ui/ui.colorProvider.js
+xgee/core/res/js/workspace/workspace.jobs.js
+xgee/core/res/js/workspace/workspace.js
 xgee/eoqserver/PyEoq2WebServer.py
 xgee/eoqserver/__init__.py
 xgee/eoqserver/eoq1/__init__.py
 xgee/eoqserver/eoq1/commandparser.py
 xgee/eoqserver/eoq1/queryparser.py
 xgee/eoqserver/eoq1/resultparser.py
 xgee/eoqserver/eoq1/valueparser.py
```

### Comparing `XGEE-0.2.9/setup.py` & `XGEE-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/LICENSE` & `XGEE-0.3.0/xgee/core/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/bluebird.js` & `XGEE-0.3.0/xgee/core/dep/bluebird/bluebird.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/bluebird.min.js` & `XGEE-0.3.0/xgee/core/dep/bluebird/bluebird.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/LICENSE.txt` & `XGEE-0.3.0/xgee/core/dep/font-awesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/all.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/all.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/brands.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/brands.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/fontawesome.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/fontawesome.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/regular.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/regular.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/solid.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/solid.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/svg-with-js.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/svg-with-js.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/v4-shims.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/css/v4-shims.min.css` & `XGEE-0.3.0/xgee/core/dep/font-awesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/all.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/all.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/all.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/brands.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/brands.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/brands.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/brands.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/conflict-detection.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/conflict-detection.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/conflict-detection.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/conflict-detection.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/fontawesome.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/fontawesome.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/regular.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/regular.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/regular.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/regular.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/solid.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/solid.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/solid.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/v4-shims.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/v4-shims.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/js/v4-shims.min.js` & `XGEE-0.3.0/xgee/core/dep/font-awesome/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.eot` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.svg` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.ttf` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-brands-400.woff2` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.eot` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.svg` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.ttf` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-regular-400.woff2` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.eot` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.svg` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.ttf` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/font-awesome/webfonts/fa-solid-900.woff2` & `XGEE-0.3.0/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/LICENSE` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.eot` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.ttf` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/font/context-menu-icons.woff2` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.css` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.js` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.js` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jQuery-contextMenu-2.8/jquery.ui.position.min.js` & `XGEE-0.3.0/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery/LICENSE.txt` & `XGEE-0.3.0/xgee/core/dep/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery/jquery-3.3.1.min.js` & `XGEE-0.3.0/xgee/core/dep/jquery/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/LICENSE.txt` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_444444_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_555555_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_777620_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_777777_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_cc0000_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/images/ui-icons_ffffff_256x240.png` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/jquery-ui.min.css` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/jquery-ui/jquery-ui.min.js` & `XGEE-0.3.0/xgee/core/dep/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/notify.min.js` & `XGEE-0.3.0/xgee/core/dep/notifyjs/notify.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/underscore-LICENSE` & `XGEE-0.3.0/xgee/core/dep/underscore/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/contrib/underscore-min.js` & `XGEE-0.3.0/xgee/core/dep/underscore/underscore-min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/css/app.css` & `XGEE-0.3.0/xgee/core/res/css/app.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/css/contextmenu.css` & `XGEE-0.3.0/xgee/core/res/css/contextmenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/css/notes.css` & `XGEE-0.3.0/xgee/core/res/css/notes.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/css/palette.css` & `XGEE-0.3.0/xgee/core/res/css/palette.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/css/uiControls.css` & `XGEE-0.3.0/xgee/core/res/css/uiControls.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/edit.svg` & `XGEE-0.3.0/xgee/core/res/img/edit.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/eye.svg` & `XGEE-0.3.0/xgee/core/res/img/eye.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/globe.svg` & `XGEE-0.3.0/xgee/core/res/img/globe.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/graph-view-oaam-allocations.svg` & `XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-allocations.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/graph-view-oaam-functions.svg` & `XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-functions.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/graph-view-oaam-hardware.svg` & `XGEE-0.3.0/xgee/core/res/img/graph-view-oaam-hardware.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/redo.svg` & `XGEE-0.3.0/xgee/core/res/img/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tool-domain-status-down.svg` & `XGEE-0.3.0/xgee/core/res/img/tool-domain-status-down.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tool-domain-status-error.svg` & `XGEE-0.3.0/xgee/core/res/img/tool-domain-status-error.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tool-domain-status-up-down.svg` & `XGEE-0.3.0/xgee/core/res/img/tool-domain-status-up-down.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tool-domain-status-up.svg` & `XGEE-0.3.0/xgee/core/res/img/tool-domain-status-up.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tool-domain-status.svg` & `XGEE-0.3.0/xgee/core/res/img/tool-domain-status.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/tree.svg` & `XGEE-0.3.0/xgee/core/res/img/tree.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/undo.svg` & `XGEE-0.3.0/xgee/core/res/img/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/img/view-editor.svg` & `XGEE-0.3.0/xgee/core/res/img/view-editor.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/DomainStatistics.js` & `XGEE-0.3.0/xgee/core/res/js/DomainStatistics.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/app.js` & `XGEE-0.3.0/xgee/core/res/js/app.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/commands.js` & `XGEE-0.3.0/xgee/core/res/js/commands.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/connectors/connectors.graph.js` & `XGEE-0.3.0/xgee/core/res/js/connectors/connectors.graph.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/connectors/connectors.selection.js` & `XGEE-0.3.0/xgee/core/res/js/connectors/connectors.selection.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/ports.js` & `XGEE-0.3.0/xgee/core/res/js/ports.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/ui/DomainStatusTool.js` & `XGEE-0.3.0/xgee/core/res/js/ui/DomainStatusTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/ui/ui.colorProvider.js` & `XGEE-0.3.0/xgee/core/res/js/ui/ui.colorProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/workspace/workspace.jobs.js` & `XGEE-0.3.0/xgee/core/res/js/workspace/workspace.jobs.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/js/workspace/workspace.js` & `XGEE-0.3.0/xgee/core/res/js/workspace/workspace.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/CHANGELOG.md` & `XGEE-0.3.0/xgee/core/dep/jsa/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # jsApplication Changelog
 
+### v0.6.2
+* Ambiguous check property of CheckboxCtrl and RadioCtrl removed (use value instead)
+* titleAttr property introduced for most elements, which sets the HTML title attribute of the DOM element
+* minify npm script added (minify is triggered manually by "npm run pack" in folder jsa)
+* documentation generation changed to npm script. Run "npm doc"
+* Slight improvments of the HTML examples and HTML example added that uses the minified js and css
+
 ### v0.6.1
 * Transparent menus and popups introduced (uses backdropFilter, which is disabled in the current firefox by default. Can be enabled in the settings)
 * Visual adaptation of tabs: inactive tabs are now partially transparent
 * Visual adaptation of the application tabbar: is now borderless
 * Made view header high equal to tabbar height, which looks better by default
 * Various CSS simplifications especially for tabs and popup arrows
```

### Comparing `XGEE-0.2.9/xgee/core/jsa/LICENSE` & `XGEE-0.3.0/xgee/core/dep/jsa/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/README.md` & `XGEE-0.3.0/xgee/core/dep/jsa/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/bubble-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/bubble-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/bubble.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/bubble.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/close-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/close.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/folder.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/folder.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/home.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/home.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/jsa.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/maximize-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/maximize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/maximize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/menu-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/menu-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/menu.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/menu.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/minimize-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/minimize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/minimize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/redo.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/settings.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/settings.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/undo.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/view-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/view-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/black/view.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/black/view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/close-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/close.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/jsa.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/loading.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/loading.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/maximize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/minimize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/resize-ne.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/resize-ne.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/resize-nw.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/resize-nw.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/resize-se.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/resize-se.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/resize-sw.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/resize-sw.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/restore.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/restore.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/tool-default.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/tool-default.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/view-close.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/view-close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/bubble-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/bubble-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/bubble.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/bubble.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/close-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/close.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/folder.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/folder.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/home.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/home.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/jsa.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/maximize-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/maximize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/maximize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/menu-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/menu-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/menu.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/menu.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/minimize-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/minimize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/minimize.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/redo.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/settings.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/settings.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/undo.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/view-hover.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/view-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/img/white/view.svg` & `XGEE-0.3.0/xgee/core/dep/jsa/img/white/view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/jsapplication.css` & `XGEE-0.3.0/xgee/core/dep/jsa/jsapplication.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/jsa/jsapplication.js` & `XGEE-0.3.0/xgee/core/dep/jsa/jsapplication.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
      * The current version of jsApplication
      * @var {string} VERSION
      * 
      * @example
      * // Get the jsa version
      * let v = jsa.VERSION;
      */
-    let VERSION = '0.6.1';
+    let VERSION = '0.6.2';
 
     /**
      * The maximum level of nesting in menus
      * @var {int} MAX_MENU_POPUP_LEVEL
      * 
      * @example
      * // Get the maximum menu level
@@ -493,28 +493,32 @@
 
     /**
      * This encapsulates document.createElement(...) by simultaneously 
      * creating an HTML DOM element and setting its 'id' property to
      * either a specified ID or a random ID (s. GenerateId()).
      * @function CreateDomElementWithUniqueId
      * @param {string} elementType - The tag type to be created. 
-     * @param {string} id='' - (optional) The id to be used for the new DOM element
+     * @param {string} id=null - (optional) The id to be used for the new DOM element
+     * @param {string} title=null - (optional) Sets the HTML title attribute to this value
      * @returns {HTML_DOM_ELEMENT} The new HTML DOM element
      *
      * @example
      * let domWithCustomId = jsa.CreateDomElementWithUniqueId("div","my_new_dom_element"); 
      * let domWithRandomId = jsa.CreateDomElementWithUniqueId("div"); 
      */
-    function CreateDomElementWithUniqueId(elementType, id = '') {
+    function CreateDomElementWithUniqueId(elementType, id = null, title = null) {
         let domElement = document.createElement(elementType);
         if (id) {
             domElement.id = id;
         } else {
             domElement.id = GenerateId();
         }
+        if (title) {
+            domElement.title = title;
+        }
         return domElement;
     };
 
 
     /* OBSERVABLE */
     /**
      * @class Observable
@@ -937,14 +941,15 @@
      * @property {string} params.id=(random) - The id of the related DOM element.
      * @property {string} params.name='' - The name of the element.
      * @property {Object} params.data=null - Any user data to be attached to the element, e.g. for the use in callbacks.
      * @property {boolean} params.startVisible=true - Whether the element shall be visible after creation.
      * @property {boolean} params.startEnabled=true - Whether the element shall be enabled after creation.
      * @property {boolean} params.hasTooltip=false - Whether the element shall show a tooltip on mouseover or not.
      * @property {string} params.tooltip='' - The tooltip text
+     * @property {string} params.titleAttr=null - The HTML title attribute of the HTML DOM element 
      * @comment UIElementA internals
      * @property {HTML_DOM_ELEMENT} this.domElement - (readonly) The HTML DOM element as attached to the document tree. This ensures compatibility to any other js library or function. Usually, this should not be accessed directly. Use [GetDomElement()]{@link UIElement#GetDomElement} instead.
      * @property {Application} this.app - (readonly) The jsa.Application object this element belongs to. This will be filled as soon as this object was added to an Application or any other element, which is a child of an application. Otherwise it is null.
      * @property {UIElementA} this.parent - (readonly) The parent element this element belongs to. This is set after adding it to a parent using AddChild(). Otherwise it is null.
      * @property {int} this.level=0 - (readonly) Indicates the level of nesting this UI element is currently in. The application itself has level 0. Every direct child level 1 and so on.
      * @property {HTML_STYLE_OBJECT} this.defaultDisplayStyle - (readonly) Internally used to store the original style of the corresponding HTML element during show and hide operations. Do not change it manually.
      * @property {boolean} this.isVisible - (readonly) The current state of visibility.
@@ -960,14 +965,15 @@
         this.id = GenerateId();
         this.name = '';
         this.data = null; //user data
         this.startEnabled = true;
         this.startVisible = true;
         this.hasTooltip = false;
         this.tooltip = '';
+        this.titleAttr = null;
 
         //internals
         /**
          * @private
          */
         this.domElement = {};
         this.app = null;
@@ -1410,16 +1416,15 @@
      * Creates the HTML DOM element. In general, CreateDom is called automatically by the constructor. 
      * Please see [UIElementA.CreateDom]{@link UIElementA#CreateDom} for the general explanation.
      * In this case it creates the DOM element, sets the content, and registers event listeners 
      * @returns {this} Instance of the element itself to enable method chaining
      * @method CustomUiElement.prototype.CreateDom
      */
     CustomUiElement.prototype.CreateDom = function() {
-        this.domElement = CreateDomElementWithUniqueId(this.elementType);
-        this.domElement.id = this.id;
+        this.domElement = CreateDomElementWithUniqueId(this.elementType, this.id, this.titleAttr);
         this.SetStyle(this.style);
         this.SetContent(this.content);
 
         if ('a' == this.elementType && this.href) {
             this.domElement.href = this.href;
         }
         if (this.onClickCallback) {
@@ -2863,15 +2868,14 @@
      *
      * @param {dict} params=(see_below) - A dictionary of initialization parameters. Below for details.
      * @param {boolean} createDom=true - To be used for inheritance of jsa elements. If set to false the HTML DOM element will not be created, e.g. CreateDom() is not called.
      *
      * @comment CheckboxCtrl parameters
      * @property {boolean} params.value=false - The initial value that defines the state of the checkbox. True is checked.
      * @property {string} params.name='' - A unique identifier string which is equal for all checkboxes of the same group.
-     * @property {boolean} params.checked=false - Whether the checkbox is checked on creation of not.
      * @property {boolean} params.readonly=false - Whether the user can change the checkbox or not. 
      * @property {string} params.elementType='div' - The DOM element type of the outer DOM element. The default is div.
      * @property {Array.<string>} params.style=['jsa-checkbox-ctrl']] - The CSS styles for the outer DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.ctrlStyle=['jsa-checkbox-ctrl-input']] - The CSS styles for the radio DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.labelStyle=['jsa-checkbox-ctrl-label']] - The CSS styles for the label DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.errorIndicatorStyle=['jsa-checkbox-ctrl-error-indication']] - The CSS styles for the error indication DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {function} params.onChangeCallback - This function is called if the value of the checkbox changes by user interaction.
@@ -2880,29 +2884,29 @@
      * @constructor CheckboxCtrl
      * @extends CustomUiElement
      * 
      * @example
      * app = new jsa.Application({});
      * myCheckboxCtrl = new jsa.CheckboxCtrl({
      *   content:'Check me if you like', 
+     *   name: 'my-check-group',
      *   onChangeCallback:function(evt) {
-     *     if(this.checked) {
-     *      alert('I knew you like me!');
+     *     if(this.GetValue()) {
+     *      alert('I know you like me!');
      *     }
      *   }
      * });
      * app.AddChild(myCheckboxCtrl); 
      */
     function CheckboxCtrl(params = {}, createDom = true) {
         CustomUiElement.call(this, params, false);
 
         //members
         this.value = false;
         this.name = '';
-        this.checked = false;
         this.readonly = false;
         this.style = ['jsa-checkbox-ctrl'];
         this.ctrlStyle = ['jsa-checkbox-ctrl-input'];
         this.labelStyle = ['jsa-checkbox-ctrl-label'];
         this.errorIndicatorStyle = ['jsa-checkbox-ctrl-error-indication'];
         this.onChangeCallback = function(event) {};
 
@@ -2930,18 +2934,19 @@
         this.input = document.createElement('input');
         ApplyStyles(this.ctrlStyle, this.input)
         if (this.readonly || !this.isEnabled) {
             this.Disable();
         }
         this.input.type = 'checkbox';
         this.input.name = this.name;
-        this.input.checked = this.checked;
+        this.input.id = this.id + 'Input';
         this.domElement.appendChild(this.input);
 
         this.label = document.createElement('label');
+        this.label.setAttribute("for", this.id + 'Input');
         ApplyStyles(this.labelStyle, this.label);
         this.label.innerHTML = this.content;
         this.domElement.appendChild(this.label);
 
         this.errorIndicator = document.createElement('small');
         ApplyStyles(this.errorIndicatorStyle, this.errorIndicator);
         this.domElement.appendChild(this.errorIndicator);
@@ -2977,29 +2982,29 @@
      * @example
      * // ... continuing CheckboxCtrl general example
      * myCheckboxCtrl.SetValue(true); //-> Check mark shows up
      * myCheckboxCtrl.SetValue(true); //-> Check disappears 
      */
     CheckboxCtrl.prototype.SetValue = function(value) {
         let boolValue = value ? true : false
-        this.checked = boolValue;
+        this.value = boolValue;
         this.input.checked = boolValue; //mask non bool values
         return this;
     };
 
     /**
      * Sets the checked state of the checkbox without any processing, 
      * but optionally allows cause regular change events.
      * @param {boolean} boolValue - True to set the box checked and false to uncheck.
      * @param {boolean} notify - If true, an on change event will be caused.
      * @returns {this} Instance of the element itself to enable method chaining
      * @method CheckboxCtrl.prototype.SetRawValue
      */
     CheckboxCtrl.prototype.SetRawValue = function(boolValue, notify = false) {
-        this.checked = boolValue;
+        this.value = boolValue;
         this.input.checked = boolValue; //mask non bool values
         if (notify) {
             this.input.dispatchEvent(new Event('change', {
                 'bubbles': true
             })); /* Event is the JS event not jsa */
         }
         return this;
@@ -3075,15 +3080,14 @@
      * 
      * @param {dict} params=(see_below) - A dictionary of initialization parameters. Below for details.
      * @param {boolean} [createDom=true] - To be used for inheritance of jsa elements. If set to false the HTML DOM element will not be created, e.g. CreateDom() is not called.
      *
      * @comment RadioCtrl parameters
      * @property {boolean} params.value=false - True the radio button is checked. False it is not.
      * @property {string} params.name='' - A unique group identification for the radio button. From all radio buttons in one group, only one can be active.
-     * @property {boolean} params.checked=false - Whether the radio button starts in the checked state or not.
      * @property {boolean} params.readonly=false - If true, the radio button is passive. If false it can be changed by the user.
      * @property {string} params.elementType='div' - The DOM element type of the surrounding DOM element.
      * @property {Array.<string>} params.style=['jsa-radio-ctrl']] - The CSS styles for the outer DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.ctrlStyle=['jsa-radio-ctrl-input']] - The CSS styles for the radio DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.labelStyle=['jsa-radio-ctrl-label']] - The CSS styles for the label DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {Array.<string>} params.errorIndicatorStyle=['jsa-radio-ctrl-error-indication']] - The CSS styles for the error indication DOM element. See [CustomUiElement]{@link CustomUiElement} for details on style arrays.
      * @property {function} params.onChangeCallback - This function is called if the value of the radio button changes by user interaction.
@@ -3093,34 +3097,33 @@
      * @extends CustomUiElement
      * 
      * @example
      * // Create a radio group with two buttons of that only one can be active
      * app = new jsa.Application({});
      * myRadio1 = new jsa.RadioCtrl({
      *   content:'Radio 1',
-     *   group:'my-radio-group',
+     *   name:'my-radio-group',
      *   onChangeCallback:function(evt) {
-     *     if(this.checked) {
+     *     if(this.GetValue()) {
      *      alert('First radio button is active');
      *     }
      *   }
      * });
      * myRadio2 = new jsa.RadioCtrl({
      *   content:'Radio 2',
-     *   group:'my-radio-group'
+     *   name:'my-radio-group'
      * });
      * app.AddChild(myRadio1); 
      * app.AddChild(myRadio2); 
      */
     function RadioCtrl(params = {}, createDom = true) {
         CustomUiElement.call(this, params, false);
 
         //members
         this.value = false;
-        this.checked = false;
         this.readonly = false;
         this.elementType = 'div';
         this.style = ['jsa-radio-ctrl'];
         this.ctrlStyle = ['jsa-radio-ctrl-input'];
         this.labelStyle = ['jsa-radio-ctrl-label'];
         this.errorIndicatorStyle = ['jsa-radio-ctrl-error-indication'];
         this.onChangeCallback = function(event) {};
@@ -3149,18 +3152,19 @@
         this.input = document.createElement('input');
         ApplyStyles(this.ctrlStyle, this.input)
         if (this.readonly || !this.isEnabled) {
             this.Disable();
         }
         this.input.type = 'radio';
         this.input.name = this.name;
-        this.input.checked = this.checked;
+        this.input.id = this.id + 'Input'; // add html id to radiobox
         this.domElement.appendChild(this.input);
 
         this.label = document.createElement('label');
+        this.label.setAttribute("for", this.id + 'Input'); // set for-attribute
         ApplyStyles(this.labelStyle, this.label);
         this.label.innerHTML = this.content;
         this.domElement.appendChild(this.label);
 
         this.errorIndicator = document.createElement('small');
         ApplyStyles(this.errorIndicatorStyle, this.errorIndicator);
         this.domElement.appendChild(this.errorIndicator);
@@ -3197,29 +3201,29 @@
      * @example
      * // ...continuing general RadioCtrlExample
      * myRadio1.GetValue(true);
      * let status = myRadio2.GetValue(); //must be false
      */
     RadioCtrl.prototype.SetValue = function(value) {
         let boolValue = value ? true : false
-        this.checked = boolValue;
+        this.value = boolValue;
         this.input.checked = boolValue; //mask non bool values
         return this;
     };
 
     /**
      * Sets the checked state of the radio input without any processing, 
      * but optionally allows cause regular change events.
      * @param {boolean} boolValue - True to marks the radio input checked and false unmarks it.
      * @param {boolean} notify - If true, an on change event will be caused.
      * @returns {this} Instance of the element itself to enable method chaining
      * @method RadioCtrl.prototype.SetRawValue
      */
     RadioCtrl.prototype.SetRawValue = function(boolValue, notify = false) {
-        this.checked = boolValue;
+        this.value = boolValue;
         this.input.checked = boolValue; //mask non bool values
         if (notify) {
             this.input.dispatchEvent(new Event('change', {
                 'bubbles': true
             })); /* Event is the JS event not jsa */
         }
         return this;
@@ -8507,8 +8511,10 @@
         Progressbar: Progressbar,
         Selection: Selection,
         SelectionManager: SelectionManager,
         SettingsManager: SettingsManager,
         Application: Application
     };
 
-})();
+})();
+
+window.jsa = jsa; //make sure jsa is not removed during minify
```

### Comparing `XGEE-0.2.9/xgee/core/jsa/jsapplicationPlugins.js` & `XGEE-0.3.0/xgee/core/dep/jsa/jsapplicationPlugins.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/LICENSE` & `XGEE-0.3.0/xgee/core/dep/mxgraph/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/css/common.css` & `XGEE-0.3.0/xgee/core/dep/mxgraph/css/common.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/images/collapsed.gif` & `XGEE-0.3.0/xgee/core/dep/mxgraph/images/collapsed.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/images/error.gif` & `XGEE-0.3.0/xgee/core/dep/mxgraph/images/error.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/images/expanded.gif` & `XGEE-0.3.0/xgee/core/dep/mxgraph/images/expanded.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/images/maximize.gif` & `XGEE-0.3.0/xgee/core/dep/mxgraph/images/maximize.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/images/normalize.gif` & `XGEE-0.3.0/xgee/core/dep/mxgraph/images/normalize.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultKeyHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultPopupMenu.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxDefaultToolbar.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/editor/mxEditor.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/editor/mxEditor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellHighlight.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellMarker.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxCellTracker.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxConnectionHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxConstraintHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxEdgeHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxEdgeSegmentHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxElbowEdgeHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxGraphHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxHandle.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxHandle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxKeyHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxPanningHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxPopupMenuHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxRubberband.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxRubberband.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxSelectionCellsHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxTooltipHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/handler/mxVertexHandler.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/index.txt` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/index.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCellCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCellCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxChildChangeCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxCodecRegistry.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultKeyHandlerCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultPopupMenuCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxDefaultToolbarCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxEditorCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGenericChangeCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGraphCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxGraphViewCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxModelCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxModelCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxObjectCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxRootChangeCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxStylesheetCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/io/mxTerminalChangeCodec.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCircleLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCompactTreeLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxCompositeLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxEdgeLabelLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxFastOrganicLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxGraphLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxParallelEdgeLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxPartitionLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxRadialTreeLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/layout/mxStackLayout.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/model/mxCell.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxCell.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/model/mxCellPath.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxCellPath.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/model/mxGeometry.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxGeometry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/model/mxGraphModel.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/model/mxGraphModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/mxClient.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/mxClient.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxActor.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxActor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxArrow.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxArrow.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxArrowConnector.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxCloud.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxCloud.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxConnector.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxConnector.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxCylinder.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxCylinder.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxDoubleEllipse.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxEllipse.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxEllipse.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxHexagon.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxHexagon.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxImageShape.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxImageShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxLabel.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxLabel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxLine.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxLine.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxMarker.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxMarker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxPolyline.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxPolyline.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxRectangleShape.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxRhombus.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxRhombus.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxShape.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxStencil.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxStencil.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxStencilRegistry.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxSwimlane.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxText.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxText.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/shape/mxTriangle.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/shape/mxTriangle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAbstractCanvas2D.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAnimation.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAnimation.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxAutoSaveManager.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxClipboard.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxClipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxConstants.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxConstants.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDictionary.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDictionary.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDivResizer.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDivResizer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxDragSource.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxDragSource.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEffects.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEffects.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEvent.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEventObject.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEventObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxEventSource.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxEventSource.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxForm.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxForm.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxGuide.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxGuide.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImage.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImage.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImageBundle.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImageBundle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxImageExport.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxImageExport.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxLog.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxLog.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxMorphing.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxMorphing.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxMouseEvent.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxObjectIdentity.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPanningManager.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPanningManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPoint.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPoint.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxPopupMenu.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxRectangle.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxRectangle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxResources.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxResources.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxSvgCanvas2D.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxToolbar.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxToolbar.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUndoManager.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUndoManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUndoableEdit.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUrlConverter.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxUtils.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxUtils.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxVmlCanvas2D.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxWindow.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxWindow.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxXmlCanvas2D.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/util/mxXmlRequest.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellEditor.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellEditor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellOverlay.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellRenderer.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellState.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellState.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxCellStatePreview.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxConnectionConstraint.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxEdgeStyle.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraph.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraph.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraphSelectionModel.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxGraphView.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxGraphView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxLayoutManager.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxMultiplicity.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxOutline.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxOutline.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxPerimeter.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxPerimeter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxPrintPreview.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxStyleRegistry.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxStylesheet.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxStylesheet.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxSwimlaneManager.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/mxgraph/js/view/mxTemporaryCellStates.js` & `XGEE-0.3.0/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/autostart/js/AppStartupEvent.js` & `XGEE-0.3.0/xgee/core/plugins/autostart/js/AppStartupEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/autostart/js/AppStartupObserver.js` & `XGEE-0.3.0/xgee/core/plugins/autostart/js/AppStartupObserver.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/autostart/js/Autostarter.js` & `XGEE-0.3.0/xgee/core/plugins/autostart/js/Autostarter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/autostart/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/autostart/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/AppClipboard.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/AppClipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/Clipboard.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/Clipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardAPI.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardAPI.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/ClipboardManager.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/ClipboardManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/clipboard/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/clipboard/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu/js/ContextMenu.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu/js/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu/js/util.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu/js/util.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu.ecore/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/js/util.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/js/util.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/contextMenu.eoq/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/contextMenu.eoq/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/ecore/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/ecore.xmi.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/ecore.xmi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/README.md` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/example.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/example.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/examples/test.xml` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/examples/test.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/lib/sax.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/lib/sax.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/package-lock.json` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/package-lock.json`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/package.json` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/package.json`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/bom.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/bom.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/case.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/case.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/index.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/index.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/script.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/script.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js` & `XGEE-0.3.0/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/changes/esChanges.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/changes/esChanges.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/esDebugging.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/esDebugging.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/dev/lib/libesync.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/dev/lib/libesync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esDomain.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esDomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esLookup.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esLookup.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esMetaSync.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esMetaSync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/ecoreSync.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/ecoreSync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/interfaces/esInstance.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/interfaces/esInstance.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueries.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueries.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -114,19 +114,19 @@
                 if (seg) {
                     v = seg.v
                 }
 
                 try {
                     res = await evalFunction(context, v, scope, eoqHistory, callback)
                 } catch (e) {
-                    console.error('Failed to evaluate segment. An error occured in the evaluation function ' + evalFunction.name + ': ' + e)
+                    if ($DEBUG) console.debug('Failed to evaluate segment. An error occured in the evaluation function ' + evalFunction.name + ': ' + e)
                     throw e
                 }
             } catch (e) {
-                console.error("Segment type error type:" + t + " " + e);
+                if ($DEBUG) console.debug("Segment type error type:" + t + " " + e);
                 throw e
             }
         }
 
         return res
 
 
@@ -155,15 +155,15 @@
 
                 }
                 return res
             }
             try {
                 res = await ApplyToAllElements(context, pathFunctor)
             } catch (e) {
-                console.error("Error evaluating path segment " + name + ": " + e)
+                if ($DEBUG) console.debug("Error evaluating path segment " + name + ": " + e)
                 throw e
             }
         }
         return res
     }
 
     async EvalAny(context, args, scope, eoqHistory, callback) {
@@ -236,15 +236,15 @@
             }, (change) => {
                 return relevantReferenceNames.includes(change.data[3])
             })
 
             try {
                 res = await ApplyToAllElements(context, clsFunctor)
             } catch (e) {
-                console.error("Error evaluating class segment " + name + ": " + e)
+                if ($DEBUG) console.debug("Error evaluating class segment " + name + ": " + e)
                 throw e
             }
         }
         return res
     }
 
     async EvalIno(context, name, scope, eoqHistory, callback) {
@@ -282,15 +282,15 @@
         }, (change) => {
             return relevantReferenceNames.includes(change.data[3])
         })
 
         try {
             res = await ApplyToAllElements(context, inoFunctor)
         } catch (e) {
-            console.error("Error evaluating INO segment " + name + ": " + e)
+            if ($DEBUG) console.debug("Error evaluating INO segment " + name + ": " + e)
             throw e
         }
         return res
     }
 
 
     async EvalTrm(context, args, scope, eoqHistory, callback) {
@@ -444,27 +444,27 @@
         var select = null
         try {
             select = await this.EvalOnContextAndScope(context, args, context, eoqHistory, function(select) {
                 var res = [];
                 try {
                     res = ApplyToSimilarListsOfObjects(context, select, SelListVsListFunc, SelListVsStructFunc, SelStructVsListFunc)
                 } catch (e) {
-                    console.error("Failed evaluating selector during callback: " + args + ". Selectors context and argument must be arrays of similar structure. Argument must be either be an array of Bool, but got " + select + ": " + e)
+                    if ($DEBUG) console.debug("Failed evaluating selector during callback: " + args + ". Selectors context and argument must be arrays of similar structure. Argument must be either be an array of Bool, but got " + select + ": " + e)
                     throw e
                 }
                 callback(res) //callback toward parent           
             })
         } catch (e) {
-            console.error('Select evaluation failed: ' + e)
+            if ($DEBUG) console.debug('Select evaluation failed: ' + e)
         }
 
         try {
             res = ApplyToSimilarListsOfObjects(context, select, SelListVsListFunc, SelListVsStructFunc, SelStructVsListFunc)
         } catch (e) {
-            console.error("Failed evaluating selector " + args + ". Selectors context and argument must be arrays of similar structure. Argument must be either be an array of Bool, but got " + select + ": " + e)
+            if ($DEBUG) console.debug("Failed evaluating selector " + args + ". Selectors context and argument must be arrays of similar structure. Argument must be either be an array of Bool, but got " + select + ": " + e)
             throw e
         }
 
         return res
     }
 
     async EvalEqu(context, args, scope, eoqHistory, callback) {
@@ -558,23 +558,34 @@
             }
             callback(res);
         })
 
 
         //Observe segments
         var res = null;
-        res = await this.EvalOnContextAndScope(context, args[2], context, eoqHistory, async (res) => {
-            let condition = await EvalOnContextAndScope(context, args[1], context, eoqHistory);
-            if (condition) callback(res);
-        })
 
-        res = await this.EvalOnContextAndScope(context, args[3], context, eoqHistory, async (res) => {
-            let condition = await EvalOnContextAndScope(context, args[1], context, eoqHistory);
-            if (!condition) callback(res);
-        })
+        try {
+            res = await this.EvalOnContextAndScope(context, args[2], context, eoqHistory, async (res) => {
+                let condition = await EvalOnContextAndScope(context, args[1], context, eoqHistory);
+                if (condition) callback(res);
+            })
+        } catch (error) {
+            if (condition) throw error
+            if ($DEBUG) console.debug("@IF: Errors of observing inactive query have been suppressed. This is the intended behavior. Context: " + JSON.stringify(context) + " Query: " + args[2].toString() + " Error: " + error)
+        }
+
+        try {
+            res = await this.EvalOnContextAndScope(context, args[3], context, eoqHistory, async (res) => {
+                let condition = await EvalOnContextAndScope(context, args[1], context, eoqHistory);
+                if (!condition) callback(res);
+            })
+        } catch (error) {
+            if (!condition) throw error
+            if ($DEBUG) console.debug("@IF: Errors of observing inactive query have been suppressed. This is the intended behavior. Context: " + JSON.stringify(context) + " Query: " + args[3].toString() + " Error: " + error)
+        }
 
         return res
     }
 
     EvalAdd(context, args, scope, eoqHistory, callback) {
         var res = this.EvalElementOperation(context, args, scope, 'ADD', this.addEvaluators, eoqHistory, callback)
         return res
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/auxiliaries.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/auxiliaries.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/esUtils.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/esUtils.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync/util/uuid.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync/util/uuid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/ecoreSync.ui/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/ecoreSync.ui/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/AnchorController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/AnchorController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/ContainerController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/ContainerController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/EdgeController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/EdgeController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/GraphController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/GraphController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/LabelController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/LabelController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/QueryController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/QueryController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/graph/VertexController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/graph/VertexController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/controllers/palette/PaletteController.js` & `XGEE-0.3.0/xgee/core/plugins/editor/controllers/palette/PaletteController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/css/loading.css` & `XGEE-0.3.0/xgee/core/plugins/editor/css/loading.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js` & `XGEE-0.3.0/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/graph/GraphResourceProvider.js` & `XGEE-0.3.0/xgee/core/plugins/editor/graph/GraphResourceProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/graph/mxGraphIntegration.js` & `XGEE-0.3.0/xgee/core/plugins/editor/graph/mxGraphIntegration.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/interactions/DropReception.js` & `XGEE-0.3.0/xgee/core/plugins/editor/interactions/DropReception.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/interactions/GraphInteraction.js` & `XGEE-0.3.0/xgee/core/plugins/editor/interactions/GraphInteraction.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/lib/libapi.js` & `XGEE-0.3.0/xgee/core/plugins/editor/lib/libapi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/lib/libaux.js` & `XGEE-0.3.0/xgee/core/plugins/editor/lib/libaux.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/lib/libjsa.js` & `XGEE-0.3.0/xgee/core/plugins/editor/lib/libjsa.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/lib/uuid.js` & `XGEE-0.3.0/xgee/core/plugins/editor/lib/uuid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/editorModel.ecore` & `XGEE-0.3.0/xgee/core/plugins/editor/model/editorModel.ecore`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Anchor.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Anchor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/AnchorManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/AnchorManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Container.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Container.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerProvider.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/ContainerType.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/ContainerType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/DeletableObject.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/DeletableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Edge.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Edge.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EdgeContainer.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EdgeContainer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EdgeManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EdgeManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/EventProvider.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/EventProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphEvent.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -173,14 +173,18 @@
         cmd.Crn("http://www.eoq.de/workspacemdbmodel/v1.0", "ModelResource", 1)
         cmd.Set(new eoq2.Qry().His(1), "name", layoutResourceName)
         cmd.Add(new eoq2.Qry().His(1), "contents", new eoq2.Qry().His(0))
         cmd.Add(new eoq2.Qry().Obj(this.ecoreSync.rlookup(directory)), "resources", new eoq2.Qry().His(1));
 
         var result = await this.ecoreSync.exec(cmd)
 
+        if (result.length != cmd.a.length) {
+            throw new Error('Cannot create layout resource. layout.ecore loaded?');
+        }
+
         return result[1]
     }
 
     async getLayoutResource() {
         if (this.resource != null) {
             return this.resource
         }
@@ -316,15 +320,15 @@
         cmd.Crn('http://www.xgee.de/layout/v1/def', 'Edge', 1)
         cmd.Set(new eoq2.Qry().His(-1), "refersTo", new eoq2.Obj(this.ecoreSync.rlookup(eObject)))
         cmd.Add(new eoq2.Obj(this.ecoreSync.rlookup(this.layout)), "contents", new eoq2.Qry().His(-2))
         if (supportPoints != null) {
 
         }
         var result = await this.ecoreSync.remoteExec(cmd)
-        return this.ecoreSync.getObjectById(result[0].v)
+        return this.ecoreSync.getObject(result[0].v)
     }
 
 
     async getVertexLayoutItem(vertex) {
         var layout = await this.getLayout();
         var parentVertex = null;
         var vertexLayoutItem = null;
@@ -511,49 +515,40 @@
                 await self.buildCache()
             }
         });
     }
 
 
     async observeVertexPosition(vertex, callback) {
-        return true;
-        var pos = {
-            x: 0,
-            y: 0
-        };
-        var timeout = null;
-        var timeoutInterval = 100;
-        var resetTimer = function() {
-            if (timeout) {
-                clearTimeout(timeout);
-            }
-            timeout = window.setTimeout(function() {
-                callback(pos);
-            }, timeoutInterval);
-        }
-
-        try {
-            var vertexLayoutItem = await this.getVertexLayoutItem(vertex)
-            if (vertexLayoutItem) {
-                this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('x'), function(val) {
-                    pos.x = val;
-                    resetTimer();
-                });
-                this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('y'), function(val) {
-                    pos.y = val;
-                    resetTimer();
-                });
-                return true
-            } else {
-                throw 'missing layout item'
-            }
-        } catch (e) {
-            console.error('Failed observing vertex position: ' + e)
-        }
-        return false
+        return true; // the following code has never been active, commented out to silence firefox
+        // var pos={x:0,y:0};
+        // var timeout = null;
+        // var timeoutInterval=100;
+        // var resetTimer=function(){
+        //     if(timeout){ clearTimeout(timeout);  }  timeout=window.setTimeout(function(){ callback(pos); }, timeoutInterval);
+        // }
+
+        // try{        
+        //     var vertexLayoutItem=await this.getVertexLayoutItem(vertex)
+        //     if(vertexLayoutItem)
+        //     {            
+        //         this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('x'),function(val){ pos.x=val;    resetTimer();   });
+        //         this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('y'),function(val){ pos.y=val;    resetTimer();   });
+        //         return true
+        //     }
+        //     else
+        //     {
+        //         throw 'missing layout item'
+        //     }
+        // }
+        // catch(e)
+        // {
+        //     console.error('Failed observing vertex position: '+e)
+        // }
+        // return false
     }
 
 
     addTemporaryVertexPosition(objectId, parentObjectId, pos) {
         var tempPosition = {
             objectId: objectId,
             parent: parentObjectId,
@@ -591,49 +586,40 @@
         return vertexLayoutItem
     }
 
 
 
 
     async observeVertexSize(vertex, callback) {
-        return true;
-        var size = {
-            x: 0,
-            y: 0
-        };
-        var timeout = null;
-        var timeoutInterval = 100;
-        var resetTimer = function() {
-            if (timeout) {
-                clearTimeout(timeout);
-            }
-            timeout = window.setTimeout(function() {
-                callback(size);
-            }, timeoutInterval);
-        }
-
-        try {
-            var vertexLayoutItem = await this.getVertexLayoutItem(vertex)
-            if (vertexLayoutItem) {
-                this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('sizeX'), function(val) {
-                    size.x = val;
-                    resetTimer();
-                });
-                this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('sizeY'), function(val) {
-                    size.y = val;
-                    resetTimer();
-                });
-                return true
-            } else {
-                throw 'missing layout item'
-            }
-        } catch (e) {
-            console.error('Failed observing vertex size: ' + e)
-        }
-        return false
+        return true; // the following code has never been active, commented out to silence firefox
+        // var size={x:0,y:0};
+        // var timeout = null;
+        // var timeoutInterval=100;
+        // var resetTimer=function(){
+        //     if(timeout){ clearTimeout(timeout);  }  timeout=window.setTimeout(function(){ callback(size); }, timeoutInterval);
+        // }
+
+        // try{        
+        //     var vertexLayoutItem=await this.getVertexLayoutItem(vertex)
+        //     if(vertexLayoutItem)
+        //     {            
+        //         this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('sizeX'),function(val){ size.x=val;    resetTimer();   });
+        //         this.ecoreSync.observe(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)).Pth('sizeY'),function(val){ size.y=val;    resetTimer();   });
+        //         return true
+        //     }
+        //     else
+        //     {
+        //         throw 'missing layout item'
+        //     }
+        // }
+        // catch(e)
+        // {
+        //     console.error('Failed observing vertex size: '+e)
+        // }
+        // return false
     }
 
     async setVertexSize(vertex, x = null, y = null) {
         var vertexLayoutItem = await this.getVertexLayoutItem(vertex)
         if (x != null && y != null) {
             this.updates.Set(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)), "sizeX", x)
             this.updates.Set(new eoq2.Obj(this.ecoreSync.rlookup(vertexLayoutItem)), "sizeY", y)
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModel.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModelFactory.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModelFactory.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphModelManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphModelManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphObject.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/GraphObjectManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/GraphObjectManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Label.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Label.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelSegment.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelSegment.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/LocatableObject.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/LocatableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/NestedLabel.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/NestedLabel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/SizableObject.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/SizableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertex.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertex.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertexManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertexManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/StaticVertexType.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/StaticVertexType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/TransactionObject.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/TransactionObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/Vertex.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/Vertex.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexContainer.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexContainer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexManager.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/graph/VertexType.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/graph/VertexType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/DragAndDropTool.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/DragAndDropTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
         for (let i = 0; i < this.anchors.length; i++) {
             if (this.anchors[i].get('selectionQuery') != null && this.anchors[i].get('selectionQuery') != '') {
                 let cmd = new eoq2.Cmp()
                 encodedEObjects.forEach((o) => {
                     // cmd.Get(eval('new eoq2.Obj('+o.v+').'+this.anchors[i].get('selectionQuery')))
                     let cmdStr = "#" + o.v + this.anchors[i].get('selectionQuery')
                     let addCmd = ts.deserialize(cmdStr)
-                    console.log('Anchor cmdStr:            ' + cmdStr)
+                    if ($DEBUG) console.log('Anchor cmdStr:            ' + cmdStr)
                     cmd.Get(addCmd)
                 })
 
                 //remote call due to performance issues of the local query runner
                 let selectionResults = await this.ecoreSync.remoteExec(cmd)
                 vertices.forEach((v, idx) => {
                     if (selectionResults[idx]) {
@@ -230,60 +230,62 @@
         return edgeSpan
     }
 
 
     canCreate(source, target) {
         var edgeSpan = this.getEdgeSpan(source, target)
         return edgeSpan.valid
-        sourceAnchor = sourceAnchor ? sourceAnchor.anchor : null
-        targetAnchor = targetAnchor ? targetAnchor.anchor : null
+        // sourceAnchor=sourceAnchor ? sourceAnchor.anchor : null
+        // targetAnchor=targetAnchor ? targetAnchor.anchor : null
 
-        //Sanity check
-        if (sourceAnchor && !sourceAnchor.get('type')) {
-            console.warn('source Anchor type undefined, defaulted to BOTH')
-            sourceAnchor.set('type', 'BOTH')
-        }
-
-        if (targetAnchor && !targetAnchor.get('type')) {
-            console.warn('target Anchor type undefined, defaulted to BOTH')
-            targetAnchor.set('type', 'BOTH')
-        }
-
-        if (sourceAnchor && targetAnchor) {
-            //strict cases where only source->target
-            let strictCases = {
-                "CASE_SOURCE_TO_TARGET": sourceAnchor.get('type') == 'SOURCE' && targetAnchor.get('type') == 'TARGET',
-                "CASE_SOURCE_TO_BOTH": sourceAnchor.get('type') == 'SOURCE' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_BOTH": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_TARGET": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'TARGET',
-            }
-
-            //non-strict cases where target->source is allowed
-            let nonStrictCases = {
-                "CASE_TARGET_TO_SOURCE": sourceAnchor.get('type') == 'TARGET' && targetAnchor.get('type') == 'SOURCE',
-                "CASE_TARGET_TO_BOTH": sourceAnchor.get('type') == 'TARGET' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_SOURCE": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'SOURCE',
-            }
-
-            let keys = Object.keys(strictCases);
-            for (let i = 0; i < keys.length; i++) {
-                results = results || strictCases[keys[i]]
-                if (results) break;
-            }
+        // //Sanity check
+        // if(sourceAnchor && !sourceAnchor.get('type')){
+        //     console.warn('source Anchor type undefined, defaulted to BOTH')
+        //     sourceAnchor.set('type','BOTH')
+        // }
+
+        // if(targetAnchor && !targetAnchor.get('type')){
+        //     console.warn('target Anchor type undefined, defaulted to BOTH')
+        //     targetAnchor.set('type','BOTH')
+        // }
+
+        // if(sourceAnchor && targetAnchor)
+        // {
+        //     //strict cases where only source->target
+        //     let strictCases={
+        //         "CASE_SOURCE_TO_TARGET": sourceAnchor.get('type')=='SOURCE' && targetAnchor.get('type')=='TARGET',
+        //         "CASE_SOURCE_TO_BOTH": sourceAnchor.get('type')=='SOURCE' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_BOTH": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_TARGET": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='TARGET',
+        //     }
+
+        //     //non-strict cases where target->source is allowed
+        //     let nonStrictCases={
+        //         "CASE_TARGET_TO_SOURCE": sourceAnchor.get('type')=='TARGET' && targetAnchor.get('type')=='SOURCE',
+        //         "CASE_TARGET_TO_BOTH": sourceAnchor.get('type')=='TARGET' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_SOURCE": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='SOURCE',
+        //     }
+
+        //     let keys=Object.keys(strictCases);            
+        //     for (let i = 0; i < keys.length; i++) {
+        //         results=results||strictCases[keys[i]]
+        //         if(results) break;
+        //     }
+
+        //     if(!isStrict && !results)
+        //     {
+        //         let keys=Object.keys(nonStrictCases);     
+        //         for (let i = 0; i < keys.length; i++) {
+        //             results=results||nonStrictCases[keys[i]]
+        //             if(results) break;
+        //         }
+        //     }      
+        // }
 
-            if (!isStrict && !results) {
-                let keys = Object.keys(nonStrictCases);
-                for (let i = 0; i < keys.length; i++) {
-                    results = results || nonStrictCases[keys[i]]
-                    if (results) break;
-                }
-            }
-        }
-
-        return results;
+        // return results;
     }
 
     async getEdgeItem() {
         let edgeItem = this.edgeItem
         this.edgeItem = ecoreSync.clone(this.template)
         return await edgeItem
     }
@@ -351,77 +353,86 @@
 
         return true
 
 
 
 
 
-        var sourceAnchor = this.anchorCache.find(function(e) {
-            return e.eObject == source
-        });
-        var targetAnchor = this.anchorCache.find(function(e) {
-            return e.eObject == target
-        });
-
-        sourceAnchor = sourceAnchor ? sourceAnchor.anchor : null
-        targetAnchor = targetAnchor ? targetAnchor.anchor : null
-
-        if (sourceAnchor && !sourceAnchor.get('type')) {
-            console.warn('source Anchor type undefined, defaulted to BOTH')
-            sourceAnchor.set('type', 'BOTH')
-        }
-
-        if (targetAnchor && !targetAnchor.get('type')) {
-            console.warn('target Anchor type undefined, defaulted to BOTH')
-            targetAnchor.set('type', 'BOTH')
-        }
-
-        if (sourceAnchor && targetAnchor) {
-            //strict cases where only source->target
-            let strictCases = {
-                "CASE_SOURCE_TO_TARGET": sourceAnchor.get('type') == 'SOURCE' && targetAnchor.get('type') == 'TARGET',
-                "CASE_SOURCE_TO_BOTH": sourceAnchor.get('type') == 'SOURCE' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_BOTH": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_TARGET": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'TARGET',
-            }
-
-            //non-strict cases where target->source is allowed
-            let nonStrictCases = {
-                "CASE_TARGET_TO_SOURCE": sourceAnchor.get('type') == 'TARGET' && targetAnchor.get('type') == 'SOURCE',
-                "CASE_TARGET_TO_BOTH": sourceAnchor.get('type') == 'TARGET' && targetAnchor.get('type') == 'BOTH',
-                "CASE_BOTH_TO_SOURCE": sourceAnchor.get('type') == 'BOTH' && targetAnchor.get('type') == 'SOURCE',
-            }
-
-            let keys = Object.keys(strictCases);
-            for (let i = 0; i < keys.length; i++) {
-                if (strictCases[keys[i]]) {
-                    matched = true
-                    inverted = false
-                    break;
-                }
-
-            }
-
-            if (!isStrict && !matched) {
-                let keys = Object.keys(nonStrictCases);
-                for (let i = 0; i < keys.length; i++) {
-                    if (nonStrictCases[keys[i]]) {
-                        matched = true
-                        inverted = true
-                        break;
-                    }
-                }
-            }
-        }
-
-        if (matched && source && target) {
-            if (!inverted) {
-                this.routeEdge(source, target)
-            } else {
-                this.routeEdge(target, source)
-            }
-
-        } else {
-            throw 'edge routing tool: no suitable match found'
-        }
+        // var sourceAnchor=this.anchorCache.find(function(e){
+        //     return e.eObject==source
+        // });
+        // var targetAnchor=this.anchorCache.find(function(e){
+        //     return e.eObject==target        
+        // });
+
+        // sourceAnchor=sourceAnchor ? sourceAnchor.anchor : null
+        // targetAnchor=targetAnchor ? targetAnchor.anchor : null
+
+        // if(sourceAnchor && !sourceAnchor.get('type')){
+        //     console.warn('source Anchor type undefined, defaulted to BOTH')
+        //     sourceAnchor.set('type','BOTH')
+        // }
+
+        // if(targetAnchor && !targetAnchor.get('type')){
+        //     console.warn('target Anchor type undefined, defaulted to BOTH')
+        //     targetAnchor.set('type','BOTH')
+        // }                 
+
+        // if(sourceAnchor && targetAnchor)
+        // {
+        //     //strict cases where only source->target
+        //     let strictCases={
+        //         "CASE_SOURCE_TO_TARGET": sourceAnchor.get('type')=='SOURCE' && targetAnchor.get('type')=='TARGET',
+        //         "CASE_SOURCE_TO_BOTH": sourceAnchor.get('type')=='SOURCE' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_BOTH": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_TARGET": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='TARGET',
+        //     }
+
+        //     //non-strict cases where target->source is allowed
+        //     let nonStrictCases={
+        //         "CASE_TARGET_TO_SOURCE": sourceAnchor.get('type')=='TARGET' && targetAnchor.get('type')=='SOURCE',
+        //         "CASE_TARGET_TO_BOTH": sourceAnchor.get('type')=='TARGET' && targetAnchor.get('type')=='BOTH',
+        //         "CASE_BOTH_TO_SOURCE": sourceAnchor.get('type')=='BOTH' && targetAnchor.get('type')=='SOURCE',
+        //     }
+
+        //     let keys=Object.keys(strictCases);            
+        //     for (let i = 0; i < keys.length; i++) {
+        //         if(strictCases[keys[i]])
+        //         {
+        //             matched=true   
+        //             inverted=false               
+        //             break;
+        //         }
+
+        //     }
+
+        //     if(!isStrict && !matched)
+        //     {
+        //         let keys=Object.keys(nonStrictCases);     
+        //         for (let i = 0; i < keys.length; i++) {
+        //             if(nonStrictCases[keys[i]])
+        //             {
+        //                 matched=true
+        //                 inverted=true
+        //                 break;
+        //             }
+        //         }
+        //     }      
+        // }    
+
+        // if(matched && source && target)
+        // {
+        //    if(!inverted){
+        //         this.routeEdge(source,target)
+        //    }
+        //    else
+        //    {
+        //         this.routeEdge(target,source)
+        //    }
+
+        // }
+        // else
+        // {
+        //     throw 'edge routing tool: no suitable match found'
+        // }
     }
 }
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/GraphTool.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/GraphTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/PaletteModel.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/PaletteModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/SelectionTool.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/SelectionTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/model/palette/ToolGenerator.js` & `XGEE-0.3.0/xgee/core/plugins/editor/model/palette/ToolGenerator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/editor/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/queries/Query.js` & `XGEE-0.3.0/xgee/core/plugins/editor/queries/Query.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/view/GraphView.js` & `XGEE-0.3.0/xgee/core/plugins/editor/view/GraphView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/view/GraphViewMenu.js` & `XGEE-0.3.0/xgee/core/plugins/editor/view/GraphViewMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/view/GraphViewPort.js` & `XGEE-0.3.0/xgee/core/plugins/editor/view/GraphViewPort.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/view/PaletteView.js` & `XGEE-0.3.0/xgee/core/plugins/editor/view/PaletteView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/editor/view/ScreenshotExport.js` & `XGEE-0.3.0/xgee/core/plugins/editor/view/ScreenshotExport.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq.actions/css/ActionsUi.css` & `XGEE-0.3.0/xgee/core/plugins/eoq.actions/css/ActionsUi.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsController.js` & `XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsCore.js` & `XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsCore.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
             let cmd = new eoq2.Gaa();
             domain.Do(cmd).then(function(val) {
                 try {
                     let actions = [];
                     let nActions = val.length;
                     for (let i = 0; i < nActions; i++) {
                         let actionInfo = val[i];
-                        let actionSegments = actionInfo[0].split("/[/\\]/");
+                        let actionSegments = actionInfo[0].replaceAll("\\", "*").replaceAll("/", "*").split("*");
                         let nSegments = actionSegments.length;
                         let actionName = actionSegments[nSegments - 1];
                         let categories = actionSegments.slice(0, nSegments - 1);
                         actions.push({
                             id: actionInfo[0],
                             name: actionName,
                             categories: categories,
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq.actions/js/ActionsUi.js` & `XGEE-0.3.0/xgee/core/plugins/eoq.actions/js/ActionsUi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq.actions/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/eoq.actions/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/eoq1/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/README.md` & `XGEE-0.3.0/xgee/core/plugins/eoq1/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/commandparser.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/commandparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/domains/bufferingdomain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/domains/bufferingdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/domains/domain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/domains/domain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/domains/httppostdomain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/domains/httppostdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/model/model.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/model/model.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/resultparser.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/resultparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq1/valueparser.js` & `XGEE-0.3.0/xgee/core/plugins/eoq1/valueparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/eoq2/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/README.md` & `XGEE-0.3.0/xgee/core/plugins/eoq2/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/action/call.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/action/call.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/command/command.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/command/command.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/command/result.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/command/result.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/domain/domain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/domain/domain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/eoq2.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/eoq2.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/event/event.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/event/event.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/frame/frame.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/frame/frame.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/legacy/legacy.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/legacy/legacy.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/query/query.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/query/query.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/jsonserializer.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/serializer.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -3,33 +3,32 @@
  */
 
 var eoq2 = eoq2 || {};
 eoq2.serialization = eoq2.serialization || {};
 
 Object.assign(eoq2.serialization, (function() {
 
-    function JsonSerializer() {
-
+    function Serializer() {
+        //ABSTRACT
     };
-    JsonSerializer.prototype = Object.create(eoq2.serialization.Serializer.prototype);
 
-    JsonSerializer.prototype.Ser = function(val) {
-        return JSON.stringify(val);
+    Serializer.prototype.Ser = function(val) {
+        throw new Error("Not implemented.");
     }
 
-    JsonSerializer.prototype.Des = function(code) {
-        console.log(code);
-        let jsonObj = JSON.parse(code);
-        let val = this.RecreateObjects(jsonObj);
-        return val;
+    Serializer.prototype.Des = function(code) {
+        throw new Error("Not implemented.");
     };
 
-    JsonSerializer.prototype.RecreateObjects = function(jsonObj) {
-        //TODO: Implement object creation if necessary
-        return jsonObj;
+    //legacy support
+    Serializer.prototype.serialize = function(val) {
+        return this.Ser(val);
     };
 
+    Serializer.prototype.deserialize = function(code) {
+        return this.Des(code);
+    };
 
     return {
-        JsonSerializer: JsonSerializer
+        Serializer: Serializer
     };
 })());
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/serialization/textserializer.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/serialization/textserializer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -256,19 +256,19 @@
 
     };
 
     /*
      *   GENERAL METHODS
      * */
     TextSerializer.prototype.EnableDebugging = function() {
-        this._debugMode = True;
+        this._debugMode = true;
     };
 
     TextSerializer.prototype.DisableDebugging = function() {
-        this._debugMode = False;
+        this._debugMode = false;
     };
 
     /*
      *   JS2TXT METHODS
      * */
 
     TextSerializer.prototype = Object.create(eoq2.serialization.Serializer.prototype);
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/eoq2/util/logger.js` & `XGEE-0.3.0/xgee/core/plugins/eoq2/util/logger.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eventBroker/SelectionChangedEvent.js` & `XGEE-0.3.0/xgee/core/plugins/eventBroker/SelectionChangedEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/eventBroker/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/eventBroker/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/iconProvider/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/iconProvider/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/keyHandler/js/KeyHandler.js` & `XGEE-0.3.0/xgee/core/plugins/keyHandler/js/KeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/keyHandler.ecore/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/keyHandler.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/LICENSE` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.contextMenu/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.contextMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView/plugin.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -700,15 +700,15 @@
 
 
         var cmenuProviders = pluginAPI.evaluate('ecoreTreeView.menus');
 
 
         //registering context menu with tree
         $.contextMenu({
-            selector: '#' + DOMelement.id + ' .fancytree-title',
+            selector: '#' + DOMelement.id.replace("#", "\\#") + ' .fancytree-title', // replace masks '#' in IDs like #WORKSPACE
             build: function($triggerElement, e) {
 
                 e.preventDefault();
                 var menu = null;
                 var node = $.ui.fancytree.getNode(e);
                 var offset = $($triggerElement).offset();
```

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/LICENSE.txt` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif` & `XGEE-0.3.0/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/css/PropertiesView.css` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/css/PropertiesView.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/js/PropertiesViewController.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/js/PropertiesViewController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.custom/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.custom/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.editors/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.editors/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.modify/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.modify/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/propertiesView.info/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/propertiesView.info/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.goToView/js/GoToViewTool.js` & `XGEE-0.3.0/xgee/core/plugins/tool.goToView/js/GoToViewTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js` & `XGEE-0.3.0/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.goToView/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/tool.goToView/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/css/NotesTool.css` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/css/NotesTool.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-error.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-error.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-info.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-info.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-success.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-success.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/img/notes-warning.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/img/notes-warning.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/img/tool-notes.svg` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/img/tool-notes.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/js/NotesTool.js` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/js/NotesTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/js/NotesToolProvider.js` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/js/NotesToolProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tool.notes/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/tool.notes/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tools/js/ToolsController.js` & `XGEE-0.3.0/xgee/core/plugins/tools/js/ToolsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/tools/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/tools/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard/img/view-dashboard.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard/img/view-dashboard.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.infoDash/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.infoDash/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.workspace/img/view-workspace.svg` & `XGEE-0.3.0/xgee/core/plugins/view.workspace/img/view-workspace.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js` & `XGEE-0.3.0/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/view.workspace/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/view.workspace/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/views/js/ViewsController.js` & `XGEE-0.3.0/xgee/core/plugins/views/js/ViewsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/views/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/views/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js` & `XGEE-0.3.0/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/viewsMenu/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/viewsMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css` & `XGEE-0.3.0/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/core/plugins/viewsTabbar/plugin.js` & `XGEE-0.3.0/xgee/core/plugins/viewsTabbar/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/PyEoq2WebServer.py` & `XGEE-0.3.0/xgee/eoqserver/PyEoq2WebServer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/actions/actionutils.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/actions/actionutils.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/actions/externalactionhandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/actions/externalactionhandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/commandparser.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/commandparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/domains/localdomain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/domains/localdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/domains/remotehttpdomain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/domains/remotehttpdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/error/error.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/error/error.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/model/__init__.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/model/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/model/model.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/model/model.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/queryparser.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/queryparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/resultparser.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/resultparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/utils/csvconnector.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/utils/csvconnector.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq1/valueparser.py` & `XGEE-0.3.0/xgee/eoqserver/eoq1/valueparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/action.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/action.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/call.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/call.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/callhandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/callhandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/callmanager.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/callmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/action/util.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/action/util.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/command/command.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/command/command.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/command/commandrunner.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/command/commandrunner.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/command/diff.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/command/diff.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/command/result.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/command/result.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/domain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/domain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/event/event.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/event/event.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/frame/domainframehandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/frame/domainframehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/frame/framehandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/frame/framehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/frame/multiversionframehandler.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/frame/multiversionframehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/legacy/legacy.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/legacy/legacy.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/mdbaccessor.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/mdbaccessor.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/query/query.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/query/query.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/query/queryrunner.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/query/queryrunner.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/jsonserializer.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/jsserializer.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/jsserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/pyserializer.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/pyserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/serialization/textserializer.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/serialization/textserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/backup.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/backup.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/benchmark.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/csvconnector.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/csvconnector.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/error.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/error.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/logger.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/logger.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/model.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/model.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/eoqserver/eoq2/util/util.py` & `XGEE-0.3.0/xgee/eoqserver/eoq2/util/util.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/meta/layout.ecore` & `XGEE-0.3.0/xgee/meta/layout.ecore`

 * *Files identical despite different names*

### Comparing `XGEE-0.2.9/xgee/xgee.py` & `XGEE-0.3.0/xgee/xgee.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     from yaml import CLoader as Loader, CDumper as Dumper
 except ImportError:
     from yaml import Loader, Dumper
 
 import __main__
 
-__version__ = '0.2.9'
+__version__ = '0.3.0'
 
 DEFAULT_PATH='./'
 DEFAULT_HOST=socket.gethostname()
 localpath=str(Path().resolve())
 FRAMEWORK_RUN_FLAG=True
 apps=[]
 
@@ -49,15 +49,15 @@
         self.metaDir='./.meta'
         self.actions=1 # actions are enabled by default
         self.actionsDir='./workspace/actions'
         self.timeout=10.0
         self.backup=0 # backups are disabled by default
         self.backupDir='./backup'
         self.logDir='./log'
-        self.logToFile=1 # loggint to file is enabled by default
+        self.logToFile=1 # logging to file is enabled by default
         self.logToConsole=0 # logging to console is disabled by default
         self.autosave=5.0 # the timeout after which autosave is triggered
         self.trackFileChanges=0 # whether tracking of changes on the filesystems is enabled (default:OFF)
         self.maxChanges=10000 # how many changes shall be remembered until the oldest change is forgotten (1 to 1000000)
         self.enableBenchmark=0 # measure time for queries and commands
 
 
@@ -115,17 +115,26 @@
                 self.eoqConfiguration.logDir=localpath+'/'+self.path+str(self.get_conf_parameter('eoq/log')).lstrip("./")
             else:
                 self.eoqConfiguration.logDir=localpath+'/'+self.path+'log'
 
             # Configure backup directory
             if self.get_conf_parameter('eoq/backup') is not None:
                 self.eoqConfiguration.backupDir=localpath+'/'+self.path+str(self.get_conf_parameter('eoq/backup')).lstrip("./")
+                self.eoqConfiguration.backup=1 # backups are enabled if a directory was set
             else:
                 self.eoqConfiguration.backupDir=localpath+'/'+self.path+'backup'
 
+            # option to log to console
+            if self.get_conf_parameter('eoq/consolelog') is not None:
+                self.eoqConfiguration.logToConsole=self.get_conf_parameter('eoq/consolelog')
+
+            # Configure autosave
+            if self.get_conf_parameter('eoq/autosave') is not None:
+                self.eoqConfiguration.autosave=self.get_conf_parameter('eoq/consolelog')
+
     def getName(self):
         return self.name
 
     def getPath(self):
         return self.path
     
     def getWebInstanceUrl(self, default='---'):
@@ -301,7 +310,8 @@
         path2apps=sys.argv[1]
     start(path2apps) 
 
         
     
 
 
+
```

