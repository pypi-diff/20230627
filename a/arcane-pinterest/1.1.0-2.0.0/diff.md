# Comparing `tmp/arcane-pinterest-1.1.0.tar.gz` & `tmp/arcane_pinterest-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-pinterest-1.1.0.tar", max compression
+gzip compressed data, was "arcane_pinterest-2.0.0.tar", max compression
```

## Comparing `arcane-pinterest-1.1.0.tar` & `arcane_pinterest-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      112 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/__init__.py
--rw-r--r--   0        0        0       51 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/const.py
--rw-r--r--   0        0        0      241 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/exceptions.py
--rw-r--r--   0        0        0     2426 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/lib.py
--rw-r--r--   0        0        0     9215 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/pinterest.py
--rw-r--r--   0        0        0      123 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/arcane/pinterest/types.py
--rw-r--r--   0        0        0      412 2022-03-10 08:48:54.564085 arcane-pinterest-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      696 2022-03-10 08:49:11.758722 arcane-pinterest-1.1.0/setup.py
--rw-r--r--   0        0        0      604 2022-03-10 08:49:11.759041 arcane-pinterest-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/const.py
+-rw-r--r--   0        0        0      241 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/exceptions.py
+-rw-r--r--   0        0        0     2394 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/lib.py
+-rw-r--r--   0        0        0     6882 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/pinterest.py
+-rw-r--r--   0        0        0      123 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/arcane/pinterest/types.py
+-rw-r--r--   0        0        0      408 2023-06-27 08:31:02.137182 arcane_pinterest-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 arcane_pinterest-2.0.0/PKG-INFO
```

### Comparing `arcane-pinterest-1.1.0/arcane/pinterest/lib.py` & `arcane_pinterest-2.0.0/arcane/pinterest/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,28 +33,28 @@
 
     Returns:
         PinterestReport: Pinterest Report response as we get
     """
 
     @backoff.on_exception(backoff.expo, PinterestAsyncReportNotReadyException, max_tries=10)
     def _get_pinterest_report_url(account_id: str, token: str, pinterest_client: PinterestClient) -> str:
-        reponse = pinterest_client.get_campaign_metrics(account_id, token).get('data', {})
+        reponse = pinterest_client.get_campaign_metrics(account_id, token)
         if reponse.get('report_status') != _PINTEREST_REPORT_READY_VALUE:
             pinterest_client.log(f"Pinterest report for account id {account_id} is not ready yet")
             raise PinterestAsyncReportNotReadyException
         return reponse['url']
 
 
     pinterest_client.log(f"Getting Pinterest report token for account id {account_id}...")
-    token = pinterest_client.post_advertiser_metrics_report(
-        advertiser_id=account_id,
+    token = pinterest_client.post_ad_account_metrics_report(
+        ad_account_id=account_id,
         start_date=start_date.strftime("%Y-%m-%d"),
         end_date=end_date.strftime("%Y-%m-%d"),
         columns=columns
-    ).get('data', {}).get('token')
+    ).get('token')
     if token is None:
         raise Error('Token should not be None when getting pinterest report')
     pinterest_client.log(f"Retrieving report url for account id {account_id}")
     url = _get_pinterest_report_url(account_id, token, pinterest_client)
 
     reponse = requests.get(url)
     reponse.raise_for_status()
```

