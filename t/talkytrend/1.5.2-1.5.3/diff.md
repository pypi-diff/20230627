# Comparing `tmp/talkytrend-1.5.2.tar.gz` & `tmp/talkytrend-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.2.tar", max compression
+gzip compressed data, was "talkytrend-1.5.3.tar", max compression
```

## Comparing `talkytrend-1.5.2.tar` & `talkytrend-1.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-26 14:27:59.521110 talkytrend-1.5.2/LICENSE
--rw-r--r--   0        0        0     2190 2023-06-26 14:27:59.521110 talkytrend-1.5.2/README.md
--rw-r--r--   0        0        0     2178 2023-06-26 14:28:00.329120 talkytrend-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-26 14:28:00.329120 talkytrend-1.5.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/config.py
--rw-r--r--   0        0        0     1653 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6419 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/main.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 20:17:36.741904 talkytrend-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2190 2023-06-27 20:17:36.741904 talkytrend-1.5.3/README.md
+-rw-r--r--   0        0        0     2178 2023-06-27 20:17:37.425910 talkytrend-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-27 20:17:37.425910 talkytrend-1.5.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/config.py
+-rw-r--r--   0        0        0     1642 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6426 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/main.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.3/PKG-INFO
```

### Comparing `talkytrend-1.5.2/LICENSE` & `talkytrend-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.2/README.md` & `talkytrend-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.2/pyproject.toml` & `talkytrend-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.2"
+version = "1.5.3"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.2/talkytrend/config.py` & `talkytrend-1.5.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.2/talkytrend/default_settings.toml` & `talkytrend-1.5.3/talkytrend/default_settings.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
 enable_news = true
-news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
+news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 [testing]
 VALUE = "On Testing"
 talkytrend_enabled = true
 talkytrend_mode = "scanner"
```

### Comparing `talkytrend-1.5.2/talkytrend/main.py` & `talkytrend-1.5.3/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
             return table.get_string()
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
 
-
     def is_new_signal(self, asset_id, interval, current_signal):
         if self.asset_signals.get(asset_id):
             if self.asset_signals[asset_id].get(interval) and current_signal != self.asset_signals[asset_id][interval]:
                 self.asset_signals[asset_id][interval] = current_signal
                 return True
         else:
             self.asset_signals[asset_id] = {interval: current_signal}
@@ -130,15 +129,15 @@
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
                     key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
                     last_item = key_news[-1]
-                    return f"{last_item['title']} {last_item['url']}"
+                    return f"📰 [{last_item['title']}]({last_item['url']})"
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
```

### Comparing `talkytrend-1.5.2/PKG-INFO` & `talkytrend-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

