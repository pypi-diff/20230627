# Comparing `tmp/roboto_sdk-0.1.0.tar.gz` & `tmp/roboto_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.0.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.1.tar", max compression
```

## Comparing `roboto_sdk-0.1.0.tar` & `roboto_sdk-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      754 2023-06-23 22:06:45.957630 roboto_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.0/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.0/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     3892 2023-06-25 17:00:28.230327 roboto_sdk-0.1.0/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.0/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.0/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      788 2023-06-24 00:11:31.029362 roboto_sdk-0.1.0/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6690 2023-06-21 21:21:55.948875 roboto_sdk-0.1.0/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3236 2023-06-25 17:23:12.369105 roboto_sdk-0.1.0/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.0/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.0/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3165 2023-06-24 00:34:28.168958 roboto_sdk-0.1.0/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.0/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.0/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.0/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.0/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.0/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0        0 2023-06-01 19:18:26.922915 roboto_sdk-0.1.0/src/roboto_sdk/delegate/__init__.py
--rw-r--r--   0        0        0      621 2023-06-13 17:13:48.413704 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/__init__.py
--rw-r--r--   0        0        0     4981 2023-06-15 18:41:26.811336 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_delegate.py
--rw-r--r--   0        0        0      651 2023-06-15 18:41:26.811435 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_resources.py
--rw-r--r--   0        0        0     3463 2023-06-22 00:30:04.537634 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      448 2023-06-15 18:41:26.811604 roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/invocation_http_resources.py
--rw-r--r--   0        0        0      166 2023-06-13 17:13:48.414122 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/__init__.py
--rw-r--r--   0        0        0     4750 2023-06-14 17:40:40.588738 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/http_delegate.py
--rw-r--r--   0        0        0      363 2023-06-13 17:13:48.414231 roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/http_resources.py
--rw-r--r--   0        0        0      297 2023-06-13 17:13:48.414296 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/__init__.py
--rw-r--r--   0        0        0     2113 2023-06-14 17:40:40.588896 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-06-13 17:13:48.414393 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/http_resources.py
--rw-r--r--   0        0        0     2323 2023-06-14 17:40:40.589039 roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/s3_delegate.py
--rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.0/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0      520 2023-06-23 23:37:43.832600 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0      893 2023-06-24 00:19:03.182623 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     2243 2023-06-24 00:19:03.180345 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      177 2023-06-23 23:37:43.833111 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1485 2023-06-24 00:19:03.185556 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1147 2023-06-23 23:37:43.833392 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      545 2023-06-23 23:37:43.833519 roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2685 2023-06-21 18:17:36.116508 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      623 2023-06-25 17:14:17.623374 roboto_sdk-0.1.0/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.0/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.0/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3032 2023-06-25 17:23:12.393083 roboto_sdk-0.1.0/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.0/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.416919 roboto_sdk-0.1.0/src/roboto_sdk/model/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-15 18:41:26.811706 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/__init__.py
--rw-r--r--   0        0        0     7019 2023-06-15 18:41:26.811800 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action.py
--rw-r--r--   0        0        0     2804 2023-06-15 18:41:26.811886 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_delegate.py
--rw-r--r--   0        0        0      792 2023-06-15 18:41:26.811996 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-06-13 17:13:48.416658 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/error.py
--rw-r--r--   0        0        0     2247 2023-06-21 18:21:45.309132 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation.py
--rw-r--r--   0        0        0     1413 2023-06-21 18:24:02.339440 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_delegate.py
--rw-r--r--   0        0        0     1464 2023-06-15 18:41:26.812185 roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_record.py
--rw-r--r--   0        0        0      395 2023-06-13 17:13:48.417131 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/__init__.py
--rw-r--r--   0        0        0     9580 2023-06-14 17:40:40.589162 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/dataset.py
--rw-r--r--   0        0        0     2132 2023-06-14 17:40:40.589271 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/delegate.py
--rw-r--r--   0        0        0      817 2023-06-13 17:13:48.417299 roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/record.py
--rw-r--r--   0        0        0      178 2023-06-14 17:40:40.589416 roboto_sdk-0.1.0/src/roboto_sdk/model/files/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-14 17:40:40.589560 roboto_sdk-0.1.0/src/roboto_sdk/model/files/delegate.py
--rw-r--r--   0        0        0      771 2023-06-14 17:40:40.589669 roboto_sdk-0.1.0/src/roboto_sdk/model/files/file.py
--rw-r--r--   0        0        0      385 2023-06-14 17:40:40.589805 roboto_sdk-0.1.0/src/roboto_sdk/model/files/record.py
--rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.0/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.0/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-25 17:05:30.425831 roboto_sdk-0.1.0/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.0/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.0/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.0/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 roboto_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0      806 2023-06-27 16:56:42.083372 roboto_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.1/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.1/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0     3892 2023-06-25 17:00:28.230327 roboto_sdk-0.1.1/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.1/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      788 2023-06-24 00:11:31.029362 roboto_sdk-0.1.1/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6690 2023-06-21 21:21:55.948875 roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3236 2023-06-25 17:23:12.369105 roboto_sdk-0.1.1/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.1/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.1/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3165 2023-06-24 00:34:28.168958 roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.1/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:18:26.922915 roboto_sdk-0.1.1/src/roboto_sdk/delegate/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-13 17:13:48.413704 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/__init__.py
+-rw-r--r--   0        0        0     4981 2023-06-15 18:41:26.811336 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      651 2023-06-15 18:41:26.811435 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_resources.py
+-rw-r--r--   0        0        0     3463 2023-06-22 00:30:04.537634 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      448 2023-06-15 18:41:26.811604 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0      166 2023-06-13 17:13:48.414122 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/__init__.py
+-rw-r--r--   0        0        0     4750 2023-06-14 17:40:40.588738 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_delegate.py
+-rw-r--r--   0        0        0      363 2023-06-13 17:13:48.414231 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_resources.py
+-rw-r--r--   0        0        0      297 2023-06-13 17:13:48.414296 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/__init__.py
+-rw-r--r--   0        0        0     2113 2023-06-14 17:40:40.588896 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-06-13 17:13:48.414393 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_resources.py
+-rw-r--r--   0        0        0     2323 2023-06-14 17:40:40.589039 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/s3_delegate.py
+-rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.1/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-23 23:37:43.832600 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-24 00:19:03.182623 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     2243 2023-06-24 00:19:03.180345 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      177 2023-06-23 23:37:43.833111 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1485 2023-06-24 00:19:03.185556 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1147 2023-06-23 23:37:43.833392 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      545 2023-06-23 23:37:43.833519 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2685 2023-06-21 18:17:36.116508 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      623 2023-06-25 17:14:17.623374 roboto_sdk-0.1.1/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.1/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.1/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3032 2023-06-25 17:23:12.393083 roboto_sdk-0.1.1/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.1/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.416919 roboto_sdk-0.1.1/src/roboto_sdk/model/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-15 18:41:26.811706 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/__init__.py
+-rw-r--r--   0        0        0     7019 2023-06-15 18:41:26.811800 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action.py
+-rw-r--r--   0        0        0     2804 2023-06-15 18:41:26.811886 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_delegate.py
+-rw-r--r--   0        0        0      792 2023-06-15 18:41:26.811996 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-06-13 17:13:48.416658 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/error.py
+-rw-r--r--   0        0        0     2247 2023-06-21 18:21:45.309132 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation.py
+-rw-r--r--   0        0        0     1413 2023-06-21 18:24:02.339440 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     1464 2023-06-15 18:41:26.812185 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_record.py
+-rw-r--r--   0        0        0      395 2023-06-13 17:13:48.417131 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/__init__.py
+-rw-r--r--   0        0        0     9580 2023-06-14 17:40:40.589162 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/dataset.py
+-rw-r--r--   0        0        0     2132 2023-06-14 17:40:40.589271 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/delegate.py
+-rw-r--r--   0        0        0      817 2023-06-13 17:13:48.417299 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/record.py
+-rw-r--r--   0        0        0      178 2023-06-14 17:40:40.589416 roboto_sdk-0.1.1/src/roboto_sdk/model/files/__init__.py
+-rw-r--r--   0        0        0     1156 2023-06-14 17:40:40.589560 roboto_sdk-0.1.1/src/roboto_sdk/model/files/delegate.py
+-rw-r--r--   0        0        0      771 2023-06-14 17:40:40.589669 roboto_sdk-0.1.1/src/roboto_sdk/model/files/file.py
+-rw-r--r--   0        0        0      385 2023-06-14 17:40:40.589805 roboto_sdk-0.1.1/src/roboto_sdk/model/files/record.py
+-rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.1/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.1/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0     2809 2023-06-25 17:05:30.425831 roboto_sdk-0.1.1/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.1/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.1/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.1/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 roboto_sdk-0.1.1/PKG-INFO
```

### Comparing `roboto_sdk-0.1.0/pyproject.toml` & `roboto_sdk-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Tools for interacting with roboto.ai"
+license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = {extras = ["crt"], version = "~1.26"}
 pathspec = "~0.11"
```

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.1/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/entry.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.1/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/__init__.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/action_http_resources.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/datasets/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/delegate/files/s3_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.1/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.1/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.1/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/__init__.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/action_record.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/actions/invocation_record.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/dataset.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/datasets/record.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/files/delegate.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/model/files/file.py` & `roboto_sdk-0.1.1/src/roboto_sdk/model/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.1/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.1/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.0/PKG-INFO` & `roboto_sdk-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Tools for interacting with roboto.ai
+License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3[crt] (>=1.26,<1.27)
 Requires-Dist: pathspec (>=0.11,<0.12)
 Requires-Dist: pydantic (>=1.10,<1.11)
 Requires-Dist: pyjwt (>=2.7,<2.8)
```

