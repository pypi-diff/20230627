# Comparing `tmp/vis-lab-1.0.0.tar.gz` & `tmp/vis-lab-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis-lab-1.0.0.tar", last modified: Tue Jun 27 01:44:53 2023, max compression
+gzip compressed data, was "vis-lab-1.0.1.tar", last modified: Tue Jun 27 01:50:39 2023, max compression
```

## Comparing `vis-lab-1.0.0.tar` & `vis-lab-1.0.1.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.215737 vis-lab-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)     1053 2023-06-09 09:07:03.000000 vis-lab-1.0.0/LICENCE.txt
--rw-r--r--   0 mac        (501) staff       (20)      664 2023-06-27 01:44:53.215570 vis-lab-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     4616 2023-06-26 06:18:07.000000 vis-lab-1.0.0/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-27 01:44:53.215810 vis-lab-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      896 2023-06-27 01:44:51.000000 vis-lab-1.0.0/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.192442 vis-lab-1.0.0/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.192782 vis-lab-1.0.0/src/Agent/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.193158 vis-lab-1.0.0/src/Agent/ActionsLayer/
--rw-r--r--   0 mac        (501) staff       (20)     1712 2023-06-18 21:45:14.000000 vis-lab-1.0.0/src/Agent/ActionsLayer/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/ActionsLayer/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.193596 vis-lab-1.0.0/src/Agent/An/
--rw-r--r--   0 mac        (501) staff       (20)     5835 2023-06-18 21:45:32.000000 vis-lab-1.0.0/src/Agent/An/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/An/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.194047 vis-lab-1.0.0/src/Agent/BasicModeling/
--rw-r--r--   0 mac        (501) staff       (20)     7172 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/BasicModeling/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/BasicModeling/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.196742 vis-lab-1.0.0/src/Agent/BiasAlgorithm/
--rw-r--r--   0 mac        (501) staff       (20)     1090 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/BiasAlgorithm/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/BiasAlgorithm/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.197495 vis-lab-1.0.0/src/Agent/Chain3/
--rw-r--r--   0 mac        (501) staff       (20)     8504 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/Chain3/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/Chain3/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.197984 vis-lab-1.0.0/src/Agent/Chain4/
--rw-r--r--   0 mac        (501) staff       (20)     7827 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/Chain4/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/Chain4/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.198103 vis-lab-1.0.0/src/Agent/Ifelse/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/Ifelse/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.198511 vis-lab-1.0.0/src/Agent/KhanhNhat/
--rw-r--r--   0 mac        (501) staff       (20)     3095 2023-06-18 21:45:32.000000 vis-lab-1.0.0/src/Agent/KhanhNhat/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/KhanhNhat/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.199270 vis-lab-1.0.0/src/Agent/MultiDimensionAlgorithm/
--rw-r--r--   0 mac        (501) staff       (20)     1937 2023-06-18 21:45:33.000000 vis-lab-1.0.0/src/Agent/MultiDimensionAlgorithm/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/MultiDimensionAlgorithm/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.200117 vis-lab-1.0.0/src/Agent/StateBasedAlgorithm/
--rw-r--r--   0 mac        (501) staff       (20)     3118 2023-06-18 21:45:32.000000 vis-lab-1.0.0/src/Agent/StateBasedAlgorithm/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/StateBasedAlgorithm/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.200520 vis-lab-1.0.0/src/Agent/StateLayer/
--rw-r--r--   0 mac        (501) staff       (20)     6360 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/StateLayer/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/StateLayer/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.200924 vis-lab-1.0.0/src/Agent/TimeBasedAlgorithm/
--rw-r--r--   0 mac        (501) staff       (20)     2064 2023-06-18 21:45:34.000000 vis-lab-1.0.0/src/Agent/TimeBasedAlgorithm/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/TimeBasedAlgorithm/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.201220 vis-lab-1.0.0/src/Agent/Y_random/
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-06-18 21:45:33.000000 vis-lab-1.0.0/src/Agent/Y_random/Agent_player.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/Y_random/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Agent/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.201324 vis-lab-1.0.0/src/Base/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.202000 vis-lab-1.0.0/src/Base/Catan/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Catan/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24417 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Catan/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    66817 2023-06-18 22:16:01.000000 vis-lab-1.0.0/src/Base/Catan/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.202892 vis-lab-1.0.0/src/Base/CatanNoExchange/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/CatanNoExchange/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    23763 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/CatanNoExchange/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    69136 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/CatanNoExchange/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.203618 vis-lab-1.0.0/src/Base/Century/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Century/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    15962 2023-06-18 22:16:00.000000 vis-lab-1.0.0/src/Base/Century/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    36653 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Century/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.204267 vis-lab-1.0.0/src/Base/Durak/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Durak/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8221 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Durak/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    15493 2023-06-18 22:16:00.000000 vis-lab-1.0.0/src/Base/Durak/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.204981 vis-lab-1.0.0/src/Base/Exploding_Kitten/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Exploding_Kitten/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9398 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Exploding_Kitten/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    33353 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Exploding_Kitten/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.205684 vis-lab-1.0.0/src/Base/GoFish/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/GoFish/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8922 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/GoFish/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    15988 2023-06-18 21:47:28.000000 vis-lab-1.0.0/src/Base/GoFish/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.206439 vis-lab-1.0.0/src/Base/Imploding_Kitten/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Imploding_Kitten/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    11790 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Imploding_Kitten/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    41253 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Imploding_Kitten/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.207031 vis-lab-1.0.0/src/Base/MachiKoro/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/MachiKoro/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    12982 2023-06-18 22:16:00.000000 vis-lab-1.0.0/src/Base/MachiKoro/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    36375 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/MachiKoro/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.207693 vis-lab-1.0.0/src/Base/Poker/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Poker/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    13636 2023-06-18 22:16:00.000000 vis-lab-1.0.0/src/Base/Poker/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    49159 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Poker/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.208402 vis-lab-1.0.0/src/Base/Sheriff/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.0/src/Base/Sheriff/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    13321 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Sheriff/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    46314 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Sheriff/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.209027 vis-lab-1.0.0/src/Base/Splendor/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/Splendor/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    10120 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    24365 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.209857 vis-lab-1.0.0/src/Base/Splendor_v2/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/Splendor_v2/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    13681 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor_v2/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    31897 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor_v2/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.210477 vis-lab-1.0.0/src/Base/Splendor_v3/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/Splendor_v3/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    13029 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor_v3/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    34940 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/Splendor_v3/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.211166 vis-lab-1.0.0/src/Base/SushiGo/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/SushiGo/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8839 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/SushiGo/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    22231 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/SushiGo/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.212178 vis-lab-1.0.0/src/Base/TLMN/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/TLMN/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7203 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/TLMN/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    28063 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/TLMN/env.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.212850 vis-lab-1.0.0/src/Base/TicketToRide/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/TicketToRide/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    18560 2023-06-18 22:16:01.000000 vis-lab-1.0.0/src/Base/TicketToRide/_render_func.py
--rw-r--r--   0 mac        (501) staff       (20)    60618 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/Base/TicketToRide/env.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/src/Base/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      873 2023-06-18 22:16:01.000000 vis-lab-1.0.0/src/Utils.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-15 07:34:10.000000 vis-lab-1.0.0/src/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1476 2023-06-18 22:16:01.000000 vis-lab-1.0.0/src/env.py
--rw-r--r--   0 mac        (501) staff       (20)     8673 2023-06-18 21:45:56.000000 vis-lab-1.0.0/src/render_template.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.214362 vis-lab-1.0.0/tests/
--rw-r--r--   0 mac        (501) staff       (20)     6598 2023-06-18 22:26:56.000000 vis-lab-1.0.0/tests/CheckEnv.py
--rw-r--r--   0 mac        (501) staff       (20)      897 2023-06-18 22:28:45.000000 vis-lab-1.0.0/tests/CheckGraphics.py
--rw-r--r--   0 mac        (501) staff       (20)     2132 2023-06-18 22:28:28.000000 vis-lab-1.0.0/tests/CheckPlayer.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.0/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      105 2023-06-09 09:07:04.000000 vis-lab-1.0.0/tests/conftest.py
--rw-r--r--   0 mac        (501) staff       (20)     1873 2023-06-09 09:07:04.000000 vis-lab-1.0.0/tests/test_agent.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:44:53.215302 vis-lab-1.0.0/vis_lab.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      664 2023-06-27 01:44:53.000000 vis-lab-1.0.0/vis_lab.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2787 2023-06-27 01:44:53.000000 vis-lab-1.0.0/vis_lab.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-27 01:44:53.000000 vis-lab-1.0.0/vis_lab.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-27 01:44:53.000000 vis-lab-1.0.0/vis_lab.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-27 01:44:53.000000 vis-lab-1.0.0/vis_lab.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.602333 vis-lab-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)     1053 2023-06-09 09:07:03.000000 vis-lab-1.0.1/LICENCE.txt
+-rw-r--r--   0 mac        (501) staff       (20)      664 2023-06-27 01:50:39.602166 vis-lab-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     4616 2023-06-26 06:18:07.000000 vis-lab-1.0.1/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.582278 vis-lab-1.0.1/docs/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-27 01:49:45.000000 vis-lab-1.0.1/docs/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-27 01:50:39.602391 vis-lab-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      896 2023-06-27 01:50:35.000000 vis-lab-1.0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.583001 vis-lab-1.0.1/src/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.583364 vis-lab-1.0.1/src/Agent/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.583735 vis-lab-1.0.1/src/Agent/ActionsLayer/
+-rw-r--r--   0 mac        (501) staff       (20)     1712 2023-06-18 21:45:14.000000 vis-lab-1.0.1/src/Agent/ActionsLayer/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/ActionsLayer/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.584122 vis-lab-1.0.1/src/Agent/An/
+-rw-r--r--   0 mac        (501) staff       (20)     5835 2023-06-18 21:45:32.000000 vis-lab-1.0.1/src/Agent/An/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/An/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.584505 vis-lab-1.0.1/src/Agent/BasicModeling/
+-rw-r--r--   0 mac        (501) staff       (20)     7172 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/BasicModeling/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/BasicModeling/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.584895 vis-lab-1.0.1/src/Agent/BiasAlgorithm/
+-rw-r--r--   0 mac        (501) staff       (20)     1090 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/BiasAlgorithm/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/BiasAlgorithm/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.585270 vis-lab-1.0.1/src/Agent/Chain3/
+-rw-r--r--   0 mac        (501) staff       (20)     8504 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/Chain3/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/Chain3/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.585638 vis-lab-1.0.1/src/Agent/Chain4/
+-rw-r--r--   0 mac        (501) staff       (20)     7827 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/Chain4/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/Chain4/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.585745 vis-lab-1.0.1/src/Agent/Ifelse/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/Ifelse/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.586130 vis-lab-1.0.1/src/Agent/KhanhNhat/
+-rw-r--r--   0 mac        (501) staff       (20)     3095 2023-06-18 21:45:32.000000 vis-lab-1.0.1/src/Agent/KhanhNhat/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/KhanhNhat/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.586491 vis-lab-1.0.1/src/Agent/MultiDimensionAlgorithm/
+-rw-r--r--   0 mac        (501) staff       (20)     1937 2023-06-18 21:45:33.000000 vis-lab-1.0.1/src/Agent/MultiDimensionAlgorithm/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/MultiDimensionAlgorithm/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.586889 vis-lab-1.0.1/src/Agent/StateBasedAlgorithm/
+-rw-r--r--   0 mac        (501) staff       (20)     3118 2023-06-18 21:45:32.000000 vis-lab-1.0.1/src/Agent/StateBasedAlgorithm/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/StateBasedAlgorithm/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.587373 vis-lab-1.0.1/src/Agent/StateLayer/
+-rw-r--r--   0 mac        (501) staff       (20)     6360 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/StateLayer/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/StateLayer/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.587686 vis-lab-1.0.1/src/Agent/TimeBasedAlgorithm/
+-rw-r--r--   0 mac        (501) staff       (20)     2064 2023-06-18 21:45:34.000000 vis-lab-1.0.1/src/Agent/TimeBasedAlgorithm/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/TimeBasedAlgorithm/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.587984 vis-lab-1.0.1/src/Agent/Y_random/
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-06-18 21:45:33.000000 vis-lab-1.0.1/src/Agent/Y_random/Agent_player.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/Y_random/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Agent/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.588107 vis-lab-1.0.1/src/Base/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.589050 vis-lab-1.0.1/src/Base/Catan/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Catan/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    24417 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Catan/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    66817 2023-06-18 22:16:01.000000 vis-lab-1.0.1/src/Base/Catan/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.589938 vis-lab-1.0.1/src/Base/CatanNoExchange/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/CatanNoExchange/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    23763 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/CatanNoExchange/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    69136 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/CatanNoExchange/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.590593 vis-lab-1.0.1/src/Base/Century/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Century/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    15962 2023-06-18 22:16:00.000000 vis-lab-1.0.1/src/Base/Century/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    36653 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Century/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.591163 vis-lab-1.0.1/src/Base/Durak/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Durak/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8221 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Durak/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    15493 2023-06-18 22:16:00.000000 vis-lab-1.0.1/src/Base/Durak/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.591739 vis-lab-1.0.1/src/Base/Exploding_Kitten/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Exploding_Kitten/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     9398 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Exploding_Kitten/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    33353 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Exploding_Kitten/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.592296 vis-lab-1.0.1/src/Base/GoFish/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/GoFish/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8922 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/GoFish/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    15988 2023-06-18 21:47:28.000000 vis-lab-1.0.1/src/Base/GoFish/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.592951 vis-lab-1.0.1/src/Base/Imploding_Kitten/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Imploding_Kitten/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    11790 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Imploding_Kitten/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    41253 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Imploding_Kitten/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.593579 vis-lab-1.0.1/src/Base/MachiKoro/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/MachiKoro/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    12982 2023-06-18 22:16:00.000000 vis-lab-1.0.1/src/Base/MachiKoro/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    36375 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/MachiKoro/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.594300 vis-lab-1.0.1/src/Base/Poker/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Poker/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    13636 2023-06-18 22:16:00.000000 vis-lab-1.0.1/src/Base/Poker/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    49159 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Poker/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.594966 vis-lab-1.0.1/src/Base/Sheriff/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:03.000000 vis-lab-1.0.1/src/Base/Sheriff/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    13321 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Sheriff/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    46314 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Sheriff/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.595696 vis-lab-1.0.1/src/Base/Splendor/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/Splendor/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    10120 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    24365 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.596672 vis-lab-1.0.1/src/Base/Splendor_v2/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/Splendor_v2/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    13681 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor_v2/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    31897 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor_v2/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.597265 vis-lab-1.0.1/src/Base/Splendor_v3/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/Splendor_v3/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    13029 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor_v3/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    34940 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/Splendor_v3/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.597919 vis-lab-1.0.1/src/Base/SushiGo/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/SushiGo/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8839 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/SushiGo/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    22231 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/SushiGo/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.598564 vis-lab-1.0.1/src/Base/TLMN/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/TLMN/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     7203 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/TLMN/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    28063 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/TLMN/env.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.599146 vis-lab-1.0.1/src/Base/TicketToRide/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/TicketToRide/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    18560 2023-06-18 22:16:01.000000 vis-lab-1.0.1/src/Base/TicketToRide/_render_func.py
+-rw-r--r--   0 mac        (501) staff       (20)    60618 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/Base/TicketToRide/env.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/src/Base/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      873 2023-06-18 22:16:01.000000 vis-lab-1.0.1/src/Utils.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-15 07:34:10.000000 vis-lab-1.0.1/src/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1476 2023-06-18 22:16:01.000000 vis-lab-1.0.1/src/env.py
+-rw-r--r--   0 mac        (501) staff       (20)     8673 2023-06-18 21:45:56.000000 vis-lab-1.0.1/src/render_template.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.600791 vis-lab-1.0.1/tests/
+-rw-r--r--   0 mac        (501) staff       (20)     6598 2023-06-18 22:26:56.000000 vis-lab-1.0.1/tests/CheckEnv.py
+-rw-r--r--   0 mac        (501) staff       (20)      897 2023-06-18 22:28:45.000000 vis-lab-1.0.1/tests/CheckGraphics.py
+-rw-r--r--   0 mac        (501) staff       (20)     2132 2023-06-18 22:28:28.000000 vis-lab-1.0.1/tests/CheckPlayer.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-09 09:07:04.000000 vis-lab-1.0.1/tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      105 2023-06-09 09:07:04.000000 vis-lab-1.0.1/tests/conftest.py
+-rw-r--r--   0 mac        (501) staff       (20)     1873 2023-06-09 09:07:04.000000 vis-lab-1.0.1/tests/test_agent.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-27 01:50:39.601861 vis-lab-1.0.1/vis_lab.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      664 2023-06-27 01:50:39.000000 vis-lab-1.0.1/vis_lab.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2804 2023-06-27 01:50:39.000000 vis-lab-1.0.1/vis_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-27 01:50:39.000000 vis-lab-1.0.1/vis_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-27 01:50:39.000000 vis-lab-1.0.1/vis_lab.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       15 2023-06-27 01:50:39.000000 vis-lab-1.0.1/vis_lab.egg-info/top_level.txt
```

### Comparing `vis-lab-1.0.0/LICENCE.txt` & `vis-lab-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/PKG-INFO` & `vis-lab-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vis-lab
-Version: 1.0.0
+Version: 1.0.1
 Summary: a system reinforcement learning
 Home-page: 
 Author: Ngo Xuan Phong
 Author-email: phong@vis-laboratory.com
 License: MIT
 Keywords: vis_game
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vis-lab-1.0.0/README.md` & `vis-lab-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/setup.py` & `vis-lab-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
 ]
  
 setup(
   name='vis-lab',
-  version='1.0.0',
+  version='1.0.1',
   description='a system reinforcement learning',
   url='',  
   author='Ngo Xuan Phong',
   author_email='phong@vis-laboratory.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='vis_game',
```

### Comparing `vis-lab-1.0.0/src/Agent/ActionsLayer/Agent_player.py` & `vis-lab-1.0.1/src/Agent/ActionsLayer/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/An/Agent_player.py` & `vis-lab-1.0.1/src/Agent/An/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/BasicModeling/Agent_player.py` & `vis-lab-1.0.1/src/Agent/BasicModeling/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/BiasAlgorithm/Agent_player.py` & `vis-lab-1.0.1/src/Agent/BiasAlgorithm/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/Chain3/Agent_player.py` & `vis-lab-1.0.1/src/Agent/Chain3/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/Chain4/Agent_player.py` & `vis-lab-1.0.1/src/Agent/Chain4/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/KhanhNhat/Agent_player.py` & `vis-lab-1.0.1/src/Agent/KhanhNhat/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/MultiDimensionAlgorithm/Agent_player.py` & `vis-lab-1.0.1/src/Agent/MultiDimensionAlgorithm/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/StateBasedAlgorithm/Agent_player.py` & `vis-lab-1.0.1/src/Agent/StateBasedAlgorithm/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/StateLayer/Agent_player.py` & `vis-lab-1.0.1/src/Agent/StateLayer/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Agent/TimeBasedAlgorithm/Agent_player.py` & `vis-lab-1.0.1/src/Agent/TimeBasedAlgorithm/Agent_player.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Catan/_render_func.py` & `vis-lab-1.0.1/src/Base/Catan/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Catan/env.py` & `vis-lab-1.0.1/src/Base/Catan/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/CatanNoExchange/_render_func.py` & `vis-lab-1.0.1/src/Base/CatanNoExchange/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/CatanNoExchange/env.py` & `vis-lab-1.0.1/src/Base/CatanNoExchange/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Century/_render_func.py` & `vis-lab-1.0.1/src/Base/Century/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Century/env.py` & `vis-lab-1.0.1/src/Base/Century/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Durak/_render_func.py` & `vis-lab-1.0.1/src/Base/Durak/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Durak/env.py` & `vis-lab-1.0.1/src/Base/Durak/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Exploding_Kitten/_render_func.py` & `vis-lab-1.0.1/src/Base/Exploding_Kitten/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Exploding_Kitten/env.py` & `vis-lab-1.0.1/src/Base/Exploding_Kitten/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/GoFish/_render_func.py` & `vis-lab-1.0.1/src/Base/GoFish/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/GoFish/env.py` & `vis-lab-1.0.1/src/Base/GoFish/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Imploding_Kitten/_render_func.py` & `vis-lab-1.0.1/src/Base/Imploding_Kitten/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Imploding_Kitten/env.py` & `vis-lab-1.0.1/src/Base/Imploding_Kitten/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/MachiKoro/_render_func.py` & `vis-lab-1.0.1/src/Base/MachiKoro/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/MachiKoro/env.py` & `vis-lab-1.0.1/src/Base/MachiKoro/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Poker/_render_func.py` & `vis-lab-1.0.1/src/Base/Poker/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Poker/env.py` & `vis-lab-1.0.1/src/Base/Poker/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Sheriff/_render_func.py` & `vis-lab-1.0.1/src/Base/Sheriff/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Sheriff/env.py` & `vis-lab-1.0.1/src/Base/Sheriff/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor/_render_func.py` & `vis-lab-1.0.1/src/Base/Splendor/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor/env.py` & `vis-lab-1.0.1/src/Base/Splendor/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor_v2/_render_func.py` & `vis-lab-1.0.1/src/Base/Splendor_v2/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor_v2/env.py` & `vis-lab-1.0.1/src/Base/Splendor_v2/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor_v3/_render_func.py` & `vis-lab-1.0.1/src/Base/Splendor_v3/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/Splendor_v3/env.py` & `vis-lab-1.0.1/src/Base/Splendor_v3/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/SushiGo/_render_func.py` & `vis-lab-1.0.1/src/Base/SushiGo/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/SushiGo/env.py` & `vis-lab-1.0.1/src/Base/SushiGo/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/TLMN/_render_func.py` & `vis-lab-1.0.1/src/Base/TLMN/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/TLMN/env.py` & `vis-lab-1.0.1/src/Base/TLMN/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/TicketToRide/_render_func.py` & `vis-lab-1.0.1/src/Base/TicketToRide/_render_func.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Base/TicketToRide/env.py` & `vis-lab-1.0.1/src/Base/TicketToRide/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/Utils.py` & `vis-lab-1.0.1/src/Utils.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/env.py` & `vis-lab-1.0.1/src/env.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/src/render_template.py` & `vis-lab-1.0.1/src/render_template.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/tests/CheckEnv.py` & `vis-lab-1.0.1/tests/CheckEnv.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/tests/CheckGraphics.py` & `vis-lab-1.0.1/tests/CheckGraphics.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/tests/CheckPlayer.py` & `vis-lab-1.0.1/tests/CheckPlayer.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/tests/test_agent.py` & `vis-lab-1.0.1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `vis-lab-1.0.0/vis_lab.egg-info/PKG-INFO` & `vis-lab-1.0.1/vis_lab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vis-lab
-Version: 1.0.0
+Version: 1.0.1
 Summary: a system reinforcement learning
 Home-page: 
 Author: Ngo Xuan Phong
 Author-email: phong@vis-laboratory.com
 License: MIT
 Keywords: vis_game
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vis-lab-1.0.0/vis_lab.egg-info/SOURCES.txt` & `vis-lab-1.0.1/vis_lab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENCE.txt
 README.md
 setup.py
+docs/__init__.py
 src/Utils.py
 src/__init__.py
 src/env.py
 src/render_template.py
 src/Agent/__init__.py
 src/Agent/ActionsLayer/Agent_player.py
 src/Agent/ActionsLayer/__init__.py
```

