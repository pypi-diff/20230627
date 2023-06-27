# Comparing `tmp/gspot_fastapi_auth-0.0.3.tar.gz` & `tmp/gspot_fastapi_auth-0.0.3b0.tar.gz`

## Comparing `gspot_fastapi_auth-0.0.3.tar` & `gspot_fastapi_auth-0.0.3b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/requirements.in
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/requirements.txt
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/example/main.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/example/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/__init__.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/auth.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/base.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/models.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/permissions.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/providers.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/services.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/settings.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/test_factory.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/tests/tests.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/requirements.in
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/requirements.txt
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/example/main.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/example/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/__init__.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/auth.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/base.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/models.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/permissions.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/providers.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/services.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/settings.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/test_factory.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/tests/tests.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/LICENSE
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/pyproject.toml
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3b0/PKG-INFO
```

### Comparing `gspot_fastapi_auth-0.0.3/.pre-commit-config.yaml` & `gspot_fastapi_auth-0.0.3b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/requirements.txt` & `gspot_fastapi_auth-0.0.3b0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,26 +31,26 @@
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
 factory-boy==3.2.1
     # via
     #   -r requirements.in
     #   gspot-fastapi-auth
-faker==18.11.1
+faker==18.11.2
     # via
     #   -r requirements.in
     #   factory-boy
     #   gspot-fastapi-auth
 fastapi==0.98.0
     # via
     #   -r requirements.in
     #   gspot-fastapi-auth
 flake8==6.0.0
     # via -r requirements.in
-gspot-fastapi-auth==0.0.1
+gspot-fastapi-auth==0.0.3
     # via -r requirements.in
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
 httpcore==0.17.2
     # via httpx
```

### Comparing `gspot_fastapi_auth-0.0.3/example/main.py` & `gspot_fastapi_auth-0.0.3b0/example/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from src.gspot_fastapi_auth import token_config
 from src.gspot_fastapi_auth.providers import RedisSingleton
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
     RedisSingleton.init_redis(
-        token_config.host,
-        token_config.port,
-        token_config.db,
-        token_config.password
+        token_config.HOST,
+        token_config.PORT,
+        token_config.DB,
+        token_config.PASSWORD
     )
     yield
-    RedisSingleton().close()
+    await RedisSingleton().close()
 
 
 app = FastAPI(lifespan=lifespan)
 
 
 @app.get("/")
 async def read_root(user=Depends(UserRedisAuth())):
```

### Comparing `gspot_fastapi_auth-0.0.3/example/tests.py` & `gspot_fastapi_auth-0.0.3b0/example/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/auth.py` & `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from typing import Type
 
 from fastapi import HTTPException, Request
 from fastapi.security import HTTPBearer, OAuth2PasswordBearer
 from starlette.status import HTTP_401_UNAUTHORIZED
 
 from .models import BaseUser, UserFactory
-from .providers import RedisClient
+from .providers import RedisClient, RedisSingleton
 from .services import TokenService
 from .settings import token_config
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl='token')
 
 
 class UserRedisAuth(HTTPBearer):
     def __init__(self, *args, **kwargs):
         super(UserRedisAuth, self).__init__(*args, **kwargs)
-        self._redis_client = RedisClient(
-            token_config.host,
-            token_config.port,
-            token_config.db,
-            token_config.password,
-        )
-        self.token_service = TokenService(self._redis_client.session)
+        self.token_service = TokenService(RedisSingleton().session)
 
     @staticmethod
     def _get_token_from_headers(request: Request) -> str:
         token = request.headers.get('HTTP_AUTHORIZATION')
         if not token:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         return token
@@ -34,15 +28,15 @@
     def _get_token_from_cookies(request: Request) -> str:
         token = request.cookies.get('Authentication')
         if not token:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         return token
 
     async def __call__(self, request: Request) -> Type[BaseUser]:
-        if token_config.storage == 'headers':
+        if token_config.TOKEN_STORAGE == 'headers':
             token = self._get_token_from_headers(request)
         else:
             token = self._get_token_from_cookies(request)
         data = await self.token_service.get_token_data(token)
         if not data:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         user_class = UserFactory().get_user(data.pop('role'))
```

### Comparing `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/models.py` & `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/permissions.py` & `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/providers.py` & `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/providers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import redis.asyncio as redis
 
 from .settings import token_config
 
 
 class RedisClient:
     def __init__(self, host: str, port: int, db: int, password: str):
-        self.host = host
-        self.port = port
-        self.db = db
-        self.password = password
         self.session = redis.Redis(
-            host=self.host,
-            port=self.port,
-            db=self.db,
-            password=self.password,
+            host=host,
+            port=port,
+            db=db,
+            password=password,
         )
 
     async def close(self):
         await self.session.close()
 
 
 class RedisSingleton:
-    _instance: RedisClient
+    _instance: RedisClient = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
-            cls._instance = RedisClient(token_config.host, token_config.port, token_config.db, token_config.password)
+            cls._instance = RedisClient(
+                token_config.HOST,
+                token_config.PORT,
+                token_config.DB,
+                token_config.PASSWORD
+            )
         return cls._instance
 
     @classmethod
     def init_redis(cls, host: str, port: int, db: int, password: str):
         cls._instance = RedisClient(host, port, db, password)
-
```

### Comparing `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/test_factory.py` & `gspot_fastapi_auth-0.0.3b0/src/gspot_fastapi_auth/test_factory.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/tests/tests.py` & `gspot_fastapi_auth-0.0.3b0/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,51 +4,65 @@
 
 from fastapi import Request
 
 from src.gspot_fastapi_auth.auth import UserRedisAuth
 from src.gspot_fastapi_auth.providers import RedisClient
 from src.gspot_fastapi_auth.services import TokenService
 from src.gspot_fastapi_auth.settings import token_config
-from src.gspot_fastapi_auth.test_factory import AdminUserFactory, CustomerUserFactory
+from src.gspot_fastapi_auth.test_factory import AdminUserFactory, CustomerUserFactory, DeveloperUserFactory
 
 
 class TestRedisService(IsolatedAsyncioTestCase):
 
     @mock.patch('redis.asyncio.Redis.get', new_callable=AsyncMock)
     async def test_010_get_token(self, redis_mock):
         redis_client = RedisClient(
-            token_config.host,
-            token_config.port,
-            token_config.db,
-            token_config.port
+            token_config.HOST,
+            token_config.PORT,
+            token_config.DB,
+            token_config.PASSWORD
         )
         token_service = TokenService(redis_client.session)
         mock_value = b'{"123": "123"}'
         redis_mock.return_value = mock_value
         value = await token_service.get_token_data('123')
         self.assertEqual(json.loads(mock_value), value)
 
     @mock.patch('redis.asyncio.Redis.get', new_callable=AsyncMock)
     async def test_020_get_valid_from_headers(self, redis_mock):
-        token_config.storage = 'headers'
+        token_config.TOKEN_STORAGE = 'headers'
         admin_data = AdminUserFactory().to_dict()
         admin_data['role'] = 'administrator'
         redis_mock.return_value = json.dumps(admin_data)
         mock_request = mock.create_autospec(Request)
         mock_request.headers.get.return_value = '123'
         auth_service = UserRedisAuth()
         user = await auth_service(mock_request)
         admin_data.pop('role')
         self.assertEqual(admin_data, user.to_dict())
 
     @mock.patch('redis.asyncio.Redis.get', new_callable=AsyncMock)
     async def test_030_valid_from_cookies(self, redis_mock):
-        token_config.storage = 'cookies'
+        token_config.TOKEN_STORAGE = 'cookies'
         customer_data = CustomerUserFactory().to_dict()
         customer_data['role'] = 'customer'
         redis_mock.return_value = json.dumps(customer_data)
         mock_request = mock.create_autospec(Request)
         mock_request.cookies.get.return_value = '123'
         auth_service = UserRedisAuth()
         user = await auth_service(mock_request)
         customer_data.pop('role')
         self.assertEqual(customer_data, user.to_dict())
+
+    @mock.patch('redis.asyncio.Redis.get', new_callable=AsyncMock)
+    async def test_040_valid_from_cookies(self, redis_mock):
+        token_config.TOKEN_STORAGE = 'headers'
+        developer_data = DeveloperUserFactory().to_dict()
+        developer_data['company'] = {}
+        developer_data['role'] = 'developer'
+        redis_mock.return_value = json.dumps(developer_data)
+        mock_request = mock.create_autospec(Request)
+        mock_request.headers.get.return_value = '123'
+        auth_service = UserRedisAuth()
+        user = await auth_service(mock_request)
+        developer_data.pop('role')
+        self.assertEqual(developer_data, user.to_dict())
```

### Comparing `gspot_fastapi_auth-0.0.3/.gitignore` & `gspot_fastapi_auth-0.0.3b0/.gitignore`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/LICENSE` & `gspot_fastapi_auth-0.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.3/pyproject.toml` & `gspot_fastapi_auth-0.0.3b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_fastapi_auth"
-version = "0.0.3"
+version = "0.0.3b"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "GSpot authentication package for FastApi"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

