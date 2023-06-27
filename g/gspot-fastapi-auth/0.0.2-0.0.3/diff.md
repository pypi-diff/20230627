# Comparing `tmp/gspot_fastapi_auth-0.0.2.tar.gz` & `tmp/gspot_fastapi_auth-0.0.3.tar.gz`

## Comparing `gspot_fastapi_auth-0.0.2.tar` & `gspot_fastapi_auth-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/requirements.in
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/requirements.txt
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/example/main.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/example/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/__init__.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/auth.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/base.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/models.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/permissions.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/providers.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/services.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/settings.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/test_factory.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/tests/tests.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/requirements.in
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/example/main.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/example/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/__init__.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/auth.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/base.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/models.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/permissions.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/providers.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/services.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/settings.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/test_factory.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/tests/tests.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.3/PKG-INFO
```

### Comparing `gspot_fastapi_auth-0.0.2/.pre-commit-config.yaml` & `gspot_fastapi_auth-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/requirements.txt` & `gspot_fastapi_auth-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/example/tests.py` & `gspot_fastapi_auth-0.0.3/example/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/auth.py` & `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/auth.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/models.py` & `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,44 +23,27 @@
     user_permissions: List[str] = field(default_factory=list)
     developer_groups: List[str] = field(default_factory=list)
     developer_permissions: List[str] = field(default_factory=list)
     groups: List[str] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
-class Company:
-    created_by: str
-    title: str
-    description: str
-    email: str
-    is_confirmed: bool
-    created_at: datetime
-    is_active: bool
-    is_banned: bool
-
-    to_dict = asdict
-
-
-@dataclass(frozen=True)
 class DeveloperUser(BaseUser):
     is_superuser: bool
     company: dict
     groups: List[str] = field(default_factory=list)
     user_permissions: List[str] = field(default_factory=list)
 
-    def __post_init__(self):
-        object.__setattr__(self, 'company', Company(**self.company))
-
 
 @dataclass(frozen=True)
 class CustomerUser(BaseUser):
     birthday: datetime
 
 
 class UserFactory:
     users = {'administrator': AdminUser, 'developer': DeveloperUser, 'customer': CustomerUser}
 
     def get_user(self, role: str):
         return self.users.get(role)
 
 
-__all__ = ['CustomerUser', 'AdminUser', 'DeveloperUser', 'UserFactory', 'Company', 'BaseUser']
+__all__ = ['CustomerUser', 'AdminUser', 'DeveloperUser', 'UserFactory', 'BaseUser']
```

### Comparing `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/permissions.py` & `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/src/gspot_fastapi_auth/test_factory.py` & `gspot_fastapi_auth-0.0.3/src/gspot_fastapi_auth/test_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 import factory
 from faker import Faker
 
-from .models import AdminUser, BaseUser, Company, CustomerUser, DeveloperUser
+from .models import AdminUser, BaseUser, CustomerUser, DeveloperUser
 
 fake = Faker(['ru_Ru'])
 
 
 class BaseUserFactory(factory.Factory):
     class Meta:
         model = BaseUser
@@ -40,22 +40,23 @@
 
 
 class DeveloperUserFactory(BaseUserFactory):
     class Meta:
         model = DeveloperUser
 
     is_superuser = True
-    company = Company(
-        created_by=fake.uuid4(),
-        title=fake.word(),
-        description=fake.text(),
-        email=fake.email(),
-        is_confirmed=True,
-        created_at=str(datetime.now()),
-        is_active=True,
-        is_banned=True,
-    ).to_dict()
+    company = {
+        'created_by': fake.uuid4(),
+        'title': fake.word(),
+        'description': fake.text(),
+        'email': fake.email(),
+        'is_confirmed': True,
+        'created_at': str(datetime.now()),
+        'is_active': True,
+        'is_banned': True
+
+    }
     groups = []
     user_permissions = []
 
 
 __all__ = ['AdminUserFactory', 'CustomerUserFactory', 'DeveloperUserFactory']
```

### Comparing `gspot_fastapi_auth-0.0.2/tests/tests.py` & `gspot_fastapi_auth-0.0.3/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/.gitignore` & `gspot_fastapi_auth-0.0.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+publish.sh
 #Log files#
 logfiles/
 
 #Transcribing Models
 tr_models/
 models/
```

### Comparing `gspot_fastapi_auth-0.0.2/LICENSE` & `gspot_fastapi_auth-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.2/pyproject.toml` & `gspot_fastapi_auth-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_fastapi_auth"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "GSpot authentication package for FastApi"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_fastapi_auth-0.0.2/PKG-INFO` & `gspot_fastapi_auth-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_fastapi_auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: GSpot authentication package for FastApi
 Project-URL: Homepage, https://github.com/gravity48/gspot_fastapi_auth
 Project-URL: Bug Tracker, https://github.com/gravity48/gspot_fastapi_auth/issues
 Author-email: gravity48 <gravity4849@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

