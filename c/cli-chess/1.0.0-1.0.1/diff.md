# Comparing `tmp/cli-chess-1.0.0.tar.gz` & `tmp/cli-chess-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-chess-1.0.0.tar", last modified: Fri Mar 31 03:37:16 2023, max compression
+gzip compressed data, was "cli-chess-1.0.1.tar", last modified: Tue Jun 27 19:34:50 2023, max compression
```

## Comparing `cli-chess-1.0.0.tar` & `cli-chess-1.0.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    35823 2023-03-31 03:37:02.000000 cli-chess-1.0.0/LICENSE
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      118 2023-03-31 03:37:02.000000 cli-chess-1.0.0/MANIFEST.in
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     7312 2023-03-31 03:37:16.985397 cli-chess-1.0.0/PKG-INFO
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6027 2023-03-31 03:37:02.000000 cli-chess-1.0.0/README.md
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1282 2023-03-31 03:37:16.989397 cli-chess-1.0.0/setup.cfg
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1734 2023-03-31 03:37:02.000000 cli-chess-1.0.0/setup.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.961397 cli-chess-1.0.0/src/
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.965397 cli-chess-1.0.0/src/cli_chess/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      334 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      886 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/__main__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      981 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/__metadata__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.965397 cli-chess-1.0.0/src/cli_chess/core/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.965397 cli-chess-1.0.0/src/cli_chess/core/api/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      212 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/api/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2190 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/api/api_manager.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4847 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/api/game_state_dispatcher.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3737 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/api/incoming_event_manger.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/core/game/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      340 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5262 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/game_model_base.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5173 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/game_options.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5224 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/game_presenter_base.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     7365 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/game_view_base.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/core/game/offline_game/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      153 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/offline_game/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5868 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6855 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2082 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/core/game/online_game/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      147 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    15286 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5512 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2130 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      148 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    12478 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2092 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3454 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/core/main/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      108 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/main/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1583 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/main/main_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2112 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/main/main_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     7279 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/core/main/main_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/menus/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      398 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/menus/main_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      152 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/main_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1572 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1878 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6506 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_view.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2964 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/menu_common.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1729 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3790 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6996 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.969397 cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      211 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1296 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1459 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3007 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      204 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1606 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1769 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4611 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      204 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4318 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2173 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1150 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/menus/settings_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      180 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/settings_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1514 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1648 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3285 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      190 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1985 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1392 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2517 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/menus/versus_menus/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      272 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/versus_menus/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4932 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_models.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4356 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_presenters.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1950 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_views.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/modules/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.973397 cli-chess-1.0.0/src/cli_chess/modules/about/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)       78 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/about/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1377 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/about/about_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3834 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/about/about_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.977397 cli-chess-1.0.0/src/cli_chess/modules/board/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      114 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/board/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    14280 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/board/board_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     8009 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/board/board_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2807 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/board/board_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.977397 cli-chess-1.0.0/src/cli_chess/modules/clock/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)       78 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/clock/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2500 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/clock/clock_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1601 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/clock/clock_view.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1261 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/common.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.977397 cli-chess-1.0.0/src/cli_chess/modules/engine/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)       84 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.981397 cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/
--rwxrwxr-x   0 trevor    (1000) trevor    (1000)   697544 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos
--rwxrwxr-x   0 trevor    (1000) trevor    (1000)   797928 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux
--rwxrwxr-x   0 trevor    (1000) trevor    (1000)   761256 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos
--rwxrwxr-x   0 trevor    (1000) trevor    (1000)  1916430 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4496 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/engine_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1395 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/engine/engine_presenter.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.981397 cli-chess-1.0.0/src/cli_chess/modules/material_difference/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      195 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/material_difference/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6343 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4246 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2506 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/modules/move_list/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      135 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/move_list/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3214 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3345 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3680 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/modules/player_info/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      100 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/player_info/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1864 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/player_info/player_info_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4083 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/player_info/player_info_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/modules/token_manager/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      159 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/token_manager/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5149 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1886 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4844 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_view.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/modules/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/__init__.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/modules/board/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/board/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    14880 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/board/test_board_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    11841 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/board/test_board_presenter.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6963 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5369 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4431 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/test_move_list_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     5772 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1333 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/test_common.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4407 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     1974 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/tests/utils/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/utils/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     4421 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/tests/utils/test_event.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.985397 cli-chess-1.0.0/src/cli_chess/utils/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      395 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/__init__.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2672 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/argparse.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     3931 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/common.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)    14905 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/config.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2804 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/event.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2191 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/logging.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     2804 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/styles.py
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6549 2023-03-31 03:37:02.000000 cli-chess-1.0.0/src/cli_chess/utils/ui_common.py
-drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-03-31 03:37:16.965397 cli-chess-1.0.0/src/cli_chess.egg-info/
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     7312 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/PKG-INFO
--rw-rw-r--   0 trevor    (1000) trevor    (1000)     6424 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/SOURCES.txt
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        1 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/dependency_links.txt
--rw-rw-r--   0 trevor    (1000) trevor    (1000)       55 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/entry_points.txt
--rw-rw-r--   0 trevor    (1000) trevor    (1000)        1 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/not-zip-safe
--rw-rw-r--   0 trevor    (1000) trevor    (1000)      198 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/requires.txt
--rw-rw-r--   0 trevor    (1000) trevor    (1000)       10 2023-03-31 03:37:16.000000 cli-chess-1.0.0/src/cli_chess.egg-info/top_level.txt
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.595588 cli-chess-1.0.1/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    35823 2023-04-14 18:32:25.000000 cli-chess-1.0.1/LICENSE
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      118 2023-04-14 18:32:25.000000 cli-chess-1.0.1/MANIFEST.in
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     7704 2023-06-27 19:34:50.595588 cli-chess-1.0.1/PKG-INFO
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6469 2023-06-27 19:31:14.000000 cli-chess-1.0.1/README.md
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1243 2023-06-27 19:34:50.595588 cli-chess-1.0.1/setup.cfg
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1723 2023-05-08 13:37:04.000000 cli-chess-1.0.1/setup.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.555588 cli-chess-1.0.1/src/
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.563588 cli-chess-1.0.1/src/cli_chess/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      334 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      886 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/__main__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      981 2023-06-27 19:31:14.000000 cli-chess-1.0.1/src/cli_chess/__metadata__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.563588 cli-chess-1.0.1/src/cli_chess/core/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.563588 cli-chess-1.0.1/src/cli_chess/core/api/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      212 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/api/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2190 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/api/api_manager.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4847 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/api/game_state_dispatcher.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3737 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/api/incoming_event_manger.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.567588 cli-chess-1.0.1/src/cli_chess/core/game/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      340 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5262 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/game_model_base.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5173 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/game_options.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5224 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/game_presenter_base.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     7365 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/game_view_base.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.567588 cli-chess-1.0.1/src/cli_chess/core/game/offline_game/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      153 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/offline_game/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5868 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6855 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2082 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.567588 cli-chess-1.0.1/src/cli_chess/core/game/online_game/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      147 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    15699 2023-06-27 19:02:28.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5512 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2130 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.567588 cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      148 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    12478 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2092 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3454 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.567588 cli-chess-1.0.1/src/cli_chess/core/main/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      108 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/main/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1583 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/main/main_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2112 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/main/main_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     7279 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/core/main/main_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      398 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/main_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      152 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/main_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1572 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1878 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6506 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_view.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2964 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/menu_common.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1729 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3790 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6996 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      211 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1296 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1459 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3007 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      204 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1606 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1769 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4611 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      204 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4318 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2173 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1150 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.571588 cli-chess-1.0.1/src/cli_chess/menus/settings_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      180 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/settings_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1514 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1648 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3285 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      190 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1985 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1392 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2517 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/menus/versus_menus/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      272 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/versus_menus/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4932 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_models.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4356 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_presenters.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1950 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_views.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/modules/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/modules/about/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)       78 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/about/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1377 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/about/about_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3834 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/about/about_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/modules/board/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      114 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/board/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    14280 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/board/board_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     8009 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/board/board_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2807 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/board/board_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.575588 cli-chess-1.0.1/src/cli_chess/modules/clock/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)       78 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/clock/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2500 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/clock/clock_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1601 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/clock/clock_view.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1261 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/common.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.579588 cli-chess-1.0.1/src/cli_chess/modules/engine/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)       84 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.583588 cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/
+-rwxrwxr-x   0 trevor    (1000) trevor    (1000)   697544 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos
+-rwxrwxr-x   0 trevor    (1000) trevor    (1000)   797928 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux
+-rwxrwxr-x   0 trevor    (1000) trevor    (1000)   761256 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos
+-rwxrwxr-x   0 trevor    (1000) trevor    (1000)  1916430 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4496 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/engine_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1395 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/engine/engine_presenter.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.587588 cli-chess-1.0.1/src/cli_chess/modules/material_difference/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      195 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/material_difference/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6343 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4246 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2506 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.587588 cli-chess-1.0.1/src/cli_chess/modules/move_list/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      135 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/move_list/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3214 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3345 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3680 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.587588 cli-chess-1.0.1/src/cli_chess/modules/player_info/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      100 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/player_info/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1864 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/player_info/player_info_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4083 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/player_info/player_info_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/modules/token_manager/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      159 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/token_manager/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5149 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1886 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4844 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_view.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/modules/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/__init__.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/modules/board/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/board/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    14880 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/board/test_board_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    11841 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/board/test_board_presenter.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6963 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5369 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4431 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/test_move_list_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     5772 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1333 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/test_common.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4407 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     1974 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.591588 cli-chess-1.0.1/src/cli_chess/tests/utils/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        0 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/utils/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     4421 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/tests/utils/test_event.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.595588 cli-chess-1.0.1/src/cli_chess/utils/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      395 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/__init__.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2672 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/argparse.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     3931 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/common.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)    14905 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/config.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2804 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/event.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2191 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/logging.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     2804 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/styles.py
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6549 2023-04-14 18:32:25.000000 cli-chess-1.0.1/src/cli_chess/utils/ui_common.py
+drwxrwxr-x   0 trevor    (1000) trevor    (1000)        0 2023-06-27 19:34:50.563588 cli-chess-1.0.1/src/cli_chess.egg-info/
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     7704 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/PKG-INFO
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)     6424 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/SOURCES.txt
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        1 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/dependency_links.txt
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)       55 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/entry_points.txt
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)        1 2023-04-14 18:43:19.000000 cli-chess-1.0.1/src/cli_chess.egg-info/not-zip-safe
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)      187 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/requires.txt
+-rw-rw-r--   0 trevor    (1000) trevor    (1000)       10 2023-06-27 19:34:50.000000 cli-chess-1.0.1/src/cli_chess.egg-info/top_level.txt
```

### Comparing `cli-chess-1.0.0/LICENSE` & `cli-chess-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/PKG-INFO` & `cli-chess-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: cli-chess
-Version: 1.0.0
+Version: 1.0.1
 Summary: A highly customizable way to play chess in your terminal
 Home-page: https://github.com/trevorbayless/cli-chess
 Author: Trevor Bayless
 Author-email: trevorbayless1@gmail.com
 License: GPL-3.0+
 Keywords: chess,terminal,fairy-stockfish,stockfish,lichess,lichess.org,cli,san,uci
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-45a2-97cb-6a25b5ca9c0c.png"/></a>
 </p>
@@ -42,18 +41,26 @@
     <a href="https://github.com/trevorbayless/cli-chess/actions/">
         <img alt="CI Workflow" src="https://github.com/trevorbayless/cli-chess/actions/workflows/ci.yml/badge.svg?branch=master&event=push">
     </a>
     <a href="https://pypi.org/project/cli-chess/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/cli-chess?color=informational&label=PyPI&logo=PyPI">
     </a>
     <a href="#">
-        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.7%2B&color=informational&logo=python">
+        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.8%2B&color=informational&logo=python">
     </a>
 </p>
 
+<details><summary>Demo</summary>
+
+Offline against Fairy-Stockfish            |  Watching Lichess Bullet TV
+:-------------------------:|:-------------------------:
+<img src=https://user-images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-714e2a9c9c83.gif width=450 width=222> | <img src=https://user-images.githubusercontent.com/3620552/229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif width=430 height=245>
+
+</details>
+
 ## Main Features
 - Play online using your Lichess.org account
 - Play offline against the Fairy-Stockfish engine
 - Supports playing all Lichess [variants](https://lichess.org/variant)
 - Theme the chess board and pieces to the colors of your choice
 - Theme UI components to the colors of your choice
 - Supports making moves in UCI, SAN, or LAN
@@ -85,15 +92,15 @@
 [default style elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/styles.py)
 in the `custom_style.py` file. This file will be located at `$HOME/.config/cli-chess/` for Linux and macOS and
 `$APPDATA/cli-chess/` for Windows.
 
 Colors are expected to be [HTML color names](https://www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`)
 or [HTML hex colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`). The display of selected
 colors is dependent on the terminal supporting true colors and the `Terminal Color Depth` option in cli-chess program
-setting being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
+settings being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
 to the closest supported color.
 
 Restarting cli-chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this custom style sheet is
 invalid in any way, the default cli-chess style will be applied. This file must be kept in dictionary format.
 
 Example `custom_style.py` to override board and piece colors:
 ```json
```

#### html2text {}

```diff
@@ -1,68 +1,72 @@
-Metadata-Version: 2.1 Name: cli-chess Version: 1.0.0 Summary: A highly
+Metadata-Version: 2.1 Name: cli-chess Version: 1.0.1 Summary: A highly
 customizable way to play chess in your terminal Home-page: https://github.com/
 trevorbayless/cli-chess Author: Trevor Bayless Author-email:
 trevorbayless1@gmail.com License: GPL-3.0+ Keywords: chess,terminal,fairy-
 stockfish,stockfish,lichess,lichess.org,cli,san,uci Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Environment :: Console Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Games/Entertainment
-:: Board Games Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
-Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
-Audience :: Developers Classifier: Natural Language :: English Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Games/Entertainment :: Board Games Classifier: Topic :: Games/
+Entertainment :: Turn Based Strategy Classifier: Intended Audience :: End
+Users/Desktop Classifier: Intended Audience :: Developers Classifier: Natural
+Language :: English Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: dev License-File: LICENSE
   [https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-
                           45a2-97cb-6a25b5ca9c0c.png]
   A highly customizable way to play chess in your terminal. Supports playing
  online (via Lichess.org) and offline against the Fairy-Stockfish engine. All
                         Lichess variants are supported.
                          [CI_Workflow] [PyPI] [Python]
-## Main Features - Play online using your Lichess.org account - Play offline
-against the Fairy-Stockfish engine - Supports playing all Lichess [variants]
-(https://lichess.org/variant) - Theme the chess board and pieces to the colors
-of your choice - Theme UI components to the colors of your choice - Supports
-making moves in UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ##
-Getting started 1. Open your terminal and run `pip install cli-chess` 2. Type
-`cli-chess` to start 3. Use your keyboard arrows, tab, or click to navigate the
-menus. Multi value menu options (e.g. changing the variant) can be cycled by
-pressing spacebar, enter, or by clicking on the value. ## Playing Online In
-order to play online using your Lichess account you will need to create an API
-token for cli-chess to authenticate with. Follow the steps below to create the
-token and register it with cli-chess. Generally, these steps will only need to
-be run once as cli-chess will remember the API token. 1. Open your browser and
-login to your Lichess account 2. Click [here](https://lichess.org/account/
-oauth/token/create?scopes[]=board:play&scopes[]=challenge:read&scopes
-[]=challenge:write&description=cli-chess+token) to create a Lichess API token
-for cli-chess to authenticate with _(**NOTE**: Do not uncheck any of the token
-permissions as these are required by cli-chess)_ 3. Click "Create" 4. Highlight
-and copy the token 5. Run cli-chess using the following command: `cli-chess --
-token ****` _(replace *'s with your API token)_ ## Custom styling Nearly every
-component of cli-chess can be styled by overriding parts of the [default style
-elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/
-utils/styles.py) in the `custom_style.py` file. This file will be located at
+Demo Offline against Fairy-Stockfish | Watching Lichess Bullet TV :------------
+-------------:|:-------------------------: [https://user-
+images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-
+714e2a9c9c83.gif] | [https://user-images.githubusercontent.com/3620552/
+229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif]  ## Main Features - Play
+online using your Lichess.org account - Play offline against the Fairy-
+Stockfish engine - Supports playing all Lichess [variants](https://lichess.org/
+variant) - Theme the chess board and pieces to the colors of your choice -
+Theme UI components to the colors of your choice - Supports making moves in
+UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ## Getting started
+1. Open your terminal and run `pip install cli-chess` 2. Type `cli-chess` to
+start 3. Use your keyboard arrows, tab, or click to navigate the menus. Multi
+value menu options (e.g. changing the variant) can be cycled by pressing
+spacebar, enter, or by clicking on the value. ## Playing Online In order to
+play online using your Lichess account you will need to create an API token for
+cli-chess to authenticate with. Follow the steps below to create the token and
+register it with cli-chess. Generally, these steps will only need to be run
+once as cli-chess will remember the API token. 1. Open your browser and login
+to your Lichess account 2. Click [here](https://lichess.org/account/oauth/
+token/create?scopes[]=board:play&scopes[]=challenge:read&scopes[]=challenge:
+write&description=cli-chess+token) to create a Lichess API token for cli-chess
+to authenticate with _(**NOTE**: Do not uncheck any of the token permissions as
+these are required by cli-chess)_ 3. Click "Create" 4. Highlight and copy the
+token 5. Run cli-chess using the following command: `cli-chess --token ****` _
+(replace *'s with your API token)_ ## Custom styling Nearly every component of
+cli-chess can be styled by overriding parts of the [default style elements]
+(https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/
+styles.py) in the `custom_style.py` file. This file will be located at
 `$HOME/.config/cli-chess/` for Linux and macOS and `$APPDATA/cli-chess/` for
 Windows. Colors are expected to be [HTML color names](https://
 www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`) or [HTML hex
 colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`).
 The display of selected colors is dependent on the terminal supporting true
-colors and the `Terminal Color Depth` option in cli-chess program setting being
-set to `True Colors`). If the terminal does not support true colors, the colors
-selected will be mapped to the closest supported color. Restarting cli-chess,
-or pressing `Ctrl+R` on any screen will force a style refresh. If this custom
-style sheet is invalid in any way, the default cli-chess style will be applied.
-This file must be kept in dictionary format. Example `custom_style.py` to
-override board and piece colors: ```json { "light-square": "bg:wheat", "light-
-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black", "dark-
-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
+colors and the `Terminal Color Depth` option in cli-chess program settings
+being set to `True Colors`). If the terminal does not support true colors, the
+colors selected will be mapped to the closest supported color. Restarting cli-
+chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this
+custom style sheet is invalid in any way, the default cli-chess style will be
+applied. This file must be kept in dictionary format. Example `custom_style.py`
+to override board and piece colors: ```json { "light-square": "bg:wheat",
+"light-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black",
+"dark-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
 square.dark-piece": "fg:black", "last-move": "bg:slateblue", "last-move.light-
 piece": "fg:white", "last-move.dark-piece": "fg:black", "in-check": "bg:
 #FFA500", "in-check.light-piece": "fg:white", "in-check.dark-piece": "fg:black"
 } ``` ## Questions #### 1. How do I make a move? Moves are case-sensitive and
 must be made in SAN, LAN, or UCI. Moves cannot be made using the mouse. Pawn
 promotions must specify the promotion piece type (e.g. `e8=Q` or `e7e8q`).
 Moves that are ambiguous must specify the _from square_ when using SAN (e.g.
```

### Comparing `cli-chess-1.0.0/README.md` & `cli-chess-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,26 @@
     <a href="https://github.com/trevorbayless/cli-chess/actions/">
         <img alt="CI Workflow" src="https://github.com/trevorbayless/cli-chess/actions/workflows/ci.yml/badge.svg?branch=master&event=push">
     </a>
     <a href="https://pypi.org/project/cli-chess/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/cli-chess?color=informational&label=PyPI&logo=PyPI">
     </a>
     <a href="#">
-        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.7%2B&color=informational&logo=python">
+        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.8%2B&color=informational&logo=python">
     </a>
 </p>
 
+<details><summary>Demo</summary>
+
+Offline against Fairy-Stockfish            |  Watching Lichess Bullet TV
+:-------------------------:|:-------------------------:
+<img src=https://user-images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-714e2a9c9c83.gif width=450 width=222> | <img src=https://user-images.githubusercontent.com/3620552/229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif width=430 height=245>
+
+</details>
+
 ## Main Features
 - Play online using your Lichess.org account
 - Play offline against the Fairy-Stockfish engine
 - Supports playing all Lichess [variants](https://lichess.org/variant)
 - Theme the chess board and pieces to the colors of your choice
 - Theme UI components to the colors of your choice
 - Supports making moves in UCI, SAN, or LAN
@@ -54,15 +62,15 @@
 [default style elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/styles.py)
 in the `custom_style.py` file. This file will be located at `$HOME/.config/cli-chess/` for Linux and macOS and
 `$APPDATA/cli-chess/` for Windows.
 
 Colors are expected to be [HTML color names](https://www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`)
 or [HTML hex colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`). The display of selected
 colors is dependent on the terminal supporting true colors and the `Terminal Color Depth` option in cli-chess program
-setting being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
+settings being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
 to the closest supported color.
 
 Restarting cli-chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this custom style sheet is
 invalid in any way, the default cli-chess style will be applied. This file must be kept in dictionary format.
 
 Example `custom_style.py` to override board and piece colors:
 ```json
```

#### html2text {}

```diff
@@ -1,50 +1,55 @@
   [https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-
                           45a2-97cb-6a25b5ca9c0c.png]
   A highly customizable way to play chess in your terminal. Supports playing
  online (via Lichess.org) and offline against the Fairy-Stockfish engine. All
                         Lichess variants are supported.
                          [CI_Workflow] [PyPI] [Python]
-## Main Features - Play online using your Lichess.org account - Play offline
-against the Fairy-Stockfish engine - Supports playing all Lichess [variants]
-(https://lichess.org/variant) - Theme the chess board and pieces to the colors
-of your choice - Theme UI components to the colors of your choice - Supports
-making moves in UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ##
-Getting started 1. Open your terminal and run `pip install cli-chess` 2. Type
-`cli-chess` to start 3. Use your keyboard arrows, tab, or click to navigate the
-menus. Multi value menu options (e.g. changing the variant) can be cycled by
-pressing spacebar, enter, or by clicking on the value. ## Playing Online In
-order to play online using your Lichess account you will need to create an API
-token for cli-chess to authenticate with. Follow the steps below to create the
-token and register it with cli-chess. Generally, these steps will only need to
-be run once as cli-chess will remember the API token. 1. Open your browser and
-login to your Lichess account 2. Click [here](https://lichess.org/account/
-oauth/token/create?scopes[]=board:play&scopes[]=challenge:read&scopes
-[]=challenge:write&description=cli-chess+token) to create a Lichess API token
-for cli-chess to authenticate with _(**NOTE**: Do not uncheck any of the token
-permissions as these are required by cli-chess)_ 3. Click "Create" 4. Highlight
-and copy the token 5. Run cli-chess using the following command: `cli-chess --
-token ****` _(replace *'s with your API token)_ ## Custom styling Nearly every
-component of cli-chess can be styled by overriding parts of the [default style
-elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/
-utils/styles.py) in the `custom_style.py` file. This file will be located at
+Demo Offline against Fairy-Stockfish | Watching Lichess Bullet TV :------------
+-------------:|:-------------------------: [https://user-
+images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-
+714e2a9c9c83.gif] | [https://user-images.githubusercontent.com/3620552/
+229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif]  ## Main Features - Play
+online using your Lichess.org account - Play offline against the Fairy-
+Stockfish engine - Supports playing all Lichess [variants](https://lichess.org/
+variant) - Theme the chess board and pieces to the colors of your choice -
+Theme UI components to the colors of your choice - Supports making moves in
+UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ## Getting started
+1. Open your terminal and run `pip install cli-chess` 2. Type `cli-chess` to
+start 3. Use your keyboard arrows, tab, or click to navigate the menus. Multi
+value menu options (e.g. changing the variant) can be cycled by pressing
+spacebar, enter, or by clicking on the value. ## Playing Online In order to
+play online using your Lichess account you will need to create an API token for
+cli-chess to authenticate with. Follow the steps below to create the token and
+register it with cli-chess. Generally, these steps will only need to be run
+once as cli-chess will remember the API token. 1. Open your browser and login
+to your Lichess account 2. Click [here](https://lichess.org/account/oauth/
+token/create?scopes[]=board:play&scopes[]=challenge:read&scopes[]=challenge:
+write&description=cli-chess+token) to create a Lichess API token for cli-chess
+to authenticate with _(**NOTE**: Do not uncheck any of the token permissions as
+these are required by cli-chess)_ 3. Click "Create" 4. Highlight and copy the
+token 5. Run cli-chess using the following command: `cli-chess --token ****` _
+(replace *'s with your API token)_ ## Custom styling Nearly every component of
+cli-chess can be styled by overriding parts of the [default style elements]
+(https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/
+styles.py) in the `custom_style.py` file. This file will be located at
 `$HOME/.config/cli-chess/` for Linux and macOS and `$APPDATA/cli-chess/` for
 Windows. Colors are expected to be [HTML color names](https://
 www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`) or [HTML hex
 colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`).
 The display of selected colors is dependent on the terminal supporting true
-colors and the `Terminal Color Depth` option in cli-chess program setting being
-set to `True Colors`). If the terminal does not support true colors, the colors
-selected will be mapped to the closest supported color. Restarting cli-chess,
-or pressing `Ctrl+R` on any screen will force a style refresh. If this custom
-style sheet is invalid in any way, the default cli-chess style will be applied.
-This file must be kept in dictionary format. Example `custom_style.py` to
-override board and piece colors: ```json { "light-square": "bg:wheat", "light-
-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black", "dark-
-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
+colors and the `Terminal Color Depth` option in cli-chess program settings
+being set to `True Colors`). If the terminal does not support true colors, the
+colors selected will be mapped to the closest supported color. Restarting cli-
+chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this
+custom style sheet is invalid in any way, the default cli-chess style will be
+applied. This file must be kept in dictionary format. Example `custom_style.py`
+to override board and piece colors: ```json { "light-square": "bg:wheat",
+"light-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black",
+"dark-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
 square.dark-piece": "fg:black", "last-move": "bg:slateblue", "last-move.light-
 piece": "fg:white", "last-move.dark-piece": "fg:black", "in-check": "bg:
 #FFA500", "in-check.light-piece": "fg:white", "in-check.dark-piece": "fg:black"
 } ``` ## Questions #### 1. How do I make a move? Moves are case-sensitive and
 must be made in SAN, LAN, or UCI. Moves cannot be made using the mouse. Pawn
 promotions must specify the promotion piece type (e.g. `e8=Q` or `e7e8q`).
 Moves that are ambiguous must specify the _from square_ when using SAN (e.g.
```

### Comparing `cli-chess-1.0.0/setup.cfg` & `cli-chess-1.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows
 	Operating System :: MacOS
 	Environment :: Console
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Games/Entertainment :: Board Games
 	Topic :: Games/Entertainment :: Turn Based Strategy
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
 	Natural Language :: English
 
 [options]
 packages = find:
 package_dir = = src
-python_requires = >= 3.7
+python_requires = >= 3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `cli-chess-1.0.0/setup.py` & `cli-chess-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from re import findall
 
 metadata_file = open("src/cli_chess/__metadata__.py").read()
 metadata = dict(findall(r'__(\w*)__\s*=\s*"([^"]+)"', metadata_file))
 
 dependencies = [
     "chess>=1.9.4,<2.0.0",
-    "berserk-downstream>=0.11.12,<1.0.0",
+    "berserk>=0.12.0,<0.13.0",
     "prompt-toolkit==3.0.38"  # pin as breaking changes have been
                               # introduced in previous patch versions
                               # read PT changelog before bumping
 ]
 
 dev_dependencies = {
     'dev': [
```

### Comparing `cli-chess-1.0.0/src/cli_chess/__main__.py` & `cli-chess-1.0.1/src/cli_chess/__main__.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/__metadata__.py` & `cli-chess-1.0.1/src/cli_chess/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 Trevor Bayless <trevorbayless1@gmail.com>
+# Copyright (C) 2021-2023 Trevor Bayless <trevorbayless1@gmail.com>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = "cli-chess"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __description__ = "A highly customizable way to play chess in your terminal"
 __url__ = "https://github.com/trevorbayless/cli-chess"
 __author__ = "Trevor Bayless"
 __author_email__ = "trevorbayless1@gmail.com"
 __license__ = "GPL-3.0+"
```

### Comparing `cli-chess-1.0.0/src/cli_chess/core/api/api_manager.py` & `cli-chess-1.0.1/src/cli_chess/core/api/api_manager.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/api/game_state_dispatcher.py` & `cli-chess-1.0.1/src/cli_chess/core/api/game_state_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/api/incoming_event_manger.py` & `cli-chess-1.0.1/src/cli_chess/core/api/incoming_event_manger.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/game_model_base.py` & `cli-chess-1.0.1/src/cli_chess/core/game/game_model_base.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/game_options.py` & `cli-chess-1.0.1/src/cli_chess/core/game/game_options.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/game_presenter_base.py` & `cli-chess-1.0.1/src/cli_chess/core/game/game_presenter_base.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/game_view_base.py` & `cli-chess-1.0.1/src/cli_chess/core/game/game_view_base.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_model.py` & `cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_presenter.py` & `cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/offline_game/offline_game_view.py` & `cli-chess-1.0.1/src/cli_chess/core/game/offline_game/offline_game_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_model.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             #  add some further specific clauses like color, time control, date, etc?
             if not self.game_in_progress and not event.get('hasMoved') and event.get('compat', {}).get('board'):
                 self._save_game_metadata(iem_gameStart=event)
                 self._start_game(event.get('gameId'))
 
         elif 'gameFinish' in kwargs:
             event = kwargs['gameFinish'].get('game')
+            self._save_game_metadata(iem_gameFinish=event)
             if self.game_in_progress and self.playing_game_id == event.get('gameId'):
                 self._game_end()
 
     def handle_game_state_dispatcher_event(self, **kwargs) -> None:
         """Handles received from the GameStateDispatcher"""
         if 'gameFull' in kwargs:
             event = kwargs['gameFull']
@@ -237,14 +238,19 @@
                 data = kwargs['iem_gameStart']
                 self.game_metadata['gameId'] = data.get('gameId')
                 self.game_metadata['my_color_str'] = data.get('color')
                 self.game_metadata['rated'] = data.get('rated')
                 self.game_metadata['variant'] = data.get('variant', {}).get('name')
                 self.game_metadata['speed'] = data['speed']
 
+            elif 'iem_gameFinish' in kwargs:
+                data = kwargs['iem_gameFinish']
+                self.game_metadata['players'][COLOR_NAMES[self.my_color]]['rating_diff'] = data.get('ratingDiff', "")
+                self.game_metadata['players'][COLOR_NAMES[not self.my_color]]['rating_diff'] = data.get('opponent', {}).get('ratingDiff', "")
+
             elif 'gsd_gameFull' in kwargs:
                 data = kwargs['gsd_gameFull']
 
                 for color in COLOR_NAMES:
                     if data.get(color, {}).get('name'):
                         self.game_metadata['players'][color]['title'] = data.get(color, {}).get('title')
                         self.game_metadata['players'][color]['name'] = data.get(color, {}).get('name', "?")
```

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_presenter.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/online_game_view.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/online_game_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py` & `cli-chess-1.0.1/src/cli_chess/core/game/online_game/watch_tv/watch_tv_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/main/main_model.py` & `cli-chess-1.0.1/src/cli_chess/core/main/main_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/main/main_presenter.py` & `cli-chess-1.0.1/src/cli_chess/core/main/main_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/core/main/main_view.py` & `cli-chess-1.0.1/src/cli_chess/core/main/main_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/main_menu/main_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/main_menu/main_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/menu_common.py` & `cli-chess-1.0.1/src/cli_chess/menus/menu_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/offline_games_menu/offline_games_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/online_games_menu/online_games_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/online_games_menu/online_games_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/program_settings_menu/program_settings_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/settings_menu/settings_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/settings_menu/settings_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py` & `cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py` & `cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py` & `cli-chess-1.0.1/src/cli_chess/menus/tv_channel_menu/tv_channel_menu_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_models.py` & `cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_models.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_presenters.py` & `cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_presenters.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/menus/versus_menus/versus_menu_views.py` & `cli-chess-1.0.1/src/cli_chess/menus/versus_menus/versus_menu_views.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/about/about_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/about/about_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/about/about_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/about/about_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/board/board_model.py` & `cli-chess-1.0.1/src/cli_chess/modules/board/board_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/board/board_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/board/board_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/board/board_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/board/board_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/clock/clock_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/clock/clock_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/clock/clock_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/clock/clock_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/common.py` & `cli-chess-1.0.1/src/cli_chess/modules/common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos` & `cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_arm64_macos`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux` & `cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_linux`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos` & `cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_macos`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe` & `cli-chess-1.0.1/src/cli_chess/modules/engine/binaries/fairy-stockfish_x86-64_windows.exe`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/engine_model.py` & `cli-chess-1.0.1/src/cli_chess/modules/engine/engine_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/engine/engine_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/engine/engine_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_model.py` & `cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/material_difference/material_difference_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/material_difference/material_difference_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_model.py` & `cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/move_list/move_list_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/move_list/move_list_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/player_info/player_info_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/player_info/player_info_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/player_info/player_info_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/player_info/player_info_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_model.py` & `cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_presenter.py` & `cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/modules/token_manager/token_manager_view.py` & `cli-chess-1.0.1/src/cli_chess/modules/token_manager/token_manager_view.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/board/test_board_model.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/board/test_board_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/board/test_board_presenter.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/board/test_board_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/test_material_difference_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/material_difference/test_material_difference_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/test_move_list_model.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/test_move_list_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/move_list/test_move_list_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/test_common.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/test_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/test_token_manager_model.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py` & `cli-chess-1.0.1/src/cli_chess/tests/modules/token_manager/test_token_manager_presenter.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/tests/utils/test_event.py` & `cli-chess-1.0.1/src/cli_chess/tests/utils/test_event.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/argparse.py` & `cli-chess-1.0.1/src/cli_chess/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/common.py` & `cli-chess-1.0.1/src/cli_chess/utils/common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/config.py` & `cli-chess-1.0.1/src/cli_chess/utils/config.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/event.py` & `cli-chess-1.0.1/src/cli_chess/utils/event.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/logging.py` & `cli-chess-1.0.1/src/cli_chess/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/styles.py` & `cli-chess-1.0.1/src/cli_chess/utils/styles.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess/utils/ui_common.py` & `cli-chess-1.0.1/src/cli_chess/utils/ui_common.py`

 * *Files identical despite different names*

### Comparing `cli-chess-1.0.0/src/cli_chess.egg-info/PKG-INFO` & `cli-chess-1.0.1/src/cli_chess.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: cli-chess
-Version: 1.0.0
+Version: 1.0.1
 Summary: A highly customizable way to play chess in your terminal
 Home-page: https://github.com/trevorbayless/cli-chess
 Author: Trevor Bayless
 Author-email: trevorbayless1@gmail.com
 License: GPL-3.0+
 Keywords: chess,terminal,fairy-stockfish,stockfish,lichess,lichess.org,cli,san,uci
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-45a2-97cb-6a25b5ca9c0c.png"/></a>
 </p>
@@ -42,18 +41,26 @@
     <a href="https://github.com/trevorbayless/cli-chess/actions/">
         <img alt="CI Workflow" src="https://github.com/trevorbayless/cli-chess/actions/workflows/ci.yml/badge.svg?branch=master&event=push">
     </a>
     <a href="https://pypi.org/project/cli-chess/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/cli-chess?color=informational&label=PyPI&logo=PyPI">
     </a>
     <a href="#">
-        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.7%2B&color=informational&logo=python">
+        <img alt="Python" src="https://img.shields.io/static/v1?label=Python&message=3.8%2B&color=informational&logo=python">
     </a>
 </p>
 
+<details><summary>Demo</summary>
+
+Offline against Fairy-Stockfish            |  Watching Lichess Bullet TV
+:-------------------------:|:-------------------------:
+<img src=https://user-images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-714e2a9c9c83.gif width=450 width=222> | <img src=https://user-images.githubusercontent.com/3620552/229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif width=430 height=245>
+
+</details>
+
 ## Main Features
 - Play online using your Lichess.org account
 - Play offline against the Fairy-Stockfish engine
 - Supports playing all Lichess [variants](https://lichess.org/variant)
 - Theme the chess board and pieces to the colors of your choice
 - Theme UI components to the colors of your choice
 - Supports making moves in UCI, SAN, or LAN
@@ -85,15 +92,15 @@
 [default style elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/styles.py)
 in the `custom_style.py` file. This file will be located at `$HOME/.config/cli-chess/` for Linux and macOS and
 `$APPDATA/cli-chess/` for Windows.
 
 Colors are expected to be [HTML color names](https://www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`)
 or [HTML hex colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`). The display of selected
 colors is dependent on the terminal supporting true colors and the `Terminal Color Depth` option in cli-chess program
-setting being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
+settings being set to `True Colors`). If the terminal does not support true colors, the colors selected will be mapped
 to the closest supported color.
 
 Restarting cli-chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this custom style sheet is
 invalid in any way, the default cli-chess style will be applied. This file must be kept in dictionary format.
 
 Example `custom_style.py` to override board and piece colors:
 ```json
```

#### html2text {}

```diff
@@ -1,68 +1,72 @@
-Metadata-Version: 2.1 Name: cli-chess Version: 1.0.0 Summary: A highly
+Metadata-Version: 2.1 Name: cli-chess Version: 1.0.1 Summary: A highly
 customizable way to play chess in your terminal Home-page: https://github.com/
 trevorbayless/cli-chess Author: Trevor Bayless Author-email:
 trevorbayless1@gmail.com License: GPL-3.0+ Keywords: chess,terminal,fairy-
 stockfish,stockfish,lichess,lichess.org,cli,san,uci Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Environment :: Console Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Games/Entertainment
-:: Board Games Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
-Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
-Audience :: Developers Classifier: Natural Language :: English Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Games/Entertainment :: Board Games Classifier: Topic :: Games/
+Entertainment :: Turn Based Strategy Classifier: Intended Audience :: End
+Users/Desktop Classifier: Intended Audience :: Developers Classifier: Natural
+Language :: English Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: dev License-File: LICENSE
   [https://user-images.githubusercontent.com/3620552/214357735-53c2174c-5ada-
                           45a2-97cb-6a25b5ca9c0c.png]
   A highly customizable way to play chess in your terminal. Supports playing
  online (via Lichess.org) and offline against the Fairy-Stockfish engine. All
                         Lichess variants are supported.
                          [CI_Workflow] [PyPI] [Python]
-## Main Features - Play online using your Lichess.org account - Play offline
-against the Fairy-Stockfish engine - Supports playing all Lichess [variants]
-(https://lichess.org/variant) - Theme the chess board and pieces to the colors
-of your choice - Theme UI components to the colors of your choice - Supports
-making moves in UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ##
-Getting started 1. Open your terminal and run `pip install cli-chess` 2. Type
-`cli-chess` to start 3. Use your keyboard arrows, tab, or click to navigate the
-menus. Multi value menu options (e.g. changing the variant) can be cycled by
-pressing spacebar, enter, or by clicking on the value. ## Playing Online In
-order to play online using your Lichess account you will need to create an API
-token for cli-chess to authenticate with. Follow the steps below to create the
-token and register it with cli-chess. Generally, these steps will only need to
-be run once as cli-chess will remember the API token. 1. Open your browser and
-login to your Lichess account 2. Click [here](https://lichess.org/account/
-oauth/token/create?scopes[]=board:play&scopes[]=challenge:read&scopes
-[]=challenge:write&description=cli-chess+token) to create a Lichess API token
-for cli-chess to authenticate with _(**NOTE**: Do not uncheck any of the token
-permissions as these are required by cli-chess)_ 3. Click "Create" 4. Highlight
-and copy the token 5. Run cli-chess using the following command: `cli-chess --
-token ****` _(replace *'s with your API token)_ ## Custom styling Nearly every
-component of cli-chess can be styled by overriding parts of the [default style
-elements](https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/
-utils/styles.py) in the `custom_style.py` file. This file will be located at
+Demo Offline against Fairy-Stockfish | Watching Lichess Bullet TV :------------
+-------------:|:-------------------------: [https://user-
+images.githubusercontent.com/3620552/229156062-309d5ae9-bcc2-43bc-ab4c-
+714e2a9c9c83.gif] | [https://user-images.githubusercontent.com/3620552/
+229156269-8a0bb436-ab9e-4e55-9218-b488e5a2eccb.gif]  ## Main Features - Play
+online using your Lichess.org account - Play offline against the Fairy-
+Stockfish engine - Supports playing all Lichess [variants](https://lichess.org/
+variant) - Theme the chess board and pieces to the colors of your choice -
+Theme UI components to the colors of your choice - Supports making moves in
+UCI, SAN, or LAN - Play blindfold chess - Watch Lichess TV ## Getting started
+1. Open your terminal and run `pip install cli-chess` 2. Type `cli-chess` to
+start 3. Use your keyboard arrows, tab, or click to navigate the menus. Multi
+value menu options (e.g. changing the variant) can be cycled by pressing
+spacebar, enter, or by clicking on the value. ## Playing Online In order to
+play online using your Lichess account you will need to create an API token for
+cli-chess to authenticate with. Follow the steps below to create the token and
+register it with cli-chess. Generally, these steps will only need to be run
+once as cli-chess will remember the API token. 1. Open your browser and login
+to your Lichess account 2. Click [here](https://lichess.org/account/oauth/
+token/create?scopes[]=board:play&scopes[]=challenge:read&scopes[]=challenge:
+write&description=cli-chess+token) to create a Lichess API token for cli-chess
+to authenticate with _(**NOTE**: Do not uncheck any of the token permissions as
+these are required by cli-chess)_ 3. Click "Create" 4. Highlight and copy the
+token 5. Run cli-chess using the following command: `cli-chess --token ****` _
+(replace *'s with your API token)_ ## Custom styling Nearly every component of
+cli-chess can be styled by overriding parts of the [default style elements]
+(https://github.com/trevorbayless/cli-chess/blob/master/src/cli_chess/utils/
+styles.py) in the `custom_style.py` file. This file will be located at
 `$HOME/.config/cli-chess/` for Linux and macOS and `$APPDATA/cli-chess/` for
 Windows. Colors are expected to be [HTML color names](https://
 www.w3schools.com/tags/ref_colornames.asp) (e.g. `seagreen`) or [HTML hex
 colors](https://www.w3schools.com/colors/colors_picker.asp) (e.g. `#2E8B57`).
 The display of selected colors is dependent on the terminal supporting true
-colors and the `Terminal Color Depth` option in cli-chess program setting being
-set to `True Colors`). If the terminal does not support true colors, the colors
-selected will be mapped to the closest supported color. Restarting cli-chess,
-or pressing `Ctrl+R` on any screen will force a style refresh. If this custom
-style sheet is invalid in any way, the default cli-chess style will be applied.
-This file must be kept in dictionary format. Example `custom_style.py` to
-override board and piece colors: ```json { "light-square": "bg:wheat", "light-
-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black", "dark-
-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
+colors and the `Terminal Color Depth` option in cli-chess program settings
+being set to `True Colors`). If the terminal does not support true colors, the
+colors selected will be mapped to the closest supported color. Restarting cli-
+chess, or pressing `Ctrl+R` on any screen will force a style refresh. If this
+custom style sheet is invalid in any way, the default cli-chess style will be
+applied. This file must be kept in dictionary format. Example `custom_style.py`
+to override board and piece colors: ```json { "light-square": "bg:wheat",
+"light-square.light-piece": "fg:white", "light-square.dark-piece": "fg:black",
+"dark-square": "bg:#2E8B57", "dark-square.light-piece": "fg:white", "dark-
 square.dark-piece": "fg:black", "last-move": "bg:slateblue", "last-move.light-
 piece": "fg:white", "last-move.dark-piece": "fg:black", "in-check": "bg:
 #FFA500", "in-check.light-piece": "fg:white", "in-check.dark-piece": "fg:black"
 } ``` ## Questions #### 1. How do I make a move? Moves are case-sensitive and
 must be made in SAN, LAN, or UCI. Moves cannot be made using the mouse. Pawn
 promotions must specify the promotion piece type (e.g. `e8=Q` or `e7e8q`).
 Moves that are ambiguous must specify the _from square_ when using SAN (e.g.
```

### Comparing `cli-chess-1.0.0/src/cli_chess.egg-info/SOURCES.txt` & `cli-chess-1.0.1/src/cli_chess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

