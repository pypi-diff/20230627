# Comparing `tmp/runit-server-0.2.3.tar.gz` & `tmp/runit-server-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit-server-0.2.3.tar", last modified: Mon Dec 12 00:36:38 2022, max compression
+gzip compressed data, was "runit-server-0.2.4.tar", last modified: Tue Jun 27 15:37:59 2023, max compression
```

## Comparing `runit-server-0.2.3.tar` & `runit-server-0.2.4.tar`

### file list

```diff
@@ -1,205 +1,594 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:38.771111 runit-server-0.2.3/
--rw-rw-rw-   0        0        0     1089 2022-11-03 12:16:42.000000 runit-server-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      196 2022-12-02 15:48:27.000000 runit-server-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3181 2022-12-12 00:36:38.768106 runit-server-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2224 2022-12-02 16:08:50.000000 runit-server-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:52.975644 runit-server-0.2.3/runit_server/
--rw-rw-rw-   0        0        0      708 2022-11-02 20:41:25.000000 runit-server-0.2.3/runit_server/Request.py
--rw-rw-rw-   0        0        0       21 2022-11-03 13:39:04.000000 runit-server-0.2.3/runit_server/__init__.py
--rw-rw-rw-   0        0        0     4556 2022-12-11 17:30:09.000000 runit-server-0.2.3/runit_server/app.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:55.780110 runit-server-0.2.3/runit_server/blueprints/
--rw-rw-rw-   0        0        0      206 2022-12-07 14:04:02.000000 runit-server-0.2.3/runit_server/blueprints/__init__.py
--rw-rw-rw-   0        0        0     4016 2022-12-07 13:50:20.000000 runit-server-0.2.3/runit_server/blueprints/account.py
--rw-rw-rw-   0        0        0     5392 2022-12-07 13:44:41.000000 runit-server-0.2.3/runit_server/blueprints/admin.py
--rw-rw-rw-   0        0        0     3512 2022-12-10 23:07:44.000000 runit-server-0.2.3/runit_server/blueprints/database.py
--rw-rw-rw-   0        0        0      768 2022-12-02 18:51:34.000000 runit-server-0.2.3/runit_server/blueprints/functions.py
--rw-rw-rw-   0        0        0     5353 2022-12-10 22:22:04.000000 runit-server-0.2.3/runit_server/blueprints/project.py
--rw-rw-rw-   0        0        0     3077 2022-12-10 22:43:07.000000 runit-server-0.2.3/runit_server/blueprints/public.py
--rw-rw-rw-   0        0        0     1225 2022-12-02 18:49:29.000000 runit-server-0.2.3/runit_server/blueprints/setup.py
--rw-rw-rw-   0        0        0     7369 2022-12-11 20:07:02.000000 runit-server-0.2.3/runit_server/cli.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:55.970057 runit-server-0.2.3/runit_server/common/
--rw-rw-rw-   0        0        0      365 2022-12-11 17:29:44.000000 runit-server-0.2.3/runit_server/common/__init__.py
--rw-rw-rw-   0        0        0     9921 2022-12-11 23:59:17.000000 runit-server-0.2.3/runit_server/common/apis.py
--rw-rw-rw-   0        0        0      640 2022-11-25 13:00:28.000000 runit-server-0.2.3/runit_server/common/security.py
--rw-rw-rw-   0        0        0     1063 2022-11-02 20:41:26.000000 runit-server-0.2.3/runit_server/common/utils.py
--rw-rw-rw-   0        0        0     3494 2022-11-02 20:41:25.000000 runit-server-0.2.3/runit_server/favicon.ico
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:58.983678 runit-server-0.2.3/runit_server/models/
--rw-rw-rw-   0        0        0      168 2022-12-07 14:07:06.000000 runit-server-0.2.3/runit_server/models/__init__.py
--rw-rw-rw-   0        0        0     2995 2022-12-07 13:36:11.000000 runit-server-0.2.3/runit_server/models/admin.py
--rw-rw-rw-   0        0        0     1807 2022-12-11 10:21:22.000000 runit-server-0.2.3/runit_server/models/database.py
--rw-rw-rw-   0        0        0     3347 2022-11-03 14:46:59.000000 runit-server-0.2.3/runit_server/models/function.py
--rw-rw-rw-   0        0        0     1306 2022-11-25 13:00:28.000000 runit-server-0.2.3/runit_server/models/permission.py
--rw-rw-rw-   0        0        0     3381 2022-11-03 14:42:18.000000 runit-server-0.2.3/runit_server/models/project.py
--rw-rw-rw-   0        0        0     2243 2022-12-07 13:35:47.000000 runit-server-0.2.3/runit_server/models/role.py
--rw-rw-rw-   0        0        0     2648 2022-11-25 13:00:28.000000 runit-server-0.2.3/runit_server/models/user.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:59.133035 runit-server-0.2.3/runit_server/modules/
--rw-rw-rw-   0        0        0       30 2022-11-25 13:00:28.000000 runit-server-0.2.3/runit_server/modules/__init__.py
--rw-rw-rw-   0        0        0     7940 2022-12-02 18:55:57.000000 runit-server-0.2.3/runit_server/modules/account.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:52.352446 runit-server-0.2.3/runit_server/static/
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:04.178584 runit-server-0.2.3/runit_server/static/css/
--rw-rw-rw-   0        0        0    58578 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/all.min.css
--rw-rw-rw-   0        0        0    73641 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/animate.css
--rw-rw-rw-   0        0        0    25983 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/aos.css
--rw-rw-rw-   0        0        0    17945 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/bootstrap-datepicker.css
--rw-rw-rw-   0        0        0   193529 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521648 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0     1279 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/flaticon.css
--rw-rw-rw-   0        0        0    79875 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/icomoon.css
--rw-rw-rw-   0        0        0    46816 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/ionicons.min.css
--rw-rw-rw-   0        0        0    32076 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/jquery-ui.min.css
--rw-rw-rw-   0        0        0     1588 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/jquery.timepicker.css
--rw-rw-rw-   0        0        0     6950 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/magnific-popup.css
--rw-rw-rw-   0        0        0     9467 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/open-iconic-bootstrap.min.css
--rw-rw-rw-   0        0        0     3351 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/owl.carousel.min.css
--rw-rw-rw-   0        0        0      965 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/owl.theme.default.min.css
--rw-rw-rw-   0        0        0     2505 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/slicknav.min.css
--rw-rw-rw-   0        0        0   289481 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/css/style.css
--rw-rw-rw-   0        0        0     2231 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/css/styles.css
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:04.467706 runit-server-0.2.3/runit_server/static/fonts/
--rw-rw-rw-   0        0        0     6148 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/.DS_Store
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:04.617102 runit-server-0.2.3/runit_server/static/fonts/flaticon/
--rw-rw-rw-   0        0        0     6148 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/.DS_Store
--rw-rw-rw-   0        0        0      712 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/backup.txt
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:07.032707 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/
--rw-rw-rw-   0        0        0     3570 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/Flaticon.eot
--rw-rw-rw-   0        0        0    14620 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/Flaticon.svg
--rw-rw-rw-   0        0        0     3392 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/Flaticon.ttf
--rw-rw-rw-   0        0        0     2492 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/Flaticon.woff
--rw-rw-rw-   0        0        0     1924 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/Flaticon.woff2
--rw-rw-rw-   0        0        0     1370 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/_flaticon.scss
--rw-rw-rw-   0        0        0     1033 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/flaticon.css
--rw-rw-rw-   0        0        0    17993 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/font/flaticon.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:07.370709 runit-server-0.2.3/runit_server/static/fonts/flaticon/license/
--rw-rw-rw-   0        0        0    36473 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/flaticon/license/license.pdf
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:08.984707 runit-server-0.2.3/runit_server/static/fonts/icomoon/
--rw-rw-rw-   0        0        0   307332 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/icomoon/icomoon.eot
--rw-rw-rw-   0        0        0   935341 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/icomoon/icomoon.svg
--rw-rw-rw-   0        0        0   307168 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/icomoon/icomoon.ttf
--rw-rw-rw-   0        0        0   307244 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/icomoon/icomoon.woff
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:52.336118 runit-server-0.2.3/runit_server/static/fonts/ionicons/
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:10.648715 runit-server-0.2.3/runit_server/static/fonts/ionicons/css/
--rw-rw-rw-   0        0        0    57268 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/css/_ionicons.scss
--rw-rw-rw-   0        0        0    51284 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/css/ionicons.min.css
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:20.133074 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/
--rw-rw-rw-   0        0        0     6148 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/.DS_Store
--rw-rw-rw-   0        0        0   112826 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/ionicons.eot
--rw-rw-rw-   0        0        0   313199 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/ionicons.svg
--rw-rw-rw-   0        0        0   112648 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/ionicons.ttf
--rw-rw-rw-   0        0        0    66024 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/ionicons.woff
--rw-rw-rw-   0        0        0    50592 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/ionicons/fonts/ionicons.woff2
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:23.112522 runit-server-0.2.3/runit_server/static/fonts/open-iconic/
--rw-rw-rw-   0        0        0    28196 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/open-iconic/open-iconic.eot
--rw-rw-rw-   0        0        0    20996 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/open-iconic/open-iconic.otf
--rw-rw-rw-   0        0        0    54789 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/open-iconic/open-iconic.svg
--rw-rw-rw-   0        0        0    28028 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/open-iconic/open-iconic.ttf
--rw-rw-rw-   0        0        0    14984 2022-11-02 20:41:29.000000 runit-server-0.2.3/runit_server/static/fonts/open-iconic/open-iconic.woff
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:23.133334 runit-server-0.2.3/runit_server/static/images/
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:27.833869 runit-server-0.2.3/runit_server/static/images/logos/
--rw-rw-rw-   0        0        0     1044 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/html5.svg
--rw-rw-rw-   0        0        0    46753 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/nodejs.png
--rw-rw-rw-   0        0        0     2603 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/nodejs.svg
--rw-rw-rw-   0        0        0     1997 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/php.svg
--rw-rw-rw-   0        0        0   150090 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/python.png
--rw-rw-rw-   0        0        0      559 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/python.svg
--rw-rw-rw-   0        0        0     5501 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/python1.svg
--rw-rw-rw-   0        0        0   587840 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
--rw-rw-rw-   0        0        0      600 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/images/terminal.svg
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:32.360741 runit-server-0.2.3/runit_server/static/js/
--rw-rw-rw-   0        0        0    14244 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/aos.js
--rw-rw-rw-   0        0        0    46820 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/bootstrap-datepicker.js
--rw-rw-rw-   0        0        0    79742 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   328436 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0    60055 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   214177 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/js/bootstrap.min.js.map
--rw-rw-rw-   0        0        0    89501 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery-3.6.0.min.js
--rw-rw-rw-   0        0        0   137972 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery-3.6.0.min.map
--rw-rw-rw-   0        0        0    11421 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery-migrate-3.0.1.min.js
--rw-rw-rw-   0        0        0   253669 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery-ui.min.js
--rw-rw-rw-   0        0        0     1391 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.animateNumber.min.js
--rw-rw-rw-   0        0        0     8111 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.easing.1.3.js
--rw-rw-rw-   0        0        0    20216 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.magnific-popup.min.js
--rw-rw-rw-   0        0        0    60010 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.nicescroll.min.js
--rw-rw-rw-   0        0        0     8415 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.slicknav.min.js
--rw-rw-rw-   0        0        0    12597 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.stellar.min.js
--rw-rw-rw-   0        0        0     8835 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.waypoints.min.js
--rw-rw-rw-   0        0        0     2616 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/jquery.zoom.min.js
--rw-rw-rw-   0        0        0     6777 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/main.js
--rw-rw-rw-   0        0        0    43237 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/owl.carousel.min.js
--rw-rw-rw-   0        0        0    19032 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/popper.min.js
--rw-rw-rw-   0        0        0     2526 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/projects.js
--rw-rw-rw-   0        0        0      998 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/range.js
--rw-rw-rw-   0        0        0    24125 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/scripts.js
--rw-rw-rw-   0        0        0     7447 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/scrollax.min.js
--rw-rw-rw-   0        0        0     3866 2022-11-02 20:41:28.000000 runit-server-0.2.3/runit_server/static/js/setup.js
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:33.956764 runit-server-0.2.3/runit_server/static/webfonts/
--rw-rw-rw-   0        0        0   133034 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   715890 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   132728 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    89824 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76612 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34390 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   144322 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    34092 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16800 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13584 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   202902 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   897426 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   202616 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   103300 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    79444 2022-11-02 20:41:27.000000 runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:34.148761 runit-server-0.2.3/runit_server/templates/
--rw-rw-rw-   0        0        0     1117 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/404.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:34.292770 runit-server-0.2.3/runit_server/templates/account/
--rw-rw-rw-   0        0        0      925 2022-12-07 14:04:53.000000 runit-server-0.2.3/runit_server/templates/account/home.html
--rw-rw-rw-   0        0        0     4909 2022-12-07 16:18:26.000000 runit-server-0.2.3/runit_server/templates/account/layout.html
--rw-rw-rw-   0        0        0     9930 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/account/profile.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:34.626772 runit-server-0.2.3/runit_server/templates/admin/
--rw-rw-rw-   0        0        0      927 2022-12-07 13:47:21.000000 runit-server-0.2.3/runit_server/templates/admin/index.html
--rw-rw-rw-   0        0        0     4886 2022-12-05 09:03:01.000000 runit-server-0.2.3/runit_server/templates/admin/layout.html
--rw-rw-rw-   0        0        0     2194 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/admin/login.html
--rw-rw-rw-   0        0        0      541 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/admin/profile.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:35.710768 runit-server-0.2.3/runit_server/templates/admin/projects/
--rw-rw-rw-   0        0        0    10150 2022-12-05 08:54:43.000000 runit-server-0.2.3/runit_server/templates/admin/projects/details.html
--rw-rw-rw-   0        0        0     1341 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/projects/grid.html
--rw-rw-rw-   0        0        0     2245 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/projects/index.html
--rw-rw-rw-   0        0        0     2435 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/projects/list.html
--rw-rw-rw-   0        0        0     2134 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/projects/modal.html
--rw-rw-rw-   0        0        0     1028 2022-12-07 13:46:23.000000 runit-server-0.2.3/runit_server/templates/admin/sidebar.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:35.995763 runit-server-0.2.3/runit_server/templates/admin/users/
--rw-rw-rw-   0        0        0     9640 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/users/details.html
--rw-rw-rw-   0        0        0      774 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/admin/users/grid.html
--rw-rw-rw-   0        0        0     2217 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/users/index.html
--rw-rw-rw-   0        0        0     2336 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/users/list.html
--rw-rw-rw-   0        0        0     2027 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/admin/users/modal.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:36.563764 runit-server-0.2.3/runit_server/templates/databases/
--rw-rw-rw-   0        0        0     6910 2022-12-10 23:02:44.000000 runit-server-0.2.3/runit_server/templates/databases/details.html
--rw-rw-rw-   0        0        0     1213 2022-12-10 22:15:39.000000 runit-server-0.2.3/runit_server/templates/databases/grid.html
--rw-rw-rw-   0        0        0     2322 2022-12-07 16:11:44.000000 runit-server-0.2.3/runit_server/templates/databases/index.html
--rw-rw-rw-   0        0        0     1976 2022-12-11 09:23:27.000000 runit-server-0.2.3/runit_server/templates/databases/list.html
--rw-rw-rw-   0        0        0     2135 2022-12-10 21:52:13.000000 runit-server-0.2.3/runit_server/templates/databases/modal.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:36.670761 runit-server-0.2.3/runit_server/templates/functions/
--rw-rw-rw-   0        0        0     5839 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/functions/index.html
--rw-rw-rw-   0        0        0     1600 2022-12-07 16:18:03.000000 runit-server-0.2.3/runit_server/templates/layout.html
--rw-rw-rw-   0        0        0     3226 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/login.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:36.772771 runit-server-0.2.3/runit_server/templates/modals/
--rw-rw-rw-   0        0        0     1042 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/modals/confirm.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:38.596996 runit-server-0.2.3/runit_server/templates/projects/
--rw-rw-rw-   0        0        0    10257 2022-12-06 11:51:34.000000 runit-server-0.2.3/runit_server/templates/projects/details.html
--rw-rw-rw-   0        0        0     1498 2022-12-10 21:06:11.000000 runit-server-0.2.3/runit_server/templates/projects/grid.html
--rw-rw-rw-   0        0        0     2235 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/projects/index.html
--rw-rw-rw-   0        0        0     2431 2022-11-02 20:41:31.000000 runit-server-0.2.3/runit_server/templates/projects/list.html
--rw-rw-rw-   0        0        0     2791 2022-12-10 21:32:49.000000 runit-server-0.2.3/runit_server/templates/projects/modal.html
--rw-rw-rw-   0        0        0     2974 2022-11-02 20:41:30.000000 runit-server-0.2.3/runit_server/templates/register.html
-drwxrwxrwx   0        0        0        0 2022-12-12 00:36:38.758118 runit-server-0.2.3/runit_server/templates/setup/
--rw-rw-rw-   0        0        0     7463 2022-12-05 07:21:09.000000 runit-server-0.2.3/runit_server/templates/setup/index.html
--rw-rw-rw-   0        0        0      968 2022-12-07 14:04:41.000000 runit-server-0.2.3/runit_server/templates/sidebar.html
--rw-rw-rw-   0        0        0       90 2022-11-16 14:50:26.000000 runit-server-0.2.3/runit_server/test.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:35:53.372639 runit-server-0.2.3/runit_server.egg-info/
--rw-rw-rw-   0        0        0     3181 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7128 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-12 00:35:51.000000 runit-server-0.2.3/runit_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 00:36:38.772108 runit-server-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1602 2022-12-11 20:06:51.000000 runit-server-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:59.194358 runit-server-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2023-06-27 15:28:52.000000 runit-server-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      196 2022-12-02 15:48:27.000000 runit-server-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3222 2023-06-27 15:37:59.177856 runit-server-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2224 2023-06-27 15:28:52.000000 runit-server-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.791078 runit-server-0.2.4/runit_server/
+-rw-rw-rw-   0        0        0      708 2022-11-02 20:41:25.000000 runit-server-0.2.4/runit_server/Request.py
+-rw-rw-rw-   0        0        0       21 2022-11-03 13:39:04.000000 runit-server-0.2.4/runit_server/__init__.py
+-rw-rw-rw-   0        0        0     4658 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/app.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.905074 runit-server-0.2.4/runit_server/blueprints/
+-rw-rw-rw-   0        0        0      206 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/account.py
+-rw-rw-rw-   0        0        0     5367 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/admin.py
+-rw-rw-rw-   0        0        0     4488 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/database.py
+-rw-rw-rw-   0        0        0      768 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/functions.py
+-rw-rw-rw-   0        0        0     7753 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/project.py
+-rw-rw-rw-   0        0        0     3302 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/public.py
+-rw-rw-rw-   0        0        0     1225 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/blueprints/setup.py
+-rw-rw-rw-   0        0        0     7921 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.947073 runit-server-0.2.4/runit_server/common/
+-rw-rw-rw-   0        0        0      365 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/common/__init__.py
+-rw-rw-rw-   0        0        0     9759 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/common/apis.py
+-rw-rw-rw-   0        0        0      640 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/common/security.py
+-rw-rw-rw-   0        0        0     1063 2022-11-02 20:41:26.000000 runit-server-0.2.4/runit_server/common/utils.py
+-rw-rw-rw-   0        0        0      618 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/docker.py
+-rw-rw-rw-   0        0        0     3494 2022-11-02 20:41:25.000000 runit-server-0.2.4/runit_server/favicon.ico
+-rw-rw-rw-   0        0        0     1301 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/kubernetes-1.py
+-rw-rw-rw-   0        0        0     1665 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/kubernetes-2.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.997073 runit-server-0.2.4/runit_server/models/
+-rw-rw-rw-   0        0        0      204 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/__init__.py
+-rw-rw-rw-   0        0        0     2995 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/admin.py
+-rw-rw-rw-   0        0        0     2507 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/collection.py
+-rw-rw-rw-   0        0        0     2372 2023-01-29 17:49:59.000000 runit-server-0.2.4/runit_server/models/database.py
+-rw-rw-rw-   0        0        0     3347 2022-11-03 14:46:59.000000 runit-server-0.2.4/runit_server/models/function.py
+-rw-rw-rw-   0        0        0     1306 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/permission.py
+-rw-rw-rw-   0        0        0     3501 2023-02-20 13:20:35.000000 runit-server-0.2.4/runit_server/models/project.py
+-rw-rw-rw-   0        0        0     2243 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/role.py
+-rw-rw-rw-   0        0        0     2648 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/models/user.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:31.029072 runit-server-0.2.4/runit_server/modules/
+-rw-rw-rw-   0        0        0       30 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/modules/__init__.py
+-rw-rw-rw-   0        0        0     7940 2022-12-02 18:55:57.000000 runit-server-0.2.4/runit_server/modules/account.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.569074 runit-server-0.2.4/runit_server/static/
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:31.303068 runit-server-0.2.4/runit_server/static/css/
+-rw-rw-rw-   0        0        0    58578 2022-11-02 20:41:29.000000 runit-server-0.2.4/runit_server/static/css/all.min.css
+-rw-rw-rw-   0        0        0   193529 2022-11-02 20:41:29.000000 runit-server-0.2.4/runit_server/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521648 2022-11-02 20:41:29.000000 runit-server-0.2.4/runit_server/static/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0     2231 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/css/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:31.320069 runit-server-0.2.4/runit_server/static/images/
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:31.593549 runit-server-0.2.4/runit_server/static/images/logos/
+-rw-rw-rw-   0        0        0     1044 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/html5.svg
+-rw-rw-rw-   0        0        0    46753 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/nodejs.png
+-rw-rw-rw-   0        0        0     2603 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/nodejs.svg
+-rw-rw-rw-   0        0        0     1997 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/php.svg
+-rw-rw-rw-   0        0        0   150090 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/python.png
+-rw-rw-rw-   0        0        0      559 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/python.svg
+-rw-rw-rw-   0        0        0     5501 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/python1.svg
+-rw-rw-rw-   0        0        0   587840 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
+-rw-rw-rw-   0        0        0      600 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/images/terminal.svg
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:32.486323 runit-server-0.2.4/runit_server/static/js/
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:53.024520 runit-server-0.2.4/runit_server/static/js/ace/
+-rw-rw-rw-   0        0        0   434222 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ace.js
+-rw-rw-rw-   0        0        0     4510 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-beautify.js
+-rw-rw-rw-   0        0        0     4174 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-code_lens.js
+-rw-rw-rw-   0        0        0    12731 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-command_bar.js
+-rw-rw-rw-   0        0        0     4101 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-elastic_tabstops_lite.js
+-rw-rw-rw-   0        0        0    25371 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-emmet.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:52.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-error_marker.js
+-rw-rw-rw-   0        0        0     1981 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-hardwrap.js
+-rw-rw-rw-   0        0        0    67178 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-inline_autocomplete.js
+-rw-rw-rw-   0        0        0     4442 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-keybinding_menu.js
+-rw-rw-rw-   0        0        0    46502 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-language_tools.js
+-rw-rw-rw-   0        0        0     1229 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-linking.js
+-rw-rw-rw-   0        0        0     5032 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-modelist.js
+-rw-rw-rw-   0        0        0    16079 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-options.js
+-rw-rw-rw-   0        0        0    57142 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-prompt.js
+-rw-rw-rw-   0        0        0     2594 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-rtl.js
+-rw-rw-rw-   0        0        0    13202 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-searchbox.js
+-rw-rw-rw-   0        0        0    16636 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-settings_menu.js
+-rw-rw-rw-   0        0        0     1596 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-spellcheck.js
+-rw-rw-rw-   0        0        0     3878 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-split.js
+-rw-rw-rw-   0        0        0     4352 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-static_highlight.js
+-rw-rw-rw-   0        0        0     1284 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-statusbar.js
+-rw-rw-rw-   0        0        0     6687 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-textarea.js
+-rw-rw-rw-   0        0        0     1771 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-themelist.js
+-rw-rw-rw-   0        0        0     3253 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/ext-whitespace.js
+-rw-rw-rw-   0        0        0    25071 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/keybinding-emacs.js
+-rw-rw-rw-   0        0        0     7882 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/keybinding-sublime.js
+-rw-rw-rw-   0        0        0   112356 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/keybinding-vim.js
+-rw-rw-rw-   0        0        0     5742 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/keybinding-vscode.js
+-rw-rw-rw-   0        0        0     6142 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-abap.js
+-rw-rw-rw-   0        0        0     5114 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-abc.js
+-rw-rw-rw-   0        0        0    20942 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-actionscript.js
+-rw-rw-rw-   0        0        0     2635 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ada.js
+-rw-rw-rw-   0        0        0     5406 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-alda.js
+-rw-rw-rw-   0        0        0    14258 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-apache_conf.js
+-rw-rw-rw-   0        0        0     8665 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-apex.js
+-rw-rw-rw-   0        0        0     5748 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-applescript.js
+-rw-rw-rw-   0        0        0     4358 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-aql.js
+-rw-rw-rw-   0        0        0     8495 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-asciidoc.js
+-rw-rw-rw-   0        0        0     8977 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-asl.js
+-rw-rw-rw-   0        0        0     9240 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-assembly_x86.js
+-rw-rw-rw-   0        0        0    64001 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-autohotkey.js
+-rw-rw-rw-   0        0        0     5203 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-batchfile.js
+-rw-rw-rw-   0        0        0     5246 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-bibtex.js
+-rw-rw-rw-   0        0        0     4418 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-c9search.js
+-rw-rw-rw-   0        0        0    11425 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-c_cpp.js
+-rw-rw-rw-   0        0        0     3348 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-cirru.js
+-rw-rw-rw-   0        0        0     9033 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-clojure.js
+-rw-rw-rw-   0        0        0     2646 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-cobol.js
+-rw-rw-rw-   0        0        0     7798 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-coffee.js
+-rw-rw-rw-   0        0        0    64725 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-coldfusion.js
+-rw-rw-rw-   0        0        0    10290 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-crystal.js
+-rw-rw-rw-   0        0        0     9148 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-csharp.js
+-rw-rw-rw-   0        0        0    76649 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-csound_document.js
+-rw-rw-rw-   0        0        0    42061 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-csound_orchestra.js
+-rw-rw-rw-   0        0        0     7976 2023-06-27 15:28:53.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-csound_score.js
+-rw-rw-rw-   0        0        0     1580 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-csp.js
+-rw-rw-rw-   0        0        0    20959 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-css.js
+-rw-rw-rw-   0        0        0    63214 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-curly.js
+-rw-rw-rw-   0        0        0     9292 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-d.js
+-rw-rw-rw-   0        0        0    14916 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-dart.js
+-rw-rw-rw-   0        0        0     2756 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-diff.js
+-rw-rw-rw-   0        0        0    63554 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-django.js
+-rw-rw-rw-   0        0        0     8562 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-dockerfile.js
+-rw-rw-rw-   0        0        0     7914 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-dot.js
+-rw-rw-rw-   0        0        0    11595 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-drools.js
+-rw-rw-rw-   0        0        0     3206 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-edifact.js
+-rw-rw-rw-   0        0        0     3178 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-eiffel.js
+-rw-rw-rw-   0        0        0    82331 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ejs.js
+-rw-rw-rw-   0        0        0    16087 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-elixir.js
+-rw-rw-rw-   0        0        0     5274 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-elm.js
+-rw-rw-rw-   0        0        0    30096 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-erlang.js
+-rw-rw-rw-   0        0        0     7332 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-forth.js
+-rw-rw-rw-   0        0        0     8773 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-fortran.js
+-rw-rw-rw-   0        0        0     5781 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-fsharp.js
+-rw-rw-rw-   0        0        0     5053 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-fsl.js
+-rw-rw-rw-   0        0        0    36145 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ftl.js
+-rw-rw-rw-   0        0        0     1797 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-gcode.js
+-rw-rw-rw-   0        0        0     2700 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-gherkin.js
+-rw-rw-rw-   0        0        0     1236 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-gitignore.js
+-rw-rw-rw-   0        0        0    13505 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-glsl.js
+-rw-rw-rw-   0        0        0    31388 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-gobstones.js
+-rw-rw-rw-   0        0        0     7207 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-golang.js
+-rw-rw-rw-   0        0        0     3831 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-graphqlschema.js
+-rw-rw-rw-   0        0        0    26867 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-groovy.js
+-rw-rw-rw-   0        0        0    49498 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-haml.js
+-rw-rw-rw-   0        0        0    64079 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-handlebars.js
+-rw-rw-rw-   0        0        0    11867 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-haskell.js
+-rw-rw-rw-   0        0        0     2623 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-haskell_cabal.js
+-rw-rw-rw-   0        0        0     6825 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-haxe.js
+-rw-rw-rw-   0        0        0     6313 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-hjson.js
+-rw-rw-rw-   0        0        0    62194 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-html.js
+-rw-rw-rw-   0        0        0    79404 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-html_elixir.js
+-rw-rw-rw-   0        0        0    82666 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-html_ruby.js
+-rw-rw-rw-   0        0        0     3041 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ini.js
+-rw-rw-rw-   0        0        0     5682 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-io.js
+-rw-rw-rw-   0        0        0     8087 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ion.js
+-rw-rw-rw-   0        0        0     6053 2023-06-27 15:28:54.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jack.js
+-rw-rw-rw-   0        0        0    50911 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jade.js
+-rw-rw-rw-   0        0        0    27740 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-java.js
+-rw-rw-rw-   0        0        0    21767 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-javascript.js
+-rw-rw-rw-   0        0        0     5125 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jexl.js
+-rw-rw-rw-   0        0        0     5568 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-json.js
+-rw-rw-rw-   0        0        0     6217 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-json5.js
+-rw-rw-rw-   0        0        0   233695 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jsoniq.js
+-rw-rw-rw-   0        0        0    41343 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jsp.js
+-rw-rw-rw-   0        0        0     6236 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jssm.js
+-rw-rw-rw-   0        0        0     7249 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-jsx.js
+-rw-rw-rw-   0        0        0     7882 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-julia.js
+-rw-rw-rw-   0        0        0     8405 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-kotlin.js
+-rw-rw-rw-   0        0        0     5376 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-latex.js
+-rw-rw-rw-   0        0        0    65930 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-latte.js
+-rw-rw-rw-   0        0        0    22954 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-less.js
+-rw-rw-rw-   0        0        0    69540 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-liquid.js
+-rw-rw-rw-   0        0        0     2293 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-lisp.js
+-rw-rw-rw-   0        0        0     5411 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-livescript.js
+-rw-rw-rw-   0        0        0     5993 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-logiql.js
+-rw-rw-rw-   0        0        0    10936 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-logtalk.js
+-rw-rw-rw-   0        0        0    26912 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-lsl.js
+-rw-rw-rw-   0        0        0     7921 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-lua.js
+-rw-rw-rw-   0        0        0    70950 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-luapage.js
+-rw-rw-rw-   0        0        0     2775 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-lucene.js
+-rw-rw-rw-   0        0        0     6937 2023-06-27 15:28:55.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-makefile.js
+-rw-rw-rw-   0        0        0    73872 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-markdown.js
+-rw-rw-rw-   0        0        0    45783 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mask.js
+-rw-rw-rw-   0        0        0    20901 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-matlab.js
+-rw-rw-rw-   0        0        0     5262 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-maze.js
+-rw-rw-rw-   0        0        0     9703 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mediawiki.js
+-rw-rw-rw-   0        0        0    25227 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mel.js
+-rw-rw-rw-   0        0        0     5641 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mips.js
+-rw-rw-rw-   0        0        0     3176 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mixal.js
+-rw-rw-rw-   0        0        0     7048 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mushcode.js
+-rw-rw-rw-   0        0        0     8236 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-mysql.js
+-rw-rw-rw-   0        0        0    16230 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-nginx.js
+-rw-rw-rw-   0        0        0     6953 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-nim.js
+-rw-rw-rw-   0        0        0    13705 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-nix.js
+-rw-rw-rw-   0        0        0    10780 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-nsis.js
+-rw-rw-rw-   0        0        0    65640 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-nunjucks.js
+-rw-rw-rw-   0        0        0    55145 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-objectivec.js
+-rw-rw-rw-   0        0        0    15926 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ocaml.js
+-rw-rw-rw-   0        0        0     8350 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-odin.js
+-rw-rw-rw-   0        0        0    13101 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-partiql.js
+-rw-rw-rw-   0        0        0     4521 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-pascal.js
+-rw-rw-rw-   0        0        0     7763 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-perl.js
+-rw-rw-rw-   0        0        0    63512 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-pgsql.js
+-rw-rw-rw-   0        0        0   503168 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-php.js
+-rw-rw-rw-   0        0        0   507718 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-php_laravel_blade.js
+-rw-rw-rw-   0        0        0     6653 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-pig.js
+-rw-rw-rw-   0        0        0      844 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-plain_text.js
+-rw-rw-rw-   0        0        0     6218 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-plsql.js
+-rw-rw-rw-   0        0        0    32987 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-powershell.js
+-rw-rw-rw-   0        0        0    10738 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-praat.js
+-rw-rw-rw-   0        0        0     8589 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-prisma.js
+-rw-rw-rw-   0        0        0     8711 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-prolog.js
+-rw-rw-rw-   0        0        0     1437 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-properties.js
+-rw-rw-rw-   0        0        0    13127 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-protobuf.js
+-rw-rw-rw-   0        0        0     7393 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-puppet.js
+-rw-rw-rw-   0        0        0     8310 2023-06-27 15:28:56.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-python.js
+-rw-rw-rw-   0        0        0    16430 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-qml.js
+-rw-rw-rw-   0        0        0     5519 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-r.js
+-rw-rw-rw-   0        0        0    17901 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-raku.js
+-rw-rw-rw-   0        0        0    70009 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-razor.js
+-rw-rw-rw-   0        0        0     5024 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-rdoc.js
+-rw-rw-rw-   0        0        0    12944 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-red.js
+-rw-rw-rw-   0        0        0     8388 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-redshift.js
+-rw-rw-rw-   0        0        0    67260 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-rhtml.js
+-rw-rw-rw-   0        0        0     4424 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-robot.js
+-rw-rw-rw-   0        0        0     3393 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-rst.js
+-rw-rw-rw-   0        0        0    19973 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-ruby.js
+-rw-rw-rw-   0        0        0     8753 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-rust.js
+-rw-rw-rw-   0        0        0     7042 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sac.js
+-rw-rw-rw-   0        0        0    16017 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sass.js
+-rw-rw-rw-   0        0        0     6805 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-scad.js
+-rw-rw-rw-   0        0        0    27006 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-scala.js
+-rw-rw-rw-   0        0        0     3992 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-scheme.js
+-rw-rw-rw-   0        0        0     7505 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-scrypt.js
+-rw-rw-rw-   0        0        0    24141 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-scss.js
+-rw-rw-rw-   0        0        0     7517 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sh.js
+-rw-rw-rw-   0        0        0    24920 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sjs.js
+-rw-rw-rw-   0        0        0   113890 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-slim.js
+-rw-rw-rw-   0        0        0    65662 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-smarty.js
+-rw-rw-rw-   0        0        0     8979 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-smithy.js
+-rw-rw-rw-   0        0        0     4066 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-snippets.js
+-rw-rw-rw-   0        0        0    70697 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-soy_template.js
+-rw-rw-rw-   0        0        0     2569 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-space.js
+-rw-rw-rw-   0        0        0     8199 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sparql.js
+-rw-rw-rw-   0        0        0     4855 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sql.js
+-rw-rw-rw-   0        0        0    16948 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-sqlserver.js
+-rw-rw-rw-   0        0        0    14779 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-stylus.js
+-rw-rw-rw-   0        0        0    33732 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-svg.js
+-rw-rw-rw-   0        0        0     7314 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-swift.js
+-rw-rw-rw-   0        0        0     6536 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-tcl.js
+-rw-rw-rw-   0        0        0     7142 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-terraform.js
+-rw-rw-rw-   0        0        0     3130 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-tex.js
+-rw-rw-rw-   0        0        0      332 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-text.js
+-rw-rw-rw-   0        0        0     2464 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-textile.js
+-rw-rw-rw-   0        0        0     2536 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-toml.js
+-rw-rw-rw-   0        0        0    23801 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-tsx.js
+-rw-rw-rw-   0        0        0     5368 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-turtle.js
+-rw-rw-rw-   0        0        0    65829 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-twig.js
+-rw-rw-rw-   0        0        0    23496 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-typescript.js
+-rw-rw-rw-   0        0        0    16801 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-vala.js
+-rw-rw-rw-   0        0        0    12011 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-vbscript.js
+-rw-rw-rw-   0        0        0    66981 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-velocity.js
+-rw-rw-rw-   0        0        0     3235 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-verilog.js
+-rw-rw-rw-   0        0        0     2530 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-vhdl.js
+-rw-rw-rw-   0        0        0    64860 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-visualforce.js
+-rw-rw-rw-   0        0        0    24734 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-wollok.js
+-rw-rw-rw-   0        0        0    10222 2023-06-27 15:28:57.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-xml.js
+-rw-rw-rw-   0        0        0   231078 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-xquery.js
+-rw-rw-rw-   0        0        0     5418 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-yaml.js
+-rw-rw-rw-   0        0        0     9427 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/mode-zeek.js
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:57.202307 runit-server-0.2.4/runit_server/static/js/ace/snippets/
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/abap.js
+-rw-rw-rw-   0        0        0     1428 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/abc.js
+-rw-rw-rw-   0        0        0     3490 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/actionscript.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ada.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/alda.js
+-rw-rw-rw-   0        0        0      343 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/apache_conf.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/apex.js
+-rw-rw-rw-   0        0        0      343 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/applescript.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/aql.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/asciidoc.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/asl.js
+-rw-rw-rw-   0        0        0      344 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/assembly_x86.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/autohotkey.js
+-rw-rw-rw-   0        0        0      341 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/batchfile.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/bibtex.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/c9search.js
+-rw-rw-rw-   0        0        0     3152 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/c_cpp.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/cirru.js
+-rw-rw-rw-   0        0        0     2537 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/clojure.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/cobol.js
+-rw-rw-rw-   0        0        0     2726 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/coffee.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/coldfusion.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/crystal.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/csharp.js
+-rw-rw-rw-   0        0        0      831 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/csound_document.js
+-rw-rw-rw-   0        0        0     1606 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/csound_orchestra.js
+-rw-rw-rw-   0        0        0      344 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/csound_score.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/csp.js
+-rw-rw-rw-   0        0        0    20131 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/css.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/curly.js
+-rw-rw-rw-   0        0        0      333 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/d.js
+-rw-rw-rw-   0        0        0     1804 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/dart.js
+-rw-rw-rw-   0        0        0     1036 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/diff.js
+-rw-rw-rw-   0        0        0     4493 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/django.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/dockerfile.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/dot.js
+-rw-rw-rw-   0        0        0      863 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/drools.js
+-rw-rw-rw-   0        0        0     4814 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/edifact.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/eiffel.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ejs.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/elixir.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/elm.js
+-rw-rw-rw-   0        0        0     4067 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/erlang.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/forth.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/fortran.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/fsharp.js
+-rw-rw-rw-   0        0        0      826 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/fsl.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ftl.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/gcode.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/gherkin.js
+-rw-rw-rw-   0        0        0      341 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/gitignore.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/glsl.js
+-rw-rw-rw-   0        0        0    39613 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/gobstones.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/golang.js
+-rw-rw-rw-   0        0        0     1183 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/graphqlschema.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/groovy.js
+-rw-rw-rw-   0        0        0      933 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/haml.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/handlebars.js
+-rw-rw-rw-   0        0        0     2472 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/haskell.js
+-rw-rw-rw-   0        0        0      345 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/haskell_cabal.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/haxe.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/hjson.js
+-rw-rw-rw-   0        0        0    19641 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/html.js
+-rw-rw-rw-   0        0        0      343 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/html_elixir.js
+-rw-rw-rw-   0        0        0      341 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/html_ruby.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ini.js
+-rw-rw-rw-   0        0        0     1553 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/io.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ion.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jack.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jade.js
+-rw-rw-rw-   0        0        0     4807 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/java.js
+-rw-rw-rw-   0        0        0     4349 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/javascript.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jexl.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/json.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/json5.js
+-rw-rw-rw-   0        0        0     2209 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jsoniq.js
+-rw-rw-rw-   0        0        0     3259 2023-06-27 15:28:58.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jsp.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jssm.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/jsx.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/julia.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/kotlin.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/latex.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/latte.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/less.js
+-rw-rw-rw-   0        0        0    20015 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/liquid.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/lisp.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/livescript.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/logiql.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/logtalk.js
+-rw-rw-rw-   0        0        0    35904 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/lsl.js
+-rw-rw-rw-   0        0        0      989 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/lua.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/luapage.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/lucene.js
+-rw-rw-rw-   0        0        0      699 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/makefile.js
+-rw-rw-rw-   0        0        0     2474 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/markdown.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mask.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/matlab.js
+-rw-rw-rw-   0        0        0      755 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/maze.js
+-rw-rw-rw-   0        0        0      341 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mediawiki.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mel.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mips.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mixal.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mushcode.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/mysql.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/nginx.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/nim.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/nix.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/nsis.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/nunjucks.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/objectivec.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ocaml.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/odin.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/partiql.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/pascal.js
+-rw-rw-rw-   0        0        0     5998 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/perl.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/pgsql.js
+-rw-rw-rw-   0        0        0     7434 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/php.js
+-rw-rw-rw-   0        0        0      349 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/php_laravel_blade.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/pig.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/plain_text.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/plsql.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/powershell.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/praat.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/prisma.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/prolog.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/properties.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/protobuf.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/puppet.js
+-rw-rw-rw-   0        0        0     4165 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/python.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/qml.js
+-rw-rw-rw-   0        0        0     3103 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/r.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/raku.js
+-rw-rw-rw-   0        0        0      653 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/razor.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/rdoc.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/red.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/redshift.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/rhtml.js
+-rw-rw-rw-   0        0        0     2084 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/robot.js
+-rw-rw-rw-   0        0        0      923 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/rst.js
+-rw-rw-rw-   0        0        0    21764 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/ruby.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/rust.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sac.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sass.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/scad.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/scala.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/scheme.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/scrypt.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/scss.js
+-rw-rw-rw-   0        0        0     2530 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sh.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sjs.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/slim.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/smarty.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/smithy.js
+-rw-rw-rw-   0        0        0      798 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/snippets.js
+-rw-rw-rw-   0        0        0      344 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/soy_template.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/space.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sparql.js
+-rw-rw-rw-   0        0        0     1423 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sql.js
+-rw-rw-rw-   0        0        0     2644 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/sqlserver.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/stylus.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/svg.js
+-rw-rw-rw-   0        0        0      337 2023-06-27 15:28:59.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/swift.js
+-rw-rw-rw-   0        0        0     2171 2023-06-27 15:29:00.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/tcl.js
+-rw-rw-rw-   0        0        0      341 2023-06-27 15:29:01.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/terraform.js
+-rw-rw-rw-   0        0        0     4117 2023-06-27 15:29:02.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/tex.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/text.js
+-rw-rw-rw-   0        0        0     1037 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/textile.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/toml.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/tsx.js
+-rw-rw-rw-   0        0        0      338 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/turtle.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/twig.js
+-rw-rw-rw-   0        0        0      342 2023-06-27 15:29:03.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/typescript.js
+-rw-rw-rw-   0        0        0     3463 2023-06-27 15:29:04.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/vala.js
+-rw-rw-rw-   0        0        0      340 2023-06-27 15:29:04.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/vbscript.js
+-rw-rw-rw-   0        0        0     1152 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/velocity.js
+-rw-rw-rw-   0        0        0      339 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/verilog.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/vhdl.js
+-rw-rw-rw-   0        0        0      343 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/visualforce.js
+-rw-rw-rw-   0        0        0     1756 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/wollok.js
+-rw-rw-rw-   0        0        0      335 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/xml.js
+-rw-rw-rw-   0        0        0     2209 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/xquery.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/yaml.js
+-rw-rw-rw-   0        0        0      336 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/snippets/zeek.js
+-rw-rw-rw-   0        0        0    28724 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-ambiance.js
+-rw-rw-rw-   0        0        0     3866 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-chaos.js
+-rw-rw-rw-   0        0        0     3884 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-chrome.js
+-rw-rw-rw-   0        0        0     4188 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-cloud9_day.js
+-rw-rw-rw-   0        0        0     4297 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-cloud9_night.js
+-rw-rw-rw-   0        0        0     4318 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-cloud9_night_low_color.js
+-rw-rw-rw-   0        0        0     3138 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-clouds.js
+-rw-rw-rw-   0        0        0     3439 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-clouds_midnight.js
+-rw-rw-rw-   0        0        0     3371 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-cobalt.js
+-rw-rw-rw-   0        0        0     3997 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-crimson_editor.js
+-rw-rw-rw-   0        0        0     3335 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-dawn.js
+-rw-rw-rw-   0        0        0     4833 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-dracula.js
+-rw-rw-rw-   0        0        0     4396 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-dreamweaver.js
+-rw-rw-rw-   0        0        0     3197 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-eclipse.js
+-rw-rw-rw-   0        0        0     3528 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-github.js
+-rw-rw-rw-   0        0        0     3819 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-github_dark.js
+-rw-rw-rw-   0        0        0     3376 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-gob.js
+-rw-rw-rw-   0        0        0     2592 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-gruvbox.js
+-rw-rw-rw-   0        0        0     4072 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-gruvbox_dark_hard.js
+-rw-rw-rw-   0        0        0     4424 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-gruvbox_light_hard.js
+-rw-rw-rw-   0        0        0     3244 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-idle_fingers.js
+-rw-rw-rw-   0        0        0     7628 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-iplastic.js
+-rw-rw-rw-   0        0        0     4584 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-katzenmilch.js
+-rw-rw-rw-   0        0        0     3298 2023-06-27 15:29:05.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-kr_theme.js
+-rw-rw-rw-   0        0        0     3305 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-kuroir.js
+-rw-rw-rw-   0        0        0     3205 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-merbivore.js
+-rw-rw-rw-   0        0        0     3444 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-merbivore_soft.js
+-rw-rw-rw-   0        0        0     3832 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-mono_industrial.js
+-rw-rw-rw-   0        0        0     3366 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-monokai.js
+-rw-rw-rw-   0        0        0     2926 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-nord_dark.js
+-rw-rw-rw-   0        0        0     3864 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-one_dark.js
+-rw-rw-rw-   0        0        0     3679 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-pastel_on_dark.js
+-rw-rw-rw-   0        0        0     3282 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-solarized_dark.js
+-rw-rw-rw-   0        0        0     3446 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-solarized_light.js
+-rw-rw-rw-   0        0        0     4208 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-sqlserver.js
+-rw-rw-rw-   0        0        0     3935 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-terminal.js
+-rw-rw-rw-   0        0        0      623 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-textmate.js
+-rw-rw-rw-   0        0        0     3653 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-tomorrow.js
+-rw-rw-rw-   0        0        0     3848 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-tomorrow_night.js
+-rw-rw-rw-   0        0        0     4076 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-tomorrow_night_blue.js
+-rw-rw-rw-   0        0        0     4605 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-tomorrow_night_bright.js
+-rw-rw-rw-   0        0        0     4294 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-tomorrow_night_eighties.js
+-rw-rw-rw-   0        0        0     3481 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-twilight.js
+-rw-rw-rw-   0        0        0     3185 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-vibrant_ink.js
+-rw-rw-rw-   0        0        0     3043 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/theme-xcode.js
+-rw-rw-rw-   0        0        0    21854 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-base.js
+-rw-rw-rw-   0        0        0   323308 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-coffee.js
+-rw-rw-rw-   0        0        0   150957 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-css.js
+-rw-rw-rw-   0        0        0   208757 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-html.js
+-rw-rw-rw-   0        0        0   514171 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-javascript.js
+-rw-rw-rw-   0        0        0    24221 2023-06-27 15:29:06.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-json.js
+-rw-rw-rw-   0        0        0    48101 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-lua.js
+-rw-rw-rw-   0        0        0    78609 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-php.js
+-rw-rw-rw-   0        0        0    46751 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-xml.js
+-rw-rw-rw-   0        0        0  1624794 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-xquery.js
+-rw-rw-rw-   0        0        0    76583 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/ace/worker-yaml.js
+-rw-rw-rw-   0        0        0    79742 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   328436 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0     3261 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/databases.js
+-rw-rw-rw-   0        0        0     5028 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/static/js/editor.js
+-rw-rw-rw-   0        0        0     6777 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/main.js
+-rw-rw-rw-   0        0        0     2526 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/projects.js
+-rw-rw-rw-   0        0        0    24125 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/scripts.js
+-rw-rw-rw-   0        0        0     3866 2022-11-02 20:41:28.000000 runit-server-0.2.4/runit_server/static/js/setup.js
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.008516 runit-server-0.2.4/runit_server/static/webfonts/
+-rw-rw-rw-   0        0        0   133034 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   715890 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   132728 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    89824 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76612 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34390 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   144322 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    34092 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16800 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13584 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   202902 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   897426 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   202616 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   103300 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    79444 2022-11-02 20:41:27.000000 runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.215308 runit-server-0.2.4/runit_server/templates/
+-rw-rw-rw-   0        0        0     1117 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/404.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.287742 runit-server-0.2.4/runit_server/templates/account/
+-rw-rw-rw-   0        0        0      925 2022-12-07 14:04:53.000000 runit-server-0.2.4/runit_server/templates/account/home.html
+-rw-rw-rw-   0        0        0     5453 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/account/layout.html
+-rw-rw-rw-   0        0        0     9930 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/account/profile.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.425037 runit-server-0.2.4/runit_server/templates/admin/
+-rw-rw-rw-   0        0        0      927 2022-12-07 13:47:21.000000 runit-server-0.2.4/runit_server/templates/admin/index.html
+-rw-rw-rw-   0        0        0     5495 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/layout.html
+-rw-rw-rw-   0        0        0     2194 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/admin/login.html
+-rw-rw-rw-   0        0        0      541 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/admin/profile.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.564023 runit-server-0.2.4/runit_server/templates/admin/projects/
+-rw-rw-rw-   0        0        0    10453 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/projects/details.html
+-rw-rw-rw-   0        0        0     1418 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/projects/grid.html
+-rw-rw-rw-   0        0        0     2453 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/projects/index.html
+-rw-rw-rw-   0        0        0     1757 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/projects/list.html
+-rw-rw-rw-   0        0        0     2134 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/admin/projects/modal.html
+-rw-rw-rw-   0        0        0      590 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/sidebar.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.747535 runit-server-0.2.4/runit_server/templates/admin/users/
+-rw-rw-rw-   0        0        0     9640 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/admin/users/details.html
+-rw-rw-rw-   0        0        0      774 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/admin/users/grid.html
+-rw-rw-rw-   0        0        0     2217 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/admin/users/index.html
+-rw-rw-rw-   0        0        0     2389 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/admin/users/list.html
+-rw-rw-rw-   0        0        0     2027 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/admin/users/modal.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.838537 runit-server-0.2.4/runit_server/templates/databases/
+-rw-rw-rw-   0        0        0     9180 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/databases/details.html
+-rw-rw-rw-   0        0        0     1297 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/databases/grid.html
+-rw-rw-rw-   0        0        0     2492 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/databases/index.html
+-rw-rw-rw-   0        0        0     1800 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/databases/list.html
+-rw-rw-rw-   0        0        0     2078 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/databases/modal.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.872572 runit-server-0.2.4/runit_server/templates/functions/
+-rw-rw-rw-   0        0        0     5839 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/functions/index.html
+-rw-rw-rw-   0        0        0     1414 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/layout.html
+-rw-rw-rw-   0        0        0     3226 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/login.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:58.933464 runit-server-0.2.4/runit_server/templates/modals/
+-rw-rw-rw-   0        0        0     1042 2022-11-02 20:41:31.000000 runit-server-0.2.4/runit_server/templates/modals/confirm.html
+-rw-rw-rw-   0        0        0     1735 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/modals/create_database.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:59.146969 runit-server-0.2.4/runit_server/templates/projects/
+-rw-rw-rw-   0        0        0    11771 2023-06-27 15:29:07.000000 runit-server-0.2.4/runit_server/templates/projects/details.html
+-rw-rw-rw-   0        0        0     3161 2023-06-07 13:26:57.000000 runit-server-0.2.4/runit_server/templates/projects/editor.html
+-rw-rw-rw-   0        0        0     1581 2023-06-27 15:29:08.000000 runit-server-0.2.4/runit_server/templates/projects/grid.html
+-rw-rw-rw-   0        0        0     2445 2023-06-27 15:29:08.000000 runit-server-0.2.4/runit_server/templates/projects/index.html
+-rw-rw-rw-   0        0        0     2057 2023-06-27 15:29:08.000000 runit-server-0.2.4/runit_server/templates/projects/list.html
+-rw-rw-rw-   0        0        0     2791 2023-06-03 12:38:38.000000 runit-server-0.2.4/runit_server/templates/projects/modal.html
+-rw-rw-rw-   0        0        0     2974 2022-11-02 20:41:30.000000 runit-server-0.2.4/runit_server/templates/register.html
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:59.172845 runit-server-0.2.4/runit_server/templates/setup/
+-rw-rw-rw-   0        0        0     7463 2022-12-05 07:21:09.000000 runit-server-0.2.4/runit_server/templates/setup/index.html
+-rw-rw-rw-   0        0        0      592 2023-06-27 15:29:08.000000 runit-server-0.2.4/runit_server/templates/sidebar.html
+-rw-rw-rw-   0        0        0       90 2022-11-16 14:50:26.000000 runit-server-0.2.4/runit_server/test.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:37:30.845075 runit-server-0.2.4/runit_server.egg-info/
+-rw-rw-rw-   0        0        0     3222 2023-06-27 15:37:29.000000 runit-server-0.2.4/runit_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    24413 2023-06-27 15:37:30.000000 runit-server-0.2.4/runit_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:37:29.000000 runit-server-0.2.4/runit_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-27 15:37:29.000000 runit-server-0.2.4/runit_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2023-06-27 15:37:29.000000 runit-server-0.2.4/runit_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 15:37:29.000000 runit-server-0.2.4/runit_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:37:59.194358 runit-server-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-06-27 15:29:08.000000 runit-server-0.2.4/setup.py
```

### Comparing `runit-server-0.2.3/LICENSE` & `runit-server-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/PKG-INFO` & `runit-server-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.2.3
+Version: 0.2.4
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # runit-server-Server ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The runit-server Command Line Interface (CLI) Tools can be used to test, manage, and deploy your runit-server project from the command line.
 - Create new runit-server project
 - Run a local web server for your runit-server project
 - publish code and assets to your runit-server-server domain
```

### Comparing `runit-server-0.2.3/README.md` & `runit-server-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/Request.py` & `runit-server-0.2.4/runit_server/Request.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/app.py` & `runit-server-0.2.4/runit_server/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 from .common import  Login, Account, ProjectById, ProjectRS, ProjectCloneRS, Document
 
 from .models import Admin
 from .models import Role
 
 import os
 import logging
+from sys import platform
 from datetime import timedelta
 from dotenv import load_dotenv, dotenv_values, find_dotenv, set_key
 
+WORKDIR = os.path.join(os.getenv('USERPROFILE', os.getenv('HOME', '')), 'RUNIT_WORKDIR')
+
 app = Flask(__name__)
 api = Api(app, prefix='/api')
 
 load_dotenv()
 app.secret_key =  "dsafidsalkjdsaofwpdsncdsfdsafdsafjhdkjsfndsfkjsldfdsfjaskljdf"
 app.config['SERVER_NAME'] = os.getenv('RUNIT_SERVERNAME')
 app.config["JWT_SECRET_KEY"] = "972a444fb071aa8ee83bf128808d255ec72e3a6b464a836b7d06254529c6"
@@ -94,27 +97,27 @@
 @app.route('/get_app_requests/')
 def get_parameters():
     global REQUESTS
     if len(REQUESTS) > 0:
         return jsonify(REQUESTS.pop())
     return jsonify({'GET': {}, 'POST': {}})
 
-@app.before_first_request
-def init():
-    global app
+with app.app_context():
+    if not os.path.exists(WORKDIR):
+        os.mkdir(WORKDIR)
     
-    if not (os.path.exists(os.path.join(os.curdir, 'accounts'))):
-        os.mkdir(os.path.join(os.curdir, 'accounts'))
-    if not (os.path.exists(os.path.join(os.curdir, 'projects'))):
-        os.mkdir(os.path.join(os.curdir, 'projects'))
+    if not (os.path.exists(os.path.join(WORKDIR, 'accounts'))):
+        os.mkdir(os.path.join(WORKDIR, 'accounts'))
+        
+    if not (os.path.exists(os.path.join(WORKDIR, 'projects'))):
+        os.mkdir(os.path.join(WORKDIR, 'projects'))
 
     settings = dotenv_values(find_dotenv())
 
     if 'SETUP' in settings.keys() and settings['SETUP'] == 'completed':
-        print('--Setting up database connection')
         DBMS.initialize(settings['DBMS'], settings['DATABASE_HOST'], settings['DATABASE_PORT'],
                     settings['DATABASE_USERNAME'], settings['DATABASE_PASSWORD'], 
                     settings['DATABASE_NAME'])
     
 @app.before_request
 def startup():
     # if not os.path.exists('.env'):
```

### Comparing `runit-server-0.2.3/runit_server/blueprints/account.py` & `runit-server-0.2.4/runit_server/blueprints/account.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/blueprints/admin.py` & `runit-server-0.2.4/runit_server/blueprints/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from ..models import Function
 from ..common import Utils
 
 
 from runit import RunIt
 
 EXTENSIONS = {'python': '.py', 'python3': '.py', 'php': '.php', 'javascript': '.js'}
-LANGUAGE_ICONS = {'python': 'python', 'python3': 'python', 'php': 'php',
+LANGUAGE_ICONS = {'python': 'python', 'php': 'php',
                   'javascript': 'node-js', 'typescript': 'node-js'}
 
 CURRENT_PATH = os.path.dirname(os.path.realpath(__file__))
-HOMEDIR = os.getenv('RUNIT_HOMEDIR', os.path.realpath(os.path.join(CURRENT_PATH, '..')))
+HOMEDIR = os.path.join(os.getenv('USERPROFILE', os.getenv('HOME')), 'RUNIT_WORKDIR')
 PROJECTS_DIR = os.path.join(HOMEDIR, 'projects')
 
 admin = Blueprint('admin', __name__, subdomain='admin', static_folder=os.path.join('..','static'))
 
 @admin.before_request
 def authorize():
     pass
```

### Comparing `runit-server-0.2.3/runit_server/blueprints/functions.py` & `runit-server-0.2.4/runit_server/blueprints/functions.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/blueprints/public.py` & `runit-server-0.2.4/runit_server/blueprints/public.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dotenv import load_dotenv, find_dotenv, dotenv_values
 
 from runit import RunIt
 
 load_dotenv()
 
 CURRENT_PATH = os.path.dirname(os.path.realpath(__file__))
-HOMEDIR = os.getenv('RUNIT_HOMEDIR', os.path.realpath(os.path.join(CURRENT_PATH, '..')))
+HOMEDIR =  os.path.join(os.getenv('USERPROFILE', os.getenv('HOME')), 'RUNIT_WORKDIR')
 PROJECTS_DIR = os.path.join(HOMEDIR, 'projects')
 
 public = Blueprint('public', __name__)
 
 '''
 @public.before_request
 def initial():
@@ -32,28 +32,33 @@
         return redirect(url_for('setup.index'))
     if 'user_id' in session:
         return redirect(url_for('account.index'))
     return render_template('login.html')
 
 @public.get('/<string:project_id>/')
 def project(project_id):
-    if os.path.isdir(os.path.join(PROJECTS_DIR, project_id)):
-        result = RunIt.start(project_id, 'index', os.path.join(PROJECTS_DIR, project_id))
-        os.chdir(HOMEDIR)
-        return result
+    current_project_dir = os.path.join(PROJECTS_DIR, project_id)
+    if os.path.isdir(current_project_dir):
+        if not RunIt.is_private(project_id, current_project_dir):
+            result = RunIt.start(project_id, 'index', current_project_dir)
+            os.chdir(HOMEDIR)
+            
+            return result
 
     return RunIt.notfound()
 
 @public.get('/<string:project_id>/<string:function>')
 @public.get('/<string:project_id>/<string:function>/')
 def run(project_id, function):
-    if os.path.isdir(os.path.join(PROJECTS_DIR, project_id)):
-        result = RunIt.start(project_id, function, os.path.join(PROJECTS_DIR, project_id))
-        os.chdir(HOMEDIR)
-        return result
+    current_project_dir = os.path.join(PROJECTS_DIR, project_id)
+    if os.path.isdir(current_project_dir):
+        if not RunIt.is_private(project_id, current_project_dir):
+            result = RunIt.start(project_id, function, current_project_dir)
+            os.chdir(HOMEDIR)
+            return result
 
     return RunIt.notfound()
 
 @public.route('/register/', methods=['GET', 'POST'])
 def register():
     if request.method == 'POST':
         name = request.form.get('name')
```

### Comparing `runit-server-0.2.3/runit_server/blueprints/setup.py` & `runit-server-0.2.4/runit_server/blueprints/setup.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/cli.py` & `runit-server-0.2.4/runit_server/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 from odbms import DBMS
 from .models import Role, Admin
 
 load_dotenv()
 
 CURDIR = os.path.dirname(os.path.realpath(__file__))
-VERSION = "0.2.3"
+WORKDIR = os.path.join(os.getenv('USERPROFILE', os.getenv('HOME')), 'RUNIT_WORKDIR')
+VERSION = "0.2.4"
 
 def setup_database():
     '''
     Connect to database using connection settings from .env
     
     @params None
     @return None
@@ -36,19 +37,22 @@
         Role('developer', []).save()
         Role('superadmin', []).save()
         Role('subadmin', []).save()
         print('[--] Roles populated')
     
 
 def create_folders():
-    if not os.path.exists(os.path.join(CURDIR, 'projects')):
-        os.mkdir(os.path.join(CURDIR, 'projects'))
+    if not os.path.exists(WORKDIR):
+        os.mkdir(WORKDIR)
     
-    if not os.path.exists(os.path.join(CURDIR, 'accounts')):
-        os.mkdir(os.path.join(CURDIR, 'accounts'))
+    if not (os.path.exists(os.path.join(WORKDIR, 'accounts'))):
+        os.mkdir(os.path.join(WORKDIR, 'accounts'))
+        
+    if not (os.path.exists(os.path.join(WORKDIR, 'projects'))):
+        os.mkdir(os.path.join(WORKDIR, 'projects'))
 
 def create_dot_env(settings: dict):
     '''
     Create .env file and populate with {settings}
     
     @param settings dict Dictionary of default settings
     @return None
@@ -108,14 +112,15 @@
         
     domain = args.domain if hasattr(args, 'domain') else ''
     allowed = ['DBMS', 'DATABASE_HOST', 'DATABASE_PORT', 
                'DATABASE_USERNAME', 'DATABASE_PASSWORD', 
                'DATABASE_NAME', 'RUNTIME_PYTHON',
                'RUNTIME_PHP', 'RUNTIME_JAVASCRIPT']
     default_settings = {
+        'RUNIT_WORKDIR': os.path.join(os.getenv('USERPROFILE', os.getenv('HOME')), 'RUNIT_WORKDIR'),
         'RUNIT_HOMEDIR': CURDIR,
         'RUNIT_SERVERNAME': '',
         'DBMS': 'mongodb',
         'DATABASE_HOST': 'localhost',
         'DATABASE_PORT': '27017',
         'DATABASE_USERNAME': '',
         'DATABASE_PASSWORD': '',
@@ -159,14 +164,17 @@
 
 def run_server(args = None):
     if not find_dotenv():
         print('[#] Complete Setup configuration first.\n')
         setup_runit(args)
         print('')
 
+    os.environ['RUNIT_DOCKER'] = str(args.docker)
+    os.environ['RUNIT_KUBERNETES'] = str(args.kubernetes)
+
     if args and args.production:
         serve(app, listen=f"*:{args.port}")
     else:
         app.run(host=args.host, port=args.port, debug=args.debug)
 
 def get_arguments():
     global parser
@@ -181,17 +189,19 @@
     setup_parser.add_argument('--dbport', type=str, help="Database host port")
     setup_parser.add_argument('--dbusername', type=str, help="Database user username")
     setup_parser.add_argument('--dbpassword', type=str, help="Database user password")
     setup_parser.add_argument('--dbname', type=str, help="Database name")
     setup_parser.add_argument('--admin', action='store_true', help="Manage administrator account")
     setup_parser.set_defaults(func=setup_runit)
     
+    parser.add_argument('--docker', action='store_true', help="Run program in docker container")
+    parser.add_argument('--kubernetes', action='store_true', help="Run program using kubernetes")
     parser.add_argument('--host', type=str, default='127.0.0.1', help='Host address to run server on')
     parser.add_argument('--port', type=int, default=9000, help='Host port to run server on')
-    parser.add_argument('--debug', type=bool, choices=[True, False], default=True, help="Enable debug mode")
+    parser.add_argument('--debug', action='store_true', help="Enable debug mode")
     parser.add_argument('--production', action='store_true', help="Run in production mode")
     parser.add_argument('-v','--version', action='version', version=f'%(prog)s {VERSION}')
     parser.set_defaults(func=run_server)
     return parser.parse_args()
 
 def main():
     global parser
```

### Comparing `runit-server-0.2.3/runit_server/common/apis.py` & `runit-server-0.2.4/runit_server/common/apis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from odbms import DBMS, normalise
-from flask import request, jsonify
+from flask import request, jsonify, send_from_directory
 from flask_restful import Resource
 from flask_jwt_extended import jwt_required, create_access_token, get_jwt_identity, get_jwt
 
 from werkzeug.utils import secure_filename
+from werkzeug.security import safe_join
 
 from ..models import Function
 from ..models import Project
 from ..models import User
 from ..models import Database
+from ..models import Collection
 from .security import authenticate
 
 import os
 from dotenv import load_dotenv
 from datetime import datetime, timedelta
+from threading import Thread
 
 from runit import RunIt
 
 load_dotenv()
 
 CURRENT_PATH = os.path.dirname(os.path.realpath(__file__))
-HOMEDIR = os.getenv('RUNIT_HOMEDIR', os.path.realpath(os.path.join(CURRENT_PATH, '..')))
-PROJECTS_DIR = os.path.join(HOMEDIR, 'projects')
+WORKDIR =  os.path.join(os.getenv('USERPROFILE', os.getenv('HOME')), 'RUNIT_WORKDIR')
+PROJECTS_DIR = os.path.join(WORKDIR, 'projects')
 
 def stringifyObjectIds(model: object, properties: list)-> object:
     for property in properties:
         property._id = str(property._id)
 
 class Login(Resource):
     '''
@@ -69,57 +72,59 @@
         '''
         Api for publishing project
 
         @param project_id Project _id
         @param function Function Name
         @return Projects: dict Get all projects
         '''
-        try:
-            data = dict(request.form)
-            file = request.files['file']
-            
-            result = {'status': 'success'}
-            user = User.get(get_jwt_identity())
 
+        data = dict(request.form)
+        file = request.files['file']
+        
+        result = {'status': 'success'}
+        user = User.get(get_jwt_identity())
+
+        
+        if not '_id' in data.keys() or not len(data['_id']):
+            del data['_id']
+            project = Project(user.id, **data)
+            project_id = project.save().inserted_id
+            project_id = str(project_id)
+            project.id = project_id
+            homepage = f"{os.getenv('RUNIT_PROTOCOL')}{os.getenv('RUNIT_SERVERNAME')}/{project_id}/"
+            project.update({'homepage': homepage})
+            result['project_id'] = project_id
+        else:
+            project_id = data['_id']
+            project = Project.get(data['_id'])
+            del data['_id']
+            project.update(data, {'id': project.id})
+
+        if not os.path.exists(os.path.join(PROJECTS_DIR, project_id)):
+            os.mkdir(os.path.join(PROJECTS_DIR, project_id))
             
-            if not '_id' in data.keys() or not len(data['_id']):
-                del data['_id']
-                project = Project(user.id, **data)
-                project_id = project.save().inserted_id
-                project_id = str(project_id)
-                project.id = project_id
-                homepage = f"{os.getenv('RUNIT_PROTOCOL')}{os.getenv('RUNIT_SERVERNAME')}/{project_id}/"
-                project.update({'homepage': homepage})
-                result['project_id'] = project_id
-            else:
-                project_id = data['_id']
-                project = Project.get(data['_id'])
-                del data['_id']
-                project.update(data, {'id': project.id})
-    
-            if not os.path.exists(os.path.join(PROJECTS_DIR, project_id)):
-                os.mkdir(os.path.join(PROJECTS_DIR, project_id))
-            filepath = os.path.join(PROJECTS_DIR, project_id, secure_filename(file.filename))
-            file.save(filepath)
-
-            RunIt.extract_project(filepath)
-            os.chdir(os.path.join(PROJECTS_DIR, project_id))
-            #os.unlink(secure_filename(file.filename))
-            runit = RunIt(**RunIt.load_config())
-            runit._id = project_id
-            runit.update_config()
-
-            funcs = []
-            for func in runit.get_functions():
-                funcs.append(f"{request.scheme}://{os.getenv('RUNIT_SERVERNAME')}/{project_id}/{func}/")
-            result['functions'] = funcs
-            result['homepage'] = f"{request.scheme}://{os.getenv('RUNIT_SERVERNAME')}/{project_id}/{func}/"
-            return result
-        except Exception as e:
-            return {'status': 'error', 'msg': str(e)}
+        filepath = os.path.join(PROJECTS_DIR, project_id, secure_filename(file.filename))
+        file.save(filepath)
+
+        RunIt.extract_project(filepath)
+        os.chdir(os.path.join(PROJECTS_DIR, project_id))
+        #os.unlink(secure_filename(file.filename))
+        runit = RunIt(**RunIt.load_config())
+        Thread(target=runit.install_dependency_packages, args=()).start()
+        
+        runit._id = project_id
+        runit.update_config()
+        
+        funcs = []
+        for func in runit.get_functions():
+            funcs.append(f"{request.scheme}://{os.getenv('RUNIT_SERVERNAME')}/{project_id}/{func}/")
+        
+        result['functions'] = funcs
+        result['homepage'] = funcs[0]
+        return result
 
 class ProjectCloneRS(Resource):
     '''
     Projects Api
     '''
 
     @jwt_required()
@@ -127,36 +132,37 @@
         '''
         Clone project from terminal
         
         @param project_id str ID of the project to clone
         @return Compressed file of files in project directory
         '''
         global PROJECTS_DIR
-        PROJECTS_DIR = os.path.realpath(os.path.join(CURRENT_PATH, '..', 'projects'))
         
-        project = Project.find({'name': project, 'user_id': get_jwt_identity()})
-        
-        if len(project):
-            if not os.path.exists(os.path.join(PROJECTS_DIR, project[0].id)):
-                raise Exception('Project not found!')
-                
-            os.chdir(os.path.join(PROJECTS_DIR, project[0].id))
-            config = RunIt.load_config()
-            
-            if not config:
-                raise FileNotFoundError
-            
-            project = RunIt(**config)
-            filename = project.compress()
-            os.chdir(HOMEDIR)
-            print(filename)
+        try:
+            project = Project.find_one({'name': project, 'user_id': get_jwt_identity()})
             
-            return send_from_directory(os.path.join(PROJECTS_DIR, project_id), filename, as_attachment=True)
-        else:
-            return jsonify({'status': 'error', 'msg': 'Project does not exist'})
+            if project:
+                if not os.path.exists(os.path.join(PROJECTS_DIR, project.id)):
+                    raise Exception('Project not found!')
+                    
+                os.chdir(os.path.join(PROJECTS_DIR, project.id))
+                config = RunIt.load_config()
+                
+                if not config:
+                    raise FileNotFoundError
+                
+                project = RunIt(**config)
+                filename = project.compress()
+                # os.chdir(WORKDIR)
+                
+                return send_from_directory(safe_join(PROJECTS_DIR, project._id), filename, as_attachment=True)
+            else:
+                return jsonify({'status': 'error', 'msg': 'Project does not exist'})
+        except Exception as e:
+            return jsonify({'status': 'error', 'msg': str(e)})
 
 class ProjectById(Resource):
     '''
     Project Api
     '''
 
     @jwt_required()
@@ -234,61 +240,68 @@
     '''
     Api for manipulating documents (crud)
     '''
 
     @jwt_required()
     def post(self, project_id, collection):
         '''
-        Api for retrieving documents
+        Endpoint for CRUD actions on documents
 
         @param project_id Project ID
         @param collection Collection Name
         @return Documents Documents from collection
         '''
 
         try:
             data = request.get_json()
 
+            user_id = get_jwt_identity()
+            db = Database.find_one({'user_id': user_id, 'name': collection})
+            
+            if not db:
+                raise NameError("Collection wasn't found")
+
+            Collection.TABLE_NAME = db.collection_name
+            
             if not 'function' in data.keys():
                 raise SyntaxError('No database function to run')
             
             function = data['function']
 
-            if function == 'all' or function == 'find_many':
-                results = Database.find({'project_id': project_id, 'name': collection})
-                #results = DBMS.Database.find(db, {}, data['columns'])
+            if function == 'all' or function == 'find' or function == 'find_many':
+                projection = {}
+                for item in data['projection']:
+                    projection[item] = 1
+                results = Collection.find(data['_filter'], projection)
 
             elif function == 'find_one':
-                data['filter']['project_id'] = project_id
-                data['filter']['name'] = collection
-                results = Database.find(data['filter'])[0]
-                #results = DBMS.Database.find_one(db, normalise(data['filter'], 'params'), data['columns'])
+                projection = {}
+                for item in data['projection']:
+                    projection[item] = 1
+                
+                results = Collection.find_one(data['_filter'], projection)
 
             elif function == 'insert':
-                update_document = {collection: data['document']}
-                results = Database.update({'project_id': project_id, 'user_id': get_jwt_identity()}, update_document)
-                #results = DBMS.Database.insert(db, normalise(main_data, 'params')).inserted_id
+                results = Collection(**data['document']).save()
+            
+            elif function == 'insert_many':
+                results = Collection.insert_many(data['documents'])
 
             elif function == 'update':
-                data['filter']['name'] = collection
-                data['filter']['user_id'] = get_jwt_identity()
-                results = Database.update(data['filter'], data['update'])
-                #results = DBMS.Database.update(db, normalise(data['filter'], 'params'), normalise(data['update'], 'params'))
+                results = Collection.update(data['_filter'], data['update'])
             
             elif function == 'count':
-                data['filter']['name'] = collection
-                results = Database.count(data['filter'])
-                #results = DBMS.Database.count(db, normalise(data['filter'], 'params'))
+                results = Collection.count(data['_filter'])
             
-            if function == 'find_many' or function == 'all':
+            if function == 'find_many' or function == 'find' or function == 'all':
                 return jsonify([result.json() for result in results])
             elif function == 'find_one':
                 return jsonify(results.json())
             elif function == 'insert':
-                return jsonify({'status': 'success', 'msg': 'Operation successful'})
+                return jsonify({'status': 'success', 'msg': str(results.inserted_id)})
             elif function == 'count':
                 return jsonify({'count': results})
             else:
                 return jsonify({'status': 'success', 'msg': 'Operation successful'})
 
         except Exception as e:
             return jsonify({'status': 'error', 'msg': str(e)})
```

### Comparing `runit-server-0.2.3/runit_server/common/security.py` & `runit-server-0.2.4/runit_server/common/security.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/common/utils.py` & `runit-server-0.2.4/runit_server/common/utils.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/favicon.ico` & `runit-server-0.2.4/runit_server/favicon.ico`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/models/admin.py` & `runit-server-0.2.4/runit_server/models/admin.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/models/database.py` & `runit-server-0.2.4/runit_server/models/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from odbms import DBMS, Model
 
 class Database(Model):
     TABLE_NAME = 'databases'
 
-    def __init__(self, name, user_id, project_id = None, created_at=None, updated_at=None, id=None, **kwargs):
+    def __init__(self, name, collection_name, user_id, project_id = None, schema={}, created_at=None, updated_at=None, id=None, **kwargs):
         super().__init__(created_at, updated_at, id)
         self.name = name
+        self.collection_name = collection_name
         self.user_id = user_id
         self.project_id = project_id
+        self.schema = schema
 
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
     def save(self):
         '''
         Instance Method for saving Database instance to database
@@ -37,14 +39,27 @@
         @params None
         @return User Instance
         '''
 
         return Model.normalise(DBMS.Database.find_one('users', Model.normalise({'id': self.user_id}, 'params')))
 
     @classmethod
+    def get_by_name(cls, collection_name: str)-> list:
+        '''
+        Class Method for retrieving collection by a name
+
+        @param collectinon_name:str name of the collection
+        @return List of Database instances
+        '''
+        
+        databases = DBMS.Database.find(Database.TABLE_NAME, Model.normalise({'name': collection_name}, 'params'))
+        
+        return [cls(**Model.normalise(elem)) for elem in databases]
+    
+    @classmethod
     def get_by_user(cls, user_id: str)-> list:
         '''
         Class Method for retrieving databases by a user
 
         @param user_id:str _id of the user
         @return List of Database instances
         '''
```

### Comparing `runit-server-0.2.3/runit_server/models/function.py` & `runit-server-0.2.4/runit_server/models/function.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/models/permission.py` & `runit-server-0.2.4/runit_server/models/permission.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/models/project.py` & `runit-server-0.2.4/runit_server/models/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from odbms import DBMS, Model
 
 class Project(Model):
     TABLE_NAME = 'projects'
 
     def __init__(self, user_id, name, version="0.0.1", description="", homepage="",
-    language="", runtime="", start_file="", author={}, created_at=None, updated_at=None, id=None):
+    language="", runtime="", start_file="", private=False, author={}, created_at=None, updated_at=None, id=None):
         super().__init__(created_at, updated_at, id)
         self.name = name
         self.user_id = user_id
         self.version = version
         self.description = description
         self.homepage = homepage
         self.language = language
         self.runtime = runtime
+        self.private = private
         self.start_file = start_file
         self.author = author
 
     def save(self):
         '''
         Instance Method for saving Project instance to database
 
@@ -28,14 +29,15 @@
             "name": self.name,
             "user_id": self.user_id,
             "version": self.version,
             "description": self.description,
             "homepage": self.homepage,
             "language": self.language,
             "runtime": self.runtime,
+            "private": self.private,
             "start_file": self.start_file,
             "author": self.author
         }
 
         if DBMS.Database.dbms == 'mongodb':
             data["created_at"]: self.created_at
             data["updated_at"]: self.updated_at
@@ -84,14 +86,15 @@
             "name": self.name,
             "user_id": str(self.user_id),
             "version": self.version,
             "description": self.description,
             "homepage": self.homepage,
             "language": self.language,
             "runtime": self.runtime,
+            "private": self.private,
             "start_file": self.start_file,
             "author": self.author,
             "functions": self.count_functions(),
             "created_at": self.created_at,
             "updated_at": self.updated_at
         }
```

### Comparing `runit-server-0.2.3/runit_server/models/role.py` & `runit-server-0.2.4/runit_server/models/role.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/models/user.py` & `runit-server-0.2.4/runit_server/models/user.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/modules/account.py` & `runit-server-0.2.4/runit_server/modules/account.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/css/all.min.css` & `runit-server-0.2.4/runit_server/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/css/bootstrap.min.css` & `runit-server-0.2.4/runit_server/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/css/bootstrap.min.css.map` & `runit-server-0.2.4/runit_server/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/css/styles.css` & `runit-server-0.2.4/runit_server/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/html5.svg` & `runit-server-0.2.4/runit_server/static/images/logos/html5.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/nodejs.png` & `runit-server-0.2.4/runit_server/static/images/logos/nodejs.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/nodejs.svg` & `runit-server-0.2.4/runit_server/static/images/logos/nodejs.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/php.svg` & `runit-server-0.2.4/runit_server/static/images/logos/php.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/python.png` & `runit-server-0.2.4/runit_server/static/images/logos/python.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/python.svg` & `runit-server-0.2.4/runit_server/static/images/logos/python.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/python1.svg` & `runit-server-0.2.4/runit_server/static/images/logos/python1.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png` & `runit-server-0.2.4/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/images/terminal.svg` & `runit-server-0.2.4/runit_server/static/images/terminal.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/bootstrap.bundle.min.js` & `runit-server-0.2.4/runit_server/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/bootstrap.bundle.min.js.map` & `runit-server-0.2.4/runit_server/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/main.js` & `runit-server-0.2.4/runit_server/static/js/main.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/projects.js` & `runit-server-0.2.4/runit_server/static/js/projects.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/scripts.js` & `runit-server-0.2.4/runit_server/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/js/setup.js` & `runit-server-0.2.4/runit_server/static/js/setup.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.eot` & `runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.svg` & `runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.ttf` & `runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.woff` & `runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-brands-400.woff2` & `runit-server-0.2.4/runit_server/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.eot` & `runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.svg` & `runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.ttf` & `runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.woff` & `runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-regular-400.woff2` & `runit-server-0.2.4/runit_server/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.eot` & `runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.svg` & `runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.ttf` & `runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.woff` & `runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/static/webfonts/fa-solid-900.woff2` & `runit-server-0.2.4/runit_server/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/404.html` & `runit-server-0.2.4/runit_server/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/account/home.html` & `runit-server-0.2.4/runit_server/templates/account/home.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/account/layout.html` & `runit-server-0.2.4/runit_server/templates/account/layout.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,135 @@
-<!DOCTYPE html>
-<html>
-
-<head>
-    <meta charset="utf-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
-
-    <link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800" rel="s
-tylesheet">
-    <link href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900" rel="styles
-heet">
-    <link href="https://fonts.googleapis.com/css?family=Roboto+Condensed:300,400,700" rel="st
-ylesheet">
-    <link href="https://fonts.googleapis.com/css?family=Josefin+Sans:300,300i,400,400i,700,700i" rel="stylesheet">
-
-    <title>{% block title %}Runit{% endblock %}</title>
-    <meta name='viewport'
-        content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
-    <meta name="description" content="">
-    <meta name="keywords" content="">
-    <!-- <link rel="stylesheet" href="/static/css/open-iconic-bootstrap.min.css"> -->
-    <link rel="stylesheet" href="/static/css/animate.css">
-
-    <link href="/static/css/bootstrap.min.css" rel="stylesheet">
-    <link href="/static/css/all.min.css" rel="stylesheet">
-
-    <link rel='icon' href="{{url_for('static', filename='images/terminal.svg')}}">
-
-    <meta name="msapplication-TileColor" content="#ffff00">
-    
-    <meta name="theme-color" content="#ffff00">
-</head>
-
-<body class="bg-light bg-gradient">
-    <style>
-        body {
-            overflow: hidden;
-            font-size: 16px;
-        }
-
-        .sidebar a:hover {
-            opacity: 1 !important;
-        }
-    
-        .sidebar a.active {
-            opacity: 1 !important;
-        }
-
-        .main-content {
-            height: 100vh;
-            overflow-y: auto;
-        }
-
-        .hover\:shadow-sm:hover {
-            box-shadow: 0 .125rem .25rem rgba(0,0,0,.075)!important;
-        }
-
-        .hover\:text-dark:hover {
-            color: rgba(var(--bs-dark-rgb),var(--bs-text-opacity))!important;
-        }
-
-        @media screen and (min-width: 576px) {
-            .main-content {
-                height: 80vh;
-            }
-        }
-    </style>
-    <div class="offcanvas offcanvas-start w-auto" tabindex="-1" id="offcanvasMenu" aria-labelledby="offcanvasMenuLabel">
-        <div class="offcanvas-header">
-            <h5 class="offcanvas-title" id="offcanvasMenuLabel">Menu</h5>
-            <!--<button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>-->
-        </div>
-        <div class="offcanvas-body d-flex flex-column text-bg-light">
-            {% for item in session['menu'] %}
-            <a href="{{ url_for(item['url']) }}" 
-                class="nav-link p-2 py-3 opacity-75 {% if item['name'] == page %}opacity-100{% endif %}"
-                title="{{ item['name'] | capitalize }}">
-                <i class="fas fa-{{ item['icon']}} fa-fw fa-2x"></i>
-            </a>
-            {% endfor %}
-            <a href="{{ url_for('account.logout') }}" class="nav-link p-2 py-3 text-danger position-absolute bottom-0">
-                <i class="fas fa-sign-out-alt fa-fw fa-2x"></i>
-            </a>
-        </div>
-    </div>
-
-    <main class="vh-100 vw-100 d-flex justify-content-center align-items-center">
-        <div class="container">
-            <div class="row justify-content-center">
-                <div class="col-12 col-lg-10 p-0">
-                    <div class="card shadow align-self-center">
-                        <div class="card-body p-0">
-                            <div class="d-flex">
-                                {% include 'sidebar.html' %}
-                                <div class="main-content w-100 position-relative">
-                                    <nav class="d-flex justify-content-between p-4">
-                                        <a href="#offcanvasMenu" class="nav-link text-dark d-sm-none" data-bs-toggle="offcanvas" role="button" aria-controls="offcanvasMenu">
-                                            <i class="fas fa-bars fa-2x fa-fw"></i>
-                                        </a>
-                                        <div class="h5">
-                                            <strong>
-                                                {% block pagetitle %}
-                                                {{ page | upper }}
-                                                {% endblock %}
-                                            </strong>
-                                        </div>
-                                    </nav>
-                                    {% block content %}
-                                    {% endblock %}
-                                </div>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-    </main>
-    {% block scripts %}
-    <script src="{{url_for('static', filename='js/bootstrap.bundle.min.js')}}"></script>
-    {% endblock %}
-</body>
-</html>
+<!DOCTYPE html>
+<html>
+
+<head>
+    <meta charset="utf-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
+
+    <link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800" rel="s
+tylesheet">
+    <link href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900" rel="styles
+heet">
+    <link href="https://fonts.googleapis.com/css?family=Roboto+Condensed:300,400,700" rel="st
+ylesheet">
+    <link href="https://fonts.googleapis.com/css?family=Josefin+Sans:300,300i,400,400i,700,700i" rel="stylesheet">
+
+    <title>{% block title %}Runit{% endblock %}</title>
+    <meta name='viewport'
+        content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
+    <meta name="description" content="">
+    <meta name="keywords" content="">
+
+    <link href="/static/css/bootstrap.min.css" rel="stylesheet">
+    <link href="/static/css/all.min.css" rel="stylesheet">
+
+    <link rel='icon' href="{{url_for('static', filename='images/terminal.svg')}}">
+
+    <meta name="msapplication-TileColor" content="#ffff00">
+    
+    <meta name="theme-color" content="#ffff00">
+</head>
+
+<body class="bg-light bg-gradient">
+    <style>
+        body {
+            overflow: hidden;
+            font-size: 16px;
+        }
+
+        .sidebar a:hover {
+            opacity: 1 !important;
+        }
+    
+        .sidebar a.active {
+            opacity: 1 !important;
+        }
+
+        .main-content {
+            height: 100vh;
+            overflow-y: auto;
+        }
+
+        .hover\:shadow-sm:hover {
+            box-shadow: 0 .125rem .25rem rgba(0,0,0,.075)!important;
+        }
+
+        .hover\:text-dark:hover {
+            color: rgba(var(--bs-dark-rgb),var(--bs-text-opacity))!important;
+        }
+
+        .custom-flex-wrap {
+            flex-wrap: wrap;
+        }
+
+        .white-space-nowrap {
+            white-space: nowrap;
+        }
+
+        @media screen and (min-width: 576px) {
+            .main-content {
+                height: 80vh;
+            }
+        }
+    </style>
+    <div class="offcanvas offcanvas-start w-auto" tabindex="-1" id="offcanvasMenu" aria-labelledby="offcanvasMenuLabel">
+        <div class="offcanvas-header">
+            <h5 class="offcanvas-title" id="offcanvasMenuLabel">Menu</h5>
+            <!--<button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>-->
+        </div>
+        {% set menu = [
+            {'name': 'home', 'icon': 'home', 'url': 'account.index'},
+            {'name': 'projects', 'icon': 'sitemap', 'url': 'project.index'},
+            {'name': 'functions', 'icon': 'terminal', 'url': 'account.functions'},
+            {'name': 'databases', 'icon': 'database', 'url': 'database.index'},
+            {'name': 'profile', 'icon': 'user', 'url': 'account.profile'}
+        ] %}
+        <div class="offcanvas-body d-flex flex-column text-bg-light">
+            {% for item in menu %}
+            <a href="{{ url_for(item['url']) }}" 
+                class="nav-link p-2 py-3 text-secondary {% if item['name'] == page %}text-dark{% endif %}"
+                title="{{ item['name'] | capitalize }}">
+                <i class="fas fa-{{ item['icon']}} fa-fw fa-2x"></i>
+            </a>
+            {% endfor %}
+            <a href="{{ url_for('account.logout') }}" class="nav-link p-2 py-3 text-danger position-absolute bottom-0">
+                <i class="fas fa-sign-out-alt fa-fw fa-2x"></i>
+            </a>
+        </div>
+    </div>
+
+    <main class="vh-100 vw-100 d-flex justify-content-center align-items-center">
+        <div class="container">
+            <div class="row justify-content-center">
+                <div class="col-12 col-lg-10 p-0">
+                    <div class="card shadow align-self-center">
+                        <div class="card-body p-0">
+                            <div class="d-flex">
+                                {% include 'sidebar.html' %}
+                                <div class="main-content w-100 position-relative">
+                                    <nav class="d-flex justify-content-between p-4">
+                                        <a href="#offcanvasMenu" class="nav-link text-dark d-sm-none" data-bs-toggle="offcanvas" role="button" aria-controls="offcanvasMenu">
+                                            <i class="fas fa-bars fa-2x fa-fw"></i>
+                                        </a>
+                                        <div class="h5">
+                                            <strong>
+                                                {% block pagetitle %}
+                                                {{ page | upper }}
+                                                {% endblock %}
+                                            </strong>
+                                        </div>
+                                    </nav>
+                                    {% block content %}
+                                    {% endblock %}
+                                </div>
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
+        </div>
+    </main>
+    {% block scripts %}
+    <script src="{{url_for('static', filename='js/bootstrap.bundle.min.js')}}"></script>
+    {% endblock %}
+</body>
+</html>
```

#### html2text {}

```diff
@@ -6,16 +6,20 @@
 
 
 
 
 
 
 
-
 ** Menu **
-{% for item in session['menu'] %}  {% endfor %}
+{% set menu = [ {'name': 'home', 'icon': 'home', 'url': 'account.index'},
+{'name': 'projects', 'icon': 'sitemap', 'url': 'project.index'}, {'name':
+'functions', 'icon': 'terminal', 'url': 'account.functions'}, {'name':
+'databases', 'icon': 'database', 'url': 'database.index'}, {'name': 'profile',
+'icon': 'user', 'url': 'account.profile'} ] %}
+{% for item in menu %}  {% endfor %}
 {% include 'sidebar.html' %}
 
 {% block pagetitle %} {{ page | upper }} {% endblock %}
  {% block content %} {% endblock %}
  {% block scripts %}
  {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/account/profile.html` & `runit-server-0.2.4/runit_server/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/index.html` & `runit-server-0.2.4/runit_server/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/login.html` & `runit-server-0.2.4/runit_server/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/profile.html` & `runit-server-0.2.4/runit_server/templates/admin/profile.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/projects/details.html` & `runit-server-0.2.4/runit_server/templates/admin/users/details.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,173 +1,159 @@
 {% extends "admin/layout.html" %}
 {% block title %} 
-{{super()}} | {{page | capitalize}} | {{project.name}}
+{{super()}} | {{page | capitalize}} | {{user.name}}
 {% endblock %}
 
 {% block pagetitle %}
 <div class="d-flex align-items center">
-    <a href="{{url_for('admin.projects')}}" class="nav-link p-0 text-black-50 hover:text-dark">
+    <a href="{{url_for('admin.users')}}" class="nav-link p-0 text-black-50 hover:text-dark">
         <i class="fas fa-arrow-left fa-fw"></i> {{ super() }}</a>
     / 
-    <span>{{ project.name | upper}}</span>
+    <span>{{ user.name | upper}}</span>
 </div>
 {% endblock %}
 
 {% block content %}
-{% include 'admin/projects/modal.html' %}
+{% include 'admin/users/modal.html' %}
 <div class="container">
     {% for (category, message) in get_flashed_messages(with_categories=True) %}
     <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
         <strong>{{message}}</strong>
         <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
     </div>
     {% endfor %}
 
-    <div class="tools d-flex justify-content-end">
-        <div class="btn-group" role="group" aria-label="tool buttons">
-            <nav class="nav-item dropdown">
-                <a href="#" class="btn btn-sm btn-dark hover:shadow-sm mb-2" data-bs-toggle="dropdown" role="button" aria-expanded="false" title="Run Functions">
-                    <i class="fas fa-terminal"></i>
-                </a>
-                <ul class="dropdown-menu rounded-0 shadow py-0">
-                    {% for func in funcs %}
-                    <li>
-                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="dropdown-item small border-bottom text-bg-danger bg-gradient" target="_blank">
-                            <i class="fas fa-terminal fa-fw text-dark"></i> {{func.name}}
-                        </a>
-                    </li>
-                    {% endfor %}
-                </ul>
-            </nav>
-            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-secondary hover:shadow-sm mb-2" title="Disable Project">
-                <i class="fas fa-eye-slash"></i>
-            </a>
-            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-danger hover:shadow-sm mb-2" title="Delete Project">
-                <i class="fas fa-trash-alt"></i>
-            </a>
-        </div>
-    </div>
-
     <div class="card rounded-0 border-0">
         <nav>
             <div class="nav nav-tabs" id="nav-tab" role="tablist">
                 <button class="nav-link active rounded-0" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
-                    <small>Config</small>
+                    <small>Projects <span class="bg-dark text-white px-1">{{user['projects']}}</span></small>
                 </button>
-                <button class="nav-link rounded-0" id="nav-functions-tab" data-bs-toggle="tab" data-bs-target="#nav-functions" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
-                    <small>Functions</small>
+                <button class="nav-link rounded-0" id="nav-profile-tab" data-bs-toggle="tab" data-bs-target="#nav-profile" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
+                    <small>Profile</small>
                 </button>
-                <button class="nav-link rounded-0" id="nav-settings-tab" data-bs-toggle="tab" data-bs-target="#nav-settings" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
-                    <small>Settings</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-logs-tab" data-bs-toggle="tab" data-bs-target="#nav-logs" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false" disabled>
-                    <small>Logs</small>
+                <button class="nav-link rounded-0" id="nav-security-tab" data-bs-toggle="tab" data-bs-target="#nav-security" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false">
+                    <small>Security</small>
                 </button>
                 <button class="nav-link rounded-0" id="nav-console-tab" data-bs-toggle="tab" data-bs-target="#nav-console" type="button" role="tab" aria-controls="nav-console" aria-selected="false" disabled>
-                    <small>Console</small>
+                    <small>Settings</small>
                 </button>
             </div>
         </nav>
         <div class="tab-content" id="nav-tabContent">
             <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab" tabindex="0">
-                <div class="card rounded-0 border-0 shadow-sm my-2">
+
+                <div class="card rounded-0 border-0 my-2">
                     <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
                         <small class="fw-bold"></small>
-                        <div class="btn-group">
-                            <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
-                                <i class="fas fa-save fa-fw"></i> Update
-                            </button>
+                        <div class="tools d-flex justify-content-end">
+                            <div class="btn-group" role="group" aria-label="tool buttons">
+                                <a href="{{url_for('admin.user', user_id=user.id)}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
+                                    <small><i class="fas fa-th-large fa-fw"></i></small>
+                                </a>
+                                <a href="{{url_for('admin.user', user_id=user.id)}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
+                                    <small><i class="fas fa-th-list fa-fw"></i></small>
+                                </a>
+                                <a href="#confirmModal" role="button" class="btn btn-sm btn-danger" data-bs-toggle="modal">
+                                    <small><i class="fas fa-trash-alt fa-fw"></i></small>
+                                </a>
+                                <a href="#projectModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
+                                   <small>
+                                    <i class="fas fa-plus fa-fw"></i>
+                                    New Project
+                                   </small>
+                                </a>
+                            </div>
                         </div>
                     </div>
                     <div class="card-body pb-0">
                         <div class="row">
-                        {% for key, value in project.items() %}
-                            <div class="col-md-4">
-                                <div class="form-group mb-2">
-                                    <label for="">
-                                        <small>{{key}}</small>
-                                    </label>
-                                    <input type="text" value="{{value}}" placeholder="" class="form-control form-control-sm bg-gradient text-muted" readonly>
-                                </div>
-                            </div>
-                        {% endfor %}
+                            {% if view == 'list' %} 
+                            {% include 'admin/projects/list.html' %} 
+                            {% else %} 
+                            {% include 'admin/projects/grid.html' %}
+                            {% endif %}
                         </div>
                     </div>
                 </div>
             </div>
-            <div class="tab-pane fade bg-light" id="nav-functions" role="tabpanel" aria-labelledby="nav-functions-tab" tabindex="0">
-                <div class="card rounded-0 border-0 shadow-sm my-2 bg-light">
+            <div class="tab-pane fade" id="nav-profile" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
+                <div class="card rounded-0 border-0 my-2">
+                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
+                        <small class="fw-bold"></small>
+                        <div class="btn-group">
+                            <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
+                                <i class="fas fa-save fa-fw"></i> Update
+                            </button>
+                        </div>
+                    </div>
                     <div class="card-body pb-0">
                         <div class="row">
-                            <div class="col-md-6 d-flex flex-column">
-                                {% for func in funcs %}
-                                    <div class="d-flex justify-content-between align-items-center p-2 bg-white border border-light mb-2 rounded-1">
-                                        <a href="{{func.link}}" class="nav-link p-0" target="_blank">
-                                            <h4 class="small text-primary text-uppercase">{{func.name}}</h4>
-                                        </a>
-                                        <a href="{{func.link}}" class="nav-link p-0" target="_blank">
-                                            <i class="fas fa-terminal fa-fw text-bg-dark p-1 rounded-1"></i>
-                                        </a>
-                                    </div>
-                                {% endfor %}
+                            <div class="col-md-8 mb-2">
+                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
+                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Full Name</div>
+                                    <input type="text" value="{{user.name}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end">
+                                </div>
+                            </div>
+                            <div class="col-md-8 mb-2">
+                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
+                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Email Address</div>
+                                    <input type="text" value="{{user.email}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
+                                </div>
+                            </div>
+                            <div class="col-md-8 mb-2">
+                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
+                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">No. of Projects</div>
+                                    <input type="text" value="{{user.projects}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
+                                </div>
+                            </div>
+                            <div class="col-md-8 mb-2">
+                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
+                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Signup Date</div>
+                                    <input type="text" value="{{user.created_at}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
+                                </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
-            <div class="tab-pane fade" id="nav-settings" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
+            <div class="tab-pane fade" id="nav-security" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">
                 <div class="row">
-                    <div class="col-md-6">
-                        <div class="card rounded-0 border-0 shadow-sm my-2">
-                            <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
-                                <small class="fw-bold">Environment Variables</small>
-                                <div class="btn-group">
-                                    <button type="button" class="btn btn-sm btn-dark" onclick="createEnv()">
-                                        <i class="fas fa-plus"></i>
-                                    </button>
-                                    <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
-                                        <i class="fas fa-save fa-fw"></i> Save
-                                    </button>
-                                </div>
-                            </div>
-                            <div class="card-body pb-0">
-                                <form action="{{url_for('project.environ', project_id=project._id)}}" method="post" class="env-form">
-                                    {% for key, value in environs.items() %}
-                                    {% set id = 'env'+(loop.index | string) %}
-                                    {% set envKey = 'envKey'+(loop.index | string) %}
-                                        <div class="form-group row align-items-center mb-2" id="{{id}}">
-                                            <div class="col-5">
-                                                <input type="text" value="{{key}}" placeholder="key" class="form-control form-control-sm key-input" data-name="{{envKey}}" required onkeyup="setEnvKey(this)">
-                                            </div>
-                                            <div class="col-1">
-                                                <span>=</span>
-                                            </div>
-                                            <div class="col-5">
-                                                <input type="text" name="{{key}}" value="{{value}}" placeholder="value" id="{{envKey}}" class="form-control form-control-sm" required>
-                                            </div>
-                                            <div class="col-1">
-                                                <a href="javascript: deleteElem('{{id}}')" class="nav-link">
-                                                    <i class="fas fa-trash-alt"></i>
-                                                </a>
-                                            </div>
-                                        </div>
-                                    {% endfor %}
-                                </form>
+                    <div class="col-md-6 pt-4">
+                        <div class="card">
+                            <div class="card-header">Update Password</div>
+                            <div class="card-body">
+                                <div class="form-group mb-2">
+                                    <label for="">
+                                        <small>Current Password</small>
+                                    </label>
+                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
+                                </div>
+                                <div class="form-group mb-2">
+                                    <label for="">
+                                        <small>New Password</small>
+                                    </label>
+                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
+                                </div>
+                                <div class="form-group mb-2">
+                                    <label for="">
+                                        <small>Confirm New Password</small>
+                                    </label>
+                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
+                                </div>
                             </div>
                         </div>
                     </div>
-                    <div class="col-md-6"></div>
                 </div>
             </div>
-            <div class="tab-pane fade" id="nav-logs" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">...</div>
             <div class="tab-pane fade" id="nav-console" role="tabpanel" aria-labelledby="nav-console-tab" tabindex="0">
                 Terminal Console
             </div>
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
-<script src="{{url_for('static', filename='js/projects.js')}}"></script>
+<script src="{{url_for('static', filename='js/users.js')}}"></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,34 +1,29 @@
 {% extends "admin/layout.html" %} {% block title %} {{super()}} | {{page |
-capitalize}} | {{project.name}} {% endblock %} {% block pagetitle %}
+capitalize}} | {{user.name}} {% endblock %} {% block pagetitle %}
  {{_super()_}}
- / {{ project.name | upper}}
-{% endblock %} {% block content %} {% include 'admin/projects/modal.html' %}
+ / {{ user.name | upper}}
+{% endblock %} {% block content %} {% include 'admin/users/modal.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
 {% endfor %}
+ Projects {{user['projects']}}   Profile   Security   Settings
 
-    * {% for func in funcs %}
-    *  {{func.name}}
-    * {% endfor %}
-
- Config   Functions   Settings   Logs   Console
+ New_Project
+{% if view == 'list' %} {% include 'admin/projects/list.html' %} {% else %} {%
+include 'admin/projects/grid.html' %} {% endif %}
   Update
-{% for key, value in project.items() %}
- {{key}}  [{{value}}           ]
-{% endfor %}
-{% for func in funcs %}
-***_{{func.name}}_***
-
-{% endfor %}
-Environment Variables
-     Save
-{% for key, value in environs.items() %} {% set id = 'env'+(loop.index |
-string) %} {% set envKey = 'envKey'+(loop.index | string) %}
-[{{key}}             ]
-=
-[{{value}}           ]
-{% endfor %}
-...
+Full Name
+[{{user.name}}       ]
+Email Address
+[{{user.email}}      ]
+No. of Projects
+[{{user.projects}}   ]
+Signup Date
+[{{user.created_at}} ]
+Update Password
+ Current Password  [********************]
+ New Password  [********************]
+ Confirm New Password  [********************]
 Terminal Console
 {% endblock %} {% block scripts %} {{super()}}
  {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/projects/index.html` & `runit-server-0.2.4/runit_server/templates/admin/users/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 
 {% block title %}
 {{super()}} | {{page | capitalize}}
 {% endblock %}
 
 {% block content %}
 {% include 'modals/confirm.html' %}
-{% include 'projects/modal.html' %}
+{% include 'admin/users/modal.html' %}
 <div class="container">
     {% for (category, message) in get_flashed_messages(with_categories=True) %}
     <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
         <strong>{{message}}</strong>
         <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
     </div>
     {% endfor %}
-    {% if projects %}
+    {% if users %}
 
     <div class="tools d-flex justify-content-end">
         <div class="btn-group" role="group" aria-label="tool buttons">
-            <a href="{{url_for('project.index')}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
+            <a href="{{url_for('admin.users')}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
                 <small><i class="fas fa-th-large fa-fw"></i></small>
             </a>
-            <a href="{{url_for('project.index')}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
+            <a href="{{url_for('admin.users')}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
                 <small><i class="fas fa-th-list fa-fw"></i></small>
             </a>
             <a href="#confirmModal" role="button" class="btn btn-sm btn-danger" data-bs-toggle="modal">
                 <small><i class="fas fa-trash-alt fa-fw"></i></small>
             </a>
-            <a href="#projectModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
+            <a href="#userModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
                <small>
                 <i class="fas fa-plus fa-fw"></i>
-                New Project
+                New user
                </small>
             </a>
         </div>
     </div>
     {% if view == 'list' %} 
-    {% include 'admin/projects/list.html' %} 
+    {% include 'admin/users/list.html' %} 
     {% else %} 
-    {% include 'admin/projects/grid.html' %}
+    {% include 'admin/users/grid.html' %}
     {% endif %}
 </div>
 {% endif %}
-{% if not projects %}
-<a href="#projectModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="projectModal">
+{% if not users %}
+<a href="#userModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="userModal">
     <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
-    New Project
+    New user
 </a>
 {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends "admin/layout.html" %} {% block title %} {{super()}} | {{page |
 capitalize}} {% endblock %} {% block content %} {% include 'modals/
-confirm.html' %} {% include 'projects/modal.html' %}
+confirm.html' %} {% include 'admin/users/modal.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
-{% endfor %} {% if projects %}
+{% endfor %} {% if users %}
 
- New_Project
-{% if view == 'list' %} {% include 'admin/projects/list.html' %} {% else %} {%
-include 'admin/projects/grid.html' %} {% endif %}
-{% endif %} {% if not projects %}
- New_Project
+ New_user
+{% if view == 'list' %} {% include 'admin/users/list.html' %} {% else %} {%
+include 'admin/users/grid.html' %} {% endif %}
+{% endif %} {% if not users %}
+ New_user
  {% endif %} {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/projects/list.html` & `runit-server-0.2.4/runit_server/templates/admin/users/list.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-<div class="card rounded-0 border-0 shadow-sm p-0">
-    <div class="card-body p-0">
-        <div class="table-responsive">
-            <table class="table table-light table-striped table-hover mb-0 small">
-                <thead>
-                    <th>#</th>
-                    <th>Name</th>
-                    <th>Language</th>
-                    <th>Updated At</th>
-                    <th class="text-center">Actions</th>
-                </thead>
-                <tbody>
-                    {% for project in projects %}
-                    <tr>
-                        <td><input type="checkbox" name="" id="" class="form-check custom"></td>
-                        <td>
-                            <a href="{{url_for('project.details', project_id=project.id)}}" class="nav-link">
-                                {{ project['name'] }}
-                            </a>
-                        </td>
-                        <td>{{project['language']}}</td>
-                        <td>{{ project['updated_at'] }}</td>
-                        <td class="text-center">
-                            <nav class="dropdown">
-                                <a class="nav-link p-0" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
-                                    <i class="fas fa-ellipsis-v bg-white border rounded-circle"></i>
-                                </a>
-                                <ul class="dropdown-menu dropdown-menu-left position-fixed rounded-0 shadow" role="menu">
-                                    <li>
-                                        <a href="{{url_for('project.details', project_id=project['id'])}}" class="dropdown-item small py-0">
-                                            Open
-                                        </a>
-                                    </li>
-                                    <li><hr class="dropdown-divider"></li>
-                                    <li><a class="dropdown-item small py-0" href="#">Update</a></li>
-                                    <li><hr class="dropdown-divider"></li>
-                                    <li><a class="dropdown-item text-danger small py-0" href="#">Delete</a></li>
-                                </ul>
-                            </nav>
-                        </td>
-                    </tr>
-                    {% endfor %}
-                </tbody>
-            </table>
-        </div>
-    </div>
+<div class="card rounded-0 border-0 shadow-sm">
+    <div class="card-body p-0">
+        <div class="table-responsive">
+            <table class="table table-light table-striped table-hover mb-0 small">
+                <thead>
+                    <th>#</th>
+                    <th>Name</th>
+                    <th>Updated At</th>
+                    <th class="text-center">Actions</th>
+                </thead>
+                <tbody>
+                    {% for project in projects %}
+                    <tr>
+                        <td><input type="checkbox" name="" id="" class="form-check custom"></td>
+                        <td>
+                            <a href="{{url_for('project.details', project_id=project.id)}}" class="nav-link">
+                                {{ project['name'] }}
+                            </a>
+                        </td>
+                        <td>{{ project['updated_at'] }}</td>
+                        <td class="text-center">
+                            <nav class="dropdown">
+                                <a class="nav-link p-0" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
+                                    <i class="fas fa-ellipsis-v bg-white border rounded-circle"></i>
+                                </a>
+                                <ul class="dropdown-menu dropdown-menu-left position-fixed rounded-0 shadow border-0" role="menu">
+                                    <li>
+                                        <a href="{{url_for('project.details', project_id=project['id'])}}" class="dropdown-item small py-0">
+                                            Open
+                                        </a>
+                                    </li>
+                                    <li><hr class="dropdown-divider"></li>
+                                    <li><a class="dropdown-item small py-0" href="#">Update</a></li>
+                                    <li><hr class="dropdown-divider"></li>
+                                    <li><a class="dropdown-item text-danger small py-0" href="#">Delete</a></li>
+                                </ul>
+                            </nav>
+                        </td>
+                    </tr>
+                    {% endfor %}
+                </tbody>
+            </table>
+        </div>
+    </div>
 </div>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 
-                                                             * Open
-�{{_project['name']_}} {{project      {{ project            * ================
-                        ['language']}} ['updated_at'] }}     * Update
-                                                             * ================
-                                                             * Delete
+                                                        * Open
+�{{_project['name']_}} {{ project['updated_at'] }}     * =====================
+                                                        * Update
+                                                        * =====================
+                                                        * Delete
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/projects/modal.html` & `runit-server-0.2.4/runit_server/templates/admin/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/users/details.html` & `runit-server-0.2.4/runit_server/templates/admin/projects/details.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,159 +1,175 @@
-{% extends "admin/layout.html" %}
-{% block title %} 
-{{super()}} | {{page | capitalize}} | {{user.name}}
-{% endblock %}
-
-{% block pagetitle %}
-<div class="d-flex align-items center">
-    <a href="{{url_for('admin.users')}}" class="nav-link p-0 text-black-50 hover:text-dark">
-        <i class="fas fa-arrow-left fa-fw"></i> {{ super() }}</a>
-    / 
-    <span>{{ user.name | upper}}</span>
-</div>
-{% endblock %}
-
-{% block content %}
-{% include 'admin/users/modal.html' %}
-<div class="container">
-    {% for (category, message) in get_flashed_messages(with_categories=True) %}
-    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
-        <strong>{{message}}</strong>
-        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
-    </div>
-    {% endfor %}
-
-    <div class="card rounded-0 border-0">
-        <nav>
-            <div class="nav nav-tabs" id="nav-tab" role="tablist">
-                <button class="nav-link active rounded-0" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
-                    <small>Projects <span class="bg-dark text-white px-1">{{user['projects']}}</span></small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-profile-tab" data-bs-toggle="tab" data-bs-target="#nav-profile" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
-                    <small>Profile</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-security-tab" data-bs-toggle="tab" data-bs-target="#nav-security" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false">
-                    <small>Security</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-console-tab" data-bs-toggle="tab" data-bs-target="#nav-console" type="button" role="tab" aria-controls="nav-console" aria-selected="false" disabled>
-                    <small>Settings</small>
-                </button>
-            </div>
-        </nav>
-        <div class="tab-content" id="nav-tabContent">
-            <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab" tabindex="0">
-
-                <div class="card rounded-0 border-0 my-2">
-                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
-                        <small class="fw-bold"></small>
-                        <div class="tools d-flex justify-content-end">
-                            <div class="btn-group" role="group" aria-label="tool buttons">
-                                <a href="{{url_for('admin.user', user_id=user.id)}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
-                                    <small><i class="fas fa-th-large fa-fw"></i></small>
-                                </a>
-                                <a href="{{url_for('admin.user', user_id=user.id)}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
-                                    <small><i class="fas fa-th-list fa-fw"></i></small>
-                                </a>
-                                <a href="#confirmModal" role="button" class="btn btn-sm btn-danger" data-bs-toggle="modal">
-                                    <small><i class="fas fa-trash-alt fa-fw"></i></small>
-                                </a>
-                                <a href="#projectModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
-                                   <small>
-                                    <i class="fas fa-plus fa-fw"></i>
-                                    New Project
-                                   </small>
-                                </a>
-                            </div>
-                        </div>
-                    </div>
-                    <div class="card-body pb-0">
-                        <div class="row">
-                            {% if view == 'list' %} 
-                            {% include 'admin/projects/list.html' %} 
-                            {% else %} 
-                            {% include 'admin/projects/grid.html' %}
-                            {% endif %}
-                        </div>
-                    </div>
-                </div>
-            </div>
-            <div class="tab-pane fade" id="nav-profile" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
-                <div class="card rounded-0 border-0 my-2">
-                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
-                        <small class="fw-bold"></small>
-                        <div class="btn-group">
-                            <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
-                                <i class="fas fa-save fa-fw"></i> Update
-                            </button>
-                        </div>
-                    </div>
-                    <div class="card-body pb-0">
-                        <div class="row">
-                            <div class="col-md-8 mb-2">
-                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
-                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Full Name</div>
-                                    <input type="text" value="{{user.name}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end">
-                                </div>
-                            </div>
-                            <div class="col-md-8 mb-2">
-                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
-                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Email Address</div>
-                                    <input type="text" value="{{user.email}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
-                                </div>
-                            </div>
-                            <div class="col-md-8 mb-2">
-                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
-                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">No. of Projects</div>
-                                    <input type="text" value="{{user.projects}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
-                                </div>
-                            </div>
-                            <div class="col-md-8 mb-2">
-                                <div class="form-group d-flex border border-dark mb-2 rounded-end">
-                                    <div class="d-flex align-items-center justify-content-center border-end border-dark w-50 bg-dark text-white">Signup Date</div>
-                                    <input type="text" value="{{user.created_at}}" placeholder="" class="form-control form-control-sm rounded-0 rounded-end bg-white" readonly>
-                                </div>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-            <div class="tab-pane fade" id="nav-security" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">
-                <div class="row">
-                    <div class="col-md-6 pt-4">
-                        <div class="card">
-                            <div class="card-header">Update Password</div>
-                            <div class="card-body">
-                                <div class="form-group mb-2">
-                                    <label for="">
-                                        <small>Current Password</small>
-                                    </label>
-                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
-                                </div>
-                                <div class="form-group mb-2">
-                                    <label for="">
-                                        <small>New Password</small>
-                                    </label>
-                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
-                                </div>
-                                <div class="form-group mb-2">
-                                    <label for="">
-                                        <small>Confirm New Password</small>
-                                    </label>
-                                    <input type="password" value="" placeholder="" class="form-control form-control-sm">
-                                </div>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-            <div class="tab-pane fade" id="nav-console" role="tabpanel" aria-labelledby="nav-console-tab" tabindex="0">
-                Terminal Console
-            </div>
-        </div>
-    </div>
-</div>
-{% endblock %}
-
-{% block scripts %} 
-{{super()}}
-<script src="{{url_for('static', filename='js/users.js')}}"></script>
+{% extends "admin/layout.html" %}
+{% block title %} 
+{{super()}} | {{page | capitalize}} | {{project.name}}
+{% endblock %}
+
+{% block pagetitle %}
+<div class="d-flex align-items center custom-flex-wrap white-space-nowrap">
+    <a href="{{url_for('admin.projects')}}" class="nav-link p-0 text-black-50 hover:text-dark">
+        <i class="fas fa-arrow-left fa-fw"></i> 
+        <span class="d-none d-sm-inline">{{ super() }}</span>
+    </a>
+    <span class="d-none d-sm-inline">/</span>
+    <span>{{ project.name | upper}}</span>
+</div>
+{% endblock %}
+
+{% block content %}
+{% include 'admin/projects/modal.html' %}
+<div class="container">
+    {% for (category, message) in get_flashed_messages(with_categories=True) %}
+    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
+        <strong>{{message}}</strong>
+        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
+    </div>
+    {% endfor %}
+
+    <div class="tools d-flex justify-content-end">
+        <div class="btn-group" role="group" aria-label="tool buttons">
+            <nav class="nav-item dropdown">
+                <a href="#" class="btn btn-sm btn-dark hover:shadow-sm mb-2" data-bs-toggle="dropdown" role="button" aria-expanded="false" title="Run Functions">
+                    <i class="fas fa-terminal"></i>
+                </a>
+                <ul class="dropdown-menu rounded-0 shadow py-0">
+                    {% for func in funcs %}
+                    <li>
+                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="dropdown-item small border-bottom text-bg-danger bg-gradient" target="_blank">
+                            <i class="fas fa-terminal fa-fw text-dark"></i> {{func.name}}
+                        </a>
+                    </li>
+                    {% endfor %}
+                </ul>
+            </nav>
+            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-secondary hover:shadow-sm mb-2" title="Disable Project">
+                <i class="fas fa-eye-slash"></i>
+            </a>
+            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-danger hover:shadow-sm mb-2" title="Delete Project">
+                <i class="fas fa-trash-alt"></i>
+            </a>
+        </div>
+    </div>
+
+    <div class="card rounded-0 border-0">
+        <nav>
+            <div class="nav nav-tabs" id="nav-tab" role="tablist">
+                <button class="nav-link active rounded-0" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
+                    <small>Config</small>
+                </button>
+                <button class="nav-link rounded-0" id="nav-functions-tab" data-bs-toggle="tab" data-bs-target="#nav-functions" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
+                    <small>Functions</small>
+                </button>
+                <button class="nav-link rounded-0" id="nav-settings-tab" data-bs-toggle="tab" data-bs-target="#nav-settings" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
+                    <small>Settings</small>
+                </button>
+                <button class="nav-link rounded-0" id="nav-logs-tab" data-bs-toggle="tab" data-bs-target="#nav-logs" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false" disabled>
+                    <small>Logs</small>
+                </button>
+                <button class="nav-link rounded-0" id="nav-console-tab" data-bs-toggle="tab" data-bs-target="#nav-console" type="button" role="tab" aria-controls="nav-console" aria-selected="false" disabled>
+                    <small>Console</small>
+                </button>
+            </div>
+        </nav>
+        <div class="tab-content" id="nav-tabContent">
+            <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab" tabindex="0">
+                <div class="card rounded-0 border-0 shadow-sm my-2">
+                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
+                        <small class="fw-bold"></small>
+                        <div class="btn-group">
+                            <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
+                                <i class="fas fa-save fa-fw"></i> Update
+                            </button>
+                        </div>
+                    </div>
+                    <div class="card-body pb-0">
+                        <div class="row">
+                        {% for key, value in project.items() %}
+                            <div class="col-md-4">
+                                <div class="form-group mb-2">
+                                    <label for="">
+                                        <small>{{key}}</small>
+                                    </label>
+                                    <input type="text" value="{{value}}" placeholder="" class="form-control form-control-sm bg-gradient text-muted" readonly>
+                                </div>
+                            </div>
+                        {% endfor %}
+                        </div>
+                    </div>
+                </div>
+            </div>
+            <div class="tab-pane fade bg-light" id="nav-functions" role="tabpanel" aria-labelledby="nav-functions-tab" tabindex="0">
+                <div class="card rounded-0 border-0 shadow-sm my-2 bg-light">
+                    <div class="card-body pb-0">
+                        <div class="row">
+                            <div class="col-md-6 d-flex flex-column">
+                                {% for func in funcs %}
+                                    <div class="d-flex justify-content-between align-items-center p-2 bg-white border border-light mb-2 rounded-1">
+                                        <a href="{{func.link}}" class="nav-link p-0" target="_blank">
+                                            <h4 class="small text-primary text-uppercase">{{func.name}}</h4>
+                                        </a>
+                                        <a href="{{func.link}}" class="nav-link p-0" target="_blank">
+                                            <i class="fas fa-terminal fa-fw text-bg-dark p-1 rounded-1"></i>
+                                        </a>
+                                    </div>
+                                {% endfor %}
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
+            <div class="tab-pane fade" id="nav-settings" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
+                <div class="row">
+                    <div class="col-md-6">
+                        <div class="card rounded-0 border-0 shadow-sm my-2">
+                            <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
+                                <small class="fw-bold">Environment Variables</small>
+                                <div class="btn-group">
+                                    <button type="button" class="btn btn-sm btn-dark" onclick="createEnv()">
+                                        <i class="fas fa-plus"></i>
+                                    </button>
+                                    <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
+                                        <i class="fas fa-save fa-fw"></i> Save
+                                    </button>
+                                </div>
+                            </div>
+                            <div class="card-body pb-0">
+                                <form action="{{url_for('project.environ', project_id=project._id)}}" method="post" class="env-form">
+                                    {% for key, value in environs.items() %}
+                                    {% set id = 'env'+(loop.index | string) %}
+                                    {% set envKey = 'envKey'+(loop.index | string) %}
+                                        <div class="form-group row align-items-center mb-2" id="{{id}}">
+                                            <div class="col-5">
+                                                <input type="text" value="{{key}}" placeholder="key" class="form-control form-control-sm key-input" data-name="{{envKey}}" required onkeyup="setEnvKey(this)">
+                                            </div>
+                                            <div class="col-1">
+                                                <span>=</span>
+                                            </div>
+                                            <div class="col-5">
+                                                <input type="text" name="{{key}}" value="{{value}}" placeholder="value" id="{{envKey}}" class="form-control form-control-sm" required>
+                                            </div>
+                                            <div class="col-1">
+                                                <a href="javascript: deleteElem('{{id}}')" class="nav-link">
+                                                    <i class="fas fa-trash-alt"></i>
+                                                </a>
+                                            </div>
+                                        </div>
+                                    {% endfor %}
+                                </form>
+                            </div>
+                        </div>
+                    </div>
+                    <div class="col-md-6"></div>
+                </div>
+            </div>
+            <div class="tab-pane fade" id="nav-logs" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">...</div>
+            <div class="tab-pane fade" id="nav-console" role="tabpanel" aria-labelledby="nav-console-tab" tabindex="0">
+                Terminal Console
+            </div>
+        </div>
+    </div>
+</div>
+{% endblock %}
+
+{% block scripts %} 
+{{super()}}
+<script src="{{url_for('static', filename='js/projects.js')}}"></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,29 +1,34 @@
 {% extends "admin/layout.html" %} {% block title %} {{super()}} | {{page |
-capitalize}} | {{user.name}} {% endblock %} {% block pagetitle %}
+capitalize}} | {{project.name}} {% endblock %} {% block pagetitle %}
  {{_super()_}}
- / {{ user.name | upper}}
-{% endblock %} {% block content %} {% include 'admin/users/modal.html' %}
+ / {{ project.name | upper}}
+{% endblock %} {% block content %} {% include 'admin/projects/modal.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
 {% endfor %}
- Projects {{user['projects']}}   Profile   Security   Settings
 
- New_Project
-{% if view == 'list' %} {% include 'admin/projects/list.html' %} {% else %} {%
-include 'admin/projects/grid.html' %} {% endif %}
+    * {% for func in funcs %}
+    *  {{func.name}}
+    * {% endfor %}
+
+ Config   Functions   Settings   Logs   Console
   Update
-Full Name
-[{{user.name}}       ]
-Email Address
-[{{user.email}}      ]
-No. of Projects
-[{{user.projects}}   ]
-Signup Date
-[{{user.created_at}} ]
-Update Password
- Current Password  [********************]
- New Password  [********************]
- Confirm New Password  [********************]
+{% for key, value in project.items() %}
+ {{key}}  [{{value}}           ]
+{% endfor %}
+{% for func in funcs %}
+***_{{func.name}}_***
+
+{% endfor %}
+Environment Variables
+     Save
+{% for key, value in environs.items() %} {% set id = 'env'+(loop.index |
+string) %} {% set envKey = 'envKey'+(loop.index | string) %}
+[{{key}}             ]
+=
+[{{value}}           ]
+{% endfor %}
+...
 Terminal Console
 {% endblock %} {% block scripts %} {{super()}}
  {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/users/grid.html` & `runit-server-0.2.4/runit_server/templates/admin/users/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/admin/users/index.html` & `runit-server-0.2.4/runit_server/templates/admin/projects/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-{% extends "admin/layout.html" %}
-
-{% block title %}
-{{super()}} | {{page | capitalize}}
-{% endblock %}
-
-{% block content %}
-{% include 'modals/confirm.html' %}
-{% include 'admin/users/modal.html' %}
-<div class="container">
-    {% for (category, message) in get_flashed_messages(with_categories=True) %}
-    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
-        <strong>{{message}}</strong>
-        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
-    </div>
-    {% endfor %}
-    {% if users %}
-
-    <div class="tools d-flex justify-content-end">
-        <div class="btn-group" role="group" aria-label="tool buttons">
-            <a href="{{url_for('admin.users')}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
-                <small><i class="fas fa-th-large fa-fw"></i></small>
-            </a>
-            <a href="{{url_for('admin.users')}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
-                <small><i class="fas fa-th-list fa-fw"></i></small>
-            </a>
-            <a href="#confirmModal" role="button" class="btn btn-sm btn-danger" data-bs-toggle="modal">
-                <small><i class="fas fa-trash-alt fa-fw"></i></small>
-            </a>
-            <a href="#userModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
-               <small>
-                <i class="fas fa-plus fa-fw"></i>
-                New user
-               </small>
-            </a>
-        </div>
-    </div>
-    {% if view == 'list' %} 
-    {% include 'admin/users/list.html' %} 
-    {% else %} 
-    {% include 'admin/users/grid.html' %}
-    {% endif %}
-</div>
-{% endif %}
-{% if not users %}
-<a href="#userModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="userModal">
-    <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
-    New user
-</a>
-{% endif %}
-{% endblock %}
+{% extends "admin/layout.html" %}
+
+{% block title %}
+{{super()}} | {{page | capitalize}}
+{% endblock %}
+
+{% block content %}
+{% include 'modals/confirm.html' %}
+{% include 'projects/modal.html' %}
+<div class="container">
+    {% for (category, message) in get_flashed_messages(with_categories=True) %}
+    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
+        <strong>{{message}}</strong>
+        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
+    </div>
+    {% endfor %}
+    {% if projects %}
+    <div class="tools d-flex justify-content-end">
+        <div class="btn-group shadow-sm" role="group" aria-label="tool buttons">
+            <a href="{{url_for('project.index')}}" class="btn btn-{{'' if view != 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Grid view">
+                <small><i class="fas fa-th-large fa-fw"></i></small>
+            </a>
+            <a href="{{url_for('project.index')}}?view=list" class="btn btn-{{'' if view == 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Table view">
+                <small><i class="fas fa-th-list fa-fw"></i></small>
+            </a>
+        </div>
+        <div class="btn-group shadow-sm ms-3" role="group" aria-label="tool buttons">
+            <a href="#confirmModal" role="button" class="btn btn-outline-danger bg-gradient" data-bs-toggle="modal">
+                <small><i class="fas fa-trash-alt fa-fw"></i></small>
+            </a>
+            <a href="#projectModal" role="button" class="btn btn-outline-primary bg-gradient" data-bs-toggle="modal">
+               <small>
+                <i class="fas fa-plus fa-fw"></i>
+                New Project
+               </small>
+            </a>
+        </div>
+    </div>
+    {% if view == 'list' %} 
+    {% include 'admin/projects/list.html' %} 
+    {% else %} 
+    {% include 'admin/projects/grid.html' %}
+    {% endif %}
+</div>
+{% endif %}
+{% if not projects %}
+<a href="#projectModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="projectModal">
+    <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
+    New Project
+</a>
+{% endif %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "admin/layout.html" %} {% block title %} {{super()}} | {{page |
 capitalize}} {% endblock %} {% block content %} {% include 'modals/
-confirm.html' %} {% include 'admin/users/modal.html' %}
+confirm.html' %} {% include 'projects/modal.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
-{% endfor %} {% if users %}
+{% endfor %} {% if projects %}
 
- New_user
-{% if view == 'list' %} {% include 'admin/users/list.html' %} {% else %} {%
-include 'admin/users/grid.html' %} {% endif %}
-{% endif %} {% if not users %}
- New_user
+
+ New_Project
+{% if view == 'list' %} {% include 'admin/projects/list.html' %} {% else %} {%
+include 'admin/projects/grid.html' %} {% endif %}
+{% endif %} {% if not projects %}
+ New_Project
  {% endif %} {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/users/list.html` & `runit-server-0.2.4/runit_server/templates/admin/projects/list.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-<div class="card rounded-0 border-0 shadow-sm">
-    <div class="card-body p-0">
-        <div class="table-responsive">
-            <table class="table table-light table-striped table-hover mb-0 small">
-                <thead>
-                    <th>#</th>
-                    <th>Name</th>
-                    <th>Updated At</th>
-                    <th class="text-center">Actions</th>
-                </thead>
-                <tbody>
-                    {% for project in projects %}
-                    <tr>
-                        <td><input type="checkbox" name="" id="" class="form-check custom"></td>
-                        <td>
-                            <a href="{{url_for('project.details', project_id=project.id)}}" class="nav-link">
-                                {{ project['name'] }}
-                            </a>
-                        </td>
-                        <td>{{ project['updated_at'] }}</td>
-                        <td class="text-center">
-                            <nav class="dropdown">
-                                <a class="nav-link p-0" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
-                                    <i class="fas fa-ellipsis-v bg-white border rounded-circle"></i>
-                                </a>
-                                <ul class="dropdown-menu dropdown-menu-left position-fixed rounded-0 shadow" role="menu">
-                                    <li>
-                                        <a href="{{url_for('project.details', project_id=project['id'])}}" class="dropdown-item small py-0">
-                                            Open
-                                        </a>
-                                    </li>
-                                    <li><hr class="dropdown-divider"></li>
-                                    <li><a class="dropdown-item small py-0" href="#">Update</a></li>
-                                    <li><hr class="dropdown-divider"></li>
-                                    <li><a class="dropdown-item text-danger small py-0" href="#">Delete</a></li>
-                                </ul>
-                            </nav>
-                        </td>
-                    </tr>
-                    {% endfor %}
-                </tbody>
-            </table>
-        </div>
-    </div>
+<div class="card rounded-0 border-0 shadow-sm p-0">
+    <div class="card-body p-0">
+        <div class="table-responsive">
+            <table class="table table-light table-striped table-hover mb-0 small">
+                <thead>
+                    <th>#</th>
+                    <th>Name</th>
+                    <th>Language</th>
+                    <!-- <th>Updated At</th> -->
+                    <th class="text-center">Actions</th>
+                </thead>
+                <tbody>
+                    {% for project in projects %}
+                    <tr>
+                        <td><input type="checkbox" name="" id="" class="form-check custom"></td>
+                        <td>
+                            <a href="{{url_for('project.details', project_id=project.id)}}" class="nav-link">
+                                {{ project['name'] }}
+                            </a>
+                        </td>
+                        <td>{{project['language']}}</td>
+                        <!-- <td>{{ project['updated_at'] }}</td> -->
+                        <td class="d-flex justify-content-center gap-3">
+                            <a href="{{url_for('project.details', project_id=project.id)}}" class="nav-link">
+                                <i class="far fa-file-alt text-primary"></i>
+                            </a>
+                            <a href="#confirmModal" role="button" class="nav-link"  data-bs-toggle="modal">
+                                <i class="fas fa-trash-alt text-danger"></i>
+                            </a>
+                        </td>
+                    </tr>
+                    {% endfor %}
+                </tbody>
+            </table>
+        </div>
+    </div>
 </div>
```

#### html2text {}

```diff
@@ -1,6 +1 @@
-
-                                                        * Open
-�{{_project['name']_}} {{ project['updated_at'] }}     * =====================
-                                                        * Update
-                                                        * =====================
-                                                        * Delete
+�{{_project['name']_}} {{project['language']}}
```

### Comparing `runit-server-0.2.3/runit_server/templates/admin/users/modal.html` & `runit-server-0.2.4/runit_server/templates/admin/users/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/databases/details.html` & `runit-server-0.2.4/runit_server/templates/setup/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,432 +1,467 @@
-00000000: 7b25 2065 7874 656e 6473 2022 6163 636f  {% extends "acco
-00000010: 756e 742f 6c61 796f 7574 2e68 746d 6c22  unt/layout.html"
-00000020: 2025 7d0a 7b25 2062 6c6f 636b 2074 6974   %}.{% block tit
-00000030: 6c65 2025 7d20 0a7b 7b73 7570 6572 2829  le %} .{{super()
-00000040: 7d7d 207c 207b 7b70 6167 6520 7c20 6361  }} | {{page | ca
-00000050: 7069 7461 6c69 7a65 7d7d 207c 207b 7b64  pitalize}} | {{d
-00000060: 6174 6162 6173 652e 6e61 6d65 7d7d 0a7b  atabase.name}}.{
-00000070: 2520 656e 6462 6c6f 636b 2025 7d0a 0a7b  % endblock %}..{
-00000080: 2520 626c 6f63 6b20 7061 6765 7469 746c  % block pagetitl
-00000090: 6520 257d 0a3c 6469 7620 636c 6173 733d  e %}.<div class=
-000000a0: 2264 2d66 6c65 7820 616c 6967 6e2d 6974  "d-flex align-it
-000000b0: 656d 7320 6365 6e74 6572 223e 0a20 2020  ems center">.   
-000000c0: 203c 6120 6872 6566 3d22 7b7b 7572 6c5f   <a href="{{url_
-000000d0: 666f 7228 2764 6174 6162 6173 652e 696e  for('database.in
-000000e0: 6465 7827 297d 7d22 2063 6c61 7373 3d22  dex')}}" class="
-000000f0: 6e61 762d 6c69 6e6b 2070 2d30 2074 6578  nav-link p-0 tex
-00000100: 742d 626c 6163 6b2d 3530 2068 6f76 6572  t-black-50 hover
-00000110: 3a74 6578 742d 6461 726b 223e 0a20 2020  :text-dark">.   
-00000120: 2020 2020 203c 6920 636c 6173 733d 2266       <i class="f
-00000130: 6173 2066 612d 6172 726f 772d 6c65 6674  as fa-arrow-left
-00000140: 2066 612d 6677 223e 3c2f 693e 207b 7b20   fa-fw"></i> {{ 
-00000150: 7375 7065 7228 2920 7d7d 3c2f 613e 0a20  super() }}</a>. 
-00000160: 2020 202f 200a 2020 2020 3c73 7061 6e3e     / .    <span>
-00000170: 7b7b 2064 6174 6162 6173 652e 6e61 6d65  {{ database.name
-00000180: 207c 2075 7070 6572 7d7d 3c2f 7370 616e   | upper}}</span
-00000190: 3e0a 3c2f 6469 763e 0a7b 2520 656e 6462  >.</div>.{% endb
-000001a0: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-000001b0: 6b20 636f 6e74 656e 7420 257d 0a7b 2520  k content %}.{% 
-000001c0: 696e 636c 7564 6520 2764 6174 6162 6173  include 'databas
-000001d0: 6573 2f6d 6f64 616c 2e68 746d 6c27 2025  es/modal.html' %
-000001e0: 7d0a 3c64 6976 2063 6c61 7373 3d22 636f  }.<div class="co
-000001f0: 6e74 6169 6e65 7222 3e0a 2020 2020 7b25  ntainer">.    {%
-00000200: 2066 6f72 2028 6361 7465 676f 7279 2c20   for (category, 
-00000210: 6d65 7373 6167 6529 2069 6e20 6765 745f  message) in get_
-00000220: 666c 6173 6865 645f 6d65 7373 6167 6573  flashed_messages
-00000230: 2877 6974 685f 6361 7465 676f 7269 6573  (with_categories
-00000240: 3d54 7275 6529 2025 7d0a 2020 2020 3c64  =True) %}.    <d
-00000250: 6976 2063 6c61 7373 3d22 616c 6572 7420  iv class="alert 
-00000260: 616c 6572 742d 7b7b 6361 7465 676f 7279  alert-{{category
-00000270: 7d7d 2061 6c65 7274 2d64 6973 6d69 7373  }} alert-dismiss
-00000280: 6962 6c65 2062 672d 6772 6164 6965 6e74  ible bg-gradient
-00000290: 2064 2d66 6c65 7820 6a75 7374 6966 792d   d-flex justify-
-000002a0: 636f 6e74 656e 742d 6265 7477 6565 6e20  content-between 
-000002b0: 726f 756e 6465 642d 3022 3e0a 2020 2020  rounded-0">.    
-000002c0: 2020 2020 3c73 7472 6f6e 673e 7b7b 6d65      <strong>{{me
-000002d0: 7373 6167 657d 7d3c 2f73 7472 6f6e 673e  ssage}}</strong>
-000002e0: 0a20 2020 2020 2020 203c 6275 7474 6f6e  .        <button
-000002f0: 2074 7970 653d 2262 7574 746f 6e22 2063   type="button" c
-00000300: 6c61 7373 3d22 6274 6e20 6274 6e2d 636c  lass="btn btn-cl
-00000310: 6f73 6522 2064 6174 612d 6273 2d64 6973  ose" data-bs-dis
-00000320: 6d69 7373 3d22 616c 6572 7422 3e3c 2f62  miss="alert"></b
-00000330: 7574 746f 6e3e 0a20 2020 203c 2f64 6976  utton>.    </div
-00000340: 3e0a 2020 2020 7b25 2065 6e64 666f 7220  >.    {% endfor 
-00000350: 257d 0a0a 2020 2020 3c64 6976 2063 6c61  %}..    <div cla
-00000360: 7373 3d22 746f 6f6c 7320 642d 666c 6578  ss="tools d-flex
-00000370: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-00000380: 2d65 6e64 223e 0a20 2020 2020 2020 203c  -end">.        <
-00000390: 6469 7620 636c 6173 733d 2262 746e 2d67  div class="btn-g
-000003a0: 726f 7570 2220 726f 6c65 3d22 6772 6f75  roup" role="grou
-000003b0: 7022 2061 7269 612d 6c61 6265 6c3d 2274  p" aria-label="t
-000003c0: 6f6f 6c20 6275 7474 6f6e 7322 3e0a 2020  ool buttons">.  
-000003d0: 2020 2020 2020 2020 2020 3c61 2068 7265            <a hre
-000003e0: 663d 227b 7b20 7572 6c5f 666f 7228 2764  f="{{ url_for('d
-000003f0: 6174 6162 6173 652e 696e 6465 7827 297d  atabase.index')}
-00000400: 7d22 2072 6f6c 653d 2262 7574 746f 6e22  }" role="button"
-00000410: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
-00000420: 736d 2062 746e 2d73 6563 6f6e 6461 7279  sm btn-secondary
-00000430: 2062 672d 6772 6164 6965 6e74 2068 6f76   bg-gradient hov
-00000440: 6572 3a73 6861 646f 772d 736d 206d 622d  er:shadow-sm mb-
-00000450: 3222 2074 6974 6c65 3d22 4469 7361 626c  2" title="Disabl
-00000460: 6520 4461 7461 6261 7365 223e 0a20 2020  e Database">.   
-00000470: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
-00000480: 636c 6173 733d 2266 6173 2066 612d 6579  class="fas fa-ey
-00000490: 652d 736c 6173 6822 3e3c 2f69 3e0a 2020  e-slash"></i>.  
-000004a0: 2020 2020 2020 2020 2020 3c2f 613e 0a20            </a>. 
-000004b0: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
-000004c0: 6566 3d22 7b7b 2075 726c 5f66 6f72 2827  ef="{{ url_for('
-000004d0: 6461 7461 6261 7365 2e69 6e64 6578 2729  database.index')
-000004e0: 7d7d 2220 726f 6c65 3d22 6275 7474 6f6e  }}" role="button
-000004f0: 2220 636c 6173 733d 2262 746e 2062 746e  " class="btn btn
-00000500: 2d73 6d20 6274 6e2d 6461 6e67 6572 2062  -sm btn-danger b
-00000510: 672d 6772 6164 6965 6e74 2068 6f76 6572  g-gradient hover
-00000520: 3a73 6861 646f 772d 736d 206d 622d 3222  :shadow-sm mb-2"
-00000530: 2074 6974 6c65 3d22 4465 6c65 7465 2044   title="Delete D
-00000540: 6174 6162 6173 6522 3e0a 2020 2020 2020  atabase">.      
-00000550: 2020 2020 2020 2020 2020 3c69 2063 6c61            <i cla
-00000560: 7373 3d22 6661 7320 6661 2d74 7261 7368  ss="fas fa-trash
-00000570: 2d61 6c74 223e 3c2f 693e 0a20 2020 2020  -alt"></i>.     
-00000580: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
-00000590: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
-000005a0: 2f64 6976 3e0a 0a20 2020 203c 6469 7620  /div>..    <div 
-000005b0: 636c 6173 733d 2263 6172 6420 726f 756e  class="card roun
-000005c0: 6465 642d 3020 626f 7264 6572 2d30 223e  ded-0 border-0">
-000005d0: 0a20 2020 2020 2020 203c 6e61 763e 0a20  .        <nav>. 
-000005e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000005f0: 636c 6173 733d 226e 6176 206e 6176 2d74  class="nav nav-t
-00000600: 6162 7322 2069 643d 226e 6176 2d74 6162  abs" id="nav-tab
-00000610: 2220 726f 6c65 3d22 7461 626c 6973 7422  " role="tablist"
-00000620: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000630: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
-00000640: 226e 6176 2d6c 696e 6b20 6163 7469 7665  "nav-link active
-00000650: 2072 6f75 6e64 6564 2d30 2220 6964 3d22   rounded-0" id="
-00000660: 6e61 762d 686f 6d65 2d74 6162 2220 6461  nav-home-tab" da
-00000670: 7461 2d62 732d 746f 6767 6c65 3d22 7461  ta-bs-toggle="ta
-00000680: 6222 2064 6174 612d 6273 2d74 6172 6765  b" data-bs-targe
-00000690: 743d 2223 6e61 762d 686f 6d65 2220 7479  t="#nav-home" ty
-000006a0: 7065 3d22 6275 7474 6f6e 2220 726f 6c65  pe="button" role
-000006b0: 3d22 7461 6222 2061 7269 612d 636f 6e74  ="tab" aria-cont
-000006c0: 726f 6c73 3d22 6e61 762d 686f 6d65 2220  rols="nav-home" 
-000006d0: 6172 6961 2d73 656c 6563 7465 643d 2274  aria-selected="t
-000006e0: 7275 6522 3e0a 2020 2020 2020 2020 2020  rue">.          
-000006f0: 2020 2020 2020 2020 2020 3c73 6d61 6c6c            <small
-00000700: 3e44 6574 6169 6c73 3c2f 736d 616c 6c3e  >Details</small>
-00000710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000720: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
-00000730: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
-00000740: 6f6e 2063 6c61 7373 3d22 6e61 762d 6c69  on class="nav-li
-00000750: 6e6b 2072 6f75 6e64 6564 2d30 2220 6964  nk rounded-0" id
-00000760: 3d22 6e61 762d 6675 6e63 7469 6f6e 732d  ="nav-functions-
-00000770: 7461 6222 2064 6174 612d 6273 2d74 6f67  tab" data-bs-tog
-00000780: 676c 653d 2274 6162 2220 6461 7461 2d62  gle="tab" data-b
-00000790: 732d 7461 7267 6574 3d22 236e 6176 2d63  s-target="#nav-c
-000007a0: 6f6c 6c65 6374 696f 6e73 2220 7479 7065  ollections" type
-000007b0: 3d22 6275 7474 6f6e 2220 726f 6c65 3d22  ="button" role="
-000007c0: 7461 6222 2061 7269 612d 636f 6e74 726f  tab" aria-contro
-000007d0: 6c73 3d22 6e61 762d 636f 6c6c 6563 7469  ls="nav-collecti
-000007e0: 6f6e 7322 2061 7269 612d 7365 6c65 6374  ons" aria-select
-000007f0: 6564 3d22 7472 7565 223e 0a20 2020 2020  ed="true">.     
-00000800: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000810: 736d 616c 6c3e 436f 6c6c 6563 7469 6f6e  small>Collection
-00000820: 733c 2f73 6d61 6c6c 3e0a 2020 2020 2020  s</small>.      
-00000830: 2020 2020 2020 2020 2020 3c2f 6275 7474            </butt
-00000840: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00000850: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
-00000860: 733d 226e 6176 2d6c 696e 6b20 726f 756e  s="nav-link roun
-00000870: 6465 642d 3022 2069 643d 226e 6176 2d73  ded-0" id="nav-s
-00000880: 6574 7469 6e67 732d 7461 6222 2064 6174  ettings-tab" dat
-00000890: 612d 6273 2d74 6f67 676c 653d 2274 6162  a-bs-toggle="tab
-000008a0: 2220 6461 7461 2d62 732d 7461 7267 6574  " data-bs-target
-000008b0: 3d22 236e 6176 2d73 6574 7469 6e67 7322  ="#nav-settings"
-000008c0: 2074 7970 653d 2262 7574 746f 6e22 2072   type="button" r
-000008d0: 6f6c 653d 2274 6162 2220 6172 6961 2d63  ole="tab" aria-c
-000008e0: 6f6e 7472 6f6c 733d 226e 6176 2d73 6574  ontrols="nav-set
-000008f0: 7469 6e67 7322 2061 7269 612d 7365 6c65  tings" aria-sele
-00000900: 6374 6564 3d22 6661 6c73 6522 3e0a 2020  cted="false">.  
-00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000920: 2020 3c73 6d61 6c6c 3e53 6574 7469 6e67    <small>Setting
-00000930: 733c 2f73 6d61 6c6c 3e0a 2020 2020 2020  s</small>.      
-00000940: 2020 2020 2020 2020 2020 3c2f 6275 7474            </butt
-00000950: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00000960: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
-00000970: 733d 226e 6176 2d6c 696e 6b20 726f 756e  s="nav-link roun
-00000980: 6465 642d 3022 2069 643d 226e 6176 2d63  ded-0" id="nav-c
-00000990: 6f6e 736f 6c65 2d74 6162 2220 6461 7461  onsole-tab" data
-000009a0: 2d62 732d 746f 6767 6c65 3d22 7461 6222  -bs-toggle="tab"
-000009b0: 2064 6174 612d 6273 2d74 6172 6765 743d   data-bs-target=
-000009c0: 2223 6e61 762d 636f 6e73 6f6c 6522 2074  "#nav-console" t
-000009d0: 7970 653d 2262 7574 746f 6e22 2072 6f6c  ype="button" rol
-000009e0: 653d 2274 6162 2220 6172 6961 2d63 6f6e  e="tab" aria-con
-000009f0: 7472 6f6c 733d 226e 6176 2d63 6f6e 736f  trols="nav-conso
-00000a00: 6c65 2220 6172 6961 2d73 656c 6563 7465  le" aria-selecte
-00000a10: 643d 2266 616c 7365 2220 6469 7361 626c  d="false" disabl
-00000a20: 6564 3e0a 2020 2020 2020 2020 2020 2020  ed>.            
-00000a30: 2020 2020 2020 2020 3c73 6d61 6c6c 3e43          <small>C
-00000a40: 6f6e 736f 6c65 3c2f 736d 616c 6c3e 0a20  onsole</small>. 
-00000a50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000a60: 2f62 7574 746f 6e3e 0a09 0909 093c 6275  /button>.....<bu
-00000a70: 7474 6f6e 2063 6c61 7373 3d22 6e61 762d  tton class="nav-
-00000a80: 6c69 6e6b 2072 6f75 6e64 6564 2d30 2220  link rounded-0" 
-00000a90: 6964 3d22 6e61 762d 696e 6974 6961 6c69  id="nav-initiali
-00000aa0: 7a61 7469 6f6e 2d74 6162 2220 6461 7461  zation-tab" data
-00000ab0: 2d62 732d 746f 6767 6c65 3d22 7461 6222  -bs-toggle="tab"
-00000ac0: 2064 6174 612d 6273 2d74 6172 6765 743d   data-bs-target=
-00000ad0: 2223 6e61 762d 696e 6974 6961 6c69 7a61  "#nav-initializa
-00000ae0: 7469 6f6e 2220 7479 7065 3d22 6275 7474  tion" type="butt
-00000af0: 6f6e 2220 726f 6c65 3d22 7461 6222 2061  on" role="tab" a
-00000b00: 7269 612d 636f 6e74 726f 6c73 3d22 6e61  ria-controls="na
-00000b10: 762d 696e 6974 6961 6c69 7a61 7469 6f6e  v-initialization
-00000b20: 2220 6172 6961 2d73 656c 6563 7465 643d  " aria-selected=
-00000b30: 2266 616c 7365 223e 0a20 2020 2020 2020  "false">.       
-00000b40: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
-00000b50: 616c 6c3e 496e 6974 6961 6c69 7a61 7469  all>Initializati
-00000b60: 6f6e 3c2f 736d 616c 6c3e 0a20 2020 2020  on</small>.     
-00000b70: 2020 2020 2020 2020 2020 203c 2f62 7574             </but
-00000b80: 746f 6e3e 0a20 2020 2020 2020 2020 2020  ton>.           
-00000b90: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000ba0: 3c2f 6e61 763e 0a20 2020 2020 2020 203c  </nav>.        <
-00000bb0: 6469 7620 636c 6173 733d 2274 6162 2d63  div class="tab-c
-00000bc0: 6f6e 7465 6e74 2220 6964 3d22 6e61 762d  ontent" id="nav-
-00000bd0: 7461 6243 6f6e 7465 6e74 223e 0a20 2020  tabContent">.   
-00000be0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000bf0: 6173 733d 2274 6162 2d70 616e 6520 6661  ass="tab-pane fa
-00000c00: 6465 2073 686f 7720 6163 7469 7665 2220  de show active" 
-00000c10: 6964 3d22 6e61 762d 686f 6d65 2220 726f  id="nav-home" ro
-00000c20: 6c65 3d22 7461 6270 616e 656c 2220 6172  le="tabpanel" ar
-00000c30: 6961 2d6c 6162 656c 6c65 6462 793d 226e  ia-labelledby="n
-00000c40: 6176 2d68 6f6d 652d 7461 6222 2074 6162  av-home-tab" tab
-00000c50: 696e 6465 783d 2230 223e 0a20 2020 2020  index="0">.     
-00000c60: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000c70: 636c 6173 733d 2263 6172 6420 726f 756e  class="card roun
-00000c80: 6465 642d 3020 626f 7264 6572 2d30 2073  ded-0 border-0 s
-00000c90: 6861 646f 772d 736d 206d 792d 3222 3e0a  hadow-sm my-2">.
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000cc0: 6361 7264 2d68 6561 6465 7220 702d 3020  card-header p-0 
-00000cd0: 702d 3220 642d 666c 6578 206a 7573 7469  p-2 d-flex justi
-00000ce0: 6679 2d63 6f6e 7465 6e74 2d62 6574 7765  fy-content-betwe
-00000cf0: 656e 2061 6c69 6e67 2d69 7465 6d73 2d63  en aling-items-c
-00000d00: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 3c73 6d61 6c6c 2063 6c61 7373 3d22 6677  <small class="fw
-00000d30: 2d62 6f6c 6422 3e3c 2f73 6d61 6c6c 3e0a  -bold"></small>.
+00000000: 7b25 2065 7874 656e 6473 2022 6c61 796f  {% extends "layo
+00000010: 7574 2e68 746d 6c22 2025 7d0a 7b25 2062  ut.html" %}.{% b
+00000020: 6c6f 636b 2074 6974 6c65 2025 7d0a 7b7b  lock title %}.{{
+00000030: 7375 7065 7228 297d 7d20 7c20 5365 7475  super()}} | Setu
+00000040: 7020 5061 6765 0a7b 2520 656e 6462 6c6f  p Page.{% endblo
+00000050: 636b 2025 7d0a 0a7b 2520 626c 6f63 6b20  ck %}..{% block 
+00000060: 636f 6e74 656e 7420 257d 0a3c 6d61 696e  content %}.<main
+00000070: 2063 6c61 7373 3d22 7668 2d31 3030 2076   class="vh-100 v
+00000080: 772d 3130 3020 642d 666c 6578 2061 6c69  w-100 d-flex ali
+00000090: 676e 2d69 7465 6d73 2d63 656e 7465 7220  gn-items-center 
+000000a0: 6a75 7374 6966 792d 636f 6e74 656e 742d  justify-content-
+000000b0: 6365 6e74 6572 223e 0a20 2020 203c 6469  center">.    <di
+000000c0: 7620 636c 6173 733d 2263 6f6e 7461 696e  v class="contain
+000000d0: 6572 223e 0a20 2020 2020 2020 203c 6469  er">.        <di
+000000e0: 7620 636c 6173 733d 2272 6f77 206a 7573  v class="row jus
+000000f0: 7469 6679 2d63 6f6e 7465 6e74 2d63 656e  tify-content-cen
+00000100: 7465 7222 3e0a 2020 2020 2020 2020 2020  ter">.          
+00000110: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00000120: 6c2d 736d 2d31 3020 636f 6c2d 6d64 2d37  l-sm-10 col-md-7
+00000130: 2063 6f6c 2d6c 672d 3522 3e0a 2020 2020   col-lg-5">.    
+00000140: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000150: 2063 6c61 7373 3d22 6361 7264 2073 6861   class="card sha
+00000160: 646f 7720 616c 6967 6e2d 7365 6c66 2d63  dow align-self-c
+00000170: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+00000180: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000190: 2063 6c61 7373 3d22 6361 7264 2d68 6561   class="card-hea
+000001a0: 6465 7220 702d 3222 3e0a 2020 2020 2020  der p-2">.      
+000001b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001c0: 2020 3c68 3520 636c 6173 733d 2274 6578    <h5 class="tex
+000001d0: 742d 6365 6e74 6572 2074 6578 742d 626c  t-center text-bl
+000001e0: 6163 6b2d 3530 2066 732d 3420 702d 3020  ack-50 fs-4 p-0 
+000001f0: 6d2d 3022 3e7b 7b27 7365 7475 7027 207c  m-0">{{'setup' |
+00000200: 2063 6170 6974 616c 697a 657d 7d3c 2f68   capitalize}}</h
+00000210: 353e 0a20 2020 2020 2020 2020 2020 2020  5>.             
+00000220: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000240: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
+00000250: 7264 2d62 6f64 7922 3e0a 2020 2020 2020  rd-body">.      
+00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000270: 2020 3c66 6f72 6d20 636c 6173 733d 2266    <form class="f
+00000280: 6f72 6d2d 666c 6f61 7469 6e67 2062 672d  orm-floating bg-
+00000290: 6772 6164 6965 6e74 2220 6163 7469 6f6e  gradient" action
+000002a0: 3d22 7b7b 2075 726c 5f66 6f72 2827 7365  ="{{ url_for('se
+000002b0: 7475 702e 696e 6974 7365 7475 7027 2920  tup.initsetup') 
+000002c0: 7d7d 2220 6d65 7468 6f64 3d22 706f 7374  }}" method="post
+000002d0: 2220 6964 3d22 7365 7475 7046 6f72 6d22  " id="setupForm"
+000002e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000002f0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000300: 2066 6f72 2028 6361 7465 676f 7279 2c20   for (category, 
+00000310: 6d65 7373 6167 6529 2069 6e20 6765 745f  message) in get_
+00000320: 666c 6173 6865 645f 6d65 7373 6167 6573  flashed_messages
+00000330: 2877 6974 685f 6361 7465 676f 7269 6573  (with_categories
+00000340: 3d54 7275 6529 2025 7d0a 2020 2020 2020  =True) %}.      
+00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000360: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 2020 2020 2020 2020 2063 6c61 7373             class
+00000390: 3d22 616c 6572 7420 616c 6572 742d 7b7b  ="alert alert-{{
+000003a0: 6361 7465 676f 7279 7d7d 2061 6c65 7274  category}} alert
+000003b0: 2d64 6973 6d69 7373 6962 6c65 2062 672d  -dismissible bg-
+000003c0: 6772 6164 6965 6e74 2064 2d66 6c65 7820  gradient d-flex 
+000003d0: 6a75 7374 6966 792d 636f 6e74 656e 742d  justify-content-
+000003e0: 6265 7477 6565 6e20 726f 756e 6465 642d  between rounded-
+000003f0: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
+00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000410: 2020 2020 3c73 7472 6f6e 673e 7b7b 6d65      <strong>{{me
+00000420: 7373 6167 657d 7d3c 2f73 7472 6f6e 673e  ssage}}</strong>
+00000430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 203c 6275 7474 6f6e 2074 7970 653d 2262   <button type="b
+00000460: 7574 746f 6e22 2063 6c61 7373 3d22 6274  utton" class="bt
+00000470: 6e20 6274 6e2d 636c 6f73 6522 2064 6174  n btn-close" dat
+00000480: 612d 6273 2d64 6973 6d69 7373 3d22 616c  a-bs-dismiss="al
+00000490: 6572 7422 3e3c 2f62 7574 746f 6e3e 0a20  ert"></button>. 
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+000004c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000004d0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000004e0: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 2020 203c 6469 7620 6964 3d22         <div id="
+00000510: 7365 7475 7057 697a 6172 6422 3e0a 2020  setupWizard">.  
+00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000530: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000540: 6976 2063 6c61 7373 3d22 7365 7475 702d  iv class="setup-
+00000550: 7374 6570 223e 0a20 2020 2020 2020 2020  step">.         
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 2020 2020 2020 2020 2020 203c 6836 2063             <h6 c
+00000580: 6c61 7373 3d22 7465 7874 2d63 656e 7465  lass="text-cente
+00000590: 7220 7465 7874 2d64 616e 6765 7220 6673  r text-danger fs
+000005a0: 2d36 223e 4461 7461 6261 7365 2053 6574  -6">Database Set
+000005b0: 7570 3c2f 6836 3e0a 2020 2020 2020 2020  up</h6>.        
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000005e0: 2063 6c61 7373 3d22 666f 726d 2d67 726f   class="form-gro
+000005f0: 7570 206d 622d 3122 3e0a 2020 2020 2020  up mb-1">.      
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000620: 2020 3c6c 6162 656c 2063 6c61 7373 3d22    <label class="
+00000630: 736d 616c 6c22 2066 6f72 3d22 656d 6169  small" for="emai
+00000640: 6c22 3e44 424d 533c 2f6c 6162 656c 3e0a  l">DBMS</label>.
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000670: 2020 2020 2020 2020 3c73 656c 6563 7420          <select 
+00000680: 6e61 6d65 3d22 4442 4d53 2220 6964 3d22  name="DBMS" id="
+00000690: 2220 636c 6173 733d 2266 6f72 6d2d 7365  " class="form-se
+000006a0: 6c65 6374 2066 6f72 6d2d 7365 6c65 6374  lect form-select
+000006b0: 2d73 6d20 7465 7874 2d62 6c61 636b 2d35  -sm text-black-5
+000006c0: 3022 2072 6571 7569 7265 6420 6f6e 6368  0" required onch
+000006d0: 616e 6765 3d22 7365 6c65 6374 444d 456e  ange="selectDMEn
+000006e0: 6769 6e65 2874 6869 732e 7661 6c75 6529  gine(this.value)
+000006f0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000720: 6f70 7469 6f6e 3e3c 2f6f 7074 696f 6e3e  option></option>
+00000730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 2020 2020 2020 2020 2020 2020 203c 6f70               <op
+00000760: 7469 6f6e 2076 616c 7565 3d22 6d6f 6e67  tion value="mong
+00000770: 6f64 6222 3e4d 6f6e 676f 4442 3c2f 6f70  odb">MongoDB</op
+00000780: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 3c6f 7074 696f 6e20 7661 6c75 653d    <option value=
+000007c0: 226d 7973 716c 223e 4d79 7371 6c3c 2f6f  "mysql">Mysql</o
+000007d0: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 203c 6f70 7469 6f6e 2076 616c 7565     <option value
+00000810: 3d22 7371 6c69 7465 223e 5371 6c69 7465  ="sqlite">Sqlite
+00000820: 733c 2f6f 7074 696f 6e3e 0a20 2020 2020  s</option>.     
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 203c 2f73 656c 6563 743e 0a20 2020     </select>.   
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000008b0: 2063 6c61 7373 3d22 666f 726d 2d67 726f   class="form-gro
+000008c0: 7570 206d 622d 3122 3e0a 2020 2020 2020  up mb-1">.      
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 3c6c 6162 656c 2063 6c61 7373 3d22    <label class="
+00000900: 736d 616c 6c22 3e48 6f73 743c 2f6c 6162  small">Host</lab
+00000910: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
+00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000930: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+00000940: 7574 2074 7970 653d 2274 6578 7422 2076  ut type="text" v
+00000950: 616c 7565 3d22 3132 372e 302e 302e 3122  alue="127.0.0.1"
+00000960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+00000990: 7373 3d22 666f 726d 2d63 6f6e 7472 6f6c  ss="form-control
+000009a0: 2066 6f72 6d2d 636f 6e74 726f 6c2d 736d   form-control-sm
+000009b0: 2074 6578 742d 626c 6163 6b2d 3530 2220   text-black-50" 
+000009c0: 6e61 6d65 3d22 4441 5441 4241 5345 5f48  name="DATABASE_H
+000009d0: 4f53 5422 2072 6571 7569 7265 643e 0a20  OST" required>. 
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000a30: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+00000a40: 726f 7570 206d 622d 3122 3e0a 2020 2020  roup mb-1">.    
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2020 2020 3c6c 6162 656c 2063 6c61 7373      <label class
+00000a80: 3d22 736d 616c 6c22 3e50 6f72 743c 2f6c  ="small">Port</l
+00000a90: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00000ac0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
+00000ad0: 2063 6c61 7373 3d22 666f 726d 2d63 6f6e   class="form-con
+00000ae0: 7472 6f6c 2066 6f72 6d2d 636f 6e74 726f  trol form-contro
+00000af0: 6c2d 736d 2074 6578 742d 626c 6163 6b2d  l-sm text-black-
+00000b00: 3530 220a 2020 2020 2020 2020 2020 2020  50".            
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 6e61 6d65 3d22 4441 5441 4241 5345 5f50  name="DATABASE_P
+00000b40: 4f52 5422 2072 6571 7569 7265 643e 0a20  ORT" required>. 
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000ba0: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+00000bb0: 726f 7570 206d 622d 3122 3e0a 2020 2020  roup mb-1">.    
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 2020 3c6c 6162 656c 2063 6c61 7373      <label class
+00000bf0: 3d22 736d 616c 6c22 3e44 6174 6162 6173  ="small">Databas
+00000c00: 6520 4e61 6d65 3c2f 6c61 6265 6c3e 0a20  e Name</label>. 
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c30: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00000c40: 7065 3d22 7465 7874 2220 6e61 6d65 3d22  pe="text" name="
+00000c50: 4441 5441 4241 5345 5f4e 414d 4522 2076  DATABASE_NAME" v
+00000c60: 616c 7565 3d22 7275 6e69 7422 0a20 2020  alue="runit".   
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
+00000ca0: 666f 726d 2d63 6f6e 7472 6f6c 2066 6f72  form-control for
+00000cb0: 6d2d 636f 6e74 726f 6c2d 736d 2074 6578  m-control-sm tex
+00000cc0: 742d 626c 6163 6b2d 3530 223e 0a20 2020  t-black-50">.   
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000d20: 2063 6c61 7373 3d22 666f 726d 2d67 726f   class="form-gro
+00000d30: 7570 206d 622d 3122 3e0a 2020 2020 2020  up mb-1">.      
 00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000d60: 7373 3d22 6274 6e2d 6772 6f75 7022 3e0a  ss="btn-group">.
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00000d90: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
-00000da0: 2220 636c 6173 733d 2262 746e 2062 746e  " class="btn btn
-00000db0: 2d73 6d20 6274 6e2d 7072 696d 6172 7920  -sm btn-primary 
-00000dc0: 6267 2d67 7261 6469 656e 7420 626f 7264  bg-gradient bord
-00000dd0: 6572 2d30 2220 6f6e 636c 6963 6b3d 2275  er-0" onclick="u
-00000de0: 7064 6174 6545 6e76 7328 2922 3e0a 2020  pdateEnvs()">.  
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000e10: 2063 6c61 7373 3d22 6661 7320 6661 2d73   class="fas fa-s
-00000e20: 6176 6520 6661 2d66 7722 3e3c 2f69 3e20  ave fa-fw"></i> 
-00000e30: 5570 6461 7465 0a20 2020 2020 2020 2020  Update.         
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 203c 2f62 7574 746f 6e3e 0a20 2020     </button>.   
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2020 3c6c 6162 656c 2063 6c61 7373 3d22    <label class="
+00000d70: 736d 616c 6c22 3e44 6174 6162 6173 6520  small">Database 
+00000d80: 5573 6572 3c2f 6c61 6265 6c3e 0a20 2020  User</label>.   
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00000dc0: 3d22 7465 7874 2220 636c 6173 733d 2266  ="text" class="f
+00000dd0: 6f72 6d2d 636f 6e74 726f 6c20 666f 726d  orm-control form
+00000de0: 2d63 6f6e 7472 6f6c 2d73 6d20 7465 7874  -control-sm text
+00000df0: 2d62 6c61 636b 2d35 3022 0a20 2020 2020  -black-50".     
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 206e 616d 653d 2244 4154         name="DAT
+00000e30: 4142 4153 455f 5553 4552 4e41 4d45 223e  ABASE_USERNAME">
+00000e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000ea0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000eb0: 636c 6173 733d 2263 6172 642d 626f 6479  class="card-body
-00000ec0: 2070 622d 3022 3e0a 0909 0909 0909 3c64   pb-0">.......<d
-00000ed0: 6976 2063 6c61 7373 3d27 772d 3130 3027  iv class='w-100'
-00000ee0: 2073 7479 6c65 3d27 7772 6170 3a20 7772   style='wrap: wr
-00000ef0: 6170 273e 0a09 0909 0909 0909 3c63 6f64  ap'>........<cod
-00000f00: 653e 0a09 0909 0909 0909 097b 7b64 6174  e>.........{{dat
-00000f10: 6162 6173 657d 7d0a 0909 0909 0909 093c  abase}}........<
-00000f20: 2f63 6f64 653e 0a09 0909 0909 093c 2f64  /code>.......</d
-00000f30: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000f40: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000f50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000f60: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000f70: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00000f80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000f90: 2274 6162 2d70 616e 6520 6661 6465 2062  "tab-pane fade b
-00000fa0: 672d 6c69 6768 7422 2069 643d 226e 6176  g-light" id="nav
-00000fb0: 2d63 6f6c 6c65 6374 696f 6e73 2220 726f  -collections" ro
-00000fc0: 6c65 3d22 7461 6270 616e 656c 2220 6172  le="tabpanel" ar
-00000fd0: 6961 2d6c 6162 656c 6c65 6462 793d 226e  ia-labelledby="n
-00000fe0: 6176 2d63 6f6c 6c65 6374 696f 6e73 2d74  av-collections-t
-00000ff0: 6162 2220 7461 6269 6e64 6578 3d22 3022  ab" tabindex="0"
-00001000: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001010: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
-00001020: 7264 2072 6f75 6e64 6564 2d30 2062 6f72  rd rounded-0 bor
-00001030: 6465 722d 3020 7368 6164 6f77 2d73 6d20  der-0 shadow-sm 
-00001040: 6d79 2d32 2062 672d 6c69 6768 7422 3e0a  my-2 bg-light">.
+00000e90: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
+00000ea0: 2d67 726f 7570 206d 622d 3322 3e0a 2020  -group mb-3">.  
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2020 2020 3c6c 6162 656c 2063 6c61        <label cla
+00000ee0: 7373 3d22 736d 616c 6c22 3e44 6174 6162  ss="small">Datab
+00000ef0: 6173 6520 5061 7373 776f 7264 3c2f 6c61  ase Password</la
+00000f00: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 2020 2020 2020 203c 696e               <in
+00000f30: 7075 7420 7479 7065 3d22 7061 7373 776f  put type="passwo
+00000f40: 7264 2220 636c 6173 733d 2266 6f72 6d2d  rd" class="form-
+00000f50: 636f 6e74 726f 6c20 666f 726d 2d63 6f6e  control form-con
+00000f60: 7472 6f6c 2d73 6d20 7465 7874 2d62 6c61  trol-sm text-bla
+00000f70: 636b 2d35 3022 0a20 2020 2020 2020 2020  ck-50".         
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 2020 206e 616d 653d 2244 4154 4142 4153     name="DATABAS
+00000fb0: 455f 5041 5353 574f 5244 223e 0a20 2020  E_PASSWORD">.   
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001000: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001030: 6469 7620 636c 6173 733d 2273 6574 7570  div class="setup
+00001040: 2d73 7465 7022 3e0a 2020 2020 2020 2020  -step">.        
 00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001070: 6361 7264 2d62 6f64 7920 7062 2d30 223e  card-body pb-0">
-00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001090: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000010a0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00001060: 2020 2020 2020 2020 2020 2020 3c68 3620              <h6 
+00001070: 636c 6173 733d 2274 6578 742d 6365 6e74  class="text-cent
+00001080: 6572 2074 6578 742d 6461 6e67 6572 2066  er text-danger f
+00001090: 732d 3622 3e52 756e 7469 6d65 2053 6574  s-6">Runtime Set
+000010a0: 7570 3c2f 6836 3e0a 2020 2020 2020 2020  up</h6>.        
 000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000010d0: 733d 2263 6f6c 2d6d 642d 3620 642d 666c  s="col-md-6 d-fl
-000010e0: 6578 2066 6c65 782d 636f 6c75 6d6e 223e  ex flex-column">
-000010f0: 0a20 2020 200a 2020 2020 2020 2020 2020  .    .          
+000010c0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000010d0: 2063 6c61 7373 3d22 666f 726d 2d67 726f   class="form-gro
+000010e0: 7570 206d 622d 3322 3e0a 2020 2020 2020  up mb-3">.      
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001140: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00001150: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001160: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001170: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00001180: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00001190: 6173 733d 2274 6162 2d70 616e 6520 6661  ass="tab-pane fa
-000011a0: 6465 2220 6964 3d22 6e61 762d 7365 7474  de" id="nav-sett
-000011b0: 696e 6773 2220 726f 6c65 3d22 7461 6270  ings" role="tabp
-000011c0: 616e 656c 2220 6172 6961 2d6c 6162 656c  anel" aria-label
-000011d0: 6c65 6462 793d 226e 6176 2d73 6574 7469  ledby="nav-setti
-000011e0: 6e67 732d 7461 6222 2074 6162 696e 6465  ngs-tab" tabinde
-000011f0: 783d 2230 223e 0a20 2020 2020 2020 2020  x="0">.         
-00001200: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001210: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
-00001220: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00001230: 7620 636c 6173 733d 2263 6f6c 2d6d 642d  v class="col-md-
-00001240: 3622 3e0a 2020 2020 2020 2020 2020 2020  6">.            
-00001250: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00001260: 2063 6c61 7373 3d22 6361 7264 2072 6f75   class="card rou
-00001270: 6e64 6564 2d30 2062 6f72 6465 722d 3020  nded-0 border-0 
-00001280: 7368 6164 6f77 2d73 6d20 6d79 2d32 223e  shadow-sm my-2">
+00001110: 2020 3c6c 6162 656c 2063 6c61 7373 3d22    <label class="
+00001120: 736d 616c 6c20 666f 6e74 2d77 6569 6768  small font-weigh
+00001130: 742d 626f 6c64 2066 6f6e 742d 726f 626f  t-bold font-robo
+00001140: 746f 223e 5079 7468 6f6e 2052 756e 7469  to">Python Runti
+00001150: 6d65 3c2f 6c61 6265 6c3e 0a20 2020 2020  me</label>.     
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
+00001190: 7465 7874 2220 636c 6173 733d 2266 6f72  text" class="for
+000011a0: 6d2d 636f 6e74 726f 6c20 666f 726d 2d63  m-control form-c
+000011b0: 6f6e 7472 6f6c 2d73 6d20 7465 7874 2d62  ontrol-sm text-b
+000011c0: 6c61 636b 2d35 3022 0a20 2020 2020 2020  lack-50".       
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2076 616c 7565 3d22 7079 7468       value="pyth
+00001200: 6f6e 2220 6e61 6d65 3d22 5255 4e54 494d  on" name="RUNTIM
+00001210: 455f 5059 5448 4f4e 2220 7265 7175 6972  E_PYTHON" requir
+00001220: 6564 3e0a 2020 2020 2020 2020 2020 2020  ed>.            
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001270: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
+00001280: 6f72 6d2d 6772 6f75 7020 6d62 2d33 223e  orm-group mb-3">
 00001290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000012b0: 7620 636c 6173 733d 2263 6172 642d 6865  v class="card-he
-000012c0: 6164 6572 2070 2d30 2070 2d32 2064 2d66  ader p-0 p-2 d-f
-000012d0: 6c65 7820 6a75 7374 6966 792d 636f 6e74  lex justify-cont
-000012e0: 656e 742d 6265 7477 6565 6e20 616c 696e  ent-between alin
-000012f0: 672d 6974 656d 732d 6365 6e74 6572 223e  g-items-center">
-00001300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
+000012c0: 636c 6173 733d 2273 6d61 6c6c 2066 6f6e  class="small fon
+000012d0: 742d 7765 6967 6874 2d62 6f6c 6420 666f  t-weight-bold fo
+000012e0: 6e74 2d72 6f62 6f74 6f22 3e50 4850 2052  nt-roboto">PHP R
+000012f0: 756e 7469 6d65 3c2f 6c61 6265 6c3e 0a20  untime</label>. 
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 203c 6469 7620 636c 6173 733d 2262 746e   <div class="btn
-00001330: 2d67 726f 7570 223e 0a20 2020 2020 2020  -group">.       
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
-00001360: 7474 6f6e 2074 7970 653d 2262 7574 746f  tton type="butto
-00001370: 6e22 2063 6c61 7373 3d22 6274 6e20 6274  n" class="btn bt
-00001380: 6e2d 736d 2062 746e 2d64 6172 6b22 206f  n-sm btn-dark" o
-00001390: 6e63 6c69 636b 3d22 6372 6561 7465 456e  nclick="createEn
-000013a0: 7628 2922 3e0a 2020 2020 2020 2020 2020  v()">.          
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-000013d0: 2063 6c61 7373 3d22 6661 7320 6661 2d70   class="fas fa-p
-000013e0: 6c75 7322 3e3c 2f69 3e0a 2020 2020 2020  lus"></i>.      
+00001320: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00001330: 7065 3d22 7465 7874 2220 636c 6173 733d  pe="text" class=
+00001340: 2266 6f72 6d2d 636f 6e74 726f 6c20 666f  "form-control fo
+00001350: 726d 2d63 6f6e 7472 6f6c 2d73 6d20 7465  rm-control-sm te
+00001360: 7874 2d62 6c61 636b 2d35 3022 0a20 2020  xt-black-50".   
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+000013a0: 7068 7022 206e 616d 653d 2252 554e 5449  php" name="RUNTI
+000013b0: 4d45 5f50 4850 2220 7265 7175 6972 6564  ME_PHP" required
+000013c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
 000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001410: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
-00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001430: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00001440: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
-00001450: 2220 636c 6173 733d 2262 746e 2062 746e  " class="btn btn
-00001460: 2d73 6d20 6274 6e2d 7072 696d 6172 7920  -sm btn-primary 
-00001470: 626f 7264 6572 2d30 2220 6f6e 636c 6963  border-0" onclic
-00001480: 6b3d 2275 7064 6174 6545 6e76 7328 2922  k="updateEnvs()"
-00001490: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2020 2020 2020 2020 2020 3c69 2063 6c61            <i cla
-000014c0: 7373 3d22 6661 7320 6661 2d73 6176 6520  ss="fas fa-save 
-000014d0: 6661 2d66 7722 3e3c 2f69 3e20 5361 7665  fa-fw"></i> Save
-000014e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 203c 2f62 7574 746f 6e3e 0a20       </button>. 
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001530: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00001580: 2263 6172 642d 626f 6479 2070 622d 3022  "card-body pb-0"
-00001590: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000015a0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-000015b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000015c0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-000015d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000015e0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000015f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 203c 6469 7620 636c 6173 733d 2266 6f72   <div class="for
+00001420: 6d2d 6772 6f75 7020 6d62 2d33 223e 0a20  m-group mb-3">. 
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 2020 203c 6c61 6265 6c20 636c         <label cl
+00001460: 6173 733d 2273 6d61 6c6c 2066 6f6e 742d  ass="small font-
+00001470: 7765 6967 6874 2d62 6f6c 6420 666f 6e74  weight-bold font
+00001480: 2d72 6f62 6f74 6f22 3e4a 6176 6173 6372  -roboto">Javascr
+00001490: 6970 7420 5275 6e74 696d 653c 2f6c 6162  ipt Runtime</lab
+000014a0: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+000014d0: 7574 2074 7970 653d 2274 6578 7422 2063  ut type="text" c
+000014e0: 6c61 7373 3d22 666f 726d 2d63 6f6e 7472  lass="form-contr
+000014f0: 6f6c 2066 6f72 6d2d 636f 6e74 726f 6c2d  ol form-control-
+00001500: 736d 2074 6578 742d 626c 6163 6b2d 3530  sm text-black-50
+00001510: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00001540: 6c75 653d 226e 6f64 6522 206e 616d 653d  lue="node" name=
+00001550: 2252 554e 5449 4d45 5f4a 4156 4153 4352  "RUNTIME_JAVASCR
+00001560: 4950 5422 2072 6571 7569 7265 643e 0a20  IPT" required>. 
+00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000015c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 203c 6469 7620 636c 6173 733d 2273 6574   <div class="set
+000015f0: 7570 2d73 7465 7022 3e0a 2020 2020 2020  up-step">.      
 00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001620: 636f 6c2d 6d64 2d36 223e 3c2f 6469 763e  col-md-6"></div>
-00001630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001640: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001650: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00001660: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001670: 733d 2274 6162 2d70 616e 6520 6661 6465  s="tab-pane fade
-00001680: 2220 6964 3d22 6e61 762d 636f 6e73 6f6c  " id="nav-consol
-00001690: 6522 2072 6f6c 653d 2274 6162 7061 6e65  e" role="tabpane
-000016a0: 6c22 2061 7269 612d 6c61 6265 6c6c 6564  l" aria-labelled
-000016b0: 6279 3d22 6e61 762d 636f 6e73 6f6c 652d  by="nav-console-
-000016c0: 7461 6222 2074 6162 696e 6465 783d 2230  tab" tabindex="0
-000016d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000016e0: 2020 2054 6572 6d69 6e61 6c20 436f 6e73     Terminal Cons
-000016f0: 6f6c 650a 2020 2020 2020 2020 2020 2020  ole.            
-00001700: 3c2f 6469 763e 0a09 0909 3c64 6976 2063  </div>....<div c
-00001710: 6c61 7373 3d22 7461 622d 7061 6e65 2066  lass="tab-pane f
-00001720: 6164 6522 2069 643d 226e 6176 2d69 6e69  ade" id="nav-ini
-00001730: 7469 616c 697a 6174 696f 6e22 2072 6f6c  tialization" rol
-00001740: 653d 2274 6162 7061 6e65 6c22 2061 7269  e="tabpanel" ari
-00001750: 612d 6c61 6265 6c6c 6564 6279 3d22 6e61  a-labelledby="na
-00001760: 762d 696e 6974 6961 6c69 7a61 7469 6f6e  v-initialization
-00001770: 2d74 6162 2220 7461 6269 6e64 6578 3d22  -tab" tabindex="
-00001780: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
-00001790: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000017a0: 6361 7264 2072 6f75 6e64 6564 2d30 2062  card rounded-0 b
-000017b0: 6f72 6465 722d 3020 7368 6164 6f77 2d73  order-0 shadow-s
-000017c0: 6d20 6d79 2d32 223e 0a20 2020 2020 2020  m my-2">.       
-000017d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000017e0: 7620 636c 6173 733d 2263 6172 642d 6865  v class="card-he
-000017f0: 6164 6572 2070 2d30 2070 2d32 2064 2d66  ader p-0 p-2 d-f
-00001800: 6c65 7820 6a75 7374 6966 792d 636f 6e74  lex justify-cont
-00001810: 656e 742d 6265 7477 6565 6e20 616c 696e  ent-between alin
-00001820: 672d 6974 656d 732d 6365 6e74 6572 223e  g-items-center">
-00001830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001840: 2020 2020 2020 2020 203c 736d 616c 6c20           <small 
-00001850: 636c 6173 733d 2266 772d 626f 6c64 223e  class="fw-bold">
-00001860: 3c2f 736d 616c 6c3e 0a20 2020 2020 2020  </small>.       
-00001870: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00001880: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00001890: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000018a0: 7373 3d22 6361 7264 2d62 6f64 7920 7062  ss="card-body pb
-000018b0: 2d30 223e 0a09 0909 0909 093c 6469 7620  -0">.......<div 
-000018c0: 636c 6173 733d 2777 2d31 3030 2720 7374  class='w-100' st
-000018d0: 796c 653d 2777 7261 703a 2077 7261 7027  yle='wrap: wrap'
-000018e0: 3e0a 0909 0909 0909 093c 636f 6465 3e0a  >........<code>.
-000018f0: 0909 0909 0909 0909 3c70 7265 2073 7479  ........<pre sty
-00001900: 6c65 3d22 7768 6974 652d 7370 6163 653a  le="white-space:
-00001910: 2070 7265 2d6c 696e 6522 3e0a 0909 0909   pre-line">.....
-00001920: 0909 0909 0966 726f 6d20 7275 6e69 742d  .....from runit-
-00001930: 6461 7461 6261 7365 2069 6d70 6f72 7420  database import 
-00001940: 446f 6375 6d65 6e74 0a09 0909 0909 0909  Document........
-00001950: 0909 446f 6375 6d65 6e74 2e69 6e69 7469  ..Document.initi
-00001960: 616c 697a 6528 0a09 0909 0909 0909 0909  alize(..........
-00001970: 0927 7b7b 7265 7175 6573 742e 726f 6f74  .'{{request.root
-00001980: 5f75 726c 7d7d 6170 6927 2c0a 0909 0909  _url}}api',.....
-00001990: 0909 0909 0909 277b 7b73 6573 7369 6f6e  ......'{{session
-000019a0: 5b22 6163 6365 7373 5f74 6f6b 656e 225d  ["access_token"]
-000019b0: 7d7d 272c 0a09 0909 0909 0909 0909 0927  }}',...........'
-000019c0: 7b7b 6461 7461 6261 7365 2e70 726f 6a65  {{database.proje
-000019d0: 6374 5f69 647d 7d27 0a09 0909 0909 0909  ct_id}}'........
-000019e0: 0909 290a 0909 0909 0909 0909 3c2f 7072  ..).........</pr
-000019f0: 653e 0a09 0909 0909 0909 3c2f 636f 6465  e>........</code
-00001a00: 3e0a 0909 0909 0909 3c2f 6469 763e 0a20  >.......</div>. 
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001a30: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00001a40: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-00001a50: 6976 3e0a 2020 2020 2020 2020 3c2f 6469  iv>.        </di
-00001a60: 763e 0a20 2020 203c 2f64 6976 3e0a 3c2f  v>.    </div>.</
-00001a70: 6469 763e 0a7b 2520 656e 6462 6c6f 636b  div>.{% endblock
-00001a80: 2025 7d0a 0a7b 2520 626c 6f63 6b20 7363   %}..{% block sc
-00001a90: 7269 7074 7320 257d 200a 7b7b 7375 7065  ripts %} .{{supe
-00001aa0: 7228 297d 7d0a 3c73 6372 6970 7420 7372  r()}}.<script sr
-00001ab0: 633d 227b 7b75 726c 5f66 6f72 2827 7374  c="{{url_for('st
-00001ac0: 6174 6963 272c 2066 696c 656e 616d 653d  atic', filename=
-00001ad0: 276a 732f 6461 7461 6261 7365 732e 6a73  'js/databases.js
-00001ae0: 2729 7d7d 223e 3c2f 7363 7269 7074 3e0a  ')}}"></script>.
-00001af0: 7b25 2065 6e64 626c 6f63 6b20 257d       {% endblock %}
+00001610: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00001620: 3620 636c 6173 733d 2274 6578 742d 6365  6 class="text-ce
+00001630: 6e74 6572 2074 6578 742d 6461 6e67 6572  nter text-danger
+00001640: 2066 732d 3622 3e41 646d 696e 6973 7472   fs-6">Administr
+00001650: 6174 6f72 2053 6574 7570 3c2f 6836 3e0a  ator Setup</h6>.
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001690: 666f 726d 2d67 726f 7570 206d 622d 3322  form-group mb-3"
+000016a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 2020 2020 2020 3c6c 6162 656c            <label
+000016d0: 2063 6c61 7373 3d22 736d 616c 6c20 666f   class="small fo
+000016e0: 6e74 2d77 6569 6768 742d 626f 6c64 2066  nt-weight-bold f
+000016f0: 6f6e 742d 726f 626f 746f 223e 5573 6572  ont-roboto">User
+00001700: 6e61 6d65 3c2f 6c61 6265 6c3e 0a20 2020  name</label>.   
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001730: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+00001740: 3d22 7465 7874 2220 636c 6173 733d 2266  ="text" class="f
+00001750: 6f72 6d2d 636f 6e74 726f 6c20 666f 726d  orm-control form
+00001760: 2d63 6f6e 7472 6f6c 2d73 6d20 7465 7874  -control-sm text
+00001770: 2d62 6c61 636b 2d35 3022 0a20 2020 2020  -black-50".     
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2020 2020 2020 2076 616c 7565 3d22 6164         value="ad
+000017b0: 6d69 6e22 206e 616d 653d 2261 646d 696e  min" name="admin
+000017c0: 7573 6572 6e61 6d65 2220 7265 7175 6972  username" requir
+000017d0: 6564 3e0a 2020 2020 2020 2020 2020 2020  ed>.            
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
+00001830: 6f72 6d2d 6772 6f75 7020 6d62 2d33 223e  orm-group mb-3">
+00001840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
+00001870: 636c 6173 733d 2273 6d61 6c6c 2066 6f6e  class="small fon
+00001880: 742d 7765 6967 6874 2d62 6f6c 6420 666f  t-weight-bold fo
+00001890: 6e74 2d72 6f62 6f74 6f22 3e50 6173 7377  nt-roboto">Passw
+000018a0: 6f72 643c 2f6c 6162 656c 3e0a 2020 2020  ord</label>.    
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+000018e0: 2270 6173 7377 6f72 6422 2063 6c61 7373  "password" class
+000018f0: 3d22 666f 726d 2d63 6f6e 7472 6f6c 2066  ="form-control f
+00001900: 6f72 6d2d 636f 6e74 726f 6c2d 736d 2074  orm-control-sm t
+00001910: 6578 742d 626c 6163 6b2d 3530 220a 2020  ext-black-50".  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00001950: 6164 6d69 6e70 6173 7377 6f72 6422 2072  adminpassword" r
+00001960: 6571 7569 7265 643e 0a20 2020 2020 2020  equired>.       
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00001990: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019f0: 2020 2020 2020 3c2f 666f 726d 3e0a 2020        </form>.  
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00001a20: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001a30: 7620 636c 6173 733d 2263 6172 642d 666f  v class="card-fo
+00001a40: 6f74 6572 2070 2d32 2064 2d66 6c65 7820  oter p-2 d-flex 
+00001a50: 6a75 7374 6966 792d 636f 6e74 656e 742d  justify-content-
+00001a60: 6265 7477 6565 6e22 3e0a 2020 2020 2020  between">.      
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
+00001a90: 6275 7474 6f6e 2220 636c 6173 733d 2262  button" class="b
+00001aa0: 746e 2062 746e 2d6c 6967 6874 2062 672d  tn btn-light bg-
+00001ab0: 6772 6164 6965 6e74 2070 782d 3422 2069  gradient px-4" i
+00001ac0: 643d 2273 6574 7570 4261 636b 4275 7474  d="setupBackButt
+00001ad0: 6f6e 223e 4261 636b 3c2f 6275 7474 6f6e  on">Back</button
+00001ae0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001af0: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
+00001b00: 6e20 7479 7065 3d22 6275 7474 6f6e 2220  n type="button" 
+00001b10: 636c 6173 733d 2262 746e 2062 746e 2d6f  class="btn btn-o
+00001b20: 7574 6c69 6e65 2d70 7269 6d61 7279 2062  utline-primary b
+00001b30: 672d 6772 6164 6965 6e74 2073 6861 646f  g-gradient shado
+00001b40: 772d 736d 2070 782d 3422 0a20 2020 2020  w-sm px-4".     
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2020 2020 2069 643d 2273 6574 7570         id="setup
+00001b70: 4e65 7874 4275 7474 6f6e 223e 4e65 7874  NextButton">Next
+00001b80: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
+00001bb0: 6275 7474 6f6e 2220 636c 6173 733d 2262  button" class="b
+00001bc0: 746e 2062 746e 2d6f 7574 6c69 6e65 2d73  tn btn-outline-s
+00001bd0: 7563 6365 7373 2062 672d 6772 6164 6965  uccess bg-gradie
+00001be0: 6e74 2073 6861 646f 772d 736d 2070 782d  nt shadow-sm px-
+00001bf0: 3420 642d 6e6f 6e65 220a 2020 2020 2020  4 d-none".      
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 6964 3d22 7365 7475 7053        id="setupS
+00001c20: 7562 6d69 7442 7574 746f 6e22 3e53 7562  ubmitButton">Sub
+00001c30: 6d69 743c 2f62 7574 746f 6e3e 0a20 2020  mit</button>.   
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00001c60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001c70: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001c80: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
+00001c90: 0a20 2020 203c 2f64 6976 3e0a 3c2f 6d61  .    </div>.</ma
+00001ca0: 696e 3e0a 7b25 2065 6e64 626c 6f63 6b20  in>.{% endblock 
+00001cb0: 257d 0a7b 2520 626c 6f63 6b20 7363 7269  %}.{% block scri
+00001cc0: 7074 7320 257d 0a7b 7b73 7570 6572 2829  pts %}.{{super()
+00001cd0: 7d7d 0a3c 7363 7269 7074 2073 7263 3d22  }}.<script src="
+00001ce0: 7b7b 7572 6c5f 666f 7228 2773 7461 7469  {{url_for('stati
+00001cf0: 6327 2c20 6669 6c65 6e61 6d65 3d27 6a73  c', filename='js
+00001d00: 2f73 6574 7570 2e6a 7327 297d 7d22 3e3c  /setup.js')}}"><
+00001d10: 2f73 6372 6970 743e 0a7b 2520 656e 6462  /script>.{% endb
+00001d20: 6c6f 636b 2025 7d                        lock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/databases/grid.html` & `runit-server-0.2.4/runit_server/templates/databases/grid.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-<div class="d-flex flex-wrap">
-{% for database in databases %}
-<div class="position-relative m-2 text-black">
-    <a href="{{url_for('database.details', database_id=database.id)}}" class="nav-link d-flex flex-column align-items-center p-2 text-black-50 hover:text-dark">
-        <i class="fas fa-database fa-fw fa-2x"></i>
-        <small>{{ database['name'] }}</small>
-    </a>
-	<nav class="nav-item dropdown position-absolute top-0" style="right: 0">
-        <a class="nav-link" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
-            <i class="fas fa-ellipsis-v"></i>
-        </a>
-        <ul class="dropdown-menu rounded-0 shadow">
-            <li>
-                <a href="{{url_for('database.details', database_id=database.id)}}" class="dropdown-item small py-0">
-                    Details
-                </a>
-            </li>
-            <li><hr class="dropdown-divider"></li>
-            <li>
-				<form method="post" action="{{ url_for('database.delete', database_id=database.id) }}">
-					<button type="submit" class="btn btn-link text-danger small py-0" style="text-decoration: none">Delete</button>
-				</form>
-			</li>
-        </ul>
-    </nav>
-</div>
-{% endfor %}
+<div class="d-flex flex-wrap mt-3">
+{% for database in databases %}
+<div class="position-relative m-2 p-3 border rounded shadow-sm">
+    <a href="{{url_for('database.details', database_id=database.id)}}" class="nav-link d-flex flex-column align-items-center p-2 text-black-50 hover:text-dark">
+        <i class="fas fa-database fa-fw fa-3x mb-2"></i>
+        <span>{{ database['name'] }}</span>
+    </a>
+	<nav class="nav-item dropdown position-absolute" style="right: 13px; top: 8px">
+        <a class="nav-link" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
+            <i class="fas fa-ellipsis-v text-secondary"></i>
+        </a>
+        <ul class="dropdown-menu rounded-0 shadow border-0">
+            <li>
+                <a href="{{url_for('database.details', database_id=database.id)}}" class="dropdown-item small py-0">
+                    Details
+                </a>
+            </li>
+            <li><hr class="dropdown-divider"></li>
+            <li>
+				<form method="post" action="{{ url_for('database.delete', database_id=database.id) }}">
+					<button type="submit" class="btn btn-link text-danger small py-0" style="text-decoration: none">Delete</button>
+				</form>
+			</li>
+        </ul>
+    </nav>
+</div>
+{% endfor %}
 </div>
```

### Comparing `runit-server-0.2.3/runit_server/templates/databases/index.html` & `runit-server-0.2.4/runit_server/templates/projects/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-{% extends "account/layout.html" %}
-
-{% block title %}
-{{super()}} | {{page | capitalize}}
-{% endblock %}
-
-{% block content %}
-{% include 'modals/confirm.html' %}
-{% include 'databases/modal.html' %}
-<div class="container">
-    {% for (category, message) in get_flashed_messages(with_categories=True) %}
-    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
-        <strong>{{message}}</strong>
-        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
-    </div>
-    {% endfor %}
-    {% if databases %}
-
-    <div class="tools d-flex justify-content-end">
-        <div class="btn-group" role="group" aria-label="tool buttons">
-            <a href="{{url_for('database.index')}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark bg-gradient" role="button" title="Grid view">
-                <small><i class="fas fa-th-large fa-fw"></i></small>
-            </a>
-            <a href="{{url_for('database.index')}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark bg-gradient" role="button" title="Table view">
-                <small><i class="fas fa-th-list fa-fw"></i></small>
-            </a>
-            <a href="#confirmModal" role="button" class="btn btn-sm btn-danger bg-gradient" data-bs-toggle="modal">
-                <small><i class="fas fa-trash-alt fa-fw"></i></small>
-            </a>
-            <a href="#databaseModal" role="button" class="btn btn-sm btn-primary bg-gradient" data-bs-toggle="modal">
-               <small>
-                <i class="fas fa-plus fa-fw"></i>
-                New Database
-               </small>
-            </a>
-        </div>
-    </div>
-    {% if view == 'list' %} 
-    {% include 'databases/list.html' %} 
-    {% else %} 
-    {% include 'databases/grid.html' %}
-    {% endif %}
-</div>
-{% endif %}
-{% if not databases %}
-<a href="#databaseModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="databaseModal">
-    <i class="fas fa-database fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
-    <span>New</span>
-	<span>Database</span>
-</a>
-{% endif %}
-{% endblock %}
+{% extends "account/layout.html" %}
+
+{% block title %}
+{{super()}} | {{page | capitalize}}
+{% endblock %}
+
+{% block content %}
+{% include 'modals/confirm.html' %}
+{% include 'projects/modal.html' %}
+<div class="container">
+    {% for (category, message) in get_flashed_messages(with_categories=True) %}
+    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
+        <strong>{{message}}</strong>
+        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
+    </div>
+    {% endfor %}
+    {% if projects %}
+
+    <div class="tools d-flex justify-content-end">
+        <div class="btn-group shadow-sm" role="group" aria-label="tool buttons">
+            <a href="{{url_for('project.index')}}" class="btn btn-{{'' if view != 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Grid view">
+                <small><i class="fas fa-th-large fa-fw"></i></small>
+            </a>
+            <a href="{{url_for('project.index')}}?view=list" class="btn btn-{{'' if view == 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Table view">
+                <small><i class="fas fa-th-list fa-fw"></i></small>
+            </a>
+        </div>
+        <div class="btn-group shadow-sm ms-3" role="group" aria-label="tool buttons">
+            <a href="#confirmModal" role="button" class="btn btn-outline-danger bg-gradient" data-bs-toggle="modal">
+                <small><i class="fas fa-trash-alt fa-fw"></i></small>
+            </a>
+            <a href="#projectModal" role="button" class="btn btn-outline-primary bg-gradient" data-bs-toggle="modal">
+               <small>
+                <i class="fas fa-plus fa-fw"></i>
+                New Project
+               </small>
+            </a>
+        </div>
+    </div>
+    {% if view == 'list' %} 
+    {% include 'projects/list.html' %} 
+    {% else %} 
+    {% include 'projects/grid.html' %}
+    {% endif %}
+</div>
+{% endif %}
+{% if not projects %}
+<a href="#projectModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="projectModal">
+    <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
+    New Project
+</a>
+{% endif %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "account/layout.html" %} {% block title %} {{super()}} | {{page |
 capitalize}} {% endblock %} {% block content %} {% include 'modals/
-confirm.html' %} {% include 'databases/modal.html' %}
+confirm.html' %} {% include 'projects/modal.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
-{% endfor %} {% if databases %}
+{% endfor %} {% if projects %}
 
- New_Database
-{% if view == 'list' %} {% include 'databases/list.html' %} {% else %} {%
-include 'databases/grid.html' %} {% endif %}
-{% endif %} {% if not databases %}
- New_Database
+
+ New_Project
+{% if view == 'list' %} {% include 'projects/list.html' %} {% else %} {%
+include 'projects/grid.html' %} {% endif %}
+{% endif %} {% if not projects %}
+ New_Project
  {% endif %} {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/databases/modal.html` & `runit-server-0.2.4/runit_server/templates/modals/create_database.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-<div class="modal fade" id="databaseModal" tabindex="-1" aria-labelledby="databaseModalLabel" aria-hidden="true">
-    <div class="modal-dialog modal-dialog-centered" role="dialog">
-        <div class="modal-content rounded-0">
-            <form action="{{ url_for('database.create') }}" method="post">
-                <div class="modal-header text-bg-dark rounded-0">
-                    <h5 class="modal-title fw-bolder" id="databaseModalLabel">New Database</h5>
-                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-                </div>
-                <div class="modal-body">
-                    <div class="form-group mb-3">
-                        <input type="text"  name="name" 
-                        class="form-control form-control-sm border-0 border-bottom border-dark rounded-0" 
-                        placeholder="Name of the database" autocomplete="off" required>
-                    </div>
-					<div class="form-group mb-3">
-                        <select name="project_id" class="form-select form-select-sm border-0 border-bottom border-dark rounded-0" required>
-                            <option selected disabled>
-                                <i class="fas fa-code fa-fw"></i> Project
-                            </option>
-                            {% for project in projects %}
-                            <option value="{{project['id'] | lower }}">
-                                {{ project['name'] | capitalize }}
-                            </option>
-                            {% endfor %}
-                        </select>
-                    </div>
-                </div>
-                <div class="modal-footer p-0">
-                    <button type="button" class="btn btn-light rounded-0 m-0" data-bs-dismiss="modal">
-                        <small>Close</small>
-                    </button>
-                    <button type="submit" class="btn btn-dark rounded-0 m-0">
-                        <small>Create Database</small>
-                    </button>
-                </div>
-            </form>
-        </div>
-    </div>
-</div>
+<div class="modal fade" id="databaseModal" tabindex="-1" aria-labelledby="databaseModalLabel" aria-hidden="true">
+    <div class="modal-dialog modal-dialog-centered" role="dialog">
+        <div class="modal-content rounded-0">
+            <form action="{{ url_for('database.create') }}" method="post">
+                <div class="modal-header text-bg-dark rounded-0">
+                    <h5 class="modal-title fw-bolder" id="databaseModalLabel">New Database</h5>
+                    <button type="button" class="btn-close bg-white" data-bs-dismiss="modal" aria-label="Close"></button>
+                </div>
+                <div class="modal-body">
+		    		<div class="form-group">
+						<label class="form-label">Database Name</label>
+						<input type="text" name="name" class="form-control form-control-lg shadow-sm"/>
+					</div>
+					<div class="form-group mt-2">
+						<label class="form-label">Project</label>
+						<select name="project_id" class="form-select form-select-lg shadow-sm">
+							<option selected>Select Project</option>
+							{% for project in projects %}
+							<option value={{project.id}}>{{project.name | title}}</option>
+							{% endfor %}
+						</select>
+					</div>
+                </div>
+                <div class="modal-footer p-0">
+                    <button type="button" class="btn btn-light btn-lg rounded-0 m-0" data-bs-dismiss="modal">
+                        <small>Close</small>
+                    </button>
+                    <button type="submit" class="btn btn-dark btn-lg rounded-0 m-0">
+                        <small>Create Database</small>
+                    </button>
+                </div>
+            </form>
+        </div>
+    </div>
+</div>
```

### Comparing `runit-server-0.2.3/runit_server/templates/functions/index.html` & `runit-server-0.2.4/runit_server/templates/functions/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/layout.html` & `runit-server-0.2.4/runit_server/templates/layout.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-<!DOCTYPE html>
-<html>
-
-<head>
-    <meta charset="utf-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
-
-    <link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800" rel="s
-tylesheet">
-    <link href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900" rel="styles
-heet">
-    <link href="https://fonts.googleapis.com/css?family=Roboto+Condensed:300,400,700" rel="st
-ylesheet">
-    <link href="https://fonts.googleapis.com/css?family=Josefin+Sans:300,300i,400,400i,700,700i" rel="stylesheet">
-
-    <title>{% block title %}Runit{% endblock %}</title>
-    <meta name='viewport'
-        content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
-    <meta name="description" content="">
-    <meta name="keywords" content="">
-    <!-- <link rel="stylesheet" href="/static/css/open-iconic-bootstrap.min.css"> -->
-    <link rel="stylesheet" href="/static/css/animate.css">
-
-    <link href="/static/css/bootstrap.min.css" rel="stylesheet">
-    <link href="/static/css/all.min.css" rel="stylesheet">
-
-    <link rel='icon' href="{{url_for('static', filename='images/terminal.svg')}}">
-
-    <meta name="msapplication-TileColor" content="#ffff00">
-    
-    <meta name="theme-color" content="#ffff00">
-    <style>
-        body {
-            font-size: 14px;
-        }
-    </style>
-</head>
-
-<body class="bg-light bg-gradient">
-    {% block content %}
-    {% endblock %}
-
-    {% block scripts %}
-    <script src="{{url_for('static', filename='js/jquery-3.6.0.min.js')}}"></script>
-    {% endblock %}
-</body>
-</html>
+<!DOCTYPE html>
+<html>
+
+<head>
+    <meta charset="utf-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
+
+    <link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800" rel="s
+tylesheet">
+    <link href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900" rel="styles
+heet">
+    <link href="https://fonts.googleapis.com/css?family=Roboto+Condensed:300,400,700" rel="st
+ylesheet">
+    <link href="https://fonts.googleapis.com/css?family=Josefin+Sans:300,300i,400,400i,700,700i" rel="stylesheet">
+
+    <title>{% block title %}Runit{% endblock %}</title>
+    <meta name='viewport'
+        content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
+    <meta name="description" content="">
+    <meta name="keywords" content="">
+
+    <link href="/static/css/bootstrap.min.css" rel="stylesheet">
+    <link href="/static/css/all.min.css" rel="stylesheet">
+
+    <link rel='icon' href="{{url_for('static', filename='images/terminal.svg')}}">
+
+    <meta name="msapplication-TileColor" content="#ffff00">
+    
+    <meta name="theme-color" content="#ffff00">
+    <style>
+        body {
+            font-size: 14px;
+        }
+    </style>
+</head>
+
+<body class="bg-light bg-gradient">
+    {% block content %}
+    {% endblock %}
+
+    {% block scripts %}
+    {% endblock %}
+</body>
+</html>
```

#### html2text {}

```diff
@@ -6,10 +6,8 @@
 
 
 
 
 
 
 
-
-{% block content %} {% endblock %} {% block scripts %}
- {% endblock %}
+{% block content %} {% endblock %} {% block scripts %} {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/login.html` & `runit-server-0.2.4/runit_server/templates/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/modals/confirm.html` & `runit-server-0.2.4/runit_server/templates/modals/confirm.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/projects/details.html` & `runit-server-0.2.4/runit_server/templates/projects/details.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,194 @@
-{% extends "account/layout.html" %}
-{% block title %} 
-{{super()}} | {{page | capitalize}} | {{project.name}}
-{% endblock %}
-
-{% block pagetitle %}
-<div class="d-flex align-items center">
-    <a href="{{url_for('project.index')}}" class="nav-link p-0 text-black-50 hover:text-dark">
-        <i class="fas fa-arrow-left fa-fw"></i> {{ super() }}</a>
-    / 
-    <span>{{ project.name | upper}}</span>
-</div>
-{% endblock %}
-
-{% block content %}
-{% include 'projects/modal.html' %}
-<div class="container">
-    {% for (category, message) in get_flashed_messages(with_categories=True) %}
-    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
-        <strong>{{message}}</strong>
-        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
-    </div>
-    {% endfor %}
-
-    <div class="tools d-flex justify-content-end">
-        <div class="btn-group" role="group" aria-label="tool buttons">
-            <nav class="nav-item dropdown">
-                <a href="#" class="btn btn-sm btn-dark hover:shadow-sm mb-2" data-bs-toggle="dropdown" role="button" aria-expanded="false" title="Run Functions">
-                    <i class="fas fa-terminal"></i>
-                </a>
-                <ul class="dropdown-menu rounded-0 shadow py-0">
-                    {% for func in funcs %}
-                    <li>
-                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="dropdown-item small border-bottom text-bg-danger bg-gradient" target="_blank">
-                            <i class="fas fa-terminal fa-fw text-dark"></i> {{func.name}}
-                        </a>
-                    </li>
-                    {% endfor %}
-                </ul>
-            </nav>
-            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-secondary hover:shadow-sm mb-2" title="Disable Project">
-                <i class="fas fa-eye-slash"></i>
-            </a>
-            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-sm btn-danger hover:shadow-sm mb-2" title="Delete Project">
-                <i class="fas fa-trash-alt"></i>
-            </a>
-        </div>
-    </div>
-
-    <div class="card rounded-0 border-0">
-        <nav>
-            <div class="nav nav-tabs" id="nav-tab" role="tablist">
-                <button class="nav-link active rounded-0" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
-                    <small>Config</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-functions-tab" data-bs-toggle="tab" data-bs-target="#nav-functions" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
-                    <small>Functions</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-settings-tab" data-bs-toggle="tab" data-bs-target="#nav-settings" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
-                    <small>Settings</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-logs-tab" data-bs-toggle="tab" data-bs-target="#nav-logs" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false" disabled>
-                    <small>Logs</small>
-                </button>
-                <button class="nav-link rounded-0" id="nav-console-tab" data-bs-toggle="tab" data-bs-target="#nav-console" type="button" role="tab" aria-controls="nav-console" aria-selected="false" disabled>
-                    <small>Console</small>
-                </button>
-            </div>
-        </nav>
-        <div class="tab-content" id="nav-tabContent">
-            <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab" tabindex="0">
-                <div class="card rounded-0 border-0 shadow-sm my-2">
-                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
-                        <small class="fw-bold"></small>
-                        <div class="btn-group">
-                            <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
-                                <i class="fas fa-save fa-fw"></i> Update
-                            </button>
-                        </div>
-                    </div>
-                    <div class="card-body pb-0">
-                        <div class="row">
-                        {% for key, value in project.items() %}
-                            <div class="col-md-4">
-                                <div class="form-group mb-2">
-                                    <label for="">
-                                        <small>{{key}}</small>
-                                    </label>
-                                    <input type="text" value="{{value}}" placeholder="" class="form-control form-control-sm bg-gradient text-muted" readonly>
-                                </div>
-                            </div>
-                        {% endfor %}
-                        </div>
-                    </div>
-                </div>
-            </div>
-            <div class="tab-pane fade bg-light" id="nav-functions" role="tabpanel" aria-labelledby="nav-functions-tab" tabindex="0">
-                <div class="card rounded-0 border-0 shadow-sm my-2 bg-light">
-                    <div class="card-body pb-0">
-                        <div class="row">
-                            <div class="col-md-6 d-flex flex-column">
-                                {% for func in funcs %}
-                                    <div class="d-flex justify-content-between align-items-center p-2 bg-white border border-light mb-2 rounded-1">
-                                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="nav-link p-0" target="_blank">
-                                            <h4 class="small text-primary text-uppercase">{{func.name}}</h4>
-                                        </a>
-                                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="nav-link p-0" target="_blank">
-                                            <i class="fas fa-terminal fa-fw text-bg-dark p-1 rounded-1"></i>
-                                        </a>
-                                    </div>
-                                {% endfor %}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-            <div class="tab-pane fade" id="nav-settings" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
-                <div class="row">
-                    <div class="col-md-6">
-                        <div class="card rounded-0 border-0 shadow-sm my-2">
-                            <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
-                                <small class="fw-bold">Environment Variables</small>
-                                <div class="btn-group">
-                                    <button type="button" class="btn btn-sm btn-dark" onclick="createEnv()">
-                                        <i class="fas fa-plus"></i>
-                                    </button>
-                                    <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
-                                        <i class="fas fa-save fa-fw"></i> Save
-                                    </button>
-                                </div>
-                            </div>
-                            <div class="card-body pb-0">
-                                <form action="{{url_for('project.environ', project_id=project._id)}}" method="post" class="env-form">
-                                    {% for key, value in environs.items() %}
-                                    {% set id = 'env'+(loop.index | string) %}
-                                    {% set envKey = 'envKey'+(loop.index | string) %}
-                                        <div class="form-group row align-items-center mb-2" id="{{id}}">
-                                            <div class="col-5">
-                                                <input type="text" value="{{key}}" placeholder="key" class="form-control form-control-sm key-input" data-name="{{envKey}}" required onkeyup="setEnvKey(this)">
-                                            </div>
-                                            <div class="col-1">
-                                                <span>=</span>
-                                            </div>
-                                            <div class="col-5">
-                                                <input type="text" name="{{key}}" value="{{value}}" placeholder="value" id="{{envKey}}" class="form-control form-control-sm" required>
-                                            </div>
-                                            <div class="col-1">
-                                                <a href="javascript: deleteElem('{{id}}')" class="nav-link">
-                                                    <i class="fas fa-trash-alt"></i>
-                                                </a>
-                                            </div>
-                                        </div>
-                                    {% endfor %}
-                                </form>
-                            </div>
-                        </div>
-                    </div>
-                    <div class="col-md-6"></div>
-                </div>
-            </div>
-            <div class="tab-pane fade" id="nav-logs" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">...</div>
-            <div class="tab-pane fade" id="nav-console" role="tabpanel" aria-labelledby="nav-console-tab" tabindex="0">
-                Terminal Console
-            </div>
-        </div>
-    </div>
-</div>
-{% endblock %}
-
-{% block scripts %} 
-{{super()}}
-<script src="{{url_for('static', filename='js/projects.js')}}"></script>
+{% extends "account/layout.html" %}
+{% block title %} 
+{{super()}} | {{page | capitalize}} | {{project.name}}
+{% endblock %}
+
+{% block pagetitle %}
+<div class="d-flex align-items center custom-flex-wrap white-space-nowrap">
+    <a href="{{url_for('project.index')}}" class="nav-link p-0 text-black-50 hover:text-dark">
+        <i class="fas fa-arrow-left fa-fw"></i> 
+        <span class="d-none d-sm-inline">{{ super() }}</span>
+    </a>
+    <span class="d-none d-sm-inline">/</span>
+    <span>{{ project.name | upper}}</span>
+</div>
+{% endblock %}
+
+{% block content %}
+{% include 'projects/modal.html' %}
+{% include 'projects/editor.html' %}
+<div class="container">
+    {% for (category, message) in get_flashed_messages(with_categories=True) %}
+    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
+        <strong>{{message}}</strong>
+        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
+    </div>
+    {% endfor %}
+
+    <div class="tools d-flex justify-content-end">
+        <div class="btn-group shadow-sm" role="group" aria-label="tool buttons">
+            <nav class="nav-item dropdown">
+                <a href="#" class="btn btn-outline-dark mb-2 rounded-0 rounded-start" data-bs-toggle="dropdown" role="button" aria-expanded="false" title="Run Functions">
+                    <i class="fas fa-terminal"></i>
+                </a>
+                <ul class="dropdown-menu rounded-0 shadow border-0">
+                    {% for func in funcs %}
+                    <li>
+                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="dropdown-item small border-bottom" target="_blank">
+                            <i class="fas fa-terminal fa-fw text-dark me-2"></i> {{func.name}}
+                        </a>
+                    </li>
+                    {% endfor %}
+                </ul>
+            </nav>
+            <a href="#editorModal" role="button" role="button" class="btn btn-outline-success hover:shadow-sm mb-2" data-bs-toggle="modal" title="Redeploy project">
+                <i class="fas fa-wrench"></i>
+            </a>
+            <a href="#editorModal" role="button" role="button" class="btn btn-outline-primary hover:shadow-sm mb-2" data-bs-toggle="modal" title="Open in editor">
+                <i class="fas fa-code"></i>
+            </a>
+            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-outline-secondary hover:shadow-sm mb-2" title="Disable Project">
+                <i class="fas fa-eye-slash"></i>
+            </a>
+            <a href="{{ url_for('project.index')}}" role="button" class="btn btn-outline-danger hover:shadow-sm mb-2" title="Delete Project">
+                <i class="fas fa-trash-alt"></i>
+            </a>
+        </div>
+    </div>
+
+    <div class="card rounded-0 border-0">
+        <nav>
+            <div class="nav nav-tabs" id="nav-tab" role="tablist">
+                <button class="nav-link active" id="nav-home-tab" data-bs-toggle="tab" data-bs-target="#nav-home" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
+                    <span>Config</span>
+                </button>
+                <button class="nav-link" id="nav-functions-tab" data-bs-toggle="tab" data-bs-target="#nav-functions" type="button" role="tab" aria-controls="nav-home" aria-selected="true">
+                    <span>Functions</span>
+                </button>
+                <button class="nav-link" id="nav-settings-tab" data-bs-toggle="tab" data-bs-target="#nav-settings" type="button" role="tab" aria-controls="nav-settings" aria-selected="false">
+                    <span>Settings</span>
+                </button>
+                <button class="nav-link" id="nav-logs-tab" data-bs-toggle="tab" data-bs-target="#nav-logs" type="button" role="tab" aria-controls="nav-loggs" aria-selected="false" disabled>
+                    <span>Logs</span>
+                </button>
+                <button class="nav-link" id="nav-console-tab" data-bs-toggle="tab" data-bs-target="#nav-console" type="button" role="tab" aria-controls="nav-console" aria-selected="false" disabled>
+                    <span>Console</span>
+                </button>
+            </div>
+        </nav>
+        <div class="tab-content" id="nav-tabContent">
+            <div class="tab-pane fade show active" id="nav-home" role="tabpanel" aria-labelledby="nav-home-tab" tabindex="0">
+                <div class="card rounded-0 border-0 shadow-sm my-2">
+                    <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
+                        <small class="fw-bold"></small>
+                        <div class="btn-group">
+                            <button type="submit" class="btn btn-primary bg-gradient shadow-sm border-0" onclick="updateEnvs()">
+                                <i class="fas fa-save fa-fw"></i> Update
+                            </button>
+                        </div>
+                    </div>
+                    <div class="card-body pb-0 d-flex gap-3 custom-flex-wrap">
+                        {% for key, value in project.items() %}
+                            <div class="border hover:shadow-sm d-flex flex-column" style="border-radius: 25px;">
+                                <small class="border-bottom p-2 text-bg-secondary"  style="border-top-left-radius: 25px; border-top-right-radius: 25px;">{{key | upper}}</small>
+                                <small class="m-0 p-2 text-center">{{value}}</small>
+                            </div>
+                        {% endfor %}
+                    </div>
+                </div>
+            </div>
+            <div class="tab-pane fade bg-light" id="nav-functions" role="tabpanel" aria-labelledby="nav-functions-tab" tabindex="0">
+                <div class="card rounded-0 border-0 shadow-sm my-2 bg-light">
+                    <div class="card-body pb-0 w-100">
+                        <table class="table table-hover table-striped fs-5">
+                            <thead>
+                                <tr>
+                                    <th>Name</th>
+                                    <th>Link</th>
+                                    <th>Action</th>
+                                </tr>
+                            </thead>
+                            <tbody>
+                                {% for func in funcs %}
+                                <tr>
+                                    <td>
+                                        <h4 class="small text-primary">{{func.name | title}}</h4>
+                                    </td>
+                                    <td>
+                                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="nav-link p-0" target="_blank">
+                                            <small>
+                                                {{url_for('public.run', project_id=project.id, function=func.name) }}
+                                            </small>
+                                        </a>
+                                    </td>
+                                    <td>
+                                        <a href="{{url_for('public.run', project_id=project.id, function=func.name) }}" class="bg-dark nav-link px-2 rounded" style="width: fit-content" target="_blank">
+                                            <i class="fas fa-terminal fa-fw text-bg-dark p-1 rounded-1"></i>
+                                        </a>
+                                    </td>
+                                </tr>
+                                {% endfor %}
+                            </tbody>
+                        </table>
+                    </div>
+                </div>
+            </div>
+            <div class="tab-pane fade" id="nav-settings" role="tabpanel" aria-labelledby="nav-settings-tab" tabindex="0">
+                <div class="row">
+                    <div class="col-md-6">
+                        <div class="card rounded-0 border-0 shadow-sm my-2">
+                            <div class="card-header p-0 p-2 d-flex justify-content-between aling-items-center">
+                                <small class="fw-bold">Environment Variables</small>
+                                <div class="btn-group">
+                                    <button type="button" class="btn btn-sm btn-dark" onclick="createEnv()">
+                                        <i class="fas fa-plus"></i>
+                                    </button>
+                                    <button type="submit" class="btn btn-sm btn-primary border-0" onclick="updateEnvs()">
+                                        <i class="fas fa-save fa-fw"></i> Save
+                                    </button>
+                                </div>
+                            </div>
+                            <div class="card-body pb-0">
+                                <form action="{{url_for('project.environ', project_id=project._id)}}" method="post" class="env-form">
+                                    {% for key, value in environs.items() %}
+                                    {% set id = 'env'+(loop.index | string) %}
+                                    {% set envKey = 'envKey'+(loop.index | string) %}
+                                        <div class="form-group row align-items-center mb-2" id="{{id}}">
+                                            <div class="col-5">
+                                                <input type="text" value="{{key}}" placeholder="key" class="form-control form-control-sm key-input" data-name="{{envKey}}" required onkeyup="setEnvKey(this)">
+                                            </div>
+                                            <div class="col-1">
+                                                <span>=</span>
+                                            </div>
+                                            <div class="col-5">
+                                                <input type="text" name="{{key}}" value="{{value}}" placeholder="value" id="{{envKey}}" class="form-control form-control-sm" required>
+                                            </div>
+                                            <div class="col-1">
+                                                <a href="javascript: deleteElem('{{id}}')" class="nav-link">
+                                                    <i class="fas fa-trash-alt"></i>
+                                                </a>
+                                            </div>
+                                        </div>
+                                    {% endfor %}
+                                </form>
+                            </div>
+                        </div>
+                    </div>
+                    <div class="col-md-6"></div>
+                </div>
+            </div>
+            <div class="tab-pane fade" id="nav-logs" role="tabpanel" aria-labelledby="nav-logs-tab" tabindex="0">...</div>
+            <div class="tab-pane fade" id="nav-console" role="tabpanel" aria-labelledby="nav-console-tab" tabindex="0">
+                Terminal Console
+            </div>
+        </div>
+    </div>
+</div>
+{% endblock %}
+
+{% block scripts %} 
+{{super()}}
+<script src="{{url_for('static', filename='js/ace/ace.js')}}" type="text/javascript" charset="utf-8"></script>
+<script src="{{url_for('static', filename='js/projects.js')}}"></script>
+<script src="{{url_for('static', filename='js/editor.js')}}"></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
 {% extends "account/layout.html" %} {% block title %} {{super()}} | {{page |
 capitalize}} | {{project.name}} {% endblock %} {% block pagetitle %}
  {{_super()_}}
  / {{ project.name | upper}}
-{% endblock %} {% block content %} {% include 'projects/modal.html' %}
+{% endblock %} {% block content %} {% include 'projects/modal.html' %} {%
+include 'projects/editor.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
 {% endfor %}
 
     * {% for func in funcs %}
     *  {{func.name}}
     * {% endfor %}
 
  Config   Functions   Settings   Logs   Console
   Update
 {% for key, value in project.items() %}
- {{key}}  [{{value}}           ]
-{% endfor %}
-{% for func in funcs %}
-***_{{func.name}}_***
-
+{{key | upper}} {{value}}
 {% endfor %}
+Name                          Link                                       Action
+                              {{url_for('public.run',
+*** {{func.name | title}} *** project_id=project.id,_function=func.name)
+                              }}
 Environment Variables
      Save
 {% for key, value in environs.items() %} {% set id = 'env'+(loop.index |
 string) %} {% set envKey = 'envKey'+(loop.index | string) %}
 [{{key}}             ]
 =
 [{{value}}           ]
```

### Comparing `runit-server-0.2.3/runit_server/templates/projects/index.html` & `runit-server-0.2.4/runit_server/templates/databases/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-{% extends "account/layout.html" %}
-
-{% block title %}
-{{super()}} | {{page | capitalize}}
-{% endblock %}
-
-{% block content %}
-{% include 'modals/confirm.html' %}
-{% include 'projects/modal.html' %}
-<div class="container">
-    {% for (category, message) in get_flashed_messages(with_categories=True) %}
-    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
-        <strong>{{message}}</strong>
-        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
-    </div>
-    {% endfor %}
-    {% if projects %}
-
-    <div class="tools d-flex justify-content-end">
-        <div class="btn-group" role="group" aria-label="tool buttons">
-            <a href="{{url_for('project.index')}}" class="btn btn-sm btn-{{'' if view != 'list' else 'outline-'}}dark" role="button" title="Grid view">
-                <small><i class="fas fa-th-large fa-fw"></i></small>
-            </a>
-            <a href="{{url_for('project.index')}}?view=list" class="btn btn-sm btn-{{'' if view == 'list' else 'outline-'}}dark" role="button" title="Table view">
-                <small><i class="fas fa-th-list fa-fw"></i></small>
-            </a>
-            <a href="#confirmModal" role="button" class="btn btn-sm btn-danger" data-bs-toggle="modal">
-                <small><i class="fas fa-trash-alt fa-fw"></i></small>
-            </a>
-            <a href="#projectModal" role="button" class="btn btn-sm btn-primary" data-bs-toggle="modal">
-               <small>
-                <i class="fas fa-plus fa-fw"></i>
-                New Project
-               </small>
-            </a>
-        </div>
-    </div>
-    {% if view == 'list' %} 
-    {% include 'projects/list.html' %} 
-    {% else %} 
-    {% include 'projects/grid.html' %}
-    {% endif %}
-</div>
-{% endif %}
-{% if not projects %}
-<a href="#projectModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="projectModal">
-    <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
-    New Project
-</a>
-{% endif %}
-{% endblock %}
+{% extends "account/layout.html" %}
+
+{% block title %}
+{{super()}} | {{page | capitalize}}
+{% endblock %}
+
+{% block content %}
+{% include 'modals/confirm.html' %}
+{% include 'modals/create_database.html' %}
+<div class="container">
+    {% for (category, message) in get_flashed_messages(with_categories=True) %}
+    <div class="alert alert-{{category}} alert-dismissible bg-gradient d-flex justify-content-between rounded-0">
+        <strong>{{message}}</strong>
+        <button type="button" class="btn btn-close" data-bs-dismiss="alert"></button>
+    </div>
+    {% endfor %}
+    {% if databases %}
+
+    <div class="tools d-flex justify-content-end">
+        <div class="btn-group shadow-sm" role="group" aria-label="tool buttons">
+            <a href="{{url_for('database.index')}}" class="btn btn-{{'' if view != 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Grid view">
+                <small><i class="fas fa-th-large fa-fw"></i></small>
+            </a>
+            <a href="{{url_for('database.index')}}?view=list" class="btn btn-{{'' if view == 'list' else 'outline-'}}secondary bg-gradient" role="button" title="Table view">
+                <small><i class="fas fa-th-list fa-fw"></i></small>
+            </a>
+        </div>
+        <div class="btn-group shadow-sm ms-3" role="group" aria-label="tool buttons">
+            <a href="#confirmModal" role="button" class="btn btn-outline-danger bg-gradient" data-bs-toggle="modal">
+                <small><i class="fas fa-trash-alt fa-fw"></i></small>
+            </a>
+            <a href="#databaseModal" role="button" class="btn btn-outline-primary bg-gradient" data-bs-toggle="modal">
+               <small>
+                <i class="fas fa-plus fa-fw"></i>
+                New Database
+               </small>
+            </a>
+        </div>
+    </div>
+    {% if view == 'list' %} 
+    {% include 'databases/list.html' %} 
+    {% else %} 
+    {% include 'databases/grid.html' %}
+    {% endif %}
+</div>
+{% endif %}
+{% if not databases %}
+<a href="#databaseModal" class="nav-link d-flex flex-column text-center position-absolute" style="left: 50%; top: 25%; transform: translate(-50%, 50%);" data-bs-toggle="modal" role="button" aria-controls="databaseModal">
+    <i class="fas fa-database fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
+    <span>New</span>
+	<span>Database</span>
+</a>
+{% endif %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "account/layout.html" %} {% block title %} {{super()}} | {{page |
 capitalize}} {% endblock %} {% block content %} {% include 'modals/
-confirm.html' %} {% include 'projects/modal.html' %}
+confirm.html' %} {% include 'modals/create_database.html' %}
 {% for (category, message) in get_flashed_messages(with_categories=True) %}
 {{message}}
-{% endfor %} {% if projects %}
+{% endfor %} {% if databases %}
 
- New_Project
-{% if view == 'list' %} {% include 'projects/list.html' %} {% else %} {%
-include 'projects/grid.html' %} {% endif %}
-{% endif %} {% if not projects %}
- New_Project
+
+ New_Database
+{% if view == 'list' %} {% include 'databases/list.html' %} {% else %} {%
+include 'databases/grid.html' %} {% endif %}
+{% endif %} {% if not databases %}
+ New_Database
  {% endif %} {% endblock %}
```

### Comparing `runit-server-0.2.3/runit_server/templates/projects/modal.html` & `runit-server-0.2.4/runit_server/templates/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server/templates/register.html` & `runit-server-0.2.4/runit_server/templates/register.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.2.3/runit_server.egg-info/PKG-INFO` & `runit-server-0.2.4/runit_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.2.3
+Version: 0.2.4
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # runit-server-Server ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The runit-server Command Line Interface (CLI) Tools can be used to test, manage, and deploy your runit-server project from the command line.
 - Create new runit-server project
 - Run a local web server for your runit-server project
 - publish code and assets to your runit-server-server domain
```

### Comparing `runit-server-0.2.3/setup.py` & `runit-server-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='runit-server',
     version=VERSION,
     author='Amos Amissah',
     author_email='theonlyamos@gmail.com',
     description='Backend for python-runit',
     long_description=description,
+    long_description_content_type = "text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=['requests','python-dotenv', 'python-runit', 
                       'odbms', 'flask','flask-jwt-extended', 
                       'flask-restful', 'waitress', 'passlib'],
     keywords='python3 runit server backend developer serverless architecture docker',
     project_urls={
```

