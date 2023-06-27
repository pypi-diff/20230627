# Comparing `tmp/kaiju_redis-2.0.5-py3-none-any.whl.zip` & `tmp/kaiju_redis-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,12 @@
-Zip file size: 10605 bytes, number of entries: 17
--rw-r--r--  2.0 unx      367 b- defN 23-Apr-21 19:33 kaiju_redis/__init__.py
--rw-r--r--  2.0 unx     6197 b- defN 23-Apr-21 19:33 kaiju_redis/cache.py
--rw-r--r--  2.0 unx     3358 b- defN 23-Apr-21 19:33 kaiju_redis/locks.py
--rw-r--r--  2.0 unx      327 b- defN 23-Apr-21 19:33 kaiju_redis/services.py
--rw-r--r--  2.0 unx     5451 b- defN 23-Apr-21 19:33 kaiju_redis/streams.py
--rw-r--r--  2.0 unx     1521 b- defN 23-Apr-21 19:33 kaiju_redis/transport.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 19:33 kaiju_redis/tests/__init__.py
--rw-r--r--  2.0 unx     2175 b- defN 23-Apr-21 19:33 kaiju_redis/tests/fixtures.py
--rw-r--r--  2.0 unx      255 b- defN 23-Apr-21 19:33 kaiju_redis/tests/test_cache.py
--rw-r--r--  2.0 unx      270 b- defN 23-Apr-21 19:33 kaiju_redis/tests/test_locks.py
--rw-r--r--  2.0 unx      272 b- defN 23-Apr-21 19:33 kaiju_redis/tests/test_streams.py
--rw-r--r--  2.0 unx      207 b- defN 23-Apr-21 19:33 kaiju_redis/tests/test_transport.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Apr-21 19:33 kaiju_redis-2.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2906 b- defN 23-Apr-21 19:33 kaiju_redis-2.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 19:33 kaiju_redis-2.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-21 19:33 kaiju_redis-2.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1400 b- defN 23-Apr-21 19:33 kaiju_redis-2.0.5.dist-info/RECORD
-17 files, 25420 bytes uncompressed, 8293 bytes compressed:  67.4%
+Zip file size: 8995 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 19:32 kaiju_redis/__init__.py
+-rw-r--r--  2.0 unx    14978 b- defN 23-Jun-27 19:32 kaiju_redis/services.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 19:32 kaiju_redis/tests/__init__.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jun-27 19:32 kaiju_redis/tests/fixtures.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jun-27 19:32 kaiju_redis/tests/test_redis.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3002 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/RECORD
+10 files, 26668 bytes uncompressed, 7585 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,52 +1,31 @@
 Filename: kaiju_redis/__init__.py
 Comment: 
 
-Filename: kaiju_redis/cache.py
-Comment: 
-
-Filename: kaiju_redis/locks.py
-Comment: 
-
 Filename: kaiju_redis/services.py
 Comment: 
 
-Filename: kaiju_redis/streams.py
-Comment: 
-
-Filename: kaiju_redis/transport.py
-Comment: 
-
 Filename: kaiju_redis/tests/__init__.py
 Comment: 
 
 Filename: kaiju_redis/tests/fixtures.py
 Comment: 
 
-Filename: kaiju_redis/tests/test_cache.py
-Comment: 
-
-Filename: kaiju_redis/tests/test_locks.py
-Comment: 
-
-Filename: kaiju_redis/tests/test_streams.py
-Comment: 
-
-Filename: kaiju_redis/tests/test_transport.py
+Filename: kaiju_redis/tests/test_redis.py
 Comment: 
 
-Filename: kaiju_redis-2.0.5.dist-info/LICENSE
+Filename: kaiju_redis-2.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_redis-2.0.5.dist-info/METADATA
+Filename: kaiju_redis-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_redis-2.0.5.dist-info/WHEEL
+Filename: kaiju_redis-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_redis-2.0.5.dist-info/top_level.txt
+Filename: kaiju_redis-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_redis-2.0.5.dist-info/RECORD
+Filename: kaiju_redis-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_redis/__init__.py

```diff
@@ -1,11 +1,5 @@
-"""Module SHOULD usually contain only the package meta-information and imports from the package's modules.
-
-This docstring SHOULD contain the general package description and the user guide,
-because this section is shown the first in the package index.
-"""
+from .services import *
 
-__version__ = '2.0.5'
+__version__ = '2.1.0'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
-
-from .services import *
```

## kaiju_redis/services.py

```diff
@@ -1,12 +1,441 @@
-"""
-This module SHOULD only contain imports of service classes.
+"""Redis services."""
 
-The reason of this module is to feed it to the service class registry for fast
-class creation, so it should only contain the imports you need to register
-as services.
-"""
-
-from .transport import *
-from .cache import *
-from .locks import *
-from .streams import *
+import textwrap
+from typing import Collection, FrozenSet, Type, List
+
+from kaiju_tools import NSKey
+from kaiju_tools.app import service_class_registry
+
+from coredis import Redis, RedisCluster  # noqa: pycharm
+from coredis.exceptions import ResponseError, StreamConsumerGroupError  # noqa: pycharm
+
+from kaiju_tools.app import ContextableService
+from kaiju_tools.cache import BaseCacheService
+from kaiju_tools.encoding import msgpack_dumps, msgpack_loads
+from kaiju_tools.functions import retry
+from kaiju_tools.locks import BaseLocksService, NotLockOwnerError, LockExistsError
+from kaiju_tools.streams import StreamRPCClient, Listener
+
+__all__ = ['RedisTransportService', 'RedisCacheService', 'RedisLocksService', 'RedisListener', 'RedisStreamRPCClient']
+
+
+class RedisTransportService(ContextableService):
+    """Redis transport."""
+
+    transport_class = Redis
+    cluster_transport_class = RedisCluster
+
+    def __init__(
+        self,
+        app,
+        *args,
+        cluster: bool = False,
+        connect_timeout: int = 30,
+        max_idle_time: int = 60,
+        retry_on_timeout=True,
+        logger=None,
+        **kws,
+    ):
+        """Initialize.
+
+        :param app:
+        :param args: additional transport cls args
+        :param cluster: use cluster connector class
+        :param connect_timeout: connection timeout
+        :param max_idle_time: max connection idle time
+        :param retry_on_timeout: retry connection on timeout
+        :param logger:
+        :param kws: additional transport cls args
+        """
+        ContextableService.__init__(self, app, logger=logger)
+        if cluster:
+            cls = self.cluster_transport_class
+        else:
+            cls = self.transport_class
+        self._transport = cls(
+            *args,
+            connect_timeout=connect_timeout,
+            max_idle_time=max_idle_time,
+            retry_on_timeout=retry_on_timeout,
+            **kws,
+        )
+
+    def __getattr__(self, item):
+        return getattr(self._transport, item)
+
+    async def init(self):
+        self.connection_pool.reset()
+
+    async def close(self):
+        self.connection_pool.disconnect()
+
+
+class RedisCacheService(BaseCacheService):
+    """Provides caching via Redis or KeyDB."""
+
+    M_SET_EXP_SCRIPT = """
+    local ttl = ARGV[1]
+    for i, key in pairs(KEYS) do
+        redis.call('SETEX', key, ttl, ARGV[i + 1])
+    end
+    """
+
+    M_EXISTS_SCRIPT = """
+    local result = {}
+    for i, key in pairs(KEYS) do
+        result[i] = redis.call('EXISTS', key)
+    end
+    return result
+    """
+
+    _m_set_exp_script = None  #: compiled script
+    _m_exists_script = None  #: compiled script
+    _transport: RedisTransportService
+
+    async def init(self):
+        await super().init()
+        self._m_set_exp_script = self._transport.register_script(textwrap.dedent(self.M_SET_EXP_SCRIPT))
+        self._m_exists_script = self._transport.register_script(textwrap.dedent(self.M_EXISTS_SCRIPT))
+
+    @classmethod
+    def get_transport_cls(cls) -> Type:
+        return RedisTransportService
+
+    async def exists(self, id: NSKey) -> bool:
+        existing = await self._transport.exists([id])
+        return bool(existing)
+
+    async def m_exists(self, id: Collection[NSKey]) -> FrozenSet[str]:
+        keys = await self._m_exists_script.execute(keys=id)
+        return frozenset(key for key, value in zip(id, keys) if bool(value))
+
+    async def _get(self, key: str):
+        return await self._transport.get(key)
+
+    async def _m_get(self, *keys: str):
+        return await self._transport.mget(keys)
+
+    async def _set(self, key: str, value, ttl: int):
+        if ttl:
+            return await self._transport.setex(key, value, ttl)
+        else:
+            return await self._transport.set(key, value)
+
+    async def _m_set(self, keys: dict, ttl: int):
+        if ttl:
+            return await self._m_set_exp_script.execute(keys=list(keys.keys()), args=[ttl, *list(keys.values())])
+        else:
+            return await self._transport.mset(keys)
+
+    async def _delete(self, key: str):
+        return await self._transport.delete([key])
+
+    async def _m_delete(self, *keys: str):
+        self.logger.info('DELETE')
+        try:
+            await self._transport.delete(keys)
+        except Exception as exc:
+            self.logger.info(str(exc))
+        self.logger.info('OK')
+
+    async def lpush(
+        self,
+        key: NSKey,
+        *values,
+    ) -> None:
+        """Set a list data into list.
+
+        :param key: string only
+        :param values: list of serializable value
+        """
+        self.logger.info('Add key "%s"', key)
+        values = [self._dump_value(v) for v in values]
+        await self._transport.lpush(key, values)
+
+    async def rpush(self, key: NSKey, *values) -> None:
+        """Set a list data into list.
+
+        :param key: string only
+        :param values: list of serializable value
+        """
+        self.logger.info('Add key "%s"', key)
+        values = [self._dump_value(v) for v in values]
+        await self._transport.rpush(key, values)
+
+    async def llen(self, key: NSKey) -> int:
+        """Get count of list.
+
+        :param key: string only
+        """
+        self.logger.info('Get key count "%s"', key)
+        return await self._transport.llen(key)
+
+    async def lrange(self, key: NSKey, start=0, end=10):
+        """Get values from list by key.
+
+        :param key: string only
+        :param start: positive int only
+        :param end: positive int only
+        """
+        self.logger.info('Set range for key %s .', key)
+        values = await self._transport.lrange(key, start=start, stop=end)
+        if values:
+            values = [self._load_value(v) for v in values]
+        return values
+
+    async def lpop(self, key: NSKey):
+        """Get values from list by key.
+
+        :param key: string only
+        """
+        self.logger.info('Set range for key %s .', key)
+        value = await self._transport.lpop(key)
+        if value:
+            value = self._load_value(value)
+        return value
+
+
+class RedisLocksService(BaseLocksService):
+    """Locks service with Redis backend."""
+
+    class ErrorCode:
+        """Error codes used by redis scripts."""
+
+        OK = 'OK'
+        LOCK_EXISTS = 'LOCK_EXISTS'
+        NOT_LOCK_OWNER = 'NOT_LOCK_OWNER'
+
+    LOCK_SCRIPT = f"""
+    local e = redis.call('get', KEYS[1])
+    if not e then
+        redis.call('set', KEYS[1], ARGV[1])
+        redis.call('expire', KEYS[1], ARGV[2])
+        return redis.status_reply('{ErrorCode.OK}')
+    else
+        return redis.error_reply('{ErrorCode.LOCK_EXISTS}')
+    end"""
+
+    UNLOCK_SCRIPT = f"""
+    local _id = redis.call('get', KEYS[1])
+    if _id == ARGV[1] then
+        redis.call('del', KEYS[1])
+        return redis.status_reply('{ErrorCode.OK}')
+    elseif not _id then
+        return redis.status_reply('{ErrorCode.OK}')
+    else
+        return redis.error_reply('{ErrorCode.NOT_LOCK_OWNER}')
+    end"""
+
+    RENEW_SCRIPT = """
+    for i, key in pairs(KEYS) do
+        redis.call('expire', key, ARGV[i])
+    end
+    """
+
+    EXISTS_SCRIPT = RedisCacheService.M_EXISTS_SCRIPT
+    _lock_script = None
+    _unlock_script = None
+    _renew_script = None
+    _exists_script = None
+    _transport: RedisTransportService
+
+    async def init(self):
+        await super().init()
+        self._lock_script = self._transport.register_script(textwrap.dedent(self.LOCK_SCRIPT))
+        self._unlock_script = self._transport.register_script(textwrap.dedent(self.UNLOCK_SCRIPT))
+        self._renew_script = self._transport.register_script(textwrap.dedent(self.RENEW_SCRIPT))
+        self._exists_script = self._transport.register_script(textwrap.dedent(self.EXISTS_SCRIPT))
+
+    @classmethod
+    def get_transport_cls(cls) -> Type:
+        return RedisTransportService
+
+    async def m_exists(self, keys: List[NSKey]) -> FrozenSet[NSKey]:
+        data = await self._exists_script.execute(keys=keys)
+        if data:
+            return frozenset(key for key, value in zip(keys, data) if bool(value))
+        else:
+            return frozenset()
+
+    async def _acquire(self, keys: list, identifier: str, ttl: int):
+        try:
+            await self._lock_script.execute(keys=keys, args=[identifier, int(ttl)])
+        except ResponseError as exc:
+            if str(exc) == self.ErrorCode.LOCK_EXISTS:
+                exc = LockExistsError(self.ErrorCode.LOCK_EXISTS)
+            raise exc
+
+    async def _release(self, keys: list, identifier: str):
+        try:
+            await self._unlock_script.execute(keys=keys, args=[identifier])
+        except ResponseError as exc:
+            if str(exc) == self.ErrorCode.NOT_LOCK_OWNER:
+                exc = NotLockOwnerError(self.ErrorCode.NOT_LOCK_OWNER)
+            raise exc
+
+    async def _renew(self, keys: list, values: list):
+        await self._renew_script.execute(keys=keys, args=[int(v) for v in values])
+
+    async def _owner(self, key: str):
+        owner = await self._transport.get(key)
+        if owner:
+            owner = owner.decode('utf-8')
+            return owner
+
+
+class RedisListener(Listener):
+    """Redis stream listener."""
+
+    _transport: RedisTransportService
+    _loads = msgpack_loads
+    _trim_interval = 120  # s
+    _trim_op = b'~'  # either ~ or =
+
+    def __init__(
+        self,
+        *args,
+        group_id: str = None,
+        consumer_id: str = None,
+        max_batch_size: int = 10,
+        max_wait_time_ms: int = 500,
+        pending_messages_time_ms: int = None,
+        trim_size: int = None,
+        **kws,
+    ):
+        """Initialize.
+
+        :param group_id: consumer group, `app.name` by default
+        :param consumer_id: unique instance id, `app.id` by default
+        :param max_batch_size: max single acquired batch size
+        :param max_wait_time_ms: max wait time when waiting for a batch
+        :param pending_messages_time_ms: processing pending messages timeout in ms
+            (messages not acked since this interval will be auto-claimed by this listener)
+            set `None` to disable this behavior
+        :param trim_size: stream records trim size: older records will be removed
+            if the stream is longer than this value
+            set `None` to disable this behavior
+        """
+        super().__init__(*args, **kws)
+        self.group_id = group_id if group_id else self.app.name
+        self.consumer_id = consumer_id if consumer_id else str(self.app.id)
+        self.max_batch_size = max_batch_size
+        self.max_wait_time_ms = max_wait_time_ms
+        self.pending_messages_time_ms = pending_messages_time_ms
+        self.trim_size = trim_size
+        self._task_claim_pending = None
+        self._task_trim_records = None
+
+    async def init(self):
+        await self._create_group()
+        if self.pending_messages_time_ms:
+            interval = max(1, self.pending_messages_time_ms // 1000)
+            self._task_claim_pending = self._scheduler.schedule_task(
+                self._claim_pending, interval=interval, name=f'{self.service_name}._claim_pending'
+            )
+        if self.trim_size:
+            self._task_trim_records = self._scheduler.schedule_task(
+                self._trim_records, interval=self._trim_interval, name=f'{self.service_name}._trim_records'
+            )
+        await super().init()
+
+    async def close(self):
+        if self._task_claim_pending:
+            self._task_claim_pending.enabled = False
+        if self._task_trim_records:
+            self._task_trim_records.enabled = False
+        await super().close()
+
+    async def _create_group(self) -> None:
+        self.logger.info('Creating group %s for stream %s', self.group_id, self._key)
+        try:
+            groups = await self._transport.xinfo_groups(self._key)
+            self.logger.debug('groups: %s', groups)
+        except ResponseError:
+            groups, mk_stream = frozenset(), True
+        else:
+            groups, mk_stream = frozenset(group[b'name'].decode() for group in groups), False
+        if self.group_id not in groups:
+            result = await self._transport.xgroup_create(self._key, self.group_id, identifier='$', mkstream=mk_stream)
+            self.logger.debug('group create: %s', result)
+
+    @classmethod
+    def get_transport_cls(cls) -> Type:
+        return RedisTransportService
+
+    async def _read_batch(self) -> list:
+        try:
+            batch = await self._transport.xreadgroup(
+                self.group_id,
+                self.consumer_id,
+                count=self.max_batch_size,
+                block=self.max_wait_time_ms,
+                streams={self._key: '>'},
+                noack=True,
+            )
+        except StreamConsumerGroupError:
+            await self._create_group()
+        else:
+            if batch:
+                batch = next(iter(batch.values()), None)  # first topic, there should only be a single topic
+                return batch
+
+    async def _claim_pending(self) -> None:
+        """Claim pending messages."""
+        await self._transport.xautoclaim(
+            self._key, self.group_id, self.consumer_id, self.pending_messages_time_ms, justid=True
+        )
+
+    async def _trim_records(self) -> None:
+        """Trim older records."""
+        result = await self._transport.xtrim(
+            self._key, trim_strategy=b'MAXLEN', threshold=self.trim_size, trim_operator=self._trim_op
+        )
+        self.logger.debug('trim: %s', result)
+
+    async def _process_batch(self, batch: list) -> None:
+        acks = []
+        for row in batch:
+            row_id, data = row
+            data = self._loads(data[b'_'])
+            await self._process_request(data)
+            acks.append(row_id)
+        if acks:
+            await retry(
+                self._transport.xack,
+                args=(self._key, self.group_id),
+                kws={'identifiers': acks},
+                retries=5,
+                retry_timeout=1.0,
+                max_retry_timeout=10,
+                logger=self.logger,
+            )
+
+
+class RedisStreamRPCClient(StreamRPCClient):
+    """Redis stream client."""
+
+    _transport: RedisTransportService
+    _dumps = msgpack_dumps
+
+    @classmethod
+    def get_transport_cls(cls) -> Type:
+        return RedisTransportService
+
+    async def write(self, body, headers: dict = None, key=None) -> None:
+        """Write data to the stream.
+
+        :param body: rpc request body
+        :param headers: request headers
+        :param key: (optional) message id
+        """
+        msg = await self._transport.xadd(
+            self._topic, {b'_': self._dumps((body, headers))}, identifier=key if key else '*'
+        )
+        self.logger.debug('write: %s', msg)
+
+
+service_class_registry.register_class(RedisTransportService)
+service_class_registry.register_class(RedisCacheService)
+service_class_registry.register_class(RedisLocksService)
+service_class_registry.register_class(RedisListener)
+service_class_registry.register_class(RedisStreamRPCClient)
```

## kaiju_redis/tests/fixtures.py

```diff
@@ -1,76 +1,112 @@
-"""Place your pytest fixtures here."""
+import pytest  # noqa: pycharm
 
-import pytest
-
-from kaiju_tools.streams.etc import Topics
-from kaiju_tools.docker import DockerContainer
-from kaiju_tools.tests.fixtures import *
-from kaiju_tools.rpc.tests.fixtures import *
-
-from ..services import *
+from kaiju_tools.docker import DockerContainer, DockerImage
+from kaiju_tools.streams import Topic
+from kaiju_tools.tests.fixtures import get_app
+
+from kaiju_redis.services import *
+
+__all__ = [
+    'redis',
+    'redis_glob',
+    'redis_cache',
+    'redis_locks',
+    'redis_listener',
+    'redis_client',
+    'redis_transport',
+    'REDIS_PORT',
+]
 
 REDIS_PORT = 6399
 
 
-def _redis_container(logger):
+def _redis_container(app):
     return DockerContainer(
-        image={'tag': 'eqalpha/keydb', 'version': 'latest'},
+        app=app,
+        image=DockerImage(app=app, tag='eqalpha/keydb', version='latest'),
         name='pytest-redis',
         ports={'6379': str(REDIS_PORT)},
         healthcheck={
             'test': "echo 'INFO' | keydb-cli",
             'interval': 100000000,
             'timeout': 3000000000,
             'start_period': 1000000000,
             'retries': 3,
         },
-        sleep_interval=0.5,
+        sleep_interval=1,
         remove_on_exit=True,
-        logger=logger,
     )
 
 
 @pytest.fixture
-def redis(logger):
-    """Return a new redis container. See `kaiju_tools.tests.fixtures.container` for more info."""
-    with _redis_container(logger) as c:
+def redis(app):
+    """Get a new redis container."""
+    with _redis_container(app) as c:
         yield c
 
 
 @pytest.fixture(scope='session')
-def per_session_redis(logger):
-    """Return a new redis container. See `kaiju_tools.tests.fixtures.container` for more info."""
-    with _redis_container(logger) as c:
+def redis_glob(logger):
+    """Get a new redis container."""
+    app = get_app(logger)
+    with _redis_container(app) as c:
         yield c
 
 
 @pytest.fixture
-def redis_transport(application, logger):
-    """Get transport class."""
-    return RedisTransportService(app=application(), host='localhost', port=REDIS_PORT, logger=logger)
+def redis_transport(redis_glob, app) -> RedisTransportService:
+    """Get redis transport."""
+    service = RedisTransportService(app=app, host='localhost', port=REDIS_PORT)
+    app.services.add_service(service)
+    return service
 
 
 @pytest.fixture
-def redis_cache(redis_transport, logger):
-    """Get cache class."""
-    return RedisCacheService(app=redis_transport.app, transport=redis_transport, logger=logger)
+def redis_cache(app, redis_transport) -> RedisCacheService:
+    """Get redis cache."""
+    service = RedisCacheService(app=app, transport=redis_transport)
+    app.services.add_service(service)
+    return service
 
 
 @pytest.fixture
-def redis_locks(redis_transport, logger):
+def redis_locks(app, redis_transport, scheduler) -> RedisLocksService:
     """Get locks class."""
-    return RedisLocksService(app=redis_transport.app, transport=redis_transport, logger=logger)
+    service = RedisLocksService(app=app, transport=redis_transport, scheduler=scheduler)
+    app.services.add_service(service)
+    return service
+
+
+@pytest.fixture
+def redis_listener(app, rpc, mock_sessions, mock_auth, scheduler, mock_locks, redis_transport) -> RedisListener:
+    """Get stream listener class."""
+    service = RedisListener(
+        app=app,
+        topic=Topic.RPC,
+        transport=redis_transport,
+        rpc_service=rpc,
+        scheduler=scheduler,
+        session_service=mock_sessions,
+        authentication_service=mock_auth,
+        locks_service=mock_locks,
+        max_batch_size=1,
+        max_wait_time_ms=50,
+    )
+    app.services.add_service(service)
+    return service
 
 
 @pytest.fixture
-def redis_listener(redis_transport, redis_locks, rpc_interface, logger):
+def redis_client(app, redis_transport, mock_users) -> RedisStreamRPCClient:
     """Get stream listener class."""
-    return RedisListener(
-        app=redis_transport.app,
-        topics=[Topics.rpc, Topics.callback],
+    service = RedisStreamRPCClient(
+        app=app,
+        app_name=app.name,
+        topic=Topic.RPC,
+        request_logs=True,
+        response_logs=True,
         transport=redis_transport,
-        rpc_service=rpc_interface,
-        locks_service=redis_locks,
-        consumer_settings={'group_id': 'pytest', 'timeout_ms': 100},
-        logger=logger,
+        auth_str=f'Basic {mock_users.username}:{mock_users.password}',
     )
+    app.services.add_service(service)
+    return service
```

## Comparing `kaiju_redis-2.0.5.dist-info/LICENSE` & `kaiju_redis-2.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_redis-2.0.5.dist-info/METADATA` & `kaiju_redis-2.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-redis
-Version: 2.0.5
+Version: 2.1.0
 Summary: Redis and keydb services
 Home-page: https://gitlab.com/kaiju-python/kaiju-redis
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,31 +14,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hiredis (>=2.2.2)
-Requires-Dist: coredis (>=4.11.5)
-Requires-Dist: kaiju-tools (<3,>=2.0.49)
+Requires-Dist: hiredis (>=2.2.3)
+Requires-Dist: coredis (>=4.14.0)
+Requires-Dist: kaiju-tools (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
 Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
 Requires-Dist: pydocstyle (>=6.3) ; extra == 'dev'
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
+Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
+Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.2) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
 Requires-Dist: docker (>=6.0) ; extra == 'test'
```

