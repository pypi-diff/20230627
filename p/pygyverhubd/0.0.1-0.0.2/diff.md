# Comparing `tmp/pygyverhubd-0.0.1.tar.gz` & `tmp/pygyverhubd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygyverhubd-0.0.1.tar", last modified: Mon Jun 26 19:15:33 2023, max compression
+gzip compressed data, was "pygyverhubd-0.0.2.tar", last modified: Tue Jun 27 07:17:04 2023, max compression
```

## Comparing `pygyverhubd-0.0.1.tar` & `pygyverhubd-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.655892 pygyverhubd-0.0.1/
--rw-rw-rw-   0        0        0     1104 2023-06-20 18:43:04.000000 pygyverhubd-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3472 2023-06-26 19:15:33.655892 pygyverhubd-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1645 2023-06-26 18:24:38.000000 pygyverhubd-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.628804 pygyverhubd-0.0.1/gyverhubd/
--rw-rw-rw-   0        0        0      448 2023-06-26 19:06:52.000000 pygyverhubd-0.0.1/gyverhubd/__init__.py
--rw-rw-rw-   0        0        0     7010 2023-06-26 18:21:39.000000 pygyverhubd-0.0.1/gyverhubd/device.py
--rw-rw-rw-   0        0        0     3008 2023-06-26 17:22:12.000000 pygyverhubd-0.0.1/gyverhubd/filesystem.py
--rw-rw-rw-   0        0        0     2610 2023-06-26 18:21:39.000000 pygyverhubd-0.0.1/gyverhubd/info.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.631803 pygyverhubd-0.0.1/gyverhubd/proto/
--rw-rw-rw-   0        0        0       54 2023-06-22 17:24:21.000000 pygyverhubd-0.0.1/gyverhubd/proto/__init__.py
--rw-rw-rw-   0        0        0      705 2023-06-25 05:08:39.000000 pygyverhubd-0.0.1/gyverhubd/proto/proto.py
--rw-rw-rw-   0        0        0     3289 2023-06-26 17:11:42.000000 pygyverhubd-0.0.1/gyverhubd/proto/ws.py
--rw-rw-rw-   0        0        0     2107 2023-06-25 05:08:39.000000 pygyverhubd-0.0.1/gyverhubd/server.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.636318 pygyverhubd-0.0.1/gyverhubd/ui/
--rw-rw-rw-   0        0        0       70 2023-06-26 16:07:49.000000 pygyverhubd-0.0.1/gyverhubd/ui/__init__.py
--rw-rw-rw-   0        0        0      202 2023-06-26 15:59:24.000000 pygyverhubd-0.0.1/gyverhubd/ui/base.py
--rw-rw-rw-   0        0        0    12614 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/builder.py
--rw-rw-rw-   0        0        0     3517 2023-06-26 17:01:33.000000 pygyverhubd-0.0.1/gyverhubd/ui/component.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.645848 pygyverhubd-0.0.1/gyverhubd/ui/components/
--rw-rw-rw-   0        0        0        0 2023-06-25 06:56:00.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/__init__.py
--rw-rw-rw-   0        0        0      616 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/button.py
--rw-rw-rw-   0        0        0     1393 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/controls.py
--rw-rw-rw-   0        0        0     1261 2023-06-26 16:42:45.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/datetime.py
--rw-rw-rw-   0        0        0      346 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/input.py
--rw-rw-rw-   0        0        0      191 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/prompt_confirm.py
--rw-rw-rw-   0        0        0      534 2023-06-26 16:41:15.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/spinner.py
--rw-rw-rw-   0        0        0      539 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/switch.py
--rw-rw-rw-   0        0        0      553 2023-06-26 16:29:25.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/tabs.py
--rw-rw-rw-   0        0        0     1974 2023-06-26 17:04:39.000000 pygyverhubd-0.0.1/gyverhubd/ui/components/text.py
--rw-rw-rw-   0        0        0     2121 2023-06-26 16:08:59.000000 pygyverhubd-0.0.1/gyverhubd/ui/layout.py
--rw-rw-rw-   0        0        0     3639 2023-06-26 17:51:50.000000 pygyverhubd-0.0.1/gyverhubd/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:15:33.654383 pygyverhubd-0.0.1/pygyverhubd.egg-info/
--rw-rw-rw-   0        0        0     3472 2023-06-26 19:15:33.000000 pygyverhubd-0.0.1/pygyverhubd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-06-26 19:15:33.000000 pygyverhubd-0.0.1/pygyverhubd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 19:15:33.000000 pygyverhubd-0.0.1/pygyverhubd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-26 19:15:33.000000 pygyverhubd-0.0.1/pygyverhubd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 19:15:33.000000 pygyverhubd-0.0.1/pygyverhubd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      935 2023-06-26 19:13:06.000000 pygyverhubd-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 19:15:33.655892 pygyverhubd-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.286826 pygyverhubd-0.0.2/gyverhubd/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.290826 pygyverhubd-0.0.2/gyverhubd/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.290826 pygyverhubd-0.0.2/gyverhubd/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/gyverhubd/ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/prompt_confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/pygyverhubd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/setup.cfg
```

### Comparing `pygyverhubd-0.0.1/LICENSE` & `pygyverhubd-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pygyverhubd-0.0.1/PKG-INFO` & `pygyverhubd-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-Metadata-Version: 2.1
-Name: pygyverhubd
-Version: 0.0.1
-Summary: Python implementation of GyverHub device
-Author-email: NekoNekoNyan <me@neko-dev.ru>
-License: MIT License
-        
-        Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/neko-neko-nyan/pygyverhubd
-Project-URL: Bug Tracker, https://github.com/neko-neko-nyan/pygyverhubd/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Реализация сервера (устройства) GyverHub на python
-
-## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
-
-На данный момент работает только WebSocket
-
-Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
-(кроме передачи файлов по http)
-
-Пример использования [здесь](examples/components_ui.py)
-
-# Текущий прогресс
-## Сеть
-- [x] Интерфейс: WebSocket
-- [ ] Интерфейс: MQTT
-- [ ] Интерфейс: Bluetooth
-- [ ] Интерфейс: Serial
-- [x] Device discovery
-- [ ] Встроенный клиент
-
-## GUI
-- [x] Базовые компоненты
-- [ ] Canvas
-- [ ] Вкладки
-
-## Устройство
-- [x] Базовая информация - название, иконка
-- [x] Расширенная информация - сеть, память
-- [ ] Автоматический сбор расширенной информации
-
-## OTA
-- [x] OTA API
-- [ ] Обновление сервера через OTA
-- [ ] Автообновление
-- [ ] Автоматическая упаковка обновлений
-
-## ФС
-- [x] API файловой системы
-- [ ] Отражение API ФС на реальную папку
-
-## Другие компоненты
-- [ ] Перезапуск сервера по команде reboot
-- [x] CLI API
+Metadata-Version: 2.1
+Name: pygyverhubd
+Version: 0.0.2
+Summary: Python implementation of GyverHub device
+Author-email: NekoNekoNyan <me@neko-dev.ru>
+License: MIT License
+        
+        Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/neko-neko-nyan/pygyverhubd
+Project-URL: Bug Tracker, https://github.com/neko-neko-nyan/pygyverhubd/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Реализация сервера (устройства) GyverHub на python
+
+## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
+
+На данный момент работает только WebSocket
+
+Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
+(кроме передачи файлов по http)
+
+Пример использования [здесь](examples/components_ui.py)
+
+# Текущий прогресс
+## Сеть
+- [x] Интерфейс: WebSocket
+- [ ] Интерфейс: MQTT
+- [ ] Интерфейс: Bluetooth
+- [ ] Интерфейс: Serial
+- [x] Device discovery
+- [ ] Встроенный клиент
+
+## GUI
+- [x] Базовые компоненты
+- [ ] Canvas
+- [ ] Вкладки
+
+## Устройство
+- [x] Базовая информация - название, иконка
+- [x] Расширенная информация - сеть, память
+- [ ] Автоматический сбор расширенной информации
+
+## OTA
+- [x] OTA API
+- [ ] Обновление сервера через OTA
+- [ ] Автообновление
+- [ ] Автоматическая упаковка обновлений
+
+## ФС
+- [x] API файловой системы
+- [ ] Отражение API ФС на реальную папку
+
+## Другие компоненты
+- [ ] Перезапуск сервера по команде reboot
+- [x] CLI API
```

### Comparing `pygyverhubd-0.0.1/README.md` & `pygyverhubd-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
-# Реализация сервера (устройства) GyverHub на python
-
-## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
-
-На данный момент работает только WebSocket
-
-Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
-(кроме передачи файлов по http)
-
-Пример использования [здесь](examples/components_ui.py)
-
-# Текущий прогресс
-## Сеть
-- [x] Интерфейс: WebSocket
-- [ ] Интерфейс: MQTT
-- [ ] Интерфейс: Bluetooth
-- [ ] Интерфейс: Serial
-- [x] Device discovery
-- [ ] Встроенный клиент
-
-## GUI
-- [x] Базовые компоненты
-- [ ] Canvas
-- [ ] Вкладки
-
-## Устройство
-- [x] Базовая информация - название, иконка
-- [x] Расширенная информация - сеть, память
-- [ ] Автоматический сбор расширенной информации
-
-## OTA
-- [x] OTA API
-- [ ] Обновление сервера через OTA
-- [ ] Автообновление
-- [ ] Автоматическая упаковка обновлений
-
-## ФС
-- [x] API файловой системы
-- [ ] Отражение API ФС на реальную папку
-
-## Другие компоненты
-- [ ] Перезапуск сервера по команде reboot
-- [x] CLI API
+
+# Реализация сервера (устройства) GyverHub на python
+
+## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
+
+На данный момент работает только WebSocket
+
+Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
+(кроме передачи файлов по http)
+
+Пример использования [здесь](examples/components_ui.py)
+
+# Текущий прогресс
+## Сеть
+- [x] Интерфейс: WebSocket
+- [ ] Интерфейс: MQTT
+- [ ] Интерфейс: Bluetooth
+- [ ] Интерфейс: Serial
+- [x] Device discovery
+- [ ] Встроенный клиент
+
+## GUI
+- [x] Базовые компоненты
+- [ ] Canvas
+- [ ] Вкладки
+
+## Устройство
+- [x] Базовая информация - название, иконка
+- [x] Расширенная информация - сеть, память
+- [ ] Автоматический сбор расширенной информации
+
+## OTA
+- [x] OTA API
+- [ ] Обновление сервера через OTA
+- [ ] Автообновление
+- [ ] Автоматическая упаковка обновлений
+
+## ФС
+- [x] API файловой системы
+- [ ] Отражение API ФС на реальную папку
+
+## Другие компоненты
+- [ ] Перезапуск сервера по команде reboot
+- [x] CLI API
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/device.py` & `pygyverhubd-0.0.2/gyverhubd/device.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-from functools import cached_property
-
-from . import Filesystem, response, DeviceUi, Module, DeviceInfo
-
-__version__ = "0.0.1"
-
-_FS_COMMANDS = frozenset((
-    "fsbr", "format", "rename", "delete",
-    "fetch", "fetch_chunk",
-    "upload", "upload_chunk"
-))
-
-
-class Device:
-    name: str
-    id: str
-    prefix: str = "MyDevices"
-
-    icon: str = ""
-    pin: int = 0  # TODO
-    version: str = "0.0.1"
-    update_info: str = ""
-    update_format: str = "bin"
-    author: str | None = None
-    enable_auto_update: bool = False
-    info: DeviceInfo | None = None
-    fs: Filesystem | None = None
-    ui: DeviceUi | None = None
-
-    # Overridable
-
-    async def on_focus(self):
-        pass
-
-    async def on_unfocus(self):
-        pass
-
-    async def on_cli(self, command: str):
-        pass
-
-    async def reboot(self):
-        raise NotImplementedError()
-
-    async def ota_update(self, part, url: str | None = None, data: bytes | None = None, check_only: bool = False):
-        raise NotImplementedError()
-
-    async def on_discover(self) -> dict:
-        return dict(name=self.name, icon=self.icon, version=self.update_info, PIN=self.pin, ota_t=self.update_format,
-                    max_upl=0xFFFF_FFFF_FFFF_FFFF, modules=self._disabled_modules)
-
-    # API
-
-    async def send(self, typ, **data):
-        await self.server.send(typ, **data)
-
-    async def broadcast(self, typ, **data):
-        await self.server.broadcast(typ, **data)
-
-    async def send_push(self, text: str, *, broadcast=False):
-        if broadcast:
-            await self.broadcast("push", text=text)
-        else:
-            await self.send("push", text=text)
-
-    async def send_notice(self, text: str, color: int, *, broadcast=False):
-        if broadcast:
-            await self.broadcast("notice", text=text, color=color)
-        else:
-            await self.send("notice", text=text, color=color)
-
-    async def send_alert(self, text: str, *, broadcast=False):
-        if broadcast:
-            await self.broadcast("alert", text=text)
-        else:
-            await self.send("alert", text=text)
-
-    async def send_update(self, name: str, value: str, *, broadcast=False):
-        if broadcast:
-            await self.broadcast("update", updates={name: value})
-        else:
-            await self.send("update", updates={name: value})
-
-    # internal
-
-    @cached_property
-    def _disabled_modules(self):
-        value = 0
-        if self.info is None:
-            value |= Module.INFO
-        if type(self).reboot == Device.reboot:  # not overrided
-            value |= Module.REBOOT
-        if type(self).ota_update == Device.ota_update:  # not overrided
-            value |= Module.OTA | Module.OTA_URL
-        if self.ui is None:
-            value |= Module.SET
-        if self.fs is None:
-            value |= Module.FSBR | Module.FORMAT | Module.RENAME | Module.DELETE | Module.DOWNLOAD | Module.UPLOAD
-        else:
-            fst = type(self.fs)
-            if fst.get_files_info == Filesystem.get_files_info:
-                value |= Module.FSBR
-            if fst.format == Filesystem.format:
-                value |= Module.FORMAT
-            if fst.rename == Filesystem.rename:
-                value |= Module.RENAME
-            if fst.delete == Filesystem.delete:
-                value |= Module.DELETE
-            if fst.get_contents == Filesystem.get_contents:
-                value |= Module.DOWNLOAD
-            if fst.put_contents == Filesystem.put_contents:
-                value |= Module.UPLOAD
-
-        return value
-
-    def __init__(self, server):
-        self.server = server
-        self._ota_data = self._ota_name = None
-
-    async def on_message(self, req, cmd: str, name: str | None):
-        if cmd == "ping":
-            await req.respond(response("OK"))
-            return
-
-        # # UI # #
-
-        if cmd == "focus":
-            req.set_focused(True)
-            await self.on_focus()
-            if self.ui is None:
-                await req.respond(response("ui", controls=[]))
-            else:
-                await req.respond(await self.ui.on_update())
-            return
-
-        if cmd == "unfocus":
-            req.set_focused(False)
-            await self.on_unfocus()
-            return
-
-        if cmd == "set":
-            if self.ui is None:
-                await req.respond(response("OK"))
-            else:
-                await req.respond(await self.ui.on_ui_event(name, req.value))
-            return
-
-        # # INFO # #
-
-        if cmd == "info":
-            if self.info is None:
-                info = dict(versions=dict())
-            else:
-                info = self.info.to_json()
-
-            info = dict(info)
-            info['version'] = dict(info.get('version', {}))
-            info['version']['Library'] = __version__
-            if self.version:
-                info['version'].setdefault('Firmware', self.version)
-
-            await req.respond(response("info", info=info))
-            return
-
-        if cmd == "reboot":
-            await self.reboot()
-            await req.respond(response("OK"))
-            return
-
-        if cmd == "cli":
-            await self.on_cli(req.value)
-            await req.respond(response("OK"))
-            return
-
-        # # FILESYSTEM # #
-
-        if cmd in _FS_COMMANDS:
-            if self.fs is None:
-                await req.respond(response("fs_error"))
-            else:
-                await req.respond(await self.fs.on_message(req, cmd, name))
-            return
-
-        # # OTA # #
-
-        if cmd == "ota_url":
-            try:
-                await self.ota_update(name, url=req.value)
-            except Exception:
-                await req.respond(response("ota_url_err"))
-            else:
-                await req.respond(response("ota_url_ok"))
-            return
-
-        if cmd == "ota":
-            try:
-                await self.ota_update(name, check_only=True)
-            except Exception:
-                await req.respond(response("ota_err"))
-            else:
-                self._ota_name = name
-                self._ota_data = []
-                await req.respond(response("ota_start"))
-            return
-
-        if cmd == "ota_chunk":
-            if self._ota_data is None:
-                await req.respond(response("ota_err"))
-                return
-
-            self._ota_data.append(req.value)
-
-            if name == 'next':
-                await req.respond(response("ota_next_chunk"))
-                return
-
-            try:
-                await self.ota_update(self._ota_name, data=b''.join(self._ota_data))
-            except Exception:
-                await req.respond(response("ota_err"))
-            else:
-                self._ota_name = self._ota_data = None
-                await req.respond(response("ota_end"))
-            return
+from functools import cached_property
+
+from . import Filesystem, response, DeviceUi, Module, DeviceInfo
+from ._version import __version__
+
+
+_FS_COMMANDS = frozenset((
+    "fsbr", "format", "rename", "delete",
+    "fetch", "fetch_chunk",
+    "upload", "upload_chunk"
+))
+
+
+class Device:
+    name: str
+    id: str
+    prefix: str = "MyDevices"
+
+    icon: str = ""
+    pin: int = 0  # TODO
+    version: str = "0.0.1"
+    update_info: str = ""
+    update_format: str = "bin"
+    author: str | None = None
+    enable_auto_update: bool = False
+    info: DeviceInfo | None = None
+    fs: Filesystem | None = None
+    ui: DeviceUi | None = None
+
+    # Overridable
+
+    async def on_focus(self):
+        pass
+
+    async def on_unfocus(self):
+        pass
+
+    async def on_cli(self, command: str):
+        pass
+
+    async def reboot(self):
+        raise NotImplementedError()
+
+    async def ota_update(self, part, url: str | None = None, data: bytes | None = None, check_only: bool = False):
+        raise NotImplementedError()
+
+    async def on_discover(self) -> dict:
+        return dict(name=self.name, icon=self.icon, version=self.update_info, PIN=self.pin, ota_t=self.update_format,
+                    max_upl=0xFFFF_FFFF_FFFF_FFFF, modules=self._disabled_modules)
+
+    # API
+
+    async def send(self, typ, **data):
+        await self.server.send(typ, **data)
+
+    async def broadcast(self, typ, **data):
+        await self.server.broadcast(typ, **data)
+
+    async def send_push(self, text: str, *, broadcast=False):
+        if broadcast:
+            await self.broadcast("push", text=text)
+        else:
+            await self.send("push", text=text)
+
+    async def send_notice(self, text: str, color: int, *, broadcast=False):
+        if broadcast:
+            await self.broadcast("notice", text=text, color=color)
+        else:
+            await self.send("notice", text=text, color=color)
+
+    async def send_alert(self, text: str, *, broadcast=False):
+        if broadcast:
+            await self.broadcast("alert", text=text)
+        else:
+            await self.send("alert", text=text)
+
+    async def send_update(self, name: str, value: str, *, broadcast=False):
+        if broadcast:
+            await self.broadcast("update", updates={name: value})
+        else:
+            await self.send("update", updates={name: value})
+
+    # internal
+
+    @cached_property
+    def _disabled_modules(self):
+        value = 0
+        if self.info is None:
+            value |= Module.INFO
+        if type(self).reboot == Device.reboot:  # not overrided
+            value |= Module.REBOOT
+        if type(self).ota_update == Device.ota_update:  # not overrided
+            value |= Module.OTA | Module.OTA_URL
+        if self.ui is None:
+            value |= Module.SET
+        if self.fs is None:
+            value |= Module.FSBR | Module.FORMAT | Module.RENAME | Module.DELETE | Module.DOWNLOAD | Module.UPLOAD
+        else:
+            fst = type(self.fs)
+            if fst.get_files_info == Filesystem.get_files_info:
+                value |= Module.FSBR
+            if fst.format == Filesystem.format:
+                value |= Module.FORMAT
+            if fst.rename == Filesystem.rename:
+                value |= Module.RENAME
+            if fst.delete == Filesystem.delete:
+                value |= Module.DELETE
+            if fst.get_contents == Filesystem.get_contents:
+                value |= Module.DOWNLOAD
+            if fst.put_contents == Filesystem.put_contents:
+                value |= Module.UPLOAD
+
+        return value
+
+    def __init__(self, server):
+        self.server = server
+        self._ota_data = self._ota_name = None
+
+    async def on_message(self, req, cmd: str, name: str | None):
+        if cmd == "ping":
+            await req.respond(response("OK"))
+            return
+
+        # # UI # #
+
+        if cmd == "focus":
+            req.set_focused(True)
+            await self.on_focus()
+            if self.ui is None:
+                await req.respond(response("ui", controls=[]))
+            else:
+                await req.respond(await self.ui.on_update())
+            return
+
+        if cmd == "unfocus":
+            req.set_focused(False)
+            await self.on_unfocus()
+            return
+
+        if cmd == "set":
+            if self.ui is None:
+                await req.respond(response("OK"))
+            else:
+                await req.respond(await self.ui.on_ui_event(name, req.value))
+            return
+
+        # # INFO # #
+
+        if cmd == "info":
+            if self.info is None:
+                info = dict(versions=dict())
+            else:
+                info = self.info.to_json()
+
+            info = dict(info)
+            info['version'] = dict(info.get('version', {}))
+            info['version']['Library'] = __version__
+            if self.version:
+                info['version'].setdefault('Firmware', self.version)
+
+            await req.respond(response("info", info=info))
+            return
+
+        if cmd == "reboot":
+            await self.reboot()
+            await req.respond(response("OK"))
+            return
+
+        if cmd == "cli":
+            await self.on_cli(req.value)
+            await req.respond(response("OK"))
+            return
+
+        # # FILESYSTEM # #
+
+        if cmd in _FS_COMMANDS:
+            if self.fs is None:
+                await req.respond(response("fs_error"))
+            else:
+                await req.respond(await self.fs.on_message(req, cmd, name))
+            return
+
+        # # OTA # #
+
+        if cmd == "ota_url":
+            try:
+                await self.ota_update(name, url=req.value)
+            except Exception:
+                await req.respond(response("ota_url_err"))
+            else:
+                await req.respond(response("ota_url_ok"))
+            return
+
+        if cmd == "ota":
+            try:
+                await self.ota_update(name, check_only=True)
+            except Exception:
+                await req.respond(response("ota_err"))
+            else:
+                self._ota_name = name
+                self._ota_data = []
+                await req.respond(response("ota_start"))
+            return
+
+        if cmd == "ota_chunk":
+            if self._ota_data is None:
+                await req.respond(response("ota_err"))
+                return
+
+            self._ota_data.append(req.value)
+
+            if name == 'next':
+                await req.respond(response("ota_next_chunk"))
+                return
+
+            try:
+                await self.ota_update(self._ota_name, data=b''.join(self._ota_data))
+            except Exception:
+                await req.respond(response("ota_err"))
+            else:
+                self._ota_name = self._ota_data = None
+                await req.respond(response("ota_end"))
+            return
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/info.py` & `pygyverhubd-0.0.2/gyverhubd/info.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import collections
-import datetime
-import typing
-
-
-class DeviceInfo:
-    __slots__ = ('_data', '_handlers', '_device')
-
-    def __init__(self):
-        self._data = dict(version={}, net={}, memory={}, system={})
-        self._handlers = collections.defaultdict(list)
-        self._device = None
-
-    def __get__(self, instance, owner=None):
-        if self._device is None:
-            obj = type(self)
-            obj._data = self._data
-            obj._handlers = self._handlers
-            obj._device = instance
-            return obj
-        return self
-
-    def to_json(self) -> dict[str, dict]:
-        data = dict(self._data)
-        for group, handlers in self._handlers.items():
-            for handler in handlers:
-                data[group].update(handler(self._device))
-        return data
-
-    def set(self, group: str, name: str, value: str) -> typing.Self:
-        self._data[group][name] = value
-        return self
-
-    def version(self, name: str, value: str) -> typing.Self:
-        return self.set('version', name, value)
-
-    def system(self, name: str, value: str) -> typing.Self:
-        return self.set('system', name, value)
-
-    def network(self, name: str, value: str) -> typing.Self:
-        return self.set('net', name, value)
-
-    def memory(self, name: str, value: str | int, total: int | None = None) -> typing.Self:
-        if isinstance(value, (tuple, list)) and total is None:
-            value, total = value
-        if isinstance(value, int):
-            if total is None:
-                total = 0
-            value = [value, total]
-        else:
-            if total is not None:
-                raise TypeError("Argument 'total' must not be set when value is str!")
-        return self.set('memory', name, value)
-
-    def uptime(self, value: datetime.timedelta) -> typing.Self:
-        return self.set('system', 'Uptime', value.seconds)
-
-    def set_handler(self, group: str, fn: callable):
-        self._handlers[group].append(fn)
-
-    def handler(self, group: str):
-        def _decorator(fn):
-            self.set_handler(group, fn)
-            return fn
-        return _decorator
-
-    # version: dict[str, str] = dataclasses.field(default_factory=dict)  # Library, Firmware
-    # net: dict[str, str] = dataclasses.field(default_factory=dict)  # Mode, MAC, SSID, RSSI, IP
-    # memory: dict[str, tuple[int, int] | str] = dataclasses.field(default_factory=dict)  # RAM Flash Sketch
-    # system: dict[str, str] = dataclasses.field(default_factory=dict)  # Uptime (int), Model, CPU_Mhz Flash_chip
+import collections
+import datetime
+import typing
+
+
+class DeviceInfo:
+    __slots__ = ('_data', '_handlers', '_device')
+
+    def __init__(self):
+        self._data = dict(version={}, net={}, memory={}, system={})
+        self._handlers = collections.defaultdict(list)
+        self._device = None
+
+    def __get__(self, instance, owner=None):
+        if self._device is None:
+            obj = type(self)
+            obj._data = self._data
+            obj._handlers = self._handlers
+            obj._device = instance
+            return obj
+        return self
+
+    def to_json(self) -> dict[str, dict]:
+        data = dict(self._data)
+        for group, handlers in self._handlers.items():
+            for handler in handlers:
+                data[group].update(handler(self._device))
+        return data
+
+    def set(self, group: str, name: str, value: str) -> typing.Self:
+        self._data[group][name] = value
+        return self
+
+    def version(self, name: str, value: str) -> typing.Self:
+        return self.set('version', name, value)
+
+    def system(self, name: str, value: str) -> typing.Self:
+        return self.set('system', name, value)
+
+    def network(self, name: str, value: str) -> typing.Self:
+        return self.set('net', name, value)
+
+    def memory(self, name: str, value: str | int, total: int | None = None) -> typing.Self:
+        if isinstance(value, (tuple, list)) and total is None:
+            value, total = value
+        if isinstance(value, int):
+            if total is None:
+                total = 0
+            value = [value, total]
+        else:
+            if total is not None:
+                raise TypeError("Argument 'total' must not be set when value is str!")
+        return self.set('memory', name, value)
+
+    def uptime(self, value: datetime.timedelta) -> typing.Self:
+        return self.set('system', 'Uptime', value.seconds)
+
+    def set_handler(self, group: str, fn: callable):
+        self._handlers[group].append(fn)
+
+    def handler(self, group: str):
+        def _decorator(fn):
+            self.set_handler(group, fn)
+            return fn
+        return _decorator
+
+    # version: dict[str, str] = dataclasses.field(default_factory=dict)  # Library, Firmware
+    # net: dict[str, str] = dataclasses.field(default_factory=dict)  # Mode, MAC, SSID, RSSI, IP
+    # memory: dict[str, tuple[int, int] | str] = dataclasses.field(default_factory=dict)  # RAM Flash Sketch
+    # system: dict[str, str] = dataclasses.field(default_factory=dict)  # Uptime (int), Model, CPU_Mhz Flash_chip
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/proto/proto.py` & `pygyverhubd-0.0.2/gyverhubd/proto/proto.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import typing
-
-
-MessageHandler = typing.Callable[['Request'], None]
-
-
-class Protocol:
-    focused: bool = False
-    device_id: str | None = None
-
-    def set_handler_message(self, handler: MessageHandler):
-        raise NotImplementedError()
-
-    async def send(self, data: str):
-        raise NotImplementedError()
-
-    async def start(self):
-        raise NotImplementedError()
-
-    async def stop(self):
-        raise NotImplementedError()
-
-
-class Request:
-    url: str
-    value: str | None
-    protocol: Protocol
-
-    async def respond(self, data: str):
-        raise NotImplementedError()
-
-    def set_focused(self, value: bool):
-        raise NotImplementedError()
+import typing
+
+
+MessageHandler = typing.Callable[['Request'], None]
+
+
+class Protocol:
+    focused: bool = False
+    device_id: str | None = None
+
+    def set_handler_message(self, handler: MessageHandler):
+        raise NotImplementedError()
+
+    async def send(self, data: str):
+        raise NotImplementedError()
+
+    async def start(self):
+        raise NotImplementedError()
+
+    async def stop(self):
+        raise NotImplementedError()
+
+
+class Request:
+    url: str
+    value: str | None
+    protocol: Protocol
+
+    async def respond(self, data: str):
+        raise NotImplementedError()
+
+    def set_focused(self, value: bool):
+        raise NotImplementedError()
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/server.py` & `pygyverhubd-0.0.2/gyverhubd/server.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import asyncio
-import json
-
-from . import Device, Protocol, Request, parse_url
-
-
-class Server:
-    def __init__(self, device: type[Device], *, protocols: list[Protocol] = ()):
-        self._protocols: list[Protocol] = []
-        self.device = device(self)
-
-        for i in protocols:
-            self.add_protocol(i)
-
-    def add_protocol(self, proto: Protocol):
-        self._protocols.append(proto)
-        proto.set_handler_message(self._on_message)
-        proto.device_id = self.device.id
-
-    async def start(self):
-        for i in self._protocols:
-            await i.start()
-
-    async def stop(self):
-        for i in self._protocols:
-            await i.stop()
-
-    def _on_message(self, req: Request):
-        asyncio.ensure_future(self._on_message_async(req))
-
-    async def _on_message_async(self, req: Request):
-        prefix, clid, did, cmd, name = parse_url(req.url)
-
-        if self.device.prefix != prefix:
-            return
-
-        print(f">>> {cmd!r} {name!r}={req.value!r}")
-
-        dev = self.device
-        if cmd is None:
-            if did is None or dev.id == did:
-                data = await dev.on_discover()
-                if data is not None:
-                    data['type'] = 'discover'
-                    asyncio.ensure_future(req.respond(data))
-            return
-
-        if did == dev.id:
-            await dev.on_message(req, cmd, name)
-
-    async def send(self, typ, **data):
-        print(f"<<< {typ} {data}")
-        data['type'] = typ
-
-        for i in self._protocols:
-            if i.focused:
-                await i.send(data)
-
-    async def broadcast(self, typ, **data):
-        print(f"<<< {typ} {data}")
-        data['type'] = typ
-
-        for i in self._protocols:
-            await i.send(data)
-
-
-async def run_server_async(*args, **kwargs):
-    server = Server(*args, **kwargs)
-    await server.start()
-    try:
-        await asyncio.Future()
-    finally:
-        await server.stop()
-
-
-def run_server(*args, **kwargs):
-    asyncio.run(run_server_async(*args, **kwargs))
+import asyncio
+import json
+
+from . import Device, Protocol, Request, parse_url
+
+
+class Server:
+    def __init__(self, device: type[Device], *, protocols: list[Protocol] = ()):
+        self._protocols: list[Protocol] = []
+        self.device = device(self)
+
+        for i in protocols:
+            self.add_protocol(i)
+
+    def add_protocol(self, proto: Protocol):
+        self._protocols.append(proto)
+        proto.set_handler_message(self._on_message)
+        proto.device_id = self.device.id
+
+    async def start(self):
+        for i in self._protocols:
+            await i.start()
+
+    async def stop(self):
+        for i in self._protocols:
+            await i.stop()
+
+    def _on_message(self, req: Request):
+        asyncio.ensure_future(self._on_message_async(req))
+
+    async def _on_message_async(self, req: Request):
+        prefix, clid, did, cmd, name = parse_url(req.url)
+
+        if self.device.prefix != prefix:
+            return
+
+        print(f">>> {cmd!r} {name!r}={req.value!r}")
+
+        dev = self.device
+        if cmd is None:
+            if did is None or dev.id == did:
+                data = await dev.on_discover()
+                if data is not None:
+                    data['type'] = 'discover'
+                    asyncio.ensure_future(req.respond(data))
+            return
+
+        if did == dev.id:
+            await dev.on_message(req, cmd, name)
+
+    async def send(self, typ, **data):
+        print(f"<<< {typ} {data}")
+        data['type'] = typ
+
+        for i in self._protocols:
+            if i.focused:
+                await i.send(data)
+
+    async def broadcast(self, typ, **data):
+        print(f"<<< {typ} {data}")
+        data['type'] = typ
+
+        for i in self._protocols:
+            await i.send(data)
+
+
+async def run_server_async(*args, **kwargs):
+    server = Server(*args, **kwargs)
+    await server.start()
+    try:
+        await asyncio.Future()
+    finally:
+        await server.stop()
+
+
+def run_server(*args, **kwargs):
+    asyncio.run(run_server_async(*args, **kwargs))
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/ui/builder.py` & `pygyverhubd-0.0.2/gyverhubd/ui/builder.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-import enum
-import itertools
-
-from gyverhubd import Color, response
-from . import DeviceUi
-
-
-class BuildType(enum.Enum):
-    LAYOUT = enum.auto()
-    ACTION = enum.auto()
-
-
-class Builder:
-    def __init__(self, components, name=None, value=None):
-        self._build_type = BuildType.LAYOUT if name is None else BuildType.ACTION
-        self._component_name = name
-        self._value = value
-
-        self._components = components
-        self._new_name = (f"u{i}" for i in itertools.count())
-
-    def _ensure_name(self, name: str | None) -> str:
-        if name is None:
-            return next(self._new_name)
-        return name
-
-    def button(self, label, size: int = 12, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="button", name=name, label=label, size=size, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value == '1'
-
-    def button_icon(self, label, size: int = 12, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="button_i", name=name, label=label, size=size, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value == '1'
-
-    def label(self, label, value: str = "", size: int = 12, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="label", name=name, value=value, label=label, size=size, color=color, tab_w=tab_w))
-
-    def title(self, label):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="title", label=label))
-
-    def log(self, text: str, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="log", name=name, text=text, tab_w=tab_w))
-
-    def display(self, value, rows: int = 1, size: int = 12, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="display", value=value, name=name, rows=rows, size=size, color=color, tab_w=tab_w))
-
-    def html(self, value, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="html", value=value, name=name, tab_w=tab_w))
-
-    def js(self, value):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="js", value=value))
-
-    def input(self, label, value: str = "", regex: str = "", max: int | None = None, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="input", name=name, value=value, regex=regex, label=label, max=max,
-                                         color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def password(self, label, value: str = "", regex: str = "", max: int | None = None, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="pass", name=name, value=value, regex=regex, label=label, max=max,
-                                         color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def spinner(self, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="spinner", name=name, label=label, value=value, min=min, max=max, step=step,
-                                         color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def slider(self, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="slider", name=name, label=label, value=value, min=min, max=max, step=step,
-                                         color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def gauge(self, text, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="gauge", name=name, text=text, label=label, value=value, min=min, max=max, step=step,
-                                         color=color, tab_w=tab_w))
-
-    def switch(self, label, value: bool = True, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="switch", name=name, label=label, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def switch_icon(self, label, text, value: bool = True, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="switch_i", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def switch_text(self, label, text, value: bool=True, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="switch_t", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def date(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="date", name=name, label=label, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def time(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="time", name=name, label=label, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def datetime(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="datetime", name=name, label=label, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def select(self, label, text, value: int = 0, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="select", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def flags(self, label, text, value: int = 0, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="flags", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def color(self, label, value: int = 0, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="color", name=name, label=label, value=value, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def led(self, label, text="", value: bool = False, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="led", name=name, label=label, text=text, value=value, tab_w=tab_w))
-
-    def spacer(self, height: int, tab_w=None):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="spacer", height=height, tab_w=tab_w))
-
-    def stream(self, height: int, tab_w=None):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="stream", height=height, tab_w=tab_w))
-
-    def image(self, label, prd: str, value: str, tab_w=None):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="image", label=label, prd=prd, value=value, tab_w=tab_w))
-
-    def joystick(self, label, auto: bool = False, exp: bool = False, color: Color | None = None, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="joy", name=name, label=label, auto=auto, exp=exp, color=color, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def tabs(self, label, value: str, text: str, tab_w=None, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="tabs", name=name, label=label, value=value, text=text, tab_w=tab_w))
-        elif self._component_name == name:
-            return self._value
-
-    def menu(self, label, value: str, text: str, tab_w=None):
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="menu", name="_menu", label=label, value=value, text=text, tab_w=tab_w))
-        elif self._component_name == "_menu":
-            return self._value
-
-    def canvas(self, label, width: int = 100, height: int = 100, active: bool = True, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="canvas", name=name, label=label, width=width, height=height, active=active, value=[]))
-        elif self._component_name == name:
-            return self._value
-
-    def confirm(self, label, name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="confirm", name=name, label=label))
-        elif self._component_name == name:
-            return self._value
-
-    def prompt(self, label, value: str = "", name=None):
-        name = self._ensure_name(name)
-        if self._build_type == BuildType.LAYOUT:
-            self._components.append(dict(type="prompt", name=name, label=label, value=value))
-        elif self._component_name == name:
-            return self._value
-
-
-class BuilderUiWrapper(DeviceUi):
-    def __init__(self, fn, device=None):
-        self._fn = fn
-        self._device = device
-
-    def __get__(self, instance, owner=None):
-        if self._device is None:
-            return type(self)(self._fn, instance)
-        return self
-
-    async def build_ui(self, builder: Builder):
-        return await self._fn(self._device, builder)
-
-    async def on_update(self):
-        components = []
-        builder = Builder(components)
-        await self.build_ui(builder)
-        return response("ui", controls=components)
-
-    async def on_ui_event(self, name: str, value: str):
-        builder = Builder([], name, value)
-        await self.build_ui(builder)
-        return await self.on_update()
-
-
-ui_builder = BuilderUiWrapper
+import enum
+import itertools
+
+from gyverhubd import Color, response
+from . import DeviceUi
+
+
+class BuildType(enum.Enum):
+    LAYOUT = enum.auto()
+    ACTION = enum.auto()
+
+
+class Builder:
+    def __init__(self, components, name=None, value=None):
+        self._build_type = BuildType.LAYOUT if name is None else BuildType.ACTION
+        self._component_name = name
+        self._value = value
+
+        self._components = components
+        self._new_name = (f"u{i}" for i in itertools.count())
+
+    def _ensure_name(self, name: str | None) -> str:
+        if name is None:
+            return next(self._new_name)
+        return name
+
+    def button(self, label, size: int = 12, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="button", name=name, label=label, size=size, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value == '1'
+
+    def button_icon(self, label, size: int = 12, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="button_i", name=name, label=label, size=size, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value == '1'
+
+    def label(self, label, value: str = "", size: int = 12, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="label", name=name, value=value, label=label, size=size, color=color, tab_w=tab_w))
+
+    def title(self, label):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="title", label=label))
+
+    def log(self, text: str, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="log", name=name, text=text, tab_w=tab_w))
+
+    def display(self, value, rows: int = 1, size: int = 12, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="display", value=value, name=name, rows=rows, size=size, color=color, tab_w=tab_w))
+
+    def html(self, value, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="html", value=value, name=name, tab_w=tab_w))
+
+    def js(self, value):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="js", value=value))
+
+    def input(self, label, value: str = "", regex: str = "", max: int | None = None, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="input", name=name, value=value, regex=regex, label=label, max=max,
+                                         color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def password(self, label, value: str = "", regex: str = "", max: int | None = None, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="pass", name=name, value=value, regex=regex, label=label, max=max,
+                                         color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def spinner(self, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="spinner", name=name, label=label, value=value, min=min, max=max, step=step,
+                                         color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def slider(self, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="slider", name=name, label=label, value=value, min=min, max=max, step=step,
+                                         color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def gauge(self, text, label, value: int = 0, min: int = 0, max: int = 100, step: int = 1, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="gauge", name=name, text=text, label=label, value=value, min=min, max=max, step=step,
+                                         color=color, tab_w=tab_w))
+
+    def switch(self, label, value: bool = True, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="switch", name=name, label=label, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def switch_icon(self, label, text, value: bool = True, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="switch_i", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def switch_text(self, label, text, value: bool=True, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="switch_t", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def date(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="date", name=name, label=label, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def time(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="time", name=name, label=label, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def datetime(self, label, value: int = 0, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="datetime", name=name, label=label, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def select(self, label, text, value: int = 0, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="select", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def flags(self, label, text, value: int = 0, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="flags", name=name, label=label, text=text, value=value, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def color(self, label, value: int = 0, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="color", name=name, label=label, value=value, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def led(self, label, text="", value: bool = False, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="led", name=name, label=label, text=text, value=value, tab_w=tab_w))
+
+    def spacer(self, height: int, tab_w=None):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="spacer", height=height, tab_w=tab_w))
+
+    def stream(self, height: int, tab_w=None):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="stream", height=height, tab_w=tab_w))
+
+    def image(self, label, prd: str, value: str, tab_w=None):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="image", label=label, prd=prd, value=value, tab_w=tab_w))
+
+    def joystick(self, label, auto: bool = False, exp: bool = False, color: Color | None = None, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="joy", name=name, label=label, auto=auto, exp=exp, color=color, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def tabs(self, label, value: str, text: str, tab_w=None, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="tabs", name=name, label=label, value=value, text=text, tab_w=tab_w))
+        elif self._component_name == name:
+            return self._value
+
+    def menu(self, label, value: str, text: str, tab_w=None):
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="menu", name="_menu", label=label, value=value, text=text, tab_w=tab_w))
+        elif self._component_name == "_menu":
+            return self._value
+
+    def canvas(self, label, width: int = 100, height: int = 100, active: bool = True, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="canvas", name=name, label=label, width=width, height=height, active=active, value=[]))
+        elif self._component_name == name:
+            return self._value
+
+    def confirm(self, label, name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="confirm", name=name, label=label))
+        elif self._component_name == name:
+            return self._value
+
+    def prompt(self, label, value: str = "", name=None):
+        name = self._ensure_name(name)
+        if self._build_type == BuildType.LAYOUT:
+            self._components.append(dict(type="prompt", name=name, label=label, value=value))
+        elif self._component_name == name:
+            return self._value
+
+
+class BuilderUiWrapper(DeviceUi):
+    def __init__(self, fn, device=None):
+        self._fn = fn
+        self._device = device
+
+    def __get__(self, instance, owner=None):
+        if self._device is None:
+            return type(self)(self._fn, instance)
+        return self
+
+    async def build_ui(self, builder: Builder):
+        return await self._fn(self._device, builder)
+
+    async def on_update(self):
+        components = []
+        builder = Builder(components)
+        await self.build_ui(builder)
+        return response("ui", controls=components)
+
+    async def on_ui_event(self, name: str, value: str):
+        builder = Builder([], name, value)
+        await self.build_ui(builder)
+        return await self.on_update()
+
+
+ui_builder = BuilderUiWrapper
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/ui/components/datetime.py` & `pygyverhubd-0.0.2/gyverhubd/ui/components/datetime.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import datetime
-import time
-
-from gyverhubd import Component
-
-
-class DateTimeBase(Component):
-    __fields__ = (
-        ('value', 'value', 0),
-        ('color', 'color', None),
-    )
-
-
-class Date(DateTimeBase):
-    __value_field__ = ('value', 'value', datetime.date.today())
-    __type__ = "date"
-
-    def value2event(self, value: datetime.date):
-        return time.mktime(value.timetuple())
-
-    def event2value(self, value):
-        value = int(value)
-        return datetime.date.fromtimestamp(value)
-
-
-class Time(DateTimeBase):
-    __value_field__ = ('value', 'value', datetime.datetime.now().time())
-    __type__ = "time"
-
-    def value2event(self, value: datetime.time):
-        return value.hour * 3600 + value.minute * 60 + value.second
-
-    def event2value(self, value):
-        value = int(value)
-        return datetime.time(value // 3600, (value // 60) % 60, value % 60)
-
-
-class DateTime(DateTimeBase):
-    __value_field__ = ('value', 'value', datetime.datetime.now())
-    __type__ = "datetime"
-
-    def value2event(self, value: datetime.datetime):
-        return value.timestamp()
-
-    def event2value(self, value):
-        value = int(value)
-        return datetime.datetime.fromtimestamp(value)
-
+import datetime
+import time
+
+from gyverhubd import Component
+
+
+class DateTimeBase(Component):
+    __fields__ = (
+        ('value', 'value', 0),
+        ('color', 'color', None),
+    )
+
+
+class Date(DateTimeBase):
+    __value_field__ = ('value', 'value', datetime.date.today())
+    __type__ = "date"
+
+    def value2event(self, value: datetime.date):
+        return time.mktime(value.timetuple())
+
+    def event2value(self, value):
+        value = int(value)
+        return datetime.date.fromtimestamp(value)
+
+
+class Time(DateTimeBase):
+    __value_field__ = ('value', 'value', datetime.datetime.now().time())
+    __type__ = "time"
+
+    def value2event(self, value: datetime.time):
+        return value.hour * 3600 + value.minute * 60 + value.second
+
+    def event2value(self, value):
+        value = int(value)
+        return datetime.time(value // 3600, (value // 60) % 60, value % 60)
+
+
+class DateTime(DateTimeBase):
+    __value_field__ = ('value', 'value', datetime.datetime.now())
+    __type__ = "datetime"
+
+    def value2event(self, value: datetime.datetime):
+        return value.timestamp()
+
+    def event2value(self, value):
+        value = int(value)
+        return datetime.datetime.fromtimestamp(value)
+
```

### Comparing `pygyverhubd-0.0.1/gyverhubd/utils.py` & `pygyverhubd-0.0.2/gyverhubd/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import enum
-import typing
-
-
-class Module(enum.IntFlag):
-    INFO = 1 << 0
-    FSBR = 1 << 1
-    FORMAT = 1 << 2
-
-    DOWNLOAD = 1 << 3
-    UPLOAD = 1 << 4
-
-    OTA = 1 << 5
-    OTA_URL = 1 << 6
-
-    REBOOT = 1 << 7
-
-    SET = 1 << 8
-    READ = 1 << 9
-
-    DELETE = 1 << 10
-    RENAME = 1 << 11
-
-    SERIAL = 1 << 12
-    BT = 1 << 13
-    WS = 1 << 14
-    MQTT = 1 << 15
-
-
-class Color(int):
-    __slots__ = ()
-
-    @classmethod
-    def from_hex(cls, value: int) -> typing.Self:
-        return cls(value)
-
-    @classmethod
-    def from_grayscale(cls, value: int) -> typing.Self:
-        return cls.from_rgb(value, value, value)
-
-    @classmethod
-    def from_rgb(cls, r: int, g: int, b: int) -> typing.Self:
-        return cls((r << 16) | (g << 8) | (b << 0))
-
-    @classmethod
-    def from_rgbf(cls, r: float, g: float, b: float) -> typing.Self:
-        return cls.from_rgb(int(r * 255), int(g * 255), int(b * 255))
-
-    @classmethod
-    def from_hsvf(cls, h: float, s: float, v: float) -> typing.Self:
-        i, f = divmod(h * 6, 1)
-        p = v * (1 - s)
-
-        match int(i):
-            case 0:
-                t = v * (1 - (1 - f) * s)
-                r, g, b = v, t, p
-            case 1:
-                q = v * (1 - f * s)
-                r, g, b = q, v, p
-            case 2:
-                t = v * (1 - (1 - f) * s)
-                r, g, b = p, v, t
-            case 3:
-                q = v * (1 - f * s)
-                r, g, b = p, q, v
-            case 4:
-                t = v * (1 - (1 - f) * s)
-                r, g, b = t, p, v
-            case 5:
-                q = v * (1 - f * s)
-                r, g, b = v, p, q
-            case _:
-                assert False
-
-        return cls.from_rgbf(r, g, b)
-
-    @classmethod
-    def from_hsv(cls, h: int, s: int, v: int) -> typing.Self:
-        return cls.from_hsvf(h // 255, s // 255, v // 255)
-
-    @classmethod
-    def from_hue(cls, color: int):
-        if color > 170:
-            shift = (color - 170) * 3
-            return cls.from_rgb(shift, 0, 255 - shift)
-        elif color > 85:
-            shift = (color - 85) * 3
-            return cls.from_rgb(0, 255 - shift, shift)
-        else:
-            shift = color * 3
-            return cls.from_rgb(255 - shift, shift, 0)
-
-    RED: typing.ClassVar['Color']
-    ORANGE: typing.ClassVar['Color']
-    YELLOW: typing.ClassVar['Color']
-    GREEN: typing.ClassVar['Color']
-    MINT: typing.ClassVar['Color']
-    AQUA: typing.ClassVar['Color']
-    BLUE: typing.ClassVar['Color']
-    VIOLET: typing.ClassVar['Color']
-    PINK: typing.ClassVar['Color']
-    DEFAULT: typing.ClassVar['Color']
-
-
-for _k, _v in dict(RED=0xcb2839, ORANGE=0xd55f30, YELLOW=0xd69d27, GREEN=0x37A93C, MINT=0x25b18f, AQUA=0x2ba1cd,
-                   BLUE=0x297bcd, VIOLET=0x825ae7, PINK=0xc8589a, DEFAULT=0xffffffff).items():
-    setattr(Color, _k, Color.from_hex(_v))
-del _k
-del _v
-
-
-def parse_url(url: str) -> tuple[str, str | None, str | None, str | None, str | None]:
-    prefix, *url = url.split('/', maxsplit=4)
-    cmd = clid = did = name = None
-
-    if url:
-        did, *url = url
-    if len(url) == 1:
-        print(prefix, url)
-        raise ValueError("Invalid data!")
-        # return prefix, clid, did, cmd, name
-    if url:
-        clid, cmd, *url = url
-    if url:
-        name, = url
-    return prefix, clid, did, cmd, name
-
-
-def generate_did():
-    raise ValueError("Missing did and generating not supported!")
-
-
-def response(typ: str, **kwargs):
-    kwargs['type'] = typ
-    return kwargs
+import enum
+import typing
+
+
+class Module(enum.IntFlag):
+    INFO = 1 << 0
+    FSBR = 1 << 1
+    FORMAT = 1 << 2
+
+    DOWNLOAD = 1 << 3
+    UPLOAD = 1 << 4
+
+    OTA = 1 << 5
+    OTA_URL = 1 << 6
+
+    REBOOT = 1 << 7
+
+    SET = 1 << 8
+    READ = 1 << 9
+
+    DELETE = 1 << 10
+    RENAME = 1 << 11
+
+    SERIAL = 1 << 12
+    BT = 1 << 13
+    WS = 1 << 14
+    MQTT = 1 << 15
+
+
+class Color(int):
+    __slots__ = ()
+
+    @classmethod
+    def from_hex(cls, value: int) -> typing.Self:
+        return cls(value)
+
+    @classmethod
+    def from_grayscale(cls, value: int) -> typing.Self:
+        return cls.from_rgb(value, value, value)
+
+    @classmethod
+    def from_rgb(cls, r: int, g: int, b: int) -> typing.Self:
+        return cls((r << 16) | (g << 8) | (b << 0))
+
+    @classmethod
+    def from_rgbf(cls, r: float, g: float, b: float) -> typing.Self:
+        return cls.from_rgb(int(r * 255), int(g * 255), int(b * 255))
+
+    @classmethod
+    def from_hsvf(cls, h: float, s: float, v: float) -> typing.Self:
+        i, f = divmod(h * 6, 1)
+        p = v * (1 - s)
+
+        match int(i):
+            case 0:
+                t = v * (1 - (1 - f) * s)
+                r, g, b = v, t, p
+            case 1:
+                q = v * (1 - f * s)
+                r, g, b = q, v, p
+            case 2:
+                t = v * (1 - (1 - f) * s)
+                r, g, b = p, v, t
+            case 3:
+                q = v * (1 - f * s)
+                r, g, b = p, q, v
+            case 4:
+                t = v * (1 - (1 - f) * s)
+                r, g, b = t, p, v
+            case 5:
+                q = v * (1 - f * s)
+                r, g, b = v, p, q
+            case _:
+                assert False
+
+        return cls.from_rgbf(r, g, b)
+
+    @classmethod
+    def from_hsv(cls, h: int, s: int, v: int) -> typing.Self:
+        return cls.from_hsvf(h // 255, s // 255, v // 255)
+
+    @classmethod
+    def from_hue(cls, color: int):
+        if color > 170:
+            shift = (color - 170) * 3
+            return cls.from_rgb(shift, 0, 255 - shift)
+        elif color > 85:
+            shift = (color - 85) * 3
+            return cls.from_rgb(0, 255 - shift, shift)
+        else:
+            shift = color * 3
+            return cls.from_rgb(255 - shift, shift, 0)
+
+    RED: typing.ClassVar['Color']
+    ORANGE: typing.ClassVar['Color']
+    YELLOW: typing.ClassVar['Color']
+    GREEN: typing.ClassVar['Color']
+    MINT: typing.ClassVar['Color']
+    AQUA: typing.ClassVar['Color']
+    BLUE: typing.ClassVar['Color']
+    VIOLET: typing.ClassVar['Color']
+    PINK: typing.ClassVar['Color']
+    DEFAULT: typing.ClassVar['Color']
+
+
+for _k, _v in dict(RED=0xcb2839, ORANGE=0xd55f30, YELLOW=0xd69d27, GREEN=0x37A93C, MINT=0x25b18f, AQUA=0x2ba1cd,
+                   BLUE=0x297bcd, VIOLET=0x825ae7, PINK=0xc8589a, DEFAULT=0xffffffff).items():
+    setattr(Color, _k, Color.from_hex(_v))
+del _k
+del _v
+
+
+def parse_url(url: str) -> tuple[str, str | None, str | None, str | None, str | None]:
+    prefix, *url = url.split('/', maxsplit=4)
+    cmd = clid = did = name = None
+
+    if url:
+        did, *url = url
+    if len(url) == 1:
+        print(prefix, url)
+        raise ValueError("Invalid data!")
+        # return prefix, clid, did, cmd, name
+    if url:
+        clid, cmd, *url = url
+    if url:
+        name, = url
+    return prefix, clid, did, cmd, name
+
+
+def generate_did():
+    raise ValueError("Missing did and generating not supported!")
+
+
+def response(typ: str, **kwargs):
+    kwargs['type'] = typ
+    return kwargs
```

### Comparing `pygyverhubd-0.0.1/pygyverhubd.egg-info/PKG-INFO` & `pygyverhubd-0.0.2/pygyverhubd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-Metadata-Version: 2.1
-Name: pygyverhubd
-Version: 0.0.1
-Summary: Python implementation of GyverHub device
-Author-email: NekoNekoNyan <me@neko-dev.ru>
-License: MIT License
-        
-        Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/neko-neko-nyan/pygyverhubd
-Project-URL: Bug Tracker, https://github.com/neko-neko-nyan/pygyverhubd/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Реализация сервера (устройства) GyverHub на python
-
-## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
-
-На данный момент работает только WebSocket
-
-Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
-(кроме передачи файлов по http)
-
-Пример использования [здесь](examples/components_ui.py)
-
-# Текущий прогресс
-## Сеть
-- [x] Интерфейс: WebSocket
-- [ ] Интерфейс: MQTT
-- [ ] Интерфейс: Bluetooth
-- [ ] Интерфейс: Serial
-- [x] Device discovery
-- [ ] Встроенный клиент
-
-## GUI
-- [x] Базовые компоненты
-- [ ] Canvas
-- [ ] Вкладки
-
-## Устройство
-- [x] Базовая информация - название, иконка
-- [x] Расширенная информация - сеть, память
-- [ ] Автоматический сбор расширенной информации
-
-## OTA
-- [x] OTA API
-- [ ] Обновление сервера через OTA
-- [ ] Автообновление
-- [ ] Автоматическая упаковка обновлений
-
-## ФС
-- [x] API файловой системы
-- [ ] Отражение API ФС на реальную папку
-
-## Другие компоненты
-- [ ] Перезапуск сервера по команде reboot
-- [x] CLI API
+Metadata-Version: 2.1
+Name: pygyverhubd
+Version: 0.0.2
+Summary: Python implementation of GyverHub device
+Author-email: NekoNekoNyan <me@neko-dev.ru>
+License: MIT License
+        
+        Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/neko-neko-nyan/pygyverhubd
+Project-URL: Bug Tracker, https://github.com/neko-neko-nyan/pygyverhubd/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Реализация сервера (устройства) GyverHub на python
+
+## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
+
+На данный момент работает только WebSocket
+
+Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
+(кроме передачи файлов по http)
+
+Пример использования [здесь](examples/components_ui.py)
+
+# Текущий прогресс
+## Сеть
+- [x] Интерфейс: WebSocket
+- [ ] Интерфейс: MQTT
+- [ ] Интерфейс: Bluetooth
+- [ ] Интерфейс: Serial
+- [x] Device discovery
+- [ ] Встроенный клиент
+
+## GUI
+- [x] Базовые компоненты
+- [ ] Canvas
+- [ ] Вкладки
+
+## Устройство
+- [x] Базовая информация - название, иконка
+- [x] Расширенная информация - сеть, память
+- [ ] Автоматический сбор расширенной информации
+
+## OTA
+- [x] OTA API
+- [ ] Обновление сервера через OTA
+- [ ] Автообновление
+- [ ] Автоматическая упаковка обновлений
+
+## ФС
+- [x] API файловой системы
+- [ ] Отражение API ФС на реальную папку
+
+## Другие компоненты
+- [ ] Перезапуск сервера по команде reboot
+- [x] CLI API
```

### Comparing `pygyverhubd-0.0.1/pygyverhubd.egg-info/SOURCES.txt` & `pygyverhubd-0.0.2/pygyverhubd.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 gyverhubd/__init__.py
+gyverhubd/_version.py
 gyverhubd/device.py
 gyverhubd/filesystem.py
 gyverhubd/info.py
 gyverhubd/server.py
 gyverhubd/utils.py
 gyverhubd/proto/__init__.py
 gyverhubd/proto/proto.py
```

### Comparing `pygyverhubd-0.0.1/pyproject.toml` & `pygyverhubd-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-[project]
-name = "pygyverhubd"
-description = "Python implementation of GyverHub device"
-license = {file = "LICENSE"}
-authors = [
-    {name = "NekoNekoNyan", email="me@neko-dev.ru"}
-]
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent"
-]
-dependencies = [
-    "aiohttp~=3.8.4",
-    "websockets~=11.0.3"
-]
-dynamic = ["version", "readme"]
-
-[project.urls]
-"Homepage" = "https://github.com/neko-neko-nyan/pygyverhubd"
-"Bug Tracker" = "https://github.com/neko-neko-nyan/pygyverhubd/issues"
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
-include = ["gyverhubd*"]
-namespaces = false
-
-[tool.setuptools.dynamic]
-version = {attr = "gyverhubd.__version__"}
-readme = {file = "README.md", content-type = "text/markdown"}
+[project]
+name = "pygyverhubd"
+description = "Python implementation of GyverHub device"
+license = {file = "LICENSE"}
+authors = [
+    {name = "NekoNekoNyan", email="me@neko-dev.ru"}
+]
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent"
+]
+dependencies = [
+    "aiohttp~=3.8.4",
+    "websockets~=11.0.3"
+]
+dynamic = ["version", "readme"]
+
+[project.urls]
+"Homepage" = "https://github.com/neko-neko-nyan/pygyverhubd"
+"Bug Tracker" = "https://github.com/neko-neko-nyan/pygyverhubd/issues"
+
+[build-system]
+requires = ["setuptools>=61.0", "wheel", "setuptools-git-versioning<2"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools-git-versioning]
+enabled = true
+
+[tool.setuptools.packages.find]
+include = ["gyverhubd*"]
+namespaces = false
+
+[tool.setuptools.dynamic]
+readme = {file = "README.md", content-type = "text/markdown"}
```

