# Comparing `tmp/st_chat_message-0.3.5.tar.gz` & `tmp/st_chat_message-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_chat_message-0.3.5.tar", max compression
+gzip compressed data, was "st_chat_message-0.3.6.tar", max compression
```

## Comparing `st_chat_message-0.3.5.tar` & `st_chat_message-0.3.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      658 2023-06-27 09:53:09.908529 st_chat_message-0.3.5/README.md
--rw-r--r--   0        0        0      680 2023-06-27 12:05:04.280875 st_chat_message-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3854 2023-06-27 09:20:42.712230 st_chat_message-0.3.5/st_chat_message/__init__.py
--rw-r--r--   0        0        0     2648 2023-06-27 12:05:02.635642 st_chat_message-0.3.5/st_chat_message/frontend/out/404.html
--rw-r--r--   0        0        0      361 2023-06-27 12:05:02.513541 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/Dg5cdAEY-RCHv3LVfP7Lo/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-06-27 12:05:02.513809 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/Dg5cdAEY-RCHv3LVfP7Lo/_ssgManifest.js
--rw-r--r--   0        0        0   266404 2023-06-27 12:05:02.518587 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/175675d1-280cba64f0247428.js
--rw-r--r--   0        0        0   141045 2023-06-27 12:05:02.518454 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/framework-5e8ac8dd643904dd.js
--rw-r--r--   0        0        0    96246 2023-06-27 12:05:02.518453 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/main-c6459c6dbdcff8e8.js
--rw-r--r--   0        0        0      448 2023-06-27 12:05:02.518720 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/pages/_app-345c8177130438ac.js
--rw-r--r--   0        0        0      250 2023-06-27 12:05:02.518774 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
--rw-r--r--   0        0        0  1407017 2023-06-27 12:05:02.519868 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/pages/index-56e240b261b33c91.js
--rw-r--r--   0        0        0    91381 2023-06-27 12:05:02.518454 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0     1639 2023-06-27 12:05:02.518644 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/webpack-9d2bee59a0ebae7b.js
--rw-r--r--   0        0        0    26985 2023-06-27 12:05:02.513726 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/css/1f759626be541cb1.css
--rw-r--r--   0        0        0    20655 2023-06-27 12:05:02.513783 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/css/2c1d693913146cab.css
--rw-r--r--   0        0        0    33516 2023-06-27 12:05:02.514334 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.1608a09b.woff
--rw-r--r--   0        0        0    63632 2023-06-27 12:05:02.514441 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.4aafdb68.ttf
--rw-r--r--   0        0        0    28076 2023-06-27 12:05:02.514374 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.a79f1c31.woff2
--rw-r--r--   0        0        0     7716 2023-06-27 12:05:02.514314 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.b6770918.woff
--rw-r--r--   0        0        0    12368 2023-06-27 12:05:02.514515 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.cce5b8ec.ttf
--rw-r--r--   0        0        0     6912 2023-06-27 12:05:02.514513 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.ec17d132.woff2
--rw-r--r--   0        0        0    12344 2023-06-27 12:05:02.514614 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.07ef19e7.ttf
--rw-r--r--   0        0        0     6908 2023-06-27 12:05:02.514682 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.55fac258.woff2
--rw-r--r--   0        0        0     7656 2023-06-27 12:05:02.514726 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.dad44a7f.woff
--rw-r--r--   0        0        0    13296 2023-06-27 12:05:02.514746 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.9f256b85.woff
--rw-r--r--   0        0        0    19584 2023-06-27 12:05:02.514921 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.b18f59e1.ttf
--rw-r--r--   0        0        0    11348 2023-06-27 12:05:02.514874 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.d42a5579.woff2
--rw-r--r--   0        0        0    13208 2023-06-27 12:05:02.514951 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.7c187121.woff
--rw-r--r--   0        0        0    11316 2023-06-27 12:05:02.515013 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.d3c882a6.woff2
--rw-r--r--   0        0        0    19572 2023-06-27 12:05:02.515174 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.ed38e79f.ttf
--rw-r--r--   0        0        0    51336 2023-06-27 12:05:02.515383 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.b74a1a8b.ttf
--rw-r--r--   0        0        0    25324 2023-06-27 12:05:02.515270 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.c3fb5ac2.woff2
--rw-r--r--   0        0        0    29912 2023-06-27 12:05:02.515315 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.d181c465.woff
--rw-r--r--   0        0        0    16780 2023-06-27 12:05:02.515359 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.6f2bb1df.woff2
--rw-r--r--   0        0        0    32968 2023-06-27 12:05:02.515490 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.70d8b0a5.ttf
--rw-r--r--   0        0        0    19412 2023-06-27 12:05:02.515499 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.e3f82f9d.woff
--rw-r--r--   0        0        0    33580 2023-06-27 12:05:02.515653 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.47373d1e.ttf
--rw-r--r--   0        0        0    16988 2023-06-27 12:05:02.515607 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.8916142b.woff2
--rw-r--r--   0        0        0    19676 2023-06-27 12:05:02.515669 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.9024d815.woff
--rw-r--r--   0        0        0    26272 2023-06-27 12:05:02.515761 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.0462f03b.woff2
--rw-r--r--   0        0        0    30772 2023-06-27 12:05:02.515863 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.7f51fe03.woff
--rw-r--r--   0        0        0    53580 2023-06-27 12:05:02.516049 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.b7f8fe9b.ttf
--rw-r--r--   0        0        0    16400 2023-06-27 12:05:02.515992 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.572d331f.woff2
--rw-r--r--   0        0        0    31196 2023-06-27 12:05:02.516086 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.a879cf83.ttf
--rw-r--r--   0        0        0    18668 2023-06-27 12:05:02.516089 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.f1035d8d.woff
--rw-r--r--   0        0        0    18748 2023-06-27 12:05:02.516217 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.5295ba48.woff
--rw-r--r--   0        0        0    31308 2023-06-27 12:05:02.516275 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.939bc644.ttf
--rw-r--r--   0        0        0    16440 2023-06-27 12:05:02.516411 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.f28c23ac.woff2
--rw-r--r--   0        0        0    12216 2023-06-27 12:05:02.516336 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.8c5b5494.woff2
--rw-r--r--   0        0        0    24504 2023-06-27 12:05:02.516420 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.94e1e8dc.ttf
--rw-r--r--   0        0        0    14408 2023-06-27 12:05:02.516450 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.bf59d231.woff
--rw-r--r--   0        0        0    12028 2023-06-27 12:05:02.516564 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.3b1e59b3.woff2
--rw-r--r--   0        0        0    14112 2023-06-27 12:05:02.516678 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.7c9bc82b.woff
--rw-r--r--   0        0        0    22364 2023-06-27 12:05:02.516706 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.b4c20c84.ttf
--rw-r--r--   0        0        0    12316 2023-06-27 12:05:02.516682 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.74048478.woff
--rw-r--r--   0        0        0    10344 2023-06-27 12:05:02.516843 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.ba21ed5f.woff2
--rw-r--r--   0        0        0    19436 2023-06-27 12:05:02.517011 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.d4d7ba48.ttf
--rw-r--r--   0        0        0     9644 2023-06-27 12:05:02.516944 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.03e9641d.woff2
--rw-r--r--   0        0        0    10588 2023-06-27 12:05:02.517004 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.07505710.woff
--rw-r--r--   0        0        0    16648 2023-06-27 12:05:02.517130 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.fe9cbbe1.ttf
--rw-r--r--   0        0        0     6496 2023-06-27 12:05:02.517137 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.e1e279cb.woff
--rw-r--r--   0        0        0     5468 2023-06-27 12:05:02.517236 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.eae34984.woff2
--rw-r--r--   0        0        0    12228 2023-06-27 12:05:02.517260 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.fabc004a.ttf
--rw-r--r--   0        0        0     6188 2023-06-27 12:05:02.517325 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.57727022.woff
--rw-r--r--   0        0        0     5208 2023-06-27 12:05:02.517353 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.5916a24f.woff2
--rw-r--r--   0        0        0    11508 2023-06-27 12:05:02.517383 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.d6b476ec.ttf
--rw-r--r--   0        0        0     4420 2023-06-27 12:05:02.517433 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.9acaf01c.woff
--rw-r--r--   0        0        0     7588 2023-06-27 12:05:02.517464 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.a144ef58.ttf
--rw-r--r--   0        0        0     3624 2023-06-27 12:05:02.517564 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.b4230e7e.woff2
--rw-r--r--   0        0        0     4928 2023-06-27 12:05:02.517601 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.10d95fd3.woff2
--rw-r--r--   0        0        0     5980 2023-06-27 12:05:02.517664 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.7a996c9d.woff
--rw-r--r--   0        0        0    10364 2023-06-27 12:05:02.517678 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.fbccdabe.ttf
--rw-r--r--   0        0        0    16028 2023-06-27 12:05:02.517759 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.6258592b.woff
--rw-r--r--   0        0        0    13568 2023-06-27 12:05:02.517824 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.a8709e36.woff2
--rw-r--r--   0        0        0    27556 2023-06-27 12:05:02.517905 st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.d97aaf4a.ttf
--rw-r--r--   0        0        0    25931 2023-06-27 12:05:02.521914 st_chat_message-0.3.5/st_chat_message/frontend/out/favicon.ico
--rw-r--r--   0        0        0     2335 2023-06-27 12:05:02.608502 st_chat_message-0.3.5/st_chat_message/frontend/out/index.html
--rw-r--r--   0        0        0     1101 2023-06-27 12:05:02.521703 st_chat_message-0.3.5/st_chat_message/frontend/out/vercel.svg
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 st_chat_message-0.3.5/setup.py
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 st_chat_message-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      856 2023-06-27 12:09:00.859182 st_chat_message-0.3.6/README.md
+-rw-r--r--   0        0        0      680 2023-06-27 13:46:15.994804 st_chat_message-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3854 2023-06-27 09:20:42.712230 st_chat_message-0.3.6/st_chat_message/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-27 12:05:02.635642 st_chat_message-0.3.6/st_chat_message/frontend/out/404.html
+-rw-r--r--   0        0        0      361 2023-06-27 12:05:02.513541 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/Dg5cdAEY-RCHv3LVfP7Lo/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-06-27 12:05:02.513809 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/Dg5cdAEY-RCHv3LVfP7Lo/_ssgManifest.js
+-rw-r--r--   0        0        0   266404 2023-06-27 12:05:02.518587 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/175675d1-280cba64f0247428.js
+-rw-r--r--   0        0        0   141045 2023-06-27 12:05:02.518454 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/framework-5e8ac8dd643904dd.js
+-rw-r--r--   0        0        0    96246 2023-06-27 12:05:02.518453 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/main-c6459c6dbdcff8e8.js
+-rw-r--r--   0        0        0      448 2023-06-27 12:05:02.518720 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/pages/_app-345c8177130438ac.js
+-rw-r--r--   0        0        0      250 2023-06-27 12:05:02.518774 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
+-rw-r--r--   0        0        0  1407017 2023-06-27 12:05:02.519868 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/pages/index-56e240b261b33c91.js
+-rw-r--r--   0        0        0    91381 2023-06-27 12:05:02.518454 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0     1639 2023-06-27 12:05:02.518644 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/webpack-9d2bee59a0ebae7b.js
+-rw-r--r--   0        0        0    26985 2023-06-27 12:05:02.513726 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/css/1f759626be541cb1.css
+-rw-r--r--   0        0        0    20655 2023-06-27 12:05:02.513783 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/css/2c1d693913146cab.css
+-rw-r--r--   0        0        0    33516 2023-06-27 12:05:02.514334 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.1608a09b.woff
+-rw-r--r--   0        0        0    63632 2023-06-27 12:05:02.514441 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.4aafdb68.ttf
+-rw-r--r--   0        0        0    28076 2023-06-27 12:05:02.514374 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.a79f1c31.woff2
+-rw-r--r--   0        0        0     7716 2023-06-27 12:05:02.514314 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.b6770918.woff
+-rw-r--r--   0        0        0    12368 2023-06-27 12:05:02.514515 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.cce5b8ec.ttf
+-rw-r--r--   0        0        0     6912 2023-06-27 12:05:02.514513 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.ec17d132.woff2
+-rw-r--r--   0        0        0    12344 2023-06-27 12:05:02.514614 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.07ef19e7.ttf
+-rw-r--r--   0        0        0     6908 2023-06-27 12:05:02.514682 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.55fac258.woff2
+-rw-r--r--   0        0        0     7656 2023-06-27 12:05:02.514726 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.dad44a7f.woff
+-rw-r--r--   0        0        0    13296 2023-06-27 12:05:02.514746 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.9f256b85.woff
+-rw-r--r--   0        0        0    19584 2023-06-27 12:05:02.514921 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.b18f59e1.ttf
+-rw-r--r--   0        0        0    11348 2023-06-27 12:05:02.514874 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.d42a5579.woff2
+-rw-r--r--   0        0        0    13208 2023-06-27 12:05:02.514951 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.7c187121.woff
+-rw-r--r--   0        0        0    11316 2023-06-27 12:05:02.515013 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.d3c882a6.woff2
+-rw-r--r--   0        0        0    19572 2023-06-27 12:05:02.515174 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.ed38e79f.ttf
+-rw-r--r--   0        0        0    51336 2023-06-27 12:05:02.515383 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.b74a1a8b.ttf
+-rw-r--r--   0        0        0    25324 2023-06-27 12:05:02.515270 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.c3fb5ac2.woff2
+-rw-r--r--   0        0        0    29912 2023-06-27 12:05:02.515315 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.d181c465.woff
+-rw-r--r--   0        0        0    16780 2023-06-27 12:05:02.515359 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.6f2bb1df.woff2
+-rw-r--r--   0        0        0    32968 2023-06-27 12:05:02.515490 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.70d8b0a5.ttf
+-rw-r--r--   0        0        0    19412 2023-06-27 12:05:02.515499 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.e3f82f9d.woff
+-rw-r--r--   0        0        0    33580 2023-06-27 12:05:02.515653 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.47373d1e.ttf
+-rw-r--r--   0        0        0    16988 2023-06-27 12:05:02.515607 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.8916142b.woff2
+-rw-r--r--   0        0        0    19676 2023-06-27 12:05:02.515669 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.9024d815.woff
+-rw-r--r--   0        0        0    26272 2023-06-27 12:05:02.515761 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.0462f03b.woff2
+-rw-r--r--   0        0        0    30772 2023-06-27 12:05:02.515863 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.7f51fe03.woff
+-rw-r--r--   0        0        0    53580 2023-06-27 12:05:02.516049 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.b7f8fe9b.ttf
+-rw-r--r--   0        0        0    16400 2023-06-27 12:05:02.515992 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.572d331f.woff2
+-rw-r--r--   0        0        0    31196 2023-06-27 12:05:02.516086 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.a879cf83.ttf
+-rw-r--r--   0        0        0    18668 2023-06-27 12:05:02.516089 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.f1035d8d.woff
+-rw-r--r--   0        0        0    18748 2023-06-27 12:05:02.516217 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.5295ba48.woff
+-rw-r--r--   0        0        0    31308 2023-06-27 12:05:02.516275 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.939bc644.ttf
+-rw-r--r--   0        0        0    16440 2023-06-27 12:05:02.516411 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.f28c23ac.woff2
+-rw-r--r--   0        0        0    12216 2023-06-27 12:05:02.516336 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.8c5b5494.woff2
+-rw-r--r--   0        0        0    24504 2023-06-27 12:05:02.516420 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.94e1e8dc.ttf
+-rw-r--r--   0        0        0    14408 2023-06-27 12:05:02.516450 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.bf59d231.woff
+-rw-r--r--   0        0        0    12028 2023-06-27 12:05:02.516564 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.3b1e59b3.woff2
+-rw-r--r--   0        0        0    14112 2023-06-27 12:05:02.516678 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.7c9bc82b.woff
+-rw-r--r--   0        0        0    22364 2023-06-27 12:05:02.516706 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.b4c20c84.ttf
+-rw-r--r--   0        0        0    12316 2023-06-27 12:05:02.516682 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.74048478.woff
+-rw-r--r--   0        0        0    10344 2023-06-27 12:05:02.516843 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.ba21ed5f.woff2
+-rw-r--r--   0        0        0    19436 2023-06-27 12:05:02.517011 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.d4d7ba48.ttf
+-rw-r--r--   0        0        0     9644 2023-06-27 12:05:02.516944 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.03e9641d.woff2
+-rw-r--r--   0        0        0    10588 2023-06-27 12:05:02.517004 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.07505710.woff
+-rw-r--r--   0        0        0    16648 2023-06-27 12:05:02.517130 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.fe9cbbe1.ttf
+-rw-r--r--   0        0        0     6496 2023-06-27 12:05:02.517137 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.e1e279cb.woff
+-rw-r--r--   0        0        0     5468 2023-06-27 12:05:02.517236 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.eae34984.woff2
+-rw-r--r--   0        0        0    12228 2023-06-27 12:05:02.517260 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.fabc004a.ttf
+-rw-r--r--   0        0        0     6188 2023-06-27 12:05:02.517325 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.57727022.woff
+-rw-r--r--   0        0        0     5208 2023-06-27 12:05:02.517353 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.5916a24f.woff2
+-rw-r--r--   0        0        0    11508 2023-06-27 12:05:02.517383 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.d6b476ec.ttf
+-rw-r--r--   0        0        0     4420 2023-06-27 12:05:02.517433 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.9acaf01c.woff
+-rw-r--r--   0        0        0     7588 2023-06-27 12:05:02.517464 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.a144ef58.ttf
+-rw-r--r--   0        0        0     3624 2023-06-27 12:05:02.517564 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.b4230e7e.woff2
+-rw-r--r--   0        0        0     4928 2023-06-27 12:05:02.517601 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.10d95fd3.woff2
+-rw-r--r--   0        0        0     5980 2023-06-27 12:05:02.517664 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.7a996c9d.woff
+-rw-r--r--   0        0        0    10364 2023-06-27 12:05:02.517678 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.fbccdabe.ttf
+-rw-r--r--   0        0        0    16028 2023-06-27 12:05:02.517759 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.6258592b.woff
+-rw-r--r--   0        0        0    13568 2023-06-27 12:05:02.517824 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.a8709e36.woff2
+-rw-r--r--   0        0        0    27556 2023-06-27 12:05:02.517905 st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.d97aaf4a.ttf
+-rw-r--r--   0        0        0    25931 2023-06-27 12:05:02.521914 st_chat_message-0.3.6/st_chat_message/frontend/out/favicon.ico
+-rw-r--r--   0        0        0     2335 2023-06-27 12:05:02.608502 st_chat_message-0.3.6/st_chat_message/frontend/out/index.html
+-rw-r--r--   0        0        0     1101 2023-06-27 12:05:02.521703 st_chat_message-0.3.6/st_chat_message/frontend/out/vercel.svg
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 st_chat_message-0.3.6/setup.py
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 st_chat_message-0.3.6/PKG-INFO
```

### Comparing `st_chat_message-0.3.5/README.md` & `st_chat_message-0.3.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -27,10 +27,32 @@
 
 message("Hello world!", is_user=True)
 message("Hi")
 ```
 
 ![img.png](docs/img.png)
 
+## Buiding from source
+
+### Prerequisites
+
+- nodejs >= 18.x
+- yarn >= 1.22.x
+- poetry >= 1.2.x
+- python >= 3.8.x
+
+### Building
+
+```bash
+./build.sh
+```
+
+### Publishing
+
+```bash
+poetry publish 
+```
+
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `st_chat_message-0.3.5/pyproject.toml` & `st_chat_message-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-chat-message"
-version = "0.3.5"
+version = "0.3.6"
 description = "A Streamlit component to display chat messages"
 authors = ["Manolo Santos <manolo.santos@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "st_chat_message"}]
 
 license = "MIT"
```

### Comparing `st_chat_message-0.3.5/st_chat_message/__init__.py` & `st_chat_message-0.3.6/st_chat_message/__init__.py`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/404.html` & `st_chat_message-0.3.6/st_chat_message/frontend/out/404.html`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/175675d1-280cba64f0247428.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/175675d1-280cba64f0247428.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/framework-5e8ac8dd643904dd.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/framework-5e8ac8dd643904dd.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/main-c6459c6dbdcff8e8.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/main-c6459c6dbdcff8e8.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/pages/index-56e240b261b33c91.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/pages/index-56e240b261b33c91.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/chunks/webpack-9d2bee59a0ebae7b.js` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/chunks/webpack-9d2bee59a0ebae7b.js`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/css/1f759626be541cb1.css` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/css/1f759626be541cb1.css`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/css/2c1d693913146cab.css` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/css/2c1d693913146cab.css`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.1608a09b.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.1608a09b.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.4aafdb68.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.4aafdb68.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.a79f1c31.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.a79f1c31.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.b6770918.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.b6770918.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.cce5b8ec.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.cce5b8ec.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.ec17d132.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.ec17d132.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.07ef19e7.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.07ef19e7.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.55fac258.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.55fac258.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.dad44a7f.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.dad44a7f.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.9f256b85.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.9f256b85.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.b18f59e1.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.b18f59e1.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.d42a5579.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.d42a5579.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.7c187121.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.7c187121.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.d3c882a6.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.d3c882a6.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.ed38e79f.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.ed38e79f.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.b74a1a8b.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.b74a1a8b.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.c3fb5ac2.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.c3fb5ac2.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.d181c465.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.d181c465.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.6f2bb1df.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.6f2bb1df.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.70d8b0a5.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.70d8b0a5.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.e3f82f9d.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.e3f82f9d.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.47373d1e.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.47373d1e.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.8916142b.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.8916142b.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.9024d815.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.9024d815.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.0462f03b.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.0462f03b.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.7f51fe03.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.7f51fe03.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.b7f8fe9b.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.b7f8fe9b.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.572d331f.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.572d331f.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.a879cf83.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.a879cf83.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.f1035d8d.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.f1035d8d.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.5295ba48.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.5295ba48.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.939bc644.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.939bc644.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.f28c23ac.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.f28c23ac.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.8c5b5494.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.8c5b5494.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.94e1e8dc.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.94e1e8dc.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.bf59d231.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.bf59d231.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.3b1e59b3.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.3b1e59b3.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.7c9bc82b.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.7c9bc82b.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.b4c20c84.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.b4c20c84.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.74048478.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.74048478.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.ba21ed5f.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.ba21ed5f.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.d4d7ba48.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.d4d7ba48.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.03e9641d.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.03e9641d.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.07505710.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.07505710.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.fe9cbbe1.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.fe9cbbe1.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.e1e279cb.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.e1e279cb.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.eae34984.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.eae34984.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.fabc004a.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.fabc004a.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.57727022.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.57727022.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.5916a24f.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.5916a24f.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.d6b476ec.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.d6b476ec.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.9acaf01c.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.9acaf01c.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.a144ef58.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.a144ef58.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.b4230e7e.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.b4230e7e.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.10d95fd3.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.10d95fd3.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.7a996c9d.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.7a996c9d.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.fbccdabe.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.fbccdabe.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.6258592b.woff` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.6258592b.woff`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.a8709e36.woff2` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.a8709e36.woff2`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.d97aaf4a.ttf` & `st_chat_message-0.3.6/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.d97aaf4a.ttf`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/favicon.ico` & `st_chat_message-0.3.6/st_chat_message/frontend/out/favicon.ico`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/index.html` & `st_chat_message-0.3.6/st_chat_message/frontend/out/index.html`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/st_chat_message/frontend/out/vercel.svg` & `st_chat_message-0.3.6/st_chat_message/frontend/out/vercel.svg`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.3.5/setup.py` & `st_chat_message-0.3.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,17 +14,17 @@
                      'frontend/out/_next/static/media/*']}
 
 install_requires = \
 ['streamlit>=0.63']
 
 setup_kwargs = {
     'name': 'st-chat-message',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'A Streamlit component to display chat messages',
-    'long_description': '# st-chat-message\n\n## Description\n\nThis is a simple chat message component for streamlit. It is based on the [streamlit-chat](https://github.com/AI-Yash/st-chat) component, trying to be as compatible as possible, but it adding a few features:\n\n- Markdown support\n- LaTeX support\n- Tables\n\n## Installation\n\n```bash\npip install st-chat-message\n```\n\nor\n\n```bash\npoetry add st-chat-message\n```\n## Usage\n\n```python\nimport streamlit as st\nfrom st_chat_message import message\n\nmessage("Hello world!", is_user=True)\nmessage("Hi")\n```\n\n![img.png](docs/img.png)\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
+    'long_description': '# st-chat-message\n\n## Description\n\nThis is a simple chat message component for streamlit. It is based on the [streamlit-chat](https://github.com/AI-Yash/st-chat) component, trying to be as compatible as possible, but it adding a few features:\n\n- Markdown support\n- LaTeX support\n- Tables\n\n## Installation\n\n```bash\npip install st-chat-message\n```\n\nor\n\n```bash\npoetry add st-chat-message\n```\n## Usage\n\n```python\nimport streamlit as st\nfrom st_chat_message import message\n\nmessage("Hello world!", is_user=True)\nmessage("Hi")\n```\n\n![img.png](docs/img.png)\n\n## Buiding from source\n\n### Prerequisites\n\n- nodejs >= 18.x\n- yarn >= 1.22.x\n- poetry >= 1.2.x\n- python >= 3.8.x\n\n### Building\n\n```bash\n./build.sh\n```\n\n### Publishing\n\n```bash\npoetry publish \n```\n\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
     'author': 'Manolo Santos',
     'author_email': 'manolo.santos@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `st_chat_message-0.3.5/PKG-INFO` & `st_chat_message-0.3.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-chat-message
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Streamlit component to display chat messages
 License: MIT
 Author: Manolo Santos
 Author-email: manolo.santos@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -44,11 +44,33 @@
 
 message("Hello world!", is_user=True)
 message("Hi")
 ```
 
 ![img.png](docs/img.png)
 
+## Buiding from source
+
+### Prerequisites
+
+- nodejs >= 18.x
+- yarn >= 1.22.x
+- poetry >= 1.2.x
+- python >= 3.8.x
+
+### Building
+
+```bash
+./build.sh
+```
+
+### Publishing
+
+```bash
+poetry publish 
+```
+
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

