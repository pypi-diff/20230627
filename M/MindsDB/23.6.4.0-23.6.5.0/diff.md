# Comparing `tmp/MindsDB-23.6.4.0.tar.gz` & `tmp/MindsDB-23.6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.6.4.0.tar", last modified: Tue Jun 20 13:31:49 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.6.5.0.tar", last modified: Tue Jun 27 09:23:11 2023, max compression
```

## Comparing `MindsDB-23.6.4.0.tar` & `MindsDB-23.6.5.0.tar`

### file list

```diff
@@ -1,1386 +1,1413 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 13:31:30.000000 MindsDB-23.6.4.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25738 2023-06-20 13:31:48.000000 MindsDB-23.6.4.0/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66230 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:48.000000 MindsDB-23.6.4.0/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-20 13:31:48.000000 MindsDB-23.6.4.0/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:48.000000 MindsDB-23.6.4.0/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25738 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20662 2023-06-20 13:31:30.000000 MindsDB-23.6.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57116 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67825 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/question_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/chatbot_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/chatbot_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/base/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/requirements/requirements-telemetry.txt
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:31:49.000000 MindsDB-23.6.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-20 13:31:31.000000 MindsDB-23.6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 09:23:00.000000 MindsDB-23.6.5.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    67630 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-27 09:23:00.000000 MindsDB-23.6.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57116 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68016 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164968 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29331 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39688 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/web_handler/web_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/question_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/realtime_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/realtime_chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/base/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/requirements/requirements-telemetry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:23:11.000000 MindsDB-23.6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-27 09:23:01.000000 MindsDB-23.6.5.0/setup.py
```

### Comparing `MindsDB-23.6.4.0/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.6.5.0/MindsDB.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.4.0
+Version: 23.6.5.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -57,50 +57,47 @@
         	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
         </h3>
         
         </div>
         
         ----------------------------------------
         
-        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered systems from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
         
-        We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
+        ## What can you build with MindsDB?
         
-        By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
+        * **Question Answering**: This is useful when you have data (we support more than 120 data sources) and you need answers from your data given a question in natural language.
+        * **Semantic Search**: Similar to Question Answering, but in this case, you want to retrieve specific parts of your data where the answer to a question may exist.
+        * **AI Agent serving**: This is useful when you want to publish your AI Agents to enterprise conversational applications like Slack, email, Twilio, etc.
+        * **Recommendation systems**: When you use your data to help predict, narrow down, and find what people are looking for among an exponentially growing number of options.
+        * **Time Series Forecasting**: When you want to use your historical data to estimate how things will look in the future.
+        * **AI Automation pipelines**: When you need your AI systems to consume enterprise data and have the AI output stored back into your enterprise tools in an automated way.
         
-        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
+        ## Generative AI Tables
         
-        <h2 align="center">
-           <br/>
-           <br/>
-          <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
+        MindsDB empowers developers to harness the power of AI by treating AI models as **([Generative AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in enterprise data sources. This abstraction makes AI highly accessible, allowing development teams to create AI-driven applications using their existing skills.
         
-        </h2>
+        <center>
+          
+          <img width="90%" src="https://docs.google.com/drawings/d/e/2PACX-1vR7DCzimVKnIf22CGtKhFryBJKVLn08ZRL56862XxGh_zQQaVQD-0EoMXrvjKqP4ZujHxQAoSgd5jXX/pub?w=1439&h=812" alt="MindsDB">
         
-        ----------------------------------------
-        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        <center>
         
-        ----------------------------------------
+        The data-centric approach of MindsDB AI Logic server brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity and because it'sa server, everything you build on top of mindsdb is automatically ready for production.
         
-        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). 
+        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
         
-        ----------------------------------------
         
-        ## Use cases
+        ----------------------------------------
         
-        Here are some popular use cases you can build with MindsDB:
+        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
         
-        * Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
-        * Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
-        * Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
-        * Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
-        * Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
-        * Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
+        ----------------------------------------
         
-        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
         
         ## Demo
         
         You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
         
         ## Installation
         
@@ -203,129 +200,132 @@
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: grpc
 Provides-Extra: telemetry
+Provides-Extra: grpc
 Provides-Extra: all_extras
-Provides-Extra: empress
-Provides-Extra: solr
-Provides-Extra: access
-Provides-Extra: binance
+Provides-Extra: tdengine
 Provides-Extra: yugabyte
-Provides-Extra: bigquery
-Provides-Extra: timescaledb
-Provides-Extra: github
+Provides-Extra: opengauss
+Provides-Extra: merlion
+Provides-Extra: ignite
+Provides-Extra: lightwood
+Provides-Extra: datastax
+Provides-Extra: informix
+Provides-Extra: huggingface_api
+Provides-Extra: scylla
+Provides-Extra: huggingface
+Provides-Extra: access
+Provides-Extra: frappe
+Provides-Extra: teradata
+Provides-Extra: mlflow
+Provides-Extra: cockroach
+Provides-Extra: confluence
+Provides-Extra: elasticsearch
+Provides-Extra: mariadb
+Provides-Extra: cloud_sql
+Provides-Extra: empress
 Provides-Extra: cohere
-Provides-Extra: snowflake
-Provides-Extra: quickbooks
-Provides-Extra: clickhouse
-Provides-Extra: sendinblue
-Provides-Extra: youtube
-Provides-Extra: monetdb
+Provides-Extra: langchain
+Provides-Extra: mysql
+Provides-Extra: d0lt
+Provides-Extra: sheets
+Provides-Extra: druid
+Provides-Extra: phoenix
+Provides-Extra: planetscale
+Provides-Extra: paypal
+Provides-Extra: web
+Provides-Extra: mediawiki
 Provides-Extra: aurora
-Provides-Extra: s3
-Provides-Extra: autosklearn
+Provides-Extra: realtime_slack_chat
 Provides-Extra: dremio
-Provides-Extra: paypal
-Provides-Extra: rocket_chat
-Provides-Extra: edgelessdb
-Provides-Extra: cockroach
-Provides-Extra: planetscale
-Provides-Extra: google_books
-Provides-Extra: ray_serve
-Provides-Extra: starrocks
-Provides-Extra: huggingface_api
-Provides-Extra: hive
-Provides-Extra: altibase
-Provides-Extra: mariadb
-Provides-Extra: ignite
-Provides-Extra: strava
-Provides-Extra: firebird
 Provides-Extra: tidb
-Provides-Extra: crate
-Provides-Extra: influxdb
+Provides-Extra: jira
+Provides-Extra: redshift
+Provides-Extra: rockset
+Provides-Extra: twitter
+Provides-Extra: bigquery
+Provides-Extra: google_content_shopping
 Provides-Extra: neuralforecast
-Provides-Extra: merlion
-Provides-Extra: vertica
-Provides-Extra: sheets
-Provides-Extra: hana
+Provides-Extra: edgelessdb
+Provides-Extra: db2
+Provides-Extra: cloud_spanner
+Provides-Extra: databend
+Provides-Extra: youtube
+Provides-Extra: postgres
+Provides-Extra: sendinblue
+Provides-Extra: ludwig
+Provides-Extra: tpot
+Provides-Extra: airtable
+Provides-Extra: clickhouse
+Provides-Extra: influxdb
+Provides-Extra: dynamodb
+Provides-Extra: nuo_jdbc
 Provides-Extra: pinot
-Provides-Extra: confluence
-Provides-Extra: opengauss
-Provides-Extra: redshift
+Provides-Extra: matrixone
 Provides-Extra: trino
-Provides-Extra: slack
-Provides-Extra: datastax
+Provides-Extra: monkeylearn
 Provides-Extra: questdb
-Provides-Extra: nuo_jdbc
-Provides-Extra: orioledb
-Provides-Extra: teradata
+Provides-Extra: vitess
+Provides-Extra: llama_index
 Provides-Extra: gmail
-Provides-Extra: oracle
-Provides-Extra: flaml
-Provides-Extra: langchain
+Provides-Extra: openai
+Provides-Extra: cassandra
+Provides-Extra: materialize
+Provides-Extra: quickbooks
 Provides-Extra: impala
-Provides-Extra: cloud_spanner
-Provides-Extra: ingres
-Provides-Extra: tdengine
-Provides-Extra: google_fit
+Provides-Extra: singlestore
 Provides-Extra: google_search
-Provides-Extra: db2
-Provides-Extra: tpot
-Provides-Extra: shopify
-Provides-Extra: google_content_shopping
-Provides-Extra: google_calendar
-Provides-Extra: ckan
-Provides-Extra: cassandra
-Provides-Extra: rockset
-Provides-Extra: monkeylearn
-Provides-Extra: sqlany
+Provides-Extra: duckdb
+Provides-Extra: solr
 Provides-Extra: mssql
-Provides-Extra: huggingface
-Provides-Extra: postgres
-Provides-Extra: ludwig
-Provides-Extra: airtable
-Provides-Extra: mysql
-Provides-Extra: phoenix
-Provides-Extra: singlestore
-Provides-Extra: oceanbase
-Provides-Extra: vitess
-Provides-Extra: newsapi
-Provides-Extra: druid
-Provides-Extra: hsqldb
+Provides-Extra: flaml
+Provides-Extra: github
+Provides-Extra: supabase
 Provides-Extra: statsforecast
-Provides-Extra: materialize
-Provides-Extra: openai
-Provides-Extra: databricks
-Provides-Extra: jira
-Provides-Extra: scylla
-Provides-Extra: twitter
-Provides-Extra: gitlab
-Provides-Extra: surrealdb
-Provides-Extra: plaid
-Provides-Extra: duckdb
-Provides-Extra: d0lt
-Provides-Extra: databend
 Provides-Extra: stripe
+Provides-Extra: ingres
+Provides-Extra: autosklearn
+Provides-Extra: hsqldb
+Provides-Extra: slack
 Provides-Extra: mendeley
-Provides-Extra: maxdb
-Provides-Extra: derby
-Provides-Extra: mlflow
-Provides-Extra: writer
+Provides-Extra: orioledb
+Provides-Extra: gitlab
+Provides-Extra: mongodb
+Provides-Extra: vertica
+Provides-Extra: snowflake
+Provides-Extra: firebird
+Provides-Extra: strava
+Provides-Extra: crate
 Provides-Extra: couchbase
-Provides-Extra: dynamodb
+Provides-Extra: timescaledb
+Provides-Extra: binance
+Provides-Extra: maxdb
+Provides-Extra: s3
+Provides-Extra: shopify
+Provides-Extra: monetdb
 Provides-Extra: sqreamdb
-Provides-Extra: mongodb
-Provides-Extra: cloud_sql
-Provides-Extra: llama_index
-Provides-Extra: supabase
-Provides-Extra: matrixone
-Provides-Extra: informix
-Provides-Extra: elasticsearch
+Provides-Extra: ckan
+Provides-Extra: writer
+Provides-Extra: ray_serve
+Provides-Extra: sqlany
+Provides-Extra: derby
+Provides-Extra: google_calendar
+Provides-Extra: hana
+Provides-Extra: hive
+Provides-Extra: google_books
+Provides-Extra: surrealdb
+Provides-Extra: google_fit
+Provides-Extra: rocket_chat
+Provides-Extra: newsapi
 Provides-Extra: reddit
-Provides-Extra: frappe
-Provides-Extra: lightwood
+Provides-Extra: plaid
+Provides-Extra: databricks
+Provides-Extra: altibase
+Provides-Extra: starrocks
+Provides-Extra: oracle
+Provides-Extra: oceanbase
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.4.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.5.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -12,178 +12,174 @@
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 is a Server for Artificial Intelligence Logic, enabling developers to ship AI
-powered projects from prototyping & experimentation to production in a fast &
+powered systems from prototyping & experimentation to production in a fast &
 scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
 Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-We do this by abstracting Generative AI, Large Language and other Models as a
-virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
-top of enterprise databases. This increases accessibility with organizations
-and enables development teams to use their existing skills to build
-applications powered by AI. By taking a data-centric approach to AI MindsDB
-brings the process closer to the source of the data minimizing the need to
-build and maintain data pipelines and ETLâing, speeding up the time to
-deployment and reducing complexity. **P.S. If you like our open-source project
-we'd appreciate if you star it on GitHub â­!**
-                                    *****
-
-                                [MindsDB] *****
----------------------------------------- MindsDB has an active and helpful
+## What can you build with MindsDB? * **Question Answering**: This is useful
+when you have data (we support more than 120 data sources) and you need answers
+from your data given a question in natural language. * **Semantic Search**:
+Similar to Question Answering, but in this case, you want to retrieve specific
+parts of your data where the answer to a question may exist. * **AI Agent
+serving**: This is useful when you want to publish your AI Agents to enterprise
+conversational applications like Slack, email, Twilio, etc. * **Recommendation
+systems**: When you use your data to help predict, narrow down, and find what
+people are looking for among an exponentially growing number of options. *
+**Time Series Forecasting**: When you want to use your historical data to
+estimate how things will look in the future. * **AI Automation pipelines**:
+When you need your AI systems to consume enterprise data and have the AI output
+stored back into your enterprise tools in an automated way. ## Generative AI
+Tables MindsDB empowers developers to harness the power of AI by treating AI
+models as **([Generative AI Tables](https://www.youtube.com/
+watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in
+enterprise data sources. This abstraction makes AI highly accessible, allowing
+development teams to create AI-driven applications using their existing skills.
+                                   [MindsDB]
+The data-centric approach of MindsDB AI Logic server brings the process closer
+   to the source of the data minimizing the need to build and maintain data
+   pipelines and ETLâing, speeding up the time to deployment and reducing
+complexity and because it'sa server, everything you build on top of mindsdb is
+     automatically ready for production. MindsDB has an active and helpful
 community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
-check-out the [rewards and community programs](https://mindsdb.com/
+      check-out the [rewards and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
----------------------------------------- [Installation](https://github.com/
-mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
-mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
-[Database Integrations](https://github.com/mindsdb/mindsdb#database-
-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
-[Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
-(https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
-github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
-mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------------------- ## Use cases Here are
-some popular use cases you can build with MindsDB: * Conversational AI:
-Leverage MindsDB native integrations with data platforms and pre-trained large
-language models, like OpenAI's GPT, to quickly build conversational AI
-solutions without the overhead of managing complex data pipelines. * Fraud
-Detection: MindsDB can help developers build models to detect fraudulent
-activity in financial transactions, eCommerce platforms etc. * Sales
-Forecasting: MindsDB can be used to develop models to predict future sales
-based on historical sales data, allowing businesses to make better-informed
-decisions. * Customer Segmentation: MindsDB can help developers segment
-customers based on their behavior, preferences, and other factors, allowing
-businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
-native integration with pre-trained models like OpenAI GPT or Hugging Face can
-be used to analyze the sentiment of a text data, such as a customer reviews -
-in a single command, instead of individual API calls and ETL-ing data. *
-Predictive Maintenance: MindsDB can be used to build models to predict when
-equipment or machinery is likely to fail, allowing for proactive maintenance
-and minimizing downtime. See more examples and community tutorials [here]
-(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
-[demo environment](https://cloud.mindsdb.com/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
+ **P.S. If you like our open-source project we'd appreciate if you star it on
+GitHub â­!** ---------------------------------------- [Installation](https://
+   github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/
+      mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/
+    mindsdb#features) - [Database Integrations](https://github.com/mindsdb/
+   mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/
+       mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/
+mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support)
+ - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing
+ lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://
+github.com/mindsdb/mindsdb#license) ---------------------------------------- ##
+        Demo You can try MindsDB using our [demo environment](https://
+                              cloud.mindsdb.com/
+   ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
-[dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
-production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
-premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
-platforms and this list is constantly growing. If you canât find the
+ [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
+ production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
+  profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
+ premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
+  How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+    platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. CREATE MODEL to connect the AI Engine you pick that will learn from your
-data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
-you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
-[docs](https://docs.mindsdb.com/sql/create/
-model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+  2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+ data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+  1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+ (https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+ you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+                  [docs](https://docs.mindsdb.com/sql/create/
+ model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
 you want to have manual control over model engineering. 3. JOIN such model with
 your database tables to make predictions for thousands or even millions of data
-points at once, or run SELECT statements or API calls to make one time
+    points at once, or run SELECT statements or API calls to make one time
 predictions. 4. Set up a JOB to automate your re-training cycle and predictions
-pipelines for the new incoming data. 5. Alternatively, use REST API to query
-the models Follow the [quickstart guide](https://docs.mindsdb.com/
+ pipelines for the new incoming data. 5. Alternatively, use REST API to query
+      the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-with sample data to get on-boarded as fast as possible. ## Database
+      with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
-and popular applications. | Connect your Data | Connect your Data | Connect
-your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
-Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
-[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+  and popular applications. | Connect your Data | Connect your Data | Connect
+   your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+  Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+     [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
-[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+   [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+   Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
-| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+  | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
 ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
-| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
-Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
-integration?](https://github.com/mindsdb/mindsdb/issues/
+ | [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+   Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+           integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
-//
+                                      //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-## Support If you found a bug, please submit an [issue on GitHub](https://
-github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+  ## Support If you found a bug, please submit an [issue on GitHub](https://
+ github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
+   can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
 joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
-mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
-stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
-commercial support, please [contact](https://mindsdb.com/contact/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
-team. ## Contributing A great place to start contributing to MindsDB is to
+  mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+  stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+       commercial support, please [contact](https://mindsdb.com/contact/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
+  team. ## Contributing A great place to start contributing to MindsDB is to
 check our GitHub projects :checkered_flag: * Community contributor's [dashboard
-tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
-issues](https://github.com/mindsdb/mindsdb/
+  tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+                  issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
-so feel free to open new issues with your ideas and we can guide you! Being
+  so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
-[contributing documentation](https://docs.mindsdb.com/contribute/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
+       [contributing documentation](https://docs.mindsdb.com/contribute/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
 note that this project is released with a [Contributor Code of Conduct](https:/
-/github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
+ /github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
 in this project, you agree to abide by its terms. Also, check out the [rewards
-and community programs](https://mindsdb.com/
+                 and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ### Current contributors [https://contributors-img.web.app/image?repo=mindsdb/
-mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
-Subscribe to updates Join our [Slack community](https://mindsdb.com/
-joincommunity) and subscribe to the monthly [Developer Newsletter](https://
-mindsdb.com/newsletter/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
-product updates, information about MindsDB events and contests, and useful
-content, like tutorials. ## License MindsDB is licensed under [GNU General
-Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+  mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
+     Subscribe to updates Join our [Slack community](https://mindsdb.com/
+  joincommunity) and subscribe to the monthly [Developer Newsletter](https://
+                            mindsdb.com/newsletter/
+  ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
+  product updates, information about MindsDB events and contests, and useful
+  content, like tutorials. ## License MindsDB is licensed under [GNU General
+ Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+ Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
-Extra: all_extras Provides-Extra: empress Provides-Extra: solr Provides-Extra:
-access Provides-Extra: binance Provides-Extra: yugabyte Provides-Extra:
-bigquery Provides-Extra: timescaledb Provides-Extra: github Provides-Extra:
-cohere Provides-Extra: snowflake Provides-Extra: quickbooks Provides-Extra:
-clickhouse Provides-Extra: sendinblue Provides-Extra: youtube Provides-Extra:
-monetdb Provides-Extra: aurora Provides-Extra: s3 Provides-Extra: autosklearn
-Provides-Extra: dremio Provides-Extra: paypal Provides-Extra: rocket_chat
-Provides-Extra: edgelessdb Provides-Extra: cockroach Provides-Extra:
-planetscale Provides-Extra: google_books Provides-Extra: ray_serve Provides-
-Extra: starrocks Provides-Extra: huggingface_api Provides-Extra: hive Provides-
-Extra: altibase Provides-Extra: mariadb Provides-Extra: ignite Provides-Extra:
-strava Provides-Extra: firebird Provides-Extra: tidb Provides-Extra: crate
-Provides-Extra: influxdb Provides-Extra: neuralforecast Provides-Extra: merlion
-Provides-Extra: vertica Provides-Extra: sheets Provides-Extra: hana Provides-
-Extra: pinot Provides-Extra: confluence Provides-Extra: opengauss Provides-
-Extra: redshift Provides-Extra: trino Provides-Extra: slack Provides-Extra:
-datastax Provides-Extra: questdb Provides-Extra: nuo_jdbc Provides-Extra:
-orioledb Provides-Extra: teradata Provides-Extra: gmail Provides-Extra: oracle
-Provides-Extra: flaml Provides-Extra: langchain Provides-Extra: impala
-Provides-Extra: cloud_spanner Provides-Extra: ingres Provides-Extra: tdengine
-Provides-Extra: google_fit Provides-Extra: google_search Provides-Extra: db2
-Provides-Extra: tpot Provides-Extra: shopify Provides-Extra:
-google_content_shopping Provides-Extra: google_calendar Provides-Extra: ckan
-Provides-Extra: cassandra Provides-Extra: rockset Provides-Extra: monkeylearn
-Provides-Extra: sqlany Provides-Extra: mssql Provides-Extra: huggingface
-Provides-Extra: postgres Provides-Extra: ludwig Provides-Extra: airtable
-Provides-Extra: mysql Provides-Extra: phoenix Provides-Extra: singlestore
-Provides-Extra: oceanbase Provides-Extra: vitess Provides-Extra: newsapi
-Provides-Extra: druid Provides-Extra: hsqldb Provides-Extra: statsforecast
-Provides-Extra: materialize Provides-Extra: openai Provides-Extra: databricks
-Provides-Extra: jira Provides-Extra: scylla Provides-Extra: twitter Provides-
-Extra: gitlab Provides-Extra: surrealdb Provides-Extra: plaid Provides-Extra:
-duckdb Provides-Extra: d0lt Provides-Extra: databend Provides-Extra: stripe
-Provides-Extra: mendeley Provides-Extra: maxdb Provides-Extra: derby Provides-
-Extra: mlflow Provides-Extra: writer Provides-Extra: couchbase Provides-Extra:
-dynamodb Provides-Extra: sqreamdb Provides-Extra: mongodb Provides-Extra:
-cloud_sql Provides-Extra: llama_index Provides-Extra: supabase Provides-Extra:
-matrixone Provides-Extra: informix Provides-Extra: elasticsearch Provides-
-Extra: reddit Provides-Extra: frappe Provides-Extra: lightwood Provides-Extra:
-all_handlers_extras
+ Type: text/markdown Provides-Extra: telemetry Provides-Extra: grpc Provides-
+ Extra: all_extras Provides-Extra: tdengine Provides-Extra: yugabyte Provides-
+Extra: opengauss Provides-Extra: merlion Provides-Extra: ignite Provides-Extra:
+  lightwood Provides-Extra: datastax Provides-Extra: informix Provides-Extra:
+ huggingface_api Provides-Extra: scylla Provides-Extra: huggingface Provides-
+ Extra: access Provides-Extra: frappe Provides-Extra: teradata Provides-Extra:
+  mlflow Provides-Extra: cockroach Provides-Extra: confluence Provides-Extra:
+elasticsearch Provides-Extra: mariadb Provides-Extra: cloud_sql Provides-Extra:
+empress Provides-Extra: cohere Provides-Extra: langchain Provides-Extra: mysql
+  Provides-Extra: d0lt Provides-Extra: sheets Provides-Extra: druid Provides-
+  Extra: phoenix Provides-Extra: planetscale Provides-Extra: paypal Provides-
+  Extra: web Provides-Extra: mediawiki Provides-Extra: aurora Provides-Extra:
+realtime_slack_chat Provides-Extra: dremio Provides-Extra: tidb Provides-Extra:
+ jira Provides-Extra: redshift Provides-Extra: rockset Provides-Extra: twitter
+  Provides-Extra: bigquery Provides-Extra: google_content_shopping Provides-
+Extra: neuralforecast Provides-Extra: edgelessdb Provides-Extra: db2 Provides-
+Extra: cloud_spanner Provides-Extra: databend Provides-Extra: youtube Provides-
+  Extra: postgres Provides-Extra: sendinblue Provides-Extra: ludwig Provides-
+Extra: tpot Provides-Extra: airtable Provides-Extra: clickhouse Provides-Extra:
+  influxdb Provides-Extra: dynamodb Provides-Extra: nuo_jdbc Provides-Extra:
+     pinot Provides-Extra: matrixone Provides-Extra: trino Provides-Extra:
+  monkeylearn Provides-Extra: questdb Provides-Extra: vitess Provides-Extra:
+   llama_index Provides-Extra: gmail Provides-Extra: openai Provides-Extra:
+  cassandra Provides-Extra: materialize Provides-Extra: quickbooks Provides-
+    Extra: impala Provides-Extra: singlestore Provides-Extra: google_search
+  Provides-Extra: duckdb Provides-Extra: solr Provides-Extra: mssql Provides-
+ Extra: flaml Provides-Extra: github Provides-Extra: supabase Provides-Extra:
+  statsforecast Provides-Extra: stripe Provides-Extra: ingres Provides-Extra:
+   autosklearn Provides-Extra: hsqldb Provides-Extra: slack Provides-Extra:
+   mendeley Provides-Extra: orioledb Provides-Extra: gitlab Provides-Extra:
+   mongodb Provides-Extra: vertica Provides-Extra: snowflake Provides-Extra:
+firebird Provides-Extra: strava Provides-Extra: crate Provides-Extra: couchbase
+   Provides-Extra: timescaledb Provides-Extra: binance Provides-Extra: maxdb
+ Provides-Extra: s3 Provides-Extra: shopify Provides-Extra: monetdb Provides-
+  Extra: sqreamdb Provides-Extra: ckan Provides-Extra: writer Provides-Extra:
+    ray_serve Provides-Extra: sqlany Provides-Extra: derby Provides-Extra:
+   google_calendar Provides-Extra: hana Provides-Extra: hive Provides-Extra:
+  google_books Provides-Extra: surrealdb Provides-Extra: google_fit Provides-
+  Extra: rocket_chat Provides-Extra: newsapi Provides-Extra: reddit Provides-
+  Extra: plaid Provides-Extra: databricks Provides-Extra: altibase Provides-
+  Extra: starrocks Provides-Extra: oracle Provides-Extra: oceanbase Provides-
+                          Extra: all_handlers_extras
```

### Comparing `MindsDB-23.6.4.0/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.6.5.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 mindsdb/api/http/gunicorn_wrapper.py
 mindsdb/api/http/initialize.py
 mindsdb/api/http/start.py
 mindsdb/api/http/utils.py
 mindsdb/api/http/namespaces/__init__.py
 mindsdb/api/http/namespaces/analysis.py
 mindsdb/api/http/namespaces/auth.py
+mindsdb/api/http/namespaces/chatbots.py
 mindsdb/api/http/namespaces/config.py
 mindsdb/api/http/namespaces/databases.py
 mindsdb/api/http/namespaces/default.py
 mindsdb/api/http/namespaces/file.py
 mindsdb/api/http/namespaces/handlers.py
 mindsdb/api/http/namespaces/models.py
 mindsdb/api/http/namespaces/projects.py
@@ -33,14 +34,15 @@
 mindsdb/api/http/namespaces/tab.py
 mindsdb/api/http/namespaces/tree.py
 mindsdb/api/http/namespaces/util.py
 mindsdb/api/http/namespaces/views.py
 mindsdb/api/http/namespaces/configs/__init__.py
 mindsdb/api/http/namespaces/configs/analysis.py
 mindsdb/api/http/namespaces/configs/auth.py
+mindsdb/api/http/namespaces/configs/chatbots.py
 mindsdb/api/http/namespaces/configs/config.py
 mindsdb/api/http/namespaces/configs/databases.py
 mindsdb/api/http/namespaces/configs/default.py
 mindsdb/api/http/namespaces/configs/files.py
 mindsdb/api/http/namespaces/configs/handlers.py
 mindsdb/api/http/namespaces/configs/projects.py
 mindsdb/api/http/namespaces/configs/sql.py
@@ -601,14 +603,20 @@
 mindsdb/integrations/handlers/maxdb_handler/__about__.py
 mindsdb/integrations/handlers/maxdb_handler/__init__.py
 mindsdb/integrations/handlers/maxdb_handler/icon.png
 mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
 mindsdb/integrations/handlers/maxdb_handler/requirements.txt
 mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
 mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+mindsdb/integrations/handlers/mediawiki_handler/icon.png
+mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
 mindsdb/integrations/handlers/mendeley_handler/__about__.py
 mindsdb/integrations/handlers/mendeley_handler/__init__.py
 mindsdb/integrations/handlers/mendeley_handler/icon.svg
 mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
 mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
 mindsdb/integrations/handlers/mendeley_handler/requirements.txt
 mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
@@ -767,14 +775,15 @@
 mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
 mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
 mindsdb/integrations/handlers/ray_serve_handler/__about__.py
 mindsdb/integrations/handlers/ray_serve_handler/__init__.py
 mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
 mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
 mindsdb/integrations/handlers/ray_serve_handler/setup.py
+mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
 mindsdb/integrations/handlers/reddit_handler/__about__.py
 mindsdb/integrations/handlers/reddit_handler/__init__.py
 mindsdb/integrations/handlers/reddit_handler/icon.svg
 mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
 mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
 mindsdb/integrations/handlers/reddit_handler/requirements.txt
 mindsdb/integrations/handlers/redshift_handler/__about__.py
@@ -972,14 +981,20 @@
 mindsdb/integrations/handlers/vitess_handler/__about__.py
 mindsdb/integrations/handlers/vitess_handler/__init__.py
 mindsdb/integrations/handlers/vitess_handler/icon.svg
 mindsdb/integrations/handlers/vitess_handler/requirements.txt
 mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
 mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
 mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+mindsdb/integrations/handlers/web_handler/__about__.py
+mindsdb/integrations/handlers/web_handler/__init__.py
+mindsdb/integrations/handlers/web_handler/icon.png
+mindsdb/integrations/handlers/web_handler/requirements.txt
+mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+mindsdb/integrations/handlers/web_handler/web_handler.py
 mindsdb/integrations/handlers/writer_handler/__about__.py
 mindsdb/integrations/handlers/writer_handler/__init__.py
 mindsdb/integrations/handlers/writer_handler/ingest.py
 mindsdb/integrations/handlers/writer_handler/question_answer.py
 mindsdb/integrations/handlers/writer_handler/requirements.txt
 mindsdb/integrations/handlers/writer_handler/settings.py
 mindsdb/integrations/handlers/writer_handler/setup.py
@@ -1011,29 +1026,36 @@
 mindsdb/integrations/libs/api_handler.py
 mindsdb/integrations/libs/base.py
 mindsdb/integrations/libs/const.py
 mindsdb/integrations/libs/handler_helpers.py
 mindsdb/integrations/libs/ml_exec_base.py
 mindsdb/integrations/libs/ml_handler_proc.py
 mindsdb/integrations/libs/net_helpers.py
+mindsdb/integrations/libs/realtime_chat_handler.py
 mindsdb/integrations/libs/response.py
 mindsdb/integrations/libs/storage_handler.py
 mindsdb/integrations/utilities/__init__.py
 mindsdb/integrations/utilities/date_utils.py
 mindsdb/integrations/utilities/install.py
 mindsdb/integrations/utilities/processes.py
 mindsdb/integrations/utilities/sql_utils.py
 mindsdb/integrations/utilities/test_utils.py
 mindsdb/integrations/utilities/time_series_utils.py
 mindsdb/integrations/utilities/utils.py
 mindsdb/interfaces/__init__.py
 mindsdb/interfaces/chatbot/__init__.py
 mindsdb/interfaces/chatbot/chatbot_controller.py
+mindsdb/interfaces/chatbot/chatbot_message.py
 mindsdb/interfaces/chatbot/chatbot_monitor.py
+mindsdb/interfaces/chatbot/chatbot_response.py
 mindsdb/interfaces/chatbot/chatbot_task.py
+mindsdb/interfaces/chatbot/chatbot_thread.py
+mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
+mindsdb/interfaces/chatbot/realtime_chatbot_task.py
+mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
 mindsdb/interfaces/database/__init__.py
 mindsdb/interfaces/database/database.py
 mindsdb/interfaces/database/integrations.py
 mindsdb/interfaces/database/projects.py
 mindsdb/interfaces/database/views.py
 mindsdb/interfaces/file/__init__.py
 mindsdb/interfaces/file/file_controller.py
@@ -1092,14 +1114,16 @@
 mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
 mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
 mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
 mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
 mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
 mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
 mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
 mindsdb/migrations/versions/__init__.py
 mindsdb/utilities/__init__.py
 mindsdb/utilities/auth.py
 mindsdb/utilities/cache.py
 mindsdb/utilities/config.py
 mindsdb/utilities/context.py
 mindsdb/utilities/fs.py
```

### Comparing `MindsDB-23.6.4.0/MindsDB.egg-info/requires.txt` & `MindsDB-23.6.5.0/MindsDB.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,174 +29,181 @@
 clickhouse-sqlalchemy
 charset-normalizer
 dill>=0.3.4
 pyOpenSSL>=22.0.0
 pydateinfer==0.3.0
 pyarrow<10.1.0,>=10.0.1
 dataprep_ml
-grpcio-tools
 python-magic>=0.4.27
 openpyxl>=3.1.1
+slack_sdk
 
 [access]
 pyodbc
 sqlalchemy-access
 
 [airtable]
 duckdb
 
 [all_extras]
-sentry-sdk
 grpcio-tools
+sentry-sdk
 
 [all_handlers_extras]
-snowflake-connector-python>=2.7.12
-python-gitlab
-ibm-db-sa
-elasticsearch
-pydruid
-tqdm
-jaydebeapi
-websocket
-auto-sklearn
+mindsdb_sql>=0.4.0
+pandas
+neuralforecast<1.5.0,>=1.4.0
+pinotdb
+statsforecast<2.0,>=1.4.0
+pymonetdb
+html2text
 stravalib
-teradatasqlalchemy
-pymysql
-google
-mindsdb_sql<0.5.0,>=0.4.6
-duckdb
-rockset
+tensorflow
+pyphoenix
+elasticsearch
 mindsdb>=22.7.5.0
-ShopifyAPI
-fdb
+teradatasql
+ibm-db
+ibm-db-sa
+sqlalchemy-access
+rockset
+pymongo[srv]>=4.1.1
 sqlalchemy-informix
-sqlalchemy_dremio
-tensorflow
+pyHive
+monkeylearn==3.6.0
+taospy
+hyperopt
+wikipedia==1.4.0
+couchbase==4.0.2
+snowflake-sqlalchemy>=1.4.3
 paypalrestsdk
-hierarchicalforecast<1.0
-newsapi-python
-lightwood[all_extras]>=22.8.1.0
-pyodbc
 pyodbc==4.0.34
-elasticsearch-dbapi
-couchbase==4.0.2
-IfxPy
-neuralforecast<1.5.0,>=1.4.0
-torch
-flaml<=1.2.3
-pysurrealdb
-langchain==0.0.186
-sib_api_v3_sdk
+plaid-python
+slack_sdk
+stripe
+openai<=0.28.0
+sqlalchemy<2.0.0
 pysqream>=3.2.5
-sentencepiece==0.1.97
-dill
-mlflow
-html2text
-transformers==4.21.0
-boto3
-ckanapi
-mysql-connector-python
-dask
-thrift
-sqlalchemy-access
-databricks-sql-connector
-statsforecast<2.0,>=1.4.0
-hugging_py_face
-rocketchat_API
+teradatasqlalchemy
+llama-index==0.6.11
+sqlalchemy_dremio
+mindsdb-evaluator>=0.0.6
+python-gitlab
 db-dtypes
-mendeley
-salesforce-merlion<=1.3.1,>=1.2.0
-psycopg2
-sqlalchemy-solr
-hyperopt
-sqlalchemy-bigquery
-google-auth-oauthlib
-cohere==4.5.1
-mindsdb>=23.3.5.0
-praw
-openai>=0.27.0
+duckdb==0.7.1
+ckanapi
+hyperopt<1.0
+phoenixdb
+pymssql>=2.1.4
+boto3
+pymysql
+snowflake-connector-python>=2.7.12
+elasticsearch-dbapi
+google-cloud-spanner
 sqlalchemy
-ibm-db
-mindsdb>=22.10.2.1
-mindsdb>=22.12.4.3
-mindsdb_sql<0.5.0,>=0.4.9
-duckdb==0.7.1.dev187
+ray[serve]
 sasl
-impyla
-mindsdb>=23.3.2.0
-sqlalchemy-hana
-trino~=0.313.0
-oracledb==1.0.2
-binance-connector
-psycopg
-pydantic==1.10.8
+ludwig[distributed]>=0.5.2
 requests-kerberos==0.12.0
-pyphoenix
-sentence_transformers
-ray[serve]
-scylla-driver
-crate[sqlalchemy]
-ingres_sa_dialect==0.3
-pinotdb
-psycopg[binary]
-openai==0.27.0
-teradatasql
 clickhouse-sqlalchemy
-pygithub
-pandas<=1.4.3
-qbosdk
-google-api-python-client
-sqlalchemy-databricks
+binance-connector
+protobuf==3.20.*
+langchain<=0.0.192
+rocketchat_API
+tweepy
+mysql-connector-python
+pyodbc
 mindsdb>=22.6.2.1
-pandas
-sqlalchemy<2.0.0
+sqlalchemy-redshift
+salesforce-merlion<=1.3.1,>=1.2.0
+lightwood[all_extras]>=22.8.1.0
+thrift-sasl
+websocket
+tqdm
 pytz
-google-cloud-bigquery
+impyla
+dask
 tzlocal
-langchain<=0.0.192
-tiktoken>=0.3.0
-thrift-sasl
-sqlalchemy-sqlany
-plaid-python
-mindsdb-evaluator>=0.0.6
-hyperopt<1.0
+pyignite
+langchain==0.0.186
 certifi
-mindsdb_sql<0.5.0,>=0.4.4
-tweepy
-google-auth-httplib2
-protobuf==3.20.*
-snowflake-sqlalchemy>=1.4.3
-ray<=1.13.0
-wikipedia==1.4.0
-redshift_connector
-google-cloud-spanner
-sqlalchemy-redshift
-phoenixdb
-pymongo[srv]>=4.1.1
-mindsdb_sql>=0.4.0
-openai<=0.28.0
+hierarchicalforecast<1.0
+tiktoken>=0.3.0
+sqlanydb
+tpot<=0.11.7
+sib_api_v3_sdk
 hdbcli
-pyHive
-sqlalchemy-monetdb
-pyignite
-pymssql>=2.1.4
-ludwig[distributed]>=0.5.2
+dill
+sqlalchemy-databricks
+google-api-python-client
+pygithub
+openai>=0.27.0
+mediawikiapi
+mindsdb>=22.12.4.3
+ShopifyAPI
+google-cloud-bigquery
+mendeley
+oracledb==1.0.2
 atlassian-python-api
+fdb
+google-auth-oauthlib
+crate[sqlalchemy]
+mindsdb>=22.10.2.1
 pysqream_sqlalchemy>=0.8
-monkeylearn==3.6.0
-tpot<=0.11.7
-pymonetdb
-llama-index==0.6.11
-taospy
-sqlalchemy-vertica-python
+sentence_transformers
+sentencepiece==0.1.97
+praw
+transformers==4.21.0
+ray<=1.13.0
+pandas<=1.4.3
+sqlalchemy-hana
+redshift_connector
+hugging_py_face
+sqlalchemy-bigquery
+sqlalchemy-monetdb
+sqlalchemy-sqlany
+pysurrealdb
+duckdb==0.7.1.dev187
 pyhive
-stripe
+auto-sklearn
+requests==2.28.0
+torch
+pydruid
+jaydebeapi
+sqlalchemy-vertica-python
+google
+psycopg2
 vertica-python
-slack_sdk
-sqlanydb
+IfxPy
+psycopg
+openai==0.27.0
+mindsdb_sql<0.5.0,>=0.4.6
+google-auth-httplib2
+databricks-sql-connector
+psycopg[binary]
+trino~=0.313.0
+mlflow
+thrift
+bs4
+newsapi-python
+duckdb
+qbosdk
+mindsdb>=23.3.5.0
+chromadb==0.3.25
+pydantic==1.10.8
+flaml<=1.2.3
+mindsdb>=23.3.2.0
+cohere==4.5.1
+SQLAlchemy
+scylla-driver
+ingres_sa_dialect==0.3
+markupsafe==2.0.1
+mindsdb_sql<0.5.0,>=0.4.9
+sqlalchemy-solr
+mindsdb_sql<0.5.0,>=0.4.4
 
 [altibase]
 jaydebeapi
 
 [aurora]
 psycopg[binary]
 mysql-connector-python
@@ -421,14 +428,17 @@
 
 [matrixone]
 pymysql
 
 [maxdb]
 jaydebeapi
 
+[mediawiki]
+mediawikiapi
+
 [mendeley]
 mendeley
 
 [merlion]
 mindsdb>=22.6.2.1
 mindsdb_sql>=0.4.0
 pandas<=1.4.3
@@ -512,14 +522,17 @@
 [quickbooks]
 qbosdk
 
 [ray_serve]
 ray[serve]
 mindsdb>=23.3.5.0
 
+[realtime_slack_chat]
+slack_sdk
+
 [reddit]
 praw
 
 [redshift]
 redshift_connector
 sqlalchemy-redshift
 
@@ -617,17 +630,25 @@
 [vertica]
 vertica-python
 sqlalchemy-vertica-python
 
 [vitess]
 mysql-connector-python
 
+[web]
+bs4
+
 [writer]
 langchain==0.0.186
+SQLAlchemy
+duckdb==0.7.1
+chromadb==0.3.25
+requests==2.28.0
 pydantic==1.10.8
 sentence_transformers
+markupsafe==2.0.1
 
 [youtube]
 google-api-python-client
 
 [yugabyte]
 psycopg
```

### Comparing `MindsDB-23.6.4.0/PKG-INFO` & `MindsDB-23.6.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.4.0
+Version: 23.6.5.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -57,50 +57,47 @@
         	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
         </h3>
         
         </div>
         
         ----------------------------------------
         
-        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered systems from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
         
-        We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
+        ## What can you build with MindsDB?
         
-        By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
+        * **Question Answering**: This is useful when you have data (we support more than 120 data sources) and you need answers from your data given a question in natural language.
+        * **Semantic Search**: Similar to Question Answering, but in this case, you want to retrieve specific parts of your data where the answer to a question may exist.
+        * **AI Agent serving**: This is useful when you want to publish your AI Agents to enterprise conversational applications like Slack, email, Twilio, etc.
+        * **Recommendation systems**: When you use your data to help predict, narrow down, and find what people are looking for among an exponentially growing number of options.
+        * **Time Series Forecasting**: When you want to use your historical data to estimate how things will look in the future.
+        * **AI Automation pipelines**: When you need your AI systems to consume enterprise data and have the AI output stored back into your enterprise tools in an automated way.
         
-        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
+        ## Generative AI Tables
         
-        <h2 align="center">
-           <br/>
-           <br/>
-          <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
+        MindsDB empowers developers to harness the power of AI by treating AI models as **([Generative AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in enterprise data sources. This abstraction makes AI highly accessible, allowing development teams to create AI-driven applications using their existing skills.
         
-        </h2>
+        <center>
+          
+          <img width="90%" src="https://docs.google.com/drawings/d/e/2PACX-1vR7DCzimVKnIf22CGtKhFryBJKVLn08ZRL56862XxGh_zQQaVQD-0EoMXrvjKqP4ZujHxQAoSgd5jXX/pub?w=1439&h=812" alt="MindsDB">
         
-        ----------------------------------------
-        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        <center>
         
-        ----------------------------------------
+        The data-centric approach of MindsDB AI Logic server brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity and because it'sa server, everything you build on top of mindsdb is automatically ready for production.
         
-        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). 
+        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
         
-        ----------------------------------------
         
-        ## Use cases
+        ----------------------------------------
         
-        Here are some popular use cases you can build with MindsDB:
+        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
         
-        * Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
-        * Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
-        * Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
-        * Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
-        * Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
-        * Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
+        ----------------------------------------
         
-        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
         
         ## Demo
         
         You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
         
         ## Installation
         
@@ -203,129 +200,132 @@
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: grpc
 Provides-Extra: telemetry
+Provides-Extra: grpc
 Provides-Extra: all_extras
-Provides-Extra: empress
-Provides-Extra: solr
-Provides-Extra: access
-Provides-Extra: binance
+Provides-Extra: tdengine
 Provides-Extra: yugabyte
-Provides-Extra: bigquery
-Provides-Extra: timescaledb
-Provides-Extra: github
+Provides-Extra: opengauss
+Provides-Extra: merlion
+Provides-Extra: ignite
+Provides-Extra: lightwood
+Provides-Extra: datastax
+Provides-Extra: informix
+Provides-Extra: huggingface_api
+Provides-Extra: scylla
+Provides-Extra: huggingface
+Provides-Extra: access
+Provides-Extra: frappe
+Provides-Extra: teradata
+Provides-Extra: mlflow
+Provides-Extra: cockroach
+Provides-Extra: confluence
+Provides-Extra: elasticsearch
+Provides-Extra: mariadb
+Provides-Extra: cloud_sql
+Provides-Extra: empress
 Provides-Extra: cohere
-Provides-Extra: snowflake
-Provides-Extra: quickbooks
-Provides-Extra: clickhouse
-Provides-Extra: sendinblue
-Provides-Extra: youtube
-Provides-Extra: monetdb
+Provides-Extra: langchain
+Provides-Extra: mysql
+Provides-Extra: d0lt
+Provides-Extra: sheets
+Provides-Extra: druid
+Provides-Extra: phoenix
+Provides-Extra: planetscale
+Provides-Extra: paypal
+Provides-Extra: web
+Provides-Extra: mediawiki
 Provides-Extra: aurora
-Provides-Extra: s3
-Provides-Extra: autosklearn
+Provides-Extra: realtime_slack_chat
 Provides-Extra: dremio
-Provides-Extra: paypal
-Provides-Extra: rocket_chat
-Provides-Extra: edgelessdb
-Provides-Extra: cockroach
-Provides-Extra: planetscale
-Provides-Extra: google_books
-Provides-Extra: ray_serve
-Provides-Extra: starrocks
-Provides-Extra: huggingface_api
-Provides-Extra: hive
-Provides-Extra: altibase
-Provides-Extra: mariadb
-Provides-Extra: ignite
-Provides-Extra: strava
-Provides-Extra: firebird
 Provides-Extra: tidb
-Provides-Extra: crate
-Provides-Extra: influxdb
+Provides-Extra: jira
+Provides-Extra: redshift
+Provides-Extra: rockset
+Provides-Extra: twitter
+Provides-Extra: bigquery
+Provides-Extra: google_content_shopping
 Provides-Extra: neuralforecast
-Provides-Extra: merlion
-Provides-Extra: vertica
-Provides-Extra: sheets
-Provides-Extra: hana
+Provides-Extra: edgelessdb
+Provides-Extra: db2
+Provides-Extra: cloud_spanner
+Provides-Extra: databend
+Provides-Extra: youtube
+Provides-Extra: postgres
+Provides-Extra: sendinblue
+Provides-Extra: ludwig
+Provides-Extra: tpot
+Provides-Extra: airtable
+Provides-Extra: clickhouse
+Provides-Extra: influxdb
+Provides-Extra: dynamodb
+Provides-Extra: nuo_jdbc
 Provides-Extra: pinot
-Provides-Extra: confluence
-Provides-Extra: opengauss
-Provides-Extra: redshift
+Provides-Extra: matrixone
 Provides-Extra: trino
-Provides-Extra: slack
-Provides-Extra: datastax
+Provides-Extra: monkeylearn
 Provides-Extra: questdb
-Provides-Extra: nuo_jdbc
-Provides-Extra: orioledb
-Provides-Extra: teradata
+Provides-Extra: vitess
+Provides-Extra: llama_index
 Provides-Extra: gmail
-Provides-Extra: oracle
-Provides-Extra: flaml
-Provides-Extra: langchain
+Provides-Extra: openai
+Provides-Extra: cassandra
+Provides-Extra: materialize
+Provides-Extra: quickbooks
 Provides-Extra: impala
-Provides-Extra: cloud_spanner
-Provides-Extra: ingres
-Provides-Extra: tdengine
-Provides-Extra: google_fit
+Provides-Extra: singlestore
 Provides-Extra: google_search
-Provides-Extra: db2
-Provides-Extra: tpot
-Provides-Extra: shopify
-Provides-Extra: google_content_shopping
-Provides-Extra: google_calendar
-Provides-Extra: ckan
-Provides-Extra: cassandra
-Provides-Extra: rockset
-Provides-Extra: monkeylearn
-Provides-Extra: sqlany
+Provides-Extra: duckdb
+Provides-Extra: solr
 Provides-Extra: mssql
-Provides-Extra: huggingface
-Provides-Extra: postgres
-Provides-Extra: ludwig
-Provides-Extra: airtable
-Provides-Extra: mysql
-Provides-Extra: phoenix
-Provides-Extra: singlestore
-Provides-Extra: oceanbase
-Provides-Extra: vitess
-Provides-Extra: newsapi
-Provides-Extra: druid
-Provides-Extra: hsqldb
+Provides-Extra: flaml
+Provides-Extra: github
+Provides-Extra: supabase
 Provides-Extra: statsforecast
-Provides-Extra: materialize
-Provides-Extra: openai
-Provides-Extra: databricks
-Provides-Extra: jira
-Provides-Extra: scylla
-Provides-Extra: twitter
-Provides-Extra: gitlab
-Provides-Extra: surrealdb
-Provides-Extra: plaid
-Provides-Extra: duckdb
-Provides-Extra: d0lt
-Provides-Extra: databend
 Provides-Extra: stripe
+Provides-Extra: ingres
+Provides-Extra: autosklearn
+Provides-Extra: hsqldb
+Provides-Extra: slack
 Provides-Extra: mendeley
-Provides-Extra: maxdb
-Provides-Extra: derby
-Provides-Extra: mlflow
-Provides-Extra: writer
+Provides-Extra: orioledb
+Provides-Extra: gitlab
+Provides-Extra: mongodb
+Provides-Extra: vertica
+Provides-Extra: snowflake
+Provides-Extra: firebird
+Provides-Extra: strava
+Provides-Extra: crate
 Provides-Extra: couchbase
-Provides-Extra: dynamodb
+Provides-Extra: timescaledb
+Provides-Extra: binance
+Provides-Extra: maxdb
+Provides-Extra: s3
+Provides-Extra: shopify
+Provides-Extra: monetdb
 Provides-Extra: sqreamdb
-Provides-Extra: mongodb
-Provides-Extra: cloud_sql
-Provides-Extra: llama_index
-Provides-Extra: supabase
-Provides-Extra: matrixone
-Provides-Extra: informix
-Provides-Extra: elasticsearch
+Provides-Extra: ckan
+Provides-Extra: writer
+Provides-Extra: ray_serve
+Provides-Extra: sqlany
+Provides-Extra: derby
+Provides-Extra: google_calendar
+Provides-Extra: hana
+Provides-Extra: hive
+Provides-Extra: google_books
+Provides-Extra: surrealdb
+Provides-Extra: google_fit
+Provides-Extra: rocket_chat
+Provides-Extra: newsapi
 Provides-Extra: reddit
-Provides-Extra: frappe
-Provides-Extra: lightwood
+Provides-Extra: plaid
+Provides-Extra: databricks
+Provides-Extra: altibase
+Provides-Extra: starrocks
+Provides-Extra: oracle
+Provides-Extra: oceanbase
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.4.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.5.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -12,178 +12,174 @@
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 is a Server for Artificial Intelligence Logic, enabling developers to ship AI
-powered projects from prototyping & experimentation to production in a fast &
+powered systems from prototyping & experimentation to production in a fast &
 scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
 Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-We do this by abstracting Generative AI, Large Language and other Models as a
-virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
-top of enterprise databases. This increases accessibility with organizations
-and enables development teams to use their existing skills to build
-applications powered by AI. By taking a data-centric approach to AI MindsDB
-brings the process closer to the source of the data minimizing the need to
-build and maintain data pipelines and ETLâing, speeding up the time to
-deployment and reducing complexity. **P.S. If you like our open-source project
-we'd appreciate if you star it on GitHub â­!**
-                                    *****
-
-                                [MindsDB] *****
----------------------------------------- MindsDB has an active and helpful
+## What can you build with MindsDB? * **Question Answering**: This is useful
+when you have data (we support more than 120 data sources) and you need answers
+from your data given a question in natural language. * **Semantic Search**:
+Similar to Question Answering, but in this case, you want to retrieve specific
+parts of your data where the answer to a question may exist. * **AI Agent
+serving**: This is useful when you want to publish your AI Agents to enterprise
+conversational applications like Slack, email, Twilio, etc. * **Recommendation
+systems**: When you use your data to help predict, narrow down, and find what
+people are looking for among an exponentially growing number of options. *
+**Time Series Forecasting**: When you want to use your historical data to
+estimate how things will look in the future. * **AI Automation pipelines**:
+When you need your AI systems to consume enterprise data and have the AI output
+stored back into your enterprise tools in an automated way. ## Generative AI
+Tables MindsDB empowers developers to harness the power of AI by treating AI
+models as **([Generative AI Tables](https://www.youtube.com/
+watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in
+enterprise data sources. This abstraction makes AI highly accessible, allowing
+development teams to create AI-driven applications using their existing skills.
+                                   [MindsDB]
+The data-centric approach of MindsDB AI Logic server brings the process closer
+   to the source of the data minimizing the need to build and maintain data
+   pipelines and ETLâing, speeding up the time to deployment and reducing
+complexity and because it'sa server, everything you build on top of mindsdb is
+     automatically ready for production. MindsDB has an active and helpful
 community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
-check-out the [rewards and community programs](https://mindsdb.com/
+      check-out the [rewards and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
----------------------------------------- [Installation](https://github.com/
-mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
-mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
-[Database Integrations](https://github.com/mindsdb/mindsdb#database-
-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
-[Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
-(https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
-github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
-mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------------------- ## Use cases Here are
-some popular use cases you can build with MindsDB: * Conversational AI:
-Leverage MindsDB native integrations with data platforms and pre-trained large
-language models, like OpenAI's GPT, to quickly build conversational AI
-solutions without the overhead of managing complex data pipelines. * Fraud
-Detection: MindsDB can help developers build models to detect fraudulent
-activity in financial transactions, eCommerce platforms etc. * Sales
-Forecasting: MindsDB can be used to develop models to predict future sales
-based on historical sales data, allowing businesses to make better-informed
-decisions. * Customer Segmentation: MindsDB can help developers segment
-customers based on their behavior, preferences, and other factors, allowing
-businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
-native integration with pre-trained models like OpenAI GPT or Hugging Face can
-be used to analyze the sentiment of a text data, such as a customer reviews -
-in a single command, instead of individual API calls and ETL-ing data. *
-Predictive Maintenance: MindsDB can be used to build models to predict when
-equipment or machinery is likely to fail, allowing for proactive maintenance
-and minimizing downtime. See more examples and community tutorials [here]
-(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
-[demo environment](https://cloud.mindsdb.com/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
+ **P.S. If you like our open-source project we'd appreciate if you star it on
+GitHub â­!** ---------------------------------------- [Installation](https://
+   github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/
+      mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/
+    mindsdb#features) - [Database Integrations](https://github.com/mindsdb/
+   mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/
+       mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/
+mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support)
+ - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing
+ lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://
+github.com/mindsdb/mindsdb#license) ---------------------------------------- ##
+        Demo You can try MindsDB using our [demo environment](https://
+                              cloud.mindsdb.com/
+   ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
-[dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
-production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
-premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
-platforms and this list is constantly growing. If you canât find the
+ [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
+ production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
+  profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
+ premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
+  How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+    platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. CREATE MODEL to connect the AI Engine you pick that will learn from your
-data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
-you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
-[docs](https://docs.mindsdb.com/sql/create/
-model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+  2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+ data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+  1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+ (https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+ you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+                  [docs](https://docs.mindsdb.com/sql/create/
+ model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
 you want to have manual control over model engineering. 3. JOIN such model with
 your database tables to make predictions for thousands or even millions of data
-points at once, or run SELECT statements or API calls to make one time
+    points at once, or run SELECT statements or API calls to make one time
 predictions. 4. Set up a JOB to automate your re-training cycle and predictions
-pipelines for the new incoming data. 5. Alternatively, use REST API to query
-the models Follow the [quickstart guide](https://docs.mindsdb.com/
+ pipelines for the new incoming data. 5. Alternatively, use REST API to query
+      the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-with sample data to get on-boarded as fast as possible. ## Database
+      with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
-and popular applications. | Connect your Data | Connect your Data | Connect
-your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
-Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
-[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+  and popular applications. | Connect your Data | Connect your Data | Connect
+   your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+  Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+     [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
-[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+   [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+   Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
-| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+  | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
 ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
-| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
-Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
-integration?](https://github.com/mindsdb/mindsdb/issues/
+ | [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+   Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+           integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
-//
+                                      //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-## Support If you found a bug, please submit an [issue on GitHub](https://
-github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+  ## Support If you found a bug, please submit an [issue on GitHub](https://
+ github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
+   can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
 joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
-mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
-stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
-commercial support, please [contact](https://mindsdb.com/contact/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
-team. ## Contributing A great place to start contributing to MindsDB is to
+  mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+  stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+       commercial support, please [contact](https://mindsdb.com/contact/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
+  team. ## Contributing A great place to start contributing to MindsDB is to
 check our GitHub projects :checkered_flag: * Community contributor's [dashboard
-tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
-issues](https://github.com/mindsdb/mindsdb/
+  tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+                  issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
-so feel free to open new issues with your ideas and we can guide you! Being
+  so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
-[contributing documentation](https://docs.mindsdb.com/contribute/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
+       [contributing documentation](https://docs.mindsdb.com/contribute/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
 note that this project is released with a [Contributor Code of Conduct](https:/
-/github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
+ /github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
 in this project, you agree to abide by its terms. Also, check out the [rewards
-and community programs](https://mindsdb.com/
+                 and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ### Current contributors [https://contributors-img.web.app/image?repo=mindsdb/
-mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
-Subscribe to updates Join our [Slack community](https://mindsdb.com/
-joincommunity) and subscribe to the monthly [Developer Newsletter](https://
-mindsdb.com/newsletter/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
-product updates, information about MindsDB events and contests, and useful
-content, like tutorials. ## License MindsDB is licensed under [GNU General
-Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+  mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
+     Subscribe to updates Join our [Slack community](https://mindsdb.com/
+  joincommunity) and subscribe to the monthly [Developer Newsletter](https://
+                            mindsdb.com/newsletter/
+  ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
+  product updates, information about MindsDB events and contests, and useful
+  content, like tutorials. ## License MindsDB is licensed under [GNU General
+ Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+ Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
-Extra: all_extras Provides-Extra: empress Provides-Extra: solr Provides-Extra:
-access Provides-Extra: binance Provides-Extra: yugabyte Provides-Extra:
-bigquery Provides-Extra: timescaledb Provides-Extra: github Provides-Extra:
-cohere Provides-Extra: snowflake Provides-Extra: quickbooks Provides-Extra:
-clickhouse Provides-Extra: sendinblue Provides-Extra: youtube Provides-Extra:
-monetdb Provides-Extra: aurora Provides-Extra: s3 Provides-Extra: autosklearn
-Provides-Extra: dremio Provides-Extra: paypal Provides-Extra: rocket_chat
-Provides-Extra: edgelessdb Provides-Extra: cockroach Provides-Extra:
-planetscale Provides-Extra: google_books Provides-Extra: ray_serve Provides-
-Extra: starrocks Provides-Extra: huggingface_api Provides-Extra: hive Provides-
-Extra: altibase Provides-Extra: mariadb Provides-Extra: ignite Provides-Extra:
-strava Provides-Extra: firebird Provides-Extra: tidb Provides-Extra: crate
-Provides-Extra: influxdb Provides-Extra: neuralforecast Provides-Extra: merlion
-Provides-Extra: vertica Provides-Extra: sheets Provides-Extra: hana Provides-
-Extra: pinot Provides-Extra: confluence Provides-Extra: opengauss Provides-
-Extra: redshift Provides-Extra: trino Provides-Extra: slack Provides-Extra:
-datastax Provides-Extra: questdb Provides-Extra: nuo_jdbc Provides-Extra:
-orioledb Provides-Extra: teradata Provides-Extra: gmail Provides-Extra: oracle
-Provides-Extra: flaml Provides-Extra: langchain Provides-Extra: impala
-Provides-Extra: cloud_spanner Provides-Extra: ingres Provides-Extra: tdengine
-Provides-Extra: google_fit Provides-Extra: google_search Provides-Extra: db2
-Provides-Extra: tpot Provides-Extra: shopify Provides-Extra:
-google_content_shopping Provides-Extra: google_calendar Provides-Extra: ckan
-Provides-Extra: cassandra Provides-Extra: rockset Provides-Extra: monkeylearn
-Provides-Extra: sqlany Provides-Extra: mssql Provides-Extra: huggingface
-Provides-Extra: postgres Provides-Extra: ludwig Provides-Extra: airtable
-Provides-Extra: mysql Provides-Extra: phoenix Provides-Extra: singlestore
-Provides-Extra: oceanbase Provides-Extra: vitess Provides-Extra: newsapi
-Provides-Extra: druid Provides-Extra: hsqldb Provides-Extra: statsforecast
-Provides-Extra: materialize Provides-Extra: openai Provides-Extra: databricks
-Provides-Extra: jira Provides-Extra: scylla Provides-Extra: twitter Provides-
-Extra: gitlab Provides-Extra: surrealdb Provides-Extra: plaid Provides-Extra:
-duckdb Provides-Extra: d0lt Provides-Extra: databend Provides-Extra: stripe
-Provides-Extra: mendeley Provides-Extra: maxdb Provides-Extra: derby Provides-
-Extra: mlflow Provides-Extra: writer Provides-Extra: couchbase Provides-Extra:
-dynamodb Provides-Extra: sqreamdb Provides-Extra: mongodb Provides-Extra:
-cloud_sql Provides-Extra: llama_index Provides-Extra: supabase Provides-Extra:
-matrixone Provides-Extra: informix Provides-Extra: elasticsearch Provides-
-Extra: reddit Provides-Extra: frappe Provides-Extra: lightwood Provides-Extra:
-all_handlers_extras
+ Type: text/markdown Provides-Extra: telemetry Provides-Extra: grpc Provides-
+ Extra: all_extras Provides-Extra: tdengine Provides-Extra: yugabyte Provides-
+Extra: opengauss Provides-Extra: merlion Provides-Extra: ignite Provides-Extra:
+  lightwood Provides-Extra: datastax Provides-Extra: informix Provides-Extra:
+ huggingface_api Provides-Extra: scylla Provides-Extra: huggingface Provides-
+ Extra: access Provides-Extra: frappe Provides-Extra: teradata Provides-Extra:
+  mlflow Provides-Extra: cockroach Provides-Extra: confluence Provides-Extra:
+elasticsearch Provides-Extra: mariadb Provides-Extra: cloud_sql Provides-Extra:
+empress Provides-Extra: cohere Provides-Extra: langchain Provides-Extra: mysql
+  Provides-Extra: d0lt Provides-Extra: sheets Provides-Extra: druid Provides-
+  Extra: phoenix Provides-Extra: planetscale Provides-Extra: paypal Provides-
+  Extra: web Provides-Extra: mediawiki Provides-Extra: aurora Provides-Extra:
+realtime_slack_chat Provides-Extra: dremio Provides-Extra: tidb Provides-Extra:
+ jira Provides-Extra: redshift Provides-Extra: rockset Provides-Extra: twitter
+  Provides-Extra: bigquery Provides-Extra: google_content_shopping Provides-
+Extra: neuralforecast Provides-Extra: edgelessdb Provides-Extra: db2 Provides-
+Extra: cloud_spanner Provides-Extra: databend Provides-Extra: youtube Provides-
+  Extra: postgres Provides-Extra: sendinblue Provides-Extra: ludwig Provides-
+Extra: tpot Provides-Extra: airtable Provides-Extra: clickhouse Provides-Extra:
+  influxdb Provides-Extra: dynamodb Provides-Extra: nuo_jdbc Provides-Extra:
+     pinot Provides-Extra: matrixone Provides-Extra: trino Provides-Extra:
+  monkeylearn Provides-Extra: questdb Provides-Extra: vitess Provides-Extra:
+   llama_index Provides-Extra: gmail Provides-Extra: openai Provides-Extra:
+  cassandra Provides-Extra: materialize Provides-Extra: quickbooks Provides-
+    Extra: impala Provides-Extra: singlestore Provides-Extra: google_search
+  Provides-Extra: duckdb Provides-Extra: solr Provides-Extra: mssql Provides-
+ Extra: flaml Provides-Extra: github Provides-Extra: supabase Provides-Extra:
+  statsforecast Provides-Extra: stripe Provides-Extra: ingres Provides-Extra:
+   autosklearn Provides-Extra: hsqldb Provides-Extra: slack Provides-Extra:
+   mendeley Provides-Extra: orioledb Provides-Extra: gitlab Provides-Extra:
+   mongodb Provides-Extra: vertica Provides-Extra: snowflake Provides-Extra:
+firebird Provides-Extra: strava Provides-Extra: crate Provides-Extra: couchbase
+   Provides-Extra: timescaledb Provides-Extra: binance Provides-Extra: maxdb
+ Provides-Extra: s3 Provides-Extra: shopify Provides-Extra: monetdb Provides-
+  Extra: sqreamdb Provides-Extra: ckan Provides-Extra: writer Provides-Extra:
+    ray_serve Provides-Extra: sqlany Provides-Extra: derby Provides-Extra:
+   google_calendar Provides-Extra: hana Provides-Extra: hive Provides-Extra:
+  google_books Provides-Extra: surrealdb Provides-Extra: google_fit Provides-
+  Extra: rocket_chat Provides-Extra: newsapi Provides-Extra: reddit Provides-
+  Extra: plaid Provides-Extra: databricks Provides-Extra: altibase Provides-
+  Extra: starrocks Provides-Extra: oracle Provides-Extra: oceanbase Provides-
+                          Extra: all_handlers_extras
```

### Comparing `MindsDB-23.6.4.0/README.md` & `MindsDB-23.6.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,50 +48,47 @@
 	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
 </h3>
 
 </div>
 
 ----------------------------------------
 
-[MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+[MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered systems from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
 
-We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
+## What can you build with MindsDB?
 
-By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
+* **Question Answering**: This is useful when you have data (we support more than 120 data sources) and you need answers from your data given a question in natural language.
+* **Semantic Search**: Similar to Question Answering, but in this case, you want to retrieve specific parts of your data where the answer to a question may exist.
+* **AI Agent serving**: This is useful when you want to publish your AI Agents to enterprise conversational applications like Slack, email, Twilio, etc.
+* **Recommendation systems**: When you use your data to help predict, narrow down, and find what people are looking for among an exponentially growing number of options.
+* **Time Series Forecasting**: When you want to use your historical data to estimate how things will look in the future.
+* **AI Automation pipelines**: When you need your AI systems to consume enterprise data and have the AI output stored back into your enterprise tools in an automated way.
 
-**P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
+## Generative AI Tables
 
-<h2 align="center">
-   <br/>
-   <br/>
-  <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
+MindsDB empowers developers to harness the power of AI by treating AI models as **([Generative AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in enterprise data sources. This abstraction makes AI highly accessible, allowing development teams to create AI-driven applications using their existing skills.
 
-</h2>
+<center>
+  
+  <img width="90%" src="https://docs.google.com/drawings/d/e/2PACX-1vR7DCzimVKnIf22CGtKhFryBJKVLn08ZRL56862XxGh_zQQaVQD-0EoMXrvjKqP4ZujHxQAoSgd5jXX/pub?w=1439&h=812" alt="MindsDB">
 
-----------------------------------------
-MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+<center>
 
-----------------------------------------
+The data-centric approach of MindsDB AI Logic server brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity and because it'sa server, everything you build on top of mindsdb is automatically ready for production.
 
-[Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). 
+**P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
 
-----------------------------------------
 
-## Use cases
+----------------------------------------
 
-Here are some popular use cases you can build with MindsDB:
+[Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
 
-* Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
-* Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
-* Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
-* Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
-* Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
-* Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
+----------------------------------------
 
-See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
 
 ## Demo
 
 You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
 
 ## Installation
```

#### html2text {}

```diff
@@ -7,135 +7,130 @@
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 is a Server for Artificial Intelligence Logic, enabling developers to ship AI
-powered projects from prototyping & experimentation to production in a fast &
+powered systems from prototyping & experimentation to production in a fast &
 scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
 Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-We do this by abstracting Generative AI, Large Language and other Models as a
-virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
-top of enterprise databases. This increases accessibility with organizations
-and enables development teams to use their existing skills to build
-applications powered by AI. By taking a data-centric approach to AI MindsDB
-brings the process closer to the source of the data minimizing the need to
-build and maintain data pipelines and ETLâing, speeding up the time to
-deployment and reducing complexity. **P.S. If you like our open-source project
-we'd appreciate if you star it on GitHub â­!**
-                                    *****
-
-                                [MindsDB] *****
----------------------------------------- MindsDB has an active and helpful
+## What can you build with MindsDB? * **Question Answering**: This is useful
+when you have data (we support more than 120 data sources) and you need answers
+from your data given a question in natural language. * **Semantic Search**:
+Similar to Question Answering, but in this case, you want to retrieve specific
+parts of your data where the answer to a question may exist. * **AI Agent
+serving**: This is useful when you want to publish your AI Agents to enterprise
+conversational applications like Slack, email, Twilio, etc. * **Recommendation
+systems**: When you use your data to help predict, narrow down, and find what
+people are looking for among an exponentially growing number of options. *
+**Time Series Forecasting**: When you want to use your historical data to
+estimate how things will look in the future. * **AI Automation pipelines**:
+When you need your AI systems to consume enterprise data and have the AI output
+stored back into your enterprise tools in an automated way. ## Generative AI
+Tables MindsDB empowers developers to harness the power of AI by treating AI
+models as **([Generative AI Tables](https://www.youtube.com/
+watch?v=tnB4Y9T1E2k))**. These tables are capable of learning from data in
+enterprise data sources. This abstraction makes AI highly accessible, allowing
+development teams to create AI-driven applications using their existing skills.
+                                   [MindsDB]
+The data-centric approach of MindsDB AI Logic server brings the process closer
+   to the source of the data minimizing the need to build and maintain data
+   pipelines and ETLâing, speeding up the time to deployment and reducing
+complexity and because it'sa server, everything you build on top of mindsdb is
+     automatically ready for production. MindsDB has an active and helpful
 community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
-check-out the [rewards and community programs](https://mindsdb.com/
+      check-out the [rewards and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
----------------------------------------- [Installation](https://github.com/
-mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
-mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
-[Database Integrations](https://github.com/mindsdb/mindsdb#database-
-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
-[Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
-(https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
-github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
-mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------------------- ## Use cases Here are
-some popular use cases you can build with MindsDB: * Conversational AI:
-Leverage MindsDB native integrations with data platforms and pre-trained large
-language models, like OpenAI's GPT, to quickly build conversational AI
-solutions without the overhead of managing complex data pipelines. * Fraud
-Detection: MindsDB can help developers build models to detect fraudulent
-activity in financial transactions, eCommerce platforms etc. * Sales
-Forecasting: MindsDB can be used to develop models to predict future sales
-based on historical sales data, allowing businesses to make better-informed
-decisions. * Customer Segmentation: MindsDB can help developers segment
-customers based on their behavior, preferences, and other factors, allowing
-businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
-native integration with pre-trained models like OpenAI GPT or Hugging Face can
-be used to analyze the sentiment of a text data, such as a customer reviews -
-in a single command, instead of individual API calls and ETL-ing data. *
-Predictive Maintenance: MindsDB can be used to build models to predict when
-equipment or machinery is likely to fail, allowing for proactive maintenance
-and minimizing downtime. See more examples and community tutorials [here]
-(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
-[demo environment](https://cloud.mindsdb.com/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
+ **P.S. If you like our open-source project we'd appreciate if you star it on
+GitHub â­!** ---------------------------------------- [Installation](https://
+   github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/
+      mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/
+    mindsdb#features) - [Database Integrations](https://github.com/mindsdb/
+   mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/
+       mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/
+mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support)
+ - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing
+ lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://
+github.com/mindsdb/mindsdb#license) ---------------------------------------- ##
+        Demo You can try MindsDB using our [demo environment](https://
+                              cloud.mindsdb.com/
+   ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
-[dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
-production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
-premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
-platforms and this list is constantly growing. If you canât find the
+ [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
+ production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
+  profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
+ premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
+  How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+    platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. CREATE MODEL to connect the AI Engine you pick that will learn from your
-data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
-you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
-[docs](https://docs.mindsdb.com/sql/create/
-model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+  2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+ data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+  1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+ (https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+ you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+                  [docs](https://docs.mindsdb.com/sql/create/
+ model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
 you want to have manual control over model engineering. 3. JOIN such model with
 your database tables to make predictions for thousands or even millions of data
-points at once, or run SELECT statements or API calls to make one time
+    points at once, or run SELECT statements or API calls to make one time
 predictions. 4. Set up a JOB to automate your re-training cycle and predictions
-pipelines for the new incoming data. 5. Alternatively, use REST API to query
-the models Follow the [quickstart guide](https://docs.mindsdb.com/
+ pipelines for the new incoming data. 5. Alternatively, use REST API to query
+      the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-with sample data to get on-boarded as fast as possible. ## Database
+      with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
-and popular applications. | Connect your Data | Connect your Data | Connect
-your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
-Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
-[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+  and popular applications. | Connect your Data | Connect your Data | Connect
+   your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+  Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+     [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
-[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+   [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+   Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
-| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+  | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
 ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
-| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
-Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
-integration?](https://github.com/mindsdb/mindsdb/issues/
+ | [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+   Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+           integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
-//
+                                      //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-## Support If you found a bug, please submit an [issue on GitHub](https://
-github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+  ## Support If you found a bug, please submit an [issue on GitHub](https://
+ github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
+   can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
 joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
-mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
-stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
-commercial support, please [contact](https://mindsdb.com/contact/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
-team. ## Contributing A great place to start contributing to MindsDB is to
+  mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+  stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+       commercial support, please [contact](https://mindsdb.com/contact/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
+  team. ## Contributing A great place to start contributing to MindsDB is to
 check our GitHub projects :checkered_flag: * Community contributor's [dashboard
-tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
-issues](https://github.com/mindsdb/mindsdb/
+  tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+                  issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
-so feel free to open new issues with your ideas and we can guide you! Being
+  so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
-[contributing documentation](https://docs.mindsdb.com/contribute/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
+       [contributing documentation](https://docs.mindsdb.com/contribute/
+ ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
 note that this project is released with a [Contributor Code of Conduct](https:/
-/github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
+ /github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating
 in this project, you agree to abide by its terms. Also, check out the [rewards
-and community programs](https://mindsdb.com/
+                 and community programs](https://mindsdb.com/
 community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ### Current contributors [https://contributors-img.web.app/image?repo=mindsdb/
-mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
-Subscribe to updates Join our [Slack community](https://mindsdb.com/
-joincommunity) and subscribe to the monthly [Developer Newsletter](https://
-mindsdb.com/newsletter/
-?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
-product updates, information about MindsDB events and contests, and useful
-content, like tutorials. ## License MindsDB is licensed under [GNU General
-Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+  mindsdb] Made with [contributors-img](https://contributors-img.web.app). ##
+     Subscribe to updates Join our [Slack community](https://mindsdb.com/
+  joincommunity) and subscribe to the monthly [Developer Newsletter](https://
+                            mindsdb.com/newsletter/
+  ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
+  product updates, information about MindsDB events and contests, and useful
+  content, like tutorials. ## License MindsDB is licensed under [GNU General
+ Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
```

### Comparing `MindsDB-23.6.4.0/mindsdb/__main__.py` & `MindsDB-23.6.5.0/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/common/check_auth.py` & `MindsDB-23.6.5.0/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/gui.py` & `MindsDB-23.6.5.0/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.6.5.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/initialize.py` & `MindsDB-23.6.5.0/mindsdb/api/http/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from werkzeug.exceptions import HTTPException
 
 from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.api.http.gui import update_static
 from mindsdb.api.http.utils import http_error
 from mindsdb.api.http.namespaces.analysis import ns_conf as analysis_ns
 from mindsdb.api.http.namespaces.auth import ns_conf as auth_ns
+from mindsdb.api.http.namespaces.chatbots import ns_conf as chatbots_ns
 from mindsdb.api.http.namespaces.config import ns_conf as conf_ns
 from mindsdb.api.http.namespaces.databases import ns_conf as databases_ns
 from mindsdb.api.http.namespaces.default import ns_conf as default_ns, check_auth
 from mindsdb.api.http.namespaces.file import ns_conf as file_ns
 from mindsdb.api.http.namespaces.handlers import ns_conf as handlers_ns
 from mindsdb.api.http.namespaces.models import ns_conf as models_ns
 from mindsdb.api.http.namespaces.projects import ns_conf as projects_ns
@@ -206,15 +207,16 @@
         sql_ns,
         analysis_ns,
         handlers_ns,
         tree_ns,
         projects_ns,
         databases_ns,
         views_ns,
-        models_ns
+        models_ns,
+        chatbots_ns
     ]
     if with_nlp:
         protected_namespaces.append(nlp_ns)
 
     for ns in protected_namespaces:
         api.add_namespace(ns)
     api.add_namespace(default_ns)
```

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlalchemy.exc import NoResultFound
 
 
 from mindsdb.api.http.namespaces.configs.projects import ns_conf
 from mindsdb.api.http.utils import http_error
 from mindsdb.api.mysql.mysql_proxy.controllers.session_controller import SessionController
 from mindsdb.interfaces.model.functions import PredictorRecordNotFound
+from mindsdb.interfaces.storage.db import Predictor
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.dialects.mindsdb import CreatePredictor
 
 
 @ns_conf.route('/<project_name>/models')
 class ModelsList(Resource):
     @ns_conf.doc('list_models')
@@ -122,20 +123,15 @@
         project_datanode = session.datahub.get(project_name)
         if project_datanode is None:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Project not found',
                 f'Project name {project_name} does not exist')
 
-        name_no_version = model_name
-        version = None
-        parts = model_name.split('.')
-        if len(parts) > 1 and parts[-1].isdigit():
-            version = int(parts[-1])
-            name_no_version = '.'.join(parts[:-1])
+        name_no_version, version = Predictor.get_name_and_version(model_name)
         try:
             return session.model_controller.get_model(name_no_version, version=version, project_name=project_name)
         except PredictorRecordNotFound:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Model not found',
                 f'Model with name {model_name} not found')
@@ -148,21 +144,15 @@
         project_datanode = session.datahub.get(project_name)
         if project_datanode is None:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Project not found',
                 f'Project name {project_name} does not exist')
 
-        name_no_version = model_name
-        version = None
-        parts = model_name.split('.')
-        if len(parts) > 1 and parts[-1].isdigit():
-            version = int(parts[-1])
-            name_no_version = '.'.join(parts[:-1])
-
+        name_no_version, version = Predictor.get_name_and_version(model_name)
         try:
             session.model_controller.get_model(name_no_version, version=version, project_name=project_name)
         except PredictorRecordNotFound:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Model not found',
                 f'Model with name {model_name} not found')
@@ -182,20 +172,15 @@
 @ns_conf.param('project_name', 'Name of the project')
 @ns_conf.param('model_name', 'Name of the model')
 class ModelPredict(Resource):
     @ns_conf.doc('post_model_predict')
     def post(self, project_name, model_name):
         '''Call prediction'''
 
-        name_no_version = model_name
-        version = None
-        parts = model_name.split('.')
-        if len(parts) > 1 and parts[-1].isdigit():
-            version = int(parts[-1])
-            name_no_version = '.'.join(parts[:-1])
+        name_no_version, version = Predictor.get_name_and_version(model_name)
 
         session = SessionController()
         project_datanode = session.datahub.get(project_name)
         if project_datanode is None:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Project not found',
@@ -237,20 +222,15 @@
         project_datanode = session.datahub.get(project_name)
         if project_datanode is None:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Project not found',
                 f'Project name {project_name} does not exist')
 
-        name_no_version = model_name
-        version = None
-        parts = model_name.split('.')
-        if len(parts) > 1 and parts[-1].isdigit():
-            version = int(parts[-1])
-            name_no_version = '.'.join(parts[:-1])
+        name_no_version, version = Predictor.get_name_and_version(model_name)
 
         try:
             session.model_controller.get_model(name_no_version, version=version, project_name=project_name)
         except PredictorRecordNotFound:
             return http_error(
                 HTTPStatus.NOT_FOUND,
                 'Model not found',
```

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.6.5.0/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/start.py` & `MindsDB-23.6.5.0/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/http/utils.py` & `MindsDB-23.6.5.0/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/server.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.6.5.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,15 @@
             data=[[metric_value]]
         )
 
     def answer_describe_predictor(self, statement):
 
         # try full name
         attribute = None
-        model_info = self._get_model_info(statement.value)
+        model_info = self._get_model_info(statement.value, except_absent=False)
         if model_info is None:
             parts = statement.value.parts.copy()
             attribute = parts.pop(-1)
             model_info = self._get_model_info(Identifier(parts=parts))
             if model_info is None:
                 raise SqlApiException(f'Model not found: {statement.value}')
 
@@ -717,15 +717,21 @@
             data=df_dict['data']
         )
 
     def _get_model_info(self, identifier, except_absent=True):
         if len(identifier.parts) == 1:
             identifier.parts = [self.session.database, identifier.parts[0]]
 
-        database_name, model_name, model_version, _describe = resolve_model_identifier(identifier)
+        database_name, model_name, model_version = resolve_model_identifier(identifier)
+
+        if model_name is None:
+            if except_absent:
+                raise Exception(f'Model not found: {identifier.to_string()}')
+            else:
+                return
 
         model_record = get_model_record(
             name=model_name,
             project_name=database_name,
             except_absent=except_absent,
             version=model_version
         )
```

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.6.5.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/nlp/nlp.py` & `MindsDB-23.6.5.0/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.6.5.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from mindsdb.integrations.libs.const import HANDLER_TYPE
 from mindsdb.utilities.log import get_log
 
 logger = get_log()
 
 from .__about__ import __version__ as version, __description__ as description
 try:
-    from .cohere_handler import CohereHandler as Handler
+    from .llama_index_handler import  LlamaIndexHandler as Handler
     import_error = None
-    logger.info("Cohere ML engine successfully imported"")
+    logger.info("LlamaIndex  ML engine successfully imported")
 except Exception as e:
     Handler = None
     import_error = e
-    logger.error("Error Importing Cohere ML engine")
+    logger.info("Error Importing LlamaIndex ML engine")
 
-title = 'Cohere'
-name = 'cohere'
+title = 'LlamaIndex'
+name = 'llama_index'
 type = HANDLER_TYPE.ML
 permanent = True
 
 __all__ = [
     'Handler', 'version', 'name', 'type', 'title', 'description', 'import_error'
 ]
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/cohere_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/cohere_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/flaml_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/flaml_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from email.message import EmailMessage
 
 from base64 import urlsafe_b64encode, urlsafe_b64decode
 
 DEFAULT_SCOPES = ['https://www.googleapis.com/auth/gmail.compose',
-                  'https://www.googleapis.com/auth/gmail.readonly']
+                  'https://www.googleapis.com/auth/gmail.readonly',
+                  'https://www.googleapis.com/auth/gmail.modify']
 
 
 class EmailsTable(APITable):
     """Implementation for the emails table for Gmail"""
 
     def select(self, query: ast.Select) -> pd.DataFrame:
         """Pulls emails from Gmail "users.messages.list" API
@@ -53,25 +54,28 @@
         NotImplementedError
             If the query contains an unsupported operation or condition
         """
 
         conditions = extract_comparison_conditions(query.where)
 
         params = {}
+        include_attachments = False
         for op, arg1, arg2 in conditions:
 
             if op == 'or':
                 raise NotImplementedError(f'OR is not supported')
 
-            if arg1 in ['query', 'label_ids', 'include_spam_trash']:
+            if arg1 in ['query', 'label_ids', 'include_spam_trash', 'include_attachments']:
                 if op == '=':
                     if arg1 == 'query':
                         params['q'] = arg2
                     elif arg1 == 'label_ids':
                         params['labelIds'] = arg2.split(',')
+                    elif arg1 == 'include_attachments':
+                        include_attachments = arg2 == 'true'
                     else:
                         params['includeSpamTrash'] = arg2
                 else:
                     raise NotImplementedError(f'Unknown op: {op}')
 
             else:
                 raise NotImplementedError(f'Unknown clause: {arg1}')
@@ -79,15 +83,17 @@
         if query.limit is not None:
             params['maxResults'] = query.limit.value
 
         result = self.handler.call_gmail_api(
             method_name='list_messages',
             params=params
         )
-
+        attachments = []
+        if include_attachments:
+            attachments = self.handler.get_attachments(result)
         # filter targets
         columns = []
         for target in query.targets:
             if isinstance(target, ast.Star):
                 columns = self.get_columns()
                 break
             elif isinstance(target, ast.Identifier):
@@ -185,17 +191,80 @@
 
             message = {
                 'raw': encoded_message
             }
 
             if 'thread_id' in params:
                 message['threadId'] = params['thread_id']
-
             self.handler.call_gmail_api('send_message', {'body': message})
 
+    def delete(self, query: ast.Delete):
+        """
+        Deletes an event or events in the calendar.
+
+        Args:
+            query (ast.Delete): SQL query to parse.
+
+        Returns:
+            Response: Response object containing the results.
+        """
+
+        # Parse the query to get the conditions.
+        conditions = extract_comparison_conditions(query.where)
+        for op, arg1, arg2 in conditions:
+            if op == 'or':
+                raise NotImplementedError(f'OR is not supported')
+            if arg1 == 'message_id':
+                if op == '=':
+                    self.handler.call_gmail_api('delete_message', {'id': arg2})
+                else:
+                    raise NotImplementedError(f'Unknown op: {op}')
+            else:
+                raise NotImplementedError(f'Unknown clause: {arg1}')
+
+    def update(self, query: ast.Update) -> None:
+        """Updates a label of a message.
+
+        Args:
+            query (ASTNode): The SQL query to parse.
+
+        Raises:
+            NotImplementedError: If the query contains an unsupported condition.
+        """
+        params = {}
+        conditions = extract_comparison_conditions(query.where)
+        for op, arg1, arg2 in conditions:
+            if op == 'or':
+                raise NotImplementedError(f'OR is not supported')
+            if arg1 == 'id':
+                if op == '=':
+                    params['id'] = arg2
+                else:
+                    raise NotImplementedError(f'Unknown op: {op}')
+            else:
+                raise NotImplementedError(f'Unknown clause: {arg1}')
+        request_body = {}
+        values = query.update_columns.items()
+        data_list = list(values)
+        add_label = []
+        remove_label = []
+        for key, value in data_list:
+            if key == 'addLabel':
+                add_label.append(str(value)[1:-1])
+            elif key == 'removeLabel':
+                remove_label.append(str(value)[1:-1])
+            else:
+                raise NotImplementedError(f'Unknown clause: {key}')
+        if add_label:
+            request_body['addLabelIds'] = add_label
+        if remove_label:
+            request_body['removeLabelIds'] = remove_label
+        params['body'] = request_body
+        self.handler.call_gmail_api('update_message', params)
+
 
 class GmailHandler(APIHandler):
     """A class for handling connections and interactions with the Gmail API.
 
     Attributes:
         credentials_file (str): The path to the Google Auth Credentials file for authentication
         and interacting with the Gmail API on behalf of the uesr.
@@ -225,15 +294,14 @@
     def _has_creds_file(self, creds_file):
         # Giving more priority to the S3 file
         if self.s3_credentials_file:
             response = requests.get(self.s3_credentials_file)
             if response.status_code == 200:
                 with open(creds_file, 'w') as creds:
                     creds.write(response.text)
-
                 return True
             else:
                 log.logger.error("Failed to get credentials from S3", response.status_code)
 
         if self.credentials_file and os.path.isfile(self.credentials_file):
             copyfile(self.credentials_file, creds_file)
             return True
@@ -255,17 +323,17 @@
                 creds.refresh(Request())
             elif not os.path.isfile(creds_file) and not self._has_creds_file(creds_file):
                 raise ValueError('No valid Gmail Credentials filepath or S3 url found.')
             else:
                 flow = InstalledAppFlow.from_client_secrets_file(creds_file, self.scopes)
                 creds = flow.run_local_server(port=0, timeout_seconds=120)
 
-        # Save the credentials for the next run
-        with open(token_file, 'w') as token:
-            token.write(creds.to_json())
+            # Save the credentials for the next run
+            with open(token_file, 'w') as token:
+                token.write(creds.to_json())
 
         self.storage.folder_sync('config')
         return build('gmail', 'v1', credentials=creds)
 
     def connect(self) -> object:
         """Authenticate with the Gmail API using the credentials file.
 
@@ -315,15 +383,15 @@
     def native_query(self, query_string: str = None) -> Response:
         ast = parse_sql(query_string, dialect="mindsdb")
 
         return self.query(ast)
 
     def _parse_parts(self, parts, attachments):
         if not parts:
-            return
+            return ''
 
         body = ''
         for part in parts:
             if part['mimeType'] == 'text/plain':
                 part_body = part.get('body', {}).get('data', '')
                 body += urlsafe_b64decode(part_body).decode('utf-8')
             elif part['mimeType'] == 'multipart/alternative' or 'parts' in part:
@@ -379,14 +447,29 @@
         batch_req = self.service.new_batch_http_request(
             lambda id, response, exception: self._parse_message(data, response, exception))
         for message in messages:
             batch_req.add(self.service.users().messages().get(userId='me', id=message['id']))
 
         batch_req.execute()
 
+    def get_attachments(self, result):
+        for index, email in result.iterrows():
+            attachments = json.loads(email['attachments'])
+            for attachment in attachments:
+                attachment_id = attachment['attachmentId']
+                filename = attachment['filename']
+                mimeType = attachment['mimeType']
+                attachment_data = self.service.users().messages().attachments().get(
+                    userId='me', messageId=email['id'], id=attachment_id).execute()
+                file_data = attachment_data['data']
+                file_data = file_data.replace('-', '+').replace('_', '/')
+                file_data = urlsafe_b64decode(file_data)
+                with open(filename, 'wb') as f:
+                    f.write(file_data)
+
     def _handle_list_messages_response(self, data, messages):
         total_pages = len(messages) // self.max_batch_size
         for page in range(total_pages):
             self._get_messages(data, messages[page * self.max_batch_size:(page + 1) * self.max_batch_size])
 
         # Get the remaining messsages, if any
         if len(messages) % self.max_batch_size > 0:
@@ -401,14 +484,18 @@
             DataFrame
         """
         service = self.connect()
         if method_name == 'list_messages':
             method = service.users().messages().list
         elif method_name == 'send_message':
             method = service.users().messages().send
+        elif method_name == "delete_message":
+            method = service.users().messages().trash
+        elif method_name == 'update_message':
+            method = service.users().messages().modify
         else:
             raise NotImplementedError(f'Unknown method_name: {method_name}')
 
         left = None
         count_results = None
         if 'maxResults' in params:
             count_results = params['maxResults']
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 'timeZone': params['start']['timeZone'],
             },
             'end': {
                 'dateTime': params['end']['dateTime'],
                 'timeZone': params['end']['timeZone'],
             },
             'recurrence': [
-                'RRULE:FREQ=DAILY;COUNT=2'
+                'RRULE:FREQ=DAILY;COUNT=1'
             ],
             'attendees': [{'email': attendee['email']} for attendee in (params['attendees'] 
                             if isinstance(params['attendees'], list) else [params['attendees']])],
             'reminders': {
                 'useDefault': False,
                 'overrides': [
                     {'method': 'email', 'minutes': 24 * 60},
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/llama_index_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/llama_index_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,16 @@
         'description': 'The host name or IP address of the MySQL server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.',
         'required': True,
         'label': 'Host'
     },
     port={
         'type': ARG_TYPE.INT,
         'description': 'The TCP/IP port of the MySQL server. Must be an integer.',
-        'required': True
+        'required': True,
+        'label': 'Port'
     },
     ssl={
         'type': ARG_TYPE.BOOL,
         'description': 'Set it to False to disable ssl.',
         'required': False,
         'label': 'ssl'
     },
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self.default_model = 'gpt-3.5-turbo'
         self.default_mode = 'default'  # can also be 'conversational' or 'conversational-full'
         self.supported_modes = ['default', 'conversational', 'conversational-full', 'image']
         self.rate_limit = 60  # requests per minute
         self.max_batch_size = 20
         self.default_max_tokens = 100
         self.chat_completion_models = CHAT_MODELS
+        self.supported_ft_models = ('davinci', 'curie', 'babbage', 'ada')  # base models compatible with finetuning
 
     @staticmethod
     def create_validation(target, args=None, **kwargs):
         if 'using' not in args:
             raise Exception("OpenAI engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
@@ -428,15 +429,15 @@
                                              df)
                     promises.append({"choices": future})
             completion = None
             for p in promises:
                 if not completion:
                     completion = p['choices'].result()
                 else:
-                    completion['choices'].extend(p['choices'].result()['choices'])
+                    completion.extend(p['choices'].result())
 
         return completion
 
     def describe(self, attribute: Optional[str] = None) -> pd.DataFrame:
         # TODO: Update to use update() artifacts
 
         args = self.model_storage.json_get('args')
@@ -475,14 +476,17 @@
         for col in [prompt_col, completion_col]:
             if col not in set(df.columns):
                 raise Exception(f"To fine-tune this OpenAI model, please format your select data query to have a `{prompt_col}` column and a `{completion_col}` column first.")  # noqa
 
         args = {**using_args, **args}
         prev_model_name = self.base_model_storage.json_get('args').get('model_name', '')
 
+        if prev_model_name not in self.supported_ft_models:
+            raise Exception(f"This model cannot be finetuned. Supported base models are {self.supported_ft_models}")
+
         openai.api_key = self._get_openai_api_key(args)
         finetune_time = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
 
         temp_storage_path = tempfile.mkdtemp()
         temp_file_name = f"ft_{finetune_time}"
         temp_model_storage_path = f"{temp_storage_path}/{temp_file_name}.jsonl"
         df.to_json(temp_model_storage_path, orient='records', lines=True)
@@ -506,15 +510,15 @@
         jsons = {k: None for k in file_names.keys()}
         for split, file_name in file_names.items():
             if os.path.isfile(os.path.join(temp_storage_path, file_name)):
                 jsons[split] = openai.File.create(
                     file=open(f"{temp_storage_path}/{file_name}", "rb"),
                     purpose='fine-tune')
 
-        train_file_id = jsons['train'].id if isinstance(jsons['train'], openai.File) else jsons['base']
+        train_file_id = jsons['train'].id if isinstance(jsons['train'], openai.File) else jsons['base'].id
         val_file_id = jsons['val'].id if isinstance(jsons['val'], openai.File) else None
 
         def _get_model_type(model_name: str):
             for model_type in ['ada', 'curie', 'babbage', 'davinci']:
                 if model_type in model_name.lower():
                     return model_type
             return 'ada'
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,183 @@
-import psycopg
-from psycopg.pq import ExecStatus
-from pandas import DataFrame
+from collections import OrderedDict
+from typing import Optional
+import pandas as pd
+import taosrest as td
+from taosrest import sqlalchemy as SA
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
+from mindsdb.utilities.log import get_log
 from mindsdb.integrations.libs.base import DatabaseHandler
-from mindsdb.utilities import log
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
-import mindsdb.utilities.profiler as profiler
+from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
 
-class PostgresHandler(DatabaseHandler):
+log = get_log()
+
+
+class TDEngineHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the PostgreSQL statements.
+    This handler handles connection and execution of the TDEngine statements.
     """
-    name = 'postgres'
 
-    @profiler.profile('init_pg_handler')
-    def __init__(self, name=None, **kwargs):
+    name = 'tdengine'
+
+    def __init__(self, name, connection_data: Optional[dict], **kwargs):
         super().__init__(name)
+        
         self.parser = parse_sql
-        self.connection_args = kwargs.get('connection_data')
-        self.dialect = 'postgresql'
-        self.database = self.connection_args.get('database')
-        self.renderer = SqlalchemyRender('postgres')
+        self.dialect = 'tdengine'
+        self.kwargs = kwargs
+        self.connection_data = connection_data
 
         self.connection = None
         self.is_connected = False
 
-    def __del__(self):
-        if self.is_connected is True:
-            self.disconnect()
 
-    @profiler.profile()
     def connect(self):
-        """
-        Handles the connection to a PostgreSQL database instance.
-        """
         if self.is_connected is True:
             return self.connection
 
         config = {
-            'host': self.connection_args.get('host'),
-            'port': self.connection_args.get('port'),
-            'user': self.connection_args.get('user'),
-            'password': self.connection_args.get('password'),
-            'dbname': self.connection_args.get('database')
+            'url': self.connection_data.get('url', "http://localhost:6041"),
+            'token': self.connection_data.get('token'),
+            'user': self.connection_data.get('user','root'),
+            'password': self.connection_data.get('password','taosdata'),
+            'database': self.connection_data.get('database')
         }
 
-        if self.connection_args.get('sslmode'):
-            config['sslmode'] = self.connection_args.get('sslmode')
-
-        if self.connection_args.get('schema'):
-            config['options'] = f'-c search_path={self.connection_args.get("schema")},public'
-
-        connection = psycopg.connect(**config, connect_timeout=10)
-
+        connection = td.connect(**config)
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
         if self.is_connected is False:
             return
         self.connection.close()
         self.is_connected = False
+        return
 
     def check_connection(self) -> StatusResponse:
-        """
-        Check the connection of the PostgreSQL database
-        :return: success status and error message if error occurs
-        """
-        response = StatusResponse(False)
+       
+        result = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            with connection.cursor() as cur:
-                cur.execute('select 1;')
-            response.success = True
-        except psycopg.Error as e:
-            log.logger.error(f'Error connecting to PostgreSQL {self.database}, {e}!')
-            response.error_message = e
+            result.success = connection is not None
+        except Exception as e:
+            log.error(f'Error connecting to TDEngine {self.connection_data["database"]}, {e}!')
+            result.error_message = str(e)
 
-        if response.success is True and need_to_close:
+        if result.success is True and need_to_close:
             self.disconnect()
-        if response.success is False and self.is_connected is True:
+        if result.success is False and self.is_connected is True:
             self.is_connected = False
 
-        return response
+        return result
 
-    @profiler.profile()
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run in PostgreSQL
+        :param query: The SQL query to run in TDEngine
         :return: returns the records from the current recordset
         """
+
         need_to_close = self.is_connected is False
 
         connection = self.connect()
-        with connection.cursor() as cur:
-            try:
+        cur = connection.cursor() 
+        try:
                 cur.execute(query)
-                if ExecStatus(cur.pgresult.status) == ExecStatus.COMMAND_OK:
-                    response = Response(RESPONSE_TYPE.OK)
-                else:
+                
+                if cur.rowcount != 0:
                     result = cur.fetchall()
                     response = Response(
                         RESPONSE_TYPE.TABLE,
-                        DataFrame(
+                        pd.DataFrame(
                             result,
-                            columns=[x.name for x in cur.description]
+                            columns=[x[0] for x in cur.description]
                         )
                     )
+                else:
+                    response = Response(RESPONSE_TYPE.OK)
                 connection.commit()
-            except Exception as e:
-                log.logger.error(f'Error running query: {query} on {self.database}!')
+        except Exception as e:
+                log.error(f'Error running query: {query} on {self.connection_data["database"]}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
-                    error_code=0,
                     error_message=str(e)
                 )
-                connection.rollback()
-
+                # connection.rollback()
+        cur.close()
         if need_to_close is True:
             self.disconnect()
 
         return response
 
-    @profiler.profile()
     def query(self, query: ASTNode) -> Response:
         """
-        Retrieve the data from the SQL statement with eliminated rows that dont satisfy the WHERE condition
+        Retrieve the data from the SQL statement.
         """
-        query_str = self.renderer.get_string(query, with_failback=True)
+        renderer = SqlalchemyRender(SA.TaosRestDialect)
+        query_str = renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        List all tables in PostgreSQL without the system tables information_schema and pg_catalog
+        Get a list with all of the tabels in TDEngine
         """
-        query = """
-            SELECT
-                table_schema,
-                table_name,
-                table_type
-            FROM
-                information_schema.tables
-            WHERE
-                table_schema NOT IN ('information_schema', 'pg_catalog')
-                and table_type in ('BASE TABLE', 'VIEW')
-        """
-        return self.native_query(query)
-
-    def get_columns(self, table_name: str) -> Response:
-        query = f"""
-            SELECT
-                column_name as "Field",
-                data_type as "Type"
-            FROM
-                information_schema.columns
-            WHERE
-                table_name = '{table_name}'
+        q = 'SHOW TABLES;'
+
+         
+        return self.native_query(q)
+
+    def get_columns(self, table_name) -> Response:
         """
-        return self.native_query(query)
+        Show details about the table
+        """
+        q = f'DESCRIBE {table_name};'
+
+        
+        return self.native_query(q)
+
+
+connection_args = OrderedDict(
+    user={
+        'type': ARG_TYPE.STR,
+        'description': 'The user name used to authenticate with the TDEngine server.'
+    },
+    password={
+        'type': ARG_TYPE.STR,
+        'description': 'The password to authenticate the user with the TDEngine server.'
+    },
+    database={
+        'type': ARG_TYPE.STR,
+        'description': 'The database name to use when connecting with the TDEngine server.'
+    },
+    url={
+        'type': ARG_TYPE.STR,
+        'description': 'The url of the TDEngine server Instance. '
+    },
+    token={
+        'type': ARG_TYPE.INT,
+        'description': 'Unique Token to COnnect TDEngine'
+    },
+
+
+)
+
+connection_args_example = OrderedDict(
+    url='127.0.0.1:6041',
+    token='<token comes here>',
+    user='root',
+    password='taosdata',
+    database='test'
+)
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 from collections import OrderedDict
 from typing import Optional
 import pandas as pd
-import taosrest as td
-from taosrest import sqlalchemy as SA
+import vertica_python as vp
+
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
-from mindsdb.utilities.log import get_log
+from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
+# from sqlalchemy_vertica.dialect_pyodbc  import VerticaDialect
+from sqla_vertica_python.vertica_python import VerticaDialect
+
 
-log = get_log()
 
 
-class TDEngineHandler(DatabaseHandler):
+class VerticaHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the TDEngine statements.
+    This handler handles connection and execution of the Vertica statements.
     """
 
-    name = 'tdengine'
+    name = 'vertica'
 
     def __init__(self, name, connection_data: Optional[dict], **kwargs):
         super().__init__(name)
         
         self.parser = parse_sql
-        self.dialect = 'tdengine'
+        self.dialect = 'vertica'
         self.kwargs = kwargs
         self.connection_data = connection_data
+        self.schema_name = connection_data['schema_name'] if 'schema_name' in connection_data else "public"
 
         self.connection = None
         self.is_connected = False
 
 
     def connect(self):
         if self.is_connected is True:
             return self.connection
 
         config = {
-            'url': self.connection_data.get('url', "http://localhost:6041"),
-            'token': self.connection_data.get('token'),
-            'user': self.connection_data.get('user','root'),
-            'password': self.connection_data.get('password','taosdata'),
-            'database': self.connection_data.get('database')
+            'host': self.connection_data['host'],
+            'port': self.connection_data['port'],
+            'user': self.connection_data['user'],
+            'password': self.connection_data['password'],
+            'database': self.connection_data['database']
         }
 
-        connection = td.connect(**config)
+        connection = vp.connect(**config)
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
         if self.is_connected is False:
             return
@@ -67,117 +70,131 @@
     def check_connection(self) -> StatusResponse:
        
         result = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            result.success = connection is not None
+            result.success = connection.opened()
         except Exception as e:
-            log.error(f'Error connecting to TDEngine {self.connection_data["database"]}, {e}!')
+            log.logger.error(f'Error connecting to Vertica {self.connection_data["database"]}, {e}!')
             result.error_message = str(e)
 
         if result.success is True and need_to_close:
             self.disconnect()
         if result.success is False and self.is_connected is True:
             self.is_connected = False
 
         return result
 
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run in TDEngine
+        :param query: The SQL query to run in VERTICA
         :return: returns the records from the current recordset
         """
 
         need_to_close = self.is_connected is False
 
         connection = self.connect()
-        cur = connection.cursor() 
-        try:
-                cur.execute(query)
-                
-                if cur.rowcount != 0:
-                    result = cur.fetchall()
+        with connection.cursor() as cur:
+            try:
+                e=cur.execute(query)
+                result = e.fetchall()
+                if e.rowcount != -1:
+                    
                     response = Response(
                         RESPONSE_TYPE.TABLE,
                         pd.DataFrame(
                             result,
-                            columns=[x[0] for x in cur.description]
+                            columns=[x.name for x in cur.description]
                         )
                     )
                 else:
                     response = Response(RESPONSE_TYPE.OK)
                 connection.commit()
-        except Exception as e:
-                log.error(f'Error running query: {query} on {self.connection_data["database"]}!')
+            except Exception as e:
+                log.logger.error(f'Error running query: {query} on {self.connection_data["database"]}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
                     error_message=str(e)
                 )
-                # connection.rollback()
-        cur.close()
+                connection.rollback()
+
         if need_to_close is True:
             self.disconnect()
 
         return response
 
     def query(self, query: ASTNode) -> Response:
         """
         Retrieve the data from the SQL statement.
         """
-        renderer = SqlalchemyRender(SA.TaosRestDialect)
+        renderer = SqlalchemyRender(VerticaDialect)
         query_str = renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        Get a list with all of the tabels in TDEngine
+        Get a list with all of the tabels in VERTICA
         """
-        q = 'SHOW TABLES;'
+        q = f'''SELECT 
+        TABLE_NAME,
+        TABLE_SCHEMA
+        from v_catalog.tables 
+        WHERE table_schema='{self.schema_name}' 
+        order by
+        table_name;'''
 
          
         return self.native_query(q)
 
     def get_columns(self, table_name) -> Response:
         """
         Show details about the table
         """
-        q = f'DESCRIBE {table_name};'
+        q = f'''SELECT 
+        column_name , 
+        data_type 
+        FROM v_catalog.columns 
+        WHERE table_name='{table_name}';'''
 
         
         return self.native_query(q)
 
 
 connection_args = OrderedDict(
     user={
         'type': ARG_TYPE.STR,
-        'description': 'The user name used to authenticate with the TDEngine server.'
+        'description': 'The user name used to authenticate with the Vertica server.'
     },
     password={
         'type': ARG_TYPE.STR,
-        'description': 'The password to authenticate the user with the TDEngine server.'
+        'description': 'The password to authenticate the user with the VERTICA server.'
     },
     database={
         'type': ARG_TYPE.STR,
-        'description': 'The database name to use when connecting with the TDEngine server.'
+        'description': 'The database name to use when connecting with the VERTICA server.'
     },
-    url={
+    host={
         'type': ARG_TYPE.STR,
-        'description': 'The url of the TDEngine server Instance. '
+        'description': 'The host name or IP address of the VERTICA server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.'
     },
-    token={
+    port={
         'type': ARG_TYPE.INT,
-        'description': 'Unique Token to COnnect TDEngine'
+        'description': 'The TCP/IP port of the VERTICA server. Must be an integer.'
     },
-
+    schema_name={
+        'type': ARG_TYPE.STR,
+        'description': 'Table are listed according to schema name (it is optional). Note: Default value is "public"'
+    }
 
 )
 
 connection_args_example = OrderedDict(
-    url='127.0.0.1:6041',
-    token='<token comes here>',
+    host='127.0.0.1',
+    port=5433,
     user='root',
-    password='taosdata',
-    database='test'
+    password='password',
+    database='database',
+    schema_name='xyz'
 )
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,200 +1,229 @@
 from collections import OrderedDict
-from typing import Optional
-import pandas as pd
-import vertica_python as vp
 
+import psycopg
+from psycopg.pq import ExecStatus
+from pandas import DataFrame
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
-from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
+from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
+from mindsdb.utilities import log
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
-from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
+import mindsdb.utilities.profiler as profiler
 
-# from sqlalchemy_vertica.dialect_pyodbc  import VerticaDialect
-from sqla_vertica_python.vertica_python import VerticaDialect
 
-
-
-
-class VerticaHandler(DatabaseHandler):
+class PostgresHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the Vertica statements.
+    This handler handles connection and execution of the PostgreSQL statements.
     """
+    name = 'postgres'
 
-    name = 'vertica'
-
-    def __init__(self, name, connection_data: Optional[dict], **kwargs):
+    @profiler.profile('init_pg_handler')
+    def __init__(self, name=None, **kwargs):
         super().__init__(name)
-        
         self.parser = parse_sql
-        self.dialect = 'vertica'
-        self.kwargs = kwargs
-        self.connection_data = connection_data
-        self.schema_name = connection_data['schema_name'] if 'schema_name' in connection_data else "public"
+        self.connection_args = kwargs.get('connection_data')
+        self.dialect = 'postgresql'
+        self.database = self.connection_args.get('database')
+        self.renderer = SqlalchemyRender('postgres')
 
         self.connection = None
         self.is_connected = False
 
+    def __del__(self):
+        if self.is_connected is True:
+            self.disconnect()
 
+    @profiler.profile()
     def connect(self):
+        """
+        Handles the connection to a PostgreSQL database instance.
+        """
         if self.is_connected is True:
             return self.connection
 
         config = {
-            'host': self.connection_data['host'],
-            'port': self.connection_data['port'],
-            'user': self.connection_data['user'],
-            'password': self.connection_data['password'],
-            'database': self.connection_data['database']
+            'host': self.connection_args.get('host'),
+            'port': self.connection_args.get('port'),
+            'user': self.connection_args.get('user'),
+            'password': self.connection_args.get('password'),
+            'dbname': self.connection_args.get('database')
         }
 
-        connection = vp.connect(**config)
+        if self.connection_args.get('sslmode'):
+            config['sslmode'] = self.connection_args.get('sslmode')
+
+        if self.connection_args.get('schema'):
+            config['options'] = f'-c search_path={self.connection_args.get("schema")},public'
+
+        connection = psycopg.connect(**config, connect_timeout=10)
+
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
         if self.is_connected is False:
             return
         self.connection.close()
         self.is_connected = False
-        return
 
     def check_connection(self) -> StatusResponse:
-       
-        result = StatusResponse(False)
+        """
+        Check the connection of the PostgreSQL database
+        :return: success status and error message if error occurs
+        """
+        response = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            result.success = connection.opened()
-        except Exception as e:
-            log.logger.error(f'Error connecting to Vertica {self.connection_data["database"]}, {e}!')
-            result.error_message = str(e)
+            with connection.cursor() as cur:
+                cur.execute('select 1;')
+            response.success = True
+        except psycopg.Error as e:
+            log.logger.error(f'Error connecting to PostgreSQL {self.database}, {e}!')
+            response.error_message = e
 
-        if result.success is True and need_to_close:
+        if response.success is True and need_to_close:
             self.disconnect()
-        if result.success is False and self.is_connected is True:
+        if response.success is False and self.is_connected is True:
             self.is_connected = False
 
-        return result
+        return response
 
+    @profiler.profile()
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run in VERTICA
+        :param query: The SQL query to run in PostgreSQL
         :return: returns the records from the current recordset
         """
-
         need_to_close = self.is_connected is False
 
         connection = self.connect()
         with connection.cursor() as cur:
             try:
-                e=cur.execute(query)
-                result = e.fetchall()
-                if e.rowcount != -1:
-                    
+                cur.execute(query)
+                if ExecStatus(cur.pgresult.status) == ExecStatus.COMMAND_OK:
+                    response = Response(RESPONSE_TYPE.OK)
+                else:
+                    result = cur.fetchall()
                     response = Response(
                         RESPONSE_TYPE.TABLE,
-                        pd.DataFrame(
+                        DataFrame(
                             result,
                             columns=[x.name for x in cur.description]
                         )
                     )
-                else:
-                    response = Response(RESPONSE_TYPE.OK)
                 connection.commit()
             except Exception as e:
-                log.logger.error(f'Error running query: {query} on {self.connection_data["database"]}!')
+                log.logger.error(f'Error running query: {query} on {self.database}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
+                    error_code=0,
                     error_message=str(e)
                 )
                 connection.rollback()
 
         if need_to_close is True:
             self.disconnect()
 
         return response
 
+    @profiler.profile()
     def query(self, query: ASTNode) -> Response:
         """
-        Retrieve the data from the SQL statement.
+        Retrieve the data from the SQL statement with eliminated rows that dont satisfy the WHERE condition
         """
-        renderer = SqlalchemyRender(VerticaDialect)
-        query_str = renderer.get_string(query, with_failback=True)
+        query_str = self.renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        Get a list with all of the tabels in VERTICA
+        List all tables in PostgreSQL without the system tables information_schema and pg_catalog
         """
-        q = f'''SELECT 
-        TABLE_NAME,
-        TABLE_SCHEMA
-        from v_catalog.tables 
-        WHERE table_schema='{self.schema_name}' 
-        order by
-        table_name;'''
-
-         
-        return self.native_query(q)
-
-    def get_columns(self, table_name) -> Response:
-        """
-        Show details about the table
-        """
-        q = f'''SELECT 
-        column_name , 
-        data_type 
-        FROM v_catalog.columns 
-        WHERE table_name='{table_name}';'''
-
-        
-        return self.native_query(q)
-
+        query = """
+            SELECT
+                table_schema,
+                table_name,
+                table_type
+            FROM
+                information_schema.tables
+            WHERE
+                table_schema NOT IN ('information_schema', 'pg_catalog')
+                and table_type in ('BASE TABLE', 'VIEW')
+        """
+        return self.native_query(query)
+
+    def get_columns(self, table_name: str) -> Response:
+        query = f"""
+            SELECT
+                column_name as "Field",
+                data_type as "Type"
+            FROM
+                information_schema.columns
+            WHERE
+                table_name = '{table_name}'
+        """
+        return self.native_query(query)
 
 connection_args = OrderedDict(
     user={
         'type': ARG_TYPE.STR,
-        'description': 'The user name used to authenticate with the Vertica server.'
+        'description': 'The user name used to authenticate with the PostgreSQL server.',
+        'required': True,
+        'label': 'User'
     },
     password={
-        'type': ARG_TYPE.STR,
-        'description': 'The password to authenticate the user with the VERTICA server.'
+        'type': ARG_TYPE.PWD,
+        'description': 'The password to authenticate the user with the PostgreSQL server.',
+        'required': True,
+        'label': 'Password'
     },
     database={
         'type': ARG_TYPE.STR,
-        'description': 'The database name to use when connecting with the VERTICA server.'
+        'description': 'The database name to use when connecting with the PostgreSQL server.',
+        'required': True,
+        'label': 'Database'
     },
     host={
         'type': ARG_TYPE.STR,
-        'description': 'The host name or IP address of the VERTICA server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.'
+        'description': 'The host name or IP address of the PostgreSQL server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.',
+        'required': True,
+        'label': 'Host'
     },
     port={
         'type': ARG_TYPE.INT,
-        'description': 'The TCP/IP port of the VERTICA server. Must be an integer.'
+        'description': 'The TCP/IP port of the PostgreSQL server. Must be an integer.',
+        'required': True,
+        'label': 'Port'
     },
-    schema_name={
+    schema={
         'type': ARG_TYPE.STR,
-        'description': 'Table are listed according to schema name (it is optional). Note: Default value is "public"'
+        'description': 'The schema in which objects are searched first.',
+        'required': False,
+        'label': 'Schema'
+    },
+    sslmode={
+        'type': ARG_TYPE.STR,
+        'description': 'sslmode that will be used for connection.',
+        'required': False,
+        'label': 'sslmode'
     }
-
 )
 
 connection_args_example = OrderedDict(
     host='127.0.0.1',
-    port=5433,
+    port=5432,
     user='root',
     password='password',
-    database='database',
-    schema_name='xyz'
+    database='database'
 )
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/ingest.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/ingest.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/question_answer.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/question_answer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         )
         self.persist_directory = args["chromadb_storage_path"]
 
         llm = Writer(**model_parameters.dict())
         retriever = get_retriever(
             embeddings_model_name=self.embeddings_model_name,
             persist_directory=self.persist_directory,
+            collection_name=args.get('collection_name', '_default_collection')
         )
 
         self.qa = RetrievalQA.from_chain_type(
             llm=llm,
             chain_type="stuff",
             retriever=retriever,
             return_source_documents=True,
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,28 +104,29 @@
     except ValueError:
         raise ValueError(
             f"The {embeddings_model_name}  is not supported, please select a valid option from Hugging Face Hub!"
         )
     return embedding_model
 
 
-def load_chroma(embeddings_model_name, persist_directory, chroma_settings):
+def load_chroma(embeddings_model_name, persist_directory, collection_name, chroma_settings):
     return Chroma(
+        collection_name=collection_name,
         persist_directory=persist_directory,
         embedding_function=load_embeddings_model(embeddings_model_name),
         client_settings=chroma_settings,
     )
 
 
 def get_chroma_settings(persist_directory):
     return Settings(
         chroma_db_impl="duckdb+parquet",
         persist_directory=persist_directory,
         anonymized_telemetry=False,
     )
 
 
-def get_retriever(embeddings_model_name, persist_directory):
+def get_retriever(embeddings_model_name, persist_directory, collection_name):
     chroma_settings = get_chroma_settings(persist_directory)
-    db = load_chroma(embeddings_model_name, persist_directory, chroma_settings)
+    db = load_chroma(embeddings_model_name, persist_directory, collection_name, chroma_settings)
     retriever = db.as_retriever()
     return retriever
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/setup.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         args: Optional[Dict] = None,
     ):
         """
         Dispatch is running embeddings and storing in Chroma VectorDB, unless user already has embeddings persisted
         """
         args = args["using"]
 
-        if not df.empty and args["get_embeddings"]:
+        if not df.empty and args["run_embeddings"]:
             if "context_columns" not in args:
                 # if no context columns provided, use all columns in df
                 args["context_columns"] = df.columns.tolist()
 
             if "embeddings_model_name" not in args:
                 logger.info(
                     f"No embeddings model provided in query, using default model: {DEFAULT_EMBEDDINGS_MODEL}"
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.6.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/base.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/response.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.6.5.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.6.5.0/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/utilities/install.py` & `MindsDB-23.6.5.0/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.6.5.0/mindsdb/integrations/utilities/sql_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,27 +50,52 @@
             conditions.append([op, node.args[0].parts[-1], value])
 
     query_traversal(binary_op, _extract_comparison_conditions)
     return conditions
 
 
 def project_dataframe(df, targets, table_columns):
+    '''
+        case-insensitive projection
+        'select A' and 'select a' return different column case but with the same content
+    '''
+
     columns = []
+    df_cols_idx = {
+        col.lower(): col
+        for col in df.columns
+    }
+    df_col_rename = {}
+
     for target in targets:
         if isinstance(target, ast.Star):
-            columns = table_columns
+            for col in table_columns:
+                col_df = df_cols_idx.get(col.lower())
+                if col_df is not None:
+                    df_col_rename[col_df] = col
+                columns.append(col)
+
             break
         elif isinstance(target, ast.Identifier):
-            columns.append(target.parts[-1])
+            col = target.parts[-1]
+            col_df = df_cols_idx.get(col.lower())
+            if col_df is not None:
+                df_col_rename[col_df] = col
+            columns.append(col)
         else:
             raise NotImplementedError
 
     if len(df) == 0:
         df = pd.DataFrame([], columns=columns)
     else:
+
+        # adapt column names to projection
+        if len(df_col_rename) > 0:
+            df = df.rename(columns=df_col_rename)
+
         # add absent columns
         for col in set(columns) & set(df.columns) ^ set(columns):
             df[col] = None
 
         # filter by columns
         df = df[columns]
     return df
```

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.6.5.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.6.5.0/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/chatbot/chatbot_task.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/chatbot/chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/database/database.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/database/projects.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/database/views.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/model/functions.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/model/model_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
             active=None
         )
         last_version = max([x.version or 1 for x in models])
 
         return last_version + 1
 
     def prepare_finetune_statement(self, statement, database_controller):
-        project_name, model_name, model_version, _describe = resolve_model_identifier(statement.name)
+        project_name, model_name, model_version = resolve_model_identifier(statement.name)
         data_integration_ref, fetch_data_query = self._get_data_integration_ref(statement, database_controller)
 
         set_active = True
         if statement.using is not None:
             set_active = statement.using.pop('active', True)
             if set_active in ('0', 0, None):
                 set_active = False
```

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/storage/db.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/storage/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import json
 import datetime
+from typing import Dict
 
 import numpy as np
 from sqlalchemy import create_engine, types, UniqueConstraint
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, Integer, String, DateTime, Boolean, Index
 from sqlalchemy.sql.schema import ForeignKey
@@ -129,14 +130,24 @@
     lightwood_version = Column(String, nullable=True)
     dtype_dict = Column(Json, nullable=True)
     project_id = Column(Integer, ForeignKey('project.id', name='fk_project_id'), nullable=False)
     training_phase_current = Column(Integer)
     training_phase_total = Column(Integer)
     training_phase_name = Column(String)
 
+    @staticmethod
+    def get_name_and_version(full_name):
+        name_no_version = full_name
+        version = None
+        parts = full_name.split('.')
+        if len(parts) > 1 and parts[-1].isdigit():
+            version = int(parts[-1])
+            name_no_version = '.'.join(parts[:-1])
+        return name_no_version, version
+
 
 class Project(Base):
     __tablename__ = 'project'
 
     id = Column(Integer, primary_key=True)
     created_at = Column(DateTime, default=datetime.datetime.now)
     updated_at = Column(DateTime, default=datetime.datetime.now, onupdate=datetime.datetime.now)
@@ -257,12 +268,41 @@
     company_id = Column(Integer)
     user_class = Column(Integer, nullable=True)
 
     name = Column(String, nullable=False)
     project_id = Column(Integer, nullable=False)
 
     model_name = Column(String, nullable=False)
-    database_id = Column(Integer, nullable=False)
+    # If database_id is set we use an API Handler to poll chat messages.
+    database_id = Column(Integer)
+    # If chat_engine is set we use a RealtimeChatHandler to subscribe to chat messages.
+    # TODO(tmichaeldb): Consolidate existing polling logic and realtime chat logic together.
+    chat_engine = Column(String)
     params = Column(JSON)
 
+    is_running = Column(Boolean, default=True)
     updated_at = Column(DateTime, default=datetime.datetime.now, onupdate=datetime.datetime.now)
     created_at = Column(DateTime, default=datetime.datetime.now)
+
+    def as_dict(self) -> Dict:
+        return {
+            'id': self.id,
+            'name': self.name,
+            'project_id': self.project_id,
+            'model_name': self.model_name,
+            'chat_engine': self.chat_engine,
+            'params': self.params,
+            'is_running': self.is_running,
+            'created_at': self.created_at
+        }
+
+
+class ChatBotsHistory(Base):
+    __tablename__ = 'chat_bots_history'
+    id = Column(Integer, primary_key=True)
+    chat_bot_id = Column(Integer)
+    type = Column(String)
+    text = Column(String)
+    user = Column(String)
+    destination = Column(String)
+    sent_at = Column(DateTime, default=datetime.datetime.now)
+    error = Column(String)
```

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/storage/json.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.6.5.0/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.6.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/alembic.ini` & `MindsDB-23.6.5.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/env.py` & `MindsDB-23.6.5.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/migrate.py` & `MindsDB-23.6.5.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-23.6.5.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'chat_bots',
         sa.Column('id', sa.Integer(), nullable=False),
         sa.Column('company_id', sa.Integer(), nullable=True),
         sa.Column('user_class', sa.Integer(), nullable=True),
         sa.Column('name', sa.String(), nullable=False),
         sa.Column('project_id', sa.Integer(), nullable=False),
         sa.Column('model_name', sa.String(), nullable=False),
-        sa.Column('database_id', sa.Integer(), nullable=False),
+        sa.Column('database_id', sa.Integer()),
         sa.Column('params', sa.JSON(), nullable=True),
         sa.Column('updated_at', sa.DateTime(), nullable=True),
         sa.Column('created_at', sa.DateTime(), nullable=True),
         sa.PrimaryKeyConstraint('id')
     )
```

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/auth.py` & `MindsDB-23.6.5.0/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/cache.py` & `MindsDB-23.6.5.0/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/config.py` & `MindsDB-23.6.5.0/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/context.py` & `MindsDB-23.6.5.0/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/fs.py` & `MindsDB-23.6.5.0/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/functions.py` & `MindsDB-23.6.5.0/mindsdb/utilities/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,36 +105,35 @@
 
 
 def resolve_model_identifier(name: Identifier) -> tuple:
     """ split model name to parts
 
         Examples:
             >>> resolve_model_identifier(['a', 'b'])
-            ('a', 'b', None, None)
+            ('a', 'b', None)
 
             >>> resolve_model_identifier(['a', '1'])
-            (None, 'a', 1, None)
+            (None, 'a', 1)
 
             >>> resolve_model_identifier(['a'])
-            (None, 'a', None, None)
+            (None, 'a', None)
 
             >>> resolve_model_identifier(['a', 'b', 'c'])
-            ('a', 'b', None, 'c')
+            (None, None, None)  # not found
 
         Args:
             name (list): Identifier parts
 
         Returns:
             tuple: (database_name, model_name, model_version, describe)
     """
     name = name.parts
     database_name = None
     model_name = None
     model_version = None
-    describe = None
     parts_count = len(name)
     if parts_count == 1:
         database_name = None
         model_name = name[0]
         model_version = None
     elif parts_count == 2:
         if name[-1].isdigit():
@@ -147,9 +146,11 @@
             model_version = None
     elif parts_count == 3:
         database_name = name[0]
         model_name = name[1]
         if name[2].isdigit():
             model_version = int(name[2])
         else:
-            describe = name[2]
-    return (database_name, model_name, model_version, describe)
+            # not found
+            return None, None, None
+
+    return database_name, model_name, model_version
```

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.6.5.0/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/json_encoder.py` & `MindsDB-23.6.5.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/log.py` & `MindsDB-23.6.5.0/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/log_controller.py` & `MindsDB-23.6.5.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.6.5.0/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/ps.py` & `MindsDB-23.6.5.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/telemetry.py` & `MindsDB-23.6.5.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/mindsdb/utilities/wizards.py` & `MindsDB-23.6.5.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.4.0/requirements/requirements.txt` & `MindsDB-23.6.5.0/requirements/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 clickhouse-sqlalchemy
 charset-normalizer
 dill >= 0.3.4
 pyOpenSSL >= 22.0.0
 pydateinfer==0.3.0
 pyarrow >= 10.0.1, < 10.1.0
 dataprep_ml
-grpcio-tools
 python-magic >= 0.4.27
 openpyxl >= 3.1.1
+slack_sdk
```

### Comparing `MindsDB-23.6.4.0/setup.py` & `MindsDB-23.6.5.0/setup.py`

 * *Files identical despite different names*

