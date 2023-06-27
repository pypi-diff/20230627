# Comparing `tmp/django-test-plus-2.2.1.tar.gz` & `tmp/django-test-plus-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-test-plus-2.2.1.tar", last modified: Wed Oct 12 16:00:07 2022, max compression
+gzip compressed data, was "django-test-plus-2.2.2.tar", last modified: Tue Jun 27 18:51:55 2023, max compression
```

## Comparing `django-test-plus-2.2.1.tar` & `django-test-plus-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2022-10-12 16:00:07.112119 django-test-plus-2.2.1/
--rw-r--r--   0 frank      (501) staff       (20)      708 2018-01-09 21:48:49.000000 django-test-plus-2.2.1/AUTHORS.txt
--rw-r--r--   0 frank      (501) staff       (20)     4402 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/CHANGELOG.md
--rw-r--r--   0 frank      (501) staff       (20)     1559 2015-05-23 16:37:20.000000 django-test-plus-2.2.1/LICENSE
--rw-r--r--   0 frank      (501) staff       (20)      153 2018-06-15 19:56:34.000000 django-test-plus-2.2.1/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)    20249 2022-10-12 16:00:07.112194 django-test-plus-2.2.1/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)    18914 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2022-10-12 16:00:07.111339 django-test-plus-2.2.1/django_test_plus.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)    20249 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      508 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)       41 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2019-05-12 15:19:09.000000 django-test-plus-2.2.1/django_test_plus.egg-info/not-zip-safe
--rw-r--r--   0 frank      (501) staff       (20)       86 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       10 2022-10-12 16:00:07.000000 django-test-plus-2.2.1/django_test_plus.egg-info/top_level.txt
--rw-r--r--   0 frank      (501) staff       (20)      235 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/pytest.ini
--rw-r--r--   0 frank      (501) staff       (20)     1287 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/requirements.txt
--rw-r--r--   0 frank      (501) staff       (20)     1628 2022-10-12 16:00:07.112563 django-test-plus-2.2.1/setup.cfg
--rw-r--r--   0 frank      (501) staff       (20)       38 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/setup.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2022-10-12 16:00:07.111995 django-test-plus-2.2.1/test_plus/
--rw-r--r--   0 frank      (501) staff       (20)       90 2022-01-27 21:26:25.000000 django-test-plus-2.2.1/test_plus/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      890 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/test_plus/compat.py
--rw-r--r--   0 frank      (501) staff       (20)      632 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/test_plus/plugin.py
--rw-r--r--   0 frank      (501) staff       (20)      556 2017-10-24 13:55:52.000000 django-test-plus-2.2.1/test_plus/runner.py
--rw-r--r--   0 frank      (501) staff       (20)     9316 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/test_plus/status_codes.py
--rw-r--r--   0 frank      (501) staff       (20)    18884 2022-10-12 15:57:24.000000 django-test-plus-2.2.1/test_plus/test.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.744766 django-test-plus-2.2.2/
+-rw-r--r--   0 frank      (501) staff       (20)      752 2023-05-17 13:29:22.000000 django-test-plus-2.2.2/AUTHORS.txt
+-rw-r--r--   0 frank      (501) staff       (20)     4649 2023-06-27 18:42:38.000000 django-test-plus-2.2.2/CHANGELOG.md
+-rw-r--r--   0 frank      (501) staff       (20)     1559 2015-05-23 16:37:20.000000 django-test-plus-2.2.2/LICENSE
+-rw-r--r--   0 frank      (501) staff       (20)      136 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)    20239 2023-06-27 18:51:55.744843 django-test-plus-2.2.2/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)    19007 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.743691 django-test-plus-2.2.2/django_test_plus.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)    20239 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      491 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)       40 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2019-05-12 15:19:09.000000 django-test-plus-2.2.2/django_test_plus.egg-info/not-zip-safe
+-rw-r--r--   0 frank      (501) staff       (20)       86 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       10 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/top_level.txt
+-rw-r--r--   0 frank      (501) staff       (20)      229 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/pytest.ini
+-rw-r--r--   0 frank      (501) staff       (20)     1584 2023-06-27 18:51:55.745262 django-test-plus-2.2.2/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)       38 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.744653 django-test-plus-2.2.2/test_plus/
+-rw-r--r--   0 frank      (501) staff       (20)       90 2022-01-27 21:26:25.000000 django-test-plus-2.2.2/test_plus/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      890 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/compat.py
+-rw-r--r--   0 frank      (501) staff       (20)      632 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/plugin.py
+-rw-r--r--   0 frank      (501) staff       (20)      556 2017-10-24 13:55:52.000000 django-test-plus-2.2.2/test_plus/runner.py
+-rw-r--r--   0 frank      (501) staff       (20)     9316 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/status_codes.py
+-rw-r--r--   0 frank      (501) staff       (20)    19587 2023-06-27 18:36:37.000000 django-test-plus-2.2.2/test_plus/test.py
```

### Comparing `django-test-plus-2.2.1/AUTHORS.txt` & `django-test-plus-2.2.2/AUTHORS.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 Guinslym <agmond@gmx.com.br>
 David Arcos - http://davidarcos.net
 Malik Junaid - https://www.facebook.com/malik.junaid27
 Jeff Triplett <jeff.triplett@gmail.com>
 Fábio C. Barrionuevo da Lu
 Lacey Williams Henschel <laceynwilliams@gmail.com>
 Anton - https://github.com/singleton11
+Natalia Bidart - https://github.com/nessita
```

### Comparing `django-test-plus-2.2.1/CHANGELOG.md` & `django-test-plus-2.2.2/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changes
 
+## Version 2.2.2 - June 27, 2023
+
+  - Fix issue with User creation helper when User model doesn't have a username field
+  - Improve assertNumQueriesLessThan
+  - Add assertInContext
+
+## version 2.2.1 - October 12, 2022
+
+  - Add Django 4.2 support
+
 ## version 2.2.0 - May 19th, 2021
 
   - Add support for Django 3.2.
 
 ## version 2.1.1 - May 19th, 2021
 
   - Add official support for Python 3.9.
```

### Comparing `django-test-plus-2.2.1/LICENSE` & `django-test-plus-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.1/PKG-INFO` & `django-test-plus-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: django-test-plus
-Version: 2.2.1
+Version: 2.2.2
 Summary: "django-test-plus provides useful additions to Django's default TestCase"
 Home-page: https://github.com/revsys/django-test-plus/
 Author: Frank Wiles
 Author-email: frank@revsys.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 # django-test-plus
@@ -47,17 +43,17 @@
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
 ## Support
 
-Supports: Python 3.6, 3.7, 3.8, 3.9, and 3.10.
+Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
-Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1. and 3.2.
+Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
 
 Full documentation is available at http://django-test-plus.readthedocs.org
 
 ## Installation
 
@@ -124,29 +120,29 @@
 def test_url_reverse(tp_api):
     response = tp_api.client.post("myapi", format="json")
     assert response.status_code == 200
 ```
 
 ## Methods
 
-### reverse(url_name, *args, **kwargs)
+### `reverse(url_name, *args, **kwargs)`
 
 When testing views you often find yourself needing to reverse the URL's name. With django-test-plus there is no need for the `from django.core.urlresolvers import reverse` boilerplate. Instead, use:
 
 ```python
 def test_something(self):
     url = self.reverse('my-url-name')
     slug_url = self.reverse('name-takes-a-slug', slug='my-slug')
     pk_url = self.reverse('name-takes-a-pk', pk=12)
 ```
 
 As you can see our reverse also passes along any args or kwargs you need
 to pass in.
 
-## get(url_name, follow=True, *args, **kwargs)
+## `get(url_name, follow=True, *args, **kwargs)`
 
 Another thing you do often is HTTP get urls. Our `get()` method
 assumes you are passing in a named URL with any args or kwargs necessary
 to reverse the url_name.
 If needed, place kwargs for `TestClient.get()` in an 'extra' dictionary.:
 
 ```python
@@ -193,61 +189,61 @@
 ```python
 def test_testplus_get_query(self):
     self.get('search', data={'query': 'testing'})
 ```
 
 Would GET `/search/?query=testing`.
 
-## post(url_name, data, follow=True, *args, **kwargs)
+## `post(url_name, data, follow=True, *args, **kwargs)`
 
 Our `post()` method takes a named URL, an optional dictionary of data you wish
 to post and any args or kwargs necessary to reverse the url_name.
 If needed, place kwargs for `TestClient.post()` in an 'extra' dictionary.:
 
 ```python
 def test_post_named_url(self):
     response = self.post('my-url-name', data={'coolness-factor': 11.0},
                          extra={'HTTP_X_REQUESTED_WITH': 'XMLHttpRequest'})
 ```
 
 *NOTE* Along with the frequently used get and post, we support all of the HTTP verbs such as put, patch, head, trace, options, and delete in the same fashion.
 
-## get_context(key)
+## `get_context(key)`
 
 Often you need to get things out of the template context:
 
 ```python
 def test_context_data(self):
     self.get('my-view-with-some-context')
     slug = self.get_context('slug')
 ```
 
-## assertInContext(key)
+## `assertInContext(key)`
 
 You can ensure a specific key exists in the last response's context by
 using:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertInContext('some-key')
 ```
 
-## assertContext(key, value)
+## `assertContext(key, value)`
 
 We can get context values and ensure they exist, but we can also test
 equality while we're at it. This asserts that key == value:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertContext('some-key', 'expected value')
 ```
 
-## assert_http_###_<status_name>(response, msg=None) - status code checking
+## `assert_http_###_<status_name>(response, msg=None)` - status code checking
 
 Another test you often need to do is check that a response has a certain
 HTTP status code. With Django's default TestCase you would write:
 
 ```python
 from django.core.urlresolvers import reverse
 
@@ -299,15 +295,15 @@
 - `response_404()` 
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
 All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
 
-## get_check_200(url_name, *args, **kwargs)
+## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
     response = self.get_check_200('my-url-name')
 ```
@@ -351,15 +347,15 @@
 You can also pass in user permissions by passing in a string of
 '`<app_name>.<perm name>`' or '`<app_name>.*`'.  For example:
 
 ```python
 user2 = self.make_user(perms=['myapp.create_widget', 'otherapp.*'])
 ```
 
-## print_form_errors(response_or_form=None)
+## `print_form_errors(response_or_form=None)`
 
 When debugging a failing test for a view with a form, this method helps you
 quickly look at any form errors.
 
 Example usage:
 
 ```python
@@ -377,26 +373,26 @@
 
     form = MyForm(data={})
     self.print_form_errors(form)
 ```
 
 ## Authentication Helpers
 
-### assertLoginRequired(url_name, *args, **kwargs)
+### `assertLoginRequired(url_name, *args, **kwargs)`
 
 This method helps you test that a given named URL requires authorization:
 
 ```python
 def test_auth(self):
     self.assertLoginRequired('my-restricted-url')
     self.assertLoginRequired('my-restricted-object', pk=12)
     self.assertLoginRequired('my-restricted-object', slug='something')
 ```
 
-### login context
+### `login()` context
 
 Along with ensuring a view requires login and creating users, the next
 thing you end up doing is logging in as various users to test your
 restriction logic:
 
 ```python
 def test_restrictions(self):
@@ -435,31 +431,31 @@
 
     with self.login(user1):
         response = self.get('my-protected-view')
 ```
 
 ## Ensuring low query counts
 
-### assertNumQueriesLessThan(number) - context
+### `assertNumQueriesLessThan(number)` - context
 
 Django provides
-[assertNumQueries](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
+[`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
 queries. However, if this number varies due to the nature of your data, with 
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
         self.get('some-view-with-6-queries')
 ```
 
-### assertGoodView(url_name, *args, **kwargs)
+### `assertGoodView(url_name, *args, **kwargs)`
 
 This method does a few things for you. It:
 
 - Retrieves the name URL
 - Ensures the view does not generate more than 50 queries
 - Ensures the response has status code 200
 - Returns the response
@@ -528,15 +524,15 @@
 from test_plus.test import CBVTestCase
 
 class MyViewTests(CBVTestCase):
 ```
 
 ## Methods
 
-### get_instance(cls, initkwargs=None, request=None, *args, **kwargs)
+### `get_instance(cls, initkwargs=None, request=None, *args, **kwargs)`
 
 This core method simplifies the instantiation of your class, giving you
 a way to invoke class methods directly.
 
 Returns an instance of `cls`, initialized with `initkwargs`.
 Sets `request`, `args`, and `kwargs` attributes on the class instance.
 `args` and `kwargs` are the same values you would pass to `reverse()`.
@@ -557,15 +553,15 @@
 
     def test_context_data(self):
         my_view = self.get_instance(MyClass, {'object': some_object})
         context = my_view.get_context_data()
         self.assertEqual(context['answer'], 42)
 ```
 
-### get(cls, initkwargs=None, *args, **kwargs)
+### `get(cls, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.get()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 All test_plus.test.TestCase methods are valid, so the following works:
 
 ```python
@@ -576,15 +572,15 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.get()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing, you should use TestCase instead of CBVTestCase.
 
-### post(cls, data=None, initkwargs=None, *args, **kwargs)
+### `post(cls, data=None, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.post()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 Example:
 
 ```python
@@ -596,46 +592,50 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing you should use TestCase instead of CBVTestCase.
 
-### get_check_200(cls, initkwargs=None, *args, **kwargs)
+### `get_check_200(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.get_check_200()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
-### assertGoodView(cls, initkwargs=None, *args, **kwargs)
+### `assertGoodView(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.assertGoodView()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 ## Development
 
-To work on django-test-plus itself, clone this repository and run the following commands:
+To work on django-test-plus itself, clone this repository and run the following command:
 
 ```shell
-$ pip install -r requirements.txt
 $ pip install -e .
+$ pip install -e .[test]
+```
+
+## To run all tests:
+
+```shell
+$ nox
 ```
 
 **NOTE**: You will also need to ensure that the `test_project` directory, located
 at the root of this repo, is in your virtualenv's path.
 
 ## Keep in touch!
 
 If you have a question about this project, please open a GitHub issue. If you love us and want to keep track of our goings-on, here's where you can find us online:
 
 <a href="https://revsys.com?utm_medium=github&utm_source=django-test-plus"><img src="https://pbs.twimg.com/profile_images/915928618840285185/sUdRGIn1_400x400.jpg" height="50" /></a>
 <a href="https://twitter.com/revsys"><img src="https://cdn1.iconfinder.com/data/icons/new_twitter_icon/256/bird_twitter_new_simple.png" height="43" /></a>
 <a href="https://www.facebook.com/revsysllc/"><img src="https://cdn3.iconfinder.com/data/icons/picons-social/57/06-facebook-512.png" height="50" /></a>
 <a href="https://github.com/revsys/"><img src="https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png" height="53" /></a>
 <a href="https://gitlab.com/revsys"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/GitLab_Logo.svg/2000px-GitLab_Logo.svg.png" height="44" /></a>
-
-
```

### Comparing `django-test-plus-2.2.1/README.md` & `django-test-plus-2.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
 ## Support
 
-Supports: Python 3.6, 3.7, 3.8, 3.9, and 3.10.
+Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
-Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1. and 3.2.
+Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
 
 Full documentation is available at http://django-test-plus.readthedocs.org
 
 ## Installation
 
@@ -88,29 +88,29 @@
 def test_url_reverse(tp_api):
     response = tp_api.client.post("myapi", format="json")
     assert response.status_code == 200
 ```
 
 ## Methods
 
-### reverse(url_name, *args, **kwargs)
+### `reverse(url_name, *args, **kwargs)`
 
 When testing views you often find yourself needing to reverse the URL's name. With django-test-plus there is no need for the `from django.core.urlresolvers import reverse` boilerplate. Instead, use:
 
 ```python
 def test_something(self):
     url = self.reverse('my-url-name')
     slug_url = self.reverse('name-takes-a-slug', slug='my-slug')
     pk_url = self.reverse('name-takes-a-pk', pk=12)
 ```
 
 As you can see our reverse also passes along any args or kwargs you need
 to pass in.
 
-## get(url_name, follow=True, *args, **kwargs)
+## `get(url_name, follow=True, *args, **kwargs)`
 
 Another thing you do often is HTTP get urls. Our `get()` method
 assumes you are passing in a named URL with any args or kwargs necessary
 to reverse the url_name.
 If needed, place kwargs for `TestClient.get()` in an 'extra' dictionary.:
 
 ```python
@@ -157,61 +157,61 @@
 ```python
 def test_testplus_get_query(self):
     self.get('search', data={'query': 'testing'})
 ```
 
 Would GET `/search/?query=testing`.
 
-## post(url_name, data, follow=True, *args, **kwargs)
+## `post(url_name, data, follow=True, *args, **kwargs)`
 
 Our `post()` method takes a named URL, an optional dictionary of data you wish
 to post and any args or kwargs necessary to reverse the url_name.
 If needed, place kwargs for `TestClient.post()` in an 'extra' dictionary.:
 
 ```python
 def test_post_named_url(self):
     response = self.post('my-url-name', data={'coolness-factor': 11.0},
                          extra={'HTTP_X_REQUESTED_WITH': 'XMLHttpRequest'})
 ```
 
 *NOTE* Along with the frequently used get and post, we support all of the HTTP verbs such as put, patch, head, trace, options, and delete in the same fashion.
 
-## get_context(key)
+## `get_context(key)`
 
 Often you need to get things out of the template context:
 
 ```python
 def test_context_data(self):
     self.get('my-view-with-some-context')
     slug = self.get_context('slug')
 ```
 
-## assertInContext(key)
+## `assertInContext(key)`
 
 You can ensure a specific key exists in the last response's context by
 using:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertInContext('some-key')
 ```
 
-## assertContext(key, value)
+## `assertContext(key, value)`
 
 We can get context values and ensure they exist, but we can also test
 equality while we're at it. This asserts that key == value:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertContext('some-key', 'expected value')
 ```
 
-## assert_http_###_<status_name>(response, msg=None) - status code checking
+## `assert_http_###_<status_name>(response, msg=None)` - status code checking
 
 Another test you often need to do is check that a response has a certain
 HTTP status code. With Django's default TestCase you would write:
 
 ```python
 from django.core.urlresolvers import reverse
 
@@ -263,15 +263,15 @@
 - `response_404()` 
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
 All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
 
-## get_check_200(url_name, *args, **kwargs)
+## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
     response = self.get_check_200('my-url-name')
 ```
@@ -315,15 +315,15 @@
 You can also pass in user permissions by passing in a string of
 '`<app_name>.<perm name>`' or '`<app_name>.*`'.  For example:
 
 ```python
 user2 = self.make_user(perms=['myapp.create_widget', 'otherapp.*'])
 ```
 
-## print_form_errors(response_or_form=None)
+## `print_form_errors(response_or_form=None)`
 
 When debugging a failing test for a view with a form, this method helps you
 quickly look at any form errors.
 
 Example usage:
 
 ```python
@@ -341,26 +341,26 @@
 
     form = MyForm(data={})
     self.print_form_errors(form)
 ```
 
 ## Authentication Helpers
 
-### assertLoginRequired(url_name, *args, **kwargs)
+### `assertLoginRequired(url_name, *args, **kwargs)`
 
 This method helps you test that a given named URL requires authorization:
 
 ```python
 def test_auth(self):
     self.assertLoginRequired('my-restricted-url')
     self.assertLoginRequired('my-restricted-object', pk=12)
     self.assertLoginRequired('my-restricted-object', slug='something')
 ```
 
-### login context
+### `login()` context
 
 Along with ensuring a view requires login and creating users, the next
 thing you end up doing is logging in as various users to test your
 restriction logic:
 
 ```python
 def test_restrictions(self):
@@ -399,31 +399,31 @@
 
     with self.login(user1):
         response = self.get('my-protected-view')
 ```
 
 ## Ensuring low query counts
 
-### assertNumQueriesLessThan(number) - context
+### `assertNumQueriesLessThan(number)` - context
 
 Django provides
-[assertNumQueries](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
+[`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
 queries. However, if this number varies due to the nature of your data, with 
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
         self.get('some-view-with-6-queries')
 ```
 
-### assertGoodView(url_name, *args, **kwargs)
+### `assertGoodView(url_name, *args, **kwargs)`
 
 This method does a few things for you. It:
 
 - Retrieves the name URL
 - Ensures the view does not generate more than 50 queries
 - Ensures the response has status code 200
 - Returns the response
@@ -492,15 +492,15 @@
 from test_plus.test import CBVTestCase
 
 class MyViewTests(CBVTestCase):
 ```
 
 ## Methods
 
-### get_instance(cls, initkwargs=None, request=None, *args, **kwargs)
+### `get_instance(cls, initkwargs=None, request=None, *args, **kwargs)`
 
 This core method simplifies the instantiation of your class, giving you
 a way to invoke class methods directly.
 
 Returns an instance of `cls`, initialized with `initkwargs`.
 Sets `request`, `args`, and `kwargs` attributes on the class instance.
 `args` and `kwargs` are the same values you would pass to `reverse()`.
@@ -521,15 +521,15 @@
 
     def test_context_data(self):
         my_view = self.get_instance(MyClass, {'object': some_object})
         context = my_view.get_context_data()
         self.assertEqual(context['answer'], 42)
 ```
 
-### get(cls, initkwargs=None, *args, **kwargs)
+### `get(cls, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.get()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 All test_plus.test.TestCase methods are valid, so the following works:
 
 ```python
@@ -540,15 +540,15 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.get()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing, you should use TestCase instead of CBVTestCase.
 
-### post(cls, data=None, initkwargs=None, *args, **kwargs)
+### `post(cls, data=None, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.post()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 Example:
 
 ```python
@@ -560,37 +560,43 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing you should use TestCase instead of CBVTestCase.
 
-### get_check_200(cls, initkwargs=None, *args, **kwargs)
+### `get_check_200(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.get_check_200()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
-### assertGoodView(cls, initkwargs=None, *args, **kwargs)
+### `assertGoodView(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.assertGoodView()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 ## Development
 
-To work on django-test-plus itself, clone this repository and run the following commands:
+To work on django-test-plus itself, clone this repository and run the following command:
 
 ```shell
-$ pip install -r requirements.txt
 $ pip install -e .
+$ pip install -e .[test]
+```
+
+## To run all tests:
+
+```shell
+$ nox
 ```
 
 **NOTE**: You will also need to ensure that the `test_project` directory, located
 at the root of this repo, is in your virtualenv's path.
 
 ## Keep in touch!
```

### Comparing `django-test-plus-2.2.1/django_test_plus.egg-info/PKG-INFO` & `django-test-plus-2.2.2/django_test_plus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: django-test-plus
-Version: 2.2.1
+Version: 2.2.2
 Summary: "django-test-plus provides useful additions to Django's default TestCase"
 Home-page: https://github.com/revsys/django-test-plus/
 Author: Frank Wiles
 Author-email: frank@revsys.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 # django-test-plus
@@ -47,17 +43,17 @@
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
 ## Support
 
-Supports: Python 3.6, 3.7, 3.8, 3.9, and 3.10.
+Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
-Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1. and 3.2.
+Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
 
 Full documentation is available at http://django-test-plus.readthedocs.org
 
 ## Installation
 
@@ -124,29 +120,29 @@
 def test_url_reverse(tp_api):
     response = tp_api.client.post("myapi", format="json")
     assert response.status_code == 200
 ```
 
 ## Methods
 
-### reverse(url_name, *args, **kwargs)
+### `reverse(url_name, *args, **kwargs)`
 
 When testing views you often find yourself needing to reverse the URL's name. With django-test-plus there is no need for the `from django.core.urlresolvers import reverse` boilerplate. Instead, use:
 
 ```python
 def test_something(self):
     url = self.reverse('my-url-name')
     slug_url = self.reverse('name-takes-a-slug', slug='my-slug')
     pk_url = self.reverse('name-takes-a-pk', pk=12)
 ```
 
 As you can see our reverse also passes along any args or kwargs you need
 to pass in.
 
-## get(url_name, follow=True, *args, **kwargs)
+## `get(url_name, follow=True, *args, **kwargs)`
 
 Another thing you do often is HTTP get urls. Our `get()` method
 assumes you are passing in a named URL with any args or kwargs necessary
 to reverse the url_name.
 If needed, place kwargs for `TestClient.get()` in an 'extra' dictionary.:
 
 ```python
@@ -193,61 +189,61 @@
 ```python
 def test_testplus_get_query(self):
     self.get('search', data={'query': 'testing'})
 ```
 
 Would GET `/search/?query=testing`.
 
-## post(url_name, data, follow=True, *args, **kwargs)
+## `post(url_name, data, follow=True, *args, **kwargs)`
 
 Our `post()` method takes a named URL, an optional dictionary of data you wish
 to post and any args or kwargs necessary to reverse the url_name.
 If needed, place kwargs for `TestClient.post()` in an 'extra' dictionary.:
 
 ```python
 def test_post_named_url(self):
     response = self.post('my-url-name', data={'coolness-factor': 11.0},
                          extra={'HTTP_X_REQUESTED_WITH': 'XMLHttpRequest'})
 ```
 
 *NOTE* Along with the frequently used get and post, we support all of the HTTP verbs such as put, patch, head, trace, options, and delete in the same fashion.
 
-## get_context(key)
+## `get_context(key)`
 
 Often you need to get things out of the template context:
 
 ```python
 def test_context_data(self):
     self.get('my-view-with-some-context')
     slug = self.get_context('slug')
 ```
 
-## assertInContext(key)
+## `assertInContext(key)`
 
 You can ensure a specific key exists in the last response's context by
 using:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertInContext('some-key')
 ```
 
-## assertContext(key, value)
+## `assertContext(key, value)`
 
 We can get context values and ensure they exist, but we can also test
 equality while we're at it. This asserts that key == value:
 
 ```python
 def test_in_context(self):
     self.get('my-view-with-some-context')
     self.assertContext('some-key', 'expected value')
 ```
 
-## assert_http_###_<status_name>(response, msg=None) - status code checking
+## `assert_http_###_<status_name>(response, msg=None)` - status code checking
 
 Another test you often need to do is check that a response has a certain
 HTTP status code. With Django's default TestCase you would write:
 
 ```python
 from django.core.urlresolvers import reverse
 
@@ -299,15 +295,15 @@
 - `response_404()` 
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
 All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
 
-## get_check_200(url_name, *args, **kwargs)
+## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
     response = self.get_check_200('my-url-name')
 ```
@@ -351,15 +347,15 @@
 You can also pass in user permissions by passing in a string of
 '`<app_name>.<perm name>`' or '`<app_name>.*`'.  For example:
 
 ```python
 user2 = self.make_user(perms=['myapp.create_widget', 'otherapp.*'])
 ```
 
-## print_form_errors(response_or_form=None)
+## `print_form_errors(response_or_form=None)`
 
 When debugging a failing test for a view with a form, this method helps you
 quickly look at any form errors.
 
 Example usage:
 
 ```python
@@ -377,26 +373,26 @@
 
     form = MyForm(data={})
     self.print_form_errors(form)
 ```
 
 ## Authentication Helpers
 
-### assertLoginRequired(url_name, *args, **kwargs)
+### `assertLoginRequired(url_name, *args, **kwargs)`
 
 This method helps you test that a given named URL requires authorization:
 
 ```python
 def test_auth(self):
     self.assertLoginRequired('my-restricted-url')
     self.assertLoginRequired('my-restricted-object', pk=12)
     self.assertLoginRequired('my-restricted-object', slug='something')
 ```
 
-### login context
+### `login()` context
 
 Along with ensuring a view requires login and creating users, the next
 thing you end up doing is logging in as various users to test your
 restriction logic:
 
 ```python
 def test_restrictions(self):
@@ -435,31 +431,31 @@
 
     with self.login(user1):
         response = self.get('my-protected-view')
 ```
 
 ## Ensuring low query counts
 
-### assertNumQueriesLessThan(number) - context
+### `assertNumQueriesLessThan(number)` - context
 
 Django provides
-[assertNumQueries](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
+[`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
 queries. However, if this number varies due to the nature of your data, with 
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
         self.get('some-view-with-6-queries')
 ```
 
-### assertGoodView(url_name, *args, **kwargs)
+### `assertGoodView(url_name, *args, **kwargs)`
 
 This method does a few things for you. It:
 
 - Retrieves the name URL
 - Ensures the view does not generate more than 50 queries
 - Ensures the response has status code 200
 - Returns the response
@@ -528,15 +524,15 @@
 from test_plus.test import CBVTestCase
 
 class MyViewTests(CBVTestCase):
 ```
 
 ## Methods
 
-### get_instance(cls, initkwargs=None, request=None, *args, **kwargs)
+### `get_instance(cls, initkwargs=None, request=None, *args, **kwargs)`
 
 This core method simplifies the instantiation of your class, giving you
 a way to invoke class methods directly.
 
 Returns an instance of `cls`, initialized with `initkwargs`.
 Sets `request`, `args`, and `kwargs` attributes on the class instance.
 `args` and `kwargs` are the same values you would pass to `reverse()`.
@@ -557,15 +553,15 @@
 
     def test_context_data(self):
         my_view = self.get_instance(MyClass, {'object': some_object})
         context = my_view.get_context_data()
         self.assertEqual(context['answer'], 42)
 ```
 
-### get(cls, initkwargs=None, *args, **kwargs)
+### `get(cls, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.get()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 All test_plus.test.TestCase methods are valid, so the following works:
 
 ```python
@@ -576,15 +572,15 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.get()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing, you should use TestCase instead of CBVTestCase.
 
-### post(cls, data=None, initkwargs=None, *args, **kwargs)
+### `post(cls, data=None, initkwargs=None, *args, **kwargs)`
 
 Invokes `cls.post()` and returns the response, rendering template if possible.
 Builds on the `CBVTestCase.get_instance()` foundation.
 
 Example:
 
 ```python
@@ -596,46 +592,50 @@
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 **NOTE:** This method bypasses Django's middleware, and therefore context
 variables created by middleware are not available. If this affects your
 template/context testing you should use TestCase instead of CBVTestCase.
 
-### get_check_200(cls, initkwargs=None, *args, **kwargs)
+### `get_check_200(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.get_check_200()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
-### assertGoodView(cls, initkwargs=None, *args, **kwargs)
+### `assertGoodView(cls, initkwargs=None, *args, **kwargs)`
 
 Works just like `TestCase.assertGoodView()`.
 Caller must provide a view class instead of a URL name or path parameter.
 
 All test_plus TestCase side-effects are honored and all test_plus
 TestCase assertion methods work with `CBVTestCase.post()`.
 
 ## Development
 
-To work on django-test-plus itself, clone this repository and run the following commands:
+To work on django-test-plus itself, clone this repository and run the following command:
 
 ```shell
-$ pip install -r requirements.txt
 $ pip install -e .
+$ pip install -e .[test]
+```
+
+## To run all tests:
+
+```shell
+$ nox
 ```
 
 **NOTE**: You will also need to ensure that the `test_project` directory, located
 at the root of this repo, is in your virtualenv's path.
 
 ## Keep in touch!
 
 If you have a question about this project, please open a GitHub issue. If you love us and want to keep track of our goings-on, here's where you can find us online:
 
 <a href="https://revsys.com?utm_medium=github&utm_source=django-test-plus"><img src="https://pbs.twimg.com/profile_images/915928618840285185/sUdRGIn1_400x400.jpg" height="50" /></a>
 <a href="https://twitter.com/revsys"><img src="https://cdn1.iconfinder.com/data/icons/new_twitter_icon/256/bird_twitter_new_simple.png" height="43" /></a>
 <a href="https://www.facebook.com/revsysllc/"><img src="https://cdn3.iconfinder.com/data/icons/picons-social/57/06-facebook-512.png" height="50" /></a>
 <a href="https://github.com/revsys/"><img src="https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png" height="53" /></a>
 <a href="https://gitlab.com/revsys"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/GitLab_Logo.svg/2000px-GitLab_Logo.svg.png" height="44" /></a>
-
-
```

### Comparing `django-test-plus-2.2.1/setup.cfg` & `django-test-plus-2.2.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 [bumpversion]
-current_version = 2.2.1
+current_version = 2.2.2
 commit = True
 tag = True
 
 [metadata]
 name = django-test-plus
-version = 2.2.1
+version = 2.2.2
 description = "django-test-plus provides useful additions to Django's default TestCase"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Frank Wiles
 author_email = frank@revsys.com
 url = https://github.com/revsys/django-test-plus/
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 2.0
-	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Framework :: Pytest
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 packages = find:
 zip_safe = False
 setup_requires = 
 	pytest-runner
```

### Comparing `django-test-plus-2.2.1/test_plus/compat.py` & `django-test-plus-2.2.2/test_plus/compat.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.1/test_plus/plugin.py` & `django-test-plus-2.2.2/test_plus/plugin.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.1/test_plus/runner.py` & `django-test-plus-2.2.2/test_plus/runner.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.1/test_plus/status_codes.py` & `django-test-plus-2.2.2/test_plus/status_codes.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.1/test_plus/test.py` & `django-test-plus-2.2.2/test_plus/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import django
 
 from distutils.version import LooseVersion
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ImproperlyConfigured
@@ -23,29 +25,30 @@
 
 # Build a real context
 
 CAPTURE = True
 
 
 class _AssertNumQueriesLessThanContext(CaptureQueriesContext):
-    def __init__(self, test_case, num, connection):
+    def __init__(self, test_case, num, connection, verbose=False):
         self.test_case = test_case
         self.num = num
+        self.verbose = verbose
         super(_AssertNumQueriesLessThanContext, self).__init__(connection)
 
     def __exit__(self, exc_type, exc_value, traceback):
         super(_AssertNumQueriesLessThanContext, self).__exit__(exc_type, exc_value, traceback)
         if exc_type is not None:
             return
         executed = len(self)
-        self.test_case.assertTrue(
-            executed < self.num, "%d queries executed, expected less than %d" % (
-                executed, self.num
-            )
-        )
+        msg = "%d queries executed, expected less than %d" % (executed, self.num)
+        if self.verbose:
+            queries = "\n\n".join(q["sql"] for q in self.captured_queries)
+            msg += ". Executed queries were:\n\n%s" % queries
+        self.test_case.assertLess(executed, self.num, msg)
 
 
 class login(object):
     """
     A useful login context for Django tests.  If the first argument is
     a User, we will login with that user's username.  If no password is
     given we will use 'password'.
@@ -251,30 +254,25 @@
 
     @classmethod
     def make_user(cls, username='testuser', password='password', perms=None):
         """
         Build a user with <username> and password of 'password' for testing
         purposes.
         """
-        User = get_user_model()
-
         if cls.user_factory:
-            USERNAME_FIELD = getattr(
-                cls.user_factory._meta.model, 'USERNAME_FIELD', 'username')
-            test_user = cls.user_factory(**{
-                USERNAME_FIELD: username,
-            })
-            test_user.set_password(password)
-            test_user.save()
+            User = cls.user_factory._meta.model
+            user_factory = cls.user_factory
         else:
-            test_user = User.objects.create_user(
-                username,
-                '{0}@example.com'.format(username),
-                password,
-            )
+            User = get_user_model()
+            user_factory = User.objects.create_user
+
+        USERNAME_FIELD = getattr(User, 'USERNAME_FIELD', 'username')
+        test_user = user_factory(**{USERNAME_FIELD: username})
+        test_user.set_password(password)
+        test_user.save()
 
         if perms:
             from django.contrib.auth.models import Permission
             _filter = Q()
             for perm in perms:
                 if '.' not in perm:
                     raise ImproperlyConfigured(
@@ -291,44 +289,39 @@
             test_user.user_permissions.add(*list(Permission.objects.filter(_filter)))
 
         return test_user
 
     def assertNumQueriesLessThan(self, num, *args, **kwargs):
         func = kwargs.pop('func', None)
         using = kwargs.pop("using", DEFAULT_DB_ALIAS)
+        verbose = kwargs.pop("verbose", False)
         conn = connections[using]
 
-        context = _AssertNumQueriesLessThanContext(self, num, conn)
+        context = _AssertNumQueriesLessThanContext(self, num, conn, verbose=verbose)
         if func is None:
             return context
 
         with context:
             func(*args, **kwargs)
 
-    def assertGoodView(self, url_name, *args, **kwargs):
+    def assertGoodView(self, url_name, *args, verbose=False, **kwargs):
         """
         Quick-n-dirty testing of a given url name.
         Ensures URL returns a 200 status and that generates less than 50
         database queries.
         """
         query_count = kwargs.pop('test_query_count', 50)
 
-        with self.assertNumQueriesLessThan(query_count):
+        with self.assertNumQueriesLessThan(query_count, verbose=verbose):
             response = self.get(url_name, *args, **kwargs)
 
         self.response_200(response)
 
         return response
 
-    def assertInContext(self, key):
-        if self.last_response is not None:
-            self.assertTrue(key in self.last_response.context)
-        else:
-            raise NoPreviousResponse("There isn't a previous response to query")
-
     def assertResponseContains(self, text, response=None, html=True, **kwargs):
         """ Convenience wrapper for assertContains """
         response = self._which_response(response)
         self.assertContains(response, text, html=html, **kwargs)
 
     def assertResponseNotContains(self, text, response=None, html=True, **kwargs):
         """ Convenience wrapper for assertNotContains """
@@ -349,24 +342,24 @@
         """
         response = self._which_response(response)
         compare = {h: response.get(h) for h in headers}
         self.assertEqual(compare, headers)
 
     def get_context(self, key):
         if self.last_response is not None:
-            self.assertTrue(key in self.last_response.context)
+            self.assertIn(key, self.last_response.context)
             return self.last_response.context[key]
         else:
             raise NoPreviousResponse("There isn't a previous response to query")
 
+    def assertInContext(self, key):
+        return self.get_context(key)
+
     def assertContext(self, key, value):
-        if self.last_response is not None:
-            self.assertEqual(self.last_response.context[key], value)
-        else:
-            raise NoPreviousResponse("There isn't a previous response to query")
+        self.assertEqual(self.get_context(key), value)
 
 
 class TestCase(DjangoTestCase, BaseTestCase):
     """
     Django TestCase with helpful additional features
     """
     user_factory = None
@@ -377,14 +370,39 @@
 
 
 class APITestCase(TestCase):
     def __init__(self, *args, **kwargs):
         self.client_class = get_api_client()
         super(APITestCase, self).__init__(*args, **kwargs)
 
+    # APITest requests now default to JSON
+    def request(self, method, url_name, *args, **kwargs):
+        data = kwargs.pop("data", {})
+        extra = kwargs.pop("extra", {})
+        kwargs["data"] = json.dumps(data) if data is not None else None
+
+        if extra and "format" in extra:
+            format = extra.pop("format")
+        else:
+            format = None
+
+        if extra and "content_type" in extra:
+            content_type = extra.pop("content_type")
+        else:
+            content_type = None
+
+        # DRF wants either `format` or `content_type` but not both
+        if format and content_type is None:
+            extra.update({"format": "json"})
+        else:
+            extra.update({"content_type": "application/json"})
+
+        kwargs["extra"] = extra
+        return super().request(method, url_name, *args, **kwargs)
+
 
 # Note this class inherits from TestCase defined above.
 class CBVTestCase(TestCase):
     """
     Directly calls class-based generic view methods,
     bypassing the Django test Client.
```

