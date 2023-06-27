# Comparing `tmp/gyver-2.2.0.tar.gz` & `tmp/gyver-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-2.2.0.tar", max compression
+gzip compressed data, was "gyver-2.3.0.tar", max compression
```

## Comparing `gyver-2.2.0.tar` & `gyver-2.3.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
--rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.2.0/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.2.0/README.md
--rw-r--r--   0        0        0      158 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/__init__.py
--rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/__init__.py
--rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/asyncio.py
--rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/config.py
--rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/interface.py
--rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/mapper.py
--rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/mock.py
--rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/redis.py
--rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/sync.py
--rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/cache/utils.py
--rw-r--r--   0        0        0      498 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.2.0/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     5886 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0     3435 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/config/config.py
--rw-r--r--   0        0        0     2126 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/config/envconfig.py
--rw-r--r--   0        0        0      587 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/config/typedef.py
--rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/config/utils.py
--rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.2.0/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/context.py
--rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/context/typedef.py
--rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/crypto/__init__.py
--rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/crypto/config.py
--rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/crypto/fernet.py
--rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/crypto/rsa.py
--rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/database/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.2.0/gyver/database/adapter.py
--rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/config.py
--rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/context/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/context/asyncio.py
--rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/context/sync.py
--rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/drivers/__init__.py
--rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/drivers/dialect.py
--rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/drivers/interface.py
--rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/drivers/utils.py
--rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/entity.py
--rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/entity.pyi
--rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/metadata.py
--rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/query/__init__.py
--rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.2.0/gyver/database/query/_helpers.py
--rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/comp.py
--rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/exc.py
--rw-r--r--   0        0        0     1353 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/interface.py
--rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/null.py
--rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/order_by.py
--rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/paginate.py
--rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/utils.py
--rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/query/where.py
--rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/typedef.py
--rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/database/utils.py
--rw-r--r--   0        0        0     2271 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/exc.py
--rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.2.0/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3087 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2576 2023-06-27 06:38:47.115897 gyver-2.2.0/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2940 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.2.0/gyver/model.py
--rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/py.typed
--rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/url/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/core.py
--rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.2.0/gyver/url/encode.py
--rw-r--r--   0        0        0      664 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/fragment.py
--rw-r--r--   0        0        0     2834 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/netloc.py
--rw-r--r--   0        0        0     2795 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/path.py
--rw-r--r--   0        0        0     1711 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/query.py
--rw-r--r--   0        0        0      662 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/url/utils.py
--rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.2.0/gyver/utils/__init__.py
--rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.2.0/gyver/utils/exc.py
--rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.2.0/gyver/utils/finder.py
--rw-r--r--   0        0        0     4339 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/utils/helpers.py
--rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.2.0/gyver/utils/json.py
--rw-r--r--   0        0        0     2610 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/utils/lazy.py
--rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.2.0/gyver/utils/singleton.py
--rw-r--r--   0        0        0     1718 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/utils/strings.py
--rw-r--r--   0        0        0      134 2023-06-27 06:38:47.116897 gyver-2.2.0/gyver/utils/timezone.py
--rw-r--r--   0        0        0     2449 2023-06-27 06:38:47.116897 gyver-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 gyver-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.0/README.md
+-rw-r--r--   0        0        0      158 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/__init__.py
+-rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/asyncio.py
+-rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/config.py
+-rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/interface.py
+-rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/mapper.py
+-rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/mock.py
+-rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/redis.py
+-rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/sync.py
+-rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/cache/utils.py
+-rw-r--r--   0        0        0      597 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.0/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/config.py
+-rw-r--r--   0        0        0     2690 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/envconfig.py
+-rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/interface.py
+-rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/lazy.py
+-rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/config/typedef.py
+-rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/config/utils.py
+-rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.0/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/context/typedef.py
+-rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/config.py
+-rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/fernet.py
+-rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/crypto/rsa.py
+-rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/database/__init__.py
+-rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.0/gyver/database/adapter.py
+-rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/config.py
+-rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/asyncio.py
+-rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/context/sync.py
+-rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/dialect.py
+-rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/interface.py
+-rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/drivers/utils.py
+-rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/entity.py
+-rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/entity.pyi
+-rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/metadata.py
+-rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/query/__init__.py
+-rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.0/gyver/database/query/_helpers.py
+-rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/comp.py
+-rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/exc.py
+-rw-r--r--   0        0        0     1353 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/interface.py
+-rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/null.py
+-rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/order_by.py
+-rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/paginate.py
+-rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/utils.py
+-rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/query/where.py
+-rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/typedef.py
+-rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/database/utils.py
+-rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.0/gyver/exc.py
+-rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.0/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3107 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2503 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.0/gyver/model.py
+-rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/py.typed
+-rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/url/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.0/gyver/url/encode.py
+-rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/path.py
+-rw-r--r--   0        0        0     3592 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/url/utils.py
+-rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/exc.py
+-rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.0/gyver/utils/helpers.py
+-rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/json.py
+-rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/lazy.py
+-rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.0/gyver/utils/singleton.py
+-rw-r--r--   0        0        0     2224 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/strings.py
+-rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.0/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     2449 2023-06-27 06:41:36.154386 gyver-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 gyver-2.3.0/PKG-INFO
```

### Comparing `gyver-2.2.0/LICENSE` & `gyver-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/README.md` & `gyver-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/asyncio.py` & `gyver-2.3.0/gyver/cache/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/interface.py` & `gyver-2.3.0/gyver/cache/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/mapper.py` & `gyver-2.3.0/gyver/cache/mapper.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/mock.py` & `gyver-2.3.0/gyver/cache/mock.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/redis.py` & `gyver-2.3.0/gyver/cache/redis.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/sync.py` & `gyver-2.3.0/gyver/cache/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/cache/utils.py` & `gyver-2.3.0/gyver/cache/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/attrs.py` & `gyver-2.3.0/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/dataclass.py` & `gyver-2.3.0/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/factory.py` & `gyver-2.3.0/gyver/config/adapter/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from gyver.attrs import define
 from gyver.attrs import mark_factory
 from pydantic import BaseModel
 
 from gyver.config.config import MISSING
 from gyver.config.config import Config
+from gyver.config.interface import ConfigLike
 from gyver.config.utils import boolean_cast
 from gyver.exc import MissingName
 from gyver.utils import finder
 from gyver.utils import json
 from gyver.utils import panic
 from gyver.utils.strings import make_lex_separator
 
@@ -31,15 +32,15 @@
 from .pydantic import PydanticResolverStrategy
 
 _default_config = Config()
 
 T = TypeVar("T")
 
 
-def _try_each(*names: str, default: Any, cast: Any, config: Config):
+def _try_each(*names: str, default: Any, cast: Any, config: ConfigLike):
     for name in names:
         with suppress(MissingName):
             return config(name, cast)
     if default is not MISSING:
         return default
     raise panic(MissingName, f"{', '.join(names)} not found and no default was given")
 
@@ -63,15 +64,15 @@
 
 def _loads(val: Any) -> Any:
     return json.loads(val) if isinstance(val, str) else val
 
 
 @define
 class AdapterConfigFactory:
-    config: Config = _default_config
+    config: ConfigLike = _default_config
 
     def get_strategy_class(self, config_class: type) -> type[FieldResolverStrategy]:
         if hasattr(config_class, "__gyver_attrs__"):
             return GyverAttrsResolverStrategy
         elif is_dataclass(config_class):
             return DataclassResolverStrategy
         elif issubclass(config_class, BaseModel):
```

### Comparing `gyver-2.2.0/gyver/config/adapter/gattrs.py` & `gyver-2.3.0/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/interface.py` & `gyver-2.3.0/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/mark.py` & `gyver-2.3.0/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/adapter/pydantic.py` & `gyver-2.3.0/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/config/config.py` & `gyver-2.3.0/gyver/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import TypeVar
 from typing import Union
 from typing import overload
 
 from gyver.attrs import define
 from gyver.attrs import info
 
+from gyver.config.interface import MISSING
+from gyver.config.interface import _default_cast
 from gyver.exc import InvalidCast
 from gyver.exc import MissingName
 from gyver.utils.exc import panic
 from gyver.utils.lazy import lazyfield
 
 T = TypeVar("T")
 
@@ -46,22 +48,14 @@
     def __len__(self) -> int:
         return len(self.mapping)
 
 
 default_mapping = EnvMapping()
 
 
-class MISSING:
-    pass
-
-
-def _default_cast(a: Any):
-    return a
-
-
 @define
 class Config:
     env_file: Union[str, Path, None] = None
     mapping: EnvMapping = default_mapping
 
     def __post_init__(self):
         if self.env_file and os.path.isfile(self.env_file):
```

### Comparing `gyver-2.2.0/gyver/config/envconfig.py` & `gyver-2.3.0/gyver/config/envconfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 from pathlib import Path
+from typing import Any
+from typing import Callable
 from typing import Sequence
 from typing import Union
 
 from gyver.attrs import call_init
 from gyver.attrs import define
 from gyver.attrs import info
 
 from gyver import utils
+from gyver.config.config import MISSING
 
 from .config import Config
 from .config import EnvMapping
 from .config import default_mapping
 from .typedef import Env
 
 
@@ -21,19 +24,24 @@
     env: Env = info(order=lambda env: env.weight)
     apply_to_lower: bool = info(default=False, order=False)
 
     def is_higher(self, env: Env) -> bool:
         return self.env.weight >= env.weight
 
 
+def default_rule(_: Env):
+    return False
+
+
 @define
 class EnvConfig(Config):
     mapping: EnvMapping = default_mapping
     env_var: str = "CONFIG_ENV"
     dotfiles: Sequence[DotFile] = ()
+    ignore_default_rule: Callable[[Env], bool] = default_rule
 
     def __init__(
         self,
         *dotfiles: DotFile,
         env_var: str = "CONFIG_ENV",
         mapping: EnvMapping = default_mapping
     ) -> None:
@@ -48,15 +56,28 @@
         if self.dotfile:
             EnvConfig.file_values.manual_set(
                 self, dict(self._read_file(self.dotfile.filename))
             )
 
     @utils.lazyfield
     def env(self):
-        return self.__call__(self.env_var, Env.new)
+        return Config.get(self, self.env_var, Env.new)
+
+    @utils.lazyfield
+    def ignore_default(self):
+        return self.ignore_default_rule(self.env)
+
+    def get(
+        self,
+        name: str,
+        cast: Callable[..., Any] = ...,
+        default: Union[Any, type[MISSING]] = ...,
+    ) -> Any:
+        default = MISSING if self.ignore_default else default
+        return super().get(name, cast, default)
 
     @utils.lazyfield
     def dotfile(self):
         """
         The dotfile function returns the dotfile object that is applicable to
         the current environment.  It traverses the list of dotfiles in reverse order,
         so that higher priority dotfiles are checked first.  If no matching dotfile is
```

### Comparing `gyver-2.2.0/gyver/config/typedef.py` & `gyver-2.3.0/gyver/config/typedef.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 class EnvTuple(NamedTuple):
     val: str
     weight: int
 
 
 class Env(EnvTuple, Enum):
-    LOCAL = "local", 1
-    TEST = "test", 2
-    DEV = "dev", 3
-    PRD = "prd", 4
+    LOCAL = EnvTuple("local", 1)
+    TEST = EnvTuple("test", 2)
+    DEV = EnvTuple("dev", 3)
+    PRD = EnvTuple("prd", 4)
 
     @property
     def value(self) -> EnvTuple:
         return super().value
 
     @property
     def val(self):
```

### Comparing `gyver-2.2.0/gyver/context/atomic_/bound.py` & `gyver-2.3.0/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/context/atomic_/core.py` & `gyver-2.3.0/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/context/atomic_/resolver.py` & `gyver-2.3.0/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/context/context.py` & `gyver-2.3.0/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/context/interfaces/adapter.py` & `gyver-2.3.0/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/crypto/fernet.py` & `gyver-2.3.0/gyver/crypto/fernet.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/crypto/rsa.py` & `gyver-2.3.0/gyver/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/__init__.py` & `gyver-2.3.0/gyver/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/adapter.py` & `gyver-2.3.0/gyver/database/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/config.py` & `gyver-2.3.0/gyver/database/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/context/asyncio.py` & `gyver-2.3.0/gyver/database/context/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/context/sync.py` & `gyver-2.3.0/gyver/database/context/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/drivers/utils.py` & `gyver-2.3.0/gyver/database/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/entity.py` & `gyver-2.3.0/gyver/database/entity.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/__init__.py` & `gyver-2.3.0/gyver/database/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/_helpers.py` & `gyver-2.3.0/gyver/database/query/_helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/comp.py` & `gyver-2.3.0/gyver/database/query/comp.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/interface.py` & `gyver-2.3.0/gyver/database/query/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/order_by.py` & `gyver-2.3.0/gyver/database/query/order_by.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/paginate.py` & `gyver-2.3.0/gyver/database/query/paginate.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/utils.py` & `gyver-2.3.0/gyver/database/query/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/query/where.py` & `gyver-2.3.0/gyver/database/query/where.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/database/utils.py` & `gyver-2.3.0/gyver/database/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/exc.py` & `gyver-2.3.0/gyver/exc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,8 @@
 
 
 class FailedFileOperation(GyverError):
     """Exception raised when an error happened while interacting with a file"""
 
 
 class MergeConflict(GyverError):
-    """Exception raised when merge_dicts(strict=True) finds a conflict"""
+    """Exception raised when merge_dicts(strict=True) finds a conflict"""
```

### Comparing `gyver-2.2.0/gyver/filetree/filetree.py` & `gyver-2.3.0/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/filetree/interface.py` & `gyver-2.3.0/gyver/filetree/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from typing import TypeVar
 from typing import cast
 
 from gyver.exc import InvalidPath
 from gyver.utils import lazyfield
 
 from .helpers import python_filename
-from .typedef import File, TextFile
+from .typedef import File
 from .typedef import Folder
 from .typedef import T
+from .typedef import TextFile
 
 FileT = TypeVar("FileT", bound=File)
 
 
 class AbstractFileTree(Protocol[T]):
     base_dir: T
```

### Comparing `gyver-2.2.0/gyver/filetree/typedef.py` & `gyver-2.3.0/gyver/filetree/typedef.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Generic
 from typing import TypeVar
 
 import cchardet
 from gyver.attrs import define
 from typing_extensions import Self
 
-from gyver.utils.lazy import lazyfield
 
 T = TypeVar("T")
 
 
 @define
 class VirtualPath(Generic[T]):
     name: str
@@ -77,18 +76,15 @@
     def read(self, size: int = -1) -> str:
         return self.contents.read(size).decode(self.encoding)
 
     def readline(self, size: int = -1) -> str:
         return self.contents.readline(size).decode(self.encoding)
 
     def readlines(self, hint: int = -1) -> list[str]:
-        return [
-            line.decode(self.encoding)
-            for line in self.contents.readlines(hint)
-        ]
+        return [line.decode(self.encoding) for line in self.contents.readlines(hint)]
 
     def write(self, text: str) -> int:
         return self.contents.write(text.encode(self.encoding))
 
     def writelines(self, lines: list[str]):
         encoded_lines = [line.encode(self.encoding) for line in lines]
         self.contents.writelines(encoded_lines)
```

### Comparing `gyver-2.2.0/gyver/filetree/virtual.py` & `gyver-2.3.0/gyver/filetree/virtual.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,15 @@
         return self.base_dir
 
     @property
     def name(self):
         return self.root.name
 
     def from_virtual(
-        self,
-        virtual_filetree: "VirtualFileTree",
-        *path: str,
-        strict: bool = True
+        self, virtual_filetree: "VirtualFileTree", *path: str, strict: bool = True
     ):
         target = self.root
         for item in path:
             if item not in target.contents:
                 target.contents[item] = Folder.new(item)
             target = target.contents[item]
             if isinstance(target, File):
@@ -42,21 +39,17 @@
         if current_value is not None:
             if isinstance(current_value, File):
                 raise InvalidPath("Foldername conflicts with file")
             elif isinstance(current_value, Folder) and current_value.contents:
                 if not strict:
                     self._try_merge(current_value, virtual_filetree.root)
                 else:
-                    raise InvalidPath(
-                        "Non-empty folder with same name already exists"
-                    )
+                    raise InvalidPath("Non-empty folder with same name already exists")
 
-        target.contents[virtual_filetree.name] = (
-            current_value or virtual_filetree.root
-        )
+        target.contents[virtual_filetree.name] = current_value or virtual_filetree.root
         return virtual_filetree.root
 
     def _try_merge(self, current_target: Folder, virtual_folder: Folder):
         stack = deque([(current_target.contents, virtual_folder.contents)])
         while stack:
             current_contents, virtual_contents = stack.pop()
             for value in current_contents.values():
@@ -65,17 +58,15 @@
                     and value.name in virtual_contents
                     and isinstance(virtual_contents[value.name], Folder)
                 ):
                     stack.append(
                         (value.contents, virtual_contents[value.name].contents)
                     )
             current_contents.update(
-                merge_dicts(
-                    current_contents, virtual_contents, on_conflict="left"
-                )
+                merge_dicts(current_contents, virtual_contents, on_conflict="left")
             )
 
     @contextmanager
     def virtual_context(self, dirname: str, *path: str):
         try:
             folder = self.get_dir(dirname, *path) or Folder.new(dirname)
             vt = VirtualFileTree(folder)
```

### Comparing `gyver-2.2.0/gyver/model.py` & `gyver-2.3.0/gyver/model.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/pools/asyncio.py` & `gyver-2.3.0/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/pools/resource.py` & `gyver-2.3.0/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/pools/thread.py` & `gyver-2.3.0/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/utils/__init__.py` & `gyver-2.3.0/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/utils/finder.py` & `gyver-2.3.0/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/utils/helpers.py` & `gyver-2.3.0/gyver/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from collections import deque
 import functools
-from itertools import chain
 import warnings
-from typing import Callable, Literal
+from collections import deque
+from itertools import chain
+from typing import Callable
+from typing import Literal
 from typing import TypeVar
 from typing import cast
 
 from gyver.attrs import define
 from typing_extensions import ParamSpec
+
 from gyver.exc import MergeConflict
 
 from .exc import panic
 
 
 def _not_implemented(msg: str):
     def inner(*_, **__kwds__):
@@ -98,19 +100,15 @@
 
         for key, value in right_curr.items():
             if key not in left_curr:
                 output_curr[key] = value
             elif isinstance(value, (list, set, tuple)) and merge_sequences:
                 left_val = left_curr[key]
                 if isinstance(left_val, (list, set, tuple)):
-                    type_ = (
-                        type(value)
-                        if on_conflict == "right"
-                        else type(left_val)
-                    )
+                    type_ = type(value) if on_conflict == "right" else type(left_val)
                     output_curr[key] = type_(chain(left_val, value))
             elif isinstance(value, dict):
                 if isinstance(left_curr[key], dict):
                     output_curr[key] = {
                         lkey: lvalue
                         for lkey, lvalue in left_curr[key].items()
                         if lkey not in value
```

### Comparing `gyver-2.2.0/gyver/utils/lazy.py` & `gyver-2.3.0/gyver/utils/lazy.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     def __get__(
         self,
         instance: typing.Optional[SelfT],
         owner: typing.Optional[type[SelfT]] = None,
     ) -> typing.Union[T, Self]:
         if not instance:
             return self
-        assert instance is not None
         try:
             val = typing.cast(
                 T,
                 object.__getattribute__(
                     instance,
                     self.private_name,
                 ),
```

### Comparing `gyver-2.2.0/gyver/utils/singleton.py` & `gyver-2.3.0/gyver/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `gyver-2.2.0/gyver/utils/strings.py` & `gyver-2.3.0/gyver/utils/strings.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,14 +45,27 @@
 
 OuterCastT = TypeVar("OuterCastT", list, tuple, set)
 
 
 def make_lex_separator(
     outer_cast: type[OuterCastT], cast: type = str
 ) -> Callable[[str], OuterCastT]:
+    """
+    Create a lexer-based separator function.
+
+    :param outer_cast: The type to cast the resulting separated values into (e.g., list, tuple, set).
+    :param cast: The type to which each individual item will be cast (default: str).
+    :return: A callable that separates a string into an instance of outer_cast with casted items.
+
+    Usage example:
+    comma_separated = make_lex_separator(tuple, str)
+    result = comma_separated("a, b, c")
+    print(result)  # Output: ('a', 'b', 'c')
+    """
+
     def wrapper(value: str) -> OuterCastT:
         lex = shlex.shlex(value, posix=True)
         lex.whitespace = ","
         lex.whitespace_split = True
         return outer_cast(cast(item.strip()) for item in lex)
 
     return wrapper
```

### Comparing `gyver-2.2.0/pyproject.toml` & `gyver-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "2.2.0"
+version = "2.3.0"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-2.2.0/PKG-INFO` & `gyver-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 2.2.0
+Version: 2.3.0
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

