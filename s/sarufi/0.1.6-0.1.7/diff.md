# Comparing `tmp/sarufi-0.1.6-py3-none-any.whl.zip` & `tmp/sarufi-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13205 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    32457 b- defN 23-Jun-22 16:10 sarufi/__init__.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6286 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/RECORD
-6 files, 50656 bytes uncompressed, 12383 bytes compressed:  75.6%
+Zip file size: 13226 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    32511 b- defN 23-Jun-26 15:20 sarufi/__init__.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-27 13:21 sarufi-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6286 b- defN 23-Jun-27 13:21 sarufi-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 13:21 sarufi-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-27 13:21 sarufi-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      457 b- defN 23-Jun-27 13:21 sarufi-0.1.7.dist-info/RECORD
+6 files, 50710 bytes uncompressed, 12404 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.6.dist-info/LICENSE
+Filename: sarufi-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.6.dist-info/METADATA
+Filename: sarufi-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.6.dist-info/WHEEL
+Filename: sarufi-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.6.dist-info/top_level.txt
+Filename: sarufi-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.6.dist-info/RECORD
+Filename: sarufi-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -477,14 +477,15 @@
         self, bot_id: int, chat_id: str, message: str, message_type: str, channel: str
     ):
         url = self._BASE_URL + "conversation/"
         if channel == "whatsapp":
             logger.info("Sending message to bot via whatsapp")
             url = url + "whatsapp/"
 
+        logger.info(f"The URL is got to Hello {url}")
         data = {
             "chat_id": chat_id,
             "bot_id": bot_id,
             "message": message,
             "message_type": message_type,
         }
         return self._post_req(url=url, body=data)
```

## Comparing `sarufi-0.1.6.dist-info/LICENSE` & `sarufi-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.6.dist-info/METADATA` & `sarufi-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
 Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
```

