# Comparing `tmp/bl_hector-0.3.0.tar.gz` & `tmp/bl_hector-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.3.0.tar", max compression
+gzip compressed data, was "bl_hector-0.3.1.tar", max compression
```

## Comparing `bl_hector-0.3.0.tar` & `bl_hector-0.3.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.3.0/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.3.0/README.md
--rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     2044 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1971 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3729 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0     1505 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1630 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3039 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3547 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1694 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4531 2023-06-23 16:03:54.837120 bl_hector-0.3.0/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2364 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4546 2023-06-21 11:30:42.251958 bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     4012 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3363 2023-06-21 11:30:42.251958 bl_hector-0.3.0/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1690 2023-06-21 11:30:42.255958 bl_hector-0.3.0/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     5371 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5979 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1842 2023-06-23 15:58:49.368922 bl_hector-0.3.0/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    19488 2023-06-23 16:03:34.457374 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-21 11:30:42.255958 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4238 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2105 2023-06-23 15:58:49.368922 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     5746 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3633 2023-06-23 15:58:56.084839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2045 2023-06-23 16:11:12.983659 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4768 2023-06-23 15:58:56.096839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1845 2023-06-21 11:30:42.259958 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     5276 2023-06-21 11:30:42.259958 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.3.0/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1570 2023-06-23 16:16:27.055745 bl_hector-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4606 2023-06-23 16:17:09.199821 bl_hector-0.3.0/setup.py
--rw-r--r--   0        0        0     3048 2023-06-23 16:17:09.201573 bl_hector-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.3.1/README.md
+-rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.1/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2044 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1971 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3729 2023-06-21 11:30:42.239958 bl_hector-0.3.1/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0     1505 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.3.1/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1630 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3039 2023-06-21 11:30:42.243958 bl_hector-0.3.1/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3547 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1694 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4531 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-23 15:58:56.080839 bl_hector-0.3.1/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2364 2023-06-21 11:30:42.247958 bl_hector-0.3.1/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4546 2023-06-21 11:30:42.251958 bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     4012 2023-06-23 16:18:20.470332 bl_hector-0.3.1/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3363 2023-06-21 11:30:42.251958 bl_hector-0.3.1/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.3.1/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1690 2023-06-21 11:30:42.255958 bl_hector-0.3.1/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     5448 2023-06-27 05:48:10.328996 bl_hector-0.3.1/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     6060 2023-06-27 05:48:10.332996 bl_hector-0.3.1/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1842 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    19488 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-21 11:30:42.255958 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4238 2023-06-23 16:18:20.474332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2105 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     5746 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3633 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2045 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4768 2023-06-23 16:18:20.478332 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1845 2023-06-21 11:30:42.259958 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5276 2023-06-21 11:30:42.259958 bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.3.1/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-06-27 05:48:27.768996 bl_hector-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4606 2023-06-27 05:49:30.255854 bl_hector-0.3.1/setup.py
+-rw-r--r--   0        0        0     3048 2023-06-27 05:49:30.257588 bl_hector-0.3.1/PKG-INFO
```

### Comparing `bl_hector-0.3.0/LICENSE` & `bl_hector-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/README.md` & `bl_hector-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/__init__.py` & `bl_hector-0.3.1/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/__init__.py` & `bl_hector-0.3.1/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.3.1/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/configuration/__init__.py` & `bl_hector-0.3.1/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/configuration/cli.py` & `bl_hector-0.3.1/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/configuration/wsgi.py` & `bl_hector-0.3.1/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/__init__.py` & `bl_hector-0.3.1/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/__init__.py` & `bl_hector-0.3.1/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/entities.py` & `bl_hector-0.3.1/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.3.1/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/repositories.py` & `bl_hector-0.3.1/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/services.py` & `bl_hector-0.3.1/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.3.1/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/services.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.3.1/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.3.1/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/settings.py` & `bl_hector-0.3.1/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.3.1/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.3.1/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.3.1/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.3.1/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/exceptions.py` & `bl_hector-0.3.1/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/from_dict.py` & `bl_hector-0.3.1/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/from_json.py` & `bl_hector-0.3.1/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.3.1/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 update-book-failure = Book cannot be updated!
 update-book-success = Book has been updated!
 update-book-cancel = Cancel
 update-book-update = Save
 update-book-cover-help = Click to upload a new cover
 update-book-cover-format-not-supported = The format of this cover is not supported!
 
+book-does-not-exist = The book you are looking for is not in the collection!
 book-already-exists = Book already in the collection!
 # isbn (string) The ISBN of the book
 # url (string) The URL of the book
 book-added-html = Book <a href="{ $url }">{ $isbn }</a> successfully added!
 # isbn (string) The ISBN of the book
 book-added-text = Book { $isbn } successfully added!
 book-added = Book <a href="{ $url }">{ $isbn }</a> successfully added!
```

#### html2text {}

```diff
@@ -56,14 +56,15 @@
 search-books-next-page = Next # title (string) The title of the book display-
 book-title = Details for "{ $title }" update-book-requires-authentification =
 You must be authenticated before editing a book! # isbn (string) The ISBN of
 the book update-book-title = Edit information for `{ $isbn }` update-book-
 action = Edit update-book-failure = Book cannot be updated! update-book-success
 = Book has been updated! update-book-cancel = Cancel update-book-update = Save
 update-book-cover-help = Click to upload a new cover update-book-cover-format-
-not-supported = The format of this cover is not supported! book-already-exists
-= Book already in the collection! # isbn (string) The ISBN of the book # url
+not-supported = The format of this cover is not supported! book-does-not-exist
+= The book you are looking for is not in the collection! book-already-exists =
+Book already in the collection! # isbn (string) The ISBN of the book # url
 (string) The URL of the book book-added-html = Book {_$isbn_} successfully
 added! # isbn (string) The ISBN of the book book-added-text = Book { $isbn }
 successfully added! book-added = Book {_$isbn_} successfully added! book-not-
 found = Book not found! book-cannot-be-added = The book cannot be added! books-
 cannot-be-found = The search cannot be performed!
```

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.3.1/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 update-book-failure = Le livre n'a pas pu être mis à jour !
 update-book-success = Le livre a bien été mis à jour !
 update-book-cancel = Annuler
 update-book-update = Enregistrer
 update-book-cover-help = Cliquez pour téléverser une nouvelle couverture
 update-book-cover-format-not-supported = Le format de cette couverture n'est pas supporté !
 
+book-does-not-exist = Le livre que vous cherchez n'est pas dans la collection !
 book-already-exists = Ce livre est déjà dans la collection !
 # isbn (string) The ISBN of the book
 # url (string) The URL of the book
 book-added-html = Le livre <a href="{ $url }">{ $isbn }</a> a bien été ajouté !
 # isbn (string) The ISBN of the book
 book-added-text = Le livre { $isbn } a bien été ajouté !
 book-not-found = Le livre n'a pas été trouvé !
```

#### html2text {}

```diff
@@ -65,14 +65,15 @@
 devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
 The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
 }` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
 mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
 update-book-cancel = Annuler update-book-update = Enregistrer update-book-
 cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-
 cover-format-not-supported = Le format de cette couverture n'est pas
-supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! #
+supportÃ©Â ! book-does-not-exist = Le livre que vous cherchez n'est pas dans la
+collectionÂ ! book-already-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! #
 isbn (string) The ISBN of the book # url (string) The URL of the book book-
 added-html = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! # isbn (string) The
 ISBN of the book book-added-text = Le livre { $isbn } a bien Ã©tÃ© ajoutÃ©Â !
 book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le
 livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas
 pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.3.1/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/bl_hector/interfaces/utils.py` & `bl_hector-0.3.1/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.3.0/pyproject.toml` & `bl_hector-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.3.0"
+version = "0.3.1"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
```

### Comparing `bl_hector-0.3.0/setup.py` & `bl_hector-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.easter-eggs.org/bioneland/hector',
```

### Comparing `bl_hector-0.3.0/PKG-INFO` & `bl_hector-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection manager.
 Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

