# Comparing `tmp/cndi-2.1.7a2.tar.gz` & `tmp/cndi-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cndi-2.1.7a2.tar", last modified: Tue Oct 11 18:29:46 2022, max compression
+gzip compressed data, was "cndi-2.1.8.tar", last modified: Tue Jun 27 21:39:31 2023, max compression
```

## Comparing `cndi-2.1.7a2.tar` & `cndi-2.1.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-10-11 18:29:34.000000 cndi-2.1.7a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-11 18:29:46.722614 cndi-2.1.7a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-10-11 18:29:34.000000 cndi-2.1.7a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.718614 cndi-2.1.7a2/cndi/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/annotations/
--rw-r--r--   0 runner    (1001) docker     (121)     9255 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/annotations/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/annotations/events.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/binders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/binders/message/
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/message/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/message/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/binders/message/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/events/
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/exception/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/http/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/initializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/cndi/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-10-11 18:29:34.000000 cndi-2.1.7a2/cndi/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.718614 cndi-2.1.7a2/cndi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-11 18:29:46.000000 cndi-2.1.7a2/cndi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-10-11 18:29:46.000000 cndi-2.1.7a2/cndi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 18:29:46.000000 cndi-2.1.7a2/cndi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-11 18:29:46.000000 cndi-2.1.7a2/cndi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-11 18:29:46.722614 cndi-2.1.7a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-11 18:29:34.000000 cndi-2.1.7a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/tests/cndi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/tests/cndi/annotations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/annotations/test_app_initializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/annotations/test_components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/tests/cndi/binders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/binders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 18:29:46.722614 cndi-2.1.7a2/tests/cndi/binders/message/
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/cndi/binders/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-10-11 18:29:34.000000 cndi-2.1.7a2/tests/test_load_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 21:39:21.000000 cndi-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-27 21:39:31.241176 cndi-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-27 21:39:21.000000 cndi-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/annotations/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/annotations/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/binders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/binders/message/
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/message/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/message/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/binders/message/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 21:39:21.000000 cndi-2.1.8/cndi/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.237176 cndi-2.1.8/cndi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-27 21:39:31.000000 cndi-2.1.8/cndi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-27 21:39:31.000000 cndi-2.1.8/cndi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:39:31.000000 cndi-2.1.8/cndi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 21:39:31.000000 cndi-2.1.8/cndi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:39:31.241176 cndi-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-27 21:39:21.000000 cndi-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/tests/cndi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/tests/cndi/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/annotations/test_app_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/annotations/test_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/tests/cndi/binders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/binders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:39:31.241176 cndi-2.1.8/tests/cndi/binders/message/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/cndi/binders/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 21:39:21.000000 cndi-2.1.8/tests/test_load_envs.py
```

### Comparing `cndi-2.1.7a2/LICENSE` & `cndi-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/PKG-INFO` & `cndi-2.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: cndi
-Version: 2.1.7a2
+Version: 2.1.8
 Author: Mayank Shinde
 Author-email: mayank31313@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Install
 
     pip install -U git+https://github.com/mayank31313/python-dependency-injection.git
-    
+
+# Documentation
+
+Documentation is shifted [here](https://mayank31313.github.io/get-started/site/python-di/)
+
+
 # Example    
 Follow the below code to simplify understanding, or can also refer to [main.py](main.py)
     
-    from cndi.annotations import Bean, Autowired, AppInitilizer
+    from cndi.annotations import Bean, Autowired, AppInitializer
     
     class TestBean:
         def __init__(self, name):
             self.name = name
     
     
     @Bean()
     def getTestBean() -> TestBean:
         return TestBean("Test 123")
     
     testBean = None
     
-    app = AppInitilizer()
+    app = AppInitializer()
     if __name__ == "__main__":
         @Autowired()
         def setTestBean(bean: TestBean):
             global testBean
             testBean = bean
     
         app.run()
```

### Comparing `cndi-2.1.7a2/cndi/annotations/__init__.py` & `cndi-2.1.8/cndi/annotations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,37 @@
 
 
 def importModuleName(fullname):
     modules = fullname.split('.')
     module = importlib.import_module(modules[-1], package='.'.join(modules[:-1]))
     return module
 
+
 def normaliseModuleAndClassName(name):
-    nameList:list = name.split(".")
+    nameList: list = name.split(".")
     if "__init__" in nameList:
         nameList.remove("__init__")
     return '.'.join(nameList)
 
+
 def getBeanObject(objectType):
     bean = queryBeanStorage(objectType)
     objectInstance = bean['objectInstance']
     # if (objectInstance.__class__.__name__ == "function"):
     #     args[key] = objectInstance()
     # else:
     return copy.deepcopy(objectInstance) if bean['newInstance'] else objectInstance
 
+
 def queryBeanStorage(fullname):
     objectType = normaliseModuleAndClassName(fullname)
     bean = beanStore[objectType]
     return bean
 
+
 class AutowiredClass:
     def __init__(self, required, func, kwargs: dict()):
         self.fullname = '.'.join([func.__qualname__])
         self.className = normaliseModuleAndClassName('.'.join(func.__qualname__.split(".")[:-1]))
         self.func = func
         self.kwargs = kwargs
         self.required = required
@@ -76,66 +80,74 @@
             self.func(beanStore[self.className], **args)
         else:
             logger.info(f"{self.className} {self.fullname}")
             self.func(**args)
 
     def calculateDependencies(self):
         return list(
-            map(lambda dependency: normaliseModuleAndClassName('.'.join([dependency.__module__, dependency.__name__])), self.kwargs.values()))
+            map(lambda dependency: normaliseModuleAndClassName('.'.join([dependency.__module__, dependency.__name__])),
+                self.kwargs.values()))
+
 
 def OverrideBeanType(type: object):
     """
     OverrideBeanType is used to override the current annotated @Component class to be injected as some other object
 
     :param type: Class type to override while performing Dependency Injection
     :return: function wrapper
     """
+
     def inner_function(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         fullname = '.'.join([wrapper.__module__, wrapper.__name__])
 
         overrideStore[fullname] = {
             "func": wrapper,
             "overrideType": type
         }
         return wrapper
+
     return inner_function
 
+
 def queryOverideBeanStore(fullname):
     if fullname in overrideStore:
         return overrideStore[fullname]
     else:
         return None
 
+
 def Component(func: object):
     """
     When decorated with @Component, AppInitializer tries to automatically initialise the class this decorator is added to
     :param func:
     :return:
     """
+
     @wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     moduleName = wrapper.__module__[:-9] if wrapper.__module__.endswith(".__init__") else wrapper.__module__
-    componentFullName = '.'.join([moduleName,wrapper.__qualname__])
-    logger.info(f"Function name " + componentFullName)
+    componentFullName = '.'.join([moduleName, wrapper.__qualname__])
+    logger.info(f"Registering Function name " + componentFullName)
     duplicateComponents = list(filter(lambda component: component.fullname == componentFullName, components))
     if duplicateComponents.__len__() > 0:
         logger.info(f"Duplicate Component found for: {duplicateComponents}")
     else:
         components.append(ComponentClass(**{
             'fullname': componentFullName,
             'func': wrapper,
             'annotations': wrapper.__init__.__annotations__ if "__annotations__" in dir(wrapper.__init__) else {}
         }))
-    return  wrapper
+    return wrapper
+
 
 def validateBean(fullname):
     """
     Validates Beans before performing the dependency injection
     :param fullname: bean class full classpath name
     :return: Boolean type
     """
@@ -153,22 +165,27 @@
         flag &= intersectionProfiles.__len__() >= 1
 
     if condition is not None:
         callback = condition['callback']
         callbackValue = callback(condition['func'])
         flag &= bool(callbackValue)
 
+    if flag is False:
+        logger.info("Validation Failed for Bean " + fullname)
+
     return flag
 
+
 def Bean(newInstance=False):
     """
 
     :param newInstance:
     :return:
     """
+
     def inner_function(func):
         annotations = func.__annotations__
         returnType = annotations['return']
         del annotations['return']
 
         @wraps(func)
         def wrapper(*args, **kwargs):
@@ -190,20 +207,22 @@
 
             return wrapper
         else:
             return None
 
     return inner_function
 
+
 def ConditionalRendering(callback=lambda method: True):
     """
 
     :param callback:
     :return:
     """
+
     def inner_function(func: object):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         fullname = ".".join([wrapper.__module__, wrapper.__qualname__])
         conditionalRender[fullname] = {
@@ -211,26 +230,29 @@
             "callback": callback
         }
 
         return wrapper
 
     return inner_function
 
+
 def queryContitionalRenderingStore(fullname):
     if fullname in conditionalRender:
         return conditionalRender[fullname]
     else:
         return None
 
+
 def Profile(profiles=["default"]):
     """
 
     :param profiles:
     :return:
     """
+
     def inner_function(func: object):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         fullname = ".".join([wrapper.__module__, wrapper.__qualname__])
         profilesStores[fullname] = {
@@ -238,26 +260,29 @@
             "profiles": profiles
         }
 
         return wrapper
 
     return inner_function
 
+
 def queryProfileData(fullname):
     if fullname in profilesStores:
         return profilesStores.get(fullname)
     else:
         return None
 
+
 def Autowired(required=True):
     """
     
     :param required:
     :return:
     """
+
     def inner_function(func: object):
         annotations = func.__annotations__
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
@@ -266,17 +291,19 @@
             'func': wrapper
         }))
 
         return wrapper
 
     return inner_function
 
+
 def getBean(beans, name):
     return list(filter(lambda x: x['name'] == name, beans))[0]
 
+
 def workOrder(beans):
     allBeanNames = list(map(lambda bean: bean['name'], beans))
     beanQueue = list(filter(lambda bean: len(bean['kwargs']) == 0, beans))
     beanIndexes = list(map(lambda bean: bean['index'], beanQueue))
 
     beanDependents = list(filter(lambda bean: bean['index'] not in beanIndexes, beans))
     beanQueueNames = list(map(lambda bean: bean['name'], beanQueue))
@@ -296,9 +323,7 @@
 
         if flag:
             beanQueue.append(dependents)
             beanQueueNames.append(dependents['name'])
 
     assert len(beanQueue) == len(beans), "Somebeans were not initialized properly"
     return list(sorted(beanQueue, key=lambda x: x['index']))
-
-
```

### Comparing `cndi-2.1.7a2/cndi/annotations/events.py` & `cndi-2.1.8/cndi/annotations/events.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/binders/message/__init__.py` & `cndi-2.1.8/cndi/binders/message/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/binders/message/rabbitmq.py` & `cndi-2.1.8/cndi/binders/message/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/binders/message/utils.py` & `cndi-2.1.8/cndi/binders/message/utils.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/env.py` & `cndi-2.1.8/cndi/env.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/events/__init__.py` & `cndi-2.1.8/cndi/events/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/http/__init__.py` & `cndi-2.1.8/cndi/http/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi/initializers.py` & `cndi-2.1.8/cndi/initializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,29 +8,44 @@
 from cndi.annotations import beanStore, workOrder, beans, components, componentStore, autowires, getBeanObject, getBean, \
     validateBean, queryOverideBeanStore
 from cndi.env import loadEnvFromFile, getContextEnvironment
 from cndi.utils import importSubModules
 
 logger = logging.getLogger(__name__)
 
-class AppInitilizer:
+class AppInitializer:
     def __init__(self):
+        """
+        Responsible to initialise Dependency Injection for Application
+        """
         self.componentsPath = list()
         applicationYml = "resources/application.yml"
         if os.path.exists(applicationYml):
             logger.info(f"External Configuration found: {applicationYml}")
             loadEnvFromFile(applicationYml)
 
 
     def componentScan(self, module):
         importModule = importlib.import_module(module)
         self.componentsPath.append(importModule)
 
 
     def run(self):
+        """
+        Performing Dependency Injection, on priority basis
+        Steps Involved in DI
+            1. Load Modules and Sub Modules for Bean/Component scanning
+            2. Create list for the Available Beans and Components
+            3. Resolve Dependency Tree for Beans and Components and Sort in reverse tree dependency
+            4. For component classes run postConstruct method if available
+            5. Read Configuration for binders and initialise binders for given type (i.e rabbitmq, mqtt)
+            6. Perform Dependency Injection by calling setter methods
+            7. Start Binder Configuration
+        :return: None
+        """
         for module in self.componentsPath:
             importSubModules(module)
 
         workOrderBeans = workOrder(beans)
 
         for bean in workOrderBeans:
             logger.info(f"Registering Bean {bean['fullname']}")
```

### Comparing `cndi-2.1.7a2/cndi/resources.py` & `cndi-2.1.8/cndi/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,8 @@
 
         if resourceExist:
             resourcePath = os.path.join(resourceDirPath, resourcePath)
             if os.path.exists(resourcePath):
                 return resourcePath
             raise FileNotFoundError(f"Resource not found at resources/{resourcePath}")
         else:
-            raise FileNotFoundError(f"Resource Path not found resources/{resourcePath}")
-
-
-if __name__ == '__main__':
-    resourceFinder = ResourceFinder()
-    print(resourceFinder.rcnHome)
-    print(resourceFinder.findResource(""))
+            raise FileNotFoundError(f"Resource Path not found resources/{resourcePath}")
```

### Comparing `cndi-2.1.7a2/cndi/utils.py` & `cndi-2.1.8/cndi/utils.py`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/cndi.egg-info/PKG-INFO` & `cndi-2.1.8/cndi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: cndi
-Version: 2.1.7a2
+Version: 2.1.8
 Author: Mayank Shinde
 Author-email: mayank31313@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Install
 
     pip install -U git+https://github.com/mayank31313/python-dependency-injection.git
-    
+
+# Documentation
+
+Documentation is shifted [here](https://mayank31313.github.io/get-started/site/python-di/)
+
+
 # Example    
 Follow the below code to simplify understanding, or can also refer to [main.py](main.py)
     
-    from cndi.annotations import Bean, Autowired, AppInitilizer
+    from cndi.annotations import Bean, Autowired, AppInitializer
     
     class TestBean:
         def __init__(self, name):
             self.name = name
     
     
     @Bean()
     def getTestBean() -> TestBean:
         return TestBean("Test 123")
     
     testBean = None
     
-    app = AppInitilizer()
+    app = AppInitializer()
     if __name__ == "__main__":
         @Autowired()
         def setTestBean(bean: TestBean):
             global testBean
             testBean = bean
     
         app.run()
```

### Comparing `cndi-2.1.7a2/cndi.egg-info/SOURCES.txt` & `cndi-2.1.8/cndi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cndi-2.1.7a2/setup.py` & `cndi-2.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "2.1.7a2"
+VERSION = "2.1.8"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cndi",
     version=VERSION,
```

### Comparing `cndi-2.1.7a2/tests/cndi/annotations/test_app_initializer.py` & `cndi-2.1.8/tests/cndi/annotations/test_app_initializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import unittest
 
 from cndi.annotations import Autowired
-from cndi.initializers import AppInitilizer
+from cndi.initializers import AppInitializer
 from test_module.TestBean import TestBean
 
 
 class AppInitializerTest(unittest.TestCase):
     def testComponentScanAndDI(self):
         @Autowired()
         def setTestBean(bean: TestBean):
             global testBean
             print(bean)
             testBean = bean
 
-        app = AppInitilizer()
+        app = AppInitializer()
         app.componentScan("test_module")
 
         app.run()
         self.assertEqual(testBean.name, "Test 123")
         self.assertIsInstance(testBean, TestBean)
```

### Comparing `cndi-2.1.7a2/tests/cndi/annotations/test_components.py` & `cndi-2.1.8/tests/cndi/annotations/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 from cndi.annotations import Component, Bean, Autowired
 from cndi.env import VARS
-from cndi.initializers import AppInitilizer
+from cndi.initializers import AppInitializer
 from test_module.TestBean import TestBean
 
 
 @Bean()
 def getTestBean() -> TestBean:
     return TestBean("testBean")
 
@@ -33,12 +33,12 @@
 
     def testComponents(self):
         @Autowired()
         def setComponent(secondComponent: SecondTestClass, bean: TestBean):
             self.store['component'] = secondComponent
             self.store['bean'] = bean
 
-        appInitializer = AppInitilizer()
+        appInitializer = AppInitializer()
         appInitializer.run()
 
         self.assertTrue(self.store['component'].firstComponent.triggered)
         self.assertIsNotNone(self.store['component'].testBean)
```

### Comparing `cndi-2.1.7a2/tests/cndi/binders/message/__init__.py` & `cndi-2.1.8/tests/cndi/binders/message/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from cndi.annotations import Component, Autowired
 from cndi.binders.message import DefaultMessageBinder, Output, Input
 from cndi.binders.message.mqtt import MqttProducerBinding
 from cndi.binders.message.utils import MessageChannel
 from cndi.env import VARS, loadEnvFromFile, RCN_ENVS_CONFIG
-from cndi.initializers import AppInitilizer
+from cndi.initializers import AppInitializer
 
 
 @Component
 class SinkMQTTTest:
     outputChannel1Binding: MessageChannel
     @Output("default-channel-output")
     def setOutputForDefaultChannel(self, messageBinder: MqttProducerBinding):
@@ -44,15 +44,15 @@
         defaultMessageBinder = DefaultMessageBinder()
 
     def testWithAppInitializer(self):
         @Autowired()
         def setSink(sink: SinkMQTTTest):
             sink.outputChannel1Binding.send("Hello")
 
-        appInitializer = AppInitilizer()
+        appInitializer = AppInitializer()
         appInitializer.componentScan("cndi.binders")
         appInitializer.run()
 
 #
 # class RabbitMQDefaultMessageBinderTest(unittest.TestCase):
 #     def setUp(self) -> None:
 #         VARS.clear()
@@ -65,10 +65,10 @@
 #
 #     def testWithAppInitializer(self):
 #         @Autowired()
 #         def setSink(sink: SinkRabbitMQTTTest):
 #             print(sink)
 #             sink.outputChannel1Binding.send("Hello")
 #
-#         appInitializer = AppInitilizer()
+#         appInitializer = AppInitializer()
 #         appInitializer.componentScan("cndi.binders")
 #         appInitializer.run()
```

### Comparing `cndi-2.1.7a2/tests/test_load_envs.py` & `cndi-2.1.8/tests/test_load_envs.py`

 * *Files identical despite different names*

