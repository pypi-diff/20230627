# Comparing `tmp/abow-0.4.3.tar.gz` & `tmp/abow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abow-0.4.3.tar", last modified: Thu Apr 21 15:08:57 2022, max compression
+gzip compressed data, last modified: Tue Jun 27 20:46:16 2023, max compression
```

## Comparing `abow-0.4.3.tar` & `abow-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,46 @@
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/
--rw-r--r--   0 ben000    (1000) users      (100)    34283 2019-10-31 19:49:55.000000 abow-0.4.3/LICENSE.md
--rw-r--r--   0 ben000    (1000) users      (100)      448 2020-05-07 19:58:01.000000 abow-0.4.3/MANIFEST.in
--rw-r--r--   0 ben000    (1000) users      (100)     6497 2022-04-21 15:08:57.189395 abow-0.4.3/PKG-INFO
--rw-r--r--   0 ben000    (1000) users      (100)     4444 2022-04-21 15:08:52.000000 abow-0.4.3/README.md
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/
--rw-r--r--   0 ben000    (1000) users      (100)      921 2022-04-21 15:05:21.000000 abow-0.4.3/abow/__init__.py
--rw-r--r--   0 ben000    (1000) users      (100)     1182 2022-04-21 15:05:21.000000 abow-0.4.3/abow/alerts.py
--rw-r--r--   0 ben000    (1000) users      (100)     7258 2022-04-21 15:05:21.000000 abow-0.4.3/abow/app.py
--rw-r--r--   0 ben000    (1000) users      (100)     6503 2022-04-21 15:05:21.000000 abow-0.4.3/abow/backend.py
--rw-r--r--   0 ben000    (1000) users      (100)     6119 2022-04-21 15:05:21.000000 abow-0.4.3/abow/config.py
--rw-r--r--   0 ben000    (1000) users      (100)     2024 2022-04-21 15:05:21.000000 abow-0.4.3/abow/l10n.py
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/locale/
--rw-r--r--   0 ben000    (1000) users      (100)     6316 2022-04-21 15:08:52.000000 abow-0.4.3/abow/locale/abow.pot
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.185395 abow-0.4.3/abow/locale/en/
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/locale/en/LC_MESSAGES/
--rw-r--r--   0 ben000    (1000) users      (100)     5779 2022-04-21 15:08:52.000000 abow-0.4.3/abow/locale/en/LC_MESSAGES/abow.mo
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.185395 abow-0.4.3/abow/locale/fr/
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ben000    (1000) users      (100)     6055 2022-04-21 15:08:52.000000 abow-0.4.3/abow/locale/fr/LC_MESSAGES/abow.mo
--rw-r--r--   0 ben000    (1000) users      (100)     7919 2021-05-18 10:00:42.000000 abow-0.4.3/abow/mdx_tables.py
--rw-r--r--   0 ben000    (1000) users      (100)     2646 2020-04-26 19:17:38.000000 abow-0.4.3/abow/mdx_wikilinks.py
--rw-r--r--   0 ben000    (1000) users      (100)     3534 2022-04-21 15:05:21.000000 abow-0.4.3/abow/render.py
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.185395 abow-0.4.3/abow/static/
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/static/css/
--rw-r--r--   0 ben000    (1000) users      (100)     7035 2022-04-21 15:05:21.000000 abow-0.4.3/abow/static/css/abow.css
--rw-r--r--   0 ben000    (1000) users      (100)   163873 2022-04-21 14:57:32.000000 abow-0.4.3/abow/static/css/bootstrap.min.css
--rw-r--r--   0 ben000    (1000) users      (100)     4166 2019-11-23 15:56:51.000000 abow-0.4.3/abow/static/css/highlight.css
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/static/img/
--rw-r--r--   0 ben000    (1000) users      (100)     3516 2019-11-10 16:32:37.000000 abow-0.4.3/abow/static/img/abow.svg
--rw-r--r--   0 ben000    (1000) users      (100)      387 2019-11-10 17:13:47.000000 abow-0.4.3/abow/static/img/abow_16.png
--rw-r--r--   0 ben000    (1000) users      (100)     1334 2019-11-10 17:03:04.000000 abow-0.4.3/abow/static/img/abow_32.png
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/static/js/
--rw-r--r--   0 ben000    (1000) users      (100)     3586 2022-04-21 15:05:21.000000 abow-0.4.3/abow/static/js/abow.js
--rw-r--r--   0 ben000    (1000) users      (100)     3520 2021-05-20 18:54:05.000000 abow-0.4.3/abow/static/js/autosize.min.js
--rw-r--r--   0 ben000    (1000) users      (100)    78129 2022-04-21 14:57:32.000000 abow-0.4.3/abow/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 ben000    (1000) users      (100)     2142 2022-04-21 15:05:21.000000 abow-0.4.3/abow/tags.py
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow/views/
--rw-r--r--   0 ben000    (1000) users      (100)     2601 2022-04-21 15:07:23.000000 abow-0.4.3/abow/views/about.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     5721 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/edit.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     1185 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/error.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     4174 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/index.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     1083 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/index_nav_item.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     1459 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/list_pages.tpl
--rw-r--r--   0 ben000    (1000) users      (100)     1375 2022-04-21 15:05:21.000000 abow-0.4.3/abow/views/view.tpl
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/abow.egg-info/
--rw-r--r--   0 ben000    (1000) users      (100)     6497 2022-04-21 15:08:57.000000 abow-0.4.3/abow.egg-info/PKG-INFO
--rw-r--r--   0 ben000    (1000) users      (100)     1067 2022-04-21 15:08:57.000000 abow-0.4.3/abow.egg-info/SOURCES.txt
--rw-r--r--   0 ben000    (1000) users      (100)        1 2022-04-21 15:08:57.000000 abow-0.4.3/abow.egg-info/dependency_links.txt
--rw-r--r--   0 ben000    (1000) users      (100)      209 2022-04-21 15:08:57.000000 abow-0.4.3/abow.egg-info/requires.txt
--rw-r--r--   0 ben000    (1000) users      (100)        5 2022-04-21 15:08:57.000000 abow-0.4.3/abow.egg-info/top_level.txt
--rw-r--r--   0 ben000    (1000) users      (100)     1674 2022-04-21 15:06:38.000000 abow-0.4.3/changelog.md
--rw-r--r--   0 ben000    (1000) users      (100)     1486 2022-04-21 15:08:52.000000 abow-0.4.3/config.example
--rw-r--r--   0 ben000    (1000) users      (100)      377 2022-04-21 15:08:57.189395 abow-0.4.3/setup.cfg
--rw-r--r--   0 ben000    (1000) users      (100)     2638 2022-04-21 15:08:52.000000 abow-0.4.3/setup.py
-drwxr-xr-x   0 ben000    (1000) users      (100)        0 2022-04-21 15:08:57.189395 abow-0.4.3/tests/
--rw-r--r--   0 ben000    (1000) users      (100)     1259 2021-01-23 14:40:10.000000 abow-0.4.3/tests/conftest.py
--rw-r--r--   0 ben000    (1000) users      (100)      405 2020-05-17 18:30:06.000000 abow-0.4.3/tests/test_alerts.py
--rw-r--r--   0 ben000    (1000) users      (100)     7525 2020-05-17 20:23:53.000000 abow-0.4.3/tests/test_app.py
--rw-r--r--   0 ben000    (1000) users      (100)     3069 2020-05-09 16:21:33.000000 abow-0.4.3/tests/test_backend.py
--rw-r--r--   0 ben000    (1000) users      (100)     1557 2021-01-23 14:41:16.000000 abow-0.4.3/tests/test_config.py
--rw-r--r--   0 ben000    (1000) users      (100)      905 2019-11-12 22:07:36.000000 abow-0.4.3/tests/test_l10n.py
--rw-r--r--   0 ben000    (1000) users      (100)     1591 2021-05-18 10:00:42.000000 abow-0.4.3/tests/test_render.py
--rw-r--r--   0 ben000    (1000) users      (100)     1365 2020-05-01 17:58:10.000000 abow-0.4.3/tests/test_tags.py
--rw-r--r--   0 ben000    (1000) users      (100)    20343 2021-05-29 08:46:11.000000 abow-0.4.3/usage.md
--rw-r--r--   0 ben000    (1000) users      (100)      464 2021-05-20 19:20:56.000000 abow-0.4.3/welcome.md
+-rw-r--r--   0        0        0      921 2023-06-27 20:46:16.000000 abow-0.5.0/abow/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-27 20:46:16.000000 abow-0.5.0/abow/alerts.py
+-rw-r--r--   0        0        0     7187 2023-06-27 20:46:16.000000 abow-0.5.0/abow/app.py
+-rw-r--r--   0        0        0     6503 2023-06-27 20:46:16.000000 abow-0.5.0/abow/backend.py
+-rw-r--r--   0        0        0     6046 2023-06-27 20:46:16.000000 abow-0.5.0/abow/config.py
+-rw-r--r--   0        0        0     2024 2023-06-27 20:46:16.000000 abow-0.5.0/abow/l10n.py
+-rw-r--r--   0        0        0     7923 2023-06-27 20:46:16.000000 abow-0.5.0/abow/mdx_tables.py
+-rw-r--r--   0        0        0     2646 2023-06-27 20:46:16.000000 abow-0.5.0/abow/mdx_wikilinks.py
+-rw-r--r--   0        0        0     3534 2023-06-27 20:46:16.000000 abow-0.5.0/abow/render.py
+-rw-r--r--   0        0        0     2142 2023-06-27 20:46:16.000000 abow-0.5.0/abow/tags.py
+-rw-r--r--   0        0        0     6316 2023-06-27 20:46:16.000000 abow-0.5.0/abow/locale/abow.pot
+-rw-r--r--   0        0        0     5779 2023-06-27 20:46:16.000000 abow-0.5.0/abow/locale/en/LC_MESSAGES/abow.mo
+-rw-r--r--   0        0        0     6055 2023-06-27 20:46:16.000000 abow-0.5.0/abow/locale/fr/LC_MESSAGES/abow.mo
+-rw-r--r--   0        0        0     7194 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/css/abow.css
+-rw-r--r--   0        0        0   232914 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0     4166 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/css/highlight.css
+-rw-r--r--   0        0        0     3516 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/img/abow.svg
+-rw-r--r--   0        0        0      387 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/img/abow_16.png
+-rw-r--r--   0        0        0     1334 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/img/abow_32.png
+-rw-r--r--   0        0        0     4053 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/js/abow.js
+-rw-r--r--   0        0        0     3520 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/js/autosize.min.js
+-rw-r--r--   0        0        0    80421 2023-06-27 20:46:16.000000 abow-0.5.0/abow/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0     2601 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/about.tpl
+-rw-r--r--   0        0        0     5738 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/edit.tpl
+-rw-r--r--   0        0        0     1185 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/error.tpl
+-rw-r--r--   0        0        0     4216 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/index.tpl
+-rw-r--r--   0        0        0     1083 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/index_nav_item.tpl
+-rw-r--r--   0        0        0     1490 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/list_pages.tpl
+-rw-r--r--   0        0        0     1375 2023-06-27 20:46:16.000000 abow-0.5.0/abow/views/view.tpl
+-rw-r--r--   0        0        0     1929 2023-06-27 20:46:16.000000 abow-0.5.0/changelog.md
+-rw-r--r--   0        0        0     1486 2023-06-27 20:46:16.000000 abow-0.5.0/config.example
+-rw-r--r--   0        0        0     1259 2023-06-27 20:46:16.000000 abow-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      405 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_alerts.py
+-rw-r--r--   0        0        0     7525 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_app.py
+-rw-r--r--   0        0        0     3069 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_backend.py
+-rw-r--r--   0        0        0     1557 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_config.py
+-rw-r--r--   0        0        0      905 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_l10n.py
+-rw-r--r--   0        0        0     1595 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_render.py
+-rw-r--r--   0        0        0     1365 2023-06-27 20:46:16.000000 abow-0.5.0/tests/test_tags.py
+-rw-r--r--   0        0        0    20343 2023-06-27 20:46:16.000000 abow-0.5.0/usage.md
+-rw-r--r--   0        0        0      464 2023-06-27 20:46:16.000000 abow-0.5.0/welcome.md
+-rw-r--r--   0        0        0      134 2023-06-27 20:46:16.000000 abow-0.5.0/.gitignore
+-rw-r--r--   0        0        0    34283 2023-06-27 20:46:16.000000 abow-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4444 2023-06-27 20:46:16.000000 abow-0.5.0/README.md
+-rw-r--r--   0        0        0     2412 2023-06-27 20:46:16.000000 abow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5791 2023-06-27 20:46:16.000000 abow-0.5.0/PKG-INFO
```

### Comparing `abow-0.4.3/LICENSE.md` & `abow-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/PKG-INFO` & `abow-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,155 @@
 Metadata-Version: 2.1
 Name: abow
-Version: 0.4.3
+Version: 0.5.0
 Summary: A Bottle of Wiki — personal wiki
-Home-page: https://pypi.org/project/abow/
-Author: Benoît Monin
-Author-email: benoit.monin@gmx.fr
+Project-URL: Homepage, https://pypi.org/project/abow/
+Author-email: Benoît Monin <benoit.monin@gmx.fr>
 License: AGPL-3.0-or-later
-Description: # A Bottle of Wiki
-        
-        A Bottle of Wiki (abbreviated _abow_) is a personal wiki. Use it for viewing and
-        editing pages written in markdown directly in your browser. It is made to be
-        usable both on mobile and desktop.
-        
-        While you won't be hosting Wikipedia on a Bottle of Wiki, it is easy to deploy
-        and does not require a database: pages are saved as text files. It has no notion
-        of users, access rights, page history, comments, discussion or even edit
-        conflict. It is meant to be used by one person.
-        
-        A Bottle of Wiki is a wiki built with [bottle](https://bottlepy.org/).
-        
-        ## Installation
-        
-        To run a Bottle of Wiki, you will need python3 installed on a unix-like machine.
-        
-        ### Test (_a quick sip_)
-        
-        The easiest way to test a Bottle of Wiki is to install it in a virtual
-        environment. You can do so with the following commands:
-        ```sh
-        python3 -m venv abow
-        source abow/bin/activate
-        ```
-        Or use your favorite virtualenv management tool.
-        
-        Then install a Bottle of Wiki and its dependencies with pip:
-        ```sh
-        pip install abow
-        ```
-        
-        _Optional_: If you want syntax highlighting when displaying code in your page,
-        install the extra:
-        ```sh
-        pip install abow[extra]
-        ```
-        
-        Finally start the application with:
-        ```sh
-        bottle.py abow:application
-        ```
-        If all went well, you can point your browser to <http://127.0.0.1:8080/> and
-        start editing. The pages will be saved in the current directory. If you are
-        looking for inspiration, a few markdown pages (including this README) are part
-        of the [source distribution][sdist].
-        
-        [sdist]:https://files.pythonhosted.org/packages/source/a/abow/abow-0.4.3.tar.gz
-        
-        ### Deployment (_the whole bottle_)
-        
-        A Bottle of Wiki is a WSGI application, as such it can be hosted by any
-        WSGI-capable web server. The documentation of bottle has a page dedicated to the
-        [deployment](https://bottlepy.org/docs/stable/deployment.html) that can be used
-        as inspiration. Detailing how to host a WSGI application is beyond the scope of
-        this README as there are many options to choose from, but here is the most
-        important piece of advice:
-        
-        **Make sure the access is restricted.** A Bottle of Wiki has no concept of login
-        or user, so anyone with access can edit the pages. You can limit the access by
-        setting up HTTP authentication and encryption on your web server. You can also
-        serve only on a local network and access it via a VPN.
-        
-        ### Configuration
-        
-        A Bottle of Wiki can be customized with a .ini configuration file. A example is
-        provided in the source distribution, or you can generate it with the following
-        command:
-        ```sh
-        python -c "import abow.config;abow.config.print_file()"
-        ```
-        
-        The example configuration is heavily commented and should be self-explanatory.
-        It enable you to change where a Bottle of Wiki stores the pages and the locale
-        used. You can also host the static assets (css, js, ...) outside of the
-        application and serve them directly from a web server.
-        
-        The configuration is read from the following locations:
-        
-        * `/etc/abow/config`
-        * `$XDG_CONFIG_HOME/abow/config`, defaulting to `~/.config/abow/config`
-        * `$ABOW_CONFIG`, if defined
-        
-        Paths are tried one after one and each configuration file can override the
-        settings of the previous ones.
-        
-        ## Built With
-        
-        A Bottle of Wiki depends on the following python packages:
-        
-        * [Bottle](https://bottlepy.org/) -- The WSGI micro-framework used
-        * [Python-Markdown](https://python-markdown.github.io/)
-          -- The markdown interpreter
-        * [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
-          -- Extensions for Python Markdown
-        * [Pygments](https://pygments.org/) -- Syntax highlighter (_optional_)
-        
-        The following css and javascript packages are included:
-        
-        * [Bootstrap](https://getbootstrap.com) version 5.1.3 -- CSS Toolkit
-        * [Autosize](http://www.jacklmoore.com/autosize/) version 5.0.0
-          -- Script to automatically adjust textarea height
-        
-        ## Things to do
-        
-        ### Detection of edit conflict
-        
-        Right now if you edit a page from two browsers you can lose some modifications.
-        Detecting that the page has been changed on the server while being edited would
-        be nice if you want to use a Bottle of Wiki with more than one user.
-        
-        ### Page history
-        
-        While you can avoid losing changes by setting up a backup on the server (and you
-        should anyway), integrating the page history in the wiki would make is easier to
-        review the page modifications. Look into [dulwich](https://www.dulwich.io/) for
-        that?
-        
-        ## License
-        
-        This project is licensed under the Affero General Public License version 3 or later.
-        
-Keywords: wiki bottle markdown
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+License-File: LICENSE.md
+Keywords: bottle,markdown,wiki
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Bottle
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Requires-Python: >=3.8
+Requires-Dist: bottle>=0.12.0
+Requires-Dist: markdown>=3.2
+Requires-Dist: pymdown-extensions>=7.0
 Provides-Extra: dev
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
 Provides-Extra: extra
+Requires-Dist: pygments>=2.4; extra == 'extra'
+Description-Content-Type: text/markdown
+
+# A Bottle of Wiki
+
+A Bottle of Wiki (abbreviated _abow_) is a personal wiki. Use it for viewing and
+editing pages written in markdown directly in your browser. It is made to be
+usable both on mobile and desktop.
+
+While you won't be hosting Wikipedia on a Bottle of Wiki, it is easy to deploy
+and does not require a database: pages are saved as text files. It has no notion
+of users, access rights, page history, comments, discussion or even edit
+conflict. It is meant to be used by one person.
+
+A Bottle of Wiki is a wiki built with [bottle](https://bottlepy.org/).
+
+## Installation
+
+To run a Bottle of Wiki, you will need python3 installed on a unix-like machine.
+
+### Test (_a quick sip_)
+
+The easiest way to test a Bottle of Wiki is to install it in a virtual
+environment. You can do so with the following commands:
+```sh
+python3 -m venv abow
+source abow/bin/activate
+```
+Or use your favorite virtualenv management tool.
+
+Then install a Bottle of Wiki and its dependencies with pip:
+```sh
+pip install abow
+```
+
+_Optional_: If you want syntax highlighting when displaying code in your page,
+install the extra:
+```sh
+pip install abow[extra]
+```
+
+Finally start the application with:
+```sh
+bottle.py abow:application
+```
+If all went well, you can point your browser to <http://127.0.0.1:8080/> and
+start editing. The pages will be saved in the current directory. If you are
+looking for inspiration, a few markdown pages (including this README) are part
+of the [source distribution][sdist].
+
+[sdist]:https://files.pythonhosted.org/packages/source/a/abow/abow-0.5.0.tar.gz
+
+### Deployment (_the whole bottle_)
+
+A Bottle of Wiki is a WSGI application, as such it can be hosted by any
+WSGI-capable web server. The documentation of bottle has a page dedicated to the
+[deployment](https://bottlepy.org/docs/stable/deployment.html) that can be used
+as inspiration. Detailing how to host a WSGI application is beyond the scope of
+this README as there are many options to choose from, but here is the most
+important piece of advice:
+
+**Make sure the access is restricted.** A Bottle of Wiki has no concept of login
+or user, so anyone with access can edit the pages. You can limit the access by
+setting up HTTP authentication and encryption on your web server. You can also
+serve only on a local network and access it via a VPN.
+
+### Configuration
+
+A Bottle of Wiki can be customized with a .ini configuration file. A example is
+provided in the source distribution, or you can generate it with the following
+command:
+```sh
+python -c "import abow.config;abow.config.print_file()"
+```
+
+The example configuration is heavily commented and should be self-explanatory.
+It enable you to change where a Bottle of Wiki stores the pages and the locale
+used. You can also host the static assets (css, js, ...) outside of the
+application and serve them directly from a web server.
+
+The configuration is read from the following locations:
+
+* `/etc/abow/config`
+* `$XDG_CONFIG_HOME/abow/config`, defaulting to `~/.config/abow/config`
+* `$ABOW_CONFIG`, if defined
+
+Paths are tried one after one and each configuration file can override the
+settings of the previous ones.
+
+## Built With
+
+A Bottle of Wiki depends on the following python packages:
+
+* [Bottle](https://bottlepy.org/) -- The WSGI micro-framework used
+* [Python-Markdown](https://python-markdown.github.io/)
+  -- The markdown interpreter
+* [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
+  -- Extensions for Python Markdown
+* [Pygments](https://pygments.org/) -- Syntax highlighter (_optional_)
+
+The following css and javascript packages are included:
+
+* [Bootstrap](https://getbootstrap.com) version 5.3.0 -- CSS Toolkit
+* [Autosize](http://www.jacklmoore.com/autosize/) version 5.0.0
+  -- Script to automatically adjust textarea height
+
+## Things to do
+
+### Detection of edit conflict
+
+Right now if you edit a page from two browsers you can lose some modifications.
+Detecting that the page has been changed on the server while being edited would
+be nice if you want to use a Bottle of Wiki with more than one user.
+
+### Page history
+
+While you can avoid losing changes by setting up a backup on the server (and you
+should anyway), integrating the page history in the wiki would make is easier to
+review the page modifications. Look into [dulwich](https://www.dulwich.io/) for
+that?
+
+## License
+
+This project is licensed under the Affero General Public License version 3 or later.
```

### Comparing `abow-0.4.3/README.md` & `abow-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 bottle.py abow:application
 ```
 If all went well, you can point your browser to <http://127.0.0.1:8080/> and
 start editing. The pages will be saved in the current directory. If you are
 looking for inspiration, a few markdown pages (including this README) are part
 of the [source distribution][sdist].
 
-[sdist]:https://files.pythonhosted.org/packages/source/a/abow/abow-0.4.3.tar.gz
+[sdist]:https://files.pythonhosted.org/packages/source/a/abow/abow-0.5.0.tar.gz
 
 ### Deployment (_the whole bottle_)
 
 A Bottle of Wiki is a WSGI application, as such it can be hosted by any
 WSGI-capable web server. The documentation of bottle has a page dedicated to the
 [deployment](https://bottlepy.org/docs/stable/deployment.html) that can be used
 as inspiration. Detailing how to host a WSGI application is beyond the scope of
@@ -93,15 +93,15 @@
   -- The markdown interpreter
 * [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
   -- Extensions for Python Markdown
 * [Pygments](https://pygments.org/) -- Syntax highlighter (_optional_)
 
 The following css and javascript packages are included:
 
-* [Bootstrap](https://getbootstrap.com) version 5.1.3 -- CSS Toolkit
+* [Bootstrap](https://getbootstrap.com) version 5.3.0 -- CSS Toolkit
 * [Autosize](http://www.jacklmoore.com/autosize/) version 5.0.0
   -- Script to automatically adjust textarea height
 
 ## Things to do
 
 ### Detection of edit conflict
```

### Comparing `abow-0.4.3/abow/__init__.py` & `abow-0.5.0/abow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/alerts.py` & `abow-0.5.0/abow/alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/app.py` & `abow-0.5.0/abow/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,18 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import re
 import urllib.parse
 import builtins
 import math
 import bottle
-try:
-    from importlib import metadata
-except ImportError:
-    import importlib_metadata as metadata
+from importlib import metadata
 
 from . import alerts
 from . import backend
 from . import config
 from . import l10n
 from . import render
 from . import tags
```

### Comparing `abow-0.4.3/abow/backend.py` & `abow-0.5.0/abow/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/config.py` & `abow-0.5.0/abow/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-try:
-    from importlib import resources
-except ImportError:
-    import importlib_resources as resources
+from importlib import resources
 import os
 import os.path
 import locale
 import textwrap
 
 # keep a reference of the configuration
 _cfg = None
```

### Comparing `abow-0.4.3/abow/l10n.py` & `abow-0.5.0/abow/l10n.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/locale/abow.pot` & `abow-0.5.0/abow/locale/abow.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,66 +2,66 @@
 # Copyright (C) YEAR Benoît Monin
 # This file is distributed under the same license as the abow package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: abow 0.4.3\n"
+"Project-Id-Version: abow 0.5.0\n"
 "Report-Msgid-Bugs-To: benoit.monin@gmx.fr\n"
-"POT-Creation-Date: 2022-04-21 17:08+0200\n"
+"POT-Creation-Date: 2023-06-27 22:46+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: abow/app.py:50
+#: abow/app.py:47
 msgid "Application started in debug mode."
 msgstr ""
 
-#: abow/app.py:145
+#: abow/app.py:142
 msgid "Edit {}"
 msgstr ""
 
-#: abow/app.py:168
+#: abow/app.py:165
 msgid "List of pages tagged {}"
 msgstr ""
 
-#: abow/app.py:171
+#: abow/app.py:168
 msgid "List of pages containing {}"
 msgstr ""
 
-#: abow/app.py:177 abow/views/index.tpl:47
+#: abow/app.py:174 abow/views/index.tpl:47
 msgid "List of pages"
 msgstr ""
 
-#: abow/app.py:191 abow/views/index.tpl:52
+#: abow/app.py:188 abow/views/index.tpl:52
 msgid "About"
 msgstr ""
 
-#: abow/app.py:193
+#: abow/app.py:190
 msgid "Version {}"
 msgstr ""
 
-#: abow/app.py:195
+#: abow/app.py:192
 msgid "Developement version"
 msgstr ""
 
-#: abow/app.py:208
+#: abow/app.py:205
 msgid "Error {}"
 msgstr ""
 
-#: abow/app.py:222
+#: abow/app.py:219
 msgid "Page name cannot be blank and cannot contain '/' or '|'"
 msgstr ""
 
-#: abow/app.py:225
+#: abow/app.py:222
 msgid "A page named {} already exists"
 msgstr ""
 
 #: abow/backend.py:75
 msgid "Failed to read the content of page {}: {}."
 msgstr ""
 
@@ -81,31 +81,31 @@
 msgid "Failed to load the attributes of page {}: {}."
 msgstr ""
 
 #: abow/backend.py:159
 msgid "Failed to save the attributes of page {}: {}."
 msgstr ""
 
-#: abow/config.py:50
+#: abow/config.py:47
 msgid "Path to the backend storage"
 msgstr ""
 
-#: abow/config.py:58
+#: abow/config.py:55
 msgid "Base url for the static resources, if hosted outside of the app"
 msgstr ""
 
-#: abow/config.py:66
+#: abow/config.py:63
 msgid "The locale to use"
 msgstr ""
 
-#: abow/config.py:73
+#: abow/config.py:70
 msgid "Name of the welcome page of the wiki"
 msgstr ""
 
-#: abow/config.py:82
+#: abow/config.py:79
 msgid "Name of the help page of the wiki"
 msgstr ""
 
 #: abow/l10n.py:40
 #, python-brace-format
 msgid "Invalid locale \"{cfg}\", using \"{dflt}\""
 msgstr ""
```

### Comparing `abow-0.4.3/abow/locale/en/LC_MESSAGES/abow.mo` & `abow-0.5.0/abow/locale/en/LC_MESSAGES/abow.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,10 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: abow 0.4.3\n"
+"Project-Id-Version: abow 0.5.0\n"
 "Report-Msgid-Bugs-To: benoit.monin@gmx.fr\n"
 "PO-Revision-Date: 2020-05-01 21:08+0200\n"
 "Last-Translator: Benoît Monin <benoit.monin@gmx.fr>\n"
 "Language-Team: \n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
```

### Comparing `abow-0.4.3/abow/locale/fr/LC_MESSAGES/abow.mo` & `abow-0.5.0/abow/locale/fr/LC_MESSAGES/abow.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,10 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: abow 0.4.3\n"
+"Project-Id-Version: abow 0.5.0\n"
 "Report-Msgid-Bugs-To: benoit.monin@gmx.fr\n"
 "PO-Revision-Date: 2020-05-01 21:09+0200\n"
 "Last-Translator: Benoît Monin <benoit.monin@gmx.fr>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
```

### Comparing `abow-0.4.3/abow/mdx_tables.py` & `abow-0.5.0/abow/mdx_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
         # Build table
         div_resp = etree.SubElement(parent, 'div')
         div_resp.set('class', 'table-responsive')
         table = etree.SubElement(div_resp, 'table')
         table.set('class', 'table table-bordered')
         thead = etree.SubElement(table, 'thead')
-        thead.set('class', 'table-secondary')
         self._build_row(header, thead, align)
         tbody = etree.SubElement(table, 'tbody')
+        tbody.set('class', 'table-group-divider')
         if len(rows) == 0:
             # Handle empty table
             self._build_empty_row(tbody, align)
         else:
             for row in rows:
                 self._build_row(row.strip(' '), tbody, align)
```

### Comparing `abow-0.4.3/abow/mdx_wikilinks.py` & `abow-0.5.0/abow/mdx_wikilinks.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/abow/render.py` & `abow-0.5.0/abow/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/static/css/abow.css` & `abow-0.5.0/abow/static/css/abow.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /* A Bottle of Wiki — personal wiki
  * SPDX-License-Identifier: AGPL-3.0-or-later
- * Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+ * Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Affero General Public License as
  * published by the Free Software Foundation, either version 3 of the
  * License, or (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -107,15 +107,15 @@
     overflow-y: auto;
     top: 4.5rem;
     height: calc(100vh - 5.5rem);
 }
 
 /* style for the toc */
 div.toc {
-    border-left: 1px solid #dee2e6;
+    border-left: 1px solid var(--bs-secondary-bg);
 }
 div.toc ul {
     padding-left: 0rem;
     margin: 0.1rem;
     list-style: none;
 }
 div.toc li {
@@ -149,15 +149,15 @@
     content: "↗︎";
 }
 .abow_view a.wikilink::after {
     content: "";
 }
 .abow_view blockquote {
     border-width: 0 0 0 0.2rem;
-    border-color: #dee2e6;
+    border-color: var(--bs-secondary-bg);
     border-style: solid;
     padding-left: 1rem;
     margin-left: 0.2rem;
 }
 .abow_view pre {
     border: 0;
 }
@@ -167,23 +167,23 @@
 }
 .abow_view dd {
     margin-left: 2.5rem;
 }
 
 /* code block */
 div.highlight {
-    background-color: var(--bs-light);
+    background-color: var(--bs-tertiary-bg);
     border-radius: 0.25rem;
 }
 
 /* admonitions, insipred by bootstrap documentation callouts */
 div.admonition {
     padding: 1rem 1.25rem;
     margin: 1.25rem 0;
-    border: 1px solid #eee;
+    border: 1px solid var(--bs-secondary-bg);
     border-left-width: .25rem;
     border-radius: .25rem;
 }
 div.admonition.attention {
     border-left-color: var(--bs-info);
 }
 div.admonition.caution {
@@ -246,15 +246,15 @@
 .task-list-control input[type="checkbox"]:checked + .task-list-indicator::before {
     display: block;
     margin-top: -0.25rem;
     margin-left: 0;
     font-size: 1.25rem;
     line-height: 1;
     content: "✔︎";
-    color: var(--bs-dark);
+    color: var(--bs-secondary-color);
 }
 
 /* footnotes */
 a.footnote-ref::after {
     content: "";
 }
 a.footnote-backref::after {
@@ -265,56 +265,56 @@
 }
 
 /* tabbed blocks */
 .tabbed-set {
     display: flex;
     position: relative;
     flex-wrap: wrap;
-    border: 1px solid #eee;
+    border: 1px solid var(--bs-secondary-bg);
     border-radius: 0.25rem;
     margin-bottom: 1rem;
 }
 .tabbed-set > .tabbed-content {
     display: none;
     order: 99;
     width: 100%;
     padding: 1rem 0.5rem 0;
-    border-top: #eee solid 1px;
+    border-top: var(--bs-secondary-bg) solid 1px;
 }
 .tabbed-set > label {
     width: auto;
     margin: 0;
     padding: 0.5rem;
     cursor: pointer;
     color: var(--bs-primary);
 }
 .tabbed-set > input {
     position: absolute;
     opacity: 0;
     z-index: -1;
 }
 .tabbed-set input:nth-child(n+1):checked + label {
-    border-bottom: #eee solid 0.2rem;
+    border-bottom: var(--bs-secondary-bg) solid 0.2rem;
     font-weight: bold;
-    color: var(--bs-dark);
+    color: var(--bs-secondary-color);
 }
 .tabbed-set input:nth-child(n+1):checked + label + .tabbed-content {
     display: block;
 }
 @media print {
     .tabbed-set {
         display: block;
     }
     .tabbed-set > .tabbed-content {
         display: block;
     }
     .tabbed-set > label {
-        border-bottom: #eee solid 0.2rem;
+        border-bottom: var(--bs-secondary-bg) solid 0.2rem;
         font-weight: bold;
-        color: var(--bs-dark);
+        color: var(--bs-secondary-color);
     }
     .abow_view a::after {
         content: " ("attr(href)")";
     }
     .abow_view a.wikilink::after {
         content: "";
     }
```

### Comparing `abow-0.4.3/abow/static/css/highlight.css` & `abow-0.5.0/abow/static/css/highlight.css`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/abow/static/img/abow.svg` & `abow-0.5.0/abow/static/img/abow.svg`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/abow/static/img/abow_32.png` & `abow-0.5.0/abow/static/img/abow_32.png`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/abow/static/js/abow.js` & `abow-0.5.0/abow/static/js/abow.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /* A Bottle of Wiki — personal wiki
  * SPDX-License-Identifier: AGPL-3.0-or-later
- * Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+ * Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Affero General Public License as
  * published by the Free Software Foundation, either version 3 of the
  * License, or (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -99,8 +99,23 @@
     /* set the text selection to the content */
     editor.selectionStart = start + preamble.length;
     editor.selectionEnd = editor.selectionStart + content.length;
 
     /* resize the editor and set the focus */
     autosize.update(editor);
     editor.focus();
-}
+}
+
+/* Set the bootstrap color theme based on the prefered color scheme
+ */
+function set_bs_theme() {
+    const colorMode = window.matchMedia("(prefers-color-scheme: dark)").matches ?
+        "dark" :
+        "light";
+    document.querySelector("html").setAttribute("data-bs-theme", colorMode);
+}
+
+/* Set theme on load */
+set_bs_theme()
+
+/* Update theme when the preferred scheme changes */
+window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', set_bs_theme)
```

### Comparing `abow-0.4.3/abow/static/js/autosize.min.js` & `abow-0.5.0/abow/static/js/autosize.min.js`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/abow/static/js/bootstrap.bundle.min.js` & `abow-0.5.0/abow/static/js/bootstrap.bundle.min.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,802 +1,834 @@
 /*!
- * Bootstrap v5.1.3 (https://getbootstrap.com/)
- * Copyright 2011-2021 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
+ * Bootstrap v5.3.0 (https://getbootstrap.com/)
+ * Copyright 2011-2023 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
  */
 ! function(t, e) {
     "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define(e) : (t = "undefined" != typeof globalThis ? globalThis : t || self).bootstrap = e()
 }(this, (function() {
     "use strict";
-    const t = "transitionend",
-        e = t => {
-            let e = t.getAttribute("data-bs-target");
-            if (!e || "#" === e) {
-                let i = t.getAttribute("href");
-                if (!i || !i.includes("#") && !i.startsWith(".")) return null;
-                i.includes("#") && !i.startsWith("#") && (i = `#${i.split("#")[1]}`), e = i && "#" !== i ? i.trim() : null
+    const t = new Map,
+        e = {
+            set(e, i, n) {
+                t.has(e) || t.set(e, new Map);
+                const s = t.get(e);
+                s.has(i) || 0 === s.size ? s.set(i, n) : console.error(`Bootstrap doesn't allow more than one instance per element. Bound instance: ${Array.from(s.keys())[0]}.`)
+            },
+            get: (e, i) => t.has(e) && t.get(e).get(i) || null,
+            remove(e, i) {
+                if (!t.has(e)) return;
+                const n = t.get(e);
+                n.delete(i), 0 === n.size && t.delete(e)
             }
-            return e
-        },
-        i = t => {
-            const i = e(t);
-            return i && document.querySelector(i) ? i : null
-        },
-        n = t => {
-            const i = e(t);
-            return i ? document.querySelector(i) : null
         },
-        s = e => {
-            e.dispatchEvent(new Event(t))
+        i = "transitionend",
+        n = t => (t && window.CSS && window.CSS.escape && (t = t.replace(/#([^\s"#']+)/g, ((t, e) => `#${CSS.escape(e)}`))), t),
+        s = t => {
+            t.dispatchEvent(new Event(i))
         },
         o = t => !(!t || "object" != typeof t) && (void 0 !== t.jquery && (t = t[0]), void 0 !== t.nodeType),
-        r = t => o(t) ? t.jquery ? t[0] : t : "string" == typeof t && t.length > 0 ? document.querySelector(t) : null,
-        a = (t, e, i) => {
-            Object.keys(i).forEach((n => {
-                const s = i[n],
-                    r = e[n],
-                    a = r && o(r) ? "element" : null == (l = r) ? `${l}` : {}.toString.call(l).match(/\s([a-z]+)/i)[1].toLowerCase();
-                var l;
-                if (!new RegExp(s).test(a)) throw new TypeError(`${t.toUpperCase()}: Option "${n}" provided type "${a}" but expected type "${s}".`)
-            }))
+        r = t => o(t) ? t.jquery ? t[0] : t : "string" == typeof t && t.length > 0 ? document.querySelector(n(t)) : null,
+        a = t => {
+            if (!o(t) || 0 === t.getClientRects().length) return !1;
+            const e = "visible" === getComputedStyle(t).getPropertyValue("visibility"),
+                i = t.closest("details:not([open])");
+            if (!i) return e;
+            if (i !== t) {
+                const e = t.closest("summary");
+                if (e && e.parentNode !== i) return !1;
+                if (null === e) return !1
+            }
+            return e
         },
-        l = t => !(!o(t) || 0 === t.getClientRects().length) && "visible" === getComputedStyle(t).getPropertyValue("visibility"),
-        c = t => !t || t.nodeType !== Node.ELEMENT_NODE || !!t.classList.contains("disabled") || (void 0 !== t.disabled ? t.disabled : t.hasAttribute("disabled") && "false" !== t.getAttribute("disabled")),
-        h = t => {
+        l = t => !t || t.nodeType !== Node.ELEMENT_NODE || !!t.classList.contains("disabled") || (void 0 !== t.disabled ? t.disabled : t.hasAttribute("disabled") && "false" !== t.getAttribute("disabled")),
+        c = t => {
             if (!document.documentElement.attachShadow) return null;
             if ("function" == typeof t.getRootNode) {
                 const e = t.getRootNode();
                 return e instanceof ShadowRoot ? e : null
             }
-            return t instanceof ShadowRoot ? t : t.parentNode ? h(t.parentNode) : null
+            return t instanceof ShadowRoot ? t : t.parentNode ? c(t.parentNode) : null
         },
-        d = () => {},
-        u = t => {
+        h = () => {},
+        d = t => {
             t.offsetHeight
         },
-        f = () => {
-            const {
-                jQuery: t
-            } = window;
-            return t && !document.body.hasAttribute("data-bs-no-jquery") ? t : null
-        },
-        p = [],
-        m = () => "rtl" === document.documentElement.dir,
-        g = t => {
+        u = () => window.jQuery && !document.body.hasAttribute("data-bs-no-jquery") ? window.jQuery : null,
+        f = [],
+        p = () => "rtl" === document.documentElement.dir,
+        m = t => {
             var e;
             e = () => {
-                const e = f();
+                const e = u();
                 if (e) {
                     const i = t.NAME,
                         n = e.fn[i];
                     e.fn[i] = t.jQueryInterface, e.fn[i].Constructor = t, e.fn[i].noConflict = () => (e.fn[i] = n, t.jQueryInterface)
                 }
-            }, "loading" === document.readyState ? (p.length || document.addEventListener("DOMContentLoaded", (() => {
-                p.forEach((t => t()))
-            })), p.push(e)) : e()
-        },
-        _ = t => {
-            "function" == typeof t && t()
-        },
-        b = (e, i, n = !0) => {
-            if (!n) return void _(e);
+            }, "loading" === document.readyState ? (f.length || document.addEventListener("DOMContentLoaded", (() => {
+                for (const t of f) t()
+            })), f.push(e)) : e()
+        },
+        g = (t, e = [], i = t) => "function" == typeof t ? t(...e) : i,
+        _ = (t, e, n = !0) => {
+            if (!n) return void g(t);
             const o = (t => {
                 if (!t) return 0;
                 let {
                     transitionDuration: e,
                     transitionDelay: i
                 } = window.getComputedStyle(t);
                 const n = Number.parseFloat(e),
                     s = Number.parseFloat(i);
                 return n || s ? (e = e.split(",")[0], i = i.split(",")[0], 1e3 * (Number.parseFloat(e) + Number.parseFloat(i))) : 0
-            })(i) + 5;
+            })(e) + 5;
             let r = !1;
             const a = ({
                 target: n
             }) => {
-                n === i && (r = !0, i.removeEventListener(t, a), _(e))
+                n === e && (r = !0, e.removeEventListener(i, a), g(t))
             };
-            i.addEventListener(t, a), setTimeout((() => {
-                r || s(i)
+            e.addEventListener(i, a), setTimeout((() => {
+                r || s(e)
             }), o)
         },
-        v = (t, e, i, n) => {
-            let s = t.indexOf(e);
-            if (-1 === s) return t[!i && n ? t.length - 1 : 0];
-            const o = t.length;
-            return s += i ? 1 : -1, n && (s = (s + o) % o), t[Math.max(0, Math.min(s, o - 1))]
-        },
-        y = /[^.]*(?=\..*)\.|.*/,
-        w = /\..*/,
-        E = /::\d+$/,
+        b = (t, e, i, n) => {
+            const s = t.length;
+            let o = t.indexOf(e);
+            return -1 === o ? !i && n ? t[s - 1] : t[0] : (o += i ? 1 : -1, n && (o = (o + s) % s), t[Math.max(0, Math.min(o, s - 1))])
+        },
+        v = /[^.]*(?=\..*)\.|.*/,
+        y = /\..*/,
+        w = /::\d+$/,
         A = {};
-    let T = 1;
-    const O = {
+    let E = 1;
+    const T = {
             mouseenter: "mouseover",
             mouseleave: "mouseout"
         },
-        C = /^(mouseenter|mouseleave)/i,
-        k = new Set(["click", "dblclick", "mouseup", "mousedown", "contextmenu", "mousewheel", "DOMMouseScroll", "mouseover", "mouseout", "mousemove", "selectstart", "selectend", "keydown", "keypress", "keyup", "orientationchange", "touchstart", "touchmove", "touchend", "touchcancel", "pointerdown", "pointermove", "pointerup", "pointerleave", "pointercancel", "gesturestart", "gesturechange", "gestureend", "focus", "blur", "change", "reset", "select", "submit", "focusin", "focusout", "load", "unload", "beforeunload", "resize", "move", "DOMContentLoaded", "readystatechange", "error", "abort", "scroll"]);
+        C = new Set(["click", "dblclick", "mouseup", "mousedown", "contextmenu", "mousewheel", "DOMMouseScroll", "mouseover", "mouseout", "mousemove", "selectstart", "selectend", "keydown", "keypress", "keyup", "orientationchange", "touchstart", "touchmove", "touchend", "touchcancel", "pointerdown", "pointermove", "pointerup", "pointerleave", "pointercancel", "gesturestart", "gesturechange", "gestureend", "focus", "blur", "change", "reset", "select", "submit", "focusin", "focusout", "load", "unload", "beforeunload", "resize", "move", "DOMContentLoaded", "readystatechange", "error", "abort", "scroll"]);
 
-    function L(t, e) {
-        return e && `${e}::${T++}` || t.uidEvent || T++
+    function O(t, e) {
+        return e && `${e}::${E++}` || t.uidEvent || E++
     }
 
     function x(t) {
-        const e = L(t);
+        const e = O(t);
         return t.uidEvent = e, A[e] = A[e] || {}, A[e]
     }
 
-    function D(t, e, i = null) {
-        const n = Object.keys(t);
-        for (let s = 0, o = n.length; s < o; s++) {
-            const o = t[n[s]];
-            if (o.originalHandler === e && o.delegationSelector === i) return o
-        }
-        return null
+    function k(t, e, i = null) {
+        return Object.values(t).find((t => t.callable === e && t.delegationSelector === i))
     }
 
-    function S(t, e, i) {
+    function L(t, e, i) {
         const n = "string" == typeof e,
-            s = n ? i : e;
-        let o = P(t);
-        return k.has(o) || (o = t), [n, s, o]
+            s = n ? i : e || i;
+        let o = N(t);
+        return C.has(o) || (o = t), [n, s, o]
     }
 
-    function N(t, e, i, n, s) {
+    function S(t, e, i, n, s) {
         if ("string" != typeof e || !t) return;
-        if (i || (i = n, n = null), C.test(e)) {
+        let [o, r, a] = L(e, i, n);
+        if (e in T) {
             const t = t => function(e) {
                 if (!e.relatedTarget || e.relatedTarget !== e.delegateTarget && !e.delegateTarget.contains(e.relatedTarget)) return t.call(this, e)
             };
-            n ? n = t(n) : i = t(i)
+            r = t(r)
         }
-        const [o, r, a] = S(e, i, n), l = x(t), c = l[a] || (l[a] = {}), h = D(c, r, o ? i : null);
+        const l = x(t),
+            c = l[a] || (l[a] = {}),
+            h = k(c, r, o ? i : null);
         if (h) return void(h.oneOff = h.oneOff && s);
-        const d = L(r, e.replace(y, "")),
+        const d = O(r, e.replace(v, "")),
             u = o ? function(t, e, i) {
                 return function n(s) {
                     const o = t.querySelectorAll(e);
                     for (let {
                             target: r
                         } = s; r && r !== this; r = r.parentNode)
-                        for (let a = o.length; a--;)
-                            if (o[a] === r) return s.delegateTarget = r, n.oneOff && j.off(t, s.type, e, i), i.apply(r, [s]);
-                    return null
+                        for (const a of o)
+                            if (a === r) return M(s, {
+                                delegateTarget: r
+                            }), n.oneOff && P.off(t, s.type, e, i), i.apply(r, [s])
                 }
-            }(t, i, n) : function(t, e) {
+            }(t, i, r) : function(t, e) {
                 return function i(n) {
-                    return n.delegateTarget = t, i.oneOff && j.off(t, n.type, e), e.apply(t, [n])
+                    return M(n, {
+                        delegateTarget: t
+                    }), i.oneOff && P.off(t, n.type, e), e.apply(t, [n])
                 }
-            }(t, i);
-        u.delegationSelector = o ? i : null, u.originalHandler = r, u.oneOff = s, u.uidEvent = d, c[d] = u, t.addEventListener(a, u, o)
+            }(t, r);
+        u.delegationSelector = o ? i : null, u.callable = r, u.oneOff = s, u.uidEvent = d, c[d] = u, t.addEventListener(a, u, o)
     }
 
-    function I(t, e, i, n, s) {
-        const o = D(e[i], n, s);
+    function D(t, e, i, n, s) {
+        const o = k(e[i], n, s);
         o && (t.removeEventListener(i, o, Boolean(s)), delete e[i][o.uidEvent])
     }
 
-    function P(t) {
-        return t = t.replace(w, ""), O[t] || t
+    function I(t, e, i, n) {
+        const s = e[i] || {};
+        for (const [o, r] of Object.entries(s)) o.includes(n) && D(t, e, i, r.callable, r.delegationSelector)
+    }
+
+    function N(t) {
+        return t = t.replace(y, ""), T[t] || t
+    }
+    const P = {
+        on(t, e, i, n) {
+            S(t, e, i, n, !1)
+        },
+        one(t, e, i, n) {
+            S(t, e, i, n, !0)
+        },
+        off(t, e, i, n) {
+            if ("string" != typeof e || !t) return;
+            const [s, o, r] = L(e, i, n), a = r !== e, l = x(t), c = l[r] || {}, h = e.startsWith(".");
+            if (void 0 === o) {
+                if (h)
+                    for (const i of Object.keys(l)) I(t, l, i, e.slice(1));
+                for (const [i, n] of Object.entries(c)) {
+                    const s = i.replace(w, "");
+                    a && !e.includes(s) || D(t, l, r, n.callable, n.delegationSelector)
+                }
+            } else {
+                if (!Object.keys(c).length) return;
+                D(t, l, r, o, s ? i : null)
+            }
+        },
+        trigger(t, e, i) {
+            if ("string" != typeof e || !t) return null;
+            const n = u();
+            let s = null,
+                o = !0,
+                r = !0,
+                a = !1;
+            e !== N(e) && n && (s = n.Event(e, i), n(t).trigger(s), o = !s.isPropagationStopped(), r = !s.isImmediatePropagationStopped(), a = s.isDefaultPrevented());
+            const l = M(new Event(e, {
+                bubbles: o,
+                cancelable: !0
+            }), i);
+            return a && l.preventDefault(), r && t.dispatchEvent(l), l.defaultPrevented && s && s.preventDefault(), l
+        }
+    };
+
+    function M(t, e = {}) {
+        for (const [i, n] of Object.entries(e)) try {
+            t[i] = n
+        } catch (e) {
+            Object.defineProperty(t, i, {
+                configurable: !0,
+                get: () => n
+            })
+        }
+        return t
     }
-    const j = {
-            on(t, e, i, n) {
-                N(t, e, i, n, !1)
-            },
-            one(t, e, i, n) {
-                N(t, e, i, n, !0)
-            },
-            off(t, e, i, n) {
-                if ("string" != typeof e || !t) return;
-                const [s, o, r] = S(e, i, n), a = r !== e, l = x(t), c = e.startsWith(".");
-                if (void 0 !== o) {
-                    if (!l || !l[r]) return;
-                    return void I(t, l, r, o, s ? i : null)
-                }
-                c && Object.keys(l).forEach((i => {
-                    ! function(t, e, i, n) {
-                        const s = e[i] || {};
-                        Object.keys(s).forEach((o => {
-                            if (o.includes(n)) {
-                                const n = s[o];
-                                I(t, e, i, n.originalHandler, n.delegationSelector)
-                            }
-                        }))
-                    }(t, l, i, e.slice(1))
-                }));
-                const h = l[r] || {};
-                Object.keys(h).forEach((i => {
-                    const n = i.replace(E, "");
-                    if (!a || e.includes(n)) {
-                        const e = h[i];
-                        I(t, l, r, e.originalHandler, e.delegationSelector)
-                    }
-                }))
-            },
-            trigger(t, e, i) {
-                if ("string" != typeof e || !t) return null;
-                const n = f(),
-                    s = P(e),
-                    o = e !== s,
-                    r = k.has(s);
-                let a, l = !0,
-                    c = !0,
-                    h = !1,
-                    d = null;
-                return o && n && (a = n.Event(e, i), n(t).trigger(a), l = !a.isPropagationStopped(), c = !a.isImmediatePropagationStopped(), h = a.isDefaultPrevented()), r ? (d = document.createEvent("HTMLEvents"), d.initEvent(s, l, !0)) : d = new CustomEvent(e, {
-                    bubbles: l,
-                    cancelable: !0
-                }), void 0 !== i && Object.keys(i).forEach((t => {
-                    Object.defineProperty(d, t, {
-                        get: () => i[t]
-                    })
-                })), h && d.preventDefault(), c && t.dispatchEvent(d), d.defaultPrevented && void 0 !== a && a.preventDefault(), d
-            }
-        },
-        M = new Map,
-        H = {
-            set(t, e, i) {
-                M.has(t) || M.set(t, new Map);
-                const n = M.get(t);
-                n.has(e) || 0 === n.size ? n.set(e, i) : console.error(`Bootstrap doesn't allow more than one instance per element. Bound instance: ${Array.from(n.keys())[0]}.`)
-            },
-            get: (t, e) => M.has(t) && M.get(t).get(e) || null,
-            remove(t, e) {
-                if (!M.has(t)) return;
-                const i = M.get(t);
-                i.delete(e), 0 === i.size && M.delete(t)
+
+    function j(t) {
+        if ("true" === t) return !0;
+        if ("false" === t) return !1;
+        if (t === Number(t).toString()) return Number(t);
+        if ("" === t || "null" === t) return null;
+        if ("string" != typeof t) return t;
+        try {
+            return JSON.parse(decodeURIComponent(t))
+        } catch (e) {
+            return t
+        }
+    }
+
+    function F(t) {
+        return t.replace(/[A-Z]/g, (t => `-${t.toLowerCase()}`))
+    }
+    const H = {
+        setDataAttribute(t, e, i) {
+            t.setAttribute(`data-bs-${F(e)}`, i)
+        },
+        removeDataAttribute(t, e) {
+            t.removeAttribute(`data-bs-${F(e)}`)
+        },
+        getDataAttributes(t) {
+            if (!t) return {};
+            const e = {},
+                i = Object.keys(t.dataset).filter((t => t.startsWith("bs") && !t.startsWith("bsConfig")));
+            for (const n of i) {
+                let i = n.replace(/^bs/, "");
+                i = i.charAt(0).toLowerCase() + i.slice(1, i.length), e[i] = j(t.dataset[n])
             }
-        };
-    class B {
-        constructor(t) {
-            (t = r(t)) && (this._element = t, H.set(this._element, this.constructor.DATA_KEY, this))
+            return e
+        },
+        getDataAttribute: (t, e) => j(t.getAttribute(`data-bs-${F(e)}`))
+    };
+    class $ {
+        static get Default() {
+            return {}
+        }
+        static get DefaultType() {
+            return {}
+        }
+        static get NAME() {
+            throw new Error('You have to implement the static method "NAME", for each component!')
+        }
+        _getConfig(t) {
+            return t = this._mergeConfigObj(t), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
+        }
+        _configAfterMerge(t) {
+            return t
+        }
+        _mergeConfigObj(t, e) {
+            const i = o(e) ? H.getDataAttribute(e, "config") : {};
+            return {
+                ...this.constructor.Default,
+                ..."object" == typeof i ? i : {},
+                ...o(e) ? H.getDataAttributes(e) : {},
+                ..."object" == typeof t ? t : {}
+            }
+        }
+        _typeCheckConfig(t, e = this.constructor.DefaultType) {
+            for (const [n, s] of Object.entries(e)) {
+                const e = t[n],
+                    r = o(e) ? "element" : null == (i = e) ? `${i}` : Object.prototype.toString.call(i).match(/\s([a-z]+)/i)[1].toLowerCase();
+                if (!new RegExp(s).test(r)) throw new TypeError(`${this.constructor.NAME.toUpperCase()}: Option "${n}" provided type "${r}" but expected type "${s}".`)
+            }
+            var i
+        }
+    }
+    class W extends $ {
+        constructor(t, i) {
+            super(), (t = r(t)) && (this._element = t, this._config = this._getConfig(i), e.set(this._element, this.constructor.DATA_KEY, this))
         }
         dispose() {
-            H.remove(this._element, this.constructor.DATA_KEY), j.off(this._element, this.constructor.EVENT_KEY), Object.getOwnPropertyNames(this).forEach((t => {
-                this[t] = null
-            }))
+            e.remove(this._element, this.constructor.DATA_KEY), P.off(this._element, this.constructor.EVENT_KEY);
+            for (const t of Object.getOwnPropertyNames(this)) this[t] = null
         }
         _queueCallback(t, e, i = !0) {
-            b(t, e, i)
+            _(t, e, i)
+        }
+        _getConfig(t) {
+            return t = this._mergeConfigObj(t, this._element), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
         }
         static getInstance(t) {
-            return H.get(r(t), this.DATA_KEY)
+            return e.get(r(t), this.DATA_KEY)
         }
         static getOrCreateInstance(t, e = {}) {
             return this.getInstance(t) || new this(t, "object" == typeof e ? e : null)
         }
         static get VERSION() {
-            return "5.1.3"
-        }
-        static get NAME() {
-            throw new Error('You have to implement the static method "NAME", for each component!')
+            return "5.3.0"
         }
         static get DATA_KEY() {
             return `bs.${this.NAME}`
         }
         static get EVENT_KEY() {
             return `.${this.DATA_KEY}`
         }
+        static eventName(t) {
+            return `${t}${this.EVENT_KEY}`
+        }
     }
-    const R = (t, e = "hide") => {
-        const i = `click.dismiss${t.EVENT_KEY}`,
-            s = t.NAME;
-        j.on(document, i, `[data-bs-dismiss="${s}"]`, (function(i) {
-            if (["A", "AREA"].includes(this.tagName) && i.preventDefault(), c(this)) return;
-            const o = n(this) || this.closest(`.${s}`);
-            t.getOrCreateInstance(o)[e]()
-        }))
-    };
-    class W extends B {
+    const B = t => {
+            let e = t.getAttribute("data-bs-target");
+            if (!e || "#" === e) {
+                let i = t.getAttribute("href");
+                if (!i || !i.includes("#") && !i.startsWith(".")) return null;
+                i.includes("#") && !i.startsWith("#") && (i = `#${i.split("#")[1]}`), e = i && "#" !== i ? i.trim() : null
+            }
+            return n(e)
+        },
+        z = {
+            find: (t, e = document.documentElement) => [].concat(...Element.prototype.querySelectorAll.call(e, t)),
+            findOne: (t, e = document.documentElement) => Element.prototype.querySelector.call(e, t),
+            children: (t, e) => [].concat(...t.children).filter((t => t.matches(e))),
+            parents(t, e) {
+                const i = [];
+                let n = t.parentNode.closest(e);
+                for (; n;) i.push(n), n = n.parentNode.closest(e);
+                return i
+            },
+            prev(t, e) {
+                let i = t.previousElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.previousElementSibling
+                }
+                return []
+            },
+            next(t, e) {
+                let i = t.nextElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.nextElementSibling
+                }
+                return []
+            },
+            focusableChildren(t) {
+                const e = ["a", "button", "input", "textarea", "select", "details", "[tabindex]", '[contenteditable="true"]'].map((t => `${t}:not([tabindex^="-"])`)).join(",");
+                return this.find(e, t).filter((t => !l(t) && a(t)))
+            },
+            getSelectorFromElement(t) {
+                const e = B(t);
+                return e && z.findOne(e) ? e : null
+            },
+            getElementFromSelector(t) {
+                const e = B(t);
+                return e ? z.findOne(e) : null
+            },
+            getMultipleElementsFromSelector(t) {
+                const e = B(t);
+                return e ? z.find(e) : []
+            }
+        },
+        R = (t, e = "hide") => {
+            const i = `click.dismiss${t.EVENT_KEY}`,
+                n = t.NAME;
+            P.on(document, i, `[data-bs-dismiss="${n}"]`, (function(i) {
+                if (["A", "AREA"].includes(this.tagName) && i.preventDefault(), l(this)) return;
+                const s = z.getElementFromSelector(this) || this.closest(`.${n}`);
+                t.getOrCreateInstance(s)[e]()
+            }))
+        };
+    class q extends W {
         static get NAME() {
             return "alert"
         }
         close() {
-            if (j.trigger(this._element, "close.bs.alert").defaultPrevented) return;
+            if (P.trigger(this._element, "close.bs.alert").defaultPrevented) return;
             this._element.classList.remove("show");
             const t = this._element.classList.contains("fade");
             this._queueCallback((() => this._destroyElement()), this._element, t)
         }
         _destroyElement() {
-            this._element.remove(), j.trigger(this._element, "closed.bs.alert"), this.dispose()
+            this._element.remove(), P.trigger(this._element, "closed.bs.alert"), this.dispose()
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = W.getOrCreateInstance(this);
+                const e = q.getOrCreateInstance(this);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    R(W, "close"), g(W);
-    const $ = '[data-bs-toggle="button"]';
-    class z extends B {
+    R(q, "close"), m(q);
+    const V = '[data-bs-toggle="button"]';
+    class K extends W {
         static get NAME() {
             return "button"
         }
         toggle() {
             this._element.setAttribute("aria-pressed", this._element.classList.toggle("active"))
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = z.getOrCreateInstance(this);
+                const e = K.getOrCreateInstance(this);
                 "toggle" === t && e[t]()
             }))
         }
     }
-
-    function q(t) {
-        return "true" === t || "false" !== t && (t === Number(t).toString() ? Number(t) : "" === t || "null" === t ? null : t)
-    }
-
-    function F(t) {
-        return t.replace(/[A-Z]/g, (t => `-${t.toLowerCase()}`))
-    }
-    j.on(document, "click.bs.button.data-api", $, (t => {
+    P.on(document, "click.bs.button.data-api", V, (t => {
         t.preventDefault();
-        const e = t.target.closest($);
-        z.getOrCreateInstance(e).toggle()
-    })), g(z);
-    const U = {
-            setDataAttribute(t, e, i) {
-                t.setAttribute(`data-bs-${F(e)}`, i)
-            },
-            removeDataAttribute(t, e) {
-                t.removeAttribute(`data-bs-${F(e)}`)
-            },
-            getDataAttributes(t) {
-                if (!t) return {};
-                const e = {};
-                return Object.keys(t.dataset).filter((t => t.startsWith("bs"))).forEach((i => {
-                    let n = i.replace(/^bs/, "");
-                    n = n.charAt(0).toLowerCase() + n.slice(1, n.length), e[n] = q(t.dataset[i])
-                })), e
-            },
-            getDataAttribute: (t, e) => q(t.getAttribute(`data-bs-${F(e)}`)),
-            offset(t) {
-                const e = t.getBoundingClientRect();
-                return {
-                    top: e.top + window.pageYOffset,
-                    left: e.left + window.pageXOffset
-                }
-            },
-            position: t => ({
-                top: t.offsetTop,
-                left: t.offsetLeft
-            })
+        const e = t.target.closest(V);
+        K.getOrCreateInstance(e).toggle()
+    })), m(K);
+    const Q = {
+            endCallback: null,
+            leftCallback: null,
+            rightCallback: null
         },
-        V = {
-            find: (t, e = document.documentElement) => [].concat(...Element.prototype.querySelectorAll.call(e, t)),
-            findOne: (t, e = document.documentElement) => Element.prototype.querySelector.call(e, t),
-            children: (t, e) => [].concat(...t.children).filter((t => t.matches(e))),
-            parents(t, e) {
-                const i = [];
-                let n = t.parentNode;
-                for (; n && n.nodeType === Node.ELEMENT_NODE && 3 !== n.nodeType;) n.matches(e) && i.push(n), n = n.parentNode;
-                return i
-            },
-            prev(t, e) {
-                let i = t.previousElementSibling;
-                for (; i;) {
-                    if (i.matches(e)) return [i];
-                    i = i.previousElementSibling
-                }
-                return []
-            },
-            next(t, e) {
-                let i = t.nextElementSibling;
-                for (; i;) {
-                    if (i.matches(e)) return [i];
-                    i = i.nextElementSibling
-                }
-                return []
-            },
-            focusableChildren(t) {
-                const e = ["a", "button", "input", "textarea", "select", "details", "[tabindex]", '[contenteditable="true"]'].map((t => `${t}:not([tabindex^="-"])`)).join(", ");
-                return this.find(e, t).filter((t => !c(t) && l(t)))
-            }
-        },
-        K = "carousel",
         X = {
+            endCallback: "(function|null)",
+            leftCallback: "(function|null)",
+            rightCallback: "(function|null)"
+        };
+    class Y extends $ {
+        constructor(t, e) {
+            super(), this._element = t, t && Y.isSupported() && (this._config = this._getConfig(e), this._deltaX = 0, this._supportPointerEvents = Boolean(window.PointerEvent), this._initEvents())
+        }
+        static get Default() {
+            return Q
+        }
+        static get DefaultType() {
+            return X
+        }
+        static get NAME() {
+            return "swipe"
+        }
+        dispose() {
+            P.off(this._element, ".bs.swipe")
+        }
+        _start(t) {
+            this._supportPointerEvents ? this._eventIsPointerPenTouch(t) && (this._deltaX = t.clientX) : this._deltaX = t.touches[0].clientX
+        }
+        _end(t) {
+            this._eventIsPointerPenTouch(t) && (this._deltaX = t.clientX - this._deltaX), this._handleSwipe(), g(this._config.endCallback)
+        }
+        _move(t) {
+            this._deltaX = t.touches && t.touches.length > 1 ? 0 : t.touches[0].clientX - this._deltaX
+        }
+        _handleSwipe() {
+            const t = Math.abs(this._deltaX);
+            if (t <= 40) return;
+            const e = t / this._deltaX;
+            this._deltaX = 0, e && g(e > 0 ? this._config.rightCallback : this._config.leftCallback)
+        }
+        _initEvents() {
+            this._supportPointerEvents ? (P.on(this._element, "pointerdown.bs.swipe", (t => this._start(t))), P.on(this._element, "pointerup.bs.swipe", (t => this._end(t))), this._element.classList.add("pointer-event")) : (P.on(this._element, "touchstart.bs.swipe", (t => this._start(t))), P.on(this._element, "touchmove.bs.swipe", (t => this._move(t))), P.on(this._element, "touchend.bs.swipe", (t => this._end(t))))
+        }
+        _eventIsPointerPenTouch(t) {
+            return this._supportPointerEvents && ("pen" === t.pointerType || "touch" === t.pointerType)
+        }
+        static isSupported() {
+            return "ontouchstart" in document.documentElement || navigator.maxTouchPoints > 0
+        }
+    }
+    const U = "next",
+        G = "prev",
+        J = "left",
+        Z = "right",
+        tt = "slid.bs.carousel",
+        et = "carousel",
+        it = "active",
+        nt = {
+            ArrowLeft: Z,
+            ArrowRight: J
+        },
+        st = {
             interval: 5e3,
             keyboard: !0,
-            slide: !1,
             pause: "hover",
-            wrap: !0,
-            touch: !0
+            ride: !1,
+            touch: !0,
+            wrap: !0
         },
-        Y = {
+        ot = {
             interval: "(number|boolean)",
             keyboard: "boolean",
-            slide: "(boolean|string)",
             pause: "(string|boolean)",
-            wrap: "boolean",
-            touch: "boolean"
-        },
-        Q = "next",
-        G = "prev",
-        Z = "left",
-        J = "right",
-        tt = {
-            ArrowLeft: J,
-            ArrowRight: Z
-        },
-        et = "slid.bs.carousel",
-        it = "active",
-        nt = ".active.carousel-item";
-    class st extends B {
+            ride: "(boolean|string)",
+            touch: "boolean",
+            wrap: "boolean"
+        };
+    class rt extends W {
         constructor(t, e) {
-            super(t), this._items = null, this._interval = null, this._activeElement = null, this._isPaused = !1, this._isSliding = !1, this.touchTimeout = null, this.touchStartX = 0, this.touchDeltaX = 0, this._config = this._getConfig(e), this._indicatorsElement = V.findOne(".carousel-indicators", this._element), this._touchSupported = "ontouchstart" in document.documentElement || navigator.maxTouchPoints > 0, this._pointerEvent = Boolean(window.PointerEvent), this._addEventListeners()
+            super(t, e), this._interval = null, this._activeElement = null, this._isSliding = !1, this.touchTimeout = null, this._swipeHelper = null, this._indicatorsElement = z.findOne(".carousel-indicators", this._element), this._addEventListeners(), this._config.ride === et && this.cycle()
         }
         static get Default() {
-            return X
+            return st
+        }
+        static get DefaultType() {
+            return ot
         }
         static get NAME() {
-            return K
+            return "carousel"
         }
         next() {
-            this._slide(Q)
+            this._slide(U)
         }
         nextWhenVisible() {
-            !document.hidden && l(this._element) && this.next()
+            !document.hidden && a(this._element) && this.next()
         }
         prev() {
             this._slide(G)
         }
-        pause(t) {
-            t || (this._isPaused = !0), V.findOne(".carousel-item-next, .carousel-item-prev", this._element) && (s(this._element), this.cycle(!0)), clearInterval(this._interval), this._interval = null
+        pause() {
+            this._isSliding && s(this._element), this._clearInterval()
+        }
+        cycle() {
+            this._clearInterval(), this._updateInterval(), this._interval = setInterval((() => this.nextWhenVisible()), this._config.interval)
         }
-        cycle(t) {
-            t || (this._isPaused = !1), this._interval && (clearInterval(this._interval), this._interval = null), this._config && this._config.interval && !this._isPaused && (this._updateInterval(), this._interval = setInterval((document.visibilityState ? this.nextWhenVisible : this.next).bind(this), this._config.interval))
+        _maybeEnableCycle() {
+            this._config.ride && (this._isSliding ? P.one(this._element, tt, (() => this.cycle())) : this.cycle())
         }
         to(t) {
-            this._activeElement = V.findOne(nt, this._element);
-            const e = this._getItemIndex(this._activeElement);
-            if (t > this._items.length - 1 || t < 0) return;
-            if (this._isSliding) return void j.one(this._element, et, (() => this.to(t)));
-            if (e === t) return this.pause(), void this.cycle();
-            const i = t > e ? Q : G;
-            this._slide(i, this._items[t])
+            const e = this._getItems();
+            if (t > e.length - 1 || t < 0) return;
+            if (this._isSliding) return void P.one(this._element, tt, (() => this.to(t)));
+            const i = this._getItemIndex(this._getActive());
+            if (i === t) return;
+            const n = t > i ? U : G;
+            this._slide(n, e[t])
         }
-        _getConfig(t) {
-            return t = {
-                ...X,
-                ...U.getDataAttributes(this._element),
-                ..."object" == typeof t ? t : {}
-            }, a(K, t, Y), t
+        dispose() {
+            this._swipeHelper && this._swipeHelper.dispose(), super.dispose()
         }
-        _handleSwipe() {
-            const t = Math.abs(this.touchDeltaX);
-            if (t <= 40) return;
-            const e = t / this.touchDeltaX;
-            this.touchDeltaX = 0, e && this._slide(e > 0 ? J : Z)
+        _configAfterMerge(t) {
+            return t.defaultInterval = t.interval, t
         }
         _addEventListeners() {
-            this._config.keyboard && j.on(this._element, "keydown.bs.carousel", (t => this._keydown(t))), "hover" === this._config.pause && (j.on(this._element, "mouseenter.bs.carousel", (t => this.pause(t))), j.on(this._element, "mouseleave.bs.carousel", (t => this.cycle(t)))), this._config.touch && this._touchSupported && this._addTouchEventListeners()
+            this._config.keyboard && P.on(this._element, "keydown.bs.carousel", (t => this._keydown(t))), "hover" === this._config.pause && (P.on(this._element, "mouseenter.bs.carousel", (() => this.pause())), P.on(this._element, "mouseleave.bs.carousel", (() => this._maybeEnableCycle()))), this._config.touch && Y.isSupported() && this._addTouchEventListeners()
         }
         _addTouchEventListeners() {
-            const t = t => this._pointerEvent && ("pen" === t.pointerType || "touch" === t.pointerType),
-                e = e => {
-                    t(e) ? this.touchStartX = e.clientX : this._pointerEvent || (this.touchStartX = e.touches[0].clientX)
-                },
-                i = t => {
-                    this.touchDeltaX = t.touches && t.touches.length > 1 ? 0 : t.touches[0].clientX - this.touchStartX
-                },
-                n = e => {
-                    t(e) && (this.touchDeltaX = e.clientX - this.touchStartX), this._handleSwipe(), "hover" === this._config.pause && (this.pause(), this.touchTimeout && clearTimeout(this.touchTimeout), this.touchTimeout = setTimeout((t => this.cycle(t)), 500 + this._config.interval))
-                };
-            V.find(".carousel-item img", this._element).forEach((t => {
-                j.on(t, "dragstart.bs.carousel", (t => t.preventDefault()))
-            })), this._pointerEvent ? (j.on(this._element, "pointerdown.bs.carousel", (t => e(t))), j.on(this._element, "pointerup.bs.carousel", (t => n(t))), this._element.classList.add("pointer-event")) : (j.on(this._element, "touchstart.bs.carousel", (t => e(t))), j.on(this._element, "touchmove.bs.carousel", (t => i(t))), j.on(this._element, "touchend.bs.carousel", (t => n(t))))
+            for (const t of z.find(".carousel-item img", this._element)) P.on(t, "dragstart.bs.carousel", (t => t.preventDefault()));
+            const t = {
+                leftCallback: () => this._slide(this._directionToOrder(J)),
+                rightCallback: () => this._slide(this._directionToOrder(Z)),
+                endCallback: () => {
+                    "hover" === this._config.pause && (this.pause(), this.touchTimeout && clearTimeout(this.touchTimeout), this.touchTimeout = setTimeout((() => this._maybeEnableCycle()), 500 + this._config.interval))
+                }
+            };
+            this._swipeHelper = new Y(this._element, t)
         }
         _keydown(t) {
             if (/input|textarea/i.test(t.target.tagName)) return;
-            const e = tt[t.key];
-            e && (t.preventDefault(), this._slide(e))
+            const e = nt[t.key];
+            e && (t.preventDefault(), this._slide(this._directionToOrder(e)))
         }
         _getItemIndex(t) {
-            return this._items = t && t.parentNode ? V.find(".carousel-item", t.parentNode) : [], this._items.indexOf(t)
-        }
-        _getItemByOrder(t, e) {
-            const i = t === Q;
-            return v(this._items, e, i, this._config.wrap)
-        }
-        _triggerSlideEvent(t, e) {
-            const i = this._getItemIndex(t),
-                n = this._getItemIndex(V.findOne(nt, this._element));
-            return j.trigger(this._element, "slide.bs.carousel", {
-                relatedTarget: t,
-                direction: e,
-                from: n,
-                to: i
-            })
+            return this._getItems().indexOf(t)
         }
         _setActiveIndicatorElement(t) {
-            if (this._indicatorsElement) {
-                const e = V.findOne(".active", this._indicatorsElement);
-                e.classList.remove(it), e.removeAttribute("aria-current");
-                const i = V.find("[data-bs-target]", this._indicatorsElement);
-                for (let e = 0; e < i.length; e++)
-                    if (Number.parseInt(i[e].getAttribute("data-bs-slide-to"), 10) === this._getItemIndex(t)) {
-                        i[e].classList.add(it), i[e].setAttribute("aria-current", "true");
-                        break
-                    }
-            }
+            if (!this._indicatorsElement) return;
+            const e = z.findOne(".active", this._indicatorsElement);
+            e.classList.remove(it), e.removeAttribute("aria-current");
+            const i = z.findOne(`[data-bs-slide-to="${t}"]`, this._indicatorsElement);
+            i && (i.classList.add(it), i.setAttribute("aria-current", "true"))
         }
         _updateInterval() {
-            const t = this._activeElement || V.findOne(nt, this._element);
+            const t = this._activeElement || this._getActive();
             if (!t) return;
             const e = Number.parseInt(t.getAttribute("data-bs-interval"), 10);
-            e ? (this._config.defaultInterval = this._config.defaultInterval || this._config.interval, this._config.interval = e) : this._config.interval = this._config.defaultInterval || this._config.interval
+            this._config.interval = e || this._config.defaultInterval
         }
-        _slide(t, e) {
-            const i = this._directionToOrder(t),
-                n = V.findOne(nt, this._element),
-                s = this._getItemIndex(n),
-                o = e || this._getItemByOrder(i, n),
-                r = this._getItemIndex(o),
-                a = Boolean(this._interval),
-                l = i === Q,
-                c = l ? "carousel-item-start" : "carousel-item-end",
-                h = l ? "carousel-item-next" : "carousel-item-prev",
-                d = this._orderToDirection(i);
-            if (o && o.classList.contains(it)) return void(this._isSliding = !1);
+        _slide(t, e = null) {
             if (this._isSliding) return;
-            if (this._triggerSlideEvent(o, d).defaultPrevented) return;
-            if (!n || !o) return;
-            this._isSliding = !0, a && this.pause(), this._setActiveIndicatorElement(o), this._activeElement = o;
-            const f = () => {
-                j.trigger(this._element, et, {
-                    relatedTarget: o,
-                    direction: d,
-                    from: s,
-                    to: r
-                })
-            };
-            if (this._element.classList.contains("slide")) {
-                o.classList.add(h), u(o), n.classList.add(c), o.classList.add(c);
-                const t = () => {
-                    o.classList.remove(c, h), o.classList.add(it), n.classList.remove(it, h, c), this._isSliding = !1, setTimeout(f, 0)
-                };
-                this._queueCallback(t, n, !0)
-            } else n.classList.remove(it), o.classList.add(it), this._isSliding = !1, f();
-            a && this.cycle()
+            const i = this._getActive(),
+                n = t === U,
+                s = e || b(this._getItems(), i, n, this._config.wrap);
+            if (s === i) return;
+            const o = this._getItemIndex(s),
+                r = e => P.trigger(this._element, e, {
+                    relatedTarget: s,
+                    direction: this._orderToDirection(t),
+                    from: this._getItemIndex(i),
+                    to: o
+                });
+            if (r("slide.bs.carousel").defaultPrevented) return;
+            if (!i || !s) return;
+            const a = Boolean(this._interval);
+            this.pause(), this._isSliding = !0, this._setActiveIndicatorElement(o), this._activeElement = s;
+            const l = n ? "carousel-item-start" : "carousel-item-end",
+                c = n ? "carousel-item-next" : "carousel-item-prev";
+            s.classList.add(c), d(s), i.classList.add(l), s.classList.add(l), this._queueCallback((() => {
+                s.classList.remove(l, c), s.classList.add(it), i.classList.remove(it, c, l), this._isSliding = !1, r(tt)
+            }), i, this._isAnimated()), a && this.cycle()
+        }
+        _isAnimated() {
+            return this._element.classList.contains("slide")
+        }
+        _getActive() {
+            return z.findOne(".active.carousel-item", this._element)
+        }
+        _getItems() {
+            return z.find(".carousel-item", this._element)
+        }
+        _clearInterval() {
+            this._interval && (clearInterval(this._interval), this._interval = null)
         }
         _directionToOrder(t) {
-            return [J, Z].includes(t) ? m() ? t === Z ? G : Q : t === Z ? Q : G : t
+            return p() ? t === J ? G : U : t === J ? U : G
         }
         _orderToDirection(t) {
-            return [Q, G].includes(t) ? m() ? t === G ? Z : J : t === G ? J : Z : t
-        }
-        static carouselInterface(t, e) {
-            const i = st.getOrCreateInstance(t, e);
-            let {
-                _config: n
-            } = i;
-            "object" == typeof e && (n = {
-                ...n,
-                ...e
-            });
-            const s = "string" == typeof e ? e : n.slide;
-            if ("number" == typeof e) i.to(e);
-            else if ("string" == typeof s) {
-                if (void 0 === i[s]) throw new TypeError(`No method named "${s}"`);
-                i[s]()
-            } else n.interval && n.ride && (i.pause(), i.cycle())
+            return p() ? t === G ? J : Z : t === G ? Z : J
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                st.carouselInterface(this, t)
+                const e = rt.getOrCreateInstance(this, t);
+                if ("number" != typeof t) {
+                    if ("string" == typeof t) {
+                        if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
+                        e[t]()
+                    }
+                } else e.to(t)
             }))
         }
-        static dataApiClickHandler(t) {
-            const e = n(this);
-            if (!e || !e.classList.contains("carousel")) return;
-            const i = {
-                    ...U.getDataAttributes(e),
-                    ...U.getDataAttributes(this)
-                },
-                s = this.getAttribute("data-bs-slide-to");
-            s && (i.interval = !1), st.carouselInterface(e, i), s && st.getInstance(e).to(s), t.preventDefault()
-        }
     }
-    j.on(document, "click.bs.carousel.data-api", "[data-bs-slide], [data-bs-slide-to]", st.dataApiClickHandler), j.on(window, "load.bs.carousel.data-api", (() => {
-        const t = V.find('[data-bs-ride="carousel"]');
-        for (let e = 0, i = t.length; e < i; e++) st.carouselInterface(t[e], st.getInstance(t[e]))
-    })), g(st);
-    const ot = "collapse",
-        rt = {
-            toggle: !0,
-            parent: null
-        },
-        at = {
-            toggle: "boolean",
-            parent: "(null|element)"
-        },
-        lt = "show",
-        ct = "collapse",
-        ht = "collapsing",
-        dt = "collapsed",
-        ut = ":scope .collapse .collapse",
-        ft = '[data-bs-toggle="collapse"]';
-    class pt extends B {
+    P.on(document, "click.bs.carousel.data-api", "[data-bs-slide], [data-bs-slide-to]", (function(t) {
+        const e = z.getElementFromSelector(this);
+        if (!e || !e.classList.contains(et)) return;
+        t.preventDefault();
+        const i = rt.getOrCreateInstance(e),
+            n = this.getAttribute("data-bs-slide-to");
+        return n ? (i.to(n), void i._maybeEnableCycle()) : "next" === H.getDataAttribute(this, "slide") ? (i.next(), void i._maybeEnableCycle()) : (i.prev(), void i._maybeEnableCycle())
+    })), P.on(window, "load.bs.carousel.data-api", (() => {
+        const t = z.find('[data-bs-ride="carousel"]');
+        for (const e of t) rt.getOrCreateInstance(e)
+    })), m(rt);
+    const at = "show",
+        lt = "collapse",
+        ct = "collapsing",
+        ht = '[data-bs-toggle="collapse"]',
+        dt = {
+            parent: null,
+            toggle: !0
+        },
+        ut = {
+            parent: "(null|element)",
+            toggle: "boolean"
+        };
+    class ft extends W {
         constructor(t, e) {
-            super(t), this._isTransitioning = !1, this._config = this._getConfig(e), this._triggerArray = [];
-            const n = V.find(ft);
-            for (let t = 0, e = n.length; t < e; t++) {
-                const e = n[t],
-                    s = i(e),
-                    o = V.find(s).filter((t => t === this._element));
-                null !== s && o.length && (this._selector = s, this._triggerArray.push(e))
+            super(t, e), this._isTransitioning = !1, this._triggerArray = [];
+            const i = z.find(ht);
+            for (const t of i) {
+                const e = z.getSelectorFromElement(t),
+                    i = z.find(e).filter((t => t === this._element));
+                null !== e && i.length && this._triggerArray.push(t)
             }
             this._initializeChildren(), this._config.parent || this._addAriaAndCollapsedClass(this._triggerArray, this._isShown()), this._config.toggle && this.toggle()
         }
         static get Default() {
-            return rt
+            return dt
+        }
+        static get DefaultType() {
+            return ut
         }
         static get NAME() {
-            return ot
+            return "collapse"
         }
         toggle() {
             this._isShown() ? this.hide() : this.show()
         }
         show() {
             if (this._isTransitioning || this._isShown()) return;
-            let t, e = [];
-            if (this._config.parent) {
-                const t = V.find(ut, this._config.parent);
-                e = V.find(".collapse.show, .collapse.collapsing", this._config.parent).filter((e => !t.includes(e)))
-            }
-            const i = V.findOne(this._selector);
-            if (e.length) {
-                const n = e.find((t => i !== t));
-                if (t = n ? pt.getInstance(n) : null, t && t._isTransitioning) return
-            }
-            if (j.trigger(this._element, "show.bs.collapse").defaultPrevented) return;
-            e.forEach((e => {
-                i !== e && pt.getOrCreateInstance(e, {
+            let t = [];
+            if (this._config.parent && (t = this._getFirstLevelChildren(".collapse.show, .collapse.collapsing").filter((t => t !== this._element)).map((t => ft.getOrCreateInstance(t, {
                     toggle: !1
-                }).hide(), t || H.set(e, "bs.collapse", null)
-            }));
-            const n = this._getDimension();
-            this._element.classList.remove(ct), this._element.classList.add(ht), this._element.style[n] = 0, this._addAriaAndCollapsedClass(this._triggerArray, !0), this._isTransitioning = !0;
-            const s = `scroll${n[0].toUpperCase()+n.slice(1)}`;
+                })))), t.length && t[0]._isTransitioning) return;
+            if (P.trigger(this._element, "show.bs.collapse").defaultPrevented) return;
+            for (const e of t) e.hide();
+            const e = this._getDimension();
+            this._element.classList.remove(lt), this._element.classList.add(ct), this._element.style[e] = 0, this._addAriaAndCollapsedClass(this._triggerArray, !0), this._isTransitioning = !0;
+            const i = `scroll${e[0].toUpperCase()+e.slice(1)}`;
             this._queueCallback((() => {
-                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct, lt), this._element.style[n] = "", j.trigger(this._element, "shown.bs.collapse")
-            }), this._element, !0), this._element.style[n] = `${this._element[s]}px`
+                this._isTransitioning = !1, this._element.classList.remove(ct), this._element.classList.add(lt, at), this._element.style[e] = "", P.trigger(this._element, "shown.bs.collapse")
+            }), this._element, !0), this._element.style[e] = `${this._element[i]}px`
         }
         hide() {
             if (this._isTransitioning || !this._isShown()) return;
-            if (j.trigger(this._element, "hide.bs.collapse").defaultPrevented) return;
+            if (P.trigger(this._element, "hide.bs.collapse").defaultPrevented) return;
             const t = this._getDimension();
-            this._element.style[t] = `${this._element.getBoundingClientRect()[t]}px`, u(this._element), this._element.classList.add(ht), this._element.classList.remove(ct, lt);
-            const e = this._triggerArray.length;
-            for (let t = 0; t < e; t++) {
-                const e = this._triggerArray[t],
-                    i = n(e);
-                i && !this._isShown(i) && this._addAriaAndCollapsedClass([e], !1)
+            this._element.style[t] = `${this._element.getBoundingClientRect()[t]}px`, d(this._element), this._element.classList.add(ct), this._element.classList.remove(lt, at);
+            for (const t of this._triggerArray) {
+                const e = z.getElementFromSelector(t);
+                e && !this._isShown(e) && this._addAriaAndCollapsedClass([t], !1)
             }
             this._isTransitioning = !0, this._element.style[t] = "", this._queueCallback((() => {
-                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct), j.trigger(this._element, "hidden.bs.collapse")
+                this._isTransitioning = !1, this._element.classList.remove(ct), this._element.classList.add(lt), P.trigger(this._element, "hidden.bs.collapse")
             }), this._element, !0)
         }
         _isShown(t = this._element) {
-            return t.classList.contains(lt)
+            return t.classList.contains(at)
         }
-        _getConfig(t) {
-            return (t = {
-                ...rt,
-                ...U.getDataAttributes(this._element),
-                ...t
-            }).toggle = Boolean(t.toggle), t.parent = r(t.parent), a(ot, t, at), t
+        _configAfterMerge(t) {
+            return t.toggle = Boolean(t.toggle), t.parent = r(t.parent), t
         }
         _getDimension() {
             return this._element.classList.contains("collapse-horizontal") ? "width" : "height"
         }
         _initializeChildren() {
             if (!this._config.parent) return;
-            const t = V.find(ut, this._config.parent);
-            V.find(ft, this._config.parent).filter((e => !t.includes(e))).forEach((t => {
-                const e = n(t);
-                e && this._addAriaAndCollapsedClass([t], this._isShown(e))
-            }))
+            const t = this._getFirstLevelChildren(ht);
+            for (const e of t) {
+                const t = z.getElementFromSelector(e);
+                t && this._addAriaAndCollapsedClass([e], this._isShown(t))
+            }
+        }
+        _getFirstLevelChildren(t) {
+            const e = z.find(":scope .collapse .collapse", this._config.parent);
+            return z.find(t, this._config.parent).filter((t => !e.includes(t)))
         }
         _addAriaAndCollapsedClass(t, e) {
-            t.length && t.forEach((t => {
-                e ? t.classList.remove(dt) : t.classList.add(dt), t.setAttribute("aria-expanded", e)
-            }))
+            if (t.length)
+                for (const i of t) i.classList.toggle("collapsed", !e), i.setAttribute("aria-expanded", e)
         }
         static jQueryInterface(t) {
-            return this.each((function() {
-                const e = {};
-                "string" == typeof t && /show|hide/.test(t) && (e.toggle = !1);
-                const i = pt.getOrCreateInstance(this, e);
+            const e = {};
+            return "string" == typeof t && /show|hide/.test(t) && (e.toggle = !1), this.each((function() {
+                const i = ft.getOrCreateInstance(this, e);
                 if ("string" == typeof t) {
                     if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
                     i[t]()
                 }
             }))
         }
     }
-    j.on(document, "click.bs.collapse.data-api", ft, (function(t) {
+    P.on(document, "click.bs.collapse.data-api", ht, (function(t) {
         ("A" === t.target.tagName || t.delegateTarget && "A" === t.delegateTarget.tagName) && t.preventDefault();
-        const e = i(this);
-        V.find(e).forEach((t => {
-            pt.getOrCreateInstance(t, {
-                toggle: !1
-            }).toggle()
-        }))
-    })), g(pt);
-    var mt = "top",
-        gt = "bottom",
-        _t = "right",
-        bt = "left",
-        vt = "auto",
-        yt = [mt, gt, _t, bt],
-        wt = "start",
-        Et = "end",
+        for (const t of z.getMultipleElementsFromSelector(this)) ft.getOrCreateInstance(t, {
+            toggle: !1
+        }).toggle()
+    })), m(ft);
+    var pt = "top",
+        mt = "bottom",
+        gt = "right",
+        _t = "left",
+        bt = "auto",
+        vt = [pt, mt, gt, _t],
+        yt = "start",
+        wt = "end",
         At = "clippingParents",
-        Tt = "viewport",
-        Ot = "popper",
+        Et = "viewport",
+        Tt = "popper",
         Ct = "reference",
-        kt = yt.reduce((function(t, e) {
-            return t.concat([e + "-" + wt, e + "-" + Et])
+        Ot = vt.reduce((function(t, e) {
+            return t.concat([e + "-" + yt, e + "-" + wt])
         }), []),
-        Lt = [].concat(yt, [vt]).reduce((function(t, e) {
-            return t.concat([e, e + "-" + wt, e + "-" + Et])
+        xt = [].concat(vt, [bt]).reduce((function(t, e) {
+            return t.concat([e, e + "-" + yt, e + "-" + wt])
         }), []),
-        xt = "beforeRead",
-        Dt = "read",
+        kt = "beforeRead",
+        Lt = "read",
         St = "afterRead",
-        Nt = "beforeMain",
+        Dt = "beforeMain",
         It = "main",
-        Pt = "afterMain",
-        jt = "beforeWrite",
+        Nt = "afterMain",
+        Pt = "beforeWrite",
         Mt = "write",
-        Ht = "afterWrite",
-        Bt = [xt, Dt, St, Nt, It, Pt, jt, Mt, Ht];
+        jt = "afterWrite",
+        Ft = [kt, Lt, St, Dt, It, Nt, Pt, Mt, jt];
 
-    function Rt(t) {
+    function Ht(t) {
         return t ? (t.nodeName || "").toLowerCase() : null
     }
 
-    function Wt(t) {
+    function $t(t) {
         if (null == t) return window;
         if ("[object Window]" !== t.toString()) {
             var e = t.ownerDocument;
             return e && e.defaultView || window
         }
         return t
     }
 
-    function $t(t) {
-        return t instanceof Wt(t).Element || t instanceof Element
+    function Wt(t) {
+        return t instanceof $t(t).Element || t instanceof Element
     }
 
-    function zt(t) {
-        return t instanceof Wt(t).HTMLElement || t instanceof HTMLElement
+    function Bt(t) {
+        return t instanceof $t(t).HTMLElement || t instanceof HTMLElement
     }
 
-    function qt(t) {
-        return "undefined" != typeof ShadowRoot && (t instanceof Wt(t).ShadowRoot || t instanceof ShadowRoot)
+    function zt(t) {
+        return "undefined" != typeof ShadowRoot && (t instanceof $t(t).ShadowRoot || t instanceof ShadowRoot)
     }
-    const Ft = {
+    const Rt = {
         name: "applyStyles",
         enabled: !0,
         phase: "write",
         fn: function(t) {
             var e = t.state;
             Object.keys(e.elements).forEach((function(t) {
                 var i = e.styles[t] || {},
                     n = e.attributes[t] || {},
                     s = e.elements[t];
-                zt(s) && Rt(s) && (Object.assign(s.style, i), Object.keys(n).forEach((function(t) {
+                Bt(s) && Ht(s) && (Object.assign(s.style, i), Object.keys(n).forEach((function(t) {
                     var e = n[t];
                     !1 === e ? s.removeAttribute(t) : s.setAttribute(t, !0 === e ? "" : e)
                 })))
             }))
         },
         effect: function(t) {
             var e = t.state,
@@ -816,588 +848,633 @@
                 function() {
                     Object.keys(e.elements).forEach((function(t) {
                         var n = e.elements[t],
                             s = e.attributes[t] || {},
                             o = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : i[t]).reduce((function(t, e) {
                                 return t[e] = "", t
                             }), {});
-                        zt(n) && Rt(n) && (Object.assign(n.style, o), Object.keys(s).forEach((function(t) {
+                        Bt(n) && Ht(n) && (Object.assign(n.style, o), Object.keys(s).forEach((function(t) {
                             n.removeAttribute(t)
                         })))
                     }))
                 }
         },
         requires: ["computeStyles"]
     };
 
-    function Ut(t) {
+    function qt(t) {
         return t.split("-")[0]
     }
-
-    function Vt(t, e) {
-        var i = t.getBoundingClientRect();
+    var Vt = Math.max,
+        Kt = Math.min,
+        Qt = Math.round;
+
+    function Xt() {
+        var t = navigator.userAgentData;
+        return null != t && t.brands && Array.isArray(t.brands) ? t.brands.map((function(t) {
+            return t.brand + "/" + t.version
+        })).join(" ") : navigator.userAgent
+    }
+
+    function Yt() {
+        return !/^((?!chrome|android).)*safari/i.test(Xt())
+    }
+
+    function Ut(t, e, i) {
+        void 0 === e && (e = !1), void 0 === i && (i = !1);
+        var n = t.getBoundingClientRect(),
+            s = 1,
+            o = 1;
+        e && Bt(t) && (s = t.offsetWidth > 0 && Qt(n.width) / t.offsetWidth || 1, o = t.offsetHeight > 0 && Qt(n.height) / t.offsetHeight || 1);
+        var r = (Wt(t) ? $t(t) : window).visualViewport,
+            a = !Yt() && i,
+            l = (n.left + (a && r ? r.offsetLeft : 0)) / s,
+            c = (n.top + (a && r ? r.offsetTop : 0)) / o,
+            h = n.width / s,
+            d = n.height / o;
         return {
-            width: i.width / 1,
-            height: i.height / 1,
-            top: i.top / 1,
-            right: i.right / 1,
-            bottom: i.bottom / 1,
-            left: i.left / 1,
-            x: i.left / 1,
-            y: i.top / 1
+            width: h,
+            height: d,
+            top: c,
+            right: l + h,
+            bottom: c + d,
+            left: l,
+            x: l,
+            y: c
         }
     }
 
-    function Kt(t) {
-        var e = Vt(t),
+    function Gt(t) {
+        var e = Ut(t),
             i = t.offsetWidth,
             n = t.offsetHeight;
         return Math.abs(e.width - i) <= 1 && (i = e.width), Math.abs(e.height - n) <= 1 && (n = e.height), {
             x: t.offsetLeft,
             y: t.offsetTop,
             width: i,
             height: n
         }
     }
 
-    function Xt(t, e) {
+    function Jt(t, e) {
         var i = e.getRootNode && e.getRootNode();
         if (t.contains(e)) return !0;
-        if (i && qt(i)) {
+        if (i && zt(i)) {
             var n = e;
             do {
                 if (n && t.isSameNode(n)) return !0;
                 n = n.parentNode || n.host
             } while (n)
         }
         return !1
     }
 
-    function Yt(t) {
-        return Wt(t).getComputedStyle(t)
+    function Zt(t) {
+        return $t(t).getComputedStyle(t)
     }
 
-    function Qt(t) {
-        return ["table", "td", "th"].indexOf(Rt(t)) >= 0
+    function te(t) {
+        return ["table", "td", "th"].indexOf(Ht(t)) >= 0
     }
 
-    function Gt(t) {
-        return (($t(t) ? t.ownerDocument : t.document) || window.document).documentElement
+    function ee(t) {
+        return ((Wt(t) ? t.ownerDocument : t.document) || window.document).documentElement
     }
 
-    function Zt(t) {
-        return "html" === Rt(t) ? t : t.assignedSlot || t.parentNode || (qt(t) ? t.host : null) || Gt(t)
+    function ie(t) {
+        return "html" === Ht(t) ? t : t.assignedSlot || t.parentNode || (zt(t) ? t.host : null) || ee(t)
     }
 
-    function Jt(t) {
-        return zt(t) && "fixed" !== Yt(t).position ? t.offsetParent : null
+    function ne(t) {
+        return Bt(t) && "fixed" !== Zt(t).position ? t.offsetParent : null
     }
 
-    function te(t) {
-        for (var e = Wt(t), i = Jt(t); i && Qt(i) && "static" === Yt(i).position;) i = Jt(i);
-        return i && ("html" === Rt(i) || "body" === Rt(i) && "static" === Yt(i).position) ? e : i || function(t) {
-            var e = -1 !== navigator.userAgent.toLowerCase().indexOf("firefox");
-            if (-1 !== navigator.userAgent.indexOf("Trident") && zt(t) && "fixed" === Yt(t).position) return null;
-            for (var i = Zt(t); zt(i) && ["html", "body"].indexOf(Rt(i)) < 0;) {
-                var n = Yt(i);
+    function se(t) {
+        for (var e = $t(t), i = ne(t); i && te(i) && "static" === Zt(i).position;) i = ne(i);
+        return i && ("html" === Ht(i) || "body" === Ht(i) && "static" === Zt(i).position) ? e : i || function(t) {
+            var e = /firefox/i.test(Xt());
+            if (/Trident/i.test(Xt()) && Bt(t) && "fixed" === Zt(t).position) return null;
+            var i = ie(t);
+            for (zt(i) && (i = i.host); Bt(i) && ["html", "body"].indexOf(Ht(i)) < 0;) {
+                var n = Zt(i);
                 if ("none" !== n.transform || "none" !== n.perspective || "paint" === n.contain || -1 !== ["transform", "perspective"].indexOf(n.willChange) || e && "filter" === n.willChange || e && n.filter && "none" !== n.filter) return i;
                 i = i.parentNode
             }
             return null
         }(t) || e
     }
 
-    function ee(t) {
+    function oe(t) {
         return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
     }
-    var ie = Math.max,
-        ne = Math.min,
-        se = Math.round;
 
-    function oe(t, e, i) {
-        return ie(t, ne(e, i))
+    function re(t, e, i) {
+        return Vt(t, Kt(e, i))
     }
 
-    function re(t) {
+    function ae(t) {
         return Object.assign({}, {
             top: 0,
             right: 0,
             bottom: 0,
             left: 0
         }, t)
     }
 
-    function ae(t, e) {
+    function le(t, e) {
         return e.reduce((function(e, i) {
             return e[i] = t, e
         }), {})
     }
-    const le = {
+    const ce = {
         name: "arrow",
         enabled: !0,
         phase: "main",
         fn: function(t) {
             var e, i = t.state,
                 n = t.name,
                 s = t.options,
                 o = i.elements.arrow,
                 r = i.modifiersData.popperOffsets,
-                a = Ut(i.placement),
-                l = ee(a),
-                c = [bt, _t].indexOf(a) >= 0 ? "height" : "width";
+                a = qt(i.placement),
+                l = oe(a),
+                c = [_t, gt].indexOf(a) >= 0 ? "height" : "width";
             if (o && r) {
                 var h = function(t, e) {
-                        return re("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
+                        return ae("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
                             placement: e.placement
-                        })) : t) ? t : ae(t, yt))
+                        })) : t) ? t : le(t, vt))
                     }(s.padding, i),
-                    d = Kt(o),
-                    u = "y" === l ? mt : bt,
-                    f = "y" === l ? gt : _t,
+                    d = Gt(o),
+                    u = "y" === l ? pt : _t,
+                    f = "y" === l ? mt : gt,
                     p = i.rects.reference[c] + i.rects.reference[l] - r[l] - i.rects.popper[c],
                     m = r[l] - i.rects.reference[l],
-                    g = te(o),
+                    g = se(o),
                     _ = g ? "y" === l ? g.clientHeight || 0 : g.clientWidth || 0 : 0,
                     b = p / 2 - m / 2,
                     v = h[u],
                     y = _ - d[c] - h[f],
                     w = _ / 2 - d[c] / 2 + b,
-                    E = oe(v, w, y),
-                    A = l;
-                i.modifiersData[n] = ((e = {})[A] = E, e.centerOffset = E - w, e)
+                    A = re(v, w, y),
+                    E = l;
+                i.modifiersData[n] = ((e = {})[E] = A, e.centerOffset = A - w, e)
             }
         },
         effect: function(t) {
             var e = t.state,
                 i = t.options.element,
                 n = void 0 === i ? "[data-popper-arrow]" : i;
-            null != n && ("string" != typeof n || (n = e.elements.popper.querySelector(n))) && Xt(e.elements.popper, n) && (e.elements.arrow = n)
+            null != n && ("string" != typeof n || (n = e.elements.popper.querySelector(n))) && Jt(e.elements.popper, n) && (e.elements.arrow = n)
         },
         requires: ["popperOffsets"],
         requiresIfExists: ["preventOverflow"]
     };
 
-    function ce(t) {
+    function he(t) {
         return t.split("-")[1]
     }
-    var he = {
+    var de = {
         top: "auto",
         right: "auto",
         bottom: "auto",
         left: "auto"
     };
 
-    function de(t) {
+    function ue(t) {
         var e, i = t.popper,
             n = t.popperRect,
             s = t.placement,
             o = t.variation,
             r = t.offsets,
             a = t.position,
             l = t.gpuAcceleration,
             c = t.adaptive,
             h = t.roundOffsets,
-            d = !0 === h ? function(t) {
-                var e = t.x,
-                    i = t.y,
-                    n = window.devicePixelRatio || 1;
-                return {
-                    x: se(se(e * n) / n) || 0,
-                    y: se(se(i * n) / n) || 0
-                }
-            }(r) : "function" == typeof h ? h(r) : r,
-            u = d.x,
+            d = t.isFixed,
+            u = r.x,
             f = void 0 === u ? 0 : u,
-            p = d.y,
+            p = r.y,
             m = void 0 === p ? 0 : p,
-            g = r.hasOwnProperty("x"),
-            _ = r.hasOwnProperty("y"),
-            b = bt,
-            v = mt,
-            y = window;
+            g = "function" == typeof h ? h({
+                x: f,
+                y: m
+            }) : {
+                x: f,
+                y: m
+            };
+        f = g.x, m = g.y;
+        var _ = r.hasOwnProperty("x"),
+            b = r.hasOwnProperty("y"),
+            v = _t,
+            y = pt,
+            w = window;
         if (c) {
-            var w = te(i),
+            var A = se(i),
                 E = "clientHeight",
-                A = "clientWidth";
-            w === Wt(i) && "static" !== Yt(w = Gt(i)).position && "absolute" === a && (E = "scrollHeight", A = "scrollWidth"), w = w, s !== mt && (s !== bt && s !== _t || o !== Et) || (v = gt, m -= w[E] - n.height, m *= l ? 1 : -1), s !== bt && (s !== mt && s !== gt || o !== Et) || (b = _t, f -= w[A] - n.width, f *= l ? 1 : -1)
+                T = "clientWidth";
+            A === $t(i) && "static" !== Zt(A = ee(i)).position && "absolute" === a && (E = "scrollHeight", T = "scrollWidth"), (s === pt || (s === _t || s === gt) && o === wt) && (y = mt, m -= (d && A === w && w.visualViewport ? w.visualViewport.height : A[E]) - n.height, m *= l ? 1 : -1), s !== _t && (s !== pt && s !== mt || o !== wt) || (v = gt, f -= (d && A === w && w.visualViewport ? w.visualViewport.width : A[T]) - n.width, f *= l ? 1 : -1)
         }
-        var T, O = Object.assign({
-            position: a
-        }, c && he);
-        return l ? Object.assign({}, O, ((T = {})[v] = _ ? "0" : "", T[b] = g ? "0" : "", T.transform = (y.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + m + "px)" : "translate3d(" + f + "px, " + m + "px, 0)", T)) : Object.assign({}, O, ((e = {})[v] = _ ? m + "px" : "", e[b] = g ? f + "px" : "", e.transform = "", e))
+        var C, O = Object.assign({
+                position: a
+            }, c && de),
+            x = !0 === h ? function(t, e) {
+                var i = t.x,
+                    n = t.y,
+                    s = e.devicePixelRatio || 1;
+                return {
+                    x: Qt(i * s) / s || 0,
+                    y: Qt(n * s) / s || 0
+                }
+            }({
+                x: f,
+                y: m
+            }, $t(i)) : {
+                x: f,
+                y: m
+            };
+        return f = x.x, m = x.y, l ? Object.assign({}, O, ((C = {})[y] = b ? "0" : "", C[v] = _ ? "0" : "", C.transform = (w.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + m + "px)" : "translate3d(" + f + "px, " + m + "px, 0)", C)) : Object.assign({}, O, ((e = {})[y] = b ? m + "px" : "", e[v] = _ ? f + "px" : "", e.transform = "", e))
     }
-    const ue = {
+    const fe = {
         name: "computeStyles",
         enabled: !0,
         phase: "beforeWrite",
         fn: function(t) {
             var e = t.state,
                 i = t.options,
                 n = i.gpuAcceleration,
                 s = void 0 === n || n,
                 o = i.adaptive,
                 r = void 0 === o || o,
                 a = i.roundOffsets,
                 l = void 0 === a || a,
                 c = {
-                    placement: Ut(e.placement),
-                    variation: ce(e.placement),
+                    placement: qt(e.placement),
+                    variation: he(e.placement),
                     popper: e.elements.popper,
                     popperRect: e.rects.popper,
-                    gpuAcceleration: s
+                    gpuAcceleration: s,
+                    isFixed: "fixed" === e.options.strategy
                 };
-            null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, de(Object.assign({}, c, {
+            null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, ue(Object.assign({}, c, {
                 offsets: e.modifiersData.popperOffsets,
                 position: e.options.strategy,
                 adaptive: r,
                 roundOffsets: l
-            })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, de(Object.assign({}, c, {
+            })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, ue(Object.assign({}, c, {
                 offsets: e.modifiersData.arrow,
                 position: "absolute",
                 adaptive: !1,
                 roundOffsets: l
             })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
                 "data-popper-placement": e.placement
             })
         },
         data: {}
     };
-    var fe = {
+    var pe = {
         passive: !0
     };
-    const pe = {
+    const me = {
         name: "eventListeners",
         enabled: !0,
         phase: "write",
         fn: function() {},
         effect: function(t) {
             var e = t.state,
                 i = t.instance,
                 n = t.options,
                 s = n.scroll,
                 o = void 0 === s || s,
                 r = n.resize,
                 a = void 0 === r || r,
-                l = Wt(e.elements.popper),
+                l = $t(e.elements.popper),
                 c = [].concat(e.scrollParents.reference, e.scrollParents.popper);
             return o && c.forEach((function(t) {
-                    t.addEventListener("scroll", i.update, fe)
-                })), a && l.addEventListener("resize", i.update, fe),
+                    t.addEventListener("scroll", i.update, pe)
+                })), a && l.addEventListener("resize", i.update, pe),
                 function() {
                     o && c.forEach((function(t) {
-                        t.removeEventListener("scroll", i.update, fe)
-                    })), a && l.removeEventListener("resize", i.update, fe)
+                        t.removeEventListener("scroll", i.update, pe)
+                    })), a && l.removeEventListener("resize", i.update, pe)
                 }
         },
         data: {}
     };
-    var me = {
+    var ge = {
         left: "right",
         right: "left",
         bottom: "top",
         top: "bottom"
     };
 
-    function ge(t) {
+    function _e(t) {
         return t.replace(/left|right|bottom|top/g, (function(t) {
-            return me[t]
+            return ge[t]
         }))
     }
-    var _e = {
+    var be = {
         start: "end",
         end: "start"
     };
 
-    function be(t) {
+    function ve(t) {
         return t.replace(/start|end/g, (function(t) {
-            return _e[t]
+            return be[t]
         }))
     }
 
-    function ve(t) {
-        var e = Wt(t);
+    function ye(t) {
+        var e = $t(t);
         return {
             scrollLeft: e.pageXOffset,
             scrollTop: e.pageYOffset
         }
     }
 
-    function ye(t) {
-        return Vt(Gt(t)).left + ve(t).scrollLeft
+    function we(t) {
+        return Ut(ee(t)).left + ye(t).scrollLeft
     }
 
-    function we(t) {
-        var e = Yt(t),
+    function Ae(t) {
+        var e = Zt(t),
             i = e.overflow,
             n = e.overflowX,
             s = e.overflowY;
         return /auto|scroll|overlay|hidden/.test(i + s + n)
     }
 
     function Ee(t) {
-        return ["html", "body", "#document"].indexOf(Rt(t)) >= 0 ? t.ownerDocument.body : zt(t) && we(t) ? t : Ee(Zt(t))
+        return ["html", "body", "#document"].indexOf(Ht(t)) >= 0 ? t.ownerDocument.body : Bt(t) && Ae(t) ? t : Ee(ie(t))
     }
 
-    function Ae(t, e) {
+    function Te(t, e) {
         var i;
         void 0 === e && (e = []);
         var n = Ee(t),
             s = n === (null == (i = t.ownerDocument) ? void 0 : i.body),
-            o = Wt(n),
-            r = s ? [o].concat(o.visualViewport || [], we(n) ? n : []) : n,
+            o = $t(n),
+            r = s ? [o].concat(o.visualViewport || [], Ae(n) ? n : []) : n,
             a = e.concat(r);
-        return s ? a : a.concat(Ae(Zt(r)))
+        return s ? a : a.concat(Te(ie(r)))
     }
 
-    function Te(t) {
+    function Ce(t) {
         return Object.assign({}, t, {
             left: t.x,
             top: t.y,
             right: t.x + t.width,
             bottom: t.y + t.height
         })
     }
 
-    function Oe(t, e) {
-        return e === Tt ? Te(function(t) {
-            var e = Wt(t),
-                i = Gt(t),
-                n = e.visualViewport,
-                s = i.clientWidth,
-                o = i.clientHeight,
-                r = 0,
-                a = 0;
-            return n && (s = n.width, o = n.height, /^((?!chrome|android).)*safari/i.test(navigator.userAgent) || (r = n.offsetLeft, a = n.offsetTop)), {
-                width: s,
-                height: o,
-                x: r + ye(t),
-                y: a
-            }
-        }(t)) : zt(e) ? function(t) {
-            var e = Vt(t);
-            return e.top = e.top + t.clientTop, e.left = e.left + t.clientLeft, e.bottom = e.top + t.clientHeight, e.right = e.left + t.clientWidth, e.width = t.clientWidth, e.height = t.clientHeight, e.x = e.left, e.y = e.top, e
-        }(e) : Te(function(t) {
-            var e, i = Gt(t),
-                n = ve(t),
+    function Oe(t, e, i) {
+        return e === Et ? Ce(function(t, e) {
+            var i = $t(t),
+                n = ee(t),
+                s = i.visualViewport,
+                o = n.clientWidth,
+                r = n.clientHeight,
+                a = 0,
+                l = 0;
+            if (s) {
+                o = s.width, r = s.height;
+                var c = Yt();
+                (c || !c && "fixed" === e) && (a = s.offsetLeft, l = s.offsetTop)
+            }
+            return {
+                width: o,
+                height: r,
+                x: a + we(t),
+                y: l
+            }
+        }(t, i)) : Wt(e) ? function(t, e) {
+            var i = Ut(t, !1, "fixed" === e);
+            return i.top = i.top + t.clientTop, i.left = i.left + t.clientLeft, i.bottom = i.top + t.clientHeight, i.right = i.left + t.clientWidth, i.width = t.clientWidth, i.height = t.clientHeight, i.x = i.left, i.y = i.top, i
+        }(e, i) : Ce(function(t) {
+            var e, i = ee(t),
+                n = ye(t),
                 s = null == (e = t.ownerDocument) ? void 0 : e.body,
-                o = ie(i.scrollWidth, i.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
-                r = ie(i.scrollHeight, i.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
-                a = -n.scrollLeft + ye(t),
+                o = Vt(i.scrollWidth, i.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
+                r = Vt(i.scrollHeight, i.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
+                a = -n.scrollLeft + we(t),
                 l = -n.scrollTop;
-            return "rtl" === Yt(s || i).direction && (a += ie(i.clientWidth, s ? s.clientWidth : 0) - o), {
+            return "rtl" === Zt(s || i).direction && (a += Vt(i.clientWidth, s ? s.clientWidth : 0) - o), {
                 width: o,
                 height: r,
                 x: a,
                 y: l
             }
-        }(Gt(t)))
+        }(ee(t)))
     }
 
-    function Ce(t) {
+    function xe(t) {
         var e, i = t.reference,
             n = t.element,
             s = t.placement,
-            o = s ? Ut(s) : null,
-            r = s ? ce(s) : null,
+            o = s ? qt(s) : null,
+            r = s ? he(s) : null,
             a = i.x + i.width / 2 - n.width / 2,
             l = i.y + i.height / 2 - n.height / 2;
         switch (o) {
-            case mt:
+            case pt:
                 e = {
                     x: a,
                     y: i.y - n.height
                 };
                 break;
-            case gt:
+            case mt:
                 e = {
                     x: a,
                     y: i.y + i.height
                 };
                 break;
-            case _t:
+            case gt:
                 e = {
                     x: i.x + i.width,
                     y: l
                 };
                 break;
-            case bt:
+            case _t:
                 e = {
                     x: i.x - n.width,
                     y: l
                 };
                 break;
             default:
                 e = {
                     x: i.x,
                     y: i.y
                 }
         }
-        var c = o ? ee(o) : null;
+        var c = o ? oe(o) : null;
         if (null != c) {
             var h = "y" === c ? "height" : "width";
             switch (r) {
-                case wt:
+                case yt:
                     e[c] = e[c] - (i[h] / 2 - n[h] / 2);
                     break;
-                case Et:
+                case wt:
                     e[c] = e[c] + (i[h] / 2 - n[h] / 2)
             }
         }
         return e
     }
 
     function ke(t, e) {
         void 0 === e && (e = {});
         var i = e,
             n = i.placement,
             s = void 0 === n ? t.placement : n,
-            o = i.boundary,
-            r = void 0 === o ? At : o,
-            a = i.rootBoundary,
-            l = void 0 === a ? Tt : a,
-            c = i.elementContext,
-            h = void 0 === c ? Ot : c,
-            d = i.altBoundary,
-            u = void 0 !== d && d,
-            f = i.padding,
-            p = void 0 === f ? 0 : f,
-            m = re("number" != typeof p ? p : ae(p, yt)),
-            g = h === Ot ? Ct : Ot,
-            _ = t.rects.popper,
-            b = t.elements[u ? g : h],
-            v = function(t, e, i) {
-                var n = "clippingParents" === e ? function(t) {
-                        var e = Ae(Zt(t)),
-                            i = ["absolute", "fixed"].indexOf(Yt(t).position) >= 0 && zt(t) ? te(t) : t;
-                        return $t(i) ? e.filter((function(t) {
-                            return $t(t) && Xt(t, i) && "body" !== Rt(t)
+            o = i.strategy,
+            r = void 0 === o ? t.strategy : o,
+            a = i.boundary,
+            l = void 0 === a ? At : a,
+            c = i.rootBoundary,
+            h = void 0 === c ? Et : c,
+            d = i.elementContext,
+            u = void 0 === d ? Tt : d,
+            f = i.altBoundary,
+            p = void 0 !== f && f,
+            m = i.padding,
+            g = void 0 === m ? 0 : m,
+            _ = ae("number" != typeof g ? g : le(g, vt)),
+            b = u === Tt ? Ct : Tt,
+            v = t.rects.popper,
+            y = t.elements[p ? b : u],
+            w = function(t, e, i, n) {
+                var s = "clippingParents" === e ? function(t) {
+                        var e = Te(ie(t)),
+                            i = ["absolute", "fixed"].indexOf(Zt(t).position) >= 0 && Bt(t) ? se(t) : t;
+                        return Wt(i) ? e.filter((function(t) {
+                            return Wt(t) && Jt(t, i) && "body" !== Ht(t)
                         })) : []
                     }(t) : [].concat(e),
-                    s = [].concat(n, [i]),
-                    o = s[0],
-                    r = s.reduce((function(e, i) {
-                        var n = Oe(t, i);
-                        return e.top = ie(n.top, e.top), e.right = ne(n.right, e.right), e.bottom = ne(n.bottom, e.bottom), e.left = ie(n.left, e.left), e
-                    }), Oe(t, o));
-                return r.width = r.right - r.left, r.height = r.bottom - r.top, r.x = r.left, r.y = r.top, r
-            }($t(b) ? b : b.contextElement || Gt(t.elements.popper), r, l),
-            y = Vt(t.elements.reference),
-            w = Ce({
-                reference: y,
-                element: _,
+                    o = [].concat(s, [i]),
+                    r = o[0],
+                    a = o.reduce((function(e, i) {
+                        var s = Oe(t, i, n);
+                        return e.top = Vt(s.top, e.top), e.right = Kt(s.right, e.right), e.bottom = Kt(s.bottom, e.bottom), e.left = Vt(s.left, e.left), e
+                    }), Oe(t, r, n));
+                return a.width = a.right - a.left, a.height = a.bottom - a.top, a.x = a.left, a.y = a.top, a
+            }(Wt(y) ? y : y.contextElement || ee(t.elements.popper), l, h, r),
+            A = Ut(t.elements.reference),
+            E = xe({
+                reference: A,
+                element: v,
                 strategy: "absolute",
                 placement: s
             }),
-            E = Te(Object.assign({}, _, w)),
-            A = h === Ot ? E : y,
-            T = {
-                top: v.top - A.top + m.top,
-                bottom: A.bottom - v.bottom + m.bottom,
-                left: v.left - A.left + m.left,
-                right: A.right - v.right + m.right
+            T = Ce(Object.assign({}, v, E)),
+            C = u === Tt ? T : A,
+            O = {
+                top: w.top - C.top + _.top,
+                bottom: C.bottom - w.bottom + _.bottom,
+                left: w.left - C.left + _.left,
+                right: C.right - w.right + _.right
             },
-            O = t.modifiersData.offset;
-        if (h === Ot && O) {
-            var C = O[s];
-            Object.keys(T).forEach((function(t) {
-                var e = [_t, gt].indexOf(t) >= 0 ? 1 : -1,
-                    i = [mt, gt].indexOf(t) >= 0 ? "y" : "x";
-                T[t] += C[i] * e
+            x = t.modifiersData.offset;
+        if (u === Tt && x) {
+            var k = x[s];
+            Object.keys(O).forEach((function(t) {
+                var e = [gt, mt].indexOf(t) >= 0 ? 1 : -1,
+                    i = [pt, mt].indexOf(t) >= 0 ? "y" : "x";
+                O[t] += k[i] * e
             }))
         }
-        return T
+        return O
     }
 
     function Le(t, e) {
         void 0 === e && (e = {});
         var i = e,
             n = i.placement,
             s = i.boundary,
             o = i.rootBoundary,
             r = i.padding,
             a = i.flipVariations,
             l = i.allowedAutoPlacements,
-            c = void 0 === l ? Lt : l,
-            h = ce(n),
-            d = h ? a ? kt : kt.filter((function(t) {
-                return ce(t) === h
-            })) : yt,
+            c = void 0 === l ? xt : l,
+            h = he(n),
+            d = h ? a ? Ot : Ot.filter((function(t) {
+                return he(t) === h
+            })) : vt,
             u = d.filter((function(t) {
                 return c.indexOf(t) >= 0
             }));
         0 === u.length && (u = d);
         var f = u.reduce((function(e, i) {
             return e[i] = ke(t, {
                 placement: i,
                 boundary: s,
                 rootBoundary: o,
                 padding: r
-            })[Ut(i)], e
+            })[qt(i)], e
         }), {});
         return Object.keys(f).sort((function(t, e) {
             return f[t] - f[e]
         }))
     }
-    const xe = {
+    const Se = {
         name: "flip",
         enabled: !0,
         phase: "main",
         fn: function(t) {
             var e = t.state,
                 i = t.options,
                 n = t.name;
             if (!e.modifiersData[n]._skip) {
-                for (var s = i.mainAxis, o = void 0 === s || s, r = i.altAxis, a = void 0 === r || r, l = i.fallbackPlacements, c = i.padding, h = i.boundary, d = i.rootBoundary, u = i.altBoundary, f = i.flipVariations, p = void 0 === f || f, m = i.allowedAutoPlacements, g = e.options.placement, _ = Ut(g), b = l || (_ !== g && p ? function(t) {
-                        if (Ut(t) === vt) return [];
-                        var e = ge(t);
-                        return [be(t), e, be(e)]
-                    }(g) : [ge(g)]), v = [g].concat(b).reduce((function(t, i) {
-                        return t.concat(Ut(i) === vt ? Le(e, {
+                for (var s = i.mainAxis, o = void 0 === s || s, r = i.altAxis, a = void 0 === r || r, l = i.fallbackPlacements, c = i.padding, h = i.boundary, d = i.rootBoundary, u = i.altBoundary, f = i.flipVariations, p = void 0 === f || f, m = i.allowedAutoPlacements, g = e.options.placement, _ = qt(g), b = l || (_ !== g && p ? function(t) {
+                        if (qt(t) === bt) return [];
+                        var e = _e(t);
+                        return [ve(t), e, ve(e)]
+                    }(g) : [_e(g)]), v = [g].concat(b).reduce((function(t, i) {
+                        return t.concat(qt(i) === bt ? Le(e, {
                             placement: i,
                             boundary: h,
                             rootBoundary: d,
                             padding: c,
                             flipVariations: p,
                             allowedAutoPlacements: m
                         }) : i)
-                    }), []), y = e.rects.reference, w = e.rects.popper, E = new Map, A = !0, T = v[0], O = 0; O < v.length; O++) {
-                    var C = v[O],
-                        k = Ut(C),
-                        L = ce(C) === wt,
-                        x = [mt, gt].indexOf(k) >= 0,
-                        D = x ? "width" : "height",
-                        S = ke(e, {
-                            placement: C,
+                    }), []), y = e.rects.reference, w = e.rects.popper, A = new Map, E = !0, T = v[0], C = 0; C < v.length; C++) {
+                    var O = v[C],
+                        x = qt(O),
+                        k = he(O) === yt,
+                        L = [pt, mt].indexOf(x) >= 0,
+                        S = L ? "width" : "height",
+                        D = ke(e, {
+                            placement: O,
                             boundary: h,
                             rootBoundary: d,
                             altBoundary: u,
                             padding: c
                         }),
-                        N = x ? L ? _t : bt : L ? gt : mt;
-                    y[D] > w[D] && (N = ge(N));
-                    var I = ge(N),
+                        I = L ? k ? gt : _t : k ? mt : pt;
+                    y[S] > w[S] && (I = _e(I));
+                    var N = _e(I),
                         P = [];
-                    if (o && P.push(S[k] <= 0), a && P.push(S[N] <= 0, S[I] <= 0), P.every((function(t) {
+                    if (o && P.push(D[x] <= 0), a && P.push(D[I] <= 0, D[N] <= 0), P.every((function(t) {
                             return t
                         }))) {
-                        T = C, A = !1;
+                        T = O, E = !1;
                         break
                     }
-                    E.set(C, P)
+                    A.set(O, P)
                 }
-                if (A)
-                    for (var j = function(t) {
+                if (E)
+                    for (var M = function(t) {
                             var e = v.find((function(e) {
-                                var i = E.get(e);
+                                var i = A.get(e);
                                 if (i) return i.slice(0, t).every((function(t) {
                                     return t
                                 }))
                             }));
                             if (e) return T = e, "break"
-                        }, M = p ? 3 : 1; M > 0 && "break" !== j(M); M--);
+                        }, j = p ? 3 : 1; j > 0 && "break" !== M(j); j--);
                 e.placement !== T && (e.modifiersData[n]._skip = !0, e.placement = T, e.reset = !0)
             }
         },
         requiresIfExists: ["offset"],
         data: {
             _skip: !1
         }
@@ -1411,16 +1488,16 @@
             top: t.top - e.height - i.y,
             right: t.right - e.width + i.x,
             bottom: t.bottom - e.height + i.y,
             left: t.left - e.width - i.x
         }
     }
 
-    function Se(t) {
-        return [mt, _t, gt, bt].some((function(e) {
+    function Ie(t) {
+        return [pt, gt, mt, _t].some((function(e) {
             return t[e] >= 0
         }))
     }
     const Ne = {
             name: "hide",
             enabled: !0,
             phase: "main",
@@ -1435,70 +1512,70 @@
                         elementContext: "reference"
                     }),
                     a = ke(e, {
                         altBoundary: !0
                     }),
                     l = De(r, n),
                     c = De(a, s, o),
-                    h = Se(l),
-                    d = Se(c);
+                    h = Ie(l),
+                    d = Ie(c);
                 e.modifiersData[i] = {
                     referenceClippingOffsets: l,
                     popperEscapeOffsets: c,
                     isReferenceHidden: h,
                     hasPopperEscaped: d
                 }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
                     "data-popper-reference-hidden": h,
                     "data-popper-escaped": d
                 })
             }
         },
-        Ie = {
+        Pe = {
             name: "offset",
             enabled: !0,
             phase: "main",
             requires: ["popperOffsets"],
             fn: function(t) {
                 var e = t.state,
                     i = t.options,
                     n = t.name,
                     s = i.offset,
                     o = void 0 === s ? [0, 0] : s,
-                    r = Lt.reduce((function(t, i) {
+                    r = xt.reduce((function(t, i) {
                         return t[i] = function(t, e, i) {
-                            var n = Ut(t),
-                                s = [bt, mt].indexOf(n) >= 0 ? -1 : 1,
+                            var n = qt(t),
+                                s = [_t, pt].indexOf(n) >= 0 ? -1 : 1,
                                 o = "function" == typeof i ? i(Object.assign({}, e, {
                                     placement: t
                                 })) : i,
                                 r = o[0],
                                 a = o[1];
-                            return r = r || 0, a = (a || 0) * s, [bt, _t].indexOf(n) >= 0 ? {
+                            return r = r || 0, a = (a || 0) * s, [_t, gt].indexOf(n) >= 0 ? {
                                 x: a,
                                 y: r
                             } : {
                                 x: r,
                                 y: a
                             }
                         }(i, e.rects, o), t
                     }), {}),
                     a = r[e.placement],
                     l = a.x,
                     c = a.y;
                 null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += l, e.modifiersData.popperOffsets.y += c), e.modifiersData[n] = r
             }
         },
-        Pe = {
+        Me = {
             name: "popperOffsets",
             enabled: !0,
             phase: "read",
             fn: function(t) {
                 var e = t.state,
                     i = t.name;
-                e.modifiersData[i] = Ce({
+                e.modifiersData[i] = xe({
                     reference: e.rects.reference,
                     element: e.rects.popper,
                     strategy: "absolute",
                     placement: e.placement
                 })
             },
             data: {}
@@ -1525,106 +1602,121 @@
                     m = void 0 === p ? 0 : p,
                     g = ke(e, {
                         boundary: l,
                         rootBoundary: c,
                         padding: d,
                         altBoundary: h
                     }),
-                    _ = Ut(e.placement),
-                    b = ce(e.placement),
+                    _ = qt(e.placement),
+                    b = he(e.placement),
                     v = !b,
-                    y = ee(_),
+                    y = oe(_),
                     w = "x" === y ? "y" : "x",
-                    E = e.modifiersData.popperOffsets,
-                    A = e.rects.reference,
+                    A = e.modifiersData.popperOffsets,
+                    E = e.rects.reference,
                     T = e.rects.popper,
-                    O = "function" == typeof m ? m(Object.assign({}, e.rects, {
+                    C = "function" == typeof m ? m(Object.assign({}, e.rects, {
                         placement: e.placement
                     })) : m,
-                    C = {
+                    O = "number" == typeof C ? {
+                        mainAxis: C,
+                        altAxis: C
+                    } : Object.assign({
+                        mainAxis: 0,
+                        altAxis: 0
+                    }, C),
+                    x = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
+                    k = {
                         x: 0,
                         y: 0
                     };
-                if (E) {
-                    if (o || a) {
-                        var k = "y" === y ? mt : bt,
-                            L = "y" === y ? gt : _t,
-                            x = "y" === y ? "height" : "width",
-                            D = E[y],
-                            S = E[y] + g[k],
-                            N = E[y] - g[L],
-                            I = f ? -T[x] / 2 : 0,
-                            P = b === wt ? A[x] : T[x],
-                            j = b === wt ? -T[x] : -A[x],
-                            M = e.elements.arrow,
-                            H = f && M ? Kt(M) : {
+                if (A) {
+                    if (o) {
+                        var L, S = "y" === y ? pt : _t,
+                            D = "y" === y ? mt : gt,
+                            I = "y" === y ? "height" : "width",
+                            N = A[y],
+                            P = N + g[S],
+                            M = N - g[D],
+                            j = f ? -T[I] / 2 : 0,
+                            F = b === yt ? E[I] : T[I],
+                            H = b === yt ? -T[I] : -E[I],
+                            $ = e.elements.arrow,
+                            W = f && $ ? Gt($) : {
                                 width: 0,
                                 height: 0
                             },
                             B = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
                                 top: 0,
                                 right: 0,
                                 bottom: 0,
                                 left: 0
                             },
-                            R = B[k],
-                            W = B[L],
-                            $ = oe(0, A[x], H[x]),
-                            z = v ? A[x] / 2 - I - $ - R - O : P - $ - R - O,
-                            q = v ? -A[x] / 2 + I + $ + W + O : j + $ + W + O,
-                            F = e.elements.arrow && te(e.elements.arrow),
-                            U = F ? "y" === y ? F.clientTop || 0 : F.clientLeft || 0 : 0,
-                            V = e.modifiersData.offset ? e.modifiersData.offset[e.placement][y] : 0,
-                            K = E[y] + z - V - U,
-                            X = E[y] + q - V;
-                        if (o) {
-                            var Y = oe(f ? ne(S, K) : S, D, f ? ie(N, X) : N);
-                            E[y] = Y, C[y] = Y - D
-                        }
-                        if (a) {
-                            var Q = "x" === y ? mt : bt,
-                                G = "x" === y ? gt : _t,
-                                Z = E[w],
-                                J = Z + g[Q],
-                                tt = Z - g[G],
-                                et = oe(f ? ne(J, K) : J, Z, f ? ie(tt, X) : tt);
-                            E[w] = et, C[w] = et - Z
-                        }
+                            z = B[S],
+                            R = B[D],
+                            q = re(0, E[I], W[I]),
+                            V = v ? E[I] / 2 - j - q - z - O.mainAxis : F - q - z - O.mainAxis,
+                            K = v ? -E[I] / 2 + j + q + R + O.mainAxis : H + q + R + O.mainAxis,
+                            Q = e.elements.arrow && se(e.elements.arrow),
+                            X = Q ? "y" === y ? Q.clientTop || 0 : Q.clientLeft || 0 : 0,
+                            Y = null != (L = null == x ? void 0 : x[y]) ? L : 0,
+                            U = N + K - Y,
+                            G = re(f ? Kt(P, N + V - Y - X) : P, N, f ? Vt(M, U) : M);
+                        A[y] = G, k[y] = G - N
+                    }
+                    if (a) {
+                        var J, Z = "x" === y ? pt : _t,
+                            tt = "x" === y ? mt : gt,
+                            et = A[w],
+                            it = "y" === w ? "height" : "width",
+                            nt = et + g[Z],
+                            st = et - g[tt],
+                            ot = -1 !== [pt, _t].indexOf(_),
+                            rt = null != (J = null == x ? void 0 : x[w]) ? J : 0,
+                            at = ot ? nt : et - E[it] - T[it] - rt + O.altAxis,
+                            lt = ot ? et + E[it] + T[it] - rt - O.altAxis : st,
+                            ct = f && ot ? function(t, e, i) {
+                                var n = re(t, e, i);
+                                return n > i ? i : n
+                            }(at, et, lt) : re(f ? at : nt, et, f ? lt : st);
+                        A[w] = ct, k[w] = ct - et
                     }
-                    e.modifiersData[n] = C
+                    e.modifiersData[n] = k
                 }
             },
             requiresIfExists: ["offset"]
         };
 
-    function Me(t, e, i) {
+    function Fe(t, e, i) {
         void 0 === i && (i = !1);
-        var n = zt(e);
-        zt(e) && function(t) {
-            var e = t.getBoundingClientRect();
-            e.width, t.offsetWidth, e.height, t.offsetHeight
-        }(e);
-        var s, o, r = Gt(e),
-            a = Vt(t),
-            l = {
+        var n, s, o = Bt(e),
+            r = Bt(e) && function(t) {
+                var e = t.getBoundingClientRect(),
+                    i = Qt(e.width) / t.offsetWidth || 1,
+                    n = Qt(e.height) / t.offsetHeight || 1;
+                return 1 !== i || 1 !== n
+            }(e),
+            a = ee(e),
+            l = Ut(t, r, i),
+            c = {
                 scrollLeft: 0,
                 scrollTop: 0
             },
-            c = {
+            h = {
                 x: 0,
                 y: 0
             };
-        return (n || !n && !i) && (("body" !== Rt(e) || we(r)) && (l = (s = e) !== Wt(s) && zt(s) ? {
-            scrollLeft: (o = s).scrollLeft,
-            scrollTop: o.scrollTop
-        } : ve(s)), zt(e) ? ((c = Vt(e)).x += e.clientLeft, c.y += e.clientTop) : r && (c.x = ye(r))), {
-            x: a.left + l.scrollLeft - c.x,
-            y: a.top + l.scrollTop - c.y,
-            width: a.width,
-            height: a.height
+        return (o || !o && !i) && (("body" !== Ht(e) || Ae(a)) && (c = (n = e) !== $t(n) && Bt(n) ? {
+            scrollLeft: (s = n).scrollLeft,
+            scrollTop: s.scrollTop
+        } : ye(n)), Bt(e) ? ((h = Ut(e, !0)).x += e.clientLeft, h.y += e.clientTop) : a && (h.x = we(a))), {
+            x: l.left + c.scrollLeft - h.x,
+            y: l.top + c.scrollTop - h.y,
+            width: l.width,
+            height: l.height
         }
     }
 
     function He(t) {
         var e = new Map,
             i = new Set,
             n = [];
@@ -1639,40 +1731,40 @@
         }
         return t.forEach((function(t) {
             e.set(t.name, t)
         })), t.forEach((function(t) {
             i.has(t.name) || s(t)
         })), n
     }
-    var Be = {
+    var $e = {
         placement: "bottom",
         modifiers: [],
         strategy: "absolute"
     };
 
-    function Re() {
+    function We() {
         for (var t = arguments.length, e = new Array(t), i = 0; i < t; i++) e[i] = arguments[i];
         return !e.some((function(t) {
             return !(t && "function" == typeof t.getBoundingClientRect)
         }))
     }
 
-    function We(t) {
+    function Be(t) {
         void 0 === t && (t = {});
         var e = t,
             i = e.defaultModifiers,
             n = void 0 === i ? [] : i,
             s = e.defaultOptions,
-            o = void 0 === s ? Be : s;
+            o = void 0 === s ? $e : s;
         return function(t, e, i) {
             void 0 === i && (i = o);
             var s, r, a = {
                     placement: "bottom",
                     orderedModifiers: [],
-                    options: Object.assign({}, Be, o),
+                    options: Object.assign({}, $e, o),
                     modifiersData: {},
                     elements: {
                         reference: t,
                         popper: e
                     },
                     attributes: {},
                     styles: {}
@@ -1680,20 +1772,20 @@
                 l = [],
                 c = !1,
                 h = {
                     state: a,
                     setOptions: function(i) {
                         var s = "function" == typeof i ? i(a.options) : i;
                         d(), a.options = Object.assign({}, o, a.options, s), a.scrollParents = {
-                            reference: $t(t) ? Ae(t) : t.contextElement ? Ae(t.contextElement) : [],
-                            popper: Ae(e)
+                            reference: Wt(t) ? Te(t) : t.contextElement ? Te(t.contextElement) : [],
+                            popper: Te(e)
                         };
                         var r, c, u = function(t) {
                             var e = He(t);
-                            return Bt.reduce((function(t, i) {
+                            return Ft.reduce((function(t, i) {
                                 return t.concat(e.filter((function(t) {
                                     return t.phase === i
                                 })))
                             }), [])
                         }((r = [].concat(n, a.options.modifiers), c = r.reduce((function(t, e) {
                             var i = t[e.name];
                             return t[e.name] = i ? Object.assign({}, i, e, {
@@ -1722,18 +1814,18 @@
                         })), h.update()
                     },
                     forceUpdate: function() {
                         if (!c) {
                             var t = a.elements,
                                 e = t.reference,
                                 i = t.popper;
-                            if (Re(e, i)) {
+                            if (We(e, i)) {
                                 a.rects = {
-                                    reference: Me(e, te(i), "fixed" === a.options.strategy),
-                                    popper: Kt(i)
+                                    reference: Fe(e, se(i), "fixed" === a.options.strategy),
+                                    popper: Gt(i)
                                 }, a.reset = !1, a.placement = a.options.placement, a.orderedModifiers.forEach((function(t) {
                                     return a.modifiersData[t.name] = Object.assign({}, t.data)
                                 }));
                                 for (var n = 0; n < a.orderedModifiers.length; n++)
                                     if (!0 !== a.reset) {
                                         var s = a.orderedModifiers[n],
                                             o = s.fn,
@@ -1761,176 +1853,176 @@
                             }))
                         }))), r
                     }),
                     destroy: function() {
                         d(), c = !0
                     }
                 };
-            if (!Re(t, e)) return h;
+            if (!We(t, e)) return h;
 
             function d() {
                 l.forEach((function(t) {
                     return t()
                 })), l = []
             }
             return h.setOptions(i).then((function(t) {
                 !c && i.onFirstUpdate && i.onFirstUpdate(t)
             })), h
         }
     }
-    var $e = We(),
-        ze = We({
-            defaultModifiers: [pe, Pe, ue, Ft]
+    var ze = Be(),
+        Re = Be({
+            defaultModifiers: [me, Me, fe, Rt]
         }),
-        qe = We({
-            defaultModifiers: [pe, Pe, ue, Ft, Ie, xe, je, le, Ne]
+        qe = Be({
+            defaultModifiers: [me, Me, fe, Rt, Pe, Se, je, ce, Ne]
         });
-    const Fe = Object.freeze({
+    const Ve = Object.freeze(Object.defineProperty({
             __proto__: null,
-            popperGenerator: We,
-            detectOverflow: ke,
-            createPopperBase: $e,
-            createPopper: qe,
-            createPopperLite: ze,
-            top: mt,
-            bottom: gt,
-            right: _t,
-            left: bt,
-            auto: vt,
-            basePlacements: yt,
-            start: wt,
-            end: Et,
-            clippingParents: At,
-            viewport: Tt,
-            popper: Ot,
-            reference: Ct,
-            variationPlacements: kt,
-            placements: Lt,
-            beforeRead: xt,
-            read: Dt,
+            afterMain: Nt,
             afterRead: St,
-            beforeMain: Nt,
-            main: It,
-            afterMain: Pt,
-            beforeWrite: jt,
-            write: Mt,
-            afterWrite: Ht,
-            modifierPhases: Bt,
-            applyStyles: Ft,
-            arrow: le,
-            computeStyles: ue,
-            eventListeners: pe,
-            flip: xe,
+            afterWrite: jt,
+            applyStyles: Rt,
+            arrow: ce,
+            auto: bt,
+            basePlacements: vt,
+            beforeMain: Dt,
+            beforeRead: kt,
+            beforeWrite: Pt,
+            bottom: mt,
+            clippingParents: At,
+            computeStyles: fe,
+            createPopper: qe,
+            createPopperBase: ze,
+            createPopperLite: Re,
+            detectOverflow: ke,
+            end: wt,
+            eventListeners: me,
+            flip: Se,
             hide: Ne,
-            offset: Ie,
-            popperOffsets: Pe,
-            preventOverflow: je
-        }),
-        Ue = "dropdown",
-        Ve = "Escape",
-        Ke = "Space",
-        Xe = "ArrowUp",
-        Ye = "ArrowDown",
-        Qe = new RegExp("ArrowUp|ArrowDown|Escape"),
-        Ge = "click.bs.dropdown.data-api",
-        Ze = "keydown.bs.dropdown.data-api",
-        Je = "show",
-        ti = '[data-bs-toggle="dropdown"]',
-        ei = ".dropdown-menu",
-        ii = m() ? "top-end" : "top-start",
-        ni = m() ? "top-start" : "top-end",
-        si = m() ? "bottom-end" : "bottom-start",
-        oi = m() ? "bottom-start" : "bottom-end",
-        ri = m() ? "left-start" : "right-start",
-        ai = m() ? "right-start" : "left-start",
-        li = {
-            offset: [0, 2],
+            left: _t,
+            main: It,
+            modifierPhases: Ft,
+            offset: Pe,
+            placements: xt,
+            popper: Tt,
+            popperGenerator: Be,
+            popperOffsets: Me,
+            preventOverflow: je,
+            read: Lt,
+            reference: Ct,
+            right: gt,
+            start: yt,
+            top: pt,
+            variationPlacements: Ot,
+            viewport: Et,
+            write: Mt
+        }, Symbol.toStringTag, {
+            value: "Module"
+        })),
+        Ke = "dropdown",
+        Qe = "ArrowUp",
+        Xe = "ArrowDown",
+        Ye = "click.bs.dropdown.data-api",
+        Ue = "keydown.bs.dropdown.data-api",
+        Ge = "show",
+        Je = '[data-bs-toggle="dropdown"]:not(.disabled):not(:disabled)',
+        Ze = `${Je}.show`,
+        ti = ".dropdown-menu",
+        ei = p() ? "top-end" : "top-start",
+        ii = p() ? "top-start" : "top-end",
+        ni = p() ? "bottom-end" : "bottom-start",
+        si = p() ? "bottom-start" : "bottom-end",
+        oi = p() ? "left-start" : "right-start",
+        ri = p() ? "right-start" : "left-start",
+        ai = {
+            autoClose: !0,
             boundary: "clippingParents",
-            reference: "toggle",
             display: "dynamic",
+            offset: [0, 2],
             popperConfig: null,
-            autoClose: !0
+            reference: "toggle"
         },
-        ci = {
-            offset: "(array|string|function)",
+        li = {
+            autoClose: "(boolean|string)",
             boundary: "(string|element)",
-            reference: "(string|element|object)",
             display: "string",
+            offset: "(array|string|function)",
             popperConfig: "(null|object|function)",
-            autoClose: "(boolean|string)"
+            reference: "(string|element|object)"
         };
-    class hi extends B {
+    class ci extends W {
         constructor(t, e) {
-            super(t), this._popper = null, this._config = this._getConfig(e), this._menu = this._getMenuElement(), this._inNavbar = this._detectNavbar()
+            super(t, e), this._popper = null, this._parent = this._element.parentNode, this._menu = z.next(this._element, ti)[0] || z.prev(this._element, ti)[0] || z.findOne(ti, this._parent), this._inNavbar = this._detectNavbar()
         }
         static get Default() {
-            return li
+            return ai
         }
         static get DefaultType() {
-            return ci
+            return li
         }
         static get NAME() {
-            return Ue
+            return Ke
         }
         toggle() {
             return this._isShown() ? this.hide() : this.show()
         }
         show() {
-            if (c(this._element) || this._isShown(this._menu)) return;
+            if (l(this._element) || this._isShown()) return;
             const t = {
                 relatedTarget: this._element
             };
-            if (j.trigger(this._element, "show.bs.dropdown", t).defaultPrevented) return;
-            const e = hi.getParentFromElement(this._element);
-            this._inNavbar ? U.setDataAttribute(this._menu, "popper", "none") : this._createPopper(e), "ontouchstart" in document.documentElement && !e.closest(".navbar-nav") && [].concat(...document.body.children).forEach((t => j.on(t, "mouseover", d))), this._element.focus(), this._element.setAttribute("aria-expanded", !0), this._menu.classList.add(Je), this._element.classList.add(Je), j.trigger(this._element, "shown.bs.dropdown", t)
+            if (!P.trigger(this._element, "show.bs.dropdown", t).defaultPrevented) {
+                if (this._createPopper(), "ontouchstart" in document.documentElement && !this._parent.closest(".navbar-nav"))
+                    for (const t of [].concat(...document.body.children)) P.on(t, "mouseover", h);
+                this._element.focus(), this._element.setAttribute("aria-expanded", !0), this._menu.classList.add(Ge), this._element.classList.add(Ge), P.trigger(this._element, "shown.bs.dropdown", t)
+            }
         }
         hide() {
-            if (c(this._element) || !this._isShown(this._menu)) return;
+            if (l(this._element) || !this._isShown()) return;
             const t = {
                 relatedTarget: this._element
             };
             this._completeHide(t)
         }
         dispose() {
             this._popper && this._popper.destroy(), super.dispose()
         }
         update() {
             this._inNavbar = this._detectNavbar(), this._popper && this._popper.update()
         }
         _completeHide(t) {
-            j.trigger(this._element, "hide.bs.dropdown", t).defaultPrevented || ("ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => j.off(t, "mouseover", d))), this._popper && this._popper.destroy(), this._menu.classList.remove(Je), this._element.classList.remove(Je), this._element.setAttribute("aria-expanded", "false"), U.removeDataAttribute(this._menu, "popper"), j.trigger(this._element, "hidden.bs.dropdown", t))
+            if (!P.trigger(this._element, "hide.bs.dropdown", t).defaultPrevented) {
+                if ("ontouchstart" in document.documentElement)
+                    for (const t of [].concat(...document.body.children)) P.off(t, "mouseover", h);
+                this._popper && this._popper.destroy(), this._menu.classList.remove(Ge), this._element.classList.remove(Ge), this._element.setAttribute("aria-expanded", "false"), H.removeDataAttribute(this._menu, "popper"), P.trigger(this._element, "hidden.bs.dropdown", t)
+            }
         }
         _getConfig(t) {
-            if (t = {
-                    ...this.constructor.Default,
-                    ...U.getDataAttributes(this._element),
-                    ...t
-                }, a(Ue, t, this.constructor.DefaultType), "object" == typeof t.reference && !o(t.reference) && "function" != typeof t.reference.getBoundingClientRect) throw new TypeError(`${Ue.toUpperCase()}: Option "reference" provided type "object" without a required "getBoundingClientRect" method.`);
+            if ("object" == typeof(t = super._getConfig(t)).reference && !o(t.reference) && "function" != typeof t.reference.getBoundingClientRect) throw new TypeError(`${Ke.toUpperCase()}: Option "reference" provided type "object" without a required "getBoundingClientRect" method.`);
             return t
         }
-        _createPopper(t) {
-            if (void 0 === Fe) throw new TypeError("Bootstrap's dropdowns require Popper (https://popper.js.org)");
-            let e = this._element;
-            "parent" === this._config.reference ? e = t : o(this._config.reference) ? e = r(this._config.reference) : "object" == typeof this._config.reference && (e = this._config.reference);
-            const i = this._getPopperConfig(),
-                n = i.modifiers.find((t => "applyStyles" === t.name && !1 === t.enabled));
-            this._popper = qe(e, this._menu, i), n && U.setDataAttribute(this._menu, "popper", "static")
+        _createPopper() {
+            if (void 0 === Ve) throw new TypeError("Bootstrap's dropdowns require Popper (https://popper.js.org)");
+            let t = this._element;
+            "parent" === this._config.reference ? t = this._parent : o(this._config.reference) ? t = r(this._config.reference) : "object" == typeof this._config.reference && (t = this._config.reference);
+            const e = this._getPopperConfig();
+            this._popper = qe(t, this._menu, e)
         }
-        _isShown(t = this._element) {
-            return t.classList.contains(Je)
-        }
-        _getMenuElement() {
-            return V.next(this._element, ei)[0]
+        _isShown() {
+            return this._menu.classList.contains(Ge)
         }
         _getPlacement() {
-            const t = this._element.parentNode;
-            if (t.classList.contains("dropend")) return ri;
-            if (t.classList.contains("dropstart")) return ai;
+            const t = this._parent;
+            if (t.classList.contains("dropend")) return oi;
+            if (t.classList.contains("dropstart")) return ri;
+            if (t.classList.contains("dropup-center")) return "top";
+            if (t.classList.contains("dropdown-center")) return "bottom";
             const e = "end" === getComputedStyle(this._menu).getPropertyValue("--bs-position").trim();
-            return t.classList.contains("dropup") ? e ? ni : ii : e ? oi : si
+            return t.classList.contains("dropup") ? e ? ii : ei : e ? si : ni
         }
         _detectNavbar() {
             return null !== this._element.closest(".navbar")
         }
         _getOffset() {
             const {
                 offset: t
@@ -1948,709 +2040,754 @@
                 }, {
                     name: "offset",
                     options: {
                         offset: this._getOffset()
                     }
                 }]
             };
-            return "static" === this._config.display && (t.modifiers = [{
+            return (this._inNavbar || "static" === this._config.display) && (H.setDataAttribute(this._menu, "popper", "static"), t.modifiers = [{
                 name: "applyStyles",
                 enabled: !1
             }]), {
                 ...t,
-                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(t) : this._config.popperConfig
+                ...g(this._config.popperConfig, [t])
             }
         }
         _selectMenuItem({
             key: t,
             target: e
         }) {
-            const i = V.find(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)", this._menu).filter(l);
-            i.length && v(i, e, t === Ye, !i.includes(e)).focus()
+            const i = z.find(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)", this._menu).filter((t => a(t)));
+            i.length && b(i, e, t === Xe, !i.includes(e)).focus()
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = hi.getOrCreateInstance(this, t);
+                const e = ci.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
         static clearMenus(t) {
-            if (t && (2 === t.button || "keyup" === t.type && "Tab" !== t.key)) return;
-            const e = V.find(ti);
-            for (let i = 0, n = e.length; i < n; i++) {
-                const n = hi.getInstance(e[i]);
-                if (!n || !1 === n._config.autoClose) continue;
-                if (!n._isShown()) continue;
-                const s = {
-                    relatedTarget: n._element
+            if (2 === t.button || "keyup" === t.type && "Tab" !== t.key) return;
+            const e = z.find(Ze);
+            for (const i of e) {
+                const e = ci.getInstance(i);
+                if (!e || !1 === e._config.autoClose) continue;
+                const n = t.composedPath(),
+                    s = n.includes(e._menu);
+                if (n.includes(e._element) || "inside" === e._config.autoClose && !s || "outside" === e._config.autoClose && s) continue;
+                if (e._menu.contains(t.target) && ("keyup" === t.type && "Tab" === t.key || /input|select|option|textarea|form/i.test(t.target.tagName))) continue;
+                const o = {
+                    relatedTarget: e._element
                 };
-                if (t) {
-                    const e = t.composedPath(),
-                        i = e.includes(n._menu);
-                    if (e.includes(n._element) || "inside" === n._config.autoClose && !i || "outside" === n._config.autoClose && i) continue;
-                    if (n._menu.contains(t.target) && ("keyup" === t.type && "Tab" === t.key || /input|select|option|textarea|form/i.test(t.target.tagName))) continue;
-                    "click" === t.type && (s.clickEvent = t)
-                }
-                n._completeHide(s)
+                "click" === t.type && (o.clickEvent = t), e._completeHide(o)
             }
         }
-        static getParentFromElement(t) {
-            return n(t) || t.parentNode
-        }
         static dataApiKeydownHandler(t) {
-            if (/input|textarea/i.test(t.target.tagName) ? t.key === Ke || t.key !== Ve && (t.key !== Ye && t.key !== Xe || t.target.closest(ei)) : !Qe.test(t.key)) return;
-            const e = this.classList.contains(Je);
-            if (!e && t.key === Ve) return;
-            if (t.preventDefault(), t.stopPropagation(), c(this)) return;
-            const i = this.matches(ti) ? this : V.prev(this, ti)[0],
-                n = hi.getOrCreateInstance(i);
-            if (t.key !== Ve) return t.key === Xe || t.key === Ye ? (e || n.show(), void n._selectMenuItem(t)) : void(e && t.key !== Ke || hi.clearMenus());
-            n.hide()
-        }
-    }
-    j.on(document, Ze, ti, hi.dataApiKeydownHandler), j.on(document, Ze, ei, hi.dataApiKeydownHandler), j.on(document, Ge, hi.clearMenus), j.on(document, "keyup.bs.dropdown.data-api", hi.clearMenus), j.on(document, Ge, ti, (function(t) {
-        t.preventDefault(), hi.getOrCreateInstance(this).toggle()
-    })), g(hi);
-    const di = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
-        ui = ".sticky-top";
-    class fi {
-        constructor() {
-            this._element = document.body
-        }
-        getWidth() {
-            const t = document.documentElement.clientWidth;
-            return Math.abs(window.innerWidth - t)
-        }
-        hide() {
-            const t = this.getWidth();
-            this._disableOverFlow(), this._setElementAttributes(this._element, "paddingRight", (e => e + t)), this._setElementAttributes(di, "paddingRight", (e => e + t)), this._setElementAttributes(ui, "marginRight", (e => e - t))
-        }
-        _disableOverFlow() {
-            this._saveInitialAttribute(this._element, "overflow"), this._element.style.overflow = "hidden"
-        }
-        _setElementAttributes(t, e, i) {
-            const n = this.getWidth();
-            this._applyManipulationCallback(t, (t => {
-                if (t !== this._element && window.innerWidth > t.clientWidth + n) return;
-                this._saveInitialAttribute(t, e);
-                const s = window.getComputedStyle(t)[e];
-                t.style[e] = `${i(Number.parseFloat(s))}px`
-            }))
-        }
-        reset() {
-            this._resetElementAttributes(this._element, "overflow"), this._resetElementAttributes(this._element, "paddingRight"), this._resetElementAttributes(di, "paddingRight"), this._resetElementAttributes(ui, "marginRight")
-        }
-        _saveInitialAttribute(t, e) {
-            const i = t.style[e];
-            i && U.setDataAttribute(t, e, i)
-        }
-        _resetElementAttributes(t, e) {
-            this._applyManipulationCallback(t, (t => {
-                const i = U.getDataAttribute(t, e);
-                void 0 === i ? t.style.removeProperty(e) : (U.removeDataAttribute(t, e), t.style[e] = i)
-            }))
-        }
-        _applyManipulationCallback(t, e) {
-            o(t) ? e(t) : V.find(t, this._element).forEach(e)
-        }
-        isOverflowing() {
-            return this.getWidth() > 0
-        }
-    }
-    const pi = {
+            const e = /input|textarea/i.test(t.target.tagName),
+                i = "Escape" === t.key,
+                n = [Qe, Xe].includes(t.key);
+            if (!n && !i) return;
+            if (e && !i) return;
+            t.preventDefault();
+            const s = this.matches(Je) ? this : z.prev(this, Je)[0] || z.next(this, Je)[0] || z.findOne(Je, t.delegateTarget.parentNode),
+                o = ci.getOrCreateInstance(s);
+            if (n) return t.stopPropagation(), o.show(), void o._selectMenuItem(t);
+            o._isShown() && (t.stopPropagation(), o.hide(), s.focus())
+        }
+    }
+    P.on(document, Ue, Je, ci.dataApiKeydownHandler), P.on(document, Ue, ti, ci.dataApiKeydownHandler), P.on(document, Ye, ci.clearMenus), P.on(document, "keyup.bs.dropdown.data-api", ci.clearMenus), P.on(document, Ye, Je, (function(t) {
+        t.preventDefault(), ci.getOrCreateInstance(this).toggle()
+    })), m(ci);
+    const hi = "show",
+        di = "mousedown.bs.backdrop",
+        ui = {
             className: "modal-backdrop",
-            isVisible: !0,
+            clickCallback: null,
             isAnimated: !1,
-            rootElement: "body",
-            clickCallback: null
+            isVisible: !0,
+            rootElement: "body"
         },
-        mi = {
+        fi = {
             className: "string",
-            isVisible: "boolean",
+            clickCallback: "(function|null)",
             isAnimated: "boolean",
-            rootElement: "(element|string)",
-            clickCallback: "(function|null)"
-        },
-        gi = "show",
-        _i = "mousedown.bs.backdrop";
-    class bi {
+            isVisible: "boolean",
+            rootElement: "(element|string)"
+        };
+    class pi extends $ {
         constructor(t) {
-            this._config = this._getConfig(t), this._isAppended = !1, this._element = null
+            super(), this._config = this._getConfig(t), this._isAppended = !1, this._element = null
+        }
+        static get Default() {
+            return ui
+        }
+        static get DefaultType() {
+            return fi
+        }
+        static get NAME() {
+            return "backdrop"
         }
         show(t) {
-            this._config.isVisible ? (this._append(), this._config.isAnimated && u(this._getElement()), this._getElement().classList.add(gi), this._emulateAnimation((() => {
-                _(t)
-            }))) : _(t)
+            if (!this._config.isVisible) return void g(t);
+            this._append();
+            const e = this._getElement();
+            this._config.isAnimated && d(e), e.classList.add(hi), this._emulateAnimation((() => {
+                g(t)
+            }))
         }
         hide(t) {
-            this._config.isVisible ? (this._getElement().classList.remove(gi), this._emulateAnimation((() => {
-                this.dispose(), _(t)
-            }))) : _(t)
+            this._config.isVisible ? (this._getElement().classList.remove(hi), this._emulateAnimation((() => {
+                this.dispose(), g(t)
+            }))) : g(t)
+        }
+        dispose() {
+            this._isAppended && (P.off(this._element, di), this._element.remove(), this._isAppended = !1)
         }
         _getElement() {
             if (!this._element) {
                 const t = document.createElement("div");
                 t.className = this._config.className, this._config.isAnimated && t.classList.add("fade"), this._element = t
             }
             return this._element
         }
-        _getConfig(t) {
-            return (t = {
-                ...pi,
-                ..."object" == typeof t ? t : {}
-            }).rootElement = r(t.rootElement), a("backdrop", t, mi), t
+        _configAfterMerge(t) {
+            return t.rootElement = r(t.rootElement), t
         }
         _append() {
-            this._isAppended || (this._config.rootElement.append(this._getElement()), j.on(this._getElement(), _i, (() => {
-                _(this._config.clickCallback)
-            })), this._isAppended = !0)
-        }
-        dispose() {
-            this._isAppended && (j.off(this._element, _i), this._element.remove(), this._isAppended = !1)
+            if (this._isAppended) return;
+            const t = this._getElement();
+            this._config.rootElement.append(t), P.on(t, di, (() => {
+                g(this._config.clickCallback)
+            })), this._isAppended = !0
         }
         _emulateAnimation(t) {
-            b(t, this._getElement(), this._config.isAnimated)
+            _(t, this._getElement(), this._config.isAnimated)
         }
     }
-    const vi = {
-            trapElement: null,
-            autofocus: !0
-        },
-        yi = {
-            trapElement: "element",
-            autofocus: "boolean"
-        },
-        wi = ".bs.focustrap",
-        Ei = "backward";
-    class Ai {
+    const mi = ".bs.focustrap",
+        gi = "backward",
+        _i = {
+            autofocus: !0,
+            trapElement: null
+        },
+        bi = {
+            autofocus: "boolean",
+            trapElement: "element"
+        };
+    class vi extends $ {
         constructor(t) {
-            this._config = this._getConfig(t), this._isActive = !1, this._lastTabNavDirection = null
+            super(), this._config = this._getConfig(t), this._isActive = !1, this._lastTabNavDirection = null
+        }
+        static get Default() {
+            return _i
+        }
+        static get DefaultType() {
+            return bi
+        }
+        static get NAME() {
+            return "focustrap"
         }
         activate() {
-            const {
-                trapElement: t,
-                autofocus: e
-            } = this._config;
-            this._isActive || (e && t.focus(), j.off(document, wi), j.on(document, "focusin.bs.focustrap", (t => this._handleFocusin(t))), j.on(document, "keydown.tab.bs.focustrap", (t => this._handleKeydown(t))), this._isActive = !0)
+            this._isActive || (this._config.autofocus && this._config.trapElement.focus(), P.off(document, mi), P.on(document, "focusin.bs.focustrap", (t => this._handleFocusin(t))), P.on(document, "keydown.tab.bs.focustrap", (t => this._handleKeydown(t))), this._isActive = !0)
         }
         deactivate() {
-            this._isActive && (this._isActive = !1, j.off(document, wi))
+            this._isActive && (this._isActive = !1, P.off(document, mi))
         }
         _handleFocusin(t) {
             const {
-                target: e
-            } = t, {
-                trapElement: i
+                trapElement: e
             } = this._config;
-            if (e === document || e === i || i.contains(e)) return;
-            const n = V.focusableChildren(i);
-            0 === n.length ? i.focus() : this._lastTabNavDirection === Ei ? n[n.length - 1].focus() : n[0].focus()
+            if (t.target === document || t.target === e || e.contains(t.target)) return;
+            const i = z.focusableChildren(e);
+            0 === i.length ? e.focus() : this._lastTabNavDirection === gi ? i[i.length - 1].focus() : i[0].focus()
         }
         _handleKeydown(t) {
-            "Tab" === t.key && (this._lastTabNavDirection = t.shiftKey ? Ei : "forward")
+            "Tab" === t.key && (this._lastTabNavDirection = t.shiftKey ? gi : "forward")
         }
-        _getConfig(t) {
-            return t = {
-                ...vi,
-                ..."object" == typeof t ? t : {}
-            }, a("focustrap", t, yi), t
+    }
+    const yi = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
+        wi = ".sticky-top",
+        Ai = "padding-right",
+        Ei = "margin-right";
+    class Ti {
+        constructor() {
+            this._element = document.body
+        }
+        getWidth() {
+            const t = document.documentElement.clientWidth;
+            return Math.abs(window.innerWidth - t)
+        }
+        hide() {
+            const t = this.getWidth();
+            this._disableOverFlow(), this._setElementAttributes(this._element, Ai, (e => e + t)), this._setElementAttributes(yi, Ai, (e => e + t)), this._setElementAttributes(wi, Ei, (e => e - t))
+        }
+        reset() {
+            this._resetElementAttributes(this._element, "overflow"), this._resetElementAttributes(this._element, Ai), this._resetElementAttributes(yi, Ai), this._resetElementAttributes(wi, Ei)
+        }
+        isOverflowing() {
+            return this.getWidth() > 0
+        }
+        _disableOverFlow() {
+            this._saveInitialAttribute(this._element, "overflow"), this._element.style.overflow = "hidden"
+        }
+        _setElementAttributes(t, e, i) {
+            const n = this.getWidth();
+            this._applyManipulationCallback(t, (t => {
+                if (t !== this._element && window.innerWidth > t.clientWidth + n) return;
+                this._saveInitialAttribute(t, e);
+                const s = window.getComputedStyle(t).getPropertyValue(e);
+                t.style.setProperty(e, `${i(Number.parseFloat(s))}px`)
+            }))
+        }
+        _saveInitialAttribute(t, e) {
+            const i = t.style.getPropertyValue(e);
+            i && H.setDataAttribute(t, e, i)
+        }
+        _resetElementAttributes(t, e) {
+            this._applyManipulationCallback(t, (t => {
+                const i = H.getDataAttribute(t, e);
+                null !== i ? (H.removeDataAttribute(t, e), t.style.setProperty(e, i)) : t.style.removeProperty(e)
+            }))
+        }
+        _applyManipulationCallback(t, e) {
+            if (o(t)) e(t);
+            else
+                for (const i of z.find(t, this._element)) e(i)
         }
     }
-    const Ti = "modal",
-        Oi = "Escape",
-        Ci = {
+    const Ci = ".bs.modal",
+        Oi = "hidden.bs.modal",
+        xi = "show.bs.modal",
+        ki = "modal-open",
+        Li = "show",
+        Si = "modal-static",
+        Di = {
             backdrop: !0,
-            keyboard: !0,
-            focus: !0
+            focus: !0,
+            keyboard: !0
         },
-        ki = {
+        Ii = {
             backdrop: "(boolean|string)",
-            keyboard: "boolean",
-            focus: "boolean"
-        },
-        Li = "hidden.bs.modal",
-        xi = "show.bs.modal",
-        Di = "resize.bs.modal",
-        Si = "click.dismiss.bs.modal",
-        Ni = "keydown.dismiss.bs.modal",
-        Ii = "mousedown.dismiss.bs.modal",
-        Pi = "modal-open",
-        ji = "show",
-        Mi = "modal-static";
-    class Hi extends B {
+            focus: "boolean",
+            keyboard: "boolean"
+        };
+    class Ni extends W {
         constructor(t, e) {
-            super(t), this._config = this._getConfig(e), this._dialog = V.findOne(".modal-dialog", this._element), this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._isShown = !1, this._ignoreBackdropClick = !1, this._isTransitioning = !1, this._scrollBar = new fi
+            super(t, e), this._dialog = z.findOne(".modal-dialog", this._element), this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._isShown = !1, this._isTransitioning = !1, this._scrollBar = new Ti, this._addEventListeners()
         }
         static get Default() {
-            return Ci
+            return Di
+        }
+        static get DefaultType() {
+            return Ii
         }
         static get NAME() {
-            return Ti
+            return "modal"
         }
         toggle(t) {
             return this._isShown ? this.hide() : this.show(t)
         }
         show(t) {
-            this._isShown || this._isTransitioning || j.trigger(this._element, xi, {
+            this._isShown || this._isTransitioning || P.trigger(this._element, xi, {
                 relatedTarget: t
-            }).defaultPrevented || (this._isShown = !0, this._isAnimated() && (this._isTransitioning = !0), this._scrollBar.hide(), document.body.classList.add(Pi), this._adjustDialog(), this._setEscapeEvent(), this._setResizeEvent(), j.on(this._dialog, Ii, (() => {
-                j.one(this._element, "mouseup.dismiss.bs.modal", (t => {
-                    t.target === this._element && (this._ignoreBackdropClick = !0)
-                }))
-            })), this._showBackdrop((() => this._showElement(t))))
+            }).defaultPrevented || (this._isShown = !0, this._isTransitioning = !0, this._scrollBar.hide(), document.body.classList.add(ki), this._adjustDialog(), this._backdrop.show((() => this._showElement(t))))
         }
         hide() {
-            if (!this._isShown || this._isTransitioning) return;
-            if (j.trigger(this._element, "hide.bs.modal").defaultPrevented) return;
-            this._isShown = !1;
-            const t = this._isAnimated();
-            t && (this._isTransitioning = !0), this._setEscapeEvent(), this._setResizeEvent(), this._focustrap.deactivate(), this._element.classList.remove(ji), j.off(this._element, Si), j.off(this._dialog, Ii), this._queueCallback((() => this._hideModal()), this._element, t)
+            this._isShown && !this._isTransitioning && (P.trigger(this._element, "hide.bs.modal").defaultPrevented || (this._isShown = !1, this._isTransitioning = !0, this._focustrap.deactivate(), this._element.classList.remove(Li), this._queueCallback((() => this._hideModal()), this._element, this._isAnimated())))
         }
         dispose() {
-            [window, this._dialog].forEach((t => j.off(t, ".bs.modal"))), this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
+            P.off(window, Ci), P.off(this._dialog, Ci), this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
         }
         handleUpdate() {
             this._adjustDialog()
         }
         _initializeBackDrop() {
-            return new bi({
+            return new pi({
                 isVisible: Boolean(this._config.backdrop),
                 isAnimated: this._isAnimated()
             })
         }
         _initializeFocusTrap() {
-            return new Ai({
+            return new vi({
                 trapElement: this._element
             })
         }
-        _getConfig(t) {
-            return t = {
-                ...Ci,
-                ...U.getDataAttributes(this._element),
-                ..."object" == typeof t ? t : {}
-            }, a(Ti, t, ki), t
-        }
         _showElement(t) {
-            const e = this._isAnimated(),
-                i = V.findOne(".modal-body", this._dialog);
-            this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE || document.body.append(this._element), this._element.style.display = "block", this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.scrollTop = 0, i && (i.scrollTop = 0), e && u(this._element), this._element.classList.add(ji), this._queueCallback((() => {
-                this._config.focus && this._focustrap.activate(), this._isTransitioning = !1, j.trigger(this._element, "shown.bs.modal", {
+            document.body.contains(this._element) || document.body.append(this._element), this._element.style.display = "block", this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.scrollTop = 0;
+            const e = z.findOne(".modal-body", this._dialog);
+            e && (e.scrollTop = 0), d(this._element), this._element.classList.add(Li), this._queueCallback((() => {
+                this._config.focus && this._focustrap.activate(), this._isTransitioning = !1, P.trigger(this._element, "shown.bs.modal", {
                     relatedTarget: t
                 })
-            }), this._dialog, e)
-        }
-        _setEscapeEvent() {
-            this._isShown ? j.on(this._element, Ni, (t => {
-                this._config.keyboard && t.key === Oi ? (t.preventDefault(), this.hide()) : this._config.keyboard || t.key !== Oi || this._triggerBackdropTransition()
-            })) : j.off(this._element, Ni)
+            }), this._dialog, this._isAnimated())
         }
-        _setResizeEvent() {
-            this._isShown ? j.on(window, Di, (() => this._adjustDialog())) : j.off(window, Di)
+        _addEventListeners() {
+            P.on(this._element, "keydown.dismiss.bs.modal", (t => {
+                "Escape" === t.key && (this._config.keyboard ? this.hide() : this._triggerBackdropTransition())
+            })), P.on(window, "resize.bs.modal", (() => {
+                this._isShown && !this._isTransitioning && this._adjustDialog()
+            })), P.on(this._element, "mousedown.dismiss.bs.modal", (t => {
+                P.one(this._element, "click.dismiss.bs.modal", (e => {
+                    this._element === t.target && this._element === e.target && ("static" !== this._config.backdrop ? this._config.backdrop && this.hide() : this._triggerBackdropTransition())
+                }))
+            }))
         }
         _hideModal() {
             this._element.style.display = "none", this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._isTransitioning = !1, this._backdrop.hide((() => {
-                document.body.classList.remove(Pi), this._resetAdjustments(), this._scrollBar.reset(), j.trigger(this._element, Li)
+                document.body.classList.remove(ki), this._resetAdjustments(), this._scrollBar.reset(), P.trigger(this._element, Oi)
             }))
         }
-        _showBackdrop(t) {
-            j.on(this._element, Si, (t => {
-                this._ignoreBackdropClick ? this._ignoreBackdropClick = !1 : t.target === t.currentTarget && (!0 === this._config.backdrop ? this.hide() : "static" === this._config.backdrop && this._triggerBackdropTransition())
-            })), this._backdrop.show(t)
-        }
         _isAnimated() {
             return this._element.classList.contains("fade")
         }
         _triggerBackdropTransition() {
-            if (j.trigger(this._element, "hidePrevented.bs.modal").defaultPrevented) return;
-            const {
-                classList: t,
-                scrollHeight: e,
-                style: i
-            } = this._element, n = e > document.documentElement.clientHeight;
-            !n && "hidden" === i.overflowY || t.contains(Mi) || (n || (i.overflowY = "hidden"), t.add(Mi), this._queueCallback((() => {
-                t.remove(Mi), n || this._queueCallback((() => {
-                    i.overflowY = ""
+            if (P.trigger(this._element, "hidePrevented.bs.modal").defaultPrevented) return;
+            const t = this._element.scrollHeight > document.documentElement.clientHeight,
+                e = this._element.style.overflowY;
+            "hidden" === e || this._element.classList.contains(Si) || (t || (this._element.style.overflowY = "hidden"), this._element.classList.add(Si), this._queueCallback((() => {
+                this._element.classList.remove(Si), this._queueCallback((() => {
+                    this._element.style.overflowY = e
                 }), this._dialog)
             }), this._dialog), this._element.focus())
         }
         _adjustDialog() {
             const t = this._element.scrollHeight > document.documentElement.clientHeight,
                 e = this._scrollBar.getWidth(),
                 i = e > 0;
-            (!i && t && !m() || i && !t && m()) && (this._element.style.paddingLeft = `${e}px`), (i && !t && !m() || !i && t && m()) && (this._element.style.paddingRight = `${e}px`)
+            if (i && !t) {
+                const t = p() ? "paddingLeft" : "paddingRight";
+                this._element.style[t] = `${e}px`
+            }
+            if (!i && t) {
+                const t = p() ? "paddingRight" : "paddingLeft";
+                this._element.style[t] = `${e}px`
+            }
         }
         _resetAdjustments() {
             this._element.style.paddingLeft = "", this._element.style.paddingRight = ""
         }
         static jQueryInterface(t, e) {
             return this.each((function() {
-                const i = Hi.getOrCreateInstance(this, t);
+                const i = Ni.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
                     i[t](e)
                 }
             }))
         }
     }
-    j.on(document, "click.bs.modal.data-api", '[data-bs-toggle="modal"]', (function(t) {
-        const e = n(this);
-        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), j.one(e, xi, (t => {
-            t.defaultPrevented || j.one(e, Li, (() => {
-                l(this) && this.focus()
+    P.on(document, "click.bs.modal.data-api", '[data-bs-toggle="modal"]', (function(t) {
+        const e = z.getElementFromSelector(this);
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), P.one(e, xi, (t => {
+            t.defaultPrevented || P.one(e, Oi, (() => {
+                a(this) && this.focus()
             }))
         }));
-        const i = V.findOne(".modal.show");
-        i && Hi.getInstance(i).hide(), Hi.getOrCreateInstance(e).toggle(this)
-    })), R(Hi), g(Hi);
-    const Bi = "offcanvas",
-        Ri = {
+        const i = z.findOne(".modal.show");
+        i && Ni.getInstance(i).hide(), Ni.getOrCreateInstance(e).toggle(this)
+    })), R(Ni), m(Ni);
+    const Pi = "show",
+        Mi = "showing",
+        ji = "hiding",
+        Fi = ".offcanvas.show",
+        Hi = "hidePrevented.bs.offcanvas",
+        $i = "hidden.bs.offcanvas",
+        Wi = {
             backdrop: !0,
             keyboard: !0,
             scroll: !1
         },
-        Wi = {
-            backdrop: "boolean",
+        Bi = {
+            backdrop: "(boolean|string)",
             keyboard: "boolean",
             scroll: "boolean"
-        },
-        $i = "show",
-        zi = ".offcanvas.show",
-        qi = "hidden.bs.offcanvas";
-    class Fi extends B {
+        };
+    class zi extends W {
         constructor(t, e) {
-            super(t), this._config = this._getConfig(e), this._isShown = !1, this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._addEventListeners()
+            super(t, e), this._isShown = !1, this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._addEventListeners()
         }
-        static get NAME() {
+        static get Default() {
+            return Wi
+        }
+        static get DefaultType() {
             return Bi
         }
-        static get Default() {
-            return Ri
+        static get NAME() {
+            return "offcanvas"
         }
         toggle(t) {
             return this._isShown ? this.hide() : this.show(t)
         }
         show(t) {
-            this._isShown || j.trigger(this._element, "show.bs.offcanvas", {
+            this._isShown || P.trigger(this._element, "show.bs.offcanvas", {
                 relatedTarget: t
-            }).defaultPrevented || (this._isShown = !0, this._element.style.visibility = "visible", this._backdrop.show(), this._config.scroll || (new fi).hide(), this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.classList.add($i), this._queueCallback((() => {
-                this._config.scroll || this._focustrap.activate(), j.trigger(this._element, "shown.bs.offcanvas", {
+            }).defaultPrevented || (this._isShown = !0, this._backdrop.show(), this._config.scroll || (new Ti).hide(), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.classList.add(Mi), this._queueCallback((() => {
+                this._config.scroll && !this._config.backdrop || this._focustrap.activate(), this._element.classList.add(Pi), this._element.classList.remove(Mi), P.trigger(this._element, "shown.bs.offcanvas", {
                     relatedTarget: t
                 })
             }), this._element, !0))
         }
         hide() {
-            this._isShown && (j.trigger(this._element, "hide.bs.offcanvas").defaultPrevented || (this._focustrap.deactivate(), this._element.blur(), this._isShown = !1, this._element.classList.remove($i), this._backdrop.hide(), this._queueCallback((() => {
-                this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._element.style.visibility = "hidden", this._config.scroll || (new fi).reset(), j.trigger(this._element, qi)
+            this._isShown && (P.trigger(this._element, "hide.bs.offcanvas").defaultPrevented || (this._focustrap.deactivate(), this._element.blur(), this._isShown = !1, this._element.classList.add(ji), this._backdrop.hide(), this._queueCallback((() => {
+                this._element.classList.remove(Pi, ji), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._config.scroll || (new Ti).reset(), P.trigger(this._element, $i)
             }), this._element, !0)))
         }
         dispose() {
             this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
         }
-        _getConfig(t) {
-            return t = {
-                ...Ri,
-                ...U.getDataAttributes(this._element),
-                ..."object" == typeof t ? t : {}
-            }, a(Bi, t, Wi), t
-        }
         _initializeBackDrop() {
-            return new bi({
+            const t = Boolean(this._config.backdrop);
+            return new pi({
                 className: "offcanvas-backdrop",
-                isVisible: this._config.backdrop,
+                isVisible: t,
                 isAnimated: !0,
                 rootElement: this._element.parentNode,
-                clickCallback: () => this.hide()
+                clickCallback: t ? () => {
+                    "static" !== this._config.backdrop ? this.hide() : P.trigger(this._element, Hi)
+                } : null
             })
         }
         _initializeFocusTrap() {
-            return new Ai({
+            return new vi({
                 trapElement: this._element
             })
         }
         _addEventListeners() {
-            j.on(this._element, "keydown.dismiss.bs.offcanvas", (t => {
-                this._config.keyboard && "Escape" === t.key && this.hide()
+            P.on(this._element, "keydown.dismiss.bs.offcanvas", (t => {
+                "Escape" === t.key && (this._config.keyboard ? this.hide() : P.trigger(this._element, Hi))
             }))
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = Fi.getOrCreateInstance(this, t);
+                const e = zi.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    j.on(document, "click.bs.offcanvas.data-api", '[data-bs-toggle="offcanvas"]', (function(t) {
-        const e = n(this);
-        if (["A", "AREA"].includes(this.tagName) && t.preventDefault(), c(this)) return;
-        j.one(e, qi, (() => {
-            l(this) && this.focus()
+    P.on(document, "click.bs.offcanvas.data-api", '[data-bs-toggle="offcanvas"]', (function(t) {
+        const e = z.getElementFromSelector(this);
+        if (["A", "AREA"].includes(this.tagName) && t.preventDefault(), l(this)) return;
+        P.one(e, $i, (() => {
+            a(this) && this.focus()
         }));
-        const i = V.findOne(zi);
-        i && i !== e && Fi.getInstance(i).hide(), Fi.getOrCreateInstance(e).toggle(this)
-    })), j.on(window, "load.bs.offcanvas.data-api", (() => V.find(zi).forEach((t => Fi.getOrCreateInstance(t).show())))), R(Fi), g(Fi);
-    const Ui = new Set(["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"]),
-        Vi = /^(?:(?:https?|mailto|ftp|tel|file|sms):|[^#&/:?]*(?:[#/?]|$))/i,
-        Ki = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[\d+/a-z]+=*$/i,
-        Xi = (t, e) => {
+        const i = z.findOne(Fi);
+        i && i !== e && zi.getInstance(i).hide(), zi.getOrCreateInstance(e).toggle(this)
+    })), P.on(window, "load.bs.offcanvas.data-api", (() => {
+        for (const t of z.find(Fi)) zi.getOrCreateInstance(t).show()
+    })), P.on(window, "resize.bs.offcanvas", (() => {
+        for (const t of z.find("[aria-modal][class*=show][class*=offcanvas-]")) "fixed" !== getComputedStyle(t).position && zi.getOrCreateInstance(t).hide()
+    })), R(zi), m(zi);
+    const Ri = {
+            "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
+            a: ["target", "href", "title", "rel"],
+            area: [],
+            b: [],
+            br: [],
+            col: [],
+            code: [],
+            div: [],
+            em: [],
+            hr: [],
+            h1: [],
+            h2: [],
+            h3: [],
+            h4: [],
+            h5: [],
+            h6: [],
+            i: [],
+            img: ["src", "srcset", "alt", "title", "width", "height"],
+            li: [],
+            ol: [],
+            p: [],
+            pre: [],
+            s: [],
+            small: [],
+            span: [],
+            sub: [],
+            sup: [],
+            strong: [],
+            u: [],
+            ul: []
+        },
+        qi = new Set(["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"]),
+        Vi = /^(?!javascript:)(?:[a-z0-9+.-]+:|[^&:/?#]*(?:[/?#]|$))/i,
+        Ki = (t, e) => {
             const i = t.nodeName.toLowerCase();
-            if (e.includes(i)) return !Ui.has(i) || Boolean(Vi.test(t.nodeValue) || Ki.test(t.nodeValue));
-            const n = e.filter((t => t instanceof RegExp));
-            for (let t = 0, e = n.length; t < e; t++)
-                if (n[t].test(i)) return !0;
-            return !1
-        };
-
-    function Yi(t, e, i) {
-        if (!t.length) return t;
-        if (i && "function" == typeof i) return i(t);
-        const n = (new window.DOMParser).parseFromString(t, "text/html"),
-            s = [].concat(...n.body.querySelectorAll("*"));
-        for (let t = 0, i = s.length; t < i; t++) {
-            const i = s[t],
-                n = i.nodeName.toLowerCase();
-            if (!Object.keys(e).includes(n)) {
-                i.remove();
-                continue
-            }
-            const o = [].concat(...i.attributes),
-                r = [].concat(e["*"] || [], e[n] || []);
-            o.forEach((t => {
-                Xi(t, r) || i.removeAttribute(t.nodeName)
-            }))
-        }
-        return n.body.innerHTML
-    }
-    const Qi = "tooltip",
-        Gi = new Set(["sanitize", "allowList", "sanitizeFn"]),
-        Zi = {
-            animation: "boolean",
-            template: "string",
-            title: "(string|element|function)",
-            trigger: "string",
-            delay: "(number|object)",
+            return e.includes(i) ? !qi.has(i) || Boolean(Vi.test(t.nodeValue)) : e.filter((t => t instanceof RegExp)).some((t => t.test(i)))
+        },
+        Qi = {
+            allowList: Ri,
+            content: {},
+            extraClass: "",
+            html: !1,
+            sanitize: !0,
+            sanitizeFn: null,
+            template: "<div></div>"
+        },
+        Xi = {
+            allowList: "object",
+            content: "object",
+            extraClass: "(string|function)",
             html: "boolean",
-            selector: "(string|boolean)",
-            placement: "(string|function)",
-            offset: "(array|string|function)",
-            container: "(string|element|boolean)",
-            fallbackPlacements: "array",
-            boundary: "(string|element)",
-            customClass: "(string|function)",
             sanitize: "boolean",
             sanitizeFn: "(null|function)",
-            allowList: "object",
-            popperConfig: "(null|object|function)"
+            template: "string"
         },
-        Ji = {
+        Yi = {
+            entry: "(string|element|function|null)",
+            selector: "(string|element)"
+        };
+    class Ui extends $ {
+        constructor(t) {
+            super(), this._config = this._getConfig(t)
+        }
+        static get Default() {
+            return Qi
+        }
+        static get DefaultType() {
+            return Xi
+        }
+        static get NAME() {
+            return "TemplateFactory"
+        }
+        getContent() {
+            return Object.values(this._config.content).map((t => this._resolvePossibleFunction(t))).filter(Boolean)
+        }
+        hasContent() {
+            return this.getContent().length > 0
+        }
+        changeContent(t) {
+            return this._checkContent(t), this._config.content = {
+                ...this._config.content,
+                ...t
+            }, this
+        }
+        toHtml() {
+            const t = document.createElement("div");
+            t.innerHTML = this._maybeSanitize(this._config.template);
+            for (const [e, i] of Object.entries(this._config.content)) this._setContent(t, i, e);
+            const e = t.children[0],
+                i = this._resolvePossibleFunction(this._config.extraClass);
+            return i && e.classList.add(...i.split(" ")), e
+        }
+        _typeCheckConfig(t) {
+            super._typeCheckConfig(t), this._checkContent(t.content)
+        }
+        _checkContent(t) {
+            for (const [e, i] of Object.entries(t)) super._typeCheckConfig({
+                selector: e,
+                entry: i
+            }, Yi)
+        }
+        _setContent(t, e, i) {
+            const n = z.findOne(i, t);
+            n && ((e = this._resolvePossibleFunction(e)) ? o(e) ? this._putElementInTemplate(r(e), n) : this._config.html ? n.innerHTML = this._maybeSanitize(e) : n.textContent = e : n.remove())
+        }
+        _maybeSanitize(t) {
+            return this._config.sanitize ? function(t, e, i) {
+                if (!t.length) return t;
+                if (i && "function" == typeof i) return i(t);
+                const n = (new window.DOMParser).parseFromString(t, "text/html"),
+                    s = [].concat(...n.body.querySelectorAll("*"));
+                for (const t of s) {
+                    const i = t.nodeName.toLowerCase();
+                    if (!Object.keys(e).includes(i)) {
+                        t.remove();
+                        continue
+                    }
+                    const n = [].concat(...t.attributes),
+                        s = [].concat(e["*"] || [], e[i] || []);
+                    for (const e of n) Ki(e, s) || t.removeAttribute(e.nodeName)
+                }
+                return n.body.innerHTML
+            }(t, this._config.allowList, this._config.sanitizeFn) : t
+        }
+        _resolvePossibleFunction(t) {
+            return g(t, [this])
+        }
+        _putElementInTemplate(t, e) {
+            if (this._config.html) return e.innerHTML = "", void e.append(t);
+            e.textContent = t.textContent
+        }
+    }
+    const Gi = new Set(["sanitize", "allowList", "sanitizeFn"]),
+        Ji = "fade",
+        Zi = "show",
+        tn = ".modal",
+        en = "hide.bs.modal",
+        nn = "hover",
+        sn = "focus",
+        on = {
             AUTO: "auto",
             TOP: "top",
-            RIGHT: m() ? "left" : "right",
+            RIGHT: p() ? "left" : "right",
             BOTTOM: "bottom",
-            LEFT: m() ? "right" : "left"
+            LEFT: p() ? "right" : "left"
         },
-        tn = {
+        rn = {
+            allowList: Ri,
             animation: !0,
-            template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
-            trigger: "hover focus",
-            title: "",
+            boundary: "clippingParents",
+            container: !1,
+            customClass: "",
             delay: 0,
+            fallbackPlacements: ["top", "right", "bottom", "left"],
             html: !1,
-            selector: !1,
+            offset: [0, 6],
             placement: "top",
-            offset: [0, 0],
-            container: !1,
-            fallbackPlacements: ["top", "right", "bottom", "left"],
-            boundary: "clippingParents",
-            customClass: "",
+            popperConfig: null,
             sanitize: !0,
             sanitizeFn: null,
-            allowList: {
-                "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
-                a: ["target", "href", "title", "rel"],
-                area: [],
-                b: [],
-                br: [],
-                col: [],
-                code: [],
-                div: [],
-                em: [],
-                hr: [],
-                h1: [],
-                h2: [],
-                h3: [],
-                h4: [],
-                h5: [],
-                h6: [],
-                i: [],
-                img: ["src", "srcset", "alt", "title", "width", "height"],
-                li: [],
-                ol: [],
-                p: [],
-                pre: [],
-                s: [],
-                small: [],
-                span: [],
-                sub: [],
-                sup: [],
-                strong: [],
-                u: [],
-                ul: []
-            },
-            popperConfig: null
+            selector: !1,
+            template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
+            title: "",
+            trigger: "hover focus"
         },
-        en = {
-            HIDE: "hide.bs.tooltip",
-            HIDDEN: "hidden.bs.tooltip",
-            SHOW: "show.bs.tooltip",
-            SHOWN: "shown.bs.tooltip",
-            INSERTED: "inserted.bs.tooltip",
-            CLICK: "click.bs.tooltip",
-            FOCUSIN: "focusin.bs.tooltip",
-            FOCUSOUT: "focusout.bs.tooltip",
-            MOUSEENTER: "mouseenter.bs.tooltip",
-            MOUSELEAVE: "mouseleave.bs.tooltip"
-        },
-        nn = "fade",
-        sn = "show",
-        on = "show",
-        rn = "out",
-        an = ".tooltip-inner",
-        ln = ".modal",
-        cn = "hide.bs.modal",
-        hn = "hover",
-        dn = "focus";
-    class un extends B {
+        an = {
+            allowList: "object",
+            animation: "boolean",
+            boundary: "(string|element)",
+            container: "(string|element|boolean)",
+            customClass: "(string|function)",
+            delay: "(number|object)",
+            fallbackPlacements: "array",
+            html: "boolean",
+            offset: "(array|string|function)",
+            placement: "(string|function)",
+            popperConfig: "(null|object|function)",
+            sanitize: "boolean",
+            sanitizeFn: "(null|function)",
+            selector: "(string|boolean)",
+            template: "string",
+            title: "(string|element|function)",
+            trigger: "string"
+        };
+    class ln extends W {
         constructor(t, e) {
-            if (void 0 === Fe) throw new TypeError("Bootstrap's tooltips require Popper (https://popper.js.org)");
-            super(t), this._isEnabled = !0, this._timeout = 0, this._hoverState = "", this._activeTrigger = {}, this._popper = null, this._config = this._getConfig(e), this.tip = null, this._setListeners()
+            if (void 0 === Ve) throw new TypeError("Bootstrap's tooltips require Popper (https://popper.js.org)");
+            super(t, e), this._isEnabled = !0, this._timeout = 0, this._isHovered = null, this._activeTrigger = {}, this._popper = null, this._templateFactory = null, this._newContent = null, this.tip = null, this._setListeners(), this._config.selector || this._fixTitle()
         }
         static get Default() {
-            return tn
-        }
-        static get NAME() {
-            return Qi
-        }
-        static get Event() {
-            return en
+            return rn
         }
         static get DefaultType() {
-            return Zi
+            return an
+        }
+        static get NAME() {
+            return "tooltip"
         }
         enable() {
             this._isEnabled = !0
         }
         disable() {
             this._isEnabled = !1
         }
         toggleEnabled() {
             this._isEnabled = !this._isEnabled
         }
-        toggle(t) {
-            if (this._isEnabled)
-                if (t) {
-                    const e = this._initializeOnDelegatedTarget(t);
-                    e._activeTrigger.click = !e._activeTrigger.click, e._isWithActiveTrigger() ? e._enter(null, e) : e._leave(null, e)
-                } else {
-                    if (this.getTipElement().classList.contains(sn)) return void this._leave(null, this);
-                    this._enter(null, this)
-                }
+        toggle() {
+            this._isEnabled && (this._activeTrigger.click = !this._activeTrigger.click, this._isShown() ? this._leave() : this._enter())
         }
         dispose() {
-            clearTimeout(this._timeout), j.off(this._element.closest(ln), cn, this._hideModalHandler), this.tip && this.tip.remove(), this._disposePopper(), super.dispose()
+            clearTimeout(this._timeout), P.off(this._element.closest(tn), en, this._hideModalHandler), this._element.getAttribute("data-bs-original-title") && this._element.setAttribute("title", this._element.getAttribute("data-bs-original-title")), this._disposePopper(), super.dispose()
         }
         show() {
             if ("none" === this._element.style.display) throw new Error("Please use show on visible elements");
-            if (!this.isWithContent() || !this._isEnabled) return;
-            const t = j.trigger(this._element, this.constructor.Event.SHOW),
-                e = h(this._element),
-                i = null === e ? this._element.ownerDocument.documentElement.contains(this._element) : e.contains(this._element);
-            if (t.defaultPrevented || !i) return;
-            "tooltip" === this.constructor.NAME && this.tip && this.getTitle() !== this.tip.querySelector(an).innerHTML && (this._disposePopper(), this.tip.remove(), this.tip = null);
-            const n = this.getTipElement(),
-                s = (t => {
-                    do {
-                        t += Math.floor(1e6 * Math.random())
-                    } while (document.getElementById(t));
-                    return t
-                })(this.constructor.NAME);
-            n.setAttribute("id", s), this._element.setAttribute("aria-describedby", s), this._config.animation && n.classList.add(nn);
-            const o = "function" == typeof this._config.placement ? this._config.placement.call(this, n, this._element) : this._config.placement,
-                r = this._getAttachment(o);
-            this._addAttachmentClass(r);
+            if (!this._isWithContent() || !this._isEnabled) return;
+            const t = P.trigger(this._element, this.constructor.eventName("show")),
+                e = (c(this._element) || this._element.ownerDocument.documentElement).contains(this._element);
+            if (t.defaultPrevented || !e) return;
+            this._disposePopper();
+            const i = this._getTipElement();
+            this._element.setAttribute("aria-describedby", i.getAttribute("id"));
             const {
-                container: a
+                container: n
             } = this._config;
-            H.set(n, this.constructor.DATA_KEY, this), this._element.ownerDocument.documentElement.contains(this.tip) || (a.append(n), j.trigger(this._element, this.constructor.Event.INSERTED)), this._popper ? this._popper.update() : this._popper = qe(this._element, n, this._getPopperConfig(r)), n.classList.add(sn);
-            const l = this._resolvePossibleFunction(this._config.customClass);
-            l && n.classList.add(...l.split(" ")), "ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => {
-                j.on(t, "mouseover", d)
-            }));
-            const c = this.tip.classList.contains(nn);
+            if (this._element.ownerDocument.documentElement.contains(this.tip) || (n.append(i), P.trigger(this._element, this.constructor.eventName("inserted"))), this._popper = this._createPopper(i), i.classList.add(Zi), "ontouchstart" in document.documentElement)
+                for (const t of [].concat(...document.body.children)) P.on(t, "mouseover", h);
             this._queueCallback((() => {
-                const t = this._hoverState;
-                this._hoverState = null, j.trigger(this._element, this.constructor.Event.SHOWN), t === rn && this._leave(null, this)
-            }), this.tip, c)
+                P.trigger(this._element, this.constructor.eventName("shown")), !1 === this._isHovered && this._leave(), this._isHovered = !1
+            }), this.tip, this._isAnimated())
         }
         hide() {
-            if (!this._popper) return;
-            const t = this.getTipElement();
-            if (j.trigger(this._element, this.constructor.Event.HIDE).defaultPrevented) return;
-            t.classList.remove(sn), "ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => j.off(t, "mouseover", d))), this._activeTrigger.click = !1, this._activeTrigger.focus = !1, this._activeTrigger.hover = !1;
-            const e = this.tip.classList.contains(nn);
-            this._queueCallback((() => {
-                this._isWithActiveTrigger() || (this._hoverState !== on && t.remove(), this._cleanTipClass(), this._element.removeAttribute("aria-describedby"), j.trigger(this._element, this.constructor.Event.HIDDEN), this._disposePopper())
-            }), this.tip, e), this._hoverState = ""
+            if (this._isShown() && !P.trigger(this._element, this.constructor.eventName("hide")).defaultPrevented) {
+                if (this._getTipElement().classList.remove(Zi), "ontouchstart" in document.documentElement)
+                    for (const t of [].concat(...document.body.children)) P.off(t, "mouseover", h);
+                this._activeTrigger.click = !1, this._activeTrigger.focus = !1, this._activeTrigger.hover = !1, this._isHovered = null, this._queueCallback((() => {
+                    this._isWithActiveTrigger() || (this._isHovered || this._disposePopper(), this._element.removeAttribute("aria-describedby"), P.trigger(this._element, this.constructor.eventName("hidden")))
+                }), this.tip, this._isAnimated())
+            }
         }
         update() {
-            null !== this._popper && this._popper.update()
+            this._popper && this._popper.update()
         }
-        isWithContent() {
-            return Boolean(this.getTitle())
+        _isWithContent() {
+            return Boolean(this._getTitle())
         }
-        getTipElement() {
-            if (this.tip) return this.tip;
-            const t = document.createElement("div");
-            t.innerHTML = this._config.template;
-            const e = t.children[0];
-            return this.setContent(e), e.classList.remove(nn, sn), this.tip = e, this.tip
+        _getTipElement() {
+            return this.tip || (this.tip = this._createTipElement(this._newContent || this._getContentForTemplate())), this.tip
+        }
+        _createTipElement(t) {
+            const e = this._getTemplateFactory(t).toHtml();
+            if (!e) return null;
+            e.classList.remove(Ji, Zi), e.classList.add(`bs-${this.constructor.NAME}-auto`);
+            const i = (t => {
+                do {
+                    t += Math.floor(1e6 * Math.random())
+                } while (document.getElementById(t));
+                return t
+            })(this.constructor.NAME).toString();
+            return e.setAttribute("id", i), this._isAnimated() && e.classList.add(Ji), e
         }
         setContent(t) {
-            this._sanitizeAndSetContent(t, this.getTitle(), an)
+            this._newContent = t, this._isShown() && (this._disposePopper(), this.show())
         }
-        _sanitizeAndSetContent(t, e, i) {
-            const n = V.findOne(i, t);
-            e || !n ? this.setElementContent(n, e) : n.remove()
+        _getTemplateFactory(t) {
+            return this._templateFactory ? this._templateFactory.changeContent(t) : this._templateFactory = new Ui({
+                ...this._config,
+                content: t,
+                extraClass: this._resolvePossibleFunction(this._config.customClass)
+            }), this._templateFactory
         }
-        setElementContent(t, e) {
-            if (null !== t) return o(e) ? (e = r(e), void(this._config.html ? e.parentNode !== t && (t.innerHTML = "", t.append(e)) : t.textContent = e.textContent)) : void(this._config.html ? (this._config.sanitize && (e = Yi(e, this._config.allowList, this._config.sanitizeFn)), t.innerHTML = e) : t.textContent = e)
+        _getContentForTemplate() {
+            return {
+                ".tooltip-inner": this._getTitle()
+            }
+        }
+        _getTitle() {
+            return this._resolvePossibleFunction(this._config.title) || this._element.getAttribute("data-bs-original-title")
         }
-        getTitle() {
-            const t = this._element.getAttribute("data-bs-original-title") || this._config.title;
-            return this._resolvePossibleFunction(t)
+        _initializeOnDelegatedTarget(t) {
+            return this.constructor.getOrCreateInstance(t.delegateTarget, this._getDelegateConfig())
         }
-        updateAttachment(t) {
-            return "right" === t ? "end" : "left" === t ? "start" : t
+        _isAnimated() {
+            return this._config.animation || this.tip && this.tip.classList.contains(Ji)
         }
-        _initializeOnDelegatedTarget(t, e) {
-            return e || this.constructor.getOrCreateInstance(t.delegateTarget, this._getDelegateConfig())
+        _isShown() {
+            return this.tip && this.tip.classList.contains(Zi)
+        }
+        _createPopper(t) {
+            const e = g(this._config.placement, [this, t, this._element]),
+                i = on[e.toUpperCase()];
+            return qe(this._element, t, this._getPopperConfig(i))
         }
         _getOffset() {
             const {
                 offset: t
             } = this._config;
             return "string" == typeof t ? t.split(",").map((t => Number.parseInt(t, 10))) : "function" == typeof t ? e => t(e, this._element) : t
         }
         _resolvePossibleFunction(t) {
-            return "function" == typeof t ? t.call(this._element) : t
+            return g(t, [this._element])
         }
         _getPopperConfig(t) {
             const e = {
                 placement: t,
                 modifiers: [{
                     name: "flip",
                     options: {
@@ -2668,389 +2805,416 @@
                     }
                 }, {
                     name: "arrow",
                     options: {
                         element: `.${this.constructor.NAME}-arrow`
                     }
                 }, {
-                    name: "onChange",
+                    name: "preSetPlacement",
                     enabled: !0,
-                    phase: "afterWrite",
-                    fn: t => this._handlePopperPlacementChange(t)
-                }],
-                onFirstUpdate: t => {
-                    t.options.placement !== t.placement && this._handlePopperPlacementChange(t)
-                }
+                    phase: "beforeMain",
+                    fn: t => {
+                        this._getTipElement().setAttribute("data-popper-placement", t.state.placement)
+                    }
+                }]
             };
             return {
                 ...e,
-                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(e) : this._config.popperConfig
+                ...g(this._config.popperConfig, [e])
             }
         }
-        _addAttachmentClass(t) {
-            this.getTipElement().classList.add(`${this._getBasicClassPrefix()}-${this.updateAttachment(t)}`)
-        }
-        _getAttachment(t) {
-            return Ji[t.toUpperCase()]
-        }
         _setListeners() {
-            this._config.trigger.split(" ").forEach((t => {
-                if ("click" === t) j.on(this._element, this.constructor.Event.CLICK, this._config.selector, (t => this.toggle(t)));
-                else if ("manual" !== t) {
-                    const e = t === hn ? this.constructor.Event.MOUSEENTER : this.constructor.Event.FOCUSIN,
-                        i = t === hn ? this.constructor.Event.MOUSELEAVE : this.constructor.Event.FOCUSOUT;
-                    j.on(this._element, e, this._config.selector, (t => this._enter(t))), j.on(this._element, i, this._config.selector, (t => this._leave(t)))
-                }
-            })), this._hideModalHandler = () => {
+            const t = this._config.trigger.split(" ");
+            for (const e of t)
+                if ("click" === e) P.on(this._element, this.constructor.eventName("click"), this._config.selector, (t => {
+                    this._initializeOnDelegatedTarget(t).toggle()
+                }));
+                else if ("manual" !== e) {
+                const t = e === nn ? this.constructor.eventName("mouseenter") : this.constructor.eventName("focusin"),
+                    i = e === nn ? this.constructor.eventName("mouseleave") : this.constructor.eventName("focusout");
+                P.on(this._element, t, this._config.selector, (t => {
+                    const e = this._initializeOnDelegatedTarget(t);
+                    e._activeTrigger["focusin" === t.type ? sn : nn] = !0, e._enter()
+                })), P.on(this._element, i, this._config.selector, (t => {
+                    const e = this._initializeOnDelegatedTarget(t);
+                    e._activeTrigger["focusout" === t.type ? sn : nn] = e._element.contains(t.relatedTarget), e._leave()
+                }))
+            }
+            this._hideModalHandler = () => {
                 this._element && this.hide()
-            }, j.on(this._element.closest(ln), cn, this._hideModalHandler), this._config.selector ? this._config = {
-                ...this._config,
-                trigger: "manual",
-                selector: ""
-            } : this._fixTitle()
+            }, P.on(this._element.closest(tn), en, this._hideModalHandler)
         }
         _fixTitle() {
-            const t = this._element.getAttribute("title"),
-                e = typeof this._element.getAttribute("data-bs-original-title");
-            (t || "string" !== e) && (this._element.setAttribute("data-bs-original-title", t || ""), !t || this._element.getAttribute("aria-label") || this._element.textContent || this._element.setAttribute("aria-label", t), this._element.setAttribute("title", ""))
-        }
-        _enter(t, e) {
-            e = this._initializeOnDelegatedTarget(t, e), t && (e._activeTrigger["focusin" === t.type ? dn : hn] = !0), e.getTipElement().classList.contains(sn) || e._hoverState === on ? e._hoverState = on : (clearTimeout(e._timeout), e._hoverState = on, e._config.delay && e._config.delay.show ? e._timeout = setTimeout((() => {
-                e._hoverState === on && e.show()
-            }), e._config.delay.show) : e.show())
-        }
-        _leave(t, e) {
-            e = this._initializeOnDelegatedTarget(t, e), t && (e._activeTrigger["focusout" === t.type ? dn : hn] = e._element.contains(t.relatedTarget)), e._isWithActiveTrigger() || (clearTimeout(e._timeout), e._hoverState = rn, e._config.delay && e._config.delay.hide ? e._timeout = setTimeout((() => {
-                e._hoverState === rn && e.hide()
-            }), e._config.delay.hide) : e.hide())
+            const t = this._element.getAttribute("title");
+            t && (this._element.getAttribute("aria-label") || this._element.textContent.trim() || this._element.setAttribute("aria-label", t), this._element.setAttribute("data-bs-original-title", t), this._element.removeAttribute("title"))
+        }
+        _enter() {
+            this._isShown() || this._isHovered ? this._isHovered = !0 : (this._isHovered = !0, this._setTimeout((() => {
+                this._isHovered && this.show()
+            }), this._config.delay.show))
+        }
+        _leave() {
+            this._isWithActiveTrigger() || (this._isHovered = !1, this._setTimeout((() => {
+                this._isHovered || this.hide()
+            }), this._config.delay.hide))
+        }
+        _setTimeout(t, e) {
+            clearTimeout(this._timeout), this._timeout = setTimeout(t, e)
         }
         _isWithActiveTrigger() {
-            for (const t in this._activeTrigger)
-                if (this._activeTrigger[t]) return !0;
-            return !1
+            return Object.values(this._activeTrigger).includes(!0)
         }
         _getConfig(t) {
-            const e = U.getDataAttributes(this._element);
-            return Object.keys(e).forEach((t => {
-                Gi.has(t) && delete e[t]
-            })), (t = {
-                ...this.constructor.Default,
+            const e = H.getDataAttributes(this._element);
+            for (const t of Object.keys(e)) Gi.has(t) && delete e[t];
+            return t = {
                 ...e,
                 ..."object" == typeof t && t ? t : {}
-            }).container = !1 === t.container ? document.body : r(t.container), "number" == typeof t.delay && (t.delay = {
+            }, t = this._mergeConfigObj(t), t = this._configAfterMerge(t), this._typeCheckConfig(t), t
+        }
+        _configAfterMerge(t) {
+            return t.container = !1 === t.container ? document.body : r(t.container), "number" == typeof t.delay && (t.delay = {
                 show: t.delay,
                 hide: t.delay
-            }), "number" == typeof t.title && (t.title = t.title.toString()), "number" == typeof t.content && (t.content = t.content.toString()), a(Qi, t, this.constructor.DefaultType), t.sanitize && (t.template = Yi(t.template, t.allowList, t.sanitizeFn)), t
+            }), "number" == typeof t.title && (t.title = t.title.toString()), "number" == typeof t.content && (t.content = t.content.toString()), t
         }
         _getDelegateConfig() {
             const t = {};
-            for (const e in this._config) this.constructor.Default[e] !== this._config[e] && (t[e] = this._config[e]);
-            return t
-        }
-        _cleanTipClass() {
-            const t = this.getTipElement(),
-                e = new RegExp(`(^|\\s)${this._getBasicClassPrefix()}\\S+`, "g"),
-                i = t.getAttribute("class").match(e);
-            null !== i && i.length > 0 && i.map((t => t.trim())).forEach((e => t.classList.remove(e)))
-        }
-        _getBasicClassPrefix() {
-            return "bs-tooltip"
-        }
-        _handlePopperPlacementChange(t) {
-            const {
-                state: e
-            } = t;
-            e && (this.tip = e.elements.popper, this._cleanTipClass(), this._addAttachmentClass(this._getAttachment(e.placement)))
+            for (const [e, i] of Object.entries(this._config)) this.constructor.Default[e] !== i && (t[e] = i);
+            return t.selector = !1, t.trigger = "manual", t
         }
         _disposePopper() {
-            this._popper && (this._popper.destroy(), this._popper = null)
+            this._popper && (this._popper.destroy(), this._popper = null), this.tip && (this.tip.remove(), this.tip = null)
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = un.getOrCreateInstance(this, t);
+                const e = ln.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    g(un);
-    const fn = {
-            ...un.Default,
-            placement: "right",
-            offset: [0, 8],
-            trigger: "click",
+    m(ln);
+    const cn = {
+            ...ln.Default,
             content: "",
-            template: '<div class="popover" role="tooltip"><div class="popover-arrow"></div><h3 class="popover-header"></h3><div class="popover-body"></div></div>'
-        },
-        pn = {
-            ...un.DefaultType,
-            content: "(string|element|function)"
+            offset: [0, 8],
+            placement: "right",
+            template: '<div class="popover" role="tooltip"><div class="popover-arrow"></div><h3 class="popover-header"></h3><div class="popover-body"></div></div>',
+            trigger: "click"
         },
-        mn = {
-            HIDE: "hide.bs.popover",
-            HIDDEN: "hidden.bs.popover",
-            SHOW: "show.bs.popover",
-            SHOWN: "shown.bs.popover",
-            INSERTED: "inserted.bs.popover",
-            CLICK: "click.bs.popover",
-            FOCUSIN: "focusin.bs.popover",
-            FOCUSOUT: "focusout.bs.popover",
-            MOUSEENTER: "mouseenter.bs.popover",
-            MOUSELEAVE: "mouseleave.bs.popover"
+        hn = {
+            ...ln.DefaultType,
+            content: "(null|string|element|function)"
         };
-    class gn extends un {
+    class dn extends ln {
         static get Default() {
-            return fn
+            return cn
+        }
+        static get DefaultType() {
+            return hn
         }
         static get NAME() {
             return "popover"
         }
-        static get Event() {
-            return mn
-        }
-        static get DefaultType() {
-            return pn
-        }
-        isWithContent() {
-            return this.getTitle() || this._getContent()
+        _isWithContent() {
+            return this._getTitle() || this._getContent()
         }
-        setContent(t) {
-            this._sanitizeAndSetContent(t, this.getTitle(), ".popover-header"), this._sanitizeAndSetContent(t, this._getContent(), ".popover-body")
+        _getContentForTemplate() {
+            return {
+                ".popover-header": this._getTitle(),
+                ".popover-body": this._getContent()
+            }
         }
         _getContent() {
             return this._resolvePossibleFunction(this._config.content)
         }
-        _getBasicClassPrefix() {
-            return "bs-popover"
-        }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = gn.getOrCreateInstance(this, t);
+                const e = dn.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    g(gn);
-    const _n = "scrollspy",
-        bn = {
-            offset: 10,
-            method: "auto",
-            target: ""
-        },
-        vn = {
-            offset: "number",
-            method: "string",
-            target: "(string|element)"
-        },
-        yn = "active",
-        wn = ".nav-link, .list-group-item, .dropdown-item",
-        En = "position";
-    class An extends B {
+    m(dn);
+    const un = "click.bs.scrollspy",
+        fn = "active",
+        pn = "[href]",
+        mn = {
+            offset: null,
+            rootMargin: "0px 0px -25%",
+            smoothScroll: !1,
+            target: null,
+            threshold: [.1, .5, 1]
+        },
+        gn = {
+            offset: "(number|null)",
+            rootMargin: "string",
+            smoothScroll: "boolean",
+            target: "element",
+            threshold: "array"
+        };
+    class _n extends W {
         constructor(t, e) {
-            super(t), this._scrollElement = "BODY" === this._element.tagName ? window : this._element, this._config = this._getConfig(e), this._offsets = [], this._targets = [], this._activeTarget = null, this._scrollHeight = 0, j.on(this._scrollElement, "scroll.bs.scrollspy", (() => this._process())), this.refresh(), this._process()
+            super(t, e), this._targetLinks = new Map, this._observableSections = new Map, this._rootElement = "visible" === getComputedStyle(this._element).overflowY ? null : this._element, this._activeTarget = null, this._observer = null, this._previousScrollData = {
+                visibleEntryTop: 0,
+                parentScrollTop: 0
+            }, this.refresh()
         }
         static get Default() {
-            return bn
+            return mn
+        }
+        static get DefaultType() {
+            return gn
         }
         static get NAME() {
-            return _n
+            return "scrollspy"
         }
         refresh() {
-            const t = this._scrollElement === this._scrollElement.window ? "offset" : En,
-                e = "auto" === this._config.method ? t : this._config.method,
-                n = e === En ? this._getScrollTop() : 0;
-            this._offsets = [], this._targets = [], this._scrollHeight = this._getScrollHeight(), V.find(wn, this._config.target).map((t => {
-                const s = i(t),
-                    o = s ? V.findOne(s) : null;
-                if (o) {
-                    const t = o.getBoundingClientRect();
-                    if (t.width || t.height) return [U[e](o).top + n, s]
-                }
-                return null
-            })).filter((t => t)).sort(((t, e) => t[0] - e[0])).forEach((t => {
-                this._offsets.push(t[0]), this._targets.push(t[1])
-            }))
+            this._initializeTargetsAndObservables(), this._maybeEnableSmoothScroll(), this._observer ? this._observer.disconnect() : this._observer = this._getNewObserver();
+            for (const t of this._observableSections.values()) this._observer.observe(t)
         }
         dispose() {
-            j.off(this._scrollElement, ".bs.scrollspy"), super.dispose()
+            this._observer.disconnect(), super.dispose()
         }
-        _getConfig(t) {
-            return (t = {
-                ...bn,
-                ...U.getDataAttributes(this._element),
-                ..."object" == typeof t && t ? t : {}
-            }).target = r(t.target) || document.documentElement, a(_n, t, vn), t
+        _configAfterMerge(t) {
+            return t.target = r(t.target) || document.body, t.rootMargin = t.offset ? `${t.offset}px 0px -30%` : t.rootMargin, "string" == typeof t.threshold && (t.threshold = t.threshold.split(",").map((t => Number.parseFloat(t)))), t
         }
-        _getScrollTop() {
-            return this._scrollElement === window ? this._scrollElement.pageYOffset : this._scrollElement.scrollTop
+        _maybeEnableSmoothScroll() {
+            this._config.smoothScroll && (P.off(this._config.target, un), P.on(this._config.target, un, pn, (t => {
+                const e = this._observableSections.get(t.target.hash);
+                if (e) {
+                    t.preventDefault();
+                    const i = this._rootElement || window,
+                        n = e.offsetTop - this._element.offsetTop;
+                    if (i.scrollTo) return void i.scrollTo({
+                        top: n,
+                        behavior: "smooth"
+                    });
+                    i.scrollTop = n
+                }
+            })))
         }
-        _getScrollHeight() {
-            return this._scrollElement.scrollHeight || Math.max(document.body.scrollHeight, document.documentElement.scrollHeight)
+        _getNewObserver() {
+            const t = {
+                root: this._rootElement,
+                threshold: this._config.threshold,
+                rootMargin: this._config.rootMargin
+            };
+            return new IntersectionObserver((t => this._observerCallback(t)), t)
         }
-        _getOffsetHeight() {
-            return this._scrollElement === window ? window.innerHeight : this._scrollElement.getBoundingClientRect().height
-        }
-        _process() {
-            const t = this._getScrollTop() + this._config.offset,
-                e = this._getScrollHeight(),
-                i = this._config.offset + e - this._getOffsetHeight();
-            if (this._scrollHeight !== e && this.refresh(), t >= i) {
-                const t = this._targets[this._targets.length - 1];
-                this._activeTarget !== t && this._activate(t)
-            } else {
-                if (this._activeTarget && t < this._offsets[0] && this._offsets[0] > 0) return this._activeTarget = null, void this._clear();
-                for (let e = this._offsets.length; e--;) this._activeTarget !== this._targets[e] && t >= this._offsets[e] && (void 0 === this._offsets[e + 1] || t < this._offsets[e + 1]) && this._activate(this._targets[e])
+        _observerCallback(t) {
+            const e = t => this._targetLinks.get(`#${t.target.id}`),
+                i = t => {
+                    this._previousScrollData.visibleEntryTop = t.target.offsetTop, this._process(e(t))
+                },
+                n = (this._rootElement || document.documentElement).scrollTop,
+                s = n >= this._previousScrollData.parentScrollTop;
+            this._previousScrollData.parentScrollTop = n;
+            for (const o of t) {
+                if (!o.isIntersecting) {
+                    this._activeTarget = null, this._clearActiveClass(e(o));
+                    continue
+                }
+                const t = o.target.offsetTop >= this._previousScrollData.visibleEntryTop;
+                if (s && t) {
+                    if (i(o), !n) return
+                } else s || t || i(o)
+            }
+        }
+        _initializeTargetsAndObservables() {
+            this._targetLinks = new Map, this._observableSections = new Map;
+            const t = z.find(pn, this._config.target);
+            for (const e of t) {
+                if (!e.hash || l(e)) continue;
+                const t = z.findOne(decodeURI(e.hash), this._element);
+                a(t) && (this._targetLinks.set(decodeURI(e.hash), e), this._observableSections.set(e.hash, t))
             }
         }
-        _activate(t) {
-            this._activeTarget = t, this._clear();
-            const e = wn.split(",").map((e => `${e}[data-bs-target="${t}"],${e}[href="${t}"]`)),
-                i = V.findOne(e.join(","), this._config.target);
-            i.classList.add(yn), i.classList.contains("dropdown-item") ? V.findOne(".dropdown-toggle", i.closest(".dropdown")).classList.add(yn) : V.parents(i, ".nav, .list-group").forEach((t => {
-                V.prev(t, ".nav-link, .list-group-item").forEach((t => t.classList.add(yn))), V.prev(t, ".nav-item").forEach((t => {
-                    V.children(t, ".nav-link").forEach((t => t.classList.add(yn)))
-                }))
-            })), j.trigger(this._scrollElement, "activate.bs.scrollspy", {
+        _process(t) {
+            this._activeTarget !== t && (this._clearActiveClass(this._config.target), this._activeTarget = t, t.classList.add(fn), this._activateParents(t), P.trigger(this._element, "activate.bs.scrollspy", {
                 relatedTarget: t
-            })
+            }))
         }
-        _clear() {
-            V.find(wn, this._config.target).filter((t => t.classList.contains(yn))).forEach((t => t.classList.remove(yn)))
+        _activateParents(t) {
+            if (t.classList.contains("dropdown-item")) z.findOne(".dropdown-toggle", t.closest(".dropdown")).classList.add(fn);
+            else
+                for (const e of z.parents(t, ".nav, .list-group"))
+                    for (const t of z.prev(e, ".nav-link, .nav-item > .nav-link, .list-group-item")) t.classList.add(fn)
+        }
+        _clearActiveClass(t) {
+            t.classList.remove(fn);
+            const e = z.find("[href].active", t);
+            for (const t of e) t.classList.remove(fn)
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = An.getOrCreateInstance(this, t);
+                const e = _n.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
-                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    j.on(window, "load.bs.scrollspy.data-api", (() => {
-        V.find('[data-bs-spy="scroll"]').forEach((t => new An(t)))
-    })), g(An);
-    const Tn = "active",
-        On = "fade",
-        Cn = "show",
-        kn = ".active",
-        Ln = ":scope > li > .active";
-    class xn extends B {
+    P.on(window, "load.bs.scrollspy.data-api", (() => {
+        for (const t of z.find('[data-bs-spy="scroll"]')) _n.getOrCreateInstance(t)
+    })), m(_n);
+    const bn = "ArrowLeft",
+        vn = "ArrowRight",
+        yn = "ArrowUp",
+        wn = "ArrowDown",
+        An = "active",
+        En = "fade",
+        Tn = "show",
+        Cn = '[data-bs-toggle="tab"], [data-bs-toggle="pill"], [data-bs-toggle="list"]',
+        On = `.nav-link:not(.dropdown-toggle), .list-group-item:not(.dropdown-toggle), [role="tab"]:not(.dropdown-toggle), ${Cn}`;
+    class xn extends W {
+        constructor(t) {
+            super(t), this._parent = this._element.closest('.list-group, .nav, [role="tablist"]'), this._parent && (this._setInitialAttributes(this._parent, this._getChildren()), P.on(this._element, "keydown.bs.tab", (t => this._keydown(t))))
+        }
         static get NAME() {
             return "tab"
         }
         show() {
-            if (this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE && this._element.classList.contains(Tn)) return;
-            let t;
-            const e = n(this._element),
-                i = this._element.closest(".nav, .list-group");
-            if (i) {
-                const e = "UL" === i.nodeName || "OL" === i.nodeName ? Ln : kn;
-                t = V.find(e, i), t = t[t.length - 1]
-            }
-            const s = t ? j.trigger(t, "hide.bs.tab", {
-                relatedTarget: this._element
-            }) : null;
-            if (j.trigger(this._element, "show.bs.tab", {
+            const t = this._element;
+            if (this._elemIsActive(t)) return;
+            const e = this._getActiveElem(),
+                i = e ? P.trigger(e, "hide.bs.tab", {
                     relatedTarget: t
-                }).defaultPrevented || null !== s && s.defaultPrevented) return;
-            this._activate(this._element, i);
-            const o = () => {
-                j.trigger(t, "hidden.bs.tab", {
-                    relatedTarget: this._element
-                }), j.trigger(this._element, "shown.bs.tab", {
-                    relatedTarget: t
-                })
+                }) : null;
+            P.trigger(t, "show.bs.tab", {
+                relatedTarget: e
+            }).defaultPrevented || i && i.defaultPrevented || (this._deactivate(e, t), this._activate(t, e))
+        }
+        _activate(t, e) {
+            t && (t.classList.add(An), this._activate(z.getElementFromSelector(t)), this._queueCallback((() => {
+                "tab" === t.getAttribute("role") ? (t.removeAttribute("tabindex"), t.setAttribute("aria-selected", !0), this._toggleDropDown(t, !0), P.trigger(t, "shown.bs.tab", {
+                    relatedTarget: e
+                })) : t.classList.add(Tn)
+            }), t, t.classList.contains(En)))
+        }
+        _deactivate(t, e) {
+            t && (t.classList.remove(An), t.blur(), this._deactivate(z.getElementFromSelector(t)), this._queueCallback((() => {
+                "tab" === t.getAttribute("role") ? (t.setAttribute("aria-selected", !1), t.setAttribute("tabindex", "-1"), this._toggleDropDown(t, !1), P.trigger(t, "hidden.bs.tab", {
+                    relatedTarget: e
+                })) : t.classList.remove(Tn)
+            }), t, t.classList.contains(En)))
+        }
+        _keydown(t) {
+            if (![bn, vn, yn, wn].includes(t.key)) return;
+            t.stopPropagation(), t.preventDefault();
+            const e = [vn, wn].includes(t.key),
+                i = b(this._getChildren().filter((t => !l(t))), t.target, e, !0);
+            i && (i.focus({
+                preventScroll: !0
+            }), xn.getOrCreateInstance(i).show())
+        }
+        _getChildren() {
+            return z.find(On, this._parent)
+        }
+        _getActiveElem() {
+            return this._getChildren().find((t => this._elemIsActive(t))) || null
+        }
+        _setInitialAttributes(t, e) {
+            this._setAttributeIfNotExists(t, "role", "tablist");
+            for (const t of e) this._setInitialAttributesOnChild(t)
+        }
+        _setInitialAttributesOnChild(t) {
+            t = this._getInnerElement(t);
+            const e = this._elemIsActive(t),
+                i = this._getOuterElement(t);
+            t.setAttribute("aria-selected", e), i !== t && this._setAttributeIfNotExists(i, "role", "presentation"), e || t.setAttribute("tabindex", "-1"), this._setAttributeIfNotExists(t, "role", "tab"), this._setInitialAttributesOnTargetPanel(t)
+        }
+        _setInitialAttributesOnTargetPanel(t) {
+            const e = z.getElementFromSelector(t);
+            e && (this._setAttributeIfNotExists(e, "role", "tabpanel"), t.id && this._setAttributeIfNotExists(e, "aria-labelledby", `${t.id}`))
+        }
+        _toggleDropDown(t, e) {
+            const i = this._getOuterElement(t);
+            if (!i.classList.contains("dropdown")) return;
+            const n = (t, n) => {
+                const s = z.findOne(t, i);
+                s && s.classList.toggle(n, e)
             };
-            e ? this._activate(e, e.parentNode, o) : o()
+            n(".dropdown-toggle", An), n(".dropdown-menu", Tn), i.setAttribute("aria-expanded", e)
         }
-        _activate(t, e, i) {
-            const n = (!e || "UL" !== e.nodeName && "OL" !== e.nodeName ? V.children(e, kn) : V.find(Ln, e))[0],
-                s = i && n && n.classList.contains(On),
-                o = () => this._transitionComplete(t, n, i);
-            n && s ? (n.classList.remove(Cn), this._queueCallback(o, t, !0)) : o()
-        }
-        _transitionComplete(t, e, i) {
-            if (e) {
-                e.classList.remove(Tn);
-                const t = V.findOne(":scope > .dropdown-menu .active", e.parentNode);
-                t && t.classList.remove(Tn), "tab" === e.getAttribute("role") && e.setAttribute("aria-selected", !1)
-            }
-            t.classList.add(Tn), "tab" === t.getAttribute("role") && t.setAttribute("aria-selected", !0), u(t), t.classList.contains(On) && t.classList.add(Cn);
-            let n = t.parentNode;
-            if (n && "LI" === n.nodeName && (n = n.parentNode), n && n.classList.contains("dropdown-menu")) {
-                const e = t.closest(".dropdown");
-                e && V.find(".dropdown-toggle", e).forEach((t => t.classList.add(Tn))), t.setAttribute("aria-expanded", !0)
-            }
-            i && i()
+        _setAttributeIfNotExists(t, e, i) {
+            t.hasAttribute(e) || t.setAttribute(e, i)
+        }
+        _elemIsActive(t) {
+            return t.classList.contains(An)
+        }
+        _getInnerElement(t) {
+            return t.matches(On) ? t : z.findOne(On, t)
+        }
+        _getOuterElement(t) {
+            return t.closest(".nav-item, .list-group-item") || t
         }
         static jQueryInterface(t) {
             return this.each((function() {
                 const e = xn.getOrCreateInstance(this);
                 if ("string" == typeof t) {
-                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
                     e[t]()
                 }
             }))
         }
     }
-    j.on(document, "click.bs.tab.data-api", '[data-bs-toggle="tab"], [data-bs-toggle="pill"], [data-bs-toggle="list"]', (function(t) {
-        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), c(this) || xn.getOrCreateInstance(this).show()
-    })), g(xn);
-    const Dn = "toast",
-        Sn = "hide",
-        Nn = "show",
-        In = "showing",
-        Pn = {
+    P.on(document, "click.bs.tab", Cn, (function(t) {
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), l(this) || xn.getOrCreateInstance(this).show()
+    })), P.on(window, "load.bs.tab", (() => {
+        for (const t of z.find('.active[data-bs-toggle="tab"], .active[data-bs-toggle="pill"], .active[data-bs-toggle="list"]')) xn.getOrCreateInstance(t)
+    })), m(xn);
+    const kn = "hide",
+        Ln = "show",
+        Sn = "showing",
+        Dn = {
             animation: "boolean",
             autohide: "boolean",
             delay: "number"
         },
-        jn = {
+        In = {
             animation: !0,
             autohide: !0,
             delay: 5e3
         };
-    class Mn extends B {
+    class Nn extends W {
         constructor(t, e) {
-            super(t), this._config = this._getConfig(e), this._timeout = null, this._hasMouseInteraction = !1, this._hasKeyboardInteraction = !1, this._setListeners()
-        }
-        static get DefaultType() {
-            return Pn
+            super(t, e), this._timeout = null, this._hasMouseInteraction = !1, this._hasKeyboardInteraction = !1, this._setListeners()
         }
         static get Default() {
-            return jn
+            return In
         }
-        static get NAME() {
+        static get DefaultType() {
             return Dn
         }
+        static get NAME() {
+            return "toast"
+        }
         show() {
-            j.trigger(this._element, "show.bs.toast").defaultPrevented || (this._clearTimeout(), this._config.animation && this._element.classList.add("fade"), this._element.classList.remove(Sn), u(this._element), this._element.classList.add(Nn), this._element.classList.add(In), this._queueCallback((() => {
-                this._element.classList.remove(In), j.trigger(this._element, "shown.bs.toast"), this._maybeScheduleHide()
+            P.trigger(this._element, "show.bs.toast").defaultPrevented || (this._clearTimeout(), this._config.animation && this._element.classList.add("fade"), this._element.classList.remove(kn), d(this._element), this._element.classList.add(Ln, Sn), this._queueCallback((() => {
+                this._element.classList.remove(Sn), P.trigger(this._element, "shown.bs.toast"), this._maybeScheduleHide()
             }), this._element, this._config.animation))
         }
         hide() {
-            this._element.classList.contains(Nn) && (j.trigger(this._element, "hide.bs.toast").defaultPrevented || (this._element.classList.add(In), this._queueCallback((() => {
-                this._element.classList.add(Sn), this._element.classList.remove(In), this._element.classList.remove(Nn), j.trigger(this._element, "hidden.bs.toast")
+            this.isShown() && (P.trigger(this._element, "hide.bs.toast").defaultPrevented || (this._element.classList.add(Sn), this._queueCallback((() => {
+                this._element.classList.add(kn), this._element.classList.remove(Sn, Ln), P.trigger(this._element, "hidden.bs.toast")
             }), this._element, this._config.animation)))
         }
         dispose() {
-            this._clearTimeout(), this._element.classList.contains(Nn) && this._element.classList.remove(Nn), super.dispose()
+            this._clearTimeout(), this.isShown() && this._element.classList.remove(Ln), super.dispose()
         }
-        _getConfig(t) {
-            return t = {
-                ...jn,
-                ...U.getDataAttributes(this._element),
-                ..."object" == typeof t && t ? t : {}
-            }, a(Dn, t, this.constructor.DefaultType), t
+        isShown() {
+            return this._element.classList.contains(Ln)
         }
         _maybeScheduleHide() {
             this._config.autohide && (this._hasMouseInteraction || this._hasKeyboardInteraction || (this._timeout = setTimeout((() => {
                 this.hide()
             }), this._config.delay)))
         }
         _onInteraction(t, e) {
@@ -3064,38 +3228,38 @@
                     this._hasKeyboardInteraction = e
             }
             if (e) return void this._clearTimeout();
             const i = t.relatedTarget;
             this._element === i || this._element.contains(i) || this._maybeScheduleHide()
         }
         _setListeners() {
-            j.on(this._element, "mouseover.bs.toast", (t => this._onInteraction(t, !0))), j.on(this._element, "mouseout.bs.toast", (t => this._onInteraction(t, !1))), j.on(this._element, "focusin.bs.toast", (t => this._onInteraction(t, !0))), j.on(this._element, "focusout.bs.toast", (t => this._onInteraction(t, !1)))
+            P.on(this._element, "mouseover.bs.toast", (t => this._onInteraction(t, !0))), P.on(this._element, "mouseout.bs.toast", (t => this._onInteraction(t, !1))), P.on(this._element, "focusin.bs.toast", (t => this._onInteraction(t, !0))), P.on(this._element, "focusout.bs.toast", (t => this._onInteraction(t, !1)))
         }
         _clearTimeout() {
             clearTimeout(this._timeout), this._timeout = null
         }
         static jQueryInterface(t) {
             return this.each((function() {
-                const e = Mn.getOrCreateInstance(this, t);
+                const e = Nn.getOrCreateInstance(this, t);
                 if ("string" == typeof t) {
                     if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
                     e[t](this)
                 }
             }))
         }
     }
-    return R(Mn), g(Mn), {
-        Alert: W,
-        Button: z,
-        Carousel: st,
-        Collapse: pt,
-        Dropdown: hi,
-        Modal: Hi,
-        Offcanvas: Fi,
-        Popover: gn,
-        ScrollSpy: An,
+    return R(Nn), m(Nn), {
+        Alert: q,
+        Button: K,
+        Carousel: rt,
+        Collapse: ft,
+        Dropdown: ci,
+        Modal: Ni,
+        Offcanvas: zi,
+        Popover: dn,
+        ScrollSpy: _n,
         Tab: xn,
-        Toast: Mn,
-        Tooltip: un
+        Toast: Nn,
+        Tooltip: ln
     }
 }));
 //# sourceMappingURL=bootstrap.bundle.min.js.map
```

### Comparing `abow-0.4.3/abow/tags.py` & `abow-0.5.0/abow/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # A Bottle of Wiki — personal wiki
 # SPDX-License-Identifier: AGPL-3.0-or-later
-# Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+# Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/views/about.tpl` & `abow-0.5.0/abow/views/about.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
@@ -17,25 +17,25 @@
 %
 %rebase('index.tpl')
 % #_ Do not translate A Bottle of Wiki
 <h1 class="fw-bold mb-4">{{_('About A Bottle of Wiki')}}</h1>
 <div class="text-justify mb-5 about">
 <p><img src="{{get_url('static', filepath='img/abow.svg')}}" alt="A Bottle of Wiki logo"class="me-2">{{version}}</p>
 <h2>{{_('License')}}</h2>
-<p>Copyright (C) 2019-2022 <a href="mailto:benoit.monin@gmx.fr">Benoît Monin</a></p>
+<p>Copyright (C) 2019-2023 <a href="mailto:benoit.monin@gmx.fr">Benoît Monin</a></p>
 % #_ Do not translate A Bottle of Wiki
 <p>{{_('''A Bottle of Wiki is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as
 published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.''')}}</p>
 <h2>{{_('Included software')}}</h2>
 % #_ Do not translate A Bottle of Wiki
 <p>{{_('A Bottle of Wiki includes the following software:')}}</p>
 <ul>
-<li><a href="https://getbootstrap.com/">Bootstrap</a> {{_('version')}} 5.1.3. {{_('Released under MIT license.')}}</li>
+<li><a href="https://getbootstrap.com/">Bootstrap</a> {{_('version')}} 5.3.0. {{_('Released under MIT license.')}}</li>
 <li><a href="http://www.jacklmoore.com/autosize/">Autosize</a> {{_('version')}} 5.0.0. {{_('Released under MIT license.')}}</li>
 <li>{{_('Modified Markdown extensions tables and wikilinks')}}. <a href="https://python-markdown.github.io/">Python-Markdown</a> {{_('version')}} 3.2.1. {{_('Released under BSD license.')}}</li>
 </ul>
 <h2>{{_('Configuration')}}</h2>
 %for k, v in sorted(config.items()):
 %if k.startswith('abow.') and config.meta_get(k, 'help'):
 <div class="card mb-2">
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
 % # A Bottle of Wiki â personal wiki % # SPDX-License-Identifier: AGPL-3.0-
-or-later % # Copyright (C) 2019-2022 BenoÃ®t Monin
+or-later % # Copyright (C) 2019-2023 BenoÃ®t Monin
 monin@gmx.fr> % # % # This program is free software: you can redistribute it
 and/or modify % # it under the terms of the GNU Affero General Public License
 as % # published by the Free Software Foundation, either version 3 of the % #
 License, or (at your option) any later version. % # % # This program is
 distributed in the hope that it will be useful, % # but WITHOUT ANY WARRANTY;
 without even the implied warranty of % # MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the % # GNU Affero General Public License for more
 details. % # % # You should have received a copy of the GNU Affero General
 Public License % # along with this program. If not, see
 www.gnu.org/licenses/>. % %rebase('index.tpl') % #_ Do not translate A Bottle
 of Wiki
 ****** {{_('About A Bottle of Wiki')}} ******
 [A Bottle of Wiki logo]{{version}}
 ***** {{_('License')}} *****
-Copyright (C) 2019-2022 BenoÃ®t_Monin
+Copyright (C) 2019-2023 BenoÃ®t_Monin
 % #_ Do not translate A Bottle of Wiki
 {{_('''A Bottle of Wiki is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by the
 Free Software Foundation, either version 3 of the License, or (at your option)
 any later version.''')}}
 ***** {{_('Included software')}} *****
 % #_ Do not translate A Bottle of Wiki
 {{_('A Bottle of Wiki includes the following software:')}}
-    * Bootstrap {{_('version')}} 5.1.3. {{_('Released under MIT license.')}}
+    * Bootstrap {{_('version')}} 5.3.0. {{_('Released under MIT license.')}}
     * Autosize {{_('version')}} 5.0.0. {{_('Released under MIT license.')}}
     * {{_('Modified Markdown extensions tables and wikilinks')}}. Python-
       Markdown {{_('version')}} 3.2.1. {{_('Released under BSD license.')}}
 ***** {{_('Configuration')}} *****
 %for k, v in sorted(config.items()): %if k.startswith('abow.') and
 config.meta_get(k, 'help'):
 {{k.split('.')[1]}} {{_(config.meta_get(k, 'help'))}}
```

### Comparing `abow-0.4.3/abow/views/edit.tpl` & `abow-0.5.0/abow/views/edit.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
@@ -16,15 +16,15 @@
 % # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 %
 %rebase('index.tpl')
 %import urllib.parse
 <h1 class="fw-bold text-muted text-end fst-italic mb-5">{{title}}</h1>
 <div id="preview" class="abow_view text-justify mb-5"></div>
 <form method="post">
-<div class="btn-toolbar m-1 rounded bg-light shadow-sm" role="toolbar" id="editor_toolbar" aria-label={{!_('"Editor toolbar"')}}>
+<div class="btn-toolbar my-1 rounded bg-secondary-subtle shadow-sm px-1" role="toolbar" id="editor_toolbar" aria-label={{!_('"Editor toolbar"')}}>
 <div class="btn-group my-1 me-1" role="group">
 <a role="button" class="btn btn-sm btn-secondary" href="javascript:;" onclick="insert_md(this, '**', '**')" title={{!_('"Bold"')}}><strong>{{_('B')}}</strong></a>
 <a role="button" class="btn btn-sm btn-secondary" href="javascript:;" onclick="insert_md(this, '_', '_')" title={{!_('"Italic"')}}><em>{{_('I')}}</em></a>
 <a role="button" class="btn btn-sm btn-secondary" href="javascript:;" onclick="insert_md(this, '~~', '~~')" title={{!_('"Strike through"')}}><del>{{_('S')}}</del></a>
 <a role="button" class="btn btn-sm btn-secondary" href="javascript:;" onclick="insert_md(this, '^^', '^^')" title={{!_('"Underline"')}}><ins>{{_('U')}}</ins></a>
 </div>
 <div class="btn-group my-1 me-1" role="group">
```

### Comparing `abow-0.4.3/abow/views/error.tpl` & `abow-0.5.0/abow/views/error.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/views/index.tpl` & `abow-0.5.0/abow/views/index.tpl`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
@@ -25,29 +25,29 @@
 <link rel="stylesheet" href="{{get_url('static', filepath='css/highlight.css')}}">
 <link rel="stylesheet" href="{{get_url('static', filepath='css/abow.css')}}">
 <link rel="icon" href="{{get_url('static', filepath='img/abow_32.png')}}" sizes="32x32" type="image/png">
 <link rel="icon" href="{{get_url('static', filepath='img/abow_16.png')}}" sizes="16x16" type="image/png">
 <title>{{title}} — A Bottle of Wiki</title>
 </head>
 <body>
-<header class="navbar navbar-expand-xl sticky-top navbar-dark bg-dark shadow-sm d-print-none">
+<header class="navbar navbar-expand-xl sticky-top bg-secondary-subtle shadow-sm d-print-none">
 <div class="container-fluid g-3">
 <a class="navbar-brand col-xl-3 ms-xl-3 me-xl-0" href="{{get_url('root')}}">A Bottle of Wiki</a>
 <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#abow_menu" aria-controls="abow_menu" aria-expanded="false" aria-label={{!_('"Toggle the navigation bar"')}}>
 <span class="navbar-toggler-icon"></span>
 </button>
 <div class="navbar-collapse ps-xl-3 me-xl-3 collapse" id="abow_menu">
 <ul class="navbar-nav me-auto">
 %include('index_nav_item.tpl', item='view', link='../view/' + urllib.parse.quote(get('pagename','')), display=_('View'), enabled=defined('pagename'))
 %include('index_nav_item.tpl', item='edit', link='../edit/' + urllib.parse.quote(get('pagename','')), display=_('Edit'), enabled=defined('pagename'))
 <li class="nav-item dropdown">
 <a class="nav-link dropdown-toggle" href="#" id="abow_menu_dropdown" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
 {{_('More')}}
 </a>
-<div class="dropdown-menu shadow-sm" aria-labelledby="abow_menu_dropdown">
+<div class="dropdown-menu shadow-sm bg-secondary-subtle text-primary-emphasis" aria-labelledby="abow_menu_dropdown">
 <a class="dropdown-item" href="{{get_url('search')}}">{{_('List of pages')}}</a>
 <div class="dropdown-divider"></div>
 %if help_page:
 <a class="dropdown-item" href="{{get_url('view', pagename=help_page)}}">{{_('Help')}}</a>
 %end
 <a class="dropdown-item" href="{{get_url('about')}}">{{_('About')}}</a>
 </div>
@@ -77,16 +77,16 @@
 %if defined('toc'):
 {{!toc}}
 %end
 </div>
 </div>
 </div>
 <script src="{{get_url('static', filepath='js/bootstrap.bundle.min.js')}}"></script>
+<script src="{{get_url('static', filepath='js/abow.js')}}"></script>
 %if action == 'edit':
 <script src="{{get_url('static', filepath='js/autosize.min.js')}}"></script>
-<script src="{{get_url('static', filepath='js/abow.js')}}"></script>
 <script>
 autosize(document.getElementById('editor_text'));
 </script>
 %end
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 % # A Bottle of Wiki â personal wiki % # SPDX-License-Identifier: AGPL-3.0-
-or-later % # Copyright (C) 2019-2022 BenoÃ®t Monin
+or-later % # Copyright (C) 2019-2023 BenoÃ®t Monin
 monin@gmx.fr> % # % # This program is free software: you can redistribute it
 and/or modify % # it under the terms of the GNU Affero General Public License
 as % # published by the Free Software Foundation, either version 3 of the % #
 License, or (at your option) any later version. % # % # This program is
 distributed in the hope that it will be useful, % # but WITHOUT ANY WARRANTY;
 without even the implied warranty of % # MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the % # GNU Affero General Public License for more
```

### Comparing `abow-0.4.3/abow/views/index_nav_item.tpl` & `abow-0.5.0/abow/views/index_nav_item.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
```

### Comparing `abow-0.4.3/abow/views/list_pages.tpl` & `abow-0.5.0/abow/views/list_pages.tpl`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
@@ -13,15 +13,15 @@
 % # GNU Affero General Public License for more details.
 % #
 % # You should have received a copy of the GNU Affero General Public License
 % # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 %
 %rebase('index.tpl')
 %import urllib.parse
-<h1 class="fw-bold mb-4">{{title}} <span class="badge bg-secondary align-bottom ms-2 py-2 px-3">{{len(pages_list)}}</span></h1>
+<h1 class="fw-bold mb-4">{{title}} <span class="badge bg-secondary-subtle text-secondary-emphasis align-bottom ms-2 py-2 px-3">{{len(pages_list)}}</span></h1>
 <ul>
 % for page in pages_list:
 <li><a href="../view/{{urllib.parse.quote(page)}}">{{page}}</a></li>
 % end
 </ul>
 %if defined('page_exists'):
 <hr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 % # A Bottle of Wiki â personal wiki % # SPDX-License-Identifier: AGPL-3.0-
-or-later % # Copyright (C) 2019-2022 BenoÃ®t Monin
+or-later % # Copyright (C) 2019-2023 BenoÃ®t Monin
 monin@gmx.fr> % # % # This program is free software: you can redistribute it
 and/or modify % # it under the terms of the GNU Affero General Public License
 as % # published by the Free Software Foundation, either version 3 of the % #
 License, or (at your option) any later version. % # % # This program is
 distributed in the hope that it will be useful, % # but WITHOUT ANY WARRANTY;
 without even the implied warranty of % # MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the % # GNU Affero General Public License for more
```

### Comparing `abow-0.4.3/abow/views/view.tpl` & `abow-0.5.0/abow/views/view.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % # A Bottle of Wiki — personal wiki
 % # SPDX-License-Identifier: AGPL-3.0-or-later
-% # Copyright (C) 2019-2022  Benoît Monin <benoit.monin@gmx.fr>
+% # Copyright (C) 2019-2023  Benoît Monin <benoit.monin@gmx.fr>
 % #
 % # This program is free software: you can redistribute it and/or modify
 % # it under the terms of the GNU Affero General Public License as
 % # published by the Free Software Foundation, either version 3 of the
 % # License, or (at your option) any later version.
 % #
 % # This program is distributed in the hope that it will be useful,
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 % # A Bottle of Wiki â personal wiki % # SPDX-License-Identifier: AGPL-3.0-
-or-later % # Copyright (C) 2019-2022 BenoÃ®t Monin
+or-later % # Copyright (C) 2019-2023 BenoÃ®t Monin
 monin@gmx.fr> % # % # This program is free software: you can redistribute it
 and/or modify % # it under the terms of the GNU Affero General Public License
 as % # published by the Free Software Foundation, either version 3 of the % #
 License, or (at your option) any later version. % # % # This program is
 distributed in the hope that it will be useful, % # but WITHOUT ANY WARRANTY;
 without even the implied warranty of % # MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the % # GNU Affero General Public License for more
```

### Comparing `abow-0.4.3/changelog.md` & `abow-0.5.0/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## Version 0.5.0 - _2023-06-27_
+
+* Drop compatibility with python 3.6 and 3.7.
+* Add compatibility with python 3.11.
+* Update bootstrap to 5.3.0.
+* Switch build to hatchling instead of setuptools.
+* Add dark mode, selected by the preferred color scheme.
+
 ## Version 0.4.3 - _2022-04-21_
 
 * Do not print the menu bar and the alerts, only the page content.
 * Show the URL of outside links in print media.
 * Update bootstrap to 5.1.3.
 * Drop compatibility with python 3.5.
```

### Comparing `abow-0.4.3/config.example` & `abow-0.5.0/config.example`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/conftest.py` & `abow-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/test_app.py` & `abow-0.5.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/test_backend.py` & `abow-0.5.0/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/test_config.py` & `abow-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/test_l10n.py` & `abow-0.5.0/tests/test_l10n.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/tests/test_render.py` & `abow-0.5.0/tests/test_render.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 def test_table():
     '''test the tables extension
     '''
     result = abow.render.render('| a | b |\n|---|---|\n| c | d |')
     expected = '''\
         <div class="table-responsive">
         <table class="table table-bordered">
-        <thead class="table-secondary">
+        <thead>
         <tr>
         <th>a</th>
         <th>b</th>
         </tr>
         </thead>
-        <tbody>
+        <tbody class="table-group-divider">
         <tr>
         <td>c</td>
         <td>d</td>
         </tr>
         </tbody>
         </table>
         </div>'''
```

### Comparing `abow-0.4.3/tests/test_tags.py` & `abow-0.5.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `abow-0.4.3/usage.md` & `abow-0.5.0/usage.md`

 * *Files identical despite different names*

