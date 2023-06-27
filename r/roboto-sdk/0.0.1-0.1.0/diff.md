# Comparing `tmp/roboto-sdk-0.0.1.tar.gz` & `tmp/roboto_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto-sdk-0.0.1.tar", last modified: Thu Jun  1 18:03:58 2023, max compression
+gzip compressed data, was "roboto_sdk-0.1.0.tar", max compression
```

## Comparing `roboto-sdk-0.0.1.tar` & `roboto_sdk-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,90 @@
-drwxr-xr-x   0 roboto     (502) staff       (20)        0 2023-06-01 18:03:58.627291 roboto-sdk-0.0.1/
--rw-r--r--   0 roboto     (502) staff       (20)      353 2023-06-01 18:03:58.627179 roboto-sdk-0.0.1/PKG-INFO
-drwxr-xr-x   0 roboto     (502) staff       (20)        0 2023-06-01 18:03:58.626448 roboto-sdk-0.0.1/roboto-sdk/
--rw-r--r--   0 roboto     (502) staff       (20)       43 2023-06-01 18:00:21.000000 roboto-sdk-0.0.1/roboto-sdk/__init__.py
-drwxr-xr-x   0 roboto     (502) staff       (20)        0 2023-06-01 18:03:58.627036 roboto-sdk-0.0.1/roboto_sdk.egg-info/
--rw-r--r--   0 roboto     (502) staff       (20)      353 2023-06-01 18:03:58.000000 roboto-sdk-0.0.1/roboto_sdk.egg-info/PKG-INFO
--rw-r--r--   0 roboto     (502) staff       (20)      167 2023-06-01 18:03:58.000000 roboto-sdk-0.0.1/roboto_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 roboto     (502) staff       (20)        1 2023-06-01 18:03:58.000000 roboto-sdk-0.0.1/roboto_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 roboto     (502) staff       (20)       11 2023-06-01 18:03:58.000000 roboto-sdk-0.0.1/roboto_sdk.egg-info/top_level.txt
--rw-r--r--   0 roboto     (502) staff       (20)       38 2023-06-01 18:03:58.627326 roboto-sdk-0.0.1/setup.cfg
--rw-r--r--   0 roboto     (502) staff       (20)      611 2023-06-01 18:00:37.000000 roboto-sdk-0.0.1/setup.py
+-rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0      754 2023-06-23 22:06:45.957630 roboto_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.0/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.0/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0     3892 2023-06-25 17:00:28.230327 roboto_sdk-0.1.0/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.0/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      788 2023-06-24 00:11:31.029362 roboto_sdk-0.1.0/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6690 2023-06-21 21:21:55.948875 roboto_sdk-0.1.0/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3236 2023-06-25 17:23:12.369105 roboto_sdk-0.1.0/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.0/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.0/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3165 2023-06-24 00:34:28.168958 roboto_sdk-0.1.0/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.0/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.0/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.0/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.0/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:18:26.922915 roboto_sdk-0.1.0/src/roboto_sdk/delegate/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-13 17:13:48.413704 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/__init__.py
+-rw-r--r--   0        0        0     4981 2023-06-15 18:41:26.811336 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      651 2023-06-15 18:41:26.811435 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_resources.py
+-rw-r--r--   0        0        0     3463 2023-06-22 00:30:04.537634 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      448 2023-06-15 18:41:26.811604 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0      166 2023-06-13 17:13:48.414122 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/__init__.py
+-rw-r--r--   0        0        0     4750 2023-06-14 17:40:40.588738 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/http_delegate.py
+-rw-r--r--   0        0        0      363 2023-06-13 17:13:48.414231 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/http_resources.py
+-rw-r--r--   0        0        0      297 2023-06-13 17:13:48.414296 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/__init__.py
+-rw-r--r--   0        0        0     2113 2023-06-14 17:40:40.588896 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-06-13 17:13:48.414393 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/http_resources.py
+-rw-r--r--   0        0        0     2323 2023-06-14 17:40:40.589039 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/s3_delegate.py
+-rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.0/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-23 23:37:43.832600 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-24 00:19:03.182623 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     2243 2023-06-24 00:19:03.180345 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      177 2023-06-23 23:37:43.833111 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1485 2023-06-24 00:19:03.185556 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1147 2023-06-23 23:37:43.833392 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      545 2023-06-23 23:37:43.833519 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2685 2023-06-21 18:17:36.116508 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      623 2023-06-25 17:14:17.623374 roboto_sdk-0.1.0/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.0/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.0/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3032 2023-06-25 17:23:12.393083 roboto_sdk-0.1.0/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.0/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.416919 roboto_sdk-0.1.0/src/roboto_sdk/model/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-15 18:41:26.811706 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/__init__.py
+-rw-r--r--   0        0        0     7019 2023-06-15 18:41:26.811800 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action.py
+-rw-r--r--   0        0        0     2804 2023-06-15 18:41:26.811886 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_delegate.py
+-rw-r--r--   0        0        0      792 2023-06-15 18:41:26.811996 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-06-13 17:13:48.416658 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/error.py
+-rw-r--r--   0        0        0     2247 2023-06-21 18:21:45.309132 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation.py
+-rw-r--r--   0        0        0     1413 2023-06-21 18:24:02.339440 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     1464 2023-06-15 18:41:26.812185 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_record.py
+-rw-r--r--   0        0        0      395 2023-06-13 17:13:48.417131 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/__init__.py
+-rw-r--r--   0        0        0     9580 2023-06-14 17:40:40.589162 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/dataset.py
+-rw-r--r--   0        0        0     2132 2023-06-14 17:40:40.589271 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/delegate.py
+-rw-r--r--   0        0        0      817 2023-06-13 17:13:48.417299 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/record.py
+-rw-r--r--   0        0        0      178 2023-06-14 17:40:40.589416 roboto_sdk-0.1.0/src/roboto_sdk/model/files/__init__.py
+-rw-r--r--   0        0        0     1156 2023-06-14 17:40:40.589560 roboto_sdk-0.1.0/src/roboto_sdk/model/files/delegate.py
+-rw-r--r--   0        0        0      771 2023-06-14 17:40:40.589669 roboto_sdk-0.1.0/src/roboto_sdk/model/files/file.py
+-rw-r--r--   0        0        0      385 2023-06-14 17:40:40.589805 roboto_sdk-0.1.0/src/roboto_sdk/model/files/record.py
+-rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.0/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.0/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0     2809 2023-06-25 17:05:30.425831 roboto_sdk-0.1.0/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.0/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.0/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.0/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 roboto_sdk-0.1.0/PKG-INFO
```

