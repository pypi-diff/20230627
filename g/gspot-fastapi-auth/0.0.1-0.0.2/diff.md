# Comparing `tmp/gspot_fastapi_auth-0.0.1.tar.gz` & `tmp/gspot_fastapi_auth-0.0.2.tar.gz`

## Comparing `gspot_fastapi_auth-0.0.1.tar` & `gspot_fastapi_auth-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/requirements.in
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/requirements.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/example/main.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/example/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/__init__.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/auth.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/base.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/models.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/permissions.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/providers.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/services.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/settings.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/test_factory.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/tests/tests.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/LICENSE
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/requirements.in
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/example/main.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/example/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/__init__.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/auth.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/base.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/models.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/permissions.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/providers.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/services.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/settings.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/test_factory.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/tests/tests.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/PKG-INFO
```

### Comparing `gspot_fastapi_auth-0.0.1/requirements.txt` & `gspot_fastapi_auth-0.0.2/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,124 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile
 #
+add-trailing-comma==2.5.1
+    # via -r requirements.in
 anyio==3.7.0
     # via
     #   httpcore
     #   starlette
+black==23.3.0
+    # via -r requirements.in
 bleach==6.0.0
     # via readme-renderer
 certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
-    # via uvicorn
+    # via
+    #   black
+    #   uvicorn
 cryptography==41.0.1
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
 factory-boy==3.2.1
     # via
     #   -r requirements.in
-    #   fastapi-gspot-auth
+    #   gspot-fastapi-auth
 faker==18.11.1
     # via
     #   -r requirements.in
     #   factory-boy
-    #   fastapi-gspot-auth
+    #   gspot-fastapi-auth
 fastapi==0.98.0
     # via
     #   -r requirements.in
-    #   fastapi-gspot-auth
-fastapi-gspot-auth==0.0.1
+    #   gspot-fastapi-auth
+flake8==6.0.0
+    # via -r requirements.in
+gspot-fastapi-auth==0.0.1
     # via -r requirements.in
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
 httpcore==0.17.2
     # via httpx
 httpx==0.24.1
     # via
     #   -r requirements.in
-    #   fastapi-gspot-auth
+    #   gspot-fastapi-auth
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
 importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
+isort==5.12.0
+    # via -r requirements.in
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 keyring==24.2.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
+mccabe==0.7.0
+    # via flake8
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
+mypy-extensions==1.0.0
+    # via black
+packaging==23.1
+    # via black
+pathspec==0.11.1
+    # via black
 pkginfo==1.9.6
     # via twine
+platformdirs==3.8.0
+    # via black
+pycodestyle==2.10.0
+    # via flake8
 pycparser==2.21
     # via cffi
 pydantic==1.10.9
     # via fastapi
+pyflakes==3.0.1
+    # via flake8
 pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 python-dateutil==2.8.2
     # via faker
 readme-renderer==40.0
     # via twine
 redis==4.6.0
     # via
     #   -r requirements.in
-    #   fastapi-gspot-auth
+    #   gspot-fastapi-auth
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
@@ -110,14 +134,16 @@
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 starlette==0.27.0
     # via fastapi
+tokenize-rt==5.1.0
+    # via add-trailing-comma
 twine==4.0.2
     # via -r requirements.in
 typing-extensions==4.6.3
     # via pydantic
 urllib3==2.0.3
     # via
     #   requests
```

### Comparing `gspot_fastapi_auth-0.0.1/example/tests.py` & `gspot_fastapi_auth-0.0.2/example/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 from unittest import IsolatedAsyncioTestCase, mock
 from unittest.mock import AsyncMock
 
 from fastapi.testclient import TestClient
+from gspot_fastapi_auth import token_config, BaseRedis
+from gspot_fastapi_auth.providers import RedisClient
+from gspot_fastapi_auth.test_factory import AdminUserFactory, CustomerUserFactory, DeveloperUserFactory
 
-from src.gspot_fastapi_auth import BaseRedis
-from src.gspot_fastapi_auth.providers import RedisClient
-from src.gspot_fastapi_auth.settings import token_config
 from main import app
-from src.gspot_fastapi_auth.test_factory import AdminUserFactory, CustomerUserFactory, DeveloperUserFactory
 
 
 class TestAuth(IsolatedAsyncioTestCase):
     url = '/'
     customer_url = '/customer/'
 
     async def asyncSetUp(self) -> None:
```

### Comparing `gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/auth.py` & `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 from typing import Type
 
-from fastapi import Request, HTTPException
+from fastapi import HTTPException, Request
 from fastapi.security import HTTPBearer, OAuth2PasswordBearer
 from starlette.status import HTTP_401_UNAUTHORIZED
 
 from .models import BaseUser, UserFactory
 from .providers import RedisClient
 from .services import TokenService
 from .settings import token_config
 
-oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token")
+oauth2_scheme = OAuth2PasswordBearer(tokenUrl='token')
 
 
 class UserRedisAuth(HTTPBearer):
-
     def __init__(self, *args, **kwargs):
         super(UserRedisAuth, self).__init__(*args, **kwargs)
         self._redis_client = RedisClient(
             token_config.host,
             token_config.port,
             token_config.db,
-            token_config.password
+            token_config.password,
         )
         self.token_service = TokenService(self._redis_client.session)
 
     @staticmethod
     def _get_token_from_headers(request: Request) -> str:
         token = request.headers.get('HTTP_AUTHORIZATION')
         if not token:
-            raise HTTPException(
-                status_code=HTTP_401_UNAUTHORIZED, detail="Not authenticated"
-            )
+            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         return token
 
     @staticmethod
     def _get_token_from_cookies(request: Request) -> str:
         token = request.cookies.get('Authentication')
         if not token:
-            raise HTTPException(
-                status_code=HTTP_401_UNAUTHORIZED, detail="Not authenticated"
-            )
+            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         return token
 
     async def __call__(self, request: Request) -> Type[BaseUser]:
         if token_config.storage == 'headers':
             token = self._get_token_from_headers(request)
         else:
             token = self._get_token_from_cookies(request)
         data = await self.token_service.get_token_data(token)
         if not data:
-            raise HTTPException(
-                status_code=HTTP_401_UNAUTHORIZED, detail="Not authenticated"
-            )
+            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail='Not authenticated')
         user_class = UserFactory().get_user(data.pop('role'))
         return user_class(**data)
 
 
-__all__ = ['UserRedisAuth', ]
+__all__ = [
+    'UserRedisAuth',
+]
```

### Comparing `gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/models.py` & `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass, field, asdict
+from dataclasses import asdict, dataclass, field
 from datetime import datetime
 from typing import List
 from uuid import UUID
 
 
 @dataclass(frozen=True)
 class BaseUser:
@@ -53,18 +53,14 @@
 
 @dataclass(frozen=True)
 class CustomerUser(BaseUser):
     birthday: datetime
 
 
 class UserFactory:
-    users = {
-        'administrator': AdminUser,
-        'developer': DeveloperUser,
-        'customer': CustomerUser
-    }
+    users = {'administrator': AdminUser, 'developer': DeveloperUser, 'customer': CustomerUser}
 
     def get_user(self, role: str):
         return self.users.get(role)
 
 
-__all__ = ['CustomerUser', 'AdminUser', 'DeveloperUser', 'UserFactory', 'Company']
+__all__ = ['CustomerUser', 'AdminUser', 'DeveloperUser', 'UserFactory', 'Company', 'BaseUser']
```

### Comparing `gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/permissions.py` & `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/permissions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-from fastapi import HTTPException
-
-from fastapi import Depends
+from fastapi import Depends, HTTPException
 from starlette.status import HTTP_403_FORBIDDEN
 
 from .auth import UserRedisAuth
-from .models import CustomerUser, AdminUser, DeveloperUser
+from .models import AdminUser, CustomerUser, DeveloperUser
 
 
 def is_customer(user=Depends(UserRedisAuth())):
     if isinstance(user, CustomerUser):
         return user
     else:
-        raise HTTPException(
-            status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
-        )
+        raise HTTPException(status_code=HTTP_403_FORBIDDEN, detail='Not authenticated')
 
 
 def is_admin(user=Depends(UserRedisAuth())):
     if isinstance(user, AdminUser):
         return user
     else:
-        raise HTTPException(
-            status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
-        )
+        raise HTTPException(status_code=HTTP_403_FORBIDDEN, detail='Not authenticated')
 
 
 def is_developer(user=Depends(UserRedisAuth())):
     if isinstance(user, DeveloperUser):
         return user
     else:
-        raise HTTPException(
-            status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
-        )
+        raise HTTPException(status_code=HTTP_403_FORBIDDEN, detail='Not authenticated')
 
 
 __all__ = ['is_developer', 'is_customer', 'is_admin']
```

### Comparing `gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/providers.py` & `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from contextlib import asynccontextmanager
 
 import redis.asyncio as redis
 
 
 class RedisClient:
-
     def __init__(self, host: str, port: int, db: int, password: str):
         self.host = host
         self.port = port
         self.db = db
         self.password = password
 
     @asynccontextmanager
     async def session(self):
         try:
             session = redis.Redis(
                 host=self.host,
                 port=self.port,
                 db=self.db,
-                password=self.password
+                password=self.password,
             )
             yield session
         finally:
             await session.close()
```

### Comparing `gspot_fastapi_auth-0.0.1/src/gspot_fastapi_auth/test_factory.py` & `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/test_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from datetime import datetime
 
 import factory
-
-from src.gspot_fastapi_auth import AdminUser, CustomerUser, DeveloperUser, Company
-from src.gspot_fastapi_auth.models import BaseUser
-
 from faker import Faker
 
+from .models import AdminUser, BaseUser, Company, CustomerUser, DeveloperUser
+
 fake = Faker(['ru_Ru'])
 
 
 class BaseUserFactory(factory.Factory):
     class Meta:
         model = BaseUser
 
@@ -54,7 +52,10 @@
         is_confirmed=True,
         created_at=str(datetime.now()),
         is_active=True,
         is_banned=True,
     ).to_dict()
     groups = []
     user_permissions = []
+
+
+__all__ = ['AdminUserFactory', 'CustomerUserFactory', 'DeveloperUserFactory']
```

### Comparing `gspot_fastapi_auth-0.0.1/tests/tests.py` & `gspot_fastapi_auth-0.0.2/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.1/.gitignore` & `gspot_fastapi_auth-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.1/LICENSE` & `gspot_fastapi_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.1/pyproject.toml` & `gspot_fastapi_auth-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_fastapi_auth"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "GSpot authentication package for FastApi"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -24,7 +24,22 @@
     'faker>=18.11.1',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gravity48/gspot_fastapi_auth"
 "Bug Tracker" = "https://github.com/gravity48/gspot_fastapi_auth/issues"
 
+[tool.black]
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+)/
+'''
```

### Comparing `gspot_fastapi_auth-0.0.1/PKG-INFO` & `gspot_fastapi_auth-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_fastapi_auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: GSpot authentication package for FastApi
 Project-URL: Homepage, https://github.com/gravity48/gspot_fastapi_auth
 Project-URL: Bug Tracker, https://github.com/gravity48/gspot_fastapi_auth/issues
 Author-email: gravity48 <gravity4849@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,10 +13,16 @@
 Requires-Dist: factory-boy>=3.2.1
 Requires-Dist: faker>=18.11.1
 Requires-Dist: fastapi>=0.98.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: redis>=4.6.0
 Description-Content-Type: text/markdown
 
-## GSpot authentication package
+# GSpot authentication package
 
 This package allows you to authorize users through a shared redis
+
+## Install package
+```shell
+pip install gspot-fastapi-auth
+```
+
```

