# Comparing `tmp/zammad_py-2.0.1.tar.gz` & `tmp/zammad_py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zammad_py-2.0.1.tar", max compression
+gzip compressed data, was "zammad_py-3.0.0.tar", max compression
```

## Comparing `zammad_py-2.0.1.tar` & `zammad_py-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-14 16:41:21.097899 zammad_py-2.0.1/LICENSE
--rw-r--r--   0        0        0     3307 2023-02-14 16:41:21.101899 zammad_py-2.0.1/README.rst
--rw-r--r--   0        0        0     1052 2023-02-16 08:29:01.849727 zammad_py-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      175 2023-02-14 17:34:12.047068 zammad_py-2.0.1/zammad_py/__init__.py
--rw-r--r--   0        0        0    13682 2023-02-14 17:34:12.050058 zammad_py-2.0.1/zammad_py/api.py
--rw-r--r--   0        0        0       43 2023-02-14 16:41:21.152898 zammad_py-2.0.1/zammad_py/exceptions.py
--rw-r--r--   0        0        0     4080 1970-01-01 00:00:00.000000 zammad_py-2.0.1/setup.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 zammad_py-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2017-10-24 05:33:44.000000 zammad_py-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3519 2023-04-13 06:49:54.269244 zammad_py-3.0.0/README.rst
+-rw-r--r--   0        0        0     1052 2023-06-27 09:19:17.154269 zammad_py-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-27 09:19:28.194430 zammad_py-3.0.0/zammad_py/__init__.py
+-rw-r--r--   0        0        0    14727 2023-06-27 09:14:42.705455 zammad_py-3.0.0/zammad_py/api.py
+-rw-r--r--   0        0        0       43 2022-08-04 07:37:22.948465 zammad_py-3.0.0/zammad_py/exceptions.py
+-rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 zammad_py-3.0.0/PKG-INFO
```

### Comparing `zammad_py-2.0.1/LICENSE` & `zammad_py-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zammad_py-2.0.1/README.rst` & `zammad_py-3.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 .. code-block:: python
 
     from zammad_py import ZammadAPI
 
     # Initialize the client with the URL, username, and password
+    # Note the Host URL should be in this format: 'https://zammad.example.org/api/v1/'
     client = ZammadAPI(url='<HOST>', username='<USERNAME>', password='<PASSWORD>')
 
     # Example: Access all users
     this_page = client.user.all()
     for user in this_page:
         print(user)
 
@@ -59,42 +60,44 @@
 
 
 
 General Methods
 ---------------
 Most resources support these methods:
 
-.all(): Returns a paginated response with the current page number and a list of elements.
+`.all()`: Returns a paginated response with the current page number and a list of elements.
 
-.next_page(): Returns the next page of the current pagination object.
+`.next_page()`: Returns the next page of the current pagination object.
 
-.prev_page(): Returns the previous page of the current pagination object.
+`.prev_page()`: Returns the previous page of the current pagination object.
 
-.search(params): Returns a paginated response based on the search parameters.
+`.search(params)`: Returns a paginated response based on the search parameters.
 
-.find(id): Returns a single object with the specified ID.
+`.find(id)`: Returns a single object with the specified ID.
 
-.create(params): Creates a new object with the specified parameters.
+`.create(params)`: Creates a new object with the specified parameters.
 
-.update(params): Updates an existing object with the specified parameters.
+`.update(params)`: Updates an existing object with the specified parameters.
 
-.destroy(id): Deletes an object with the specified ID.
+`.destroy(id)`: Deletes an object with the specified ID.
 
 Additional Resource Methods
 ---------------------------
 User resource also has the .me() method to get information about the current user.
 
 Ticket resource also has the .articles() method to get the articles associated with a ticket.
 
 Link resource has methods to list, add, and delete links between objects.
 
 TicketArticleAttachment resource has the .download() method to download a ticket attachment.
 
 Object resource has the .execute_migrations() method to run migrations on an object.
 
+You can set the `on_behalf_of` attribute of the ZammadAPI instance to do actions on behalf of another user.
+
 Contributing
 ------------
 The Zammad API Client (zammad_py) welcomes contributions.
 
 You can contribute by reporting bugs, fixing bugs, implementing new features, writing documentation, and submitting feedback.
 
 To get started, see the contributing section in the docs!
```

### Comparing `zammad_py-2.0.1/pyproject.toml` & `zammad_py-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zammad_py"
-version = "2.0.1"
+version = "3.0.0"
 readme  = "README.rst"
 description = "Python API client for zammad"
 authors = ["Joe Paul <joeirimpan@gmail.com>"]
 license = "MIT"
 classifiers = [
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
@@ -23,15 +23,15 @@
 python = ">=3.8.1,<4.0"
 requests = "^2.25.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 vcrpy = "^4.1.1"
 flake8 = "6.0.0"
-black = "23.1.0"
+black = "23.3.0"
 isort = "5.12.0"
 
 [tool.mypy]
 files = "zammad_py"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `zammad_py-2.0.1/zammad_py/api.py` & `zammad_py-3.0.0/zammad_py/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         username: Optional[str] = None,
         password: Optional[str] = None,
         http_token: Optional[str] = None,
         oauth2_token: Optional[str] = None,
         on_behalf_of: Optional[str] = None,
         additional_headers: Optional[List[Tuple[str, str]]] = None,
     ) -> None:
-        self.url = url
+        self.url = url if url.endswith("/") else f"{url}/"
         self._username = username
         self._password = password
         self._http_token = http_token
         self._oauth2_token = oauth2_token
         self._on_behalf_of = on_behalf_of
         self._additional_headers = additional_headers
         self._check_config()
@@ -38,15 +38,15 @@
         if self._http_token:
             self.session.headers["Authorization"] = "Token token=%s" % self._http_token
         elif oauth2_token:
             self.session.headers["Authorization"] = "Bearer %s" % self._oauth2_token
         elif self._username and self._password:  # noqa: SIM106
             self.session.auth = (self._username, self._password)
         else:
-            raise ValueError("invalid auth")
+            raise ValueError("Invalid Authentication information in config")
 
         if self._on_behalf_of:
             self.session.headers["X-On-Behalf-Of"] = self._on_behalf_of
 
         if self._additional_headers:
             for additional_header in self._additional_headers:
                 self.session.headers[additional_header[0]] = additional_header[1]
@@ -95,14 +95,19 @@
 
     @property
     def organization(self) -> "Organization":
         """Return a `Organization` instance"""
         return Organization(connection=self)
 
     @property
+    def role(self) -> "Role":
+        """Return a `Role` instance"""
+        return Role(connection=self)
+
+    @property
     def ticket(self) -> "Ticket":
         """Return a `Ticket` instance"""
         return Ticket(connection=self)
 
     @property
     def link(self):
         """Return a `Link` instance"""
@@ -137,20 +142,26 @@
     def user(self) -> "User":
         """Return a `User` instance"""
         return User(connection=self)
 
 
 class Pagination:
     def __init__(
-        self, items, resource: "Resource", filters=None, page: int = 1
+        self,
+        items,
+        resource: "Resource",
+        function_name: str,
+        params=None,
+        page: int = 1,
     ) -> None:
         self._items = items
         self._page = page
         self._resource = resource
-        self._filters = filters
+        self._params = params
+        self._function_name = function_name
 
     def __iter__(self):
         yield from self._items
 
     def __len__(self) -> int:
         return len(self._items)
 
@@ -158,19 +169,23 @@
         return self._items[index]
 
     def __setitem__(self, index: int, value) -> None:
         self._items[index] = value
 
     def next_page(self) -> "Pagination":
         self._page += 1
-        return self._resource.all(page=self._page, filters=self._filters)
+        return getattr(self._resource, self._function_name)(
+            page=self._page, **self._params
+        )
 
     def prev_page(self) -> "Pagination":
         self._page -= 1
-        return self._resource.all(page=self._page, filters=self._filters)
+        return getattr(self._resource, self._function_name)(
+            page=self._page, **self._params
+        )
 
 
 class Resource(ABC):
     def __init__(self, connection: ZammadAPI, per_page: int = 10) -> None:
         self._connection = connection
         self._per_page = per_page
 
@@ -196,15 +211,15 @@
         """Raise HTTPError before converting response to json
 
         :param response: Request response object
         """
         try:
             response.raise_for_status()
         except HTTPError:
-            raise
+            raise HTTPError(response.text)
 
         try:
             json_value = response.json()
         except ValueError:
             return response.content
         else:
             return json_value
@@ -215,23 +230,41 @@
         :param page: Page number
         :param filters: Filter arguments like page, per_page
         """
         params = filters or {}
         params.update({"page": page, "per_page": self._per_page, "expand": "true"})
         response = self._connection.session.get(self.url, params=params)
         data = self._raise_or_return_json(response)
-        return Pagination(items=data, resource=self, filters=filters, page=page)
+        return Pagination(
+            items=data,
+            resource=self,
+            function_name="all",
+            params={"filters": params},
+            page=page,
+        )
 
-    def search(self, params):
-        """Search using the given parameters
+    def search(self, search_string: str, page: int = 1, filters=None) -> Pagination:
+        """Returns the list of resources
 
-        :param params: Search parameters
+        :param search_string: option to filter for
+        :param page: Page number
+        :param filters: Filter arguments like page, per_page
         """
+        params = filters or {}
+        params.update({"query": search_string})
+        params.update({"page": page, "per_page": self._per_page, "expand": "true"})
         response = self._connection.session.get(self.url + "/search", params=params)
-        return self._raise_or_return_json(response)
+        data = self._raise_or_return_json(response)
+        return Pagination(
+            items=data,
+            resource=self,
+            function_name="search",
+            params={"search_string": search_string, "filters": params},
+            page=page,
+        )
 
     def find(self, id):
         """Return the resource associated with the id
 
         :param id: Resource id
         """
         response = self._connection.session.get(self.url + "/%s" % id)
@@ -263,14 +296,18 @@
         return self._raise_or_return_json(response)
 
 
 class Group(Resource):
     path_attribute = "groups"
 
 
+class Role(Resource):
+    path_attribute = "roles"
+
+
 class Organization(Resource):
     path_attribute = "organizations"
 
 
 class Ticket(Resource):
     path_attribute = "tickets"
 
@@ -307,58 +344,58 @@
         link_object_source_number,
         link_type="normal",
         link_object_target="Ticket",
         link_object_source="Ticket",
     ):
         """Create the link
 
-        :params link_type: Link type (for now*: 'normal')
+        :params link_type: Link type ('normal', 'parent', 'child')
         :params link_object_target: (for now*: 'Ticket')
-        :params link_object_target_value: The Ticket Number (Not the ID!)
+        :params link_object_target_value: Ticket ID
         :params link_object_source: (for now*: 'Ticket')
-        :params link_object_source_number: The Ticket Number (Not the ID!)
+        :params link_object_source_number: Ticket Number (Not the ID!)
 
         *Currently, only Tickets can be linked together.
         """
         params = {
             "link_type": link_type,
             "link_object_target": link_object_target,
             "link_object_target_value": link_object_target_value,
             "link_object_source": link_object_source,
             "link_object_source_number": link_object_source_number,
         }
 
-        response = self._connection.session.post(self.url + "add/", json=params)
+        response = self._connection.session.post(self.url + "/add", json=params)
         return self._raise_or_return_json(response)
 
     def remove(
         self,
         link_object_target_value,
         link_object_source_number,
         link_type="normal",
         link_object_target="Ticket",
         link_object_source="Ticket",
     ):
         """Remove the Link
 
-        :params link_type: Link type (for now: 'normal')
+        :params link_type: Link type ('normal', 'parent', 'child')
         :params link_object_target: (for now: 'Ticket')
-        :params link_object_target_value: The Ticket Number (Not the ID!)
+        :params link_object_target_value: Ticket ID
         :params link_object_source: (for now: 'Ticket')
-        :params link_object_source_number: The Ticket Number (Not the ID!)
+        :params link_object_source_number: Ticket ID
         """
         params = {
             "link_type": link_type,
             "link_object_target": link_object_target,
             "link_object_target_value": link_object_target_value,
             "link_object_source": link_object_source,
             "link_object_source_number": link_object_source_number,
         }
 
-        response = self._connection.session.post(self.url + "add/", json=params)
+        response = self._connection.session.delete(self.url + "/remove", json=params)
         return self._raise_or_return_json(response)
 
     def get(self, id):
         """Returns all the links associated with the ticket id
 
         :param id: Ticket id
         """
```

### Comparing `zammad_py-2.0.1/PKG-INFO` & `zammad_py-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: zammad-py
-Version: 2.0.1
+Version: 3.0.0
 Summary: Python API client for zammad
 Home-page: https://github.com/joeirimpan/zammad_py
 License: MIT
 Author: Joe Paul
 Author-email: joeirimpan@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Documentation, https://zammad-py.readthedocs.io/
 Project-URL: Repository, https://github.com/joeirimpan/zammad_py.git
 Description-Content-Type: text/x-rst
 
 =================
 Zammad API Client
@@ -55,14 +52,15 @@
 
 
 .. code-block:: python
 
     from zammad_py import ZammadAPI
 
     # Initialize the client with the URL, username, and password
+    # Note the Host URL should be in this format: 'https://zammad.example.org/api/v1/'
     client = ZammadAPI(url='<HOST>', username='<USERNAME>', password='<PASSWORD>')
 
     # Example: Access all users
     this_page = client.user.all()
     for user in this_page:
         print(user)
 
@@ -85,42 +83,44 @@
 
 
 
 General Methods
 ---------------
 Most resources support these methods:
 
-.all(): Returns a paginated response with the current page number and a list of elements.
+`.all()`: Returns a paginated response with the current page number and a list of elements.
 
-.next_page(): Returns the next page of the current pagination object.
+`.next_page()`: Returns the next page of the current pagination object.
 
-.prev_page(): Returns the previous page of the current pagination object.
+`.prev_page()`: Returns the previous page of the current pagination object.
 
-.search(params): Returns a paginated response based on the search parameters.
+`.search(params)`: Returns a paginated response based on the search parameters.
 
-.find(id): Returns a single object with the specified ID.
+`.find(id)`: Returns a single object with the specified ID.
 
-.create(params): Creates a new object with the specified parameters.
+`.create(params)`: Creates a new object with the specified parameters.
 
-.update(params): Updates an existing object with the specified parameters.
+`.update(params)`: Updates an existing object with the specified parameters.
 
-.destroy(id): Deletes an object with the specified ID.
+`.destroy(id)`: Deletes an object with the specified ID.
 
 Additional Resource Methods
 ---------------------------
 User resource also has the .me() method to get information about the current user.
 
 Ticket resource also has the .articles() method to get the articles associated with a ticket.
 
 Link resource has methods to list, add, and delete links between objects.
 
 TicketArticleAttachment resource has the .download() method to download a ticket attachment.
 
 Object resource has the .execute_migrations() method to run migrations on an object.
 
+You can set the `on_behalf_of` attribute of the ZammadAPI instance to do actions on behalf of another user.
+
 Contributing
 ------------
 The Zammad API Client (zammad_py) welcomes contributions.
 
 You can contribute by reporting bugs, fixing bugs, implementing new features, writing documentation, and submitting feedback.
 
 To get started, see the contributing section in the docs!
```

