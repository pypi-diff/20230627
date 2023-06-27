# Comparing `tmp/nonebot-plugin-twitter-0.1.7.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.7.tar", last modified: Mon Jun 12 06:32:23 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.8.tar", last modified: Tue Jun 27 15:35:27 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.7.tar` & `nonebot-plugin-twitter-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/LICENSE
--rw-r--r--   0        0        0     3053 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/README.md
--rw-r--r--   0        0        0    14773 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4741 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3154 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/README.md
+-rw-r--r--   0        0        0    14821 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.8/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.7/LICENSE` & `nonebot-plugin-twitter-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.7/README.md` & `nonebot-plugin-twitter-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -94,7 +94,13 @@
 ### 注意事项
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
 
 3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
+
+### 更新记录
+
+2023.06.27
+
+1. 临时解决回复原推文时，无法推送全部推文的问题
```

#### html2text {}

```diff
@@ -26,7 +26,9 @@
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
 (https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
 3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
+### æ´æ°è®°å½ 2023.06.27 1.
+ä¸´æ¶è§£å³åå¤åæ¨ææ¶ï¼æ æ³æ¨éå¨é¨æ¨æçé®é¢
```

### Comparing `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,19 +114,20 @@
             tweet_info = await get_tweet(user_name,line_new_tweet_id)
             if not tweet_info["status"]:
                 logger.info(f"{user_name} 的推文 {line_new_tweet_id} 获取失败")
                 return 
             else:
                 task = []
                 task_res = []
-                task_res.append(MessageSegment.node_custom(
-                    user_id=config_dev.twitter_qq,
-                    nickname=twitter_list[user_name]["screen_name"],
-                    content=Message(tweet_info["text"])
-                ))
+                for x in tweet_info["text"]:
+                    task_res.append(MessageSegment.node_custom(
+                        user_id=config_dev.twitter_qq,
+                        nickname=twitter_list[user_name]["screen_name"],
+                        content=Message(x)
+                    ))
                 
                 if tweet_info["pic_url_list"]:
                     for url in tweet_info["pic_url_list"]:
                         task_res.append(await get_pic(url,user_name))
                         
                 # 视频
                 if tweet_info["video_url"]:
```

### Comparing `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,20 @@
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}/status/{tweet_id}",cookies={"hlsPlayback": "on"})
         result = {}
         if res.status_code ==200:
             result["status"] = True
             soup = BeautifulSoup(res.text,"html.parser")
             # text
-            result["text"] = match[0].text if (match := soup.find_all('div', class_='tweet-content media-body')) else ""
+            result["text"] = []
+            if match := soup.find_all('div', class_='tweet-content media-body'):
+                for x in match:
+                    if x.parent.attrs["class"] == "replying-to":
+                        continue
+                    result["text"].append(x.text) 
             # pic
             if pic_list := soup.find_all('a', class_='still-image'):
                 result["pic_url_list"] = [x.attrs["href"] for x in pic_list]
             else:
                 result["pic_url_list"] = []
             # video
             if video_list := soup.find_all('video'):
```

### Comparing `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.7/pyproject.toml` & `nonebot-plugin-twitter-0.1.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.7"
+version = "0.1.8"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.7/PKG-INFO` & `nonebot-plugin-twitter-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.7
+Version: 0.1.8
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -106,7 +106,13 @@
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
 
 3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
 
+### 更新记录
+
+2023.06.27
+
+1. 临时解决回复原推文时，无法推送全部推文的问题
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.8 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
@@ -31,7 +31,9 @@
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
 (https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
 3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
+### æ´æ°è®°å½ 2023.06.27 1.
+ä¸´æ¶è§£å³åå¤åæ¨ææ¶ï¼æ æ³æ¨éå¨é¨æ¨æçé®é¢
```

