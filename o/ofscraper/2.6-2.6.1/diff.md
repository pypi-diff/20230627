# Comparing `tmp/ofscraper-2.6.tar.gz` & `tmp/ofscraper-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.6.tar", max compression
+gzip compressed data, was "ofscraper-2.6.1.tar", max compression
```

## Comparing `ofscraper-2.6.tar` & `ofscraper-2.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-06-25 19:47:48.618819 ofscraper-2.6/LICENSE
--rw-r--r--   0        0        0     2862 2023-06-25 19:47:48.618819 ofscraper-2.6/README.md
--rw-r--r--   0        0        0      607 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8188 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/archive.py
--rw-r--r--   0        0        0     4852 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/init.py
--rw-r--r--   0        0        0     2859 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/me.py
--rw-r--r--   0        0        0     9021 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9689 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5550 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11505 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3909 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8725 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    14097 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/check.py
--rw-r--r--   0        0        0     4884 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    13452 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6312 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4973 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7683 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27766 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1139 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    11211 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8950 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10803 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19529 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3376 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     6442 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9615 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/of.py
--rw-r--r--   0        0        0    11732 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    29248 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/table.py
--rw-r--r--   0        0        0     6089 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1694 2023-06-25 19:48:22.475505 ofscraper-2.6/pyproject.toml
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 ofscraper-2.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-27 15:23:52.029471 ofscraper-2.6.1/LICENSE
+-rw-r--r--   0        0        0     2862 2023-06-27 15:23:52.029471 ofscraper-2.6.1/README.md
+-rw-r--r--   0        0        0      607 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8281 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     4920 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2859 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9111 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9871 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5640 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11761 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3909 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3205 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8815 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    14097 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     4937 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    13452 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6337 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4973 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27766 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1139 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    11211 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8950 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10803 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19529 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3376 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     6442 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9615 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/of.py
+-rw-r--r--   0        0        0    11732 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-27 15:23:52.037472 ofscraper-2.6.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    29248 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     6089 2023-06-27 15:23:52.041472 ofscraper-2.6.1/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1696 2023-06-27 15:24:34.413645 ofscraper-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 ofscraper-2.6.1/PKG-INFO
```

### Comparing `ofscraper-2.6/LICENSE` & `ofscraper-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/README.md` & `ofscraper-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/__init__.py` & `ofscraper-2.6.1/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/__version__.py` & `ofscraper-2.6.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/api/archive.py` & `ofscraper-2.6.1/ofscraper/api/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,17 @@
     Panel(Group(job_progress)))
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                            sock_connect=None, sock_read=None)) as c: 
+        
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                            sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.AlT_SEM)) as c: 
 
             oldarchived=cache.get(f"archived_{model_id}",default=[])
             oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
             log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
             oldarchived=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldarchived))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldarchived)))
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
```

### Comparing `ofscraper-2.6/ofscraper/api/highlights.py` & `ofscraper-2.6.1/ofscraper/api/highlights.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     Panel(Group(job_progress)))
 
     output=[]
     page_count=0
     global tasks
     tasks=[]
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=1)) as c: 
             tasks.append(asyncio.create_task(scrape_highlights(c,model_id,job_progress)))
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
                     page_count=page_count+1
                     overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
```

### Comparing `ofscraper-2.6/ofscraper/api/init.py` & `ofscraper-2.6.1/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/api/me.py` & `ofscraper-2.6.1/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/api/messages.py` & `ofscraper-2.6.1/ofscraper/api/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
     tasks=[]
     responseArray=[]
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
             oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
             oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
             log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
             oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
             startdex=0 if len(oldmessages)==0 else \
             max(([i for i in range(len(oldmessages)) if arrow.get(oldmessages[i].get("createdAt") or oldmessages[i].get("postedAt")) <=(args_.getargs().before or arrow.now())] or [len(oldmessages)])[0]-1,0)
             log.debug(f"Setting Start Index at {startdex}")
```

### Comparing `ofscraper-2.6/ofscraper/api/paid.py` & `ofscraper-2.6.1/ofscraper/api/paid.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     Panel(Group(job_progress)))
 
     output=[]
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
 
             tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress)))
 
             
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
@@ -104,15 +104,15 @@
             data=await r.json()
             attempt.set(0)
             media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> media found {len(media)}")
             log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
             if  data.get("hasMore"):
                 offset += len(media)
-                tasks.append(asyncio.create_task(scrape_paid(username,job_progress,offset=offset)))
+                tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress,offset=offset)))
             job_progress.remove_task(task)
 
         else:
             log.debug(f"[bold]paid request status code:[/bold]{r.status}")
             log.debug(f"[bold]paid response:[/bold] {await r.text()}")
             log.debug(f"[bold]paid headers:[/bold] {r.headers}")
             job_progress.remove_task(task)
@@ -132,16 +132,16 @@
 
     output=[]
     min_posts=100
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
             allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
             log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
             
         
             if len(allpaid)>min_posts:
                 splitArrays=[i for i in range(0, len(allpaid), min_posts)]
                 #use the previous split for timesamp
```

### Comparing `ofscraper-2.6/ofscraper/api/pinned.py` & `ofscraper-2.6.1/ofscraper/api/pinned.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                                    sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                                    sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
             tasks.append(asyncio.create_task(scrape_pinned_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
         
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
```

### Comparing `ofscraper-2.6/ofscraper/api/posts.py` & `ofscraper-2.6.1/ofscraper/api/posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import aiohttp
 import arrow
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
+import ofscraper.constants as constants
 import ofscraper.utils.config as config
 
 
 log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
@@ -366,15 +367,16 @@
         return self._media
     @property
     async def parse_mpd(self): 
         if not self.mpd:
             return
       
         params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
-        async with aiohttp.ClientSession() as session:
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                                    sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as session:
             headers=auth.make_headers(auth.read_auth())
             headers=auth.create_sign(self.mpd, headers) 
             async with session.request("get",self.mpd,headers=headers,params=params) as r:
                 if not r.ok:
                     return None
                 return MPEGDASHParser.parse(await r.text())
     @property
```

### Comparing `ofscraper-2.6/ofscraper/api/profile.py` & `ofscraper-2.6.1/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/api/subscriptions.py` & `ofscraper-2.6.1/ofscraper/api/subscriptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 from itertools import chain
 import logging
-import httpx
+import aiohttp
 from rich.console import Console
 import arrow
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
 from ..utils import auth, dates
 import ofscraper.constants as constants
@@ -26,25 +26,24 @@
     offsets = range(0, subscribe_count, 10)
     tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
     subscriptions = await asyncio.gather(*tasks)
     return list(chain.from_iterable(subscriptions))
 
 
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_subscriptions(headers, offset=500) -> list:
-    async with httpx.AsyncClient(http2=True, headers=headers) as c:
+async def scrape_subscriptions(headers, offset=0) -> list:
+    async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,sock_connect=None, sock_read=None)) as c: 
         url = subscriptionsEP.format(offset)
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-
-        r = await c.get(subscriptionsEP.format(offset), timeout=None)
-        if not r.is_error:
-            subscriptions = r.json()
-            return subscriptions
-        r.raise_for_status()
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+            if r.ok:
+                subscriptions = await r.json()
+                return subscriptions
+            r.raise_for_status()
 
 def parse_subscriptions(subscriptions: list) -> list:
     datenow=arrow.now()
     data = [
         {"name":profile['username']
          ,"id":profile['id'],
          "sub-price":profile.get("currentSubscribePrice",{}),
```

### Comparing `ofscraper-2.6/ofscraper/api/timeline.py` & `ofscraper-2.6.1/ofscraper/api/timeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
+                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
 
             oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
             oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
             log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
             oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
```

### Comparing `ofscraper-2.6/ofscraper/commands/check.py` & `ofscraper-2.6.1/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/commands/manual.py` & `ofscraper-2.6.1/ofscraper/commands/manual.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,19 @@
     return timeline.get_individual_post(postid,client)
             
 
     
 
 def get_all_media(id_dict,inputtype=None):
     media_dict={}
+    
 
     for model_id,value in  id_dict.items():
+        if model_id==None:
+            continue
         temp = []
         user_name = profile.scrape_profile( model_id)['username']
         posts_array=list(map(lambda x:posts_.Post(
         x, model_id, user_name,responsetype=inputtype), value))
         [temp.extend(ele.media) for ele in posts_array]
         media_dict[model_id]=temp
```

### Comparing `ofscraper-2.6/ofscraper/commands/scraper.py` & `ofscraper-2.6.1/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/constants.py` & `ofscraper-2.6.1/ofscraper/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,8 +136,10 @@
 
 THREADS_DEFAULT=8
 MAX_SEMAPHORE=8
 AlT_SEM=4
 CODE_EXECUTION_DEFAULT =False
 
 NUMBER_REGEX="[0-9]"
-USERNAME_REGEX="[^/]"
+USERNAME_REGEX="[^/]"
+
+API_REEQUEST_TIMEOUT=90
```

### Comparing `ofscraper-2.6/ofscraper/db/operations.py` & `ofscraper-2.6.1/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/db/queries.py` & `ofscraper-2.6.1/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/interaction/like.py` & `ofscraper-2.6.1/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.6.1/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.6.1/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/prompts/prompts.py` & `ofscraper-2.6.1/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/start.py` & `ofscraper-2.6.1/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/args.py` & `ofscraper-2.6.1/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/auth.py` & `ofscraper-2.6.1/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/binaries.py` & `ofscraper-2.6.1/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/config.py` & `ofscraper-2.6.1/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/dates.py` & `ofscraper-2.6.1/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/download.py` & `ofscraper-2.6.1/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/encoding.py` & `ofscraper-2.6.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/exit.py` & `ofscraper-2.6.1/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/filters.py` & `ofscraper-2.6.1/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/logger.py` & `ofscraper-2.6.1/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/of.py` & `ofscraper-2.6.1/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/paths.py` & `ofscraper-2.6.1/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/profiles.py` & `ofscraper-2.6.1/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/separate.py` & `ofscraper-2.6.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/stdout.py` & `ofscraper-2.6.1/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/table.py` & `ofscraper-2.6.1/ofscraper/utils/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/ofscraper/utils/userselector.py` & `ofscraper-2.6.1/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.6/pyproject.toml` & `ofscraper-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.6"
+version = "2.6.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.6/PKG-INFO` & `ofscraper-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.6
+Version: 2.6.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

