# Comparing `tmp/mediascope_api_lib-1.1.8.tar.gz` & `tmp/mediascope_api_lib-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediascope_api_lib-1.1.8.tar", last modified: Tue Mar 28 13:18:25 2023, max compression
+gzip compressed data, was "mediascope_api_lib-1.1.9.tar", last modified: Mon Jun 26 14:27:07 2023, max compression
```

## Comparing `mediascope_api_lib-1.1.8.tar` & `mediascope_api_lib-1.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.961023 mediascope_api_lib-1.1.8/
--rw-r--r--   0 psv        (501) staff       (20)     4581 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.8/LICENSE
--rw-r--r--   0 psv        (501) staff       (20)     3333 2023-03-28 13:18:25.960782 mediascope_api_lib-1.1.8/PKG-INFO
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.922593 mediascope_api_lib-1.1.8/mediascope_api/
--rw-r--r--   0 psv        (501) staff       (20)       18 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.8/mediascope_api/__init__.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.926355 mediascope_api_lib-1.1.8/mediascope_api/core/
--rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.8/mediascope_api/core/__init__.py
--rw-r--r--   0 psv        (501) staff       (20)     2466 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.8/mediascope_api/core/cache.py
--rw-r--r--   0 psv        (501) staff       (20)      905 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.8/mediascope_api/core/errors.py
--rw-r--r--   0 psv        (501) staff       (20)    19486 2023-03-28 11:44:15.000000 mediascope_api_lib-1.1.8/mediascope_api/core/net.py
--rw-r--r--   0 psv        (501) staff       (20)     8035 2023-03-28 11:46:10.000000 mediascope_api_lib-1.1.8/mediascope_api/core/sql.py
--rw-r--r--   0 psv        (501) staff       (20)     5128 2022-11-18 07:55:29.000000 mediascope_api_lib-1.1.8/mediascope_api/core/tasks.py
--rw-r--r--   0 psv        (501) staff       (20)     1926 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.8/mediascope_api/core/utils.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.927170 mediascope_api_lib-1.1.8/mediascope_api/counter/
--rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:40:08.000000 mediascope_api_lib-1.1.8/mediascope_api/counter/__init__.py
--rw-r--r--   0 psv        (501) staff       (20)    20976 2023-03-28 11:47:31.000000 mediascope_api_lib-1.1.8/mediascope_api/counter/tasks.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.930473 mediascope_api_lib-1.1.8/mediascope_api/crossweb/
--rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.8/mediascope_api/crossweb/__init__.py
--rw-r--r--   0 psv        (501) staff       (20)   144239 2023-03-28 13:13:05.000000 mediascope_api_lib-1.1.8/mediascope_api/crossweb/catalogs.py
--rw-r--r--   0 psv        (501) staff       (20)     8796 2023-03-28 13:14:27.000000 mediascope_api_lib-1.1.8/mediascope_api/crossweb/checks.py
--rw-r--r--   0 psv        (501) staff       (20)    39402 2023-03-28 13:13:44.000000 mediascope_api_lib-1.1.8/mediascope_api/crossweb/tasks.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.934457 mediascope_api_lib-1.1.8/mediascope_api/mediavortex/
--rw-r--r--   0 psv        (501) staff       (20)        0 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.8/mediascope_api/mediavortex/__init__.py
--rw-r--r--   0 psv        (501) staff       (20)   151037 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.8/mediascope_api/mediavortex/catalogs.py
--rw-r--r--   0 psv        (501) staff       (20)    10675 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.8/mediascope_api/mediavortex/checks.py
--rw-r--r--   0 psv        (501) staff       (20)    29836 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.8/mediascope_api/mediavortex/tasks.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.936401 mediascope_api_lib-1.1.8/mediascope_api/responsum/
--rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.8/mediascope_api/responsum/__init__.py
--rwxr-xr-x   0 psv        (501) staff       (20)    30833 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.8/mediascope_api/responsum/catalogs.py
--rwxr-xr-x   0 psv        (501) staff       (20)    68325 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.8/mediascope_api/responsum/tasks.py
-drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-03-28 13:18:25.960396 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/
--rw-r--r--   0 psv        (501) staff       (20)     3333 2023-03-28 13:18:25.000000 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/PKG-INFO
--rw-r--r--   0 psv        (501) staff       (20)      920 2023-03-28 13:18:25.000000 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/SOURCES.txt
--rw-r--r--   0 psv        (501) staff       (20)        1 2023-03-28 13:18:25.000000 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/dependency_links.txt
--rw-r--r--   0 psv        (501) staff       (20)       26 2023-03-28 13:18:25.000000 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/requires.txt
--rw-r--r--   0 psv        (501) staff       (20)       15 2023-03-28 13:18:25.000000 mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/top_level.txt
--rw-r--r--   0 psv        (501) staff       (20)       38 2023-03-28 13:18:25.961106 mediascope_api_lib-1.1.8/setup.cfg
--rw-r--r--   0 psv        (501) staff       (20)     1247 2023-03-28 13:06:11.000000 mediascope_api_lib-1.1.8/setup.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.893968 mediascope_api_lib-1.1.9/
+-rw-r--r--   0 psv        (501) staff       (20)     4581 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.9/LICENSE
+-rw-r--r--   0 psv        (501) staff       (20)     3333 2023-06-26 14:27:07.893739 mediascope_api_lib-1.1.9/PKG-INFO
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.886317 mediascope_api_lib-1.1.9/mediascope_api/
+-rw-r--r--   0 psv        (501) staff       (20)       18 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.9/mediascope_api/__init__.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.888052 mediascope_api_lib-1.1.9/mediascope_api/core/
+-rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.9/mediascope_api/core/__init__.py
+-rw-r--r--   0 psv        (501) staff       (20)     2466 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.9/mediascope_api/core/cache.py
+-rw-r--r--   0 psv        (501) staff       (20)      905 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.9/mediascope_api/core/errors.py
+-rw-r--r--   0 psv        (501) staff       (20)    19511 2023-06-26 14:21:37.000000 mediascope_api_lib-1.1.9/mediascope_api/core/net.py
+-rw-r--r--   0 psv        (501) staff       (20)     8035 2023-03-28 11:46:10.000000 mediascope_api_lib-1.1.9/mediascope_api/core/sql.py
+-rw-r--r--   0 psv        (501) staff       (20)     5128 2022-11-18 07:55:29.000000 mediascope_api_lib-1.1.9/mediascope_api/core/tasks.py
+-rw-r--r--   0 psv        (501) staff       (20)     1926 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.9/mediascope_api/core/utils.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.888495 mediascope_api_lib-1.1.9/mediascope_api/counter/
+-rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:40:08.000000 mediascope_api_lib-1.1.9/mediascope_api/counter/__init__.py
+-rw-r--r--   0 psv        (501) staff       (20)    20977 2023-06-26 14:21:58.000000 mediascope_api_lib-1.1.9/mediascope_api/counter/tasks.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.889701 mediascope_api_lib-1.1.9/mediascope_api/crossweb/
+-rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.9/mediascope_api/crossweb/__init__.py
+-rw-r--r--   0 psv        (501) staff       (20)   144509 2023-06-26 14:22:45.000000 mediascope_api_lib-1.1.9/mediascope_api/crossweb/catalogs.py
+-rw-r--r--   0 psv        (501) staff       (20)     8802 2023-06-26 14:23:08.000000 mediascope_api_lib-1.1.9/mediascope_api/crossweb/checks.py
+-rw-r--r--   0 psv        (501) staff       (20)    39414 2023-06-26 14:23:32.000000 mediascope_api_lib-1.1.9/mediascope_api/crossweb/tasks.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.891054 mediascope_api_lib-1.1.9/mediascope_api/mediavortex/
+-rw-r--r--   0 psv        (501) staff       (20)        0 2023-03-28 11:43:00.000000 mediascope_api_lib-1.1.9/mediascope_api/mediavortex/__init__.py
+-rw-r--r--   0 psv        (501) staff       (20)   186623 2023-06-26 14:24:01.000000 mediascope_api_lib-1.1.9/mediascope_api/mediavortex/catalogs.py
+-rw-r--r--   0 psv        (501) staff       (20)    12590 2023-06-26 14:24:14.000000 mediascope_api_lib-1.1.9/mediascope_api/mediavortex/checks.py
+-rw-r--r--   0 psv        (501) staff       (20)    52293 2023-06-26 14:24:32.000000 mediascope_api_lib-1.1.9/mediascope_api/mediavortex/tasks.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.891928 mediascope_api_lib-1.1.9/mediascope_api/responsum/
+-rw-r--r--   0 psv        (501) staff       (20)        0 2022-09-06 16:38:17.000000 mediascope_api_lib-1.1.9/mediascope_api/responsum/__init__.py
+-rwxr-xr-x   0 psv        (501) staff       (20)    30833 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.9/mediascope_api/responsum/catalogs.py
+-rwxr-xr-x   0 psv        (501) staff       (20)    68325 2022-11-11 09:04:34.000000 mediascope_api_lib-1.1.9/mediascope_api/responsum/tasks.py
+drwxr-xr-x   0 psv        (501) staff       (20)        0 2023-06-26 14:27:07.893369 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/
+-rw-r--r--   0 psv        (501) staff       (20)     3333 2023-06-26 14:27:07.000000 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/PKG-INFO
+-rw-r--r--   0 psv        (501) staff       (20)      920 2023-06-26 14:27:07.000000 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 psv        (501) staff       (20)        1 2023-06-26 14:27:07.000000 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 psv        (501) staff       (20)       26 2023-06-26 14:27:07.000000 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/requires.txt
+-rw-r--r--   0 psv        (501) staff       (20)       15 2023-06-26 14:27:07.000000 mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/top_level.txt
+-rw-r--r--   0 psv        (501) staff       (20)       38 2023-06-26 14:27:07.894065 mediascope_api_lib-1.1.9/setup.cfg
+-rw-r--r--   0 psv        (501) staff       (20)     1265 2023-06-26 14:20:43.000000 mediascope_api_lib-1.1.9/setup.py
```

### Comparing `mediascope_api_lib-1.1.8/LICENSE` & `mediascope_api_lib-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/PKG-INFO` & `mediascope_api_lib-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mediascope_api_lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: Library for work with the Mediascope-Delivery-API
 Home-page: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib
-Download-URL: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.8
+Download-URL: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.9
 Author: Sergey Poterianski
 Author-email: sergey.poterianski@mediascope.net
 Maintainer: Mediascope JSC
 Maintainer-email: github@mediascope.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/cache.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/cache.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/errors.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/errors.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/net.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 from . import errors
 from . import utils
 from . import cache
 
 
 class MediascopeApiNetwork:
-
     DEFAULT_SETTINGS_FILENAME = 'settings.json'
 
     def __new__(cls, settings_filename: str = None, cache_path: str = None, cache_enabled: bool = True,
                 username: str = None, passw: str = None, root_url: str = None, client_id: str = None,
                 client_secret: str = None, keycloak_url: str = None, *args, **kwargs):
         if not hasattr(cls, 'instance'):
             cls.instance = super(MediascopeApiNetwork, cls).__new__(cls, *args, **kwargs)
@@ -43,30 +42,29 @@
             if settings_filename is None:
                 if os.path.exists(self.DEFAULT_SETTINGS_FILENAME):
                     settings_filename = self.DEFAULT_SETTINGS_FILENAME
                 else:
                     raise Exception('Не указаны настройки для подключения к Mediascope-API')
 
             self.username, self.passw, self.root_url, self.client_id, \
-            self.client_secret, self.keycloak_url, proxy_server = utils.load_settings(settings_filename)
+                self.client_secret, self.keycloak_url, proxy_server = utils.load_settings(settings_filename)
 
         if self.username is None or self.passw is None or self.root_url is None and \
                 self.client_id is None or self.client_secret is None or self.keycloak_url is None:
             raise Exception('Не указаны настройки для подключения к Mediascope-API')
 
         self.token = {}
 
         self.proxies = None
         if proxy_server is not None:
             self.proxies = {"https": proxy_server}
             print(f"Подсоединение через прокси {self.proxies}")
         else:
             self.proxies = {"https": ""}
 
-
     def get_token(self, username: str, passw: str) -> dict:
         """
         Получить токен по имени пользователя и паролю
 
         Parameters
         ----------
 
@@ -78,37 +76,37 @@
 
         Returns
         -------
 
         token : dict
             Токен доступа к Mediascope-API
         """
-        my_tocken_req = requests.post(
+        my_token_req = requests.post(
             url=self.keycloak_url,
             data={
                 'client_id': self.client_id,
                 'client_secret': self.client_secret,
                 'username': username,
                 'password': passw,
                 'grant_type': 'password'
             },
             headers={'Content-Type': 'application/x-www-form-urlencoded'},
             proxies=self.proxies
         )
-        if my_tocken_req.status_code == 200:
-            t = my_tocken_req.json()
+        if my_token_req.status_code == 200:
+            t = my_token_req.json()
             t['now'] = datetime.datetime.now()
             return t
-        elif my_tocken_req.status_code == 401:
+        elif my_token_req.status_code == 401:
             raise Exception(f'Ошибка авторизации!',
                             f'Не верный логин или пароль. Проверьте параметры указанные в файле: settings.json')
-        elif my_tocken_req.status_code == 403:
+        elif my_token_req.status_code == 403:
             raise Exception(f'Ошибка авторизации!', f'Доступ запрещен.')
         else:
-            raise Exception(f'Status code {my_tocken_req.status_code}', f'response: {my_tocken_req.text}')
+            raise Exception(f'Status code {my_token_req.status_code}', f'response: {my_token_req.text}')
 
     def refresh_token(self):
         """
         Обновить текущий токен или получить новый с использованием username и passw сохраненных в настройках
         """
         if 'now' in self.token:
             now = time.mktime(datetime.datetime.now().timetuple())
@@ -137,15 +135,15 @@
                 /task/duplication
 
         data : dict
             Данные отправляемые в запросе к API
 
         use_cache : bool
             Флаг кэширования
-                - True - использовать кэш. Формирует хэш для запроса и сохраняет результат в файл.
+                - True - использовать кэш. Формирует хэш для запроса, и сохраняет результат в файл.
                         Если следующие запросы совпадут по хэшу с существующим - результат возьмется из сохраненного
                         файла. Запроса к API не будет. Удобно использовать для частых запросов к большим объемам.
                 - False - кэш не используется (по умолчанию).
 
         Returns
         -------
 
@@ -202,15 +200,15 @@
                 /task/duplication
 
         data : dict
             Данные отправляемые в запросе к API
 
         use_cache : bool
             Флаг кэширования
-                - True - использовать кэш. Формирует хэш для запроса и сохраняет результат в файл.
+                - True - использовать кэш. Формирует хэш для запроса, и сохраняет результат в файл.
                         Если следующие запросы совпадут по хэшу с существующим - результат возьмется из сохраненного
                         файла. Запроса к API не будет. Удобно использовать для частых запросов к большим объемам.
                 - False - кэш не используется (по умолчанию).
 
         limit : int
             Размер порции данных получаемых за один запрос
 
@@ -259,15 +257,16 @@
                 if 'header' not in rj or 'data' not in rj:
                     break
 
                 header = rj['header']
                 if 'total' not in header:
                     is_reading = False
                     total = limit
-                total = int(header['total'])
+                else:
+                    total = int(header['total'])
                 result['header']['total'] = total
                 offset += limit
                 if offset >= total:
                     is_reading = False
 
                 if type(rj['data']) == list:
                     result_data.extend(rj['data'])
@@ -295,15 +294,15 @@
                 /task/duplication
 
         data : dict
             Данные отправляемые в запросе к API
 
         use_cache : bool
             Флаг кэширования
-                - True - использовать кэш. Формирует хэш для запроса и сохраняет результат в файл.
+                - True - использовать кэш. Формирует хэш для запроса, и сохраняет результат в файл.
                         Если следующие запросы совпадут по хэшу с существующим - результат возьмется из сохраненного
                         файла. Запроса к API не будет. Удобно использовать для частых запросов к большим объемам.
                 - False - кэш не используется (по умолчанию).
 
         Returns
         -------
 
@@ -325,15 +324,15 @@
             return req.text
         else:
             self._raise_error(req)
             return None
 
     def send_crossweb_request(self, method: str, endpoint: str, data: dict = None):
         """
-        Отправляет запрос в Mediascope-API для проект CrossWeb
+        Отправляет запрос в Mediascope-API для проекта CrossWeb
 
         method : str
             HTTP метод:
                 - get
                 - post
 
         endpoint : str
@@ -342,15 +341,15 @@
                 /task/duplication
 
         data : dict
             Данные отправляемые в запросе к API
 
         use_cache : bool
             Флаг кэширования
-                - True - использовать кэш. Формирует хэш для запроса и сохраняет результат в файл.
+                - True - использовать кэш. Формирует кэш для запроса, и сохраняет результат в файл.
                         Если следующие запросы совпадут по хэшу с существующим - результат возьмется из сохраненного
                         файла. Запроса к API не будет. Удобно использовать для частых запросов к большим объемам.
                 - False - кэш не используется (по умолчанию).
 
         Returns
         -------
 
@@ -378,15 +377,15 @@
 
         elif req is not None:
             self._raise_error(req)
             return None
 
     def get_curl_request(self, method: str, endpoint: str, data: dict = None) -> str:
         """
-        Формирует запрос к Mediascope-API в в CURL формате.
+        Формирует запрос к Mediascope-API в CURL формате.
         Можно вставлять в консоль и обратиться к API прямо из консоли.
         При этом используется текущий токен пользователи или получается новый.
 
         method : str
             HTTP метод:
                 - get
                 - post
@@ -397,15 +396,15 @@
                 /task/duplication
 
         data : dict
             Данные отправляемые в запросе к API
 
         use_cache : bool
             Флаг кэширования
-                - True - использовать кэш. Формирует хэш для запроса и сохраняет результат в файл.
+                - True - использовать кэш. Формирует кэш для запроса, и сохраняет результат в файл.
                         Если следующие запросы совпадут по хэшу с существующим - результат возьмется из сохраненного
                         файла. Запроса к API не будет. Удобно использовать для частых запросов к большим объемам.
                 - False - кэш не используется (по умолчанию).
 
         Returns
         -------
 
@@ -422,15 +421,15 @@
 
         treq = list()
         treq.append(f"curl --location --request {str(method).upper()} '{url}'")
         treq.append(f"--header 'Content-Type: application/json'")
         treq.append(f"--header 'Authorization: Bearer {self.token['access_token']}'")
         if len(data) > 0:
             treq.append(f"--data-raw '{data}'")
-        print(" \\\n".join(treq))
+        return " \\\n".join(treq)
 
     @staticmethod
     def _raise_error(req):
         if req.status_code == 204:
             raise Exception('Нет данных', f'Code: {req.status_code}, Сообщение: "{req.text}"')
         elif req.status_code == 401:
             raise Exception('Не авторизирован', f'Code: {req.status_code}, Сообщение: "{req.text}"')
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/sql.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/sql.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/tasks.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/core/utils.py` & `mediascope_api_lib-1.1.9/mediascope_api/core/utils.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/counter/tasks.py` & `mediascope_api_lib-1.1.9/mediascope_api/counter/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             cls.instance = super().__new__(cls, *args, **kwargs)
         return cls.instance
 
     def __init__(self, settings_filename: str = None, cache_path: str = None, cache_enabled: bool = True,
                  username: str = None, passw: str = None, root_url: str = None, client_id: str = None,
                  client_secret: str = None, keycloak_url: str = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
         self.msapi_network = net.MediascopeApiNetwork(settings_filename, cache_path, cache_enabled, username, passw,
                                                       root_url, client_id, client_secret, keycloak_url)
         self.task_builder = tasks.TaskBuilder()
 
     def build_task(self, task_name: str = '', date_filter: list = None, area_type_filter: list = None,
                    partner_filter: list = None, tmsec_filter: list = None, geo_filter: str = None,
                    device_type_filter: list = None, slices: list = None, statistics: list = None,
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/crossweb/catalogs.py` & `mediascope_api_lib-1.1.9/mediascope_api/crossweb/catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             res['optionValue'].append(item['optionValue'])
             res['sliceUnit'].append(item['sliceUnit'])
             if item['hasOptions']:
                 res['optionName'].append(item['optionName'])
             else:
                 res['optionName'].append('')
         return pd.DataFrame(res)
-
+    
     def load_monitoring_property(self):
         """
         Загрузить список переменных: все, по id или поиском по названию
 
         Returns
         -------
         DemoAttribs : DataFrame
@@ -193,15 +193,15 @@
             res['optionValue'].append(item['optionValue'])
             res['sliceUnit'].append(item['sliceUnit'])
             if item['hasOptions']:
                 res['optionName'].append(item['optionName'])
             else:
                 res['optionName'].append('')
         return pd.DataFrame(res)
-
+    
     def load_media_duplication_property(self):
         """
         Загрузить список переменных: все, по id или поиском по названию
 
         Returns
         -------
         DemoAttribs : DataFrame
@@ -336,29 +336,29 @@
                 v = val
             if type(v) == list:
                 data[k] = v
 
         if len(data) > 0:
             return json.dumps(data)
 
-    def get_slices(self, slice_name):
+    def get_slices(self, slice_name):        
         if slice_name == "adDescription" or slice_name == "eventDescription":
             if type(self.units_monitoring) != dict or \
                     self.units_monitoring.get('slices', None) is None or \
                     self.units_monitoring['slices'].get(slice_name, None) is None:
                 return
             return self.units_monitoring['slices'][slice_name]
         else:
             if slice_name == "duplicationMart":
                 if type(self.units_monitoring) != dict or \
                     self.units_media_duplication.get('slices', None) is None or \
                     self.units_media_duplication['slices'].get(slice_name, None) is None:
                     return
                 return self.units_media_duplication['slices'][slice_name]
-            else:
+            else:            
                 if type(self.units) != dict or \
                         self.units.get('slices', None) is None or \
                         self.units['slices'].get(slice_name, None) is None:
                     return
                 return self.units['slices'][slice_name]
 
     @staticmethod
@@ -1168,29 +1168,29 @@
 
         Returns
         -------
         info : dict
             Словарь с доступными списками
         """
         return self.msapi_network.send_request('get', self._urls['total_unit'], use_cache=False)
-
+    
     def get_monitoring_unit(self):
         """
         Получить списки доступных для использования в заданиях для мониторинга:
         - статистик
         - срезов
         - фильтров
 
         Returns
         -------
         info : dict
             Словарь с доступными списками
         """
         return self.msapi_network.send_request('get', self._urls['monitoring_unit'], use_cache=False)
-
+    
     def get_media_duplication_unit(self):
         """
         Получить списки доступных для использования в заданиях для пересечений:
         - статистик
         - срезов
         - фильтров
 
@@ -1268,15 +1268,15 @@
         if name is not None:
             df = df[df['name'].str.contains(name, case=False)]
 
         return df
 
     def get_product_brand(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список товарных брендов
 
         Parameters
         ----------
@@ -1372,44 +1372,44 @@
 
             DataFrame с товарными брендами
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_brand', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_category_l1(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список категорий товаров и услуг (уровень 1)
 
         Parameters
         ----------
@@ -1505,44 +1505,44 @@
 
             DataFrame с категориями товаров и услуг (уровень 1)
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_category_l1', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_category_l2(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список категорий товаров и услуг (уровень 2)
 
         Parameters
         ----------
@@ -1638,44 +1638,44 @@
 
             DataFrame с категориями товаров и услуг (уровень 2)
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_category_l2', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_category_l3(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список категорий товаров и услуг (уровень 3)
 
         Parameters
         ----------
@@ -1771,44 +1771,44 @@
 
             DataFrame с категориями товаров и услуг (уровень 3)
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_category_l3', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_category_l4(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список категорий товаров и услуг (уровень 4)
 
         Parameters
         ----------
@@ -1904,44 +1904,44 @@
 
             DataFrame с категориями товаров и услуг (уровень 4)
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_category_l4', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_model(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список товарных моделей
 
         Parameters
         ----------
@@ -2037,44 +2037,44 @@
 
             DataFrame с товарными моделями
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_model', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_subbrand(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список товарных суббрендов
 
         Parameters
         ----------
@@ -2170,41 +2170,41 @@
 
             DataFrame с товарными суббрендами
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
 
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('product_subbrand', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_ad_network(self):
         """
         Получить список рекламных сетей
 
         Returns
         -------
         products : DataFrame
@@ -2225,15 +2225,15 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_ad_placement(self):
         """
         Получить список мест размещений для рекламы в социальных сетях
 
         Returns
         -------
         products : DataFrame
@@ -2254,15 +2254,15 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_ad_player(self):
         """
         Получить список рекламных плееров
 
         Returns
         -------
         products : DataFrame
@@ -2283,15 +2283,15 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_ad_server(self):
         """
         Получить список рекламных серверов
 
         Returns
         -------
         products : DataFrame
@@ -2312,15 +2312,15 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_ad_source_type(self):
         """
         Получить список типов рекламы
 
         Returns
         -------
         products : DataFrame
@@ -2341,15 +2341,15 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_ad_video_utility(self):
         """
         Получить список принадлежности к видео
 
         Returns
         -------
         products : DataFrame
@@ -2370,18 +2370,18 @@
         for item in data['data']:
             # print(item)
             # print(type(item))
             res['id'].append(item['id'])
             res['name'].append(item['name'])
 
         return pd.DataFrame(res)
-
+    
     def get_product_advertiser(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить список рекламодателей
 
         Parameters
         ----------
@@ -2477,44 +2477,44 @@
 
             DataFrame с рекламодателями
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
-
+        
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
         return self._get_dict('advertiser', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_monitoring(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить дерево связей рекламных единиц контента в мониторинге
 
         Parameters
         ----------
@@ -2610,45 +2610,45 @@
 
             DataFrame с деревом связей рекламных единиц контента в мониторинге
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
-
+        
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
             'productCategoryL3Ids': product_category_l3_ids,
             'productCategoryL4Ids': product_category_l4_ids
         }
 
         return self._get_dict('monitoring', search_params, body_params, offset, limit, use_cache)
-
+    
     def get_product_category_tree(self, advertiser=None, advertiser_eng=None, product_model=None, product_model_eng=None, product_brand=None, product_brand_eng=None,
             product_subbrand=None, product_subbrand_eng=None, product_category_l1=None, product_category_l1_eng=None, product_category_l2=None,
-            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None,
+            product_category_l2_eng=None, product_category_l3=None, product_category_l3_eng=None, product_category_l4=None, product_category_l4_eng=None, 
             advertiser_ids=None, product_model_ids=None, product_brand_ids=None, product_subbrand_ids=None, product_category_l1_ids=None, product_category_l2_ids=None,
             product_category_l3_ids=None, product_category_l4_ids=None, offset=None, limit=None, use_cache=True):
         """
         Получить дерево категорий товаров и услуг
 
         Parameters
         ----------
@@ -2744,29 +2744,29 @@
 
             DataFrame с деревом категорий товаров и услуг
         """
         search_params = {
             'advertiserName': advertiser,
             'advertiserEngName': advertiser_eng,
             'productModelName': product_model,
-            'productModelEngName': product_model_eng,
+            'productModelEngName': product_model_eng, 
             'productBrandName': product_brand,
             'productBrandEngName': product_brand_eng,
             'productSubbrandName': product_subbrand,
             'productSubbrandEngName': product_subbrand_eng,
             'productCategoryL1Name': product_category_l1,
             'productCategoryL1EngName': product_category_l1_eng,
             'productCategoryL2Name': product_category_l2,
             'productCategoryL2EngName': product_category_l2_eng,
             'productCategoryL3Name': product_category_l3,
             'productCategoryL3EngName': product_category_l3_eng,
-            'productCategoryL4Name': product_category_l4,
-            'productCategoryL4EngName': product_category_l4_eng
+            'productCategoryL4Name': product_category_l4, 
+            'productCategoryL4EngName': product_category_l4_eng            
         }
-
+        
         body_params = {
             'advertiserIds': advertiser_ids,
             'productModelIds': product_model_ids,
             'productBrandIds': product_brand_ids,
             'productSubbrandIds': product_subbrand_ids,
             'productCategoryL1Ids': product_category_l1_ids,
             'productCategoryL2Ids': product_category_l2_ids,
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/crossweb/checks.py` & `mediascope_api_lib-1.1.9/mediascope_api/crossweb/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 return False
             elif type(obj) in [dict, list] and len(obj):
                 msg += self.check_list[name]['msg']
                 return False
         return True
 
     def check_task(self, task_type, date_filter, usetype_filter, geo_filter,
-                   demo_filter, mart_filter, duplication_mart_filter,
+                   demo_filter, mart_filter, duplication_mart_filter, 
                    ad_description_filter, event_description_filter, slices, statistics, scales):
         error_text = ''
         if self._check_filter('task_type', task_type, error_text):
             if task_type not in self.task_types.keys():
                 error_text += self.check_list['task_type']['msg']
 
         if self._check_filter('date_filter', date_filter, error_text):
@@ -165,7 +165,12 @@
         slices = []
         for slice, vals in self.task_types[task_type]['slices'].items():
             for v in vals:
                 slices.append(v)
         return slices
 
 
+
+
+
+
+
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/crossweb/tasks.py` & `mediascope_api_lib-1.1.9/mediascope_api/crossweb/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         mart_filter: str|None
             Условия фильтрации по медиа-объектам
             Пример:
                 mart_filter = "crossMediaResourceId = 1150 OR crossMediaResourceId = 1093"
 
             Список допустимых атрибутов можно получить через метод `get_media_unit` модуля catalogs:
             >>> cats.get_media_unit()['filters']['mart']
-
+        
         slices: list
             Порядок разбивки результата расчета, задается в виде списка
             Пример:
                 slices = ["useTypeName", "researchWeek", "crossMediaResourceId"]
 
             Список допустимых атрибутов можно получить через метод `get_media_unit` модуля catalogs:
             >>> cats.get_media_unit()['slices']
@@ -508,15 +508,15 @@
         Returns
         -------
         text : json
             Ответ сервера, содержит taskid, который необходим для получения результата
 
         """
         return self._send_task('ad', data)
-
+    
     def send_monitoring_task(self, data):
         """
         Отправить задание на расчет аудиторных статистик по мониторингу
 
         Parameters
         ----------
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/mediavortex/catalogs.py` & `mediascope_api_lib-1.1.9/mediascope_api/mediavortex/catalogs.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,33 @@
         'tv-monitoring-type': '/dictionary/tv/monitoring-type',
         'tv-db-rd-type': '/dictionary/tv/db-rd-type',
         'tv-ad-iss-sbtv': '/dictionary/tv/ad-iss-sbtv',
         'tv-demo-attribute': '/dictionary/tv/demo-attribute',
         'tv-program-country': '/dictionary/tv/program-country',
         'tv-company-holding': '/dictionary/tv/company-holding',
         'tv-company-media-holding': '/dictionary/tv/company-media-holding',
-        'tv-company-thematic': '/dictionary/tv/thematic'
+        'tv-thematic': '/dictionary/tv/thematic',
+        'custom-respondent-variable': '/custom-variable/respondent',
+        'tv-issue-status': '/dictionary/tv/issue-status',
+        'tv-area': '/dictionary/tv/area',
+        'tv-prime-time-status': '/dictionary/tv/prime-time-status',
+        'tv-ad-position': '/dictionary/tv/ad-position',
+        'tv-breaks-style': '/dictionary/tv/breaks-style',
+        'tv-breaks-position': '/dictionary/tv/breaks-position',
+        'tv-break-distribution': '/dictionary/tv/breaks-distribution',
+        'tv-breaks-content': '/dictionary/tv/breaks-content',
+        'tv-program-producer-country': '/dictionary/tv/program-producer-country',
+        'tv-program-producer': '/dictionary/tv/program-producer',
+        'tv-program-group': '/dictionary/tv/program-group',
+        'tv-no-yes-na': '/dictionary/tv/no-yes-na',
+        'tv-language': '/dictionary/tv/language',
+        'tv-company-monitoring': '/dictionary/tv/company-monitoring',
+        'tv-company-group': '/dictionary/tv/company-group',
+        'tv-company-category': '/dictionary/tv/company-category',
+        'tv-company-status': '/dictionary/tv/company-status'
     }
 
     def __new__(cls, facility_id=None, settings_filename: str = None, cache_path: str = None,
                 cache_enabled: bool = True, username: str = None, passw: str = None, root_url: str = None,
                 client_id: str = None, client_secret: str = None, keycloak_url: str = None, *args, **kwargs):
         if not hasattr(cls, 'instance'):
             # print("Creating Instance")
@@ -182,15 +200,16 @@
     def _print_header(header, offset, limit):
         if type(header) != dict or 'total' not in header:
             return
         total = header["total"]
         print(
             f'Запрошены записи: {offset} - {offset + limit}\nВсего найдено записей: {total}\n')
 
-    def _get_dict(self, entity_name, search_params=None, body_params=None, offset=None, limit=None, use_cache=True):
+    def _get_dict(self, entity_name, search_params=None, body_params=None, offset=None, limit=None, use_cache=True,
+                  request_type='post'):
         """
         Получить словарь из API
 
         Parameters
         ----------
 
         entity_name : str
@@ -226,42 +245,42 @@
         query = self._get_query(query_dict)
         if query is not None or len(query) > 0:
             url += query
 
         post_data = self._get_post_data(body_params)
 
         data = self.msapi_network.send_request_lo(
-            'post', url, data=post_data, use_cache=use_cache)
+            request_type, url, data=post_data, use_cache=use_cache)
 
         if data is None or type(data) != dict:
             return None
 
         if 'header' not in data or 'data' not in data:
             return None
-        
+
         # извлекаем все заголовки столбцов (их может быть разное количество, особенно для поля notes)
         res_headers = []
         for item in data['data']:
             for k, v in item.items():
                 if k not in res_headers:
-                    res_headers.append(k)        
-               
-        # инициализируем списки данных столбцов        
+                    res_headers.append(k)
+
+                    # инициализируем списки данных столбцов
         res = {}
         for h in res_headers:
             res[h] = []
-        
+
         # наполняем найденные столбцы значениями
         for item in data['data']:
             for h in res_headers:
                 if h in item.keys():
                     res[h].append(item[h])
                 else:
                     res[h].append('')
-            
+
         # print header        
         if offset is not None and limit is not None:
             self._print_header(data['header'], offset, limit)
         else:
             self._print_header(data['header'], 0, data['header']['total'])
         return pd.DataFrame(res)
 
@@ -294,17 +313,17 @@
                         filters = [i['name'] for i in units[0]['reports'][0]['filters']]
 
         result = {
             'statistics': stats,
             'slices': slices,
             'filters': filters
         }
-        
+
         return result
-    
+
     def get_simple_unit(self):
         """
         Получить списки доступных для использования в заданиях для simple:
         - статистик
         - срезов
         - фильтров
 
@@ -329,144 +348,125 @@
                     if 'filters' in units[0]['reports'][1]:
                         filters = [i['name'] for i in units[0]['reports'][1]['filters']]
 
         result = {
             'statistics': stats,
             'slices': slices,
             'filters': filters
-        }        
+        }
 
         return result
-    
+
     def get_crosstab_unit(self):
         """
         Получить списки доступных для использования в заданиях для crosstab:
         - статистик
         - срезов
         - фильтров
 
         Returns
         -------
         info : dict
             Словарь с доступными списками
         """
-        
+
+        units = self.msapi_network.send_request(
+            'get', self._urls['tv-kit'], use_cache=False)
+
+        stats = []
+        slices = []
+        filters = []
+        if len(units) > 0:
+            if 'reports' in units[0]:
+                if len(units[0]['reports']) > 2:
+                    if 'statistics' in units[0]['reports'][2]:
+                        stats = [i['name'] for i in units[0]['reports'][2]['statistics']]
+                    if 'slices' in units[0]['reports'][2]:
+                        slices = [i['name'] for i in units[0]['reports'][2]['slices']]
+                    if 'filters' in units[0]['reports'][2]:
+                        filters = [i['name'] for i in units[0]['reports'][2]['filters']]
+
+        result = {
+            'statistics': stats,
+            'slices': slices,
+            'filters': filters
+        }
+
+        return result
+
+    def get_consumption_target_unit(self):
+        """
+        Получить списки доступных для использования в заданиях для consumption target:
+        - статистик
+        - срезов
+        - фильтров
+
+        Returns
+        -------
+        info : dict
+            Словарь с доступными списками
+        """
+
+        units = self.msapi_network.send_request(
+            'get', self._urls['tv-kit'], use_cache=False)
+
+        stats = []
+        slices = []
+        filters = []
+        if len(units) > 0:
+            if 'reports' in units[0]:
+                if len(units[0]['reports']) > 7:
+                    if 'statistics' in units[0]['reports'][7]:
+                        stats = [i['name'] for i in units[0]['reports'][7]['statistics']]
+                    if 'slices' in units[0]['reports'][7]:
+                        slices = [i['name'] for i in units[0]['reports'][7]['slices']]
+                    if 'filters' in units[0]['reports'][7]:
+                        filters = [i['name'] for i in units[0]['reports'][7]['filters']]
+
+        result = {
+            'statistics': stats,
+            'slices': slices,
+            'filters': filters
+        }
+
+        return result
+
+    def get_duplication_timeband_unit(self):
+        """
+        Получить списки доступных для использования в заданиях для duplication_timeband:
+        - статистик
+        - срезов
+        - фильтров
+
+        Returns
+        -------
+        info : dict
+            Словарь с доступными списками
+        """
+
+        units = self.msapi_network.send_request(
+            'get', self._urls['tv-kit'], use_cache=False)
+
+        stats = []
+        slices = []
+        filters = []
+        if len(units) > 0:
+            if 'reports' in units[0]:
+                if len(units[0]['reports']) > 8:
+                    if 'statistics' in units[0]['reports'][8]:
+                        stats = [i['name'] for i in units[0]['reports'][8]['statistics']]
+                    if 'slices' in units[0]['reports'][8]:
+                        slices = [i['name'] for i in units[0]['reports'][8]['slices']]
+                    if 'filters' in units[0]['reports'][8]:
+                        filters = [i['name'] for i in units[0]['reports'][8]['filters']]
+
         result = {
-            'statistics': ['SampleAvg', 'Universe000', 'Rtg000', 'Rtg000Avg', 'RtgPerAvg', 'Rtg000Sum', 'RtgPerSum',
-                           'TAud', 'TAudAvg', 'TAudSum', 'ShareAvg', 'DurationAvg', 'DurationSum', 'Interval',
-                           'RespondentCount', 'Day', 'SummedEventWeight', 'AvReach000', 'AvReachPer', 'TgAffinPer',
-                           'TTVTAud', 'TTVRtg000Sum', 'TTVRtg000Avg', 'TTVRtgPerSum', 'TTVRtgPerAvg', 'SummedWeight',
-                           'CrossTabSummedWeight', 'Universe000Avg', 'CumReach000', 'CumReachPer', 'ATVSum', 'ATVAvg',
-                           'Quantity', 'QuantitySum', 'CostByMinSum', 'CostByGRPSum', 'ConsolidatedCostSum',
-                           'ATVReachAvg', 'ATVReachSum', 'TgAffinPerAvg', 'OTS', 'GRP'],
-            'slices': ['researchDate', 'researchWeek', 'researchMonth', 'researchQuarter', 'researchYear',
-                       'researchHalfYear', 'researchWeekDay', 'researchDayType', 'locationId', 'locationName',
-                       'locationEName', 'timeBand1', 'timeBand5', 'timeBand10', 'timeBand15', 'timeBand30',
-                       'timeBand60', 'tvCompanyId', 'tvCompanyGroupId', 'tvCompanyCategoryId', 'tvCompanyName',
-                       'tvCompanyEName', 'tvCompanyDescription', 'tvCompanyInformation', 'tvCompanyNotes',
-                       'tvThematicID', 'tvCompanyHoldingID', 'tvCompanyMediaHoldingID', 'tvChannelId', 'tvChannelName',
-                       'tvChannelEName', 'tvChannelDescription', 'tvNetId', 'tvNetName', 'tvNetEName',
-                       'tvNetDescription', 'regionId', 'regionName', 'regionEName', 'scaleRange', 'reachInterval',
-                       'geo', 'subGeo', 'sex', 'age', 'education', 'work', 'persNum', 'spendingsOnFood', 'tvNum',
-                       'ageGroup', 'incomeGroupRussia', 'housewife', 'incomeEarner', 'video', 'incLevel', 'kidsNum',
-                       'kidsAge1', 'kidsAge2', 'kidsAge3', 'kidsAge4', 'kidsAge5', 'kidsAge6', 'kidsAge7', 'status',
-                       'business', 'enterprise', 'property', 'maritalStatus', 'lifeCycle', 'computer', 'internet',
-                       'dacha', 'providerSputnik', 'providerAnalogEth', 'providerDigitalEth', 'providerAnalogCbl',
-                       'providerDigitalCbl', 'hasVm', 'kidsAgeC1', 'kidsAgeC2', 'kidsAgeC3', 'kidsAgeC4', 'occupation',
-                       'tradeIndustry', 'incomeGroup', 'federalOkrug', 'indexOkrug', 'incomeScale201401', 'equipmentV2',
-                       'availTvPort1', 'availTvPort2', 'availTvPort3', 'availTvPort4', 'availTvPort5', 'availTvPort6',
-                       'workCompIntern', 'housCompIntern', 'availAmsPort1', 'availAmsPort2', 'availAmsPort3',
-                       'availAmsPort4', 'availAmsPort5', 'availAmsPort6', 'availAmsPort7', 'zdcHholdPersCnt',
-                       'zdcIncomeGroup', 'zdcSex', 'zdcRAge18', 'zdcEducation', 'zdcWork', 'zodiacNet1View',
-                       'zodiacNet2View', 'zodiacNet4View', 'zodiacNet11View', 'zodiacNet83View', 'zodiacNet13View',
-                       'zodiacNet60View', 'zodiacNet12View', 'zodiacNet326View', 'zodiacNet206View', 'zodiacNet257View',
-                       'zodiacNet205View', 'zodiacNet204View', 'zodiacNet255View', 'zodiacNet258View',
-                       'zodiacNet259View', 'zodiacWorkPtview', 'zodiacWorkNptview', 'zodiacHolidayView',
-                       'zodiacNet84View', 'zodiacNet260View', 'zodiacNet286View', 'zodiacNet40View', 'hhSignalKind1',
-                       'hiddenFilterage1', 'hiddenFilterage18641', 'zodiacNet10View', 'zodiacNet270View',
-                       'moscowRegion', 'wghPersNum1', 'existsSmartTv', 'isPrimaryPanel', 'isSecondaryPanel',
-                       'secondPanelSeason', 'secondaryPanelMatrix', 'wghSuburbAgeGroup', 'zdcSocstat', 'wghLang',
-                       'wghDachaTvExist', 'wghDachaSex', 'wghDachaAgeGroup16', 'smartTvYesNo', 'wghVideoGameWoAge',
-                       'wghUsbTvHh', 'cubeCity', 'timezone0', 'hiddenFilterage18Zodiac', 'cube', 'cube100Plus100Minus',
-                       'sputnikTv', 'geoFrom082020', 'hasRouterMeter', 'usageSmartTv', 'hiddenFilterage18640',
-                       'rage1864', 'populationZdk', 'providerIptv', 'providerOtt', 'city', 'programStartTime',
-                       'programFinishTime', 'programRoundedStartTime', 'programRoundedFinishTime', 'programDuration',
-                       'programRoundedDuration', 'programIssueDescriptionName', 'programIssueDescriptionEName',
-                       'programSpotId', 'programId', 'programName', 'programEName', 'programTypeId', 'programTypeName',
-                       'programTypeEName', 'programCountryId', 'programCountryName', 'programCountryEName',
-                       'programCategoryId', 'programCategoryName', 'programCategoryEName', 'programSportId',
-                       'programSportName', 'programSportEName', 'programSportGroupId', 'programSportGroupName',
-                       'programSportGroupEName', 'programProducerId', 'programProducerName', 'programProducerEName',
-                       'programNotes', 'programLive', 'programNational', 'programFirstIssueDate', 'programLanguageId',
-                       'breaksStartTime', 'breaksFinishTime', 'breaksRoundedStartTime', 'breaksRoundedFinishTime',
-                       'breaksDuration', 'breaksRoundedDuration', 'breaksSpotId', 'breaksId', 'breaksName',
-                       'breaksEName', 'breaksStyleId', 'breaksDistributionType', 'breaksPositionType', 
-                       'breaksContentType', 'breaksPosition', 'GRPTypeId', 'GRPTypeName', 'GRPTypeEName', 'price',
-                       'GRPPrice', 'GRPPriceRub', 'GRPCost', 'GRPCostRub', 'adStartTime', 'adFinishTime',
-                       'adRoundedStartTime', 'adRoundedFinishTime', 'adDuration', 'adRoundedDuration', 'adSpotId',
-                       'adId', 'adName', 'adEName', 'adTypeId', 'advertiserListId', 'advertiserListName',
-                       'advertiserListEName', 'brandListId', 'brandListName', 'brandListEName', 'modelListId',
-                       'modelListName', 'modelListEName', 'articleList2Id', 'articleList2Name', 'articleList2EName', 
-                       'articleList3Id', 'articleList3Name', 'articleList3EName', 'articleList4Id', 'articleList4Name',
-                       'articleList4EName', 'adFirstIssueDate', 'subbrandListId', 'subbrandListName',
-                       'subbrandListEName', 'advertiserId', 'advertiserName', 'advertiserEName', 'brandId', 'brandName',
-                       'brandEName', 'subbrandId', 'subbrandName', 'subbrandEName', 'modelId', 'modelName',
-                       'modelEName', 'article2Id', 'article2Name', 'article2EName', 'article3Name', 'article3EName',
-                       'article4Name', 'article4EName'],
-            'filters': ['dataVersionId', 'researchDate', 'researchWeekDay', 'researchDayType', 'locationId',
-                        'timeBand1', 'timeBand5', 'timeBand10', 'timeBand15', 'timeBand30', 'timeBand60',
-                        'tvCompanyId', 'tvCompanyGroupId', 'tvCompanyCategoryId', 'tvChannelId', 'tvNetId', 'regionId',
-                        'subjectGeoType', 'geo', 'subGeo', 'sex', 'age', 'education', 'work', 'persNum',
-                        'spendingsOnFood', 'tvNum', 'ageGroup', 'incomeGroupRussia', 'housewife', 'incomeEarner',
-                        'video', 'incLevel', 'kidsNum', 'kidsAge1', 'kidsAge2', 'kidsAge3', 'kidsAge4', 'kidsAge5',
-                        'kidsAge6', 'kidsAge7', 'status', 'business', 'enterprise', 'property', 'maritalStatus',
-                        'lifeCycle', 'computer', 'internet', 'dacha', 'providerSputnik', 'providerAnalogEth',
-                        'providerDigitalEth', 'providerAnalogCbl', 'providerDigitalCbl', 'hasVm', 'kidsAgeC1',
-                        'kidsAgeC2', 'kidsAgeC3', 'kidsAgeC4', 'occupation', 'tradeIndustry', 'incomeGroup',
-                        'federalOkrug', 'indexOkrug', 'incomeScale201401', 'equipmentV2', 'availTvPort1',
-                        'availTvPort2', 'availTvPort3', 'availTvPort4', 'availTvPort5', 'availTvPort6',
-                        'workCompIntern', 'housCompIntern', 'availAmsPort1', 'availAmsPort2', 'availAmsPort3',
-                        'availAmsPort4', 'availAmsPort5', 'availAmsPort6', 'availAmsPort7', 'zdcHholdPersCnt',
-                        'zdcIncomeGroup', 'zdcSex', 'zdcRAge18', 'zdcEducation', 'zdcWork', 'zodiacNet1View',
-                        'zodiacNet2View', 'zodiacNet4View', 'zodiacNet11View', 'zodiacNet83View', 'zodiacNet13View',
-                        'zodiacNet60View', 'zodiacNet12View', 'zodiacNet326View', 'zodiacNet206View',
-                        'zodiacNet257View', 'zodiacNet205View', 'zodiacNet204View', 'zodiacNet255View',
-                        'zodiacNet258View', 'zodiacNet259View', 'zodiacWorkPtview', 'zodiacWorkNptview',
-                        'zodiacHolidayView', 'zodiacNet84View', 'zodiacNet260View', 'zodiacNet286View',
-                        'zodiacNet40View', 'hhSignalKind1', 'hiddenFilterage1', 'hiddenFilterage18641',
-                        'zodiacNet10View', 'zodiacNet270View', 'moscowRegion', 'wghPersNum1', 'existsSmartTv',
-                        'isPrimaryPanel', 'isSecondaryPanel', 'secondPanelSeason', 'secondaryPanelMatrix',
-                        'wghSuburbAgeGroup', 'zdcSocstat', 'wghLang', 'wghDachaTvExist', 'wghDachaSex',
-                        'wghDachaAgeGroup16', 'smartTvYesNo', 'wghVideoGameWoAge', 'wghUsbTvHh', 'cubeCity',
-                        'timezone0', 'hiddenFilterage18Zodiac', 'cube', 'cube100Plus100Minus', 'sputnikTv',
-                        'geoFrom082020', 'hasRouterMeter', 'usageSmartTv', 'hiddenFilterage18640', 'rage1864',
-                        'populationZdk', 'providerIptv', 'providerOtt', 'city', 'programStartTime',
-                        'programFinishTime', 'programRoundedStartTime', 'programRoundedFinishTime', 'programDuration',
-                        'programRoundedDuration', 'programSpotId', 'programId', 'programName', 'programEName',
-                        'programTypeId', 'programTypeName', 'programTypeEName', 'programCountryId',
-                        'programCountryName', 'programCountryEName', 'programCategoryId', 'programCategoryName',
-                        'programCategoryEName', 'programSportId', 'programSportName', 'programSportEName',
-                        'programSportGroupId', 'programSportGroupName', 'programSportGroupEName', 'programProducerId',
-                        'programProducerName', 'programProducerEName', 'programNotes', 'programLive', 'programNational',
-                        'programFirstIssueDate', 'programLanguageId', 'breaksStartTime', 'breaksFinishTime',
-                        'breaksRoundedStartTime', 'breaksRoundedFinishTime', 'breaksDuration', 'breaksRoundedDuration',
-                        'breaksSpotId', 'breaksId', 'breaksName', 'breaksEName', 'breaksStyleId',
-                        'breaksDistributionType', 'breaksPositionType', 'breaksContentType', 'breaksPosition',
-                        'GRPTypeId', 'GRPTypeName', 'GRPTypeEName', 'price', 'GRPPrice', 'GRPPriceRub', 'GRPCost',
-                        'GRPCostRub', 'adStartTime', 'adFinishTime', 'adRoundedStartTime', 'adRoundedFinishTime',
-                        'adDuration', 'adRoundedDuration', 'adSpotId', 'adId', 'adName', 'adEName', 'adTypeId',
-                        'advertiserListId', 'advertiserListName', 'advertiserListEName', 'brandListId', 'brandListName',
-                        'brandListEName', 'modelListId', 'modelListName', 'modelListEName', 'articleList2Id',
-                        'articleList2Name', 'articleList2EName', 'articleList3Id', 'articleList3Name',
-                        'articleList3EName', 'articleList4Id', 'articleList4Name', 'articleList4EName',
-                        'adFirstIssueDate', 'subbrandListId', 'subbrandListName', 'subbrandListEName', 'advertiserId',
-                        'advertiserName', 'advertiserEName', 'brandId', 'brandName', 'brandEName', 'subbrandId',
-                        'subbrandName', 'subbrandEName', 'modelId', 'modelName', 'modelEName', 'article2Id',
-                        'article2Name', 'article2EName', 'article3Name', 'article3EName', 'article4Name',
-                        'article4EName', 'articleId', 'article3Id', 'article4Id']
+            'statistics': stats,
+            'slices': slices,
+            'filters': filters
         }
 
         return result
 
     def get_tv_tv_ad(self, tv_ad_type_ids=None, advertiser_list_ids=None, brand_list_ids=None, model_list_ids=None,
                      article_list2_ids=None, article_list3_ids=None, article_list4_ids=None, subbrand_list_ids=None,
                      slogan_audio_ids=None, slogan_video_ids=None, ad_style_ids=None, tv_ad_ids=None, name=None,
@@ -700,27 +700,22 @@
             "id": ids,
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-subbrand-list', search_params, body_params, offset, limit, use_cache)
 
-    def get_tv_research_day_type(self, research_day_type=None, name=None, order_by=None, order_dir=None, offset=None,
+    def get_tv_research_day_type(self, order_by=None, order_dir=None, offset=None,
                                  limit=None, use_cache=True):
         """
         Получить типы дней
 
         Parameters
         ----------
-        research_day_type : string
-            Поиск по идентификатору типа дня
-        
-        name : string
-            Поиск по названию типа дня. Можно использовать часть названия
-        
+
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
             Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
 
         offset : int
@@ -745,16 +740,17 @@
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
         body_params = {
-            "researchDayType": research_day_type,
-            "name": name
+            "id": None,
+            "name": None,
+            "ename": None
         }
 
         return self._get_dict('tv-research-day-type', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_region(self, region_ids=None, name=None, ename=None, notes=None, monitoring_type=None, order_by=None,
                       order_dir=None, offset=None, limit=None, use_cache=True):
         """
@@ -818,15 +814,15 @@
 
         return self._get_dict('tv-region', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_program(self, program_ids=None, program_type_ids=None, program_category_ids=None, program_sport_ids=None,
                        sport_group_ids=None, language_ids=None, program_producer_ids=None, program_producer_reg=None,
                        program_producer_year=None, is_program_group=None, is_child=None, country_ids=None, name=None,
                        ename=None, extended_name=None, extended_ename=None, notes=None, order_by=None,
-                       order_dir=None, offset=None, limit=None, use_cache=True):
+                       order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить программы
 
         Parameters
         ----------
         program_ids : list
             Поиск по списку идентификаторов программ
@@ -843,15 +839,15 @@
         sport_group_ids : list
             Поиск по списку идентификаторов спортивных групп
 
         language_ids : list
             Поиск по списку идентификаторов языков
         
         program_producer_ids : list
-            Поиск по списку идентификаторов продюсеров програм
+            Поиск по списку идентификаторов продюсеров программ
         
         program_producer_reg : string
             Поиск по 
         
         program_producer_year : string
             Поиск по году создания
 
@@ -951,15 +947,15 @@
         notes : string
             Поиск по заметкам 
                        
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1010,15 +1006,15 @@
         notes : string
             Поиск по заметкам 
                         
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1069,15 +1065,15 @@
         notes : string
             Поиск по заметкам 
                                     
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1296,15 +1292,15 @@
             "ename": ename,
             "notes": notes
         }
 
         return self._get_dict('tv-prime-time', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_net(self, net_ids=None, name=None, ename=None, order_by=None,
-                   order_dir=None, offset=None, limit=None, use_cache=True):
+                   order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить сети
 
         Parameters
         ----------
         net_ids : list
             Поиск по списку идентификаторов сетей
@@ -1315,15 +1311,15 @@
         ename : string
             Поиск по англоязычному имени сети 
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1349,19 +1345,15 @@
         body_params = {
             "id": net_ids,
             "name": name,
             "ename": ename
         }
 
         df_net = self._get_dict('tv-net', search_params, body_params, offset, limit, use_cache)
-        try:
-            df_net.drop('notes', axis=1, inplace=True)
-        except Exception:
-            return df_net
-        
+        df_net.drop('notes', axis=1, inplace=True, errors='ignore')
         return df_net
 
     def get_tv_model(self, subbrand_ids=None, article_ids=None, ids=None, name=None, ename=None, notes=None,
                      tv_area_ids=None, order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
         """
         Получить модели
 
@@ -1388,15 +1380,15 @@
         tv_area_ids : list
             Поиск по списку идентификаторов телеплощадок 
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1441,21 +1433,21 @@
         ids : list
             Поиск по списку идентификаторов моделей
         
         name : string
             Поиск по имени
         
         ename : string
-            Поиск по англоязычному имени   
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1483,15 +1475,15 @@
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-model-list', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_location(self, location_ids=None, name=None, ename=None, order_by=None,
-                        order_dir=None, offset=None, limit=None, use_cache=True):
+                        order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить места
 
         Parameters
         ----------
         location_ids : list
             Поиск по списку идентификаторов мест
@@ -1502,15 +1494,15 @@
         ename : string
             Поиск по англоязычному имени места
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1551,24 +1543,24 @@
         ids : list
             Поиск по списку идентификаторов типов групп
         
         name : string
             Поиск по имени
         
         notes : string
-            Поиск по заметке   
+            Поиск по заметке
         
         expression : string
             Поиск по выражению 
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1613,15 +1605,15 @@
         rate : list
             Поиск по списку курсов
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1670,15 +1662,15 @@
         notes : string
             Поиск по заметкам 
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1726,15 +1718,15 @@
         day_week_ename : string
             Поиск по англоязычному имени дня  
                       
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1763,15 +1755,15 @@
             "dayWeekEName": day_week_ename
         }
 
         return self._get_dict('tv-day-week', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_company(self, tv_channel_ids=None, tv_net_ids=None, region_ids=None, tv_company_group_ids=None,
                        tv_company_category_ids=None, name=None, ename=None, ids=None, status=None,
-                       information=None, monitoring_type=None, order_by=None, order_dir=None, offset=None, 
+                       information=None, monitoring_type=None, order_by=None, order_dir=None, offset=None,
                        limit=None, use_cache=True):
         """
         Получить телекомпании
 
         Parameters
         ----------        
         tv_channel_ids : list
@@ -1849,19 +1841,15 @@
             "id": ids,
             "status": status,
             "information": information,
             "monitoringType": monitoring_type
         }
 
         df_comp = self._get_dict('tv-company', search_params, body_params, offset, limit, use_cache)
-        try:
-            df_comp.drop('notes', axis=1, inplace=True)
-        except Exception:
-            return df_comp
-        
+        df_comp.drop('notes', axis=1, inplace=True, errors='ignore')
         return df_comp
 
     def get_tv_company_merge(self, tv_channel_merge_ids=None, tv_company_ids=None, ids=None,
                              order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
         """
         Получить объединенные компании
 
@@ -1876,15 +1864,15 @@
         ids : list
             Поиск по списку идентификаторов
                                
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1928,15 +1916,15 @@
         research_day_type : list
             Поиск по списку типов дат 
                         
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -1962,26 +1950,26 @@
         body_params = {
             "researchDate": research_date,
             "researchDayType": research_day_type
         }
 
         return self._get_dict('tv-calendar', search_params, body_params, offset, limit, use_cache)
 
-    def get_tv_break(self, order_by=None, order_dir=None,
-                     offset=None, limit=None, use_cache=True):
+    def get_tv_breaks(self, order_by=None, order_dir=None,
+                      offset=None, limit=None, use_cache=True):
         """
         Получить перерывы
 
         Parameters
         ----------                        
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -2001,18 +1989,25 @@
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
         body_params = {
-
+            "name": None,
+            "ename": None,
+            "id": None,
+            "notes": None,
+            "positionType": None,
+            "distributionType": None,
+            "contentType": None,
+            "styleId": None
         }
 
-        return self._get_dict('tv-break', search_params, body_params, offset, limit, use_cache)
+        return self._get_dict('tv-breaks', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_brand(self, ids=None, name=None, ename=None, notes=None, tv_area_ids=None,
                      order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
         """
         Получить бренды
 
         Parameters
@@ -2127,15 +2122,15 @@
         }
 
         return self._get_dict('tv-brand-list', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_article(self, parent_ids=None, levels=None, ids=None, name=None, ename=None, notes=None,
                        order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
         """
-        Получить статьи
+        Получить товарные категории
 
         Parameters
         ----------        
         parent_ids : list
             Поиск по списку родительских идентификаторов
         
         levels : list
@@ -2172,15 +2167,15 @@
             с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
             получение данных.
 
         Returns
         -------
         media : DataFrame
 
-            DataFrame со статьями
+            DataFrame с товарными категориями
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
@@ -2194,15 +2189,15 @@
         }
 
         return self._get_dict('tv-article', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_article_list4(self, ids=None, name=None, ename=None, order_by=None, order_dir=None,
                              offset=None, limit=None, use_cache=True):
         """
-        Получить список статей 4
+        Получить список товарных категорий рекламы 4 уровня
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов 
         
         name : string
@@ -2230,15 +2225,15 @@
             с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
             получение данных.
 
         Returns
         -------
         media : DataFrame
 
-            DataFrame со списками статей 4
+            DataFrame с товарными категориями рекламы 4 уровня
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
@@ -2249,15 +2244,15 @@
         }
 
         return self._get_dict('tv-article-list4', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_article_list3(self, ids=None, name=None, ename=None, order_by=None, order_dir=None,
                              offset=None, limit=None, use_cache=True):
         """
-        Получить список статей 3
+        Получить список товарных категорий рекламы 3 уровня
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов 
         
         name : string
@@ -2285,15 +2280,15 @@
             с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
             получение данных.
 
         Returns
         -------
         media : DataFrame
 
-            DataFrame со списками статей 3
+            DataFrame с товарными категориями
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
@@ -2304,15 +2299,15 @@
         }
 
         return self._get_dict('tv-article-list3', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_article_list2(self, ids=None, name=None, ename=None, order_by=None, order_dir=None,
                              offset=None, limit=None, use_cache=True):
         """
-        Получить список статей 2
+        Получить список товарных категорий рекламы 2 уровня
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов 
         
         name : string
@@ -2340,15 +2335,15 @@
             с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
             получение данных.
 
         Returns
         -------
         media : DataFrame
 
-            DataFrame со списками статей 2
+            DataFrame с товарными категориями
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
         }
 
@@ -2358,15 +2353,15 @@
             "ename": ename
         }
 
         return self._get_dict('tv-article-list2', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_appendix(self, tv_ad_ids=None, model_ids=None, advertiser_ids=None, article2_ids=None,
                         article3_ids=None, article4_ids=None, subbrand_ids=None, brand_ids=None,
-                        order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
+                        order_by=None, order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить аппендикс
 
         Parameters
         ----------        
         tv_ad_ids : list
             Поиск по списку идентификаторов рекламы
@@ -2553,18 +2548,18 @@
         }
 
         return self._get_dict('tv-advertiser-list', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_ad(self, tv_ad_type_ids=None, advertiser_list_ids=None, brand_list_ids=None, model_list_ids=None,
                   article_list2_ids=None, article_list3_ids=None, article_list4_ids=None, subbrand_list_ids=None,
                   ad_style_ids=None, advertiser_list_main_ids=None, brand_list_main_ids=None, model_list_main_ids=None,
-                  article_list2_main_ids=None, article_list3_main_ids=None, article_list4_main_ids=None, 
+                  article_list2_main_ids=None, article_list3_main_ids=None, article_list4_main_ids=None,
                   subbrand_list_main_ids=None, age_restriction_ids=None, tv_ad_ids=None, name=None,
-                  ename=None, notes=None, standard_durations=None, tv_area_ids=None, slogan_audio_ids=None, 
-                  slogan_video_ids=None, order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
+                  ename=None, notes=None, standard_durations=None, tv_area_ids=None, slogan_audio_ids=None,
+                  slogan_video_ids=None, order_by=None, order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить телерекламу
 
         Parameters
         ----------
         tv_ad_type_ids : list
             Поиск по списку идентификаторов типов рекламы
@@ -2663,16 +2658,16 @@
 
             DataFrame с рекламой
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "tvAdTypeId": tv_ad_type_ids,
             "advertiserListId": advertiser_list_ids,
             "brandListId": brand_list_ids,
             "modelListId": model_list_ids,
             "articleList2Id": article_list2_ids,
             "articleList3Id": article_list3_ids,
@@ -2696,15 +2691,15 @@
             "tvAdSloganAudioId": slogan_audio_ids,
             "tvAdSloganVideoId": slogan_video_ids
         }
 
         return self._get_dict('tv-ad', search_params, body_params, offset, limit, use_cache)
 
     def get_tv_ad_type(self, tv_ad_ids=None, name=None, ename=None, notes=None, accounting_duration_type_ids=None,
-                       is_override=None, position_type=None, is_price=None, order_by=None, order_dir=None, offset=None, 
+                       is_override=None, position_type=None, is_price=None, order_by=None, order_dir=None, offset=None,
                        limit=None, use_cache=True):
         """
         Получить типы телерекламы
 
         Parameters
         ----------        
         tv_ad_ids : list
@@ -2756,16 +2751,16 @@
 
             DataFrame с типами рекламы
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": tv_ad_ids,
             "name": name,
             "ename": ename,
             "notes": notes,
             "accountingDurationType": accounting_duration_type_ids,
             "isOverride": is_override,
@@ -2877,38 +2872,38 @@
             "article3Id": article3_ids,
             "article4Id": article4_ids,
             "fileType": file_type
         }
 
         return self._get_dict('tv-ad-total', search_params, body_params, offset, limit, use_cache)
 
-    def get_tv_ad_style(self, ids=None, name=None, ename=None, notes=None, order_by=None, 
+    def get_tv_ad_style(self, ids=None, name=None, ename=None, notes=None, order_by=None,
                         order_dir=None, offset=None, limit=None, use_cache=True):
         """
         Получить рекламные стили
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени         
+            Поиск по англоязычному имени
         
         notes : string
             Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -2925,16 +2920,16 @@
 
             DataFrame с рекламными стили
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename,
             "notes": notes
         }
 
@@ -2950,21 +2945,21 @@
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени         
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -2981,16 +2976,16 @@
 
             DataFrame с рекламными видео слоганами
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-ad-slogan-video', search_params, body_params, offset, limit, use_cache)
@@ -3005,21 +3000,21 @@
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени         
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3036,25 +3031,25 @@
 
             DataFrame с рекламными аудио слоганами
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-ad-slogan-audio', search_params, body_params, offset, limit, use_cache)
 
-    def get_tv_ad_month(self, tv_company_ids=None, research_month=None, ad_ids=None, from_tv_company_ids=None, 
+    def get_tv_ad_month(self, tv_company_ids=None, research_month=None, ad_ids=None, from_tv_company_ids=None,
                         from_research_month=None, volume=None, count=None, price=None, grp_price=None,
                         issue_status=None, cnd_cost=None, distribution=None, cost_rub=None, grp_cost_rub=None,
                         cnd_cost_rub=None, order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
         """
         Получить месячную рекламу
 
         Parameters
@@ -3129,16 +3124,16 @@
 
             DataFrame с месячной рекламой
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "tvCompanyId": tv_company_ids,
             "researchMonth": research_month,
             "adId": ad_ids,
             "fromTvCompanyId": from_tv_company_ids,
             "fromResearchMonth": from_research_month,
             "volume": volume,
@@ -3181,17 +3176,17 @@
         """
         Получить справочник relation
         
         Returns
         -------
         info : Dict
             Словарь с relation
-        """                
+        """
         return self.msapi_network.send_request('get', self._urls['tv-relation'], use_cache=False)
-    
+
     def get_tv_program_prreg(self):
         """
         Получить справочник видов производства программ
         
         Returns
         -------
         info : DataFrame
@@ -3229,15 +3224,15 @@
         -------
         info : DataFrame
             DataFrame с ad_iss_sbtv
         """
         return pd.DataFrame(self.msapi_network.send_request('get', self._urls['tv-ad-iss-sbtv'], use_cache=False))
 
     def get_tv_demo_attribute(self, ids=None, value_ids=None, names=None, col_names=None, value_names=None,
-                              order_by=None, order_dir=None, offset=None, limit=None, use_cache=True):
+                              order_by=None, order_dir=None, offset=None, limit=None, use_cache=False):
         """
         Получить атрибуты
 
         Parameters
         ----------
         ids : list
             Поиск по списку идентификаторов
@@ -3254,15 +3249,15 @@
         value_names : list
             Поиск по списку имен значений
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3292,16 +3287,16 @@
             "colName": col_names,
             "valueName": value_names,
             "demoAttributeColName": col_names,
             "demoAttributeValueId": value_ids
         }
 
         return self._get_dict('tv-demo-attribute', search_params, body_params, offset, limit, use_cache)
-    
-    def get_tv_program_country(self, ids=None, name=None, ename=None, notes=None, 
+
+    def get_tv_program_country(self, ids=None, name=None, ename=None, notes=None,
                                order_by=None, order_dir=None, offset=None,
                                limit=None, use_cache=True):
         """
         Получить страны производства программ
 
         Parameters
         ----------        
@@ -3311,21 +3306,21 @@
         name : string
             Поиск по имени 
         
         ename : string
             Поиск по англоязычному имени
         
         notes : string
-            Поиск по заметкам         
+            Поиск по заметкам
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3342,47 +3337,47 @@
 
             DataFrame со странами производства программ
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename,
             "notes": notes
         }
 
         return self._get_dict('tv-program-country', search_params, body_params, offset, limit, use_cache)
 
-    def get_tv_company_holding(self, ids=None, name=None, ename=None, 
+    def get_tv_company_holding(self, ids=None, name=None, ename=None,
                                order_by=None, order_dir=None, offset=None,
                                limit=None, use_cache=True):
         """
         Получить список холдингов телекомпаний
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени     
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3399,16 +3394,16 @@
 
             DataFrame с холдингами телекомпаний
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-company-holding', search_params, body_params, offset, limit, use_cache)
@@ -3424,21 +3419,21 @@
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени     
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3455,46 +3450,45 @@
 
             DataFrame с медиа холдингами телекомпаний
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename
         }
 
         return self._get_dict('tv-company-media-holding', search_params, body_params, offset, limit, use_cache)
-    
-    def get_tv_company_thematic(self, ids=None, name=None,
-                                     ename=None, order_by=None, order_dir=None, offset=None,
-                                     limit=None, use_cache=True):
+
+    def get_tv_thematic(self, ids=None, name=None, ename=None, order_by=None, order_dir=None,
+                        offset=None, limit=None, use_cache=True):
         """
-        Получить список жанров телекомпаний
+        Получить список тематик тв рекламы
 
         Parameters
         ----------        
         ids : list
             Поиск по списку идентификаторов
             
         name : string
             Поиск по имени 
         
         ename : string
-            Поиск по англоязычному имени     
+            Поиск по англоязычному имени
             
         order_by : string
             Поле, по которому происходит сортировка
             
         order_dir : string
-            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.      
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
               
         offset : int
             Смещение от начала набора отобранных данных
 
         limit : int
             Количество записей в возвращаемом наборе данных
 
@@ -3505,22 +3499,1138 @@
             с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
             получение данных.
 
         Returns
         -------
         media : DataFrame
 
-            DataFrame с жанрами телекомпаний
+            DataFrame с тематиками тв рекламы
         """
 
         search_params = {
             'orderBy': order_by,
             'orderDir': order_dir
-        } 
-  
+        }
+
         body_params = {
             "id": ids,
             "name": name,
             "ename": ename
         }
 
-        return self._get_dict('tv-company-thematic', search_params, body_params, offset, limit, use_cache)
+        return self._get_dict('tv-thematic', search_params, body_params, offset, limit, use_cache)
+
+    def get_custom_respondent_variable(self, ids=None, mart_type=None, name=None,
+                                       order_by=None, order_dir=None, offset=0, limit=1000, use_cache=False):
+        """
+        Получение списка кастомных respondent переменных
+
+        Parameters
+        ----------
+
+        ids : list
+            Фильтр на список значений id
+
+        mart_type : str
+            Тип витрины
+
+        name : str
+            Фильтр на имя
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame со списком кастомных respondent переменных
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir,
+            "ids": ids,
+            "mart-type": mart_type,
+            "name": name
+        }
+
+        body_params = {}
+
+        return self._get_dict('custom-respondent-variable', search_params, body_params,
+                              offset, limit, use_cache, 'get')
+
+    def add_custom_respondent_variable(self, resp, name, mart_type, is_public=True):
+        """
+        Создание кастомной respondent переменной
+
+        Parameters
+        ----------
+
+        resp : str
+            Закодированные данные пользователей
+
+        name : str
+            Имя переменной
+
+        mart_type : str
+            Тип витрины
+
+        is_public : bool
+            Флаг доступности
+
+        Returns
+        -------
+            Информация о созданной переменной
+        """
+
+        data = {
+            "value": "{\"respondent\": \"" + resp + "\"}",
+            "name": name,
+            "isPublic": is_public,
+            "martType": mart_type
+        }
+
+        return self.msapi_network.send_request('post', self._urls['custom-respondent-variable'],
+                                               data=json.dumps(data), use_cache=False)
+
+    def delete_custom_respondent_variable(self, id_value):
+        """
+        Удаление кастомной respondent переменной
+
+        Parameters
+        ----------
+
+        id_value : str
+            id переменной
+
+        Returns
+        -------
+            Информация о результатах удаления
+        """
+
+        return self.msapi_network.send_request('delete', self._urls['custom-respondent-variable'] + f"/{id_value}",
+                                               use_cache=False)
+
+    def get_tv_program_producer_country(self, country_id=None, name=None, ename=None,
+                                        order_by=None, order_dir=None, offset=None,
+                                        limit=None, use_cache=True):
+        """
+        Получить типы программ производств страны
+
+        Parameters
+        ----------
+        country_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с программ производств страны
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": country_id,
+            "name": name,
+            "ename": ename,
+            "empty": True
+        }
+
+        return self._get_dict('tv-program-producer-country', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_prime_time_status(self, status_id=None, name=None, ename=None,
+                                 order_by=None, order_dir=None, offset=None,
+                                 limit=None, use_cache=True):
+        """
+        Получить прайм-тайм статусы
+
+        Parameters
+        ----------
+        status_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с прайм-тайм статусами
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": status_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-prime-time-status', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_issue_status(self, status_id=None, name=None, ename=None,
+                            order_by=None, order_dir=None, offset=None,
+                            limit=None, use_cache=True):
+        """
+        Получить статусы выпусков
+
+        Parameters
+        ----------
+        status_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame со статусами выпусков
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": status_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-issue-status', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_breaks_style(self, style_id=None, name=None, ename=None,
+                            order_by=None, order_dir=None, offset=None,
+                            limit=None, use_cache=True):
+        """
+        Получить типы стиля перерыва
+
+        Parameters
+        ----------
+        style_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с типами стиля перерыва
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": style_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-breaks-style', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_breaks_position(self, position_id=None, name=None, ename=None,
+                               order_by=None, order_dir=None, offset=None,
+                               limit=None, use_cache=True):
+        """
+        Получить типы позиций перерыва
+
+        Parameters
+        ----------
+        position_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с типами позиций перерыва
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": position_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-breaks-position', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_breaks_distribution(self, distribution_id=None, name=None, ename=None,
+                                   order_by=None, order_dir=None, offset=None,
+                                   limit=None, use_cache=True):
+        """
+        Получить типы распределения перерыва
+
+        Parameters
+        ----------
+        distribution_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с типами распределения перерыва
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": distribution_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-breaks-distribution', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_breaks_content(self, content_id=None, name=None, ename=None,
+                              order_by=None, order_dir=None, offset=None,
+                              limit=None, use_cache=True):
+        """
+        Получить типы контента перерыва
+
+        Parameters
+        ----------
+        content_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с типами контента перерыва
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": content_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-breaks-content', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_area(self, area_id=None, name=None, ename=None,
+                    order_by=None, order_dir=None, offset=None,
+                    limit=None, use_cache=True):
+        """
+        Получить зоны компании тв рекламы
+
+        Parameters
+        ----------
+        area_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с зонами компании тв рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": area_id,
+            "name": name,
+            "ename": ename,
+            "empty": True
+        }
+
+        return self._get_dict('tv-area', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_ad_position(self, ad_position_type=None, name=None, ename=None,
+                           order_by=None, order_dir=None, offset=None,
+                           limit=None, use_cache=True):
+        """
+        Получить типы позиции клипа
+
+        Parameters
+        ----------
+        ad_position_type : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с типами позиции клипа
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "type": ad_position_type,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-ad-position', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_company_status(self, company_status_id=None, name=None, ename=None,
+                              order_by=None, order_dir=None, offset=None,
+                              limit=None, use_cache=True):
+        """
+        Получить статусы компании тв рекламы
+
+        Parameters
+        ----------
+        company_status_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame со статусами компании тв рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": company_status_id,
+            "name": name,
+            "ename": ename,
+            "empty": True
+        }
+
+        return self._get_dict('tv-company-status', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_program_producer(self, program_producer_id=None, name=None, ename=None,
+                                order_by=None, order_dir=None, offset=None,
+                                limit=None, use_cache=True):
+        """
+        Получить производителей программ
+
+        Parameters
+        ----------
+        program_producer_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с производителями программ
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": program_producer_id,
+            "name": name,
+            "ename": ename,
+            "empty": True
+        }
+
+        return self._get_dict('tv-program-producer', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_program_group(self, program_group_id=None, name=None, ename=None,
+                             order_by=None, order_dir=None, offset=None,
+                             limit=None, use_cache=True):
+        """
+        Получить групповые имена программ
+
+        Parameters
+        ----------
+        program_group_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с групповыми именами программ
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": program_group_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-program-group', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_no_yes_na(self, no_yes_na_id=None, name=None, ename=None,
+                         order_by=None, order_dir=None, offset=None,
+                         limit=None, use_cache=True):
+        """
+        Получить Да-Нет-Неизвестно флаги
+
+        Parameters
+        ----------
+        no_yes_na_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с Да-Нет-Неизвестно флагами
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": no_yes_na_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-no-yes-na', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_language(self, language_id=None, name=None, ename=None,
+                        order_by=None, order_dir=None, offset=None,
+                        limit=None, use_cache=True):
+        """
+        Получить языки рекламы
+
+        Parameters
+        ----------
+        language_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с языками рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": language_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-language', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_company_monitoring(self, company_monitoring_id=None, name=None,
+                                  order_by=None, order_dir=None, offset=None,
+                                  limit=None, use_cache=True):
+        """
+        Получить режимы продолжительности компании тв рекламы
+
+        Parameters
+        ----------
+        company_monitoring_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с режимами продолжительности компании тв рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": company_monitoring_id,
+            "name": name,
+            "empty": True
+        }
+
+        return self._get_dict('tv-company-monitoring', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_company_group(self, company_group_id=None, name=None, ename=None,
+                             order_by=None, order_dir=None, offset=None,
+                             limit=None, use_cache=True):
+        """
+        Получить группы компаний тв рекламы
+
+        Parameters
+        ----------
+        company_group_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с группами компаний тв рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": company_group_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-company-group', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_company_category(self, company_category_id=None, name=None, ename=None,
+                                order_by=None, order_dir=None, offset=None,
+                                limit=None, use_cache=True):
+        """
+        Получить категории компаний тв рекламы
+
+        Parameters
+        ----------
+        company_category_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame с категориями компаний тв рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": company_category_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-company-category', search_params, body_params, offset, limit, use_cache)
+
+    def get_tv_brand_list(self, brand_list_id=None, name=None, ename=None, order_by=None,
+                          order_dir=None, offset=None, limit=None, use_cache=True):
+        """
+        Получить списки брендов рекламы
+
+        Parameters
+        ----------
+        brand_list_id : string
+            Ид для фильтрации
+
+        name : string
+            Имя для фильтрации
+
+        ename : string
+            Английское имя для фильтрации
+
+        order_by : string
+            Поле, по которому происходит сортировка
+
+        order_dir : string
+            Направление сортировки данных. Возможные значения ASC - по возрастанию и DESC - по убыванию.
+
+        offset : int
+            Смещение от начала набора отобранных данных
+
+        limit : int
+            Количество записей в возвращаемом наборе данных
+
+        use_cache : bool
+            Использовать кэширование: True - да, False - нет
+            Если опция включена (True), метод при первом получении справочника
+            сохраняет его в кэш на локальном диске, а при следующих запросах этого же справочника
+            с такими же параметрами - читает его из кэша, это позволяет существенно ускорить
+            получение данных.
+
+        Returns
+        -------
+        result : DataFrame
+
+            DataFrame со списками брендов рекламы
+        """
+
+        search_params = {
+            'orderBy': order_by,
+            'orderDir': order_dir
+        }
+
+        body_params = {
+            "id": brand_list_id,
+            "name": name,
+            "ename": ename
+        }
+
+        return self._get_dict('tv-brand-list', search_params, body_params, offset, limit, use_cache)
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/mediavortex/checks.py` & `mediascope_api_lib-1.1.9/mediascope_api/mediavortex/checks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from . import catalogs
 from ..core import sql
+import difflib as dl
 
 
 class MediaVortexTaskChecker:
-
     def __new__(cls, cats: catalogs.MediaVortexCats, *args, **kwargs):
         if not hasattr(cls, 'instance'):
             cls.instance = super(MediaVortexTaskChecker, cls).__new__(cls, *args)
         return cls.instance
 
     def __init__(self, cats: catalogs.MediaVortexCats, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.cats = cats
         self.task_types = {
             'timeband': self.cats.get_timeband_unit(),
             'simple': self.cats.get_simple_unit(),
-            'crosstab': self.cats.get_crosstab_unit()
+            'crosstab': self.cats.get_crosstab_unit(),
+            'consumption-target': self.cats.get_consumption_target_unit(),
+            'duplication-timeband': self.cats.get_duplication_timeband_unit()
             }
         self.check_list = {
-            'task_type': {'types': [str], 'msg': 'Неверно задан тип задачи\n' +
-                                                  f'Допустимые варианты: "{", ".join(self.task_types.keys())}\n"'
-                          },
+            'task_type': {
+                'types': [str], 'msg': 'Неверно задан тип задачи\n' +
+                f'Допустимые варианты: "{", ".join(self.task_types.keys())}\n"'
+                },
             'date_filter': {'types': [list], 'msg': 'Период должен быть задан, формат: ' +
                                                     '[("YYYY-MM-DD", "YYYY-MM-DD")]\n'},
             'date_filter_item': {'types': [tuple], 'msg': 'Диапазон дат внутри периода должен быть задан как tuple,' +
                                                           'формат: [("YYYY-MM-DD", "YYYY-MM-DD")] \n'},
             'weekdate_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по дням недели.\n'},
             'daytype_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по типам дней.\n'},
             'company_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по телекомпаниям.\n'},
@@ -34,14 +37,16 @@
             'basedemo_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по базовому демо.\n'},
             'targetdemo_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по целевому демо.\n'},
             'program_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по программам.\n'},
             'break_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по перерывам.\n'},
             'ad_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по рекламе.\n'},
             'subject_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по теме.\n'},
             'duration_filter': {'types': [str, dict], 'msg': 'Неверно задан фильтр по длительности.\n'},
+            'duplication_company_filter': {'types': [str, dict], 'msg': 'Неверно задан duplication company фильтр.\n'},
+            'duplication_time_filter': {'types': [str, dict], 'msg': 'Неверно задан duplication time фильтр.\n'},
             'statistics': {'types': [list], 'msg': 'Не заданы статистики для задания.\n'},
         }        
         self.error_text = ''
 
     def _check_filter(self, name, obj):
         if name not in self.check_list:
             return False
@@ -57,32 +62,37 @@
     def _check_filter_units(self, task_type, name, obj):
         result = True
         if obj:
             units = sql.sql_to_units(obj)                        
             for u in units:
                 if u not in self.task_types[task_type]['filters']:
                     result = False
-                    self.error_text += f'Неизвестная переменная "{u}" в фильтре "{name}".\n'
+                    self.error_text += f'Неизвестная переменная "{u}" в фильтре "{name}". '
+                    probably_matches = dl.get_close_matches(u, self.task_types[task_type]['filters'], n=3)
+                    if len(probably_matches) > 0:
+                        matches = '" или "'.join(probably_matches)
+                        self.error_text += f'Возможно соответствует "{matches}".\n'
         return result
 
     def check_task(self, task_type, date_filter, weekdate_filter, daytype_filter,
                    company_filter, region_filter, time_filter, location_filter,
                    basedemo_filter, targetdemo_filter, program_filter, break_filter,
-                   ad_filter, subject_filter, duration_filter, slices, statistics, scales):
+                   ad_filter, subject_filter, duration_filter, duplication_company_filter,
+                   duplication_time_filter, slices, statistics, scales):
         self.error_text = ''
         
         self._check_filter('task_type', task_type)
 
         if self._check_filter('date_filter', date_filter):
             for r in date_filter:                
                 self._check_filter('date_filter_item', r)
 
         self._check_scales(statistics, scales)
         if self._check_filter('weekdate_filter', weekdate_filter):
-           self._check_filter_units(task_type, 'weekdate_filter', weekdate_filter)
+            self._check_filter_units(task_type, 'weekdate_filter', weekdate_filter)
         
         if self._check_filter('daytype_filter', daytype_filter):
             self._check_filter_units(task_type, 'daytype_filter', daytype_filter)
                     
         if self._check_filter('company_filter', company_filter):
             self._check_filter_units(task_type, 'company_filter', company_filter)
                     
@@ -111,14 +121,20 @@
             self._check_filter_units(task_type, 'ad_filter', ad_filter)
         
         if self._check_filter('subject_filter', subject_filter):
             self._check_filter_units(task_type, 'subject_filter', subject_filter)
         
         if self._check_filter('duration_filter', duration_filter):
             self._check_filter_units(task_type, 'duration_filter', duration_filter)
+
+        if self._check_filter('duplication_company_filter', duplication_company_filter):
+            self._check_filter_units(task_type, 'duplication_company_filter', duplication_company_filter)
+
+        if self._check_filter('duplication_time_filter', duplication_time_filter):
+            self._check_filter_units(task_type, 'duplication_time_filter', duplication_time_filter)
         
         if slices is not None:
             if type(slices) is not list:
                 self.error_text += f'Неверно заданы срезы (slices).\n'
             else:
                 for s in slices:
                     if type(s) is not str:
@@ -151,25 +167,34 @@
 
     def check_units_in_task(self, task_type, tsk):
         error_text = ''
 
         if type(tsk['statistics']) == list:
             for s in tsk['statistics']:
                 if s not in self.task_types[task_type]['statistics']:
-                    error_text += f'Неизвестная  статистика "{s}".\n'
+                    error_text += f'Неизвестная статистика "{s}". '
+                    probably_matches = dl.get_close_matches(s, self.task_types[task_type]['statistics'], n=3)
+                    if len(probably_matches) > 0:
+                        matches = '" или "'.join(probably_matches)
+                        error_text += f'Возможно соответствует "{matches}".\n'
         if type(tsk['filter']) == list:
             for filter_name in tsk['filter']:                
                 self.check_units(f'фильтрах {filter_name}', filter_name,
                                  self.task_types[task_type]['filters'],
                                  error_text)
-        if type(tsk['slices']) == list:
-            avl_slices = self.get_avl_slices(task_type)
-            for slice_name in tsk['slices']:
-                if slice_name not in avl_slices:
-                    error_text += f'Недопустимое название среза: "{slice_name}"'
+        if task_type != 'consumption-target':
+            if type(tsk['slices']) == list:
+                avl_slices = self.get_avl_slices(task_type)
+                for slice_name in tsk['slices']:
+                    if slice_name not in avl_slices:
+                        error_text += f'Недопустимое название среза: "{slice_name}". '
+                        probably_matches = dl.get_close_matches(slice_name, avl_slices, n=3)
+                        if len(probably_matches) > 0:
+                            matches = '" или "'.join(probably_matches)
+                            error_text += f'Возможно соответствует "{matches}".\n'
         if len(error_text) > 0:
             print('Ошибка при формировании задания')
             print(error_text)
             return False
         else:
             return True
 
@@ -189,14 +214,7 @@
     def check_units(task_item_name, task_units, avl_units, error_text):
         for unit in task_units:
             if unit not in avl_units:
                 error_text += f'Недопустимое название атрибута: "{unit}" в {task_item_name}'
 
     def get_avl_slices(self, task_type):        
         return self.task_types[task_type]['slices']
-
-
-
-
-
-
-
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/responsum/catalogs.py` & `mediascope_api_lib-1.1.9/mediascope_api/responsum/catalogs.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api/responsum/tasks.py` & `mediascope_api_lib-1.1.9/mediascope_api/responsum/tasks.py`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/PKG-INFO` & `mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mediascope-api-lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: Library for work with the Mediascope-Delivery-API
 Home-page: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib
-Download-URL: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.8
+Download-URL: https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.9
 Author: Sergey Poterianski
 Author-email: sergey.poterianski@mediascope.net
 Maintainer: Mediascope JSC
 Maintainer-email: github@mediascope.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mediascope_api_lib-1.1.8/mediascope_api_lib.egg-info/SOURCES.txt` & `mediascope_api_lib-1.1.9/mediascope_api_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediascope_api_lib-1.1.8/setup.py` & `mediascope_api_lib-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import find_packages
 from setuptools import setup
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='mediascope_api_lib',
     packages=find_packages(),
-    version='1.1.8',
+    version='1.1.9',
     description='Library for work with the Mediascope-Delivery-API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Sergey Poterianski',
     author_email='sergey.poterianski@mediascope.net',
     maintainer='Mediascope JSC',
     maintainer_email='github@mediascope.net',
     license='BSD-3-Clause',
     requires=['pandas', 'requests', 'pyparsing'],
     install_requires=['pandas', 'requests', 'pyparsing'],
     url='https://github.com/MEDIASCOPE-JSC/mediascope-api-lib',
-    download_url='https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.8',
+    download_url='https://github.com/MEDIASCOPE-JSC/mediascope-api-lib/tarball/v1.1.9',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.6",
         "Natural Language :: Russian",
         "License :: OSI Approved :: BSD License",
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
```

