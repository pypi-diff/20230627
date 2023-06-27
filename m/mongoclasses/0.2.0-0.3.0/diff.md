# Comparing `tmp/mongoclasses-0.2.0.tar.gz` & `tmp/mongoclasses-0.3.0.tar.gz`

## Comparing `mongoclasses-0.2.0.tar` & `mongoclasses-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/.python-version
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/src/mongoclasses/__about__.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/src/mongoclasses/__init__.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_fromdict.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_mongoclass.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/tests/test_mongoclass_instances.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 mongoclasses-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/.python-version
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/docs/apiref.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/__about__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/asyncio.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/asyncio.pyi
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/dataclass.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/dataclass.pyi
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/sync.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/sync.pyi
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_dataclass.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_sync.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/README.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/PKG-INFO
```

### Comparing `mongoclasses-0.2.0/tests/test_mongoclass_instances.py` & `mongoclasses-0.3.0/tests/test_asyncio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,104 @@
-from dataclasses import asdict
-from typing import Optional
+from dataclasses import dataclass
+from typing import ClassVar, Optional
 
 from bson import ObjectId
 import pytest
 import pytest_asyncio
-from motor.motor_asyncio import AsyncIOMotorClient
+from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorCollection
 
-from mongoclasses import (
-    delete_one, find, find_one, fromdict, insert_one, mongoclass, update_one
-)
+from mongoclasses import find
+from mongoclasses.asyncio import delete_one, find_one, insert_one, update_one
 
 
-@pytest_asyncio.fixture
-async def database():
-    client = AsyncIOMotorClient()
-    await client.drop_database('test')
-    return client['test']
+@pytest.fixture
+def client():
+    return AsyncIOMotorClient()
+
+
+@pytest_asyncio.fixture(autouse=True)
+async def drop_database(client):
+    await client.drop_database("test")
+
+
+@pytest.fixture
+def test_collection(client):
+    db = client["test"]
+    return db["test_collection"]
 
 
 @pytest.fixture
-def Foo(database):
-    @mongoclass(db=database)
+def Foo(test_collection):
+    @dataclass
     class Foo:
+        collection: ClassVar[AsyncIOMotorCollection] = test_collection
         _id: Optional[ObjectId] = None
         name: str = ""
         description: str = ""
 
     return Foo
 
 
 @pytest.mark.asyncio
-async def test_insert_one_without_id(Foo, database):    
+async def test_insert_one_without_id(Foo):
     f = Foo()
     await insert_one(f)
 
     assert f._id is not None
-    assert await database['foo'].find_one({'_id': f._id}) is not None
+    assert await Foo.collection.find_one({"_id": f._id}) is not None
 
 
 @pytest.mark.asyncio
-async def test_insert_one_with_id(Foo, database):  
-    # test scenario where an _id is generated before insertion.  
+async def test_insert_one_with_id(Foo):
+    # test scenario where an _id is generated before insertion.
     object_id = ObjectId()
     f = Foo(_id=object_id)
     await insert_one(f)
 
     assert f._id == object_id
-    assert await database['foo'].find_one({'_id': f._id}) is not None
+    assert await Foo.collection.find_one({"_id": f._id}) is not None
 
 
 @pytest.mark.asyncio
-async def test_update_one(Foo, database):    
+async def test_update_one(Foo):
     f = Foo()
     await insert_one(f)
 
     f.name = "Fred"
     await update_one(f)
-    
-    doc = await database['foo'].find_one({"_id": f._id})
-    assert doc["name"] == "Fred"
-
 
-@pytest.mark.asyncio
-async def test_update_one_with_fields(Foo, database):    
-    f = Foo()
-    await insert_one(f)
+    doc = await Foo.collection.find_one({"_id": f._id})
+    assert doc["name"] == "Fred"
 
-    f.name = "Fred"
-    f.description = "foobar"
-    await update_one(f, fields=["description"])
-    
-    doc = await database['foo'].find_one({"_id": f._id})
-    assert doc["name"] == ""
-    assert doc["description"] == "foobar"
-    
 
 @pytest.mark.asyncio
-async def test_delete_one(Foo, database):    
+async def test_delete_one(Foo):
     f = Foo()
     await insert_one(f)
     await delete_one(f)
 
-    assert await database['foo'].find_one({"_id": f._id}) is None
+    assert await Foo.collection.find_one({"_id": f._id}) is None
 
 
 @pytest.mark.asyncio
 async def test_find_one(Foo):
     f = Foo()
     await insert_one(f)
 
     # Find document that exists
-    result = await find_one(Foo, {'_id': f._id})
+    result = await find_one(Foo, {"_id": f._id})
     assert result._id == f._id
 
     # find document that does not exist.
-    result = await find_one(Foo, {'_id': "abcdef"})
+    result = await find_one(Foo, {"_id": "abcdef"})
     assert result is None
 
 
 @pytest.mark.asyncio
-async def test_find(Foo, database):
+async def test_find(Foo):
     f1 = Foo(name="Alice")
     await insert_one(f1)
 
     f2 = Foo(name="Bob")
     await insert_one(f2)
 
     f3 = Foo(name="Charlie")
@@ -111,35 +106,28 @@
 
     cursor = find(Foo, {})
     objects = [foo async for foo in cursor]
     assert len(objects) == 3
 
 
 @pytest.mark.asyncio
-async def test_fromdict(Foo):
-    f1 = Foo()
-    f2 = fromdict(Foo, asdict(f1))
-    assert f1 == f2
-
-
-@pytest.mark.asyncio
 async def test_non_mongoclasses_in_mongoclass_functions():
     class Foo:
         ...
 
     with pytest.raises(TypeError):
         f = Foo()
         await insert_one(f)
-    
+
     with pytest.raises(TypeError):
         f = Foo()
         await update_one(f)
-    
+
     with pytest.raises(TypeError):
         f = Foo()
         await delete_one(f)
 
     with pytest.raises(TypeError):
         await find_one(Foo, {})
-    
+
     with pytest.raises(TypeError):
         find(Foo, {})
```

### Comparing `mongoclasses-0.2.0/.gitignore` & `mongoclasses-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.2.0/LICENSE.txt` & `mongoclasses-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.2.0/pyproject.toml` & `mongoclasses-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,75 +3,47 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "mongoclasses"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Ryan Kroon", email = "rykroon.tech@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "motor==3.1.*"
+  "motor>=3.1.1, <4"
 ]
 
 [project.urls]
 Documentation = "https://github.com/rykroon/mongoclasses#readme"
 Issues = "https://github.com/rykroon/mongoclasses/issues"
 Source = "https://github.com/rykroon/mongoclasses"
 
 [tool.hatch.version]
 path = "src/mongoclasses/__about__.py"
 
-[tool.hatch.envs.default]
+[tool.hatch.envs.test]
 dependencies = [
-  "coverage[toml]>=6.5",
   "pytest",
   "pytest-asyncio",
+  "coverage",
 ]
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
-]
+[tool.hatch.envs.test.scripts]
+test = "coverage run -m pytest"
+cov-report = "coverage report -m"
 
-[[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
-
-[tool.coverage.run]
-source_pkgs = ["mongoclasses", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/mongoclasses/__about__.py",
-]
-
-[tool.coverage.paths]
-mongoclasses = ["src/mongoclasses", "*/mongoclasses/src/mongoclasses"]
-tests = ["tests", "*/mongoclasses/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+[[tool.hatch.envs.test.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11"]
```

### Comparing `mongoclasses-0.2.0/PKG-INFO` & `mongoclasses-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: mongoclasses
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/rykroon/mongoclasses#readme
 Project-URL: Issues, https://github.com/rykroon/mongoclasses/issues
 Project-URL: Source, https://github.com/rykroon/mongoclasses
 Author-email: Ryan Kroon <rykroon.tech@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: motor==3.1.*
+Requires-Python: >=3.8
+Requires-Dist: motor<4,>=3.1.1
 Description-Content-Type: text/markdown
 
 # mongoclasses
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mongoclasses.svg)](https://pypi.org/project/mongoclasses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mongoclasses.svg)](https://pypi.org/project/mongoclasses)
```

