# Comparing `tmp/parsedmarc-8.6.0.tar.gz` & `tmp/parsedmarc-8.6.1.tar.gz`

## Comparing `parsedmarc-8.6.0.tar` & `parsedmarc-8.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/__init__.py
--rw-r--r--   0        0        0    48948 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/cli.py
--rw-r--r--   0        0        0    20853 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/elastic.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/kafkaclient.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/log.py
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/loganalytics.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/s3.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/splunk.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/syslog.py
--rw-r--r--   0        0        0    16553 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/utils.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/__init__.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/gmail.py
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/graph.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/imap.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/mailbox_connection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/resources/__init__.py
--rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/resources/dbip-country-lite.mmdb
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/LICENSE
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/pyproject.toml
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/PKG-INFO
+-rw-r--r--   0        0        0    61994 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/__init__.py
+-rw-r--r--   0        0        0    49112 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/cli.py
+-rw-r--r--   0        0        0    21027 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/elastic.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/kafkaclient.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/log.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/loganalytics.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/s3.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/splunk.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/syslog.py
+-rw-r--r--   0        0        0    16553 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/utils.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/mail/__init__.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/mail/gmail.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/mail/graph.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/mail/imap.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/mail/mailbox_connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/resources/__init__.py
+-rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/parsedmarc/resources/dbip-country-lite.mmdb
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/LICENSE
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 parsedmarc-8.6.1/PKG-INFO
```

### Comparing `parsedmarc-8.6.0/parsedmarc/__init__.py` & `parsedmarc-8.6.1/parsedmarc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from parsedmarc.log import logger
 from parsedmarc.mail import MailboxConnection
 from parsedmarc.utils import get_base_domain, get_ip_address_info
 from parsedmarc.utils import is_outlook_msg, convert_outlook_msg
 from parsedmarc.utils import parse_email
 from parsedmarc.utils import timestamp_to_human, human_timestamp_to_datetime
 
-__version__ = "8.6.0"
+__version__ = "8.6.1"
 
 logger.debug("parsedmarc v{0}".format(__version__))
 
 feedback_report_regex = re.compile(r"^([\w\-]+): (.+)$", re.MULTILINE)
 xml_header_regex = re.compile(r"^<\?xml .*?>", re.MULTILINE)
 xml_schema_regex = re.compile(r"</??xs:schema.*>", re.MULTILINE)
 text_report_regex = re.compile(r"\s*([a-zA-Z\s]+):\s(.+)", re.MULTILINE)
@@ -247,27 +247,40 @@
         new_report_metadata = OrderedDict()
         if report_metadata["org_name"] is None:
             if report_metadata["email"] is not None:
                 report_metadata["org_name"] = report_metadata[
                     "email"].split("@")[-1]
         org_name = report_metadata["org_name"]
         if org_name is not None and " " not in org_name:
-            org_name = get_base_domain(org_name)
+            new_org_name = get_base_domain(org_name)
+            if new_org_name is not None:
+                org_name = new_org_name
+        if not org_name:
+            logger.debug("Could not parse org_name from XML.\r\n{0}".format(
+                report.__str__()
+            ))
+            raise KeyError("Organization name is missing. \
+                           This field is a requirement for \
+                           saving the report")
         new_report_metadata["org_name"] = org_name
         new_report_metadata["org_email"] = report_metadata["email"]
         extra = None
         if "extra_contact_info" in report_metadata:
             extra = report_metadata["extra_contact_info"]
         new_report_metadata["org_extra_contact_info"] = extra
         new_report_metadata["report_id"] = report_metadata["report_id"]
         report_id = new_report_metadata["report_id"]
         report_id = report_id.replace("<",
                                       "").replace(">", "").split("@")[0]
         new_report_metadata["report_id"] = report_id
         date_range = report["report_metadata"]["date_range"]
+        if (int(date_range["end"]) - int(date_range["begin"]) > 2*86400):
+            raise InvalidAggregateReport("The begin and end fields span too \
+                                         many hours, should be max 24 hours \
+                                         according to RFC 7489 section 7.2")
         date_range["begin"] = timestamp_to_human(date_range["begin"])
         date_range["end"] = timestamp_to_human(date_range["end"])
         new_report_metadata["begin_date"] = date_range["begin"]
         new_report_metadata["end_date"] = date_range["end"]
         if "error" in report["report_metadata"]:
             if type(report["report_metadata"]["error"]) != list:
                 errors = [report["report_metadata"]["error"]]
@@ -358,21 +371,22 @@
     Args:
         input_: A path to a file, a file like object, or bytes
 
     Returns:
         str: The extracted XML
 
     """
-    if type(input_) == str:
-        file_object = open(input_, "rb")
-    elif type(input_) == bytes:
-        file_object = BytesIO(input_)
-    else:
-        file_object = input_
     try:
+        if type(input_) == str:
+            file_object = open(input_, "rb")
+        elif type(input_) == bytes:
+            file_object = BytesIO(input_)
+        else:
+            file_object = input_
+
         header = file_object.read(6)
         file_object.seek(0)
         if header.startswith(MAGIC_ZIP):
             _zip = zipfile.ZipFile(file_object)
             xml = _zip.open(_zip.namelist()[0]).read().decode(errors='ignore')
         elif header.startswith(MAGIC_GZIP):
             xml = GzipFile(fileobj=file_object).read().decode(errors='ignore')
@@ -380,14 +394,16 @@
             xml = file_object.read().decode(errors='ignore')
         else:
             file_object.close()
             raise InvalidAggregateReport("Not a valid zip, gzip, or xml file")
 
         file_object.close()
 
+    except FileNotFoundError:
+        raise InvalidAggregateReport("File was not found")
     except UnicodeDecodeError:
         file_object.close()
         raise InvalidAggregateReport("File objects must be opened in binary "
                                      "(rb) mode")
     except Exception as error:
         file_object.close()
         raise InvalidAggregateReport(
```

### Comparing `parsedmarc-8.6.0/parsedmarc/cli.py` & `parsedmarc-8.6.1/parsedmarc/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,17 @@
                             number_of_replicas=replicas
                         )
                 except elastic.AlreadySaved as warning:
                     logger.warning(warning.__str__())
                 except elastic.ElasticsearchError as error_:
                     logger.error("Elasticsearch Error: {0}".format(
                         error_.__str__()))
+                except Exception as error_:
+                    logger.error("Elasticsearch exception error: {}".format(
+                        error_.__str__()))
                 try:
                     if opts.kafka_hosts:
                         kafka_client.save_aggregate_reports_to_kafka(
                             report, kafka_aggregate_topic)
                 except Exception as error_:
                     logger.error("Kafka Error: {0}".format(
                          error_.__str__()))
```

### Comparing `parsedmarc-8.6.0/parsedmarc/elastic.py` & `parsedmarc-8.6.1/parsedmarc/elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,20 @@
         search = Search(index="dmarc_aggregate_{0}*".format(index_suffix))
     else:
         search = Search(index="dmarc_aggregate*")
     query = org_name_query & report_id_query & domain_query
     query = query & begin_date_query & end_date_query
     search.query = query
 
-    existing = search.execute()
+    try:
+        existing = search.execute()
+    except Exception as error_:
+        raise ElasticsearchError("Elasticsearch's search for existing report \
+            error: {}".format(error_.__str__()))
+
     if len(existing) > 0:
         raise AlreadySaved("An aggregate report ID {0} from {1} about {2} "
                            "with a date range of {3} UTC to {4} UTC already "
                            "exists in "
                            "Elasticsearch".format(report_id,
                                                   org_name,
                                                   domain,
```

### Comparing `parsedmarc-8.6.0/parsedmarc/kafkaclient.py` & `parsedmarc-8.6.1/parsedmarc/kafkaclient.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/loganalytics.py` & `parsedmarc-8.6.1/parsedmarc/loganalytics.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/s3.py` & `parsedmarc-8.6.1/parsedmarc/s3.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/splunk.py` & `parsedmarc-8.6.1/parsedmarc/splunk.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/syslog.py` & `parsedmarc-8.6.1/parsedmarc/syslog.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/utils.py` & `parsedmarc-8.6.1/parsedmarc/utils.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/mail/gmail.py` & `parsedmarc-8.6.1/parsedmarc/mail/gmail.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/mail/graph.py` & `parsedmarc-8.6.1/parsedmarc/mail/graph.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/mail/imap.py` & `parsedmarc-8.6.1/parsedmarc/mail/imap.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/mail/mailbox_connection.py` & `parsedmarc-8.6.1/parsedmarc/mail/mailbox_connection.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/parsedmarc/resources/dbip-country-lite.mmdb` & `parsedmarc-8.6.1/parsedmarc/resources/dbip-country-lite.mmdb`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/.gitignore` & `parsedmarc-8.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/LICENSE` & `parsedmarc-8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/README.md` & `parsedmarc-8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/pyproject.toml` & `parsedmarc-8.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.6.0/PKG-INFO` & `parsedmarc-8.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsedmarc
-Version: 8.6.0
+Version: 8.6.1
 Summary: A Python package and CLI for parsing aggregate and forensic DMARC reports
 Project-URL: Homepage, https://domainaware.github.io/parsedmarc
 Author-email: Sean Whalen <whalenster@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: DMARC,parser,reporting
 Classifier: Development Status :: 5 - Production/Stable
```

