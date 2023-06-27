# Comparing `tmp/python-sapcommissions-1.0.0.tar.gz` & `tmp/python-sapcommissions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-1.0.0.tar", last modified: Mon Jun 26 21:16:31 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.0.1.tar", last modified: Tue Jun 27 05:20:29 2023, max compression
```

## Comparing `python-sapcommissions-1.0.0.tar` & `python-sapcommissions-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 21:16:31.051707 python-sapcommissions-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-26 20:02:48.000000 python-sapcommissions-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    17535 2023-06-26 21:16:31.038609 python-sapcommissions-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.922087 python-sapcommissions-1.0.0/docs/
--rw-rw-rw-   0        0        0    16952 2023-06-26 20:34:26.000000 python-sapcommissions-1.0.0/docs/README.md
--rw-rw-rw-   0        0        0     1118 2023-06-26 21:15:12.000000 python-sapcommissions-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.946088 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/
--rw-rw-rw-   0        0        0    17535 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.993292 python-sapcommissions-1.0.0/sapcommissions/
--rw-rw-rw-   0        0        0      922 2023-06-26 20:08:46.000000 python-sapcommissions-1.0.0/sapcommissions/__init__.py
--rw-rw-rw-   0        0        0    25310 2023-06-26 19:40:12.000000 python-sapcommissions-1.0.0/sapcommissions/endpoints.py
--rw-rw-rw-   0        0        0      469 2023-06-26 10:08:08.000000 python-sapcommissions-1.0.0/sapcommissions/exceptions.py
--rw-rw-rw-   0        0        0   114226 2023-06-26 11:52:36.000000 python-sapcommissions-1.0.0/sapcommissions/resources.py
--rw-rw-rw-   0        0        0       42 2023-06-26 21:16:31.051707 python-sapcommissions-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-05-17 08:27:22.000000 python-sapcommissions-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 21:16:31.035611 python-sapcommissions-1.0.0/tests/
--rw-rw-rw-   0        0        0     2411 2023-06-26 20:01:52.000000 python-sapcommissions-1.0.0/tests/test_base.py
--rw-rw-rw-   0        0        0    11948 2023-06-26 19:35:30.000000 python-sapcommissions-1.0.0/tests/test_endpoints.py
--rw-rw-rw-   0        0        0     4560 2023-06-26 19:50:02.000000 python-sapcommissions-1.0.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.117092 python-sapcommissions-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/docs/ENDPOINTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 05:20:29.000000 python-sapcommissions-1.0.1/python_sapcommissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.121092 python-sapcommissions-1.0.1/sapcommissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24379 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112084 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/sapcommissions/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:20:29.125092 python-sapcommissions-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-27 05:20:16.000000 python-sapcommissions-1.0.1/tests/test_resources.py
```

### Comparing `python-sapcommissions-1.0.0/LICENSE` & `python-sapcommissions-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Niels Perfors
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Niels Perfors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `python-sapcommissions-1.0.0/PKG-INFO` & `python-sapcommissions-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,418 +1,417 @@
-Metadata-Version: 2.1
-Name: python-sapcommissions
-Version: 1.0.0
-Summary: A Python wrapper for the SAP Commissions API
-Author-email: Niels Perfors <niels.perfors1987@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# SAP Commissions
-
-A Python wrapper for the SAP Commissions API.
-
-- [SAP Commissions](#sap-commissions)
-  - [Installation](#installation)
-    - [REST API](#rest-api)
-    - [Terminology](#terminology)
-  - [Usage](#usage)
-  - [Methods](#methods)
-    - [List](#list)
-    - [Get](#get)
-    - [Get ID](#get-id)
-    - [Get Versions](#get-versions)
-    - [Create](#create)
-    - [Create Versions](#create-versions)
-    - [Update](#update)
-    - [Update Versions](#update-versions)
-    - [Delete](#delete)
-    - [Delete Versions](#delete-versions)
-
-## Installation
-
-This project is hosted on [GitHub](https://github.com/niro1987/python-sapcommissions).
-To install the project, run the following command:
-
-```text
-pip install git+https://github.com/niro1987/python-sapcommissions.git#egg=sapcommissions
-```
-
-### REST API
-
-This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
-replacing `CALD` with your tenant name, and `ENV` with your environment name.
-
-### Terminology
-
-In this documentation, we talk about endpoints and resources, here is what that means.
-
-| Keyword  | Description                                                                      |
-| -------- | -------------------------------------------------------------------------------- |
-| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
-| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
-| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
-
-## Usage
-
-To get started, import `Connection` and an endpoint of your choosing. In this
-example, we'll use `Participants` as the endpoint.
-
-```py
-from sapcommissions import Connection
-from sapcommissions.endpoints import Participants
-```
-
-Initialize a Connection by providing the tenant, environment, username,
-and password. Optionally, you can disable ssl verification, if you have problems
-connecting to the API from your corporate network.
-
-```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
-```
-
-We'll use the `Participants` endpoint to get a list of all participants in the environment.
-
-```py
-all_users = Participants(prod).list()
-```
-
-## Methods
-
-Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
-Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
-endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
-and `delete_versions()` methods.
-
-### List
-
-The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
-the current effective version of the resource (if the endpoint is versioned). To retrieve a
-different effective version, you must provide both `startDate` and `endDate` parameters.
-
-In most cases, you will want to apply some kind of filter. For a complete list of available filter
-options please visit the [REST API Documentation](#rest-api).
-
-You can limit the number of results returned by providing a `limit`, this is usefull if you want to
-explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
-return the json response from the API without converting it to a Python object.
-
-Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
-`Positions(prod).list(name='John Doe')` is equivalent to
-`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
-combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
-
-```py
-# Get a list of all positions in the environment.
-positions = Positions(prod).list()
-
-# Get a list of all positions with title 'Sales Manager'.
-sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
-```
-
-| Argument      | Type   | Required                   | Description                                      |
-| ------------- | ------ | -------------------------- | ------------------------------------------------ |
-| filter        | `str`  | False                      | A filter string to apply to the list             |
-| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
-| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
-| limit         | `int`  | False                      | Limit the number of returned resources           |
-| raw           | `bool` | False                      | Return the raw json response from the API        |
-| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
-
-| Returns          | Description                               |
-| ---------------- | ----------------------------------------- |
-| `list[Resource]` | A list of resources, single valid version |
-
-### Get
-
-The `get()` method is used to retrieve an existing resource, single (latest) version.
-The method takes a single parameter, `seq` (system unique identifier) of the object to
-retrieve. The `seq` value for a resource is stored in the first attribute, for
-simplicity, it can also be read from the `_seq` property.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns    | Description                              |
-| ---------- | ---------------------------------------- |
-| `Resource` | Requested resource, single valid version |
-
-```py
-# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
-# position, but does not contain any meaningfull information about the manager yet.
-# We can use the `get()` method to enrich the manager data.
-positions = Positions(prod).list()
-
-for position in positions:
-  if position.manager:
-    position.manager = Positions(prod).get(position.manager._seq)
-```
-
-### Get ID
-
-`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
-unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
-id, or the specified `id` could not be found, it returns `None`.
-
-| Argument | Type  | Required | Description                                 |
-| -------- | ----- | -------- | ------------------------------------------- |
-| id       | `str` | True     | The user unique identifier for the resource |
-
-| Returns    | Description                                        |
-| ---------- | -------------------------------------------------- |
-| `Resource` | Requested resource, single valid version           |
-| `None`     | Resource does not have an id or could not be found |
-
-```py
-position = Positions(prod).get_id('John Doe')
-
-# What would have been required without this method.
-position_id_attr = Position._id_attr  # returns 'name'
-positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
-position = positions[0] if positions else None
-```
-
-### Get Versions
-
-The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
-of all versions of the resource.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns          | Description                             |
-| ---------------- | --------------------------------------- |
-| `list[Resource]` | A list of all versions for a  resources |
-
-```py
-# Get all versions for a position.
-positions = Positions(prod).list()
-position = positions[0]
-
-position_versions = Positions(prod).get_versions(first_position._seq)
-```
-
-### Create
-
-With the `create()` method, you can create a new instance of the resource. Unlike the
-REST API, the `create()` method accepts only a single resource as a parameter.
-If successful, the created resource will be returned.
-
-| Argument | Type       | Required | Description                     |
-| -------- | ---------- | -------- | ------------------------------- |
-| instance | `Resource` | True     | The resource instance to create |
-
-| Returns    | Description             |
-| ---------- | ----------------------- |
-| `Resource` | Created resource object |
-
-Make sure to provide all required attributes for the resource. Check the documentation
-for the resource to see which attributes are required.
-
-```py
-# Create a new position, with title 'Account Manager'.
-new_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Account Manager"),
-)
-created_position = Positions(prod).create(new_position)
-```
-
-### Create Versions
-
-The `create_versions()` method is used to create new versions of an existing resource.
-It is imperative that you provide all versions of the resource, as this method will
-overwrite all pre-existing versions with the ones provide. This method can also be used
-to end-date an existing resource. All pre-existing versions of the resource will be
-overwritten.
-
-| Argument  | Type             | Required | Description                                   |
-| --------- | ---------------- | -------- | --------------------------------------------- |
-| seq       | `int`            | True     | The system unique identifier for the resource |
-| instances | `list[Resource]` | True     | The list of resource instances to create      |
-
-| Returns          | Description                       |
-| ---------------- | --------------------------------- |
-| `list[Resource]` | List of created resource versions |
-
-```py
-# Let's create a new version of the position that we just created.
-first_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2020, 12, 31),
-  title=Title(name="Account Manager"),
-)
-second_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2021, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Sales Manager"),
-)
-versions = [first_version, second_version]
-
-created_versions = Positions(prod).create_versions(created_position._seq, versions)
-```
-
-### Update
-
-With the `update()` method, you can update an existing resource. If the endpoint is
-versioned, this methid only updates a single valid version, matching the effective date
-range provided.
-
-| Argument | Type       | Required | Description                   |
-| -------- | ---------- | -------- | ----------------------------- |
-| update   | `Resource` | True     | The updated resource instance |
-
-| Returns    | Description                                   |
-| ---------- | --------------------------------------------- |
-| `Resource` | Updated resource object, single valid version |
-
-```py
-#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
-# to a position group 'Sales'. We'll assume that the position group already exists.
-
-# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
-positions = (
-  Positions(prod)
-  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
-)
-
-# Now update the position group and update the position.
-for position in positions
-  position.positionGroup = PositionGroup(name="Sales")
-  Positions(prod).update(position)
-```
-
-### Update Versions
-
-The `update_versions()` method is used to update the versions of an existing resource.
-It is important to understand the differance between `update()` and `update_versions()`.
-[Update](#update) allows a single valid version of the resource to be updated, it must
-pre-exist in the environment. With `update_versions()`, you can update multiple versions
-at once, and even apply an update without any prior knowledge of pre-existing versions.
-The provided versions will be applied to the current existing versions in the
-environment.
-
-| Argument | Type             | Required | Description                                   |
-| -------- | ---------------- | -------- | --------------------------------------------- |
-| seq      | `int`            | True     | The system unique identifier for the resource |
-| versions | `list[Resource]` | True     | The list of resource version update to apply  |
-
-| Returns          | Description                                                |
-| ---------------- | ---------------------------------------------------------- |
-| `list[Resource]` | List of all resource versions after the update was applied |
-
-**Example:**
-
-```py
-# Let's revisit our previous example where a position is promoted to a different title. Our position
-# already has two versions, the first with a title of 'Account Manager', the second with a title of
-# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
-# knowledge of these versions.
-
-# We'll need to seq number for the position that we are going to update.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-# Now we can update the position
-updated_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2022, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Director"),
-  positionGroup=PositionGroup(name="Management"),
-)
-
-Positions(prod).update_versions(position_seq, [updated_position])
-
-# [
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2020, 1, 1),
-#     effectiveEndDate=date(2020, 12, 31)
-#     title=Title(name="Account Manager"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2021, 1, 1),
-#     effectiveEndDate=date(2021, 12, 31)
-#     title=Title(name="Sales Manager"),
-#     positionGroup=PositionGroup(name="Sales"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2022, 1, 1),
-#     effectiveEndDate=date(2200, 1, 1)
-#     title=Title(name="Director"),
-#     positionGroup=PositionGroup(name="Management"),
-#   ),
-# ]
-```
-
-### Delete
-
-With the `delete()` method, you can fully delete a resource from the environment, all
-effective versions of the resource will be deleted.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns | Description                                                |
-| ------- | ---------------------------------------------------------- |
-| `str`   | Confirmation message `The record is successfully deleted.` |
-
-```py
-# Delete a position with the name 'John Doe'.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = Positions(prod).delete(position._seq)
-assert message == "The record is successfully deleted."
-```
-
-### Delete Versions
-
-The `delete_versions()` method deletes the given versions of the resource. The resulting
-gap will either be filled from the previous or next available version of the resource.
-The effective dates provided must match an existing version of the resource.
-
-| Argument           | Type   | Required | Description                                          |
-| ------------------ | ------ | -------- | ---------------------------------------------------- |
-| seq                | `int`  | True     | The system unique identifier for the resource        |
-| effectiveStartDate | `date` | True     | The start date of the version to delete              |
-| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
-| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
-
-| Returns | Description                                                                  |
-| ------- | ---------------------------------------------------------------------------- |
-| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
-
-```py
-# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
-# previous version.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = (
-  Positions(prod)
-  .delete_versions(
-    seq=position._seq,
-    effectiveStartDate=position.effectiveStartDate,
-    effectiveEndDate=position.effectiveEndDate,
-    fillFromRight=False
-  )
-)
-```
+Metadata-Version: 2.1
+Name: python-sapcommissions
+Version: 1.0.1
+Summary: A Python wrapper for the SAP Commissions API
+Author-email: Niels Perfors <niels.perfors1987@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# SAP Commissions
+
+A Python wrapper for the SAP Commissions API.
+
+- [SAP Commissions](#sap-commissions)
+  - [Installation](#installation)
+    - [REST API](#rest-api)
+    - [Terminology](#terminology)
+  - [Usage](#usage)
+  - [Methods](#methods)
+    - [List](#list)
+    - [Get](#get)
+    - [Get ID](#get-id)
+    - [Get Versions](#get-versions)
+    - [Create](#create)
+    - [Create Versions](#create-versions)
+    - [Update](#update)
+    - [Update Versions](#update-versions)
+    - [Delete](#delete)
+    - [Delete Versions](#delete-versions)
+
+## Installation
+
+To install the project, run the following command:
+
+```text
+pip install python-sapcommissions
+```
+
+### REST API
+
+This project mimics the usage of the SAP Commissions REST API. Visit
+`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
+replacing `CALD` with your tenant name, and `ENV` with your environment name.
+
+### Terminology
+
+In this documentation, we talk about endpoints and resources, here is what that means.
+
+| Keyword  | Description                                                                      |
+| -------- | -------------------------------------------------------------------------------- |
+| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
+| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
+| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
+
+## Usage
+
+To get started, import `Connection` and an endpoint of your choosing. In this
+example, we'll use `Participants` as the endpoint.
+
+```py
+from sapcommissions import Connection
+from sapcommissions.endpoints import Participants
+```
+
+Initialize a Connection by providing the tenant, environment, username,
+and password. Optionally, you can disable ssl verification, if you have problems
+connecting to the API from your corporate network.
+
+```python
+prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
+```
+
+We'll use the `Participants` endpoint to get a list of all participants in the environment.
+
+```py
+all_users = Participants(prod).list()
+```
+
+## Methods
+
+Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
+Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
+endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
+and `delete_versions()` methods.
+
+### List
+
+The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
+the current effective version of the resource (if the endpoint is versioned). To retrieve a
+different effective version, you must provide both `startDate` and `endDate` parameters.
+
+In most cases, you will want to apply some kind of filter. For a complete list of available filter
+options please visit the [REST API Documentation](#rest-api).
+
+You can limit the number of results returned by providing a `limit`, this is usefull if you want to
+explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
+return the json response from the API without converting it to a Python object.
+
+Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
+`Positions(prod).list(name='John Doe')` is equivalent to
+`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
+combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
+
+```py
+# Get a list of all positions in the environment.
+positions = Positions(prod).list()
+
+# Get a list of all positions with title 'Sales Manager'.
+sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
+```
+
+| Argument      | Type   | Required                   | Description                                      |
+| ------------- | ------ | -------------------------- | ------------------------------------------------ |
+| filter        | `str`  | False                      | A filter string to apply to the list             |
+| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
+| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
+| limit         | `int`  | False                      | Limit the number of returned resources           |
+| raw           | `bool` | False                      | Return the raw json response from the API        |
+| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
+
+| Returns          | Description                               |
+| ---------------- | ----------------------------------------- |
+| `list[Resource]` | A list of resources, single valid version |
+
+### Get
+
+The `get()` method is used to retrieve an existing resource, single (latest) version.
+The method takes a single parameter, `seq` (system unique identifier) of the object to
+retrieve. The `seq` value for a resource is stored in the first attribute, for
+simplicity, it can also be read from the `_seq` property.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns    | Description                              |
+| ---------- | ---------------------------------------- |
+| `Resource` | Requested resource, single valid version |
+
+```py
+# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
+# position, but does not contain any meaningfull information about the manager yet.
+# We can use the `get()` method to enrich the manager data.
+positions = Positions(prod).list()
+
+for position in positions:
+  if position.manager:
+    position.manager = Positions(prod).get(position.manager._seq)
+```
+
+### Get ID
+
+`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
+unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
+id, or the specified `id` could not be found, it returns `None`.
+
+| Argument | Type  | Required | Description                                 |
+| -------- | ----- | -------- | ------------------------------------------- |
+| id       | `str` | True     | The user unique identifier for the resource |
+
+| Returns    | Description                                        |
+| ---------- | -------------------------------------------------- |
+| `Resource` | Requested resource, single valid version           |
+| `None`     | Resource does not have an id or could not be found |
+
+```py
+position = Positions(prod).get_id('John Doe')
+
+# What would have been required without this method.
+position_id_attr = Position._id_attr  # returns 'name'
+positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
+position = positions[0] if positions else None
+```
+
+### Get Versions
+
+The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
+of all versions of the resource.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns          | Description                             |
+| ---------------- | --------------------------------------- |
+| `list[Resource]` | A list of all versions for a  resources |
+
+```py
+# Get all versions for a position.
+positions = Positions(prod).list()
+position = positions[0]
+
+position_versions = Positions(prod).get_versions(first_position._seq)
+```
+
+### Create
+
+With the `create()` method, you can create a new instance of the resource. Unlike the
+REST API, the `create()` method accepts only a single resource as a parameter.
+If successful, the created resource will be returned.
+
+| Argument | Type       | Required | Description                     |
+| -------- | ---------- | -------- | ------------------------------- |
+| instance | `Resource` | True     | The resource instance to create |
+
+| Returns    | Description             |
+| ---------- | ----------------------- |
+| `Resource` | Created resource object |
+
+Make sure to provide all required attributes for the resource. Check the documentation
+for the resource to see which attributes are required.
+
+```py
+# Create a new position, with title 'Account Manager'.
+new_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Account Manager"),
+)
+created_position = Positions(prod).create(new_position)
+```
+
+### Create Versions
+
+The `create_versions()` method is used to create new versions of an existing resource.
+It is imperative that you provide all versions of the resource, as this method will
+overwrite all pre-existing versions with the ones provide. This method can also be used
+to end-date an existing resource. All pre-existing versions of the resource will be
+overwritten.
+
+| Argument  | Type             | Required | Description                                   |
+| --------- | ---------------- | -------- | --------------------------------------------- |
+| seq       | `int`            | True     | The system unique identifier for the resource |
+| instances | `list[Resource]` | True     | The list of resource instances to create      |
+
+| Returns          | Description                       |
+| ---------------- | --------------------------------- |
+| `list[Resource]` | List of created resource versions |
+
+```py
+# Let's create a new version of the position that we just created.
+first_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2020, 12, 31),
+  title=Title(name="Account Manager"),
+)
+second_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2021, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Sales Manager"),
+)
+versions = [first_version, second_version]
+
+created_versions = Positions(prod).create_versions(created_position._seq, versions)
+```
+
+### Update
+
+With the `update()` method, you can update an existing resource. If the endpoint is
+versioned, this methid only updates a single valid version, matching the effective date
+range provided.
+
+| Argument | Type       | Required | Description                   |
+| -------- | ---------- | -------- | ----------------------------- |
+| update   | `Resource` | True     | The updated resource instance |
+
+| Returns    | Description                                   |
+| ---------- | --------------------------------------------- |
+| `Resource` | Updated resource object, single valid version |
+
+```py
+#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
+# to a position group 'Sales'. We'll assume that the position group already exists.
+
+# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
+positions = (
+  Positions(prod)
+  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
+)
+
+# Now update the position group and update the position.
+for position in positions
+  position.positionGroup = PositionGroup(name="Sales")
+  Positions(prod).update(position)
+```
+
+### Update Versions
+
+The `update_versions()` method is used to update the versions of an existing resource.
+It is important to understand the differance between `update()` and `update_versions()`.
+[Update](#update) allows a single valid version of the resource to be updated, it must
+pre-exist in the environment. With `update_versions()`, you can update multiple versions
+at once, and even apply an update without any prior knowledge of pre-existing versions.
+The provided versions will be applied to the current existing versions in the
+environment.
+
+| Argument | Type             | Required | Description                                   |
+| -------- | ---------------- | -------- | --------------------------------------------- |
+| seq      | `int`            | True     | The system unique identifier for the resource |
+| versions | `list[Resource]` | True     | The list of resource version update to apply  |
+
+| Returns          | Description                                                |
+| ---------------- | ---------------------------------------------------------- |
+| `list[Resource]` | List of all resource versions after the update was applied |
+
+**Example:**
+
+```py
+# Let's revisit our previous example where a position is promoted to a different title. Our position
+# already has two versions, the first with a title of 'Account Manager', the second with a title of
+# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
+# knowledge of these versions.
+
+# We'll need to seq number for the position that we are going to update.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+# Now we can update the position
+updated_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2022, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Director"),
+  positionGroup=PositionGroup(name="Management"),
+)
+
+Positions(prod).update_versions(position_seq, [updated_position])
+
+# [
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2020, 1, 1),
+#     effectiveEndDate=date(2020, 12, 31)
+#     title=Title(name="Account Manager"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2021, 1, 1),
+#     effectiveEndDate=date(2021, 12, 31)
+#     title=Title(name="Sales Manager"),
+#     positionGroup=PositionGroup(name="Sales"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2022, 1, 1),
+#     effectiveEndDate=date(2200, 1, 1)
+#     title=Title(name="Director"),
+#     positionGroup=PositionGroup(name="Management"),
+#   ),
+# ]
+```
+
+### Delete
+
+With the `delete()` method, you can fully delete a resource from the environment, all
+effective versions of the resource will be deleted.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns | Description                                                |
+| ------- | ---------------------------------------------------------- |
+| `str`   | Confirmation message `The record is successfully deleted.` |
+
+```py
+# Delete a position with the name 'John Doe'.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = Positions(prod).delete(position._seq)
+assert message == "The record is successfully deleted."
+```
+
+### Delete Versions
+
+The `delete_versions()` method deletes the given versions of the resource. The resulting
+gap will either be filled from the previous or next available version of the resource.
+The effective dates provided must match an existing version of the resource.
+
+| Argument           | Type   | Required | Description                                          |
+| ------------------ | ------ | -------- | ---------------------------------------------------- |
+| seq                | `int`  | True     | The system unique identifier for the resource        |
+| effectiveStartDate | `date` | True     | The start date of the version to delete              |
+| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
+| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
+
+| Returns | Description                                                                  |
+| ------- | ---------------------------------------------------------------------------- |
+| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
+
+```py
+# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
+# previous version.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = (
+  Positions(prod)
+  .delete_versions(
+    seq=position._seq,
+    effectiveStartDate=position.effectiveStartDate,
+    effectiveEndDate=position.effectiveEndDate,
+    fillFromRight=False
+  )
+)
+```
```

### Comparing `python-sapcommissions-1.0.0/docs/README.md` & `python-sapcommissions-1.0.1/python_sapcommissions.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,402 +1,417 @@
-# SAP Commissions
-
-A Python wrapper for the SAP Commissions API.
-
-- [SAP Commissions](#sap-commissions)
-  - [Installation](#installation)
-    - [REST API](#rest-api)
-    - [Terminology](#terminology)
-  - [Usage](#usage)
-  - [Methods](#methods)
-    - [List](#list)
-    - [Get](#get)
-    - [Get ID](#get-id)
-    - [Get Versions](#get-versions)
-    - [Create](#create)
-    - [Create Versions](#create-versions)
-    - [Update](#update)
-    - [Update Versions](#update-versions)
-    - [Delete](#delete)
-    - [Delete Versions](#delete-versions)
-
-## Installation
-
-This project is hosted on [GitHub](https://github.com/niro1987/python-sapcommissions).
-To install the project, run the following command:
-
-```text
-pip install git+https://github.com/niro1987/python-sapcommissions.git#egg=sapcommissions
-```
-
-### REST API
-
-This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
-replacing `CALD` with your tenant name, and `ENV` with your environment name.
-
-### Terminology
-
-In this documentation, we talk about endpoints and resources, here is what that means.
-
-| Keyword  | Description                                                                      |
-| -------- | -------------------------------------------------------------------------------- |
-| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
-| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
-| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
-
-## Usage
-
-To get started, import `Connection` and an endpoint of your choosing. In this
-example, we'll use `Participants` as the endpoint.
-
-```py
-from sapcommissions import Connection
-from sapcommissions.endpoints import Participants
-```
-
-Initialize a Connection by providing the tenant, environment, username,
-and password. Optionally, you can disable ssl verification, if you have problems
-connecting to the API from your corporate network.
-
-```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
-```
-
-We'll use the `Participants` endpoint to get a list of all participants in the environment.
-
-```py
-all_users = Participants(prod).list()
-```
-
-## Methods
-
-Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
-Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
-endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
-and `delete_versions()` methods.
-
-### List
-
-The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
-the current effective version of the resource (if the endpoint is versioned). To retrieve a
-different effective version, you must provide both `startDate` and `endDate` parameters.
-
-In most cases, you will want to apply some kind of filter. For a complete list of available filter
-options please visit the [REST API Documentation](#rest-api).
-
-You can limit the number of results returned by providing a `limit`, this is usefull if you want to
-explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
-return the json response from the API without converting it to a Python object.
-
-Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
-`Positions(prod).list(name='John Doe')` is equivalent to
-`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
-combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
-
-```py
-# Get a list of all positions in the environment.
-positions = Positions(prod).list()
-
-# Get a list of all positions with title 'Sales Manager'.
-sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
-```
-
-| Argument      | Type   | Required                   | Description                                      |
-| ------------- | ------ | -------------------------- | ------------------------------------------------ |
-| filter        | `str`  | False                      | A filter string to apply to the list             |
-| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
-| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
-| limit         | `int`  | False                      | Limit the number of returned resources           |
-| raw           | `bool` | False                      | Return the raw json response from the API        |
-| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
-
-| Returns          | Description                               |
-| ---------------- | ----------------------------------------- |
-| `list[Resource]` | A list of resources, single valid version |
-
-### Get
-
-The `get()` method is used to retrieve an existing resource, single (latest) version.
-The method takes a single parameter, `seq` (system unique identifier) of the object to
-retrieve. The `seq` value for a resource is stored in the first attribute, for
-simplicity, it can also be read from the `_seq` property.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns    | Description                              |
-| ---------- | ---------------------------------------- |
-| `Resource` | Requested resource, single valid version |
-
-```py
-# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
-# position, but does not contain any meaningfull information about the manager yet.
-# We can use the `get()` method to enrich the manager data.
-positions = Positions(prod).list()
-
-for position in positions:
-  if position.manager:
-    position.manager = Positions(prod).get(position.manager._seq)
-```
-
-### Get ID
-
-`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
-unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
-id, or the specified `id` could not be found, it returns `None`.
-
-| Argument | Type  | Required | Description                                 |
-| -------- | ----- | -------- | ------------------------------------------- |
-| id       | `str` | True     | The user unique identifier for the resource |
-
-| Returns    | Description                                        |
-| ---------- | -------------------------------------------------- |
-| `Resource` | Requested resource, single valid version           |
-| `None`     | Resource does not have an id or could not be found |
-
-```py
-position = Positions(prod).get_id('John Doe')
-
-# What would have been required without this method.
-position_id_attr = Position._id_attr  # returns 'name'
-positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
-position = positions[0] if positions else None
-```
-
-### Get Versions
-
-The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
-of all versions of the resource.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns          | Description                             |
-| ---------------- | --------------------------------------- |
-| `list[Resource]` | A list of all versions for a  resources |
-
-```py
-# Get all versions for a position.
-positions = Positions(prod).list()
-position = positions[0]
-
-position_versions = Positions(prod).get_versions(first_position._seq)
-```
-
-### Create
-
-With the `create()` method, you can create a new instance of the resource. Unlike the
-REST API, the `create()` method accepts only a single resource as a parameter.
-If successful, the created resource will be returned.
-
-| Argument | Type       | Required | Description                     |
-| -------- | ---------- | -------- | ------------------------------- |
-| instance | `Resource` | True     | The resource instance to create |
-
-| Returns    | Description             |
-| ---------- | ----------------------- |
-| `Resource` | Created resource object |
-
-Make sure to provide all required attributes for the resource. Check the documentation
-for the resource to see which attributes are required.
-
-```py
-# Create a new position, with title 'Account Manager'.
-new_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Account Manager"),
-)
-created_position = Positions(prod).create(new_position)
-```
-
-### Create Versions
-
-The `create_versions()` method is used to create new versions of an existing resource.
-It is imperative that you provide all versions of the resource, as this method will
-overwrite all pre-existing versions with the ones provide. This method can also be used
-to end-date an existing resource. All pre-existing versions of the resource will be
-overwritten.
-
-| Argument  | Type             | Required | Description                                   |
-| --------- | ---------------- | -------- | --------------------------------------------- |
-| seq       | `int`            | True     | The system unique identifier for the resource |
-| instances | `list[Resource]` | True     | The list of resource instances to create      |
-
-| Returns          | Description                       |
-| ---------------- | --------------------------------- |
-| `list[Resource]` | List of created resource versions |
-
-```py
-# Let's create a new version of the position that we just created.
-first_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2020, 12, 31),
-  title=Title(name="Account Manager"),
-)
-second_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2021, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Sales Manager"),
-)
-versions = [first_version, second_version]
-
-created_versions = Positions(prod).create_versions(created_position._seq, versions)
-```
-
-### Update
-
-With the `update()` method, you can update an existing resource. If the endpoint is
-versioned, this methid only updates a single valid version, matching the effective date
-range provided.
-
-| Argument | Type       | Required | Description                   |
-| -------- | ---------- | -------- | ----------------------------- |
-| update   | `Resource` | True     | The updated resource instance |
-
-| Returns    | Description                                   |
-| ---------- | --------------------------------------------- |
-| `Resource` | Updated resource object, single valid version |
-
-```py
-#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
-# to a position group 'Sales'. We'll assume that the position group already exists.
-
-# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
-positions = (
-  Positions(prod)
-  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
-)
-
-# Now update the position group and update the position.
-for position in positions
-  position.positionGroup = PositionGroup(name="Sales")
-  Positions(prod).update(position)
-```
-
-### Update Versions
-
-The `update_versions()` method is used to update the versions of an existing resource.
-It is important to understand the differance between `update()` and `update_versions()`.
-[Update](#update) allows a single valid version of the resource to be updated, it must
-pre-exist in the environment. With `update_versions()`, you can update multiple versions
-at once, and even apply an update without any prior knowledge of pre-existing versions.
-The provided versions will be applied to the current existing versions in the
-environment.
-
-| Argument | Type             | Required | Description                                   |
-| -------- | ---------------- | -------- | --------------------------------------------- |
-| seq      | `int`            | True     | The system unique identifier for the resource |
-| versions | `list[Resource]` | True     | The list of resource version update to apply  |
-
-| Returns          | Description                                                |
-| ---------------- | ---------------------------------------------------------- |
-| `list[Resource]` | List of all resource versions after the update was applied |
-
-**Example:**
-
-```py
-# Let's revisit our previous example where a position is promoted to a different title. Our position
-# already has two versions, the first with a title of 'Account Manager', the second with a title of
-# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
-# knowledge of these versions.
-
-# We'll need to seq number for the position that we are going to update.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-# Now we can update the position
-updated_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2022, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Director"),
-  positionGroup=PositionGroup(name="Management"),
-)
-
-Positions(prod).update_versions(position_seq, [updated_position])
-
-# [
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2020, 1, 1),
-#     effectiveEndDate=date(2020, 12, 31)
-#     title=Title(name="Account Manager"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2021, 1, 1),
-#     effectiveEndDate=date(2021, 12, 31)
-#     title=Title(name="Sales Manager"),
-#     positionGroup=PositionGroup(name="Sales"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2022, 1, 1),
-#     effectiveEndDate=date(2200, 1, 1)
-#     title=Title(name="Director"),
-#     positionGroup=PositionGroup(name="Management"),
-#   ),
-# ]
-```
-
-### Delete
-
-With the `delete()` method, you can fully delete a resource from the environment, all
-effective versions of the resource will be deleted.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns | Description                                                |
-| ------- | ---------------------------------------------------------- |
-| `str`   | Confirmation message `The record is successfully deleted.` |
-
-```py
-# Delete a position with the name 'John Doe'.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = Positions(prod).delete(position._seq)
-assert message == "The record is successfully deleted."
-```
-
-### Delete Versions
-
-The `delete_versions()` method deletes the given versions of the resource. The resulting
-gap will either be filled from the previous or next available version of the resource.
-The effective dates provided must match an existing version of the resource.
-
-| Argument           | Type   | Required | Description                                          |
-| ------------------ | ------ | -------- | ---------------------------------------------------- |
-| seq                | `int`  | True     | The system unique identifier for the resource        |
-| effectiveStartDate | `date` | True     | The start date of the version to delete              |
-| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
-| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
-
-| Returns | Description                                                                  |
-| ------- | ---------------------------------------------------------------------------- |
-| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
-
-```py
-# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
-# previous version.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = (
-  Positions(prod)
-  .delete_versions(
-    seq=position._seq,
-    effectiveStartDate=position.effectiveStartDate,
-    effectiveEndDate=position.effectiveEndDate,
-    fillFromRight=False
-  )
-)
-```
+Metadata-Version: 2.1
+Name: python-sapcommissions
+Version: 1.0.1
+Summary: A Python wrapper for the SAP Commissions API
+Author-email: Niels Perfors <niels.perfors1987@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# SAP Commissions
+
+A Python wrapper for the SAP Commissions API.
+
+- [SAP Commissions](#sap-commissions)
+  - [Installation](#installation)
+    - [REST API](#rest-api)
+    - [Terminology](#terminology)
+  - [Usage](#usage)
+  - [Methods](#methods)
+    - [List](#list)
+    - [Get](#get)
+    - [Get ID](#get-id)
+    - [Get Versions](#get-versions)
+    - [Create](#create)
+    - [Create Versions](#create-versions)
+    - [Update](#update)
+    - [Update Versions](#update-versions)
+    - [Delete](#delete)
+    - [Delete Versions](#delete-versions)
+
+## Installation
+
+To install the project, run the following command:
+
+```text
+pip install python-sapcommissions
+```
+
+### REST API
+
+This project mimics the usage of the SAP Commissions REST API. Visit
+`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
+replacing `CALD` with your tenant name, and `ENV` with your environment name.
+
+### Terminology
+
+In this documentation, we talk about endpoints and resources, here is what that means.
+
+| Keyword  | Description                                                                      |
+| -------- | -------------------------------------------------------------------------------- |
+| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
+| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
+| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
+
+## Usage
+
+To get started, import `Connection` and an endpoint of your choosing. In this
+example, we'll use `Participants` as the endpoint.
+
+```py
+from sapcommissions import Connection
+from sapcommissions.endpoints import Participants
+```
+
+Initialize a Connection by providing the tenant, environment, username,
+and password. Optionally, you can disable ssl verification, if you have problems
+connecting to the API from your corporate network.
+
+```python
+prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
+```
+
+We'll use the `Participants` endpoint to get a list of all participants in the environment.
+
+```py
+all_users = Participants(prod).list()
+```
+
+## Methods
+
+Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
+Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
+endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
+and `delete_versions()` methods.
+
+### List
+
+The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
+the current effective version of the resource (if the endpoint is versioned). To retrieve a
+different effective version, you must provide both `startDate` and `endDate` parameters.
+
+In most cases, you will want to apply some kind of filter. For a complete list of available filter
+options please visit the [REST API Documentation](#rest-api).
+
+You can limit the number of results returned by providing a `limit`, this is usefull if you want to
+explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
+return the json response from the API without converting it to a Python object.
+
+Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
+`Positions(prod).list(name='John Doe')` is equivalent to
+`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
+combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
+
+```py
+# Get a list of all positions in the environment.
+positions = Positions(prod).list()
+
+# Get a list of all positions with title 'Sales Manager'.
+sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
+```
+
+| Argument      | Type   | Required                   | Description                                      |
+| ------------- | ------ | -------------------------- | ------------------------------------------------ |
+| filter        | `str`  | False                      | A filter string to apply to the list             |
+| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
+| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
+| limit         | `int`  | False                      | Limit the number of returned resources           |
+| raw           | `bool` | False                      | Return the raw json response from the API        |
+| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
+
+| Returns          | Description                               |
+| ---------------- | ----------------------------------------- |
+| `list[Resource]` | A list of resources, single valid version |
+
+### Get
+
+The `get()` method is used to retrieve an existing resource, single (latest) version.
+The method takes a single parameter, `seq` (system unique identifier) of the object to
+retrieve. The `seq` value for a resource is stored in the first attribute, for
+simplicity, it can also be read from the `_seq` property.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns    | Description                              |
+| ---------- | ---------------------------------------- |
+| `Resource` | Requested resource, single valid version |
+
+```py
+# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
+# position, but does not contain any meaningfull information about the manager yet.
+# We can use the `get()` method to enrich the manager data.
+positions = Positions(prod).list()
+
+for position in positions:
+  if position.manager:
+    position.manager = Positions(prod).get(position.manager._seq)
+```
+
+### Get ID
+
+`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
+unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
+id, or the specified `id` could not be found, it returns `None`.
+
+| Argument | Type  | Required | Description                                 |
+| -------- | ----- | -------- | ------------------------------------------- |
+| id       | `str` | True     | The user unique identifier for the resource |
+
+| Returns    | Description                                        |
+| ---------- | -------------------------------------------------- |
+| `Resource` | Requested resource, single valid version           |
+| `None`     | Resource does not have an id or could not be found |
+
+```py
+position = Positions(prod).get_id('John Doe')
+
+# What would have been required without this method.
+position_id_attr = Position._id_attr  # returns 'name'
+positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
+position = positions[0] if positions else None
+```
+
+### Get Versions
+
+The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
+of all versions of the resource.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns          | Description                             |
+| ---------------- | --------------------------------------- |
+| `list[Resource]` | A list of all versions for a  resources |
+
+```py
+# Get all versions for a position.
+positions = Positions(prod).list()
+position = positions[0]
+
+position_versions = Positions(prod).get_versions(first_position._seq)
+```
+
+### Create
+
+With the `create()` method, you can create a new instance of the resource. Unlike the
+REST API, the `create()` method accepts only a single resource as a parameter.
+If successful, the created resource will be returned.
+
+| Argument | Type       | Required | Description                     |
+| -------- | ---------- | -------- | ------------------------------- |
+| instance | `Resource` | True     | The resource instance to create |
+
+| Returns    | Description             |
+| ---------- | ----------------------- |
+| `Resource` | Created resource object |
+
+Make sure to provide all required attributes for the resource. Check the documentation
+for the resource to see which attributes are required.
+
+```py
+# Create a new position, with title 'Account Manager'.
+new_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Account Manager"),
+)
+created_position = Positions(prod).create(new_position)
+```
+
+### Create Versions
+
+The `create_versions()` method is used to create new versions of an existing resource.
+It is imperative that you provide all versions of the resource, as this method will
+overwrite all pre-existing versions with the ones provide. This method can also be used
+to end-date an existing resource. All pre-existing versions of the resource will be
+overwritten.
+
+| Argument  | Type             | Required | Description                                   |
+| --------- | ---------------- | -------- | --------------------------------------------- |
+| seq       | `int`            | True     | The system unique identifier for the resource |
+| instances | `list[Resource]` | True     | The list of resource instances to create      |
+
+| Returns          | Description                       |
+| ---------------- | --------------------------------- |
+| `list[Resource]` | List of created resource versions |
+
+```py
+# Let's create a new version of the position that we just created.
+first_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2020, 12, 31),
+  title=Title(name="Account Manager"),
+)
+second_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2021, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Sales Manager"),
+)
+versions = [first_version, second_version]
+
+created_versions = Positions(prod).create_versions(created_position._seq, versions)
+```
+
+### Update
+
+With the `update()` method, you can update an existing resource. If the endpoint is
+versioned, this methid only updates a single valid version, matching the effective date
+range provided.
+
+| Argument | Type       | Required | Description                   |
+| -------- | ---------- | -------- | ----------------------------- |
+| update   | `Resource` | True     | The updated resource instance |
+
+| Returns    | Description                                   |
+| ---------- | --------------------------------------------- |
+| `Resource` | Updated resource object, single valid version |
+
+```py
+#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
+# to a position group 'Sales'. We'll assume that the position group already exists.
+
+# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
+positions = (
+  Positions(prod)
+  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
+)
+
+# Now update the position group and update the position.
+for position in positions
+  position.positionGroup = PositionGroup(name="Sales")
+  Positions(prod).update(position)
+```
+
+### Update Versions
+
+The `update_versions()` method is used to update the versions of an existing resource.
+It is important to understand the differance between `update()` and `update_versions()`.
+[Update](#update) allows a single valid version of the resource to be updated, it must
+pre-exist in the environment. With `update_versions()`, you can update multiple versions
+at once, and even apply an update without any prior knowledge of pre-existing versions.
+The provided versions will be applied to the current existing versions in the
+environment.
+
+| Argument | Type             | Required | Description                                   |
+| -------- | ---------------- | -------- | --------------------------------------------- |
+| seq      | `int`            | True     | The system unique identifier for the resource |
+| versions | `list[Resource]` | True     | The list of resource version update to apply  |
+
+| Returns          | Description                                                |
+| ---------------- | ---------------------------------------------------------- |
+| `list[Resource]` | List of all resource versions after the update was applied |
+
+**Example:**
+
+```py
+# Let's revisit our previous example where a position is promoted to a different title. Our position
+# already has two versions, the first with a title of 'Account Manager', the second with a title of
+# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
+# knowledge of these versions.
+
+# We'll need to seq number for the position that we are going to update.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+# Now we can update the position
+updated_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2022, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Director"),
+  positionGroup=PositionGroup(name="Management"),
+)
+
+Positions(prod).update_versions(position_seq, [updated_position])
+
+# [
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2020, 1, 1),
+#     effectiveEndDate=date(2020, 12, 31)
+#     title=Title(name="Account Manager"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2021, 1, 1),
+#     effectiveEndDate=date(2021, 12, 31)
+#     title=Title(name="Sales Manager"),
+#     positionGroup=PositionGroup(name="Sales"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2022, 1, 1),
+#     effectiveEndDate=date(2200, 1, 1)
+#     title=Title(name="Director"),
+#     positionGroup=PositionGroup(name="Management"),
+#   ),
+# ]
+```
+
+### Delete
+
+With the `delete()` method, you can fully delete a resource from the environment, all
+effective versions of the resource will be deleted.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns | Description                                                |
+| ------- | ---------------------------------------------------------- |
+| `str`   | Confirmation message `The record is successfully deleted.` |
+
+```py
+# Delete a position with the name 'John Doe'.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = Positions(prod).delete(position._seq)
+assert message == "The record is successfully deleted."
+```
+
+### Delete Versions
+
+The `delete_versions()` method deletes the given versions of the resource. The resulting
+gap will either be filled from the previous or next available version of the resource.
+The effective dates provided must match an existing version of the resource.
+
+| Argument           | Type   | Required | Description                                          |
+| ------------------ | ------ | -------- | ---------------------------------------------------- |
+| seq                | `int`  | True     | The system unique identifier for the resource        |
+| effectiveStartDate | `date` | True     | The start date of the version to delete              |
+| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
+| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
+
+| Returns | Description                                                                  |
+| ------- | ---------------------------------------------------------------------------- |
+| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
+
+```py
+# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
+# previous version.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = (
+  Positions(prod)
+  .delete_versions(
+    seq=position._seq,
+    effectiveStartDate=position.effectiveStartDate,
+    effectiveEndDate=position.effectiveEndDate,
+    fillFromRight=False
+  )
+)
+```
```

### Comparing `python-sapcommissions-1.0.0/python_sapcommissions.egg-info/PKG-INFO` & `python-sapcommissions-1.0.1/docs/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,418 +1,401 @@
-Metadata-Version: 2.1
-Name: python-sapcommissions
-Version: 1.0.0
-Summary: A Python wrapper for the SAP Commissions API
-Author-email: Niels Perfors <niels.perfors1987@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# SAP Commissions
-
-A Python wrapper for the SAP Commissions API.
-
-- [SAP Commissions](#sap-commissions)
-  - [Installation](#installation)
-    - [REST API](#rest-api)
-    - [Terminology](#terminology)
-  - [Usage](#usage)
-  - [Methods](#methods)
-    - [List](#list)
-    - [Get](#get)
-    - [Get ID](#get-id)
-    - [Get Versions](#get-versions)
-    - [Create](#create)
-    - [Create Versions](#create-versions)
-    - [Update](#update)
-    - [Update Versions](#update-versions)
-    - [Delete](#delete)
-    - [Delete Versions](#delete-versions)
-
-## Installation
-
-This project is hosted on [GitHub](https://github.com/niro1987/python-sapcommissions).
-To install the project, run the following command:
-
-```text
-pip install git+https://github.com/niro1987/python-sapcommissions.git#egg=sapcommissions
-```
-
-### REST API
-
-This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
-replacing `CALD` with your tenant name, and `ENV` with your environment name.
-
-### Terminology
-
-In this documentation, we talk about endpoints and resources, here is what that means.
-
-| Keyword  | Description                                                                      |
-| -------- | -------------------------------------------------------------------------------- |
-| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
-| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
-| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
-
-## Usage
-
-To get started, import `Connection` and an endpoint of your choosing. In this
-example, we'll use `Participants` as the endpoint.
-
-```py
-from sapcommissions import Connection
-from sapcommissions.endpoints import Participants
-```
-
-Initialize a Connection by providing the tenant, environment, username,
-and password. Optionally, you can disable ssl verification, if you have problems
-connecting to the API from your corporate network.
-
-```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
-```
-
-We'll use the `Participants` endpoint to get a list of all participants in the environment.
-
-```py
-all_users = Participants(prod).list()
-```
-
-## Methods
-
-Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
-Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
-endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
-and `delete_versions()` methods.
-
-### List
-
-The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
-the current effective version of the resource (if the endpoint is versioned). To retrieve a
-different effective version, you must provide both `startDate` and `endDate` parameters.
-
-In most cases, you will want to apply some kind of filter. For a complete list of available filter
-options please visit the [REST API Documentation](#rest-api).
-
-You can limit the number of results returned by providing a `limit`, this is usefull if you want to
-explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
-return the json response from the API without converting it to a Python object.
-
-Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
-`Positions(prod).list(name='John Doe')` is equivalent to
-`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
-combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
-
-```py
-# Get a list of all positions in the environment.
-positions = Positions(prod).list()
-
-# Get a list of all positions with title 'Sales Manager'.
-sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
-```
-
-| Argument      | Type   | Required                   | Description                                      |
-| ------------- | ------ | -------------------------- | ------------------------------------------------ |
-| filter        | `str`  | False                      | A filter string to apply to the list             |
-| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
-| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
-| limit         | `int`  | False                      | Limit the number of returned resources           |
-| raw           | `bool` | False                      | Return the raw json response from the API        |
-| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
-
-| Returns          | Description                               |
-| ---------------- | ----------------------------------------- |
-| `list[Resource]` | A list of resources, single valid version |
-
-### Get
-
-The `get()` method is used to retrieve an existing resource, single (latest) version.
-The method takes a single parameter, `seq` (system unique identifier) of the object to
-retrieve. The `seq` value for a resource is stored in the first attribute, for
-simplicity, it can also be read from the `_seq` property.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns    | Description                              |
-| ---------- | ---------------------------------------- |
-| `Resource` | Requested resource, single valid version |
-
-```py
-# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
-# position, but does not contain any meaningfull information about the manager yet.
-# We can use the `get()` method to enrich the manager data.
-positions = Positions(prod).list()
-
-for position in positions:
-  if position.manager:
-    position.manager = Positions(prod).get(position.manager._seq)
-```
-
-### Get ID
-
-`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
-unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
-id, or the specified `id` could not be found, it returns `None`.
-
-| Argument | Type  | Required | Description                                 |
-| -------- | ----- | -------- | ------------------------------------------- |
-| id       | `str` | True     | The user unique identifier for the resource |
-
-| Returns    | Description                                        |
-| ---------- | -------------------------------------------------- |
-| `Resource` | Requested resource, single valid version           |
-| `None`     | Resource does not have an id or could not be found |
-
-```py
-position = Positions(prod).get_id('John Doe')
-
-# What would have been required without this method.
-position_id_attr = Position._id_attr  # returns 'name'
-positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
-position = positions[0] if positions else None
-```
-
-### Get Versions
-
-The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
-of all versions of the resource.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns          | Description                             |
-| ---------------- | --------------------------------------- |
-| `list[Resource]` | A list of all versions for a  resources |
-
-```py
-# Get all versions for a position.
-positions = Positions(prod).list()
-position = positions[0]
-
-position_versions = Positions(prod).get_versions(first_position._seq)
-```
-
-### Create
-
-With the `create()` method, you can create a new instance of the resource. Unlike the
-REST API, the `create()` method accepts only a single resource as a parameter.
-If successful, the created resource will be returned.
-
-| Argument | Type       | Required | Description                     |
-| -------- | ---------- | -------- | ------------------------------- |
-| instance | `Resource` | True     | The resource instance to create |
-
-| Returns    | Description             |
-| ---------- | ----------------------- |
-| `Resource` | Created resource object |
-
-Make sure to provide all required attributes for the resource. Check the documentation
-for the resource to see which attributes are required.
-
-```py
-# Create a new position, with title 'Account Manager'.
-new_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Account Manager"),
-)
-created_position = Positions(prod).create(new_position)
-```
-
-### Create Versions
-
-The `create_versions()` method is used to create new versions of an existing resource.
-It is imperative that you provide all versions of the resource, as this method will
-overwrite all pre-existing versions with the ones provide. This method can also be used
-to end-date an existing resource. All pre-existing versions of the resource will be
-overwritten.
-
-| Argument  | Type             | Required | Description                                   |
-| --------- | ---------------- | -------- | --------------------------------------------- |
-| seq       | `int`            | True     | The system unique identifier for the resource |
-| instances | `list[Resource]` | True     | The list of resource instances to create      |
-
-| Returns          | Description                       |
-| ---------------- | --------------------------------- |
-| `list[Resource]` | List of created resource versions |
-
-```py
-# Let's create a new version of the position that we just created.
-first_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2020, 1, 1),
-  effectiveEndDate=date(2020, 12, 31),
-  title=Title(name="Account Manager"),
-)
-second_version = Position(
-  name="John Doe",
-  effectiveStartDate=date(2021, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Sales Manager"),
-)
-versions = [first_version, second_version]
-
-created_versions = Positions(prod).create_versions(created_position._seq, versions)
-```
-
-### Update
-
-With the `update()` method, you can update an existing resource. If the endpoint is
-versioned, this methid only updates a single valid version, matching the effective date
-range provided.
-
-| Argument | Type       | Required | Description                   |
-| -------- | ---------- | -------- | ----------------------------- |
-| update   | `Resource` | True     | The updated resource instance |
-
-| Returns    | Description                                   |
-| ---------- | --------------------------------------------- |
-| `Resource` | Updated resource object, single valid version |
-
-```py
-#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
-# to a position group 'Sales'. We'll assume that the position group already exists.
-
-# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
-positions = (
-  Positions(prod)
-  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
-)
-
-# Now update the position group and update the position.
-for position in positions
-  position.positionGroup = PositionGroup(name="Sales")
-  Positions(prod).update(position)
-```
-
-### Update Versions
-
-The `update_versions()` method is used to update the versions of an existing resource.
-It is important to understand the differance between `update()` and `update_versions()`.
-[Update](#update) allows a single valid version of the resource to be updated, it must
-pre-exist in the environment. With `update_versions()`, you can update multiple versions
-at once, and even apply an update without any prior knowledge of pre-existing versions.
-The provided versions will be applied to the current existing versions in the
-environment.
-
-| Argument | Type             | Required | Description                                   |
-| -------- | ---------------- | -------- | --------------------------------------------- |
-| seq      | `int`            | True     | The system unique identifier for the resource |
-| versions | `list[Resource]` | True     | The list of resource version update to apply  |
-
-| Returns          | Description                                                |
-| ---------------- | ---------------------------------------------------------- |
-| `list[Resource]` | List of all resource versions after the update was applied |
-
-**Example:**
-
-```py
-# Let's revisit our previous example where a position is promoted to a different title. Our position
-# already has two versions, the first with a title of 'Account Manager', the second with a title of
-# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
-# knowledge of these versions.
-
-# We'll need to seq number for the position that we are going to update.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-# Now we can update the position
-updated_position = Position(
-  name="John Doe",
-  effectiveStartDate=date(2022, 1, 1),
-  effectiveEndDate=date(2200, 1, 1),
-  title=Title(name="Director"),
-  positionGroup=PositionGroup(name="Management"),
-)
-
-Positions(prod).update_versions(position_seq, [updated_position])
-
-# [
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2020, 1, 1),
-#     effectiveEndDate=date(2020, 12, 31)
-#     title=Title(name="Account Manager"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2021, 1, 1),
-#     effectiveEndDate=date(2021, 12, 31)
-#     title=Title(name="Sales Manager"),
-#     positionGroup=PositionGroup(name="Sales"),
-#   ),
-#   Position(
-#     name="John Doe",
-#     effectiveStartDate=date(2022, 1, 1),
-#     effectiveEndDate=date(2200, 1, 1)
-#     title=Title(name="Director"),
-#     positionGroup=PositionGroup(name="Management"),
-#   ),
-# ]
-```
-
-### Delete
-
-With the `delete()` method, you can fully delete a resource from the environment, all
-effective versions of the resource will be deleted.
-
-| Argument | Type  | Required | Description                                   |
-| -------- | ----- | -------- | --------------------------------------------- |
-| seq      | `int` | True     | The system unique identifier for the resource |
-
-| Returns | Description                                                |
-| ------- | ---------------------------------------------------------- |
-| `str`   | Confirmation message `The record is successfully deleted.` |
-
-```py
-# Delete a position with the name 'John Doe'.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = Positions(prod).delete(position._seq)
-assert message == "The record is successfully deleted."
-```
-
-### Delete Versions
-
-The `delete_versions()` method deletes the given versions of the resource. The resulting
-gap will either be filled from the previous or next available version of the resource.
-The effective dates provided must match an existing version of the resource.
-
-| Argument           | Type   | Required | Description                                          |
-| ------------------ | ------ | -------- | ---------------------------------------------------- |
-| seq                | `int`  | True     | The system unique identifier for the resource        |
-| effectiveStartDate | `date` | True     | The start date of the version to delete              |
-| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
-| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
-
-| Returns | Description                                                                  |
-| ------- | ---------------------------------------------------------------------------- |
-| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
-
-```py
-# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
-# previous version.
-positions = Positions(prod).list(filter="name eq 'John Doe'")
-position = positions[0]
-
-message = (
-  Positions(prod)
-  .delete_versions(
-    seq=position._seq,
-    effectiveStartDate=position.effectiveStartDate,
-    effectiveEndDate=position.effectiveEndDate,
-    fillFromRight=False
-  )
-)
-```
+# SAP Commissions
+
+A Python wrapper for the SAP Commissions API.
+
+- [SAP Commissions](#sap-commissions)
+  - [Installation](#installation)
+    - [REST API](#rest-api)
+    - [Terminology](#terminology)
+  - [Usage](#usage)
+  - [Methods](#methods)
+    - [List](#list)
+    - [Get](#get)
+    - [Get ID](#get-id)
+    - [Get Versions](#get-versions)
+    - [Create](#create)
+    - [Create Versions](#create-versions)
+    - [Update](#update)
+    - [Update Versions](#update-versions)
+    - [Delete](#delete)
+    - [Delete Versions](#delete-versions)
+
+## Installation
+
+To install the project, run the following command:
+
+```text
+pip install python-sapcommissions
+```
+
+### REST API
+
+This project mimics the usage of the SAP Commissions REST API. Visit
+`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification,
+replacing `CALD` with your tenant name, and `ENV` with your environment name.
+
+### Terminology
+
+In this documentation, we talk about endpoints and resources, here is what that means.
+
+| Keyword  | Description                                                                      |
+| -------- | -------------------------------------------------------------------------------- |
+| Endpoint | A type of object that we can interact with, like `Participants` and `Positions`. |
+| Method   | An action to perform on an endpoint. See [Methods](#methods) below.              |
+| Resource | An instance of an endpoint, a single `Participant` or `Position` for example.    |
+
+## Usage
+
+To get started, import `Connection` and an endpoint of your choosing. In this
+example, we'll use `Participants` as the endpoint.
+
+```py
+from sapcommissions import Connection
+from sapcommissions.endpoints import Participants
+```
+
+Initialize a Connection by providing the tenant, environment, username,
+and password. Optionally, you can disable ssl verification, if you have problems
+connecting to the API from your corporate network.
+
+```python
+prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=False)
+```
+
+We'll use the `Participants` endpoint to get a list of all participants in the environment.
+
+```py
+all_users = Participants(prod).list()
+```
+
+## Methods
+
+Every endpoint exposes a number of methods. The most common are `list()` and `get()`.
+Some endpoints also expose `create()`, `update()`, and `delete()` methods. Versioned
+endpoints like `Participants` also expose `get_versions()`, `create_versions()`, `update_versions()`
+and `delete_versions()` methods.
+
+### List
+
+The `list()` method is used to retrieve multiple resources from the endpoint. By default, it returns
+the current effective version of the resource (if the endpoint is versioned). To retrieve a
+different effective version, you must provide both `startDate` and `endDate` parameters.
+
+In most cases, you will want to apply some kind of filter. For a complete list of available filter
+options please visit the [REST API Documentation](#rest-api).
+
+You can limit the number of results returned by providing a `limit`, this is usefull if you want to
+explore the data if the endpoint holds a lot of instances. Provide the `raw = True` parameter to
+return the json response from the API without converting it to a Python object.
+
+Provide `filter_kwargs` keyword arguments to apply a quick filter. For example
+`Positions(prod).list(name='John Doe')` is equivalent to
+`Positions(prod).list(filter="name eq 'John Doe'")`. Providing `filter` and `filter_kwargs` will
+combine the arguments using the `and` operator, as will multiple `filter_kwargs` arguments.
+
+```py
+# Get a list of all positions in the environment.
+positions = Positions(prod).list()
+
+# Get a list of all positions with title 'Sales Manager'.
+sales_managers = Positions(prod).list(filter="title/name eq 'Sales Manager'")
+```
+
+| Argument      | Type   | Required                   | Description                                      |
+| ------------- | ------ | -------------------------- | ------------------------------------------------ |
+| filter        | `str`  | False                      | A filter string to apply to the list             |
+| startDate     | `date` | False if endDate is None   | Filter list of resources effective for startDate |
+| endDate       | `date` | False if startDate is None | Filter list of resources effective for endDate   |
+| limit         | `int`  | False                      | Limit the number of returned resources           |
+| raw           | `bool` | False                      | Return the raw json response from the API        |
+| filter_kwargs | `dict` | False                      | Keyword arguments to apply to the filter         |
+
+| Returns          | Description                               |
+| ---------------- | ----------------------------------------- |
+| `list[Resource]` | A list of resources, single valid version |
+
+### Get
+
+The `get()` method is used to retrieve an existing resource, single (latest) version.
+The method takes a single parameter, `seq` (system unique identifier) of the object to
+retrieve. The `seq` value for a resource is stored in the first attribute, for
+simplicity, it can also be read from the `_seq` property.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns    | Description                              |
+| ---------- | ---------------------------------------- |
+| `Resource` | Requested resource, single valid version |
+
+```py
+# Let's say we retrieve a list of positions from the API. The manager attribute refers to a
+# position, but does not contain any meaningfull information about the manager yet.
+# We can use the `get()` method to enrich the manager data.
+positions = Positions(prod).list()
+
+for position in positions:
+  if position.manager:
+    position.manager = Positions(prod).get(position.manager._seq)
+```
+
+### Get ID
+
+`get_id()` is a helper method to simplify the retrieval of a resource by its ID (user
+unique identifier). The method takes a single parameter, `id`. If the resource does not provide an
+id, or the specified `id` could not be found, it returns `None`.
+
+| Argument | Type  | Required | Description                                 |
+| -------- | ----- | -------- | ------------------------------------------- |
+| id       | `str` | True     | The user unique identifier for the resource |
+
+| Returns    | Description                                        |
+| ---------- | -------------------------------------------------- |
+| `Resource` | Requested resource, single valid version           |
+| `None`     | Resource does not have an id or could not be found |
+
+```py
+position = Positions(prod).get_id('John Doe')
+
+# What would have been required without this method.
+position_id_attr = Position._id_attr  # returns 'name'
+positions = Positions(prod).list(filter=f"{position_id_attr} eq 'John Doe'")
+position = positions[0] if positions else None
+```
+
+### Get Versions
+
+The `get_versions()` method is simmilar to the [Get](#get) method, it returns a list
+of all versions of the resource.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns          | Description                             |
+| ---------------- | --------------------------------------- |
+| `list[Resource]` | A list of all versions for a  resources |
+
+```py
+# Get all versions for a position.
+positions = Positions(prod).list()
+position = positions[0]
+
+position_versions = Positions(prod).get_versions(first_position._seq)
+```
+
+### Create
+
+With the `create()` method, you can create a new instance of the resource. Unlike the
+REST API, the `create()` method accepts only a single resource as a parameter.
+If successful, the created resource will be returned.
+
+| Argument | Type       | Required | Description                     |
+| -------- | ---------- | -------- | ------------------------------- |
+| instance | `Resource` | True     | The resource instance to create |
+
+| Returns    | Description             |
+| ---------- | ----------------------- |
+| `Resource` | Created resource object |
+
+Make sure to provide all required attributes for the resource. Check the documentation
+for the resource to see which attributes are required.
+
+```py
+# Create a new position, with title 'Account Manager'.
+new_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Account Manager"),
+)
+created_position = Positions(prod).create(new_position)
+```
+
+### Create Versions
+
+The `create_versions()` method is used to create new versions of an existing resource.
+It is imperative that you provide all versions of the resource, as this method will
+overwrite all pre-existing versions with the ones provide. This method can also be used
+to end-date an existing resource. All pre-existing versions of the resource will be
+overwritten.
+
+| Argument  | Type             | Required | Description                                   |
+| --------- | ---------------- | -------- | --------------------------------------------- |
+| seq       | `int`            | True     | The system unique identifier for the resource |
+| instances | `list[Resource]` | True     | The list of resource instances to create      |
+
+| Returns          | Description                       |
+| ---------------- | --------------------------------- |
+| `list[Resource]` | List of created resource versions |
+
+```py
+# Let's create a new version of the position that we just created.
+first_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2020, 1, 1),
+  effectiveEndDate=date(2020, 12, 31),
+  title=Title(name="Account Manager"),
+)
+second_version = Position(
+  name="John Doe",
+  effectiveStartDate=date(2021, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Sales Manager"),
+)
+versions = [first_version, second_version]
+
+created_versions = Positions(prod).create_versions(created_position._seq, versions)
+```
+
+### Update
+
+With the `update()` method, you can update an existing resource. If the endpoint is
+versioned, this methid only updates a single valid version, matching the effective date
+range provided.
+
+| Argument | Type       | Required | Description                   |
+| -------- | ---------- | -------- | ----------------------------- |
+| update   | `Resource` | True     | The updated resource instance |
+
+| Returns    | Description                                   |
+| ---------- | --------------------------------------------- |
+| `Resource` | Updated resource object, single valid version |
+
+```py
+#  Say that you want to assign all positions with title 'Account Manager' or 'Sales Manager'
+# to a position group 'Sales'. We'll assume that the position group already exists.
+
+# Get a list of all positions with title 'Account Manager' or 'Sales Manager'.
+positions = (
+  Positions(prod)
+  .list(filter="title/name eq 'Account Manager' or title/name eq 'Sales Manager'")
+)
+
+# Now update the position group and update the position.
+for position in positions
+  position.positionGroup = PositionGroup(name="Sales")
+  Positions(prod).update(position)
+```
+
+### Update Versions
+
+The `update_versions()` method is used to update the versions of an existing resource.
+It is important to understand the differance between `update()` and `update_versions()`.
+[Update](#update) allows a single valid version of the resource to be updated, it must
+pre-exist in the environment. With `update_versions()`, you can update multiple versions
+at once, and even apply an update without any prior knowledge of pre-existing versions.
+The provided versions will be applied to the current existing versions in the
+environment.
+
+| Argument | Type             | Required | Description                                   |
+| -------- | ---------------- | -------- | --------------------------------------------- |
+| seq      | `int`            | True     | The system unique identifier for the resource |
+| versions | `list[Resource]` | True     | The list of resource version update to apply  |
+
+| Returns          | Description                                                |
+| ---------------- | ---------------------------------------------------------- |
+| `list[Resource]` | List of all resource versions after the update was applied |
+
+**Example:**
+
+```py
+# Let's revisit our previous example where a position is promoted to a different title. Our position
+# already has two versions, the first with a title of 'Account Manager', the second with a title of
+# 'Sales Manager' and position group 'Sales'. We can update the position without any pre-existing
+# knowledge of these versions.
+
+# We'll need to seq number for the position that we are going to update.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+# Now we can update the position
+updated_position = Position(
+  name="John Doe",
+  effectiveStartDate=date(2022, 1, 1),
+  effectiveEndDate=date(2200, 1, 1),
+  title=Title(name="Director"),
+  positionGroup=PositionGroup(name="Management"),
+)
+
+Positions(prod).update_versions(position_seq, [updated_position])
+
+# [
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2020, 1, 1),
+#     effectiveEndDate=date(2020, 12, 31)
+#     title=Title(name="Account Manager"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2021, 1, 1),
+#     effectiveEndDate=date(2021, 12, 31)
+#     title=Title(name="Sales Manager"),
+#     positionGroup=PositionGroup(name="Sales"),
+#   ),
+#   Position(
+#     name="John Doe",
+#     effectiveStartDate=date(2022, 1, 1),
+#     effectiveEndDate=date(2200, 1, 1)
+#     title=Title(name="Director"),
+#     positionGroup=PositionGroup(name="Management"),
+#   ),
+# ]
+```
+
+### Delete
+
+With the `delete()` method, you can fully delete a resource from the environment, all
+effective versions of the resource will be deleted.
+
+| Argument | Type  | Required | Description                                   |
+| -------- | ----- | -------- | --------------------------------------------- |
+| seq      | `int` | True     | The system unique identifier for the resource |
+
+| Returns | Description                                                |
+| ------- | ---------------------------------------------------------- |
+| `str`   | Confirmation message `The record is successfully deleted.` |
+
+```py
+# Delete a position with the name 'John Doe'.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = Positions(prod).delete(position._seq)
+assert message == "The record is successfully deleted."
+```
+
+### Delete Versions
+
+The `delete_versions()` method deletes the given versions of the resource. The resulting
+gap will either be filled from the previous or next available version of the resource.
+The effective dates provided must match an existing version of the resource.
+
+| Argument           | Type   | Required | Description                                          |
+| ------------------ | ------ | -------- | ---------------------------------------------------- |
+| seq                | `int`  | True     | The system unique identifier for the resource        |
+| effectiveStartDate | `date` | True     | The start date of the version to delete              |
+| effectiveEndDate   | `date` | True     | The end date of the version to delete                |
+| fillFromRight      | `bool` | False    | Default `True`, fill from the next available version |
+
+| Returns | Description                                                                  |
+| ------- | ---------------------------------------------------------------------------- |
+| `str`   | Confirmation message `All versions in given range are deleted successfully.` |
+
+```py
+# Remove the latest version of a position with the name 'John Doe' and fill the gap from the
+# previous version.
+positions = Positions(prod).list(filter="name eq 'John Doe'")
+position = positions[0]
+
+message = (
+  Positions(prod)
+  .delete_versions(
+    seq=position._seq,
+    effectiveStartDate=position.effectiveStartDate,
+    effectiveEndDate=position.effectiveEndDate,
+    fillFromRight=False
+  )
+)
+```
```

### Comparing `python-sapcommissions-1.0.0/sapcommissions/__init__.py` & `python-sapcommissions-1.0.1/sapcommissions/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""
-A Python wrapper for the SAP Commissions API.
-"""
-from dataclasses import dataclass, field
-
-
-@dataclass(frozen=True)
-class Connection:
-    """
-    Connection variables used to connect with SAP Commissions.
-    """
-
-    tenant: str = field(repr=True)
-    environment: str = field(repr=True)
-    username: str = field(repr=True)
-    password: str = field(repr=False)
-    verify_ssl: bool = field(default=True, repr=False)
-
-    @property
-    def url(self) -> str:
-        """Return the Commissions URL."""
-        return f"https://{self.tenant}-{self.environment}.callidusondemand.com"
-
-    @property
-    def api_url(self) -> str:
-        """Returns the base url for the Commissions REST API."""
-        return self.url + "/api"
-
-    @property
-    def api_document(self) -> str:
-        """Returns the url for the Commissions API documentation."""
-        return self.url + "/APIDocument"
+"""
+A Python wrapper for the SAP Commissions API.
+"""
+from dataclasses import dataclass, field
+
+
+@dataclass(frozen=True)
+class Connection:
+    """
+    Connection variables used to connect with SAP Commissions.
+    """
+
+    tenant: str = field(repr=True)
+    environment: str = field(repr=True)
+    username: str = field(repr=True)
+    password: str = field(repr=False)
+    verify_ssl: bool = field(default=True, repr=False)
+
+    @property
+    def url(self) -> str:
+        """Return the Commissions URL."""
+        return f"https://{self.tenant}-{self.environment}.callidusondemand.com"
+
+    @property
+    def api_url(self) -> str:
+        """Returns the base url for the Commissions REST API."""
+        return self.url + "/api"
+
+    @property
+    def api_document(self) -> str:
+        """Returns the url for the Commissions API documentation."""
+        return self.url + "/APIDocument"
```

### Comparing `python-sapcommissions-1.0.0/sapcommissions/endpoints.py` & `python-sapcommissions-1.0.1/sapcommissions/endpoints.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,931 +1,931 @@
-import logging
-from datetime import date
-from typing import Any
-
-from requests.auth import HTTPBasicAuth
-from requests.exceptions import HTTPError
-from requests.models import Response
-from requests.sessions import Session
-from urllib3 import disable_warnings
-
-from sapcommissions import Connection, resources
-from sapcommissions.exceptions import AuthenticationError, ClientError, ServerError
-
-LOGGER = logging.getLogger(__name__)
-
-
-class _Client(Session):
-    """Interacts with SAP Commissions REST API. Extends requests.Session."""
-
-    def __init__(
-        self,
-        base_url: str,
-        username: str,
-        password: str,
-        verify_ssl: bool = True,
-    ) -> None:
-        """Initialize an endpoint to interact with SAP Commissions."""
-        super().__init__()
-        self.base_url: str = base_url
-        self.auth = HTTPBasicAuth(username, password)
-        if verify_ssl is False:
-            disable_warnings()
-            self.verify = verify_ssl
-
-    def request(
-        self,
-        method: str,
-        uri: str,
-        parameters: dict[str, str] | None = None,
-        body: list[dict[str, str]] | None = None,
-    ) -> dict[str, Any | list[dict[str, Any]]] | Response:
-        """Perform an HTTP request to the SAP Commissions REST API."""
-        LOGGER.debug("%s %s %s", method.upper(), uri, parameters)
-        url: str = self.base_url + uri
-        with super().request(
-            method=method,
-            url=url,
-            params=parameters,
-            json=body,
-        ) as response:
-            try:
-                response.raise_for_status()
-                if "application/json" not in response.headers.get("content-type", ""):
-                    raise ValueError("Response content-type is not application/json.")
-                return response.json()
-            except HTTPError as error:
-                LOGGER.error(
-                    "%s %s %s %s",
-                    method.upper(),
-                    response.status_code,
-                    uri,
-                    response.text,
-                )
-                if 401 <= response.status_code <= 403:
-                    raise AuthenticationError(response.text) from error
-                elif 400 <= response.status_code < 500:
-                    raise ClientError(response.text) from error
-                elif 500 <= response.status_code < 600:
-                    raise ServerError(response.text) from error
-
-    def get(
-        self,
-        uri: str,
-        parameters: dict[str, str] | None = None,
-    ) -> dict[str, Any | list[dict[str, Any]]]:
-        """Perform a GET request to the SAP Commissions REST API."""
-        return self.request("GET", uri, parameters=parameters)
-
-    def delete(
-        self, uri: str, parameters: dict[str, str] | None = None
-    ) -> dict[str, Any | list[dict[str, Any]]]:
-        """Perform a DELETE request to the SAP Commissions REST API."""
-        return self.request("DELETE", uri, parameters=parameters)
-
-    def post(
-        self, uri: str, body: list[dict[str, str]]
-    ) -> dict[str, Any | list[dict[str, Any]]]:
-        """Perform a POST request to the SAP Commissions REST API."""
-        return self.request("POST", uri, body=body)
-
-    def put(
-        self, uri: str, body: list[dict[str, str]]
-    ) -> dict[str, Any | list[dict[str, Any]]]:
-        """Perform a PUT request to the SAP Commissions REST API."""
-        return self.request("PUT", uri, body=body)
-
-
-class _Endpoint:
-    """Provides a base template for an endpoint method."""
-
-    resource: resources._Resource
-
-    def __init__(self, connection: Connection) -> None:
-        """Initialize a base template for an endpoint method."""
-        self._client = _Client(
-            base_url=connection.api_url,
-            username=connection.username,
-            password=connection.password,
-            verify_ssl=connection.verify_ssl,
-        )
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.name})"
-
-    @property
-    def name(self) -> str:
-        return self.resource._name
-
-    @property
-    def url(self) -> str:
-        return f"/v2/{self.name}"
-
-
-class _Create(_Endpoint):
-    def create(self, instance: resources._Resource) -> resources._Resource:
-        """
-        Create a new resource for the endpoint.
-
-        Parameters
-        ----------
-        instances : resources._Resource
-            Resource to create.
-        """
-        LOGGER.info("Create %s", self.name)
-
-        assert isinstance(instance, self.resource)
-        json_data = instance.to_dict()
-
-        response = self._client.post(self.url, [json_data])
-        data = response[self.name]
-        created = self.resource.from_dict(data[0])
-
-        return created
-
-
-class _CreateVersions(_Endpoint):
-    def create_versions(
-        self, seq: int, versions: list[resources._Resource]
-    ) -> list[resources._Resource]:
-        """
-        Create versions of an existing resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier.
-        versions : list[resources._Resource]
-            List of resource versions to create.
-        """
-        LOGGER.info("Create versions for %s with seq %s", self.name, seq)
-
-        assert isinstance(seq, int)
-        assert isinstance(versions, list)
-        for version in versions:
-            assert isinstance(version, self.resource)
-        json_data = [version.to_dict() for version in versions]
-
-        response = self._client.post(self.url + f"({seq})/versions", json_data)
-        if response is not None:
-            data = response[self.name]
-            created_versions = [self.resource.from_dict(item) for item in data]
-        else:
-            created_versions = versions
-
-        return created_versions
-
-
-class _Delete(_Endpoint):
-    def delete(self, seq: int) -> str:
-        """
-        Delete an existing resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier to delete.
-        """
-        LOGGER.info("Delete %s with seq %s", self.name, seq)
-
-        assert isinstance(seq, int)
-
-        response = self._client.delete(f"{self.url}({seq})")
-        data = response[self.name]
-        message = data[str(seq)]
-
-        return message
-
-
-class _DeleteVersions(_Endpoint):
-    def delete_versions(
-        self,
-        seq: int,
-        effectiveStartDate: date,
-        effectiveEndDate: date,
-        fillFromRight: bool = False,
-    ) -> str:
-        """
-        Deletes the given version for an existing resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier.
-        effectiveStartDate : date
-            Resource effectiveStartDate.
-        effectiveEndDate : date
-            Resource effectiveEndDate.
-        fillFromRight : bool
-            If true, then the gap will be filled by the right (next) version,
-            otherwise by the left (prev) version. Default is false (prev).
-        """
-        LOGGER.info("Delete versions for %s with seq %s", self.name, seq)
-
-        query = dict()
-        assert isinstance(seq, int)
-        assert isinstance(effectiveStartDate, date)
-        query["effectiveStartDate"] = effectiveStartDate.strftime("%Y-%m-%d")
-        assert isinstance(effectiveEndDate, date)
-        query["effectiveEndDate"] = effectiveEndDate.strftime("%Y-%m-%d")
-        assert isinstance(fillFromRight, bool)
-        query["fillFromRight"] = fillFromRight
-
-        response = self._client.delete(self.url + f"({seq})/versions", query)
-        data = response[self.name]
-        message = data[0]
-
-        return message
-
-
-class _Get(_Endpoint):
-    def get(self, seq: int) -> resources._Resource:
-        """
-        Reads all of the attributes of an existing resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier.
-        """
-        LOGGER.info("Get %s with seq %s", self.name, seq)
-
-        assert isinstance(seq, int)
-
-        response = self._client.get(self.url + f"({seq})")
-        item = self.resource.from_dict(response)
-
-        return item
-
-
-class _GetVersions(_Endpoint):
-    def get_versions(
-        self,
-        seq: int,
-        startDate: date = None,
-        endDate: date = None,
-    ) -> list[resources._Resource]:
-        """
-        Returns all of the versions of a resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier.
-        startDate : date
-            Filter List for resources effective for startDate.
-        endDate : date
-            Filter List for resources effective for endDate.
-        """
-        LOGGER.info("Get versions of %s with seq %s", self.name, seq)
-
-        query = dict()
-        assert isinstance(seq, int)
-        if startDate:
-            assert isinstance(startDate, date)
-            query["startDate"] = startDate.strftime("%Y-%m-%d")
-        if endDate:
-            assert isinstance(endDate, date)
-            query["endDate"] = endDate.strftime("%Y-%m-%d")
-
-        response = self._client.get(self.url + f"({seq})/versions", query)
-        data = response[self.name]
-        resource_versions = [self.resource.from_dict(item) for item in data]
-
-        return resource_versions
-
-
-class _List(_Endpoint):
-    def list(
-        self,
-        filter: str = None,
-        startDate: date = None,
-        endDate: date = None,
-        limit: int = None,
-        raw: bool = False,
-        **filter_kwargs: dict,
-    ) -> list[resources._Resource]:
-        """
-        Returns a list of resources (single valid version).
-
-        Parameters
-        ----------
-        filter : str
-            Add filter conditions.
-        startDate : date
-            Filter List for resource effective for startDate.
-        endDate : date
-            Filter List for resource effective for endDate.
-        limit : int
-            Limit the number of resources returned.
-        raw : bool
-            If true, then the response is returned as is, otherwise it is converted
-            to resource objects. Default is False.
-        filter_kwargs : dict
-            Additional filter conditions, applied with the AND operator.
-
-        Examples
-        --------
-        p.list()
-            Returns all resources for today's effective date.
-        p.list(filter="name eq '*Smith*'")
-            Returns all resources with a name containing 'Smith'.
-        `p.list(name="*Smith*")`
-            Also returns all resources with a name containing 'Smith'.
-
-        The keyword arguments are converted to filters. The keyword must be a
-        part of the resource's attributes.
-        """
-        LOGGER.info("List %s", self.name)
-
-        query = {"top": limit if limit and limit < 100 else 100}
-        if expand := self.resource._expands:
-            query["expand"] = ",".join(expand)
-        if filter:
-            assert isinstance(filter, str)
-            query["$filter"] = filter
-        if startDate:
-            assert isinstance(startDate, date)
-            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
-            query["startDate"] = startDate.strftime("%Y/%m/%d")
-        if endDate:
-            assert isinstance(endDate, date)
-            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
-            query["endDate"] = endDate.strftime("%Y/%m/%d")
-
-        if filter_kwargs:
-            filters = " and ".join([f"{k} eq '{v}'" for k, v in filter_kwargs.items()])
-            if filter:
-                LOGGER.warning(
-                    "filter and filter_kwargs are both set,"
-                    " this could lead to unexpected results."
-                )
-                query["$filter"] = f"({filter}) and (filters)"
-            else:
-                query["$filter"] = filters
-
-        yield_count: int = 0
-        response = self._client.get(self.url, query)
-        data = response[self.name]
-        for item in data:
-            yield item if raw else self.resource.from_dict(item)
-            yield_count += 1
-            if limit is not None and yield_count >= limit:
-                return
-
-        while url := response.get("next"):
-            response = self._client.get(url)
-            data = response[self.name]
-            for item in data:
-                yield item if raw else self.resource.from_dict(item)
-                yield_count += 1
-                if limit and yield_count >= limit:
-                    return
-
-    def get_id(
-        self,
-        id: str,
-        raw: bool = False,
-    ) -> resources._Resource:
-        """
-        Reads all of the attributes of an existing resource.
-
-        Parameters
-        ----------
-        id : str
-            User unique identifier.
-        raw : bool
-            If true, then the response is returned as is, otherwise it is converted
-            to resource objects. Default is False.
-        """
-        LOGGER.info("Get %s with id %s", self.name, id)
-
-        assert isinstance(id, str)
-        id_attr = self.resource._id_attr
-        if id_attr is None:
-            LOGGER.warning("%s has no id attribute.", self.name)
-            return None
-
-        query = {"top": 10}
-        if expand := self.resource._expands:
-            query["expand"] = ",".join(expand)
-        query["$filter"] = f"{id_attr} eq '{id}'"
-
-        response = self._client.get(self.url, query)
-        data = response[self.name]
-        items = data if raw else [self.resource.from_dict(item) for item in data]
-        if len(data) > 1:
-            LOGGER.warning("Returned %s items for id %s.", len(data), id)
-        item = items[0] if items else None
-
-        return item
-
-    def count(
-        self,
-        filter: str = None,
-        startDate: date = None,
-        endDate: date = None,
-        **filter_kwargs: dict,
-    ) -> int:
-        """
-        Returns the number of resources.
-
-        Parameters
-        ----------
-        filter : str
-            Add filter conditions.
-        startDate : date
-            Filter List for resource effective for startDate.
-        endDate : date
-            Filter List for resource effective for endDate.
-        filter_kwargs : dict
-            Additional filter conditions, applied with the AND operator.
-
-        Examples
-        --------
-        p.count()
-            Returns the count of resources for today's effective date.
-        p.count(filter="name eq '*Smith*'")
-            Returns the count of resources with a name containing 'Smith'.
-        `p.count(name="*Smith*")`
-            Also returns the count of resources with a name containing 'Smith'.
-
-        The keyword arguments are converted to filters. The keyword must be a
-        part of the resource's attributes.
-        """
-        LOGGER.info("List %s", self.name)
-
-        query = {"top": 1, "inlineCount": True}
-        if filter:
-            assert isinstance(filter, str)
-            query["$filter"] = filter
-        if startDate:
-            assert isinstance(startDate, date)
-            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
-            query["startDate"] = startDate.strftime("%Y/%m/%d")
-        if endDate:
-            assert isinstance(endDate, date)
-            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
-            query["endDate"] = endDate.strftime("%Y/%m/%d")
-
-        if filter_kwargs:
-            filters = " and ".join([f"{k} eq '{v}'" for k, v in filter_kwargs.items()])
-            if filter:
-                LOGGER.warning(
-                    "filter and filter_kwargs are both set,"
-                    " this could lead to unexpected results."
-                )
-                query["$filter"] = f"({filter}) and (filters)"
-            else:
-                query["$filter"] = filters
-
-        response = self._client.get(self.url, query)
-        return response["total"]
-
-
-class _Update(_Endpoint):
-    def update(self, update: resources._Resource) -> resources._Resource:
-        """
-        Update an exiting resource.
-
-        Parameters
-        ----------
-        resource : resources._Resource
-            Resource to update.
-        """
-        LOGGER.info("Update %s", self.name)
-
-        assert isinstance(update, self.resource)
-        json_data = update.to_dict()
-
-        response = self._client.put(self.url, [json_data])
-        data = response[self.name]
-        updated = self.resource.from_dict(data[0])
-
-        return updated
-
-
-class _UpdateVersions(_Endpoint):
-    def update_versions(self, seq: int, versions: list[resources._Resource]) -> list:
-        """
-        Update versions of an existing resource.
-
-        Parameters
-        ----------
-        seq : int
-            Resource system identifier.
-        versions : list[resources._Resource]
-            List of resource versions with attributes for the endpoint.
-        """
-        LOGGER.info("Update versions for %s with seq %s", self.name, seq)
-
-        assert isinstance(seq, int)
-        assert isinstance(versions, list)
-        for version in versions:
-            assert isinstance(version, self.resource)
-        json_data = [item.to_dict() for item in versions]
-
-        response = self._client.put(self.url + f"({seq})/versions", json_data)
-        data = response[self.name]
-        updated_versions = [self.resource.from_dict(item) for item in data]
-
-        return updated_versions
-
-
-class AppliedDeposits(_Get, _List):
-    resource = resources.AppliedDeposit
-
-
-class AuditLogs(_Get, _List):
-    resource = resources.AuditLog
-
-
-class Balances(_Get, _List):
-    resource = resources.Balance
-
-
-class BusinessUnits(_Create, _Get, _List, _Update):
-    resource = resources.BusinessUnit
-
-
-class Calendars(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.Calendar
-
-
-class Categories(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Category
-
-
-class CategoryClassifiers(_Create, _Get, _List, _Update):
-    resource = resources.CategoryClassifier
-
-
-class CategoryTrees(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.CategoryTree
-
-
-class Commissions(_Get, _List):
-    resource = resources.Commission
-
-
-class Credits(_Create, _Get, _List, _Update):
-    resource = resources.Credit
-
-
-class CreditTypes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.CreditType
-
-
-class Customers(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Customer
-
-
-class Deposits(_Create, _Get, _List, _Update):
-    resource = resources.Deposit
-
-
-class EarningCodes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.EarningCode
-
-
-class EarningGroupCodes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.EarningGroupCode
-
-
-class EarningGroups(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.EarningGroup
-
-
-class EventTypes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.EventType
-
-
-class FixedValues(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.FixedValue
-
-
-class FixedValueTypes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.FixedValueType
-
-
-class FixedValueVariables(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.FixedValueVariable
-
-
-class Formulas(_Get, _List):
-    resource = resources.Formula
-
-
-class GenericClassifiers(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.GenericClassifier
-
-
-class GenericClassifierTypes(_Get, _List):
-    resource = resources.GenericClassifierType
-
-
-class GlobalFieldNames(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.GlobalFieldName
-
-
-class Groups(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.Group
-
-
-class Incentives(_Get, _List):
-    resource = resources.Incentive
-
-
-class LookUpTables(_Get, _List):
-    resource = resources.LookUpTable
-
-
-class LookUpTableVariables(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.LookUpTableVariable
-
-
-class Measurements(_Get, _List):
-    resource = resources.Measurement
-
-
-class MessageLogs(_Get, _List):
-    resource = resources.MessageLog
-
-
-class Messages(_Get, _List):
-    resource = resources.Message
-
-
-class Models(_Get, _List):
-    resource = resources.Model
-
-
-class Participants(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Participant
-
-
-class PaymentMappings(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.PaymentMapping
-
-
-class Payments(_Get, _List):
-    resource = resources.Payment
-
-
-class PaymentSummarys(_Get, _List):
-    resource = resources.PaymentSummary
-
-
-class Periods(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.Period
-
-
-class Pipelines(_Get, _List):
-    resource = resources.Pipeline
-
-
-class Plans(_Get, _List):
-    resource = resources.Plan
-
-
-class PositionGroups(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.PositionGroup
-
-
-class PositionRelations(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.PositionRelation
-
-
-class PositionRelationTypes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.PositionRelationType
-
-
-class Positions(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Position
-
-
-class PrimaryMeasurements(_Get, _List):
-    resource = resources.PrimaryMeasurement
-
-
-class ProcessingUnits(_Create, _Get, _List, _Update):
-    resource = resources.ProcessingUnit
-
-
-class Products(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Product
-
-
-class Quotas(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.Quota
-
-
-class RateTables(_Get, _List):
-    resource = resources.RateTable
-
-
-class RateTableVariables(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.RateTableVariable
-
-
-class Reasons(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.Reason
-
-
-class SalesOrders(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.SalesOrder
-
-
-class SalesTransactions(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.SalesTransaction
-
-
-class SecondaryMeasurements(_Get, _List):
-    resource = resources.SecondaryMeasurement
-
-
-class StatusCodes(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.StatusCode
-
-
-class Territories(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Territory
-
-
-class TerritoryVariables(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.TerritoryVariable
-
-
-class Titles(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Title
-
-
-class UnitTypes(_Get, _List):
-    resource = resources.UnitType
-
-
-class Users(_Create, _Delete, _Get, _List, _Update):
-    resource = resources.User
-
-
-class Variables(
-    _Create,
-    _CreateVersions,
-    _Delete,
-    _DeleteVersions,
-    _Get,
-    _GetVersions,
-    _List,
-    _Update,
-    _UpdateVersions,
-):
-    resource = resources.Variable
+import logging
+from datetime import date
+from typing import Any
+
+from requests.auth import HTTPBasicAuth
+from requests.exceptions import HTTPError
+from requests.models import Response
+from requests.sessions import Session
+from urllib3 import disable_warnings
+
+from sapcommissions import Connection, resources
+from sapcommissions.exceptions import AuthenticationError, ClientError, ServerError
+
+LOGGER = logging.getLogger(__name__)
+
+
+class _Client(Session):
+    """Interacts with SAP Commissions REST API. Extends requests.Session."""
+
+    def __init__(
+        self,
+        base_url: str,
+        username: str,
+        password: str,
+        verify_ssl: bool = True,
+    ) -> None:
+        """Initialize an endpoint to interact with SAP Commissions."""
+        super().__init__()
+        self.base_url: str = base_url
+        self.auth = HTTPBasicAuth(username, password)
+        if verify_ssl is False:
+            disable_warnings()
+            self.verify = verify_ssl
+
+    def request(
+        self,
+        method: str,
+        uri: str,
+        parameters: dict[str, str] | None = None,
+        body: list[dict[str, str]] | None = None,
+    ) -> dict[str, Any | list[dict[str, Any]]] | Response:
+        """Perform an HTTP request to the SAP Commissions REST API."""
+        LOGGER.debug("%s %s %s", method.upper(), uri, parameters)
+        url: str = self.base_url + uri
+        with super().request(
+            method=method,
+            url=url,
+            params=parameters,
+            json=body,
+        ) as response:
+            try:
+                response.raise_for_status()
+                if "application/json" not in response.headers.get("content-type", ""):
+                    raise ValueError("Response content-type is not application/json.")
+                return response.json()
+            except HTTPError as error:
+                LOGGER.error(
+                    "%s %s %s %s",
+                    method.upper(),
+                    response.status_code,
+                    uri,
+                    response.text,
+                )
+                if 401 <= response.status_code <= 403:
+                    raise AuthenticationError(response.text) from error
+                elif 400 <= response.status_code < 500:
+                    raise ClientError(response.text) from error
+                elif 500 <= response.status_code < 600:
+                    raise ServerError(response.text) from error
+
+    def get(
+        self,
+        uri: str,
+        parameters: dict[str, str] | None = None,
+    ) -> dict[str, Any | list[dict[str, Any]]]:
+        """Perform a GET request to the SAP Commissions REST API."""
+        return self.request("GET", uri, parameters=parameters)
+
+    def delete(
+        self, uri: str, parameters: dict[str, str] | None = None
+    ) -> dict[str, Any | list[dict[str, Any]]]:
+        """Perform a DELETE request to the SAP Commissions REST API."""
+        return self.request("DELETE", uri, parameters=parameters)
+
+    def post(
+        self, uri: str, body: list[dict[str, str]]
+    ) -> dict[str, Any | list[dict[str, Any]]]:
+        """Perform a POST request to the SAP Commissions REST API."""
+        return self.request("POST", uri, body=body)
+
+    def put(
+        self, uri: str, body: list[dict[str, str]]
+    ) -> dict[str, Any | list[dict[str, Any]]]:
+        """Perform a PUT request to the SAP Commissions REST API."""
+        return self.request("PUT", uri, body=body)
+
+
+class _Endpoint:
+    """Provides a base template for an endpoint method."""
+
+    resource: resources._Resource
+
+    def __init__(self, connection: Connection) -> None:
+        """Initialize a base template for an endpoint method."""
+        self._client = _Client(
+            base_url=connection.api_url,
+            username=connection.username,
+            password=connection.password,
+            verify_ssl=connection.verify_ssl,
+        )
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.name})"
+
+    @property
+    def name(self) -> str:
+        return self.resource._name
+
+    @property
+    def url(self) -> str:
+        return f"/v2/{self.name}"
+
+
+class _Create(_Endpoint):
+    def create(self, instance: resources._Resource) -> resources._Resource:
+        """
+        Create a new resource for the endpoint.
+
+        Parameters
+        ----------
+        instances : resources._Resource
+            Resource to create.
+        """
+        LOGGER.info("Create %s", self.name)
+
+        assert isinstance(instance, self.resource)
+        json_data = instance.to_dict()
+
+        response = self._client.post(self.url, [json_data])
+        data = response[self.name]
+        created = self.resource.from_dict(data[0])
+
+        return created
+
+
+class _CreateVersions(_Endpoint):
+    def create_versions(
+        self, seq: int, versions: list[resources._Resource]
+    ) -> list[resources._Resource]:
+        """
+        Create versions of an existing resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier.
+        versions : list[resources._Resource]
+            List of resource versions to create.
+        """
+        LOGGER.info("Create versions for %s with seq %s", self.name, seq)
+
+        assert isinstance(seq, int)
+        assert isinstance(versions, list)
+        for version in versions:
+            assert isinstance(version, self.resource)
+        json_data = [version.to_dict() for version in versions]
+
+        response = self._client.post(self.url + f"({seq})/versions", json_data)
+        if response is not None:
+            data = response[self.name]
+            created_versions = [self.resource.from_dict(item) for item in data]
+        else:
+            created_versions = versions
+
+        return created_versions
+
+
+class _Delete(_Endpoint):
+    def delete(self, seq: int) -> str:
+        """
+        Delete an existing resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier to delete.
+        """
+        LOGGER.info("Delete %s with seq %s", self.name, seq)
+
+        assert isinstance(seq, int)
+
+        response = self._client.delete(f"{self.url}({seq})")
+        data = response[self.name]
+        message = data[str(seq)]
+
+        return message
+
+
+class _DeleteVersions(_Endpoint):
+    def delete_versions(
+        self,
+        seq: int,
+        effectiveStartDate: date,
+        effectiveEndDate: date,
+        fillFromRight: bool = False,
+    ) -> str:
+        """
+        Deletes the given version for an existing resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier.
+        effectiveStartDate : date
+            Resource effectiveStartDate.
+        effectiveEndDate : date
+            Resource effectiveEndDate.
+        fillFromRight : bool
+            If true, then the gap will be filled by the right (next) version,
+            otherwise by the left (prev) version. Default is false (prev).
+        """
+        LOGGER.info("Delete versions for %s with seq %s", self.name, seq)
+
+        query = dict()
+        assert isinstance(seq, int)
+        assert isinstance(effectiveStartDate, date)
+        query["effectiveStartDate"] = effectiveStartDate.strftime("%Y-%m-%d")
+        assert isinstance(effectiveEndDate, date)
+        query["effectiveEndDate"] = effectiveEndDate.strftime("%Y-%m-%d")
+        assert isinstance(fillFromRight, bool)
+        query["fillFromRight"] = fillFromRight
+
+        response = self._client.delete(self.url + f"({seq})/versions", query)
+        data = response[self.name]
+        message = data[0]
+
+        return message
+
+
+class _Get(_Endpoint):
+    def get(self, seq: int) -> resources._Resource:
+        """
+        Reads all of the attributes of an existing resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier.
+        """
+        LOGGER.info("Get %s with seq %s", self.name, seq)
+
+        assert isinstance(seq, int)
+
+        response = self._client.get(self.url + f"({seq})")
+        item = self.resource.from_dict(response)
+
+        return item
+
+
+class _GetVersions(_Endpoint):
+    def get_versions(
+        self,
+        seq: int,
+        startDate: date = None,
+        endDate: date = None,
+    ) -> list[resources._Resource]:
+        """
+        Returns all of the versions of a resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier.
+        startDate : date
+            Filter List for resources effective for startDate.
+        endDate : date
+            Filter List for resources effective for endDate.
+        """
+        LOGGER.info("Get versions of %s with seq %s", self.name, seq)
+
+        query = dict()
+        assert isinstance(seq, int)
+        if startDate:
+            assert isinstance(startDate, date)
+            query["startDate"] = startDate.strftime("%Y-%m-%d")
+        if endDate:
+            assert isinstance(endDate, date)
+            query["endDate"] = endDate.strftime("%Y-%m-%d")
+
+        response = self._client.get(self.url + f"({seq})/versions", query)
+        data = response[self.name]
+        resource_versions = [self.resource.from_dict(item) for item in data]
+
+        return resource_versions
+
+
+class _List(_Endpoint):
+    def list(
+        self,
+        filter: str = None,
+        startDate: date = None,
+        endDate: date = None,
+        limit: int = None,
+        raw: bool = False,
+        **filter_kwargs: dict,
+    ) -> list[resources._Resource]:
+        """
+        Returns a list of resources (single valid version).
+
+        Parameters
+        ----------
+        filter : str
+            Add filter conditions.
+        startDate : date
+            Filter List for resource effective for startDate.
+        endDate : date
+            Filter List for resource effective for endDate.
+        limit : int
+            Limit the number of resources returned.
+        raw : bool
+            If true, then the response is returned as is, otherwise it is converted
+            to resource objects. Default is False.
+        filter_kwargs : dict
+            Additional filter conditions, applied with the AND operator.
+
+        Examples
+        --------
+        p.list()
+            Returns all resources for today's effective date.
+        p.list(filter="name eq '*Smith*'")
+            Returns all resources with a name containing 'Smith'.
+        `p.list(name="*Smith*")`
+            Also returns all resources with a name containing 'Smith'.
+
+        The keyword arguments are converted to filters. The keyword must be a
+        part of the resource's attributes.
+        """
+        LOGGER.info("List %s", self.name)
+
+        query = {"top": limit if limit and limit < 100 else 100}
+        if expand := self.resource._expands:
+            query["expand"] = ",".join(expand)
+        if filter:
+            assert isinstance(filter, str)
+            query["$filter"] = filter
+        if startDate:
+            assert isinstance(startDate, date)
+            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
+            query["startDate"] = startDate.strftime("%Y/%m/%d")
+        if endDate:
+            assert isinstance(endDate, date)
+            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
+            query["endDate"] = endDate.strftime("%Y/%m/%d")
+
+        if filter_kwargs:
+            filters = " and ".join([f"{k} eq '{v}'" for k, v in filter_kwargs.items()])
+            if filter:
+                LOGGER.warning(
+                    "filter and filter_kwargs are both set,"
+                    " this could lead to unexpected results."
+                )
+                query["$filter"] = f"({filter}) and (filters)"
+            else:
+                query["$filter"] = filters
+
+        yield_count: int = 0
+        response = self._client.get(self.url, query)
+        data = response[self.name]
+        for item in data:
+            yield item if raw else self.resource.from_dict(item)
+            yield_count += 1
+            if limit is not None and yield_count >= limit:
+                return
+
+        while url := response.get("next"):
+            response = self._client.get(url)
+            data = response[self.name]
+            for item in data:
+                yield item if raw else self.resource.from_dict(item)
+                yield_count += 1
+                if limit and yield_count >= limit:
+                    return
+
+    def get_id(
+        self,
+        id: str,
+        raw: bool = False,
+    ) -> resources._Resource:
+        """
+        Reads all of the attributes of an existing resource.
+
+        Parameters
+        ----------
+        id : str
+            User unique identifier.
+        raw : bool
+            If true, then the response is returned as is, otherwise it is converted
+            to resource objects. Default is False.
+        """
+        LOGGER.info("Get %s with id %s", self.name, id)
+
+        assert isinstance(id, str)
+        id_attr = self.resource._id_attr
+        if id_attr is None:
+            LOGGER.warning("%s has no id attribute.", self.name)
+            return None
+
+        query = {"top": 10}
+        if expand := self.resource._expands:
+            query["expand"] = ",".join(expand)
+        query["$filter"] = f"{id_attr} eq '{id}'"
+
+        response = self._client.get(self.url, query)
+        data = response[self.name]
+        items = data if raw else [self.resource.from_dict(item) for item in data]
+        if len(data) > 1:
+            LOGGER.warning("Returned %s items for id %s.", len(data), id)
+        item = items[0] if items else None
+
+        return item
+
+    def count(
+        self,
+        filter: str = None,
+        startDate: date = None,
+        endDate: date = None,
+        **filter_kwargs: dict,
+    ) -> int:
+        """
+        Returns the number of resources.
+
+        Parameters
+        ----------
+        filter : str
+            Add filter conditions.
+        startDate : date
+            Filter List for resource effective for startDate.
+        endDate : date
+            Filter List for resource effective for endDate.
+        filter_kwargs : dict
+            Additional filter conditions, applied with the AND operator.
+
+        Examples
+        --------
+        p.count()
+            Returns the count of resources for today's effective date.
+        p.count(filter="name eq '*Smith*'")
+            Returns the count of resources with a name containing 'Smith'.
+        `p.count(name="*Smith*")`
+            Also returns the count of resources with a name containing 'Smith'.
+
+        The keyword arguments are converted to filters. The keyword must be a
+        part of the resource's attributes.
+        """
+        LOGGER.info("List %s", self.name)
+
+        query = {"top": 1, "inlineCount": True}
+        if filter:
+            assert isinstance(filter, str)
+            query["$filter"] = filter
+        if startDate:
+            assert isinstance(startDate, date)
+            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
+            query["startDate"] = startDate.strftime("%Y/%m/%d")
+        if endDate:
+            assert isinstance(endDate, date)
+            # Unlike the other methods, this one requires a date in [YYYY/MM/DD]
+            query["endDate"] = endDate.strftime("%Y/%m/%d")
+
+        if filter_kwargs:
+            filters = " and ".join([f"{k} eq '{v}'" for k, v in filter_kwargs.items()])
+            if filter:
+                LOGGER.warning(
+                    "filter and filter_kwargs are both set,"
+                    " this could lead to unexpected results."
+                )
+                query["$filter"] = f"({filter}) and (filters)"
+            else:
+                query["$filter"] = filters
+
+        response = self._client.get(self.url, query)
+        return response["total"]
+
+
+class _Update(_Endpoint):
+    def update(self, update: resources._Resource) -> resources._Resource:
+        """
+        Update an exiting resource.
+
+        Parameters
+        ----------
+        resource : resources._Resource
+            Resource to update.
+        """
+        LOGGER.info("Update %s", self.name)
+
+        assert isinstance(update, self.resource)
+        json_data = update.to_dict()
+
+        response = self._client.put(self.url, [json_data])
+        data = response[self.name]
+        updated = self.resource.from_dict(data[0])
+
+        return updated
+
+
+class _UpdateVersions(_Endpoint):
+    def update_versions(self, seq: int, versions: list[resources._Resource]) -> list:
+        """
+        Update versions of an existing resource.
+
+        Parameters
+        ----------
+        seq : int
+            Resource system identifier.
+        versions : list[resources._Resource]
+            List of resource versions with attributes for the endpoint.
+        """
+        LOGGER.info("Update versions for %s with seq %s", self.name, seq)
+
+        assert isinstance(seq, int)
+        assert isinstance(versions, list)
+        for version in versions:
+            assert isinstance(version, self.resource)
+        json_data = [item.to_dict() for item in versions]
+
+        response = self._client.put(self.url + f"({seq})/versions", json_data)
+        data = response[self.name]
+        updated_versions = [self.resource.from_dict(item) for item in data]
+
+        return updated_versions
+
+
+class AppliedDeposits(_Get, _List):
+    resource = resources.AppliedDeposit
+
+
+class AuditLogs(_Get, _List):
+    resource = resources.AuditLog
+
+
+class Balances(_Get, _List):
+    resource = resources.Balance
+
+
+class BusinessUnits(_Create, _Get, _List, _Update):
+    resource = resources.BusinessUnit
+
+
+class Calendars(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.Calendar
+
+
+class Categories(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Category
+
+
+class CategoryClassifiers(_Create, _Get, _List, _Update):
+    resource = resources.CategoryClassifier
+
+
+class CategoryTrees(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.CategoryTree
+
+
+class Commissions(_Get, _List):
+    resource = resources.Commission
+
+
+class Credits(_Create, _Get, _List, _Update):
+    resource = resources.Credit
+
+
+class CreditTypes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.CreditType
+
+
+class Customers(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Customer
+
+
+class Deposits(_Create, _Get, _List, _Update):
+    resource = resources.Deposit
+
+
+class EarningCodes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.EarningCode
+
+
+class EarningGroupCodes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.EarningGroupCode
+
+
+class EarningGroups(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.EarningGroup
+
+
+class EventTypes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.EventType
+
+
+class FixedValues(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.FixedValue
+
+
+class FixedValueTypes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.FixedValueType
+
+
+class FixedValueVariables(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.FixedValueVariable
+
+
+class Formulas(_Get, _List):
+    resource = resources.Formula
+
+
+class GenericClassifiers(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.GenericClassifier
+
+
+class GenericClassifierTypes(_Get, _List):
+    resource = resources.GenericClassifierType
+
+
+class GlobalFieldNames(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.GlobalFieldName
+
+
+class Groups(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.Group
+
+
+class Incentives(_Get, _List):
+    resource = resources.Incentive
+
+
+class LookUpTables(_Get, _List):
+    resource = resources.LookUpTable
+
+
+class LookUpTableVariables(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.LookUpTableVariable
+
+
+class Measurements(_Get, _List):
+    resource = resources.Measurement
+
+
+class MessageLogs(_Get, _List):
+    resource = resources.MessageLog
+
+
+class Messages(_Get, _List):
+    resource = resources.Message
+
+
+class Models(_Get, _List):
+    resource = resources.Model
+
+
+class Participants(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Participant
+
+
+class PaymentMappings(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.PaymentMapping
+
+
+class Payments(_Get, _List):
+    resource = resources.Payment
+
+
+class PaymentSummarys(_Get, _List):
+    resource = resources.PaymentSummary
+
+
+class Periods(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.Period
+
+
+class Pipelines(_Get, _List):
+    resource = resources.Pipeline
+
+
+class Plans(_Get, _List):
+    resource = resources.Plan
+
+
+class PositionGroups(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.PositionGroup
+
+
+class PositionRelations(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.PositionRelation
+
+
+class PositionRelationTypes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.PositionRelationType
+
+
+class Positions(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Position
+
+
+class PrimaryMeasurements(_Get, _List):
+    resource = resources.PrimaryMeasurement
+
+
+class ProcessingUnits(_Create, _Get, _List, _Update):
+    resource = resources.ProcessingUnit
+
+
+class Products(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Product
+
+
+class Quotas(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.Quota
+
+
+class RateTables(_Get, _List):
+    resource = resources.RateTable
+
+
+class RateTableVariables(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.RateTableVariable
+
+
+class Reasons(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.Reason
+
+
+class SalesOrders(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.SalesOrder
+
+
+class SalesTransactions(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.SalesTransaction
+
+
+class SecondaryMeasurements(_Get, _List):
+    resource = resources.SecondaryMeasurement
+
+
+class StatusCodes(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.StatusCode
+
+
+class Territories(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Territory
+
+
+class TerritoryVariables(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.TerritoryVariable
+
+
+class Titles(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Title
+
+
+class UnitTypes(_Get, _List):
+    resource = resources.UnitType
+
+
+class Users(_Create, _Delete, _Get, _List, _Update):
+    resource = resources.User
+
+
+class Variables(
+    _Create,
+    _CreateVersions,
+    _Delete,
+    _DeleteVersions,
+    _Get,
+    _GetVersions,
+    _List,
+    _Update,
+    _UpdateVersions,
+):
+    resource = resources.Variable
```

### Comparing `python-sapcommissions-1.0.0/sapcommissions/resources.py` & `python-sapcommissions-1.0.1/sapcommissions/resources.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,2142 +1,2142 @@
-"""
-Create instances of SAP Commissions objects, like `Participant` and `Credit`.
-"""
-from __future__ import annotations
-
-import logging
-from dataclasses import dataclass, field, fields
-from datetime import date, datetime, timezone
-from types import UnionType
-from typing import ClassVar, get_args, get_origin, get_type_hints
-
-LOGGER = logging.getLogger(__name__)
-
-
-def _decode(value, astype):
-    if isinstance(value, list):
-        if astype is list:
-            LOGGER.error("Unknown type for list elements: %s", astype)
-            raise TypeError("Unknown type for list elements: %s", astype)
-        if get_origin(astype) is list:
-            if len(subtypes := get_args(astype)) > 1:
-                LOGGER.error("Impropper type for list elements: %s", subtypes)
-                raise TypeError("Impropper type for list elements: %s", subtypes)
-            return [_decode(v, subtypes[0]) for v in value]
-        LOGGER.error("Impropper type, value is list: %s", astype)
-        raise TypeError("Impropper type, value is list: %s", astype)
-    if isinstance(astype, UnionType):
-        LOGGER.error("UnionType is not supported: %s", astype)
-        raise NotImplementedError("Unsupported type: %s", astype)
-    if value is None:
-        return None
-    if astype is datetime:
-        return datetime.fromisoformat(value).astimezone(timezone.utc)
-    if astype is date:
-        return datetime.fromisoformat(value).astimezone(timezone.utc).date()
-    if isinstance(value, astype):
-        return value
-    if issubclass(astype, _Resource) and isinstance(value, dict):
-        return astype.from_dict(value)
-    if issubclass(astype, _Resource) and isinstance(value, (str, int)):
-        return astype(**{astype._seq_attr: value})
-    return astype(value)
-
-
-def _encode(value, fromtype):
-    if isinstance(value, list):
-        if fromtype is list:
-            LOGGER.error("Unknown type for list elements: %s", fromtype)
-            raise TypeError("Unknown type for list elements: %s", fromtype)
-        if get_origin(fromtype) is list:
-            if len(subtypes := get_args(fromtype)) > 1:
-                LOGGER.error("Impropper type for list elements: %s", subtypes)
-                raise TypeError("Impropper type for list elements: %s", subtypes)
-            return [_decode(v, subtypes[0]) for v in value]
-        LOGGER.error("Impropper type, value is list: %s", fromtype)
-        raise TypeError("Impropper type, value is list: %s", fromtype)
-    if isinstance(fromtype, UnionType):
-        LOGGER.error("UnionType is not supported: %s", fromtype)
-        raise NotImplementedError("Unsupported type: %s", fromtype)
-    if value is None:
-        return None
-    if isinstance(value, (datetime, date)):
-        return value.isoformat()
-    elif isinstance(value, _Resource):
-        return value.to_dict(ignore_seq=False)
-    if isinstance(value, int):
-        return value
-    return str(value)
-
-
-class _Resource:
-    _endpoint_name: ClassVar[str]
-
-    @classmethod
-    @property
-    def _name(cls) -> str:
-        """Returns the name resource."""
-        return cls._endpoint_name
-
-    @classmethod
-    @property
-    def _seq_attr(cls) -> str | None:
-        """Returns the name of the sequence attribute or None."""
-        for f in fields(cls):
-            if f.metadata.get("seq"):
-                return f.name
-
-    @property
-    def _seq(self) -> int | None:
-        """Returns the sequence or None."""
-        seq_attr = self._seq_attr
-        return self[seq_attr] if seq_attr else None
-
-    @classmethod
-    @property
-    def _id_attr(cls) -> str | None:
-        """Returns the name of the identifier attribute or None."""
-        for f in fields(cls):
-            if f.metadata.get("id"):
-                return f.name
-
-    @property
-    def _id(self) -> str | None:
-        """Returns the identifier or None."""
-        id_attr = self._id_attr
-        return self[id_attr] if id_attr else None
-
-    @classmethod
-    @property
-    def _expands(cls) -> tuple:
-        """Returns the name of the expandable attributes."""
-        return tuple(f.name for f in fields(cls) if f.metadata.get("expand"))
-
-    @classmethod
-    def from_dict(cls, json: dict) -> _Resource:
-        types = get_type_hints(cls)
-        invalid_json = {k: v for k, v in json.items() if k not in types.keys()}
-        for field_name in invalid_json.keys():
-            LOGGER.warning("%s is not a valid field for %s", field_name, cls.__name__)
-        valid_json = {k: v for k, v in json.items() if k in types.keys()}
-        for field_name, value in valid_json.items():
-            valid_json[field_name] = _decode(value, types[field_name])
-        return cls(**valid_json)
-
-    def to_dict(self, ignore_seq: bool = True) -> dict:
-        types = get_type_hints(self.__class__)
-        data = {}
-        for f in fields(self):
-            value = self[f.name]
-            if value is None:
-                continue
-            if f.metadata.get("json_ignore"):
-                continue
-            if ignore_seq and f.metadata.get("seq"):
-                continue
-            data[f.name] = _encode(value, types[f.name])
-        return data
-
-    def __getitem__(self, attribute: str):
-        return getattr(self, attribute)
-
-
-@dataclass(frozen=True)
-class Error:
-    message: str = field(default=None)
-    timeStamp: datetime = datetime.now()
-
-
-@dataclass
-class Address(_Resource):
-    _endpoint_name: ClassVar[str] = "address"
-    address1: str = field(default=None, repr=True)
-    address2: str = field(default=None, repr=False)
-    address3: str = field(default=None, repr=False)
-    postalCode: str = field(default=None, repr=False)
-    city: str = field(default=None, repr=False)
-    state: str = field(default=None, repr=False)
-    country: str = field(default=None, repr=False)
-    areaCode: str = field(default=None, repr=False)
-    geography: str = field(default=None, repr=False)
-    phone: str = field(default=None, repr=False)
-    fax: str = field(default=None, repr=False)
-    industry: str = field(default=None, repr=False)
-    contact: str = field(default=None, repr=False)
-    custId: str = field(default=None, repr=False)
-    company: str = field(default=None, repr=False)
-
-
-@dataclass
-class AppliedDeposit(_Resource):
-    _endpoint_name: ClassVar[str] = "appliedDeposits"
-    appliedDepositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
-    trialPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
-    postPipelineRunDate: datetime = field(default=None, repr=False)
-    entryNumber: int = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class AuditLog(_Resource):
-    _endpoint_name: ClassVar[str] = "auditLogs"
-    auditLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
-    objectSeq: str = field(default=None, repr=False)
-    eventDescription: str = field(default=None, repr=True)
-    objectName: str = field(default=None, repr=False)
-    eventType: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    userId: str = field(default=None, repr=False)
-    eventDate: date = field(default=None, repr=False)
-    objectType: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Balance(_Resource):
-    _endpoint_name: ClassVar[str] = "balances"
-    balanceSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
-    trialPipelineRunDate: datetime = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    applyPipelineRun: Pipeline = field(default=None, repr=False)
-    applyPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
-    postPipelineRunDate: datetime = field(default=None, repr=False)
-    balanceStatusId: str = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class BusinessUnit(_Resource):
-    _endpoint_name: ClassVar[str] = "businessUnits"
-    businessUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    mask: int = field(default=None, repr=False)
-    smask: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Calendar(_Resource):
-    _endpoint_name: ClassVar[str] = "calendars"
-    calendarSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    minorPeriodType: PeriodType = field(default=None, repr=False)
-    majorPeriodType: PeriodType = field(default=None, repr=False)
-    periods: Period = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Category(_Resource):
-    _endpoint_name: ClassVar[str] = "categories"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    owner: CategoryTree = field(default=None, repr=False)
-    parent: Category = field(default=None, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    returnType: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createDate: datetime = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class CategoryClassifier(_Resource):
-    _endpoint_name: ClassVar[str] = "categoryClassifiers"
-    categoryClassifiersSeq: int = field(
-        default=None, metadata={"seq": True}, repr=False
-    )
-    categoryTree: CategoryTree = field(default=None, repr=False)
-    category: Category = field(default=None, repr=False)
-    classifier: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class CategoryTree(_Resource):
-    _endpoint_name: ClassVar[str] = "categoryTrees"
-    categoryTreeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, repr=False)
-    classifierSelectorId: str = field(default=None, repr=False)
-    classifierClass: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    ruleExpression: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Commission(_Resource):
-    _endpoint_name: ClassVar[str] = "commissions"
-    commissionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    incentive: Incentive = field(default=None, repr=False)
-    credit: Credit = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    rateValue: Value = field(default=None, repr=False)
-    entryNumber: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    originTypeId: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Credit(_Resource):
-    _endpoint_name: ClassVar[str] = "credits"
-    creditSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    position: Position = field(default=None, repr=False)
-    salesOrder: SalesOrder = field(default=None, repr=False)
-    salesTransaction: SalesTransaction = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    creditType: CreditType = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    preadjustedValue: Value = field(default=None, repr=False)
-    originTypeId: str = field(default=None, repr=False)
-    reason: Reason = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    isRollable: bool = field(default=None, repr=False)
-    rollDate: date = field(default=None, repr=False)
-    isHeld: bool = field(default=None, repr=False)
-    releaseDate: date = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    compensationDate: date = field(default=None, repr=False)
-    comments: str = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class CreditType(_Resource):
-    _endpoint_name: ClassVar[str] = "creditTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    creditTypeId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Customer(_Resource):
-    _endpoint_name: ClassVar[str] = "customers"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
-    name: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    selectorId: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    address1: str = field(default=None, repr=False)
-    address2: str = field(default=None, repr=False)
-    address3: str = field(default=None, repr=False)
-    city: str = field(default=None, repr=False)
-    state: str = field(default=None, repr=False)
-    country: str = field(default=None, repr=False)
-    phone: str = field(default=None, repr=False)
-    areaCode: str = field(default=None, repr=False)
-    postalCode: str = field(default=None, repr=False)
-    geography: str = field(default=None, repr=False)
-    fax: str = field(default=None, repr=False)
-    email: str = field(default=None, repr=False)
-    industry: str = field(default=None, repr=False)
-    contact: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Deposit(_Resource):
-    _endpoint_name: ClassVar[str] = "deposits"
-    depositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    earningCodeId: str = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    position: Position = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    preadjustedValue: Value = field(default=None, repr=False)
-    originTypeId: str = field(default=None, repr=False)
-    reason: Reason = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    depositDate: date = field(default=None, repr=False)
-    isHeld: bool = field(default=None, repr=False)
-    releaseDate: date = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    comments: str = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class EarningCode(_Resource):
-    _endpoint_name: ClassVar[str] = "earningCodes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningCodeId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class EarningGroup(_Resource):
-    _endpoint_name: ClassVar[str] = "earningGroups"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningGroupId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class EarningGroupCode(_Resource):
-    _endpoint_name: ClassVar[str] = "earningGroupCodes"
-    earningGroupCodeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    earningGroupCode: str = field(default=None, metadata={"id": True}, repr=True)
-    earningCodeId: str = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class EventType(_Resource):
-    _endpoint_name: ClassVar[str] = "eventTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    eventTypeId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class FixedValue(_Resource):
-    _endpoint_name: ClassVar[str] = "fixedValues"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    calendar: Calendar = field(default=None, repr=False)
-    periodType: PeriodType = field(default=None, repr=False)
-    fixedValueType: FixedValueType = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    unitTypeSeq: UnitType = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    ruleElementSeq: str = field(default=None, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class FixedValueType(_Resource):
-    _endpoint_name: ClassVar[str] = "fixedValueTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    fixedValueTypeId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class FixedValueVariable(_Resource):
-    _endpoint_name: ClassVar[str] = "fixedValueVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    requiredPeriodType: PeriodType = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    defaultElement: FixedValue = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    referenceClassType: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Formula(_Resource):
-    _endpoint_name: ClassVar[str] = "formulas"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class GenericClassifier(_Resource):
-    _endpoint_name: ClassVar[str] = "genericClassifiers"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
-    name: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    selectorId: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class GenericClassifierType(_Resource):
-    _endpoint_name: ClassVar[str] = "genericClassifierTypes"
-    genericClassifierTypeSeq: int = field(
-        default=None, metadata={"seq": True}, repr=False
-    )
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class GlobalFieldName(_Resource):
-    _endpoint_name: ClassVar[str] = "globalFieldNames"
-    globalFieldNameSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    globalFieldNameDataTypeLength: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Group(_Resource):
-    _endpoint_name: ClassVar[str] = "groups"
-    groupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    policy: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Incentive(_Resource):
-    _endpoint_name: ClassVar[str] = "incentives"
-    incentiveSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, repr=False)
-    ruleElementOwnerSeq: str = field(default=None, repr=False)
-    isActive: bool = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    quota: Quota = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    releaseDate: datetime = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    attainment: str = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    position: Position = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class LookUpTable(_Resource):
-    _endpoint_name: ClassVar[str] = "relationalMDLTs"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    returnType: str = field(default=None, repr=False)
-    returnUnitType: UnitType = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    treatNullAsZero: bool = field(default=None, repr=False)
-    expressionTypeCounts: str = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    dimensions: LookUpTableDimension = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    indices: LookUpTableIndice = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class LookUpTableDimension(_Resource):
-    _endpoint_name: ClassVar[str] = "lookupTableDimension"
-    dimensionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    removeDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    displayOrder: int = field(default=None, repr=False)
-    dimensionType: int = field(default=None, repr=False)
-    dimensionSlot: int = field(default=None, repr=False)
-    dimensionUnitType: UnitType = field(default=None, repr=False)
-    isRanged: bool = field(default=None, repr=False)
-    includeStartInRange: bool = field(default=None, repr=False)
-    includeEndInRange: bool = field(default=None, repr=False)
-    flags: str = field(default=None, repr=False)
-    MDLT: LookUpTable = field(default=None, repr=False)
-    categoryTree: CategoryTree = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class LookUpTableIndice(_Resource):
-    _endpoint_name: ClassVar[str] = "lookuptableIndice"
-    ordinal: int = field(default=None, repr=False)
-    displayOrder: int = field(default=None, repr=False)
-    minString: str = field(default=None, repr=False)
-    maxString: str = field(default=None, repr=False)
-    minValue: str = field(default=None, repr=False)
-    maxValue: str = field(default=None, repr=False)
-    minDate: date = field(default=None, repr=False)
-    maxDate: date = field(default=None, repr=False)
-    validStart: date = field(default=None, repr=False)
-    validEnd: date = field(default=None, repr=False)
-    classifier: str = field(default=None, repr=False)  # TODO Implement Classifier
-    category: str = field(default=None, repr=False)  # TODO Implement Category
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    createDate: datetime = field(default=None, repr=False)
-    removeDate: datetime = field(default=None, repr=False)
-    MDLT: LookUpTable = field(default=None, repr=False)
-    dimensionSeq: LookUpTableDimension = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class LookUpTableVariable(_Resource):
-    _endpoint_name: ClassVar[str] = "lookUpTableVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    requiredPeriodType: PeriodType = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    defaultElement: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    referenceClassType: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Measurement(_Resource):
-    _endpoint_name: ClassVar[str] = "measurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PrimaryMeasurement(_Resource):
-    _endpoint_name: ClassVar[str] = "primaryMeasurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class SecondaryMeasurement(_Resource):
-    _endpoint_name: ClassVar[str] = "secondaryMeasurements"
-    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    numberOfCredits: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    isPrivate: bool = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Message(_Resource):
-    _endpoint_name: ClassVar[str] = "messages"
-    messageSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    messageKey: str = field(default=None, metadata={"id": True}, repr=True)
-    messageTimeStamp: datetime = field(default=None, repr=False)
-    argumentCount: int = field(default=None, repr=False)
-    subCategory: str = field(default=None, repr=False)
-    messageLog: MessageLog = field(default=None, repr=False)
-    module: str = field(default=None, repr=False)
-    rule: Rule = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    messageType: str = field(default=None, repr=False)
-    runPeriod: Period = field(default=None, repr=False)
-    objectSeq: str = field(default=None, repr=False)
-    salesTransaction: SalesTransaction = field(default=None, repr=False)
-    position: Position = field(default=None, repr=False)
-    category: str = field(default=None, repr=False)
-    credit: Credit = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class MessageLog(_Resource):
-    _endpoint_name: ClassVar[str] = "messageLogs"
-    messageLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    sourceSeq: str = field(default=None, repr=False)
-    componentName: str = field(default=None, repr=False)
-    logDate: datetime = field(default=None, repr=False)
-    logName: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Model(_Resource):
-    _endpoint_name: ClassVar[str] = "models"
-    modelSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    modelName: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    status: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    budgetType: str = field(default=None, repr=False)
-    budgetValue: Value = field(default=None, repr=False)
-    useSourcePeriodAsInput: str = field(default=None, repr=False)
-    sourceAdjustment: Value = field(default=None, repr=False)
-    sourceStartPeriod: Period = field(default=None, repr=False)
-    sourceEndPeriod: Period = field(default=None, repr=False)
-    modelStartPeriod: Period = field(default=None, repr=False)
-    modelEndPeriod: Period = field(default=None, repr=False)
-    modificationDate: datetime = field(default=None, repr=False)
-    budgetPercentValue: Value = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    useNewTransactionAsInput: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Participant(_Resource):
-    _endpoint_name: ClassVar[str] = "participants"
-    payeeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    payeeId: str = field(default=None, metadata={"id": True}, repr=True)
-    firstName: str = field(default=None, repr=False)
-    lastName: str = field(default=None, repr=False)
-    middleName: str = field(default=None, repr=False)
-    prefix: str = field(default=None, repr=False)
-    suffix: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    hireDate: date = field(default=None, repr=False)
-    terminationDate: date = field(default=None, repr=False)
-    salary: Value = field(default=None, repr=False)
-    userId: str = field(default=None, repr=False)
-    participantEmail: str = field(default=None, repr=False)
-    preferredLanguage: str = field(default=None, repr=False)
-    eventCalendar: str = field(default=None, repr=False)
-    taxId: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Payment(_Resource):
-    _endpoint_name: ClassVar[str] = "payments"
-    paymentSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    position: Position = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
-    trialPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
-    postPipelineRunDate: datetime = field(default=None, repr=False)
-    reason: str = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PaymentMapping(_Resource):
-    _endpoint_name: ClassVar[str] = "paymentMappings"
-    paymentMappingSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    sourceTableName: str = field(default=None, repr=False)
-    sourceAttribute: str = field(default=None, repr=False)
-    paymentAttribute: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PaymentSummary(_Resource):
-    _endpoint_name: ClassVar[str] = "paymentSummarys"
-    paymentSummarySeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    position: Position = field(default=None, repr=False)
-    participant: Participant = field(default=None, repr=False)
-    period: Period = field(default=None, repr=False)
-    earningGroupId: str = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    pipelineRunDate: datetime = field(default=None, repr=False)
-    appliedDeposit: Value = field(default=None, repr=False)
-    priorBalance: Value = field(default=None, repr=False)
-    balance: Value = field(default=None, repr=False)
-    payment: Value = field(default=None, repr=False)
-    Deposit: Value = field(default=None, repr=False)
-    outstandingBalance: Value = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Period(_Resource):
-    _endpoint_name: ClassVar[str] = "periods"
-    periodSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    shortName: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    periodType: PeriodType = field(default=None, repr=False)
-    parent: Period = field(default=None, repr=False)
-    startDate: date = field(default=None, repr=False)
-    endDate: date = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PeriodType(_Resource):
-    _endpoint_name: ClassVar[str] = "periodTypes"
-    periodTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    level: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Pipeline(_Resource):
-    _endpoint_name: ClassVar[str] = "pipelines"
-    pipelineRunSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    batchName: str = field(default=None, repr=False)
-    command: str = field(default=None, repr=False)
-    dateSubmitted: datetime = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    endDateScheduled: datetime = field(default=None, repr=False)
-    groupName: str = field(default=None, repr=False)
-    isolationLevel: str = field(default=None, repr=False)
-    message: str = field(default=None, repr=False)
-    modelRun: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    numErrors: int = field(default=None, repr=False)
-    numWarnings: int = field(default=None, repr=False)
-    period: str = field(default=None, repr=False)
-    priority: str = field(default=None, repr=False)
-    processingUnit: str = field(default=None, repr=False)
-    productVersion: str = field(default=None, repr=False)
-    removeDate: datetime = field(default=None, repr=False)
-    reportTypeName: str = field(default=None, repr=False)
-    runMode: str = field(default=None, repr=False)
-    runParameters: str = field(default=None, repr=False)
-    runProgress: str = field(default=None, repr=False)
-    scheduleDay: str = field(default=None, repr=False)
-    scheduleFrequency: str = field(default=None, repr=False)
-    schemaVersion: str = field(default=None, repr=False)
-    stageTables: list = field(default=None, metadata={"type": str}, repr=False)
-    stageType: str = field(default=None, repr=False)
-    startDateScheduled: datetime = field(default=None, repr=False)
-    startTime: datetime = field(default=None, repr=False)
-    state: str = field(default=None, repr=False)
-    status: str = field(default=None, repr=False)
-    stopTime: datetime = field(default=None, repr=False)
-    storedProcVersion: str = field(default=None, repr=False)
-    targetDatabase: str = field(default=None, repr=False)
-    traceLevel: str = field(default=None, repr=False)
-    userId: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Plan(_Resource):
-    _endpoint_name: ClassVar[str] = "plans"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    variableAssignments: VariableAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Position(_Resource):
-    _endpoint_name: ClassVar[str] = "positions"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
-    creditStartDate: date = field(default=None, repr=False)
-    creditEndDate: date = field(default=None, repr=False)
-    processingStartDate: date = field(default=None, repr=False)
-    processingEndDate: date = field(default=None, repr=False)
-    targetCompensation: Value = field(default=None, repr=False)
-    businessUnits: list[BusinessUnit] = field(default_factory=list, repr=False)
-    manager: Position = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    title: Title = field(default=None, repr=False)
-    positionGroup: PositionGroup = field(default=None, repr=False)
-    payee: Participant = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    plan: Plan = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    variableAssignments: list[VariableAssignment] = field(
-        default_factory=list, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PositionGroup(_Resource):
-    _endpoint_name: ClassVar[str] = "positionGroups"
-    positionGroupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PositionRelation(_Resource):
-    _endpoint_name: ClassVar[str] = "positionRelations"
-    positionRelationSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    parentPosition: Position = field(default=None, repr=False)
-    positionRelationType: PositionRelationType = field(default=None, repr=False)
-    childPosition: Position = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class PositionRelationType(_Resource):
-    _endpoint_name: ClassVar[str] = "positionRelationTypes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    relations: PositionRelation = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class ProcessingUnit(_Resource):
-    _endpoint_name: ClassVar[str] = "processingUnits"
-    processingUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Product(_Resource):
-    _endpoint_name: ClassVar[str] = "products"
-    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
-    name: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    selectorId: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    cost: Value = field(default=None, repr=False)
-    price: Value = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Quota(_Resource):
-    _endpoint_name: ClassVar[str] = "quotas"
-    quotaSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    unitType: UnitType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class RateTable(_Resource):
-    _endpoint_name: ClassVar[str] = "rateTables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class RateTableVariable(_Resource):
-    _endpoint_name: ClassVar[str] = "rateTableVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    requiredPeriodType: PeriodType = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    unitType: UnitType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    defaultElement: str = field(default=None, repr=False)
-    referenceClassType: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Reason(_Resource):
-    _endpoint_name: ClassVar[str] = "reasons"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    reasonId: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Rule(_Resource):
-    _endpoint_name: ClassVar[str] = "rules"
-    ruleSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    businessUnit: BusinessUnit = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    type: RuleType = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class RuleType(_Resource):
-    _endpoint_name: ClassVar[str] = "ruleType"
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    id: int = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class SalesOrder(_Resource):
-    _endpoint_name: ClassVar[str] = "salesOrders"
-    salesOrderSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    orderId: str = field(default=None, metadata={"id": True}, repr=True)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class SalesTransaction(_Resource):
-    _endpoint_name: ClassVar[str] = "salesTransactions"
-    salesTransactionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    salesOrder: SalesOrder = field(default=None, repr=False)
-    lineNumber: Value = field(default=None, repr=False)
-    subLineNumber: Value = field(default=None, repr=False)
-    value: Value = field(default=None, repr=False)
-    preadjustedValue: Value = field(default=None, repr=False)
-    isRunnable: bool = field(default=None, repr=False)
-    compensationDate: date = field(default=None, repr=False)
-    eventType: EventType = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modificationDate: datetime = field(default=None, repr=False)
-    reason: Reason = field(default=None, repr=False)
-    channel: str = field(default=None, repr=False)
-    poNumber: str = field(default=None, repr=False)
-    dataSource: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    shipToAddress: Address = field(default=None, repr=False)
-    otherToAddress: Address = field(default=None, repr=False)
-    billToAddress: Address = field(default=None, repr=False)
-    transactionAssignments: TransactionAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    discountType: str = field(default=None, repr=False)
-    productName: str = field(default=None, repr=False)
-    productDescription: str = field(default=None, repr=False)
-    paymentTerms: str = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    unitValue: Value = field(default=None, repr=False)
-    accountingDate: date = field(default=None, repr=False)
-    discountPercent: Value = field(default=None, repr=False)
-    comments: str = field(default=None, repr=False)
-    productId: str = field(default=None, repr=False)
-    numberOfUnits: Value = field(default=None, repr=False)
-    nativeCurrencyAmount: Value = field(default=None, repr=False)
-    nativeCurrency: str = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
-    alternateOrderNumber: str = field(default=None, repr=False)
-    originTypeId: str = field(default=None, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericAttribute17: str = field(default=None, repr=False)
-    genericAttribute18: str = field(default=None, repr=False)
-    genericAttribute19: str = field(default=None, repr=False)
-    genericAttribute20: str = field(default=None, repr=False)
-    genericAttribute21: str = field(default=None, repr=False)
-    genericAttribute22: str = field(default=None, repr=False)
-    genericAttribute23: str = field(default=None, repr=False)
-    genericAttribute24: str = field(default=None, repr=False)
-    genericAttribute25: str = field(default=None, repr=False)
-    genericAttribute26: str = field(default=None, repr=False)
-    genericAttribute27: str = field(default=None, repr=False)
-    genericAttribute28: str = field(default=None, repr=False)
-    genericAttribute29: str = field(default=None, repr=False)
-    genericAttribute30: str = field(default=None, repr=False)
-    genericAttribute31: str = field(default=None, repr=False)
-    genericAttribute32: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class StatusCode(_Resource):
-    _endpoint_name: ClassVar[str] = "statusCodes"
-    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    type: str = field(default=None, repr=False)
-    isActive: bool = field(default=None, repr=False)
-    status: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Territory(_Resource):
-    _endpoint_name: ClassVar[str] = "territories"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    definition: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    returnType: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class TerritoryVariable(_Resource):
-    _endpoint_name: ClassVar[str] = "territoryVariables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: BusinessUnit = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    defaultElement: str = field(default=None, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    referenceClassType: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    requiredPeriodType: PeriodType = field(default=None, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Title(_Resource):
-    _endpoint_name: ClassVar[str] = "titles"
-    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
-    plan: str = field(default=None, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    genericAttribute1: str = field(default=None, repr=False)
-    genericAttribute2: str = field(default=None, repr=False)
-    genericAttribute3: str = field(default=None, repr=False)
-    genericAttribute4: str = field(default=None, repr=False)
-    genericAttribute5: str = field(default=None, repr=False)
-    genericAttribute6: str = field(default=None, repr=False)
-    genericAttribute7: str = field(default=None, repr=False)
-    genericAttribute8: str = field(default=None, repr=False)
-    genericAttribute9: str = field(default=None, repr=False)
-    genericAttribute10: str = field(default=None, repr=False)
-    genericAttribute11: str = field(default=None, repr=False)
-    genericAttribute12: str = field(default=None, repr=False)
-    genericAttribute13: str = field(default=None, repr=False)
-    genericAttribute14: str = field(default=None, repr=False)
-    genericAttribute15: str = field(default=None, repr=False)
-    genericAttribute16: str = field(default=None, repr=False)
-    genericNumber1: Value = field(default=None, repr=False)
-    genericNumber2: Value = field(default=None, repr=False)
-    genericNumber3: Value = field(default=None, repr=False)
-    genericNumber4: Value = field(default=None, repr=False)
-    genericNumber5: Value = field(default=None, repr=False)
-    genericNumber6: Value = field(default=None, repr=False)
-    genericDate1: date = field(default=None, repr=False)
-    genericDate2: date = field(default=None, repr=False)
-    genericDate3: date = field(default=None, repr=False)
-    genericDate4: date = field(default=None, repr=False)
-    genericDate5: date = field(default=None, repr=False)
-    genericDate6: date = field(default=None, repr=False)
-    genericBoolean1: bool = field(default=None, repr=False)
-    genericBoolean2: bool = field(default=None, repr=False)
-    genericBoolean3: bool = field(default=None, repr=False)
-    genericBoolean4: bool = field(default=None, repr=False)
-    genericBoolean5: bool = field(default=None, repr=False)
-    genericBoolean6: bool = field(default=None, repr=False)
-    variableAssignments: VariableAssignment = field(
-        default=None, metadata={"expand": True}, repr=False
-    )
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class TransactionAssignment(_Resource):
-    _endpoint_name: ClassVar[str] = "transactionAssignment"
-    titleName: str = field(default=None, repr=False)
-    payeeId: str = field(default=None, repr=False)
-    positionName: str = field(default=None, repr=False)
-    salesOrder: SalesOrder = field(default=None, repr=False)
-    salesTransactionSeq: int = field(default=None, repr=False)
-    setNumber: int = field(default=None, repr=False)
-    compensationDate: date = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class UnitType(_Resource):
-    _endpoint_name: ClassVar[str] = "unitTypes"
-    unitTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    symbol: str = field(default=None, repr=False)
-    currencyLocale: str = field(default=None, repr=False)
-    formatting: str = field(default=None, repr=False)
-    positionOfSymbol: int = field(default=None, repr=False)
-    reportingScale: str = field(default=None, repr=False)
-    scale: int = field(default=None, repr=False)
-    valueClass: dict = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class User(_Resource):
-    _endpoint_name: ClassVar[str] = "users"
-    userSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    id: str = field(default=None, metadata={"id": True}, repr=True)
-    userName: str = field(default=None, repr=False)
-    description: str = field(default=None, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    readOnlyBusinessUnitList: BusinessUnit = field(default=None, repr=False)
-    fullAccessBusinessUnitList: BusinessUnit = field(default=None, repr=False)
-    groups: Group = field(default=None, repr=False)
-    email: str = field(default=None, repr=False)
-    preferredLanguage: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Value(_Resource):
-    _endpoint_name: ClassVar[str] = "value"
-    value: float = field(default=None, repr=False)
-    unitType: UnitType = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class Variable(_Resource):
-    _endpoint_name: ClassVar[str] = "variables"
-    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
-    name: str = field(default=None, metadata={"id": True}, repr=True)
-    description: str = field(default=None, repr=False)
-    calendar: Calendar = field(default=None, repr=False)
-    requiredPeriodType: PeriodType = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
-    plan: str = field(default=None, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
-    notAllowUpdate: bool = field(default=None, repr=False)
-    defaultElement: str = field(default=None, repr=False)
-    referenceClassType: str = field(default=None, repr=False)
-    returnType: str = field(default=None, repr=False)
-    owningElement: str = field(default=None, repr=False)
-    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-    inputSignature: str = field(default=None, repr=False)
-    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
-
-
-@dataclass
-class VariableAssignment(_Resource):
-    _endpoint_name: ClassVar[str] = "variableAssignment"
-    owner: str = field(default=None, repr=False)
-    variable: str = field(default=None, repr=False)
-    assignment: str = field(default=None, repr=False)
-    effectiveStartDate: date = field(default=None, repr=True)
-    effectiveEndDate: date = field(default=None, repr=False)
-    createDate: datetime = field(
-        default=None, metadata={"json_ignore": True}, repr=False
-    )
-    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+"""
+Create instances of SAP Commissions objects, like `Participant` and `Credit`.
+"""
+from __future__ import annotations
+
+import logging
+from dataclasses import dataclass, field, fields
+from datetime import date, datetime, timezone
+from types import UnionType
+from typing import ClassVar, get_args, get_origin, get_type_hints
+
+LOGGER = logging.getLogger(__name__)
+
+
+def _decode(value, astype):
+    if isinstance(value, list):
+        if astype is list:
+            LOGGER.error("Unknown type for list elements: %s", astype)
+            raise TypeError("Unknown type for list elements: %s", astype)
+        if get_origin(astype) is list:
+            if len(subtypes := get_args(astype)) > 1:
+                LOGGER.error("Impropper type for list elements: %s", subtypes)
+                raise TypeError("Impropper type for list elements: %s", subtypes)
+            return [_decode(v, subtypes[0]) for v in value]
+        LOGGER.error("Impropper type, value is list: %s", astype)
+        raise TypeError("Impropper type, value is list: %s", astype)
+    if isinstance(astype, UnionType):
+        LOGGER.error("UnionType is not supported: %s", astype)
+        raise NotImplementedError("Unsupported type: %s", astype)
+    if value is None:
+        return None
+    if astype is datetime:
+        return datetime.fromisoformat(value).astimezone(timezone.utc)
+    if astype is date:
+        return datetime.fromisoformat(value).astimezone(timezone.utc).date()
+    if isinstance(value, astype):
+        return value
+    if issubclass(astype, _Resource) and isinstance(value, dict):
+        return astype.from_dict(value)
+    if issubclass(astype, _Resource) and isinstance(value, (str, int)):
+        return astype(**{astype._seq_attr: value})
+    return astype(value)
+
+
+def _encode(value, fromtype):
+    if isinstance(value, list):
+        if fromtype is list:
+            LOGGER.error("Unknown type for list elements: %s", fromtype)
+            raise TypeError("Unknown type for list elements: %s", fromtype)
+        if get_origin(fromtype) is list:
+            if len(subtypes := get_args(fromtype)) > 1:
+                LOGGER.error("Impropper type for list elements: %s", subtypes)
+                raise TypeError("Impropper type for list elements: %s", subtypes)
+            return [_decode(v, subtypes[0]) for v in value]
+        LOGGER.error("Impropper type, value is list: %s", fromtype)
+        raise TypeError("Impropper type, value is list: %s", fromtype)
+    if isinstance(fromtype, UnionType):
+        LOGGER.error("UnionType is not supported: %s", fromtype)
+        raise NotImplementedError("Unsupported type: %s", fromtype)
+    if value is None:
+        return None
+    if isinstance(value, (datetime, date)):
+        return value.isoformat()
+    elif isinstance(value, _Resource):
+        return value.to_dict(ignore_seq=False)
+    if isinstance(value, int):
+        return value
+    return str(value)
+
+
+class _Resource:
+    _endpoint_name: ClassVar[str]
+
+    @classmethod
+    @property
+    def _name(cls) -> str:
+        """Returns the name resource."""
+        return cls._endpoint_name
+
+    @classmethod
+    @property
+    def _seq_attr(cls) -> str | None:
+        """Returns the name of the sequence attribute or None."""
+        for f in fields(cls):
+            if f.metadata.get("seq"):
+                return f.name
+
+    @property
+    def _seq(self) -> int | None:
+        """Returns the sequence or None."""
+        seq_attr = self._seq_attr
+        return self[seq_attr] if seq_attr else None
+
+    @classmethod
+    @property
+    def _id_attr(cls) -> str | None:
+        """Returns the name of the identifier attribute or None."""
+        for f in fields(cls):
+            if f.metadata.get("id"):
+                return f.name
+
+    @property
+    def _id(self) -> str | None:
+        """Returns the identifier or None."""
+        id_attr = self._id_attr
+        return self[id_attr] if id_attr else None
+
+    @classmethod
+    @property
+    def _expands(cls) -> tuple:
+        """Returns the name of the expandable attributes."""
+        return tuple(f.name for f in fields(cls) if f.metadata.get("expand"))
+
+    @classmethod
+    def from_dict(cls, json: dict) -> _Resource:
+        types = get_type_hints(cls)
+        invalid_json = {k: v for k, v in json.items() if k not in types.keys()}
+        for field_name in invalid_json.keys():
+            LOGGER.warning("%s is not a valid field for %s", field_name, cls.__name__)
+        valid_json = {k: v for k, v in json.items() if k in types.keys()}
+        for field_name, value in valid_json.items():
+            valid_json[field_name] = _decode(value, types[field_name])
+        return cls(**valid_json)
+
+    def to_dict(self, ignore_seq: bool = True) -> dict:
+        types = get_type_hints(self.__class__)
+        data = {}
+        for f in fields(self):
+            value = self[f.name]
+            if value is None:
+                continue
+            if f.metadata.get("json_ignore"):
+                continue
+            if ignore_seq and f.metadata.get("seq"):
+                continue
+            data[f.name] = _encode(value, types[f.name])
+        return data
+
+    def __getitem__(self, attribute: str):
+        return getattr(self, attribute)
+
+
+@dataclass(frozen=True)
+class Error:
+    message: str = field(default=None)
+    timeStamp: datetime = datetime.now()
+
+
+@dataclass
+class Address(_Resource):
+    _endpoint_name: ClassVar[str] = "address"
+    address1: str = field(default=None, repr=True)
+    address2: str = field(default=None, repr=False)
+    address3: str = field(default=None, repr=False)
+    postalCode: str = field(default=None, repr=False)
+    city: str = field(default=None, repr=False)
+    state: str = field(default=None, repr=False)
+    country: str = field(default=None, repr=False)
+    areaCode: str = field(default=None, repr=False)
+    geography: str = field(default=None, repr=False)
+    phone: str = field(default=None, repr=False)
+    fax: str = field(default=None, repr=False)
+    industry: str = field(default=None, repr=False)
+    contact: str = field(default=None, repr=False)
+    custId: str = field(default=None, repr=False)
+    company: str = field(default=None, repr=False)
+
+
+@dataclass
+class AppliedDeposit(_Resource):
+    _endpoint_name: ClassVar[str] = "appliedDeposits"
+    appliedDepositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    earningCodeId: str = field(default=None, repr=False)
+    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRunDate: datetime = field(default=None, repr=False)
+    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRunDate: datetime = field(default=None, repr=False)
+    entryNumber: int = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class AuditLog(_Resource):
+    _endpoint_name: ClassVar[str] = "auditLogs"
+    auditLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    businessUnit: BusinessUnit = field(default=None, repr=False)
+    objectSeq: str = field(default=None, repr=False)
+    eventDescription: str = field(default=None, repr=True)
+    objectName: str = field(default=None, repr=False)
+    eventType: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    userId: str = field(default=None, repr=False)
+    eventDate: date = field(default=None, repr=False)
+    objectType: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Balance(_Resource):
+    _endpoint_name: ClassVar[str] = "balances"
+    balanceSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    earningCodeId: str = field(default=None, repr=False)
+    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRunDate: datetime = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    applyPipelineRun: Pipeline = field(default=None, repr=False)
+    applyPipelineRunDate: datetime = field(default=None, repr=False)
+    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRunDate: datetime = field(default=None, repr=False)
+    balanceStatusId: str = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class BusinessUnit(_Resource):
+    _endpoint_name: ClassVar[str] = "businessUnits"
+    businessUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    mask: int = field(default=None, repr=False)
+    smask: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Calendar(_Resource):
+    _endpoint_name: ClassVar[str] = "calendars"
+    calendarSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    minorPeriodType: PeriodType = field(default=None, repr=False)
+    majorPeriodType: PeriodType = field(default=None, repr=False)
+    periods: Period = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Category(_Resource):
+    _endpoint_name: ClassVar[str] = "categories"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    owner: CategoryTree = field(default=None, repr=False)
+    parent: Category = field(default=None, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    returnType: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createDate: datetime = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class CategoryClassifier(_Resource):
+    _endpoint_name: ClassVar[str] = "categoryClassifiers"
+    categoryClassifiersSeq: int = field(
+        default=None, metadata={"seq": True}, repr=False
+    )
+    categoryTree: CategoryTree = field(default=None, repr=False)
+    category: Category = field(default=None, repr=False)
+    classifier: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class CategoryTree(_Resource):
+    _endpoint_name: ClassVar[str] = "categoryTrees"
+    categoryTreeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, repr=False)
+    classifierSelectorId: str = field(default=None, repr=False)
+    classifierClass: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleExpression: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Commission(_Resource):
+    _endpoint_name: ClassVar[str] = "commissions"
+    commissionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    incentive: Incentive = field(default=None, repr=False)
+    credit: Credit = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    rateValue: Value = field(default=None, repr=False)
+    entryNumber: str = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    originTypeId: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Credit(_Resource):
+    _endpoint_name: ClassVar[str] = "credits"
+    creditSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    position: Position = field(default=None, repr=False)
+    salesOrder: SalesOrder = field(default=None, repr=False)
+    salesTransaction: SalesTransaction = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    creditType: CreditType = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    preadjustedValue: Value = field(default=None, repr=False)
+    originTypeId: str = field(default=None, repr=False)
+    reason: Reason = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    isRollable: bool = field(default=None, repr=False)
+    rollDate: date = field(default=None, repr=False)
+    isHeld: bool = field(default=None, repr=False)
+    releaseDate: date = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    compensationDate: date = field(default=None, repr=False)
+    comments: str = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class CreditType(_Resource):
+    _endpoint_name: ClassVar[str] = "creditTypes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    creditTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Customer(_Resource):
+    _endpoint_name: ClassVar[str] = "customers"
+    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    name: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    selectorId: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    address1: str = field(default=None, repr=False)
+    address2: str = field(default=None, repr=False)
+    address3: str = field(default=None, repr=False)
+    city: str = field(default=None, repr=False)
+    state: str = field(default=None, repr=False)
+    country: str = field(default=None, repr=False)
+    phone: str = field(default=None, repr=False)
+    areaCode: str = field(default=None, repr=False)
+    postalCode: str = field(default=None, repr=False)
+    geography: str = field(default=None, repr=False)
+    fax: str = field(default=None, repr=False)
+    email: str = field(default=None, repr=False)
+    industry: str = field(default=None, repr=False)
+    contact: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Deposit(_Resource):
+    _endpoint_name: ClassVar[str] = "deposits"
+    depositSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    earningCodeId: str = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    position: Position = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    preadjustedValue: Value = field(default=None, repr=False)
+    originTypeId: str = field(default=None, repr=False)
+    reason: Reason = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    depositDate: date = field(default=None, repr=False)
+    isHeld: bool = field(default=None, repr=False)
+    releaseDate: date = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    comments: str = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class EarningCode(_Resource):
+    _endpoint_name: ClassVar[str] = "earningCodes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    earningCodeId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class EarningGroup(_Resource):
+    _endpoint_name: ClassVar[str] = "earningGroups"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    earningGroupId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class EarningGroupCode(_Resource):
+    _endpoint_name: ClassVar[str] = "earningGroupCodes"
+    earningGroupCodeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    earningGroupCode: str = field(default=None, metadata={"id": True}, repr=True)
+    earningCodeId: str = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class EventType(_Resource):
+    _endpoint_name: ClassVar[str] = "eventTypes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    eventTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class FixedValue(_Resource):
+    _endpoint_name: ClassVar[str] = "fixedValues"
+    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    calendar: Calendar = field(default=None, repr=False)
+    periodType: PeriodType = field(default=None, repr=False)
+    fixedValueType: FixedValueType = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    unitTypeSeq: UnitType = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    ruleElementSeq: str = field(default=None, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class FixedValueType(_Resource):
+    _endpoint_name: ClassVar[str] = "fixedValueTypes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    fixedValueTypeId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class FixedValueVariable(_Resource):
+    _endpoint_name: ClassVar[str] = "fixedValueVariables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    requiredPeriodType: PeriodType = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    defaultElement: FixedValue = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    referenceClassType: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Formula(_Resource):
+    _endpoint_name: ClassVar[str] = "formulas"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class GenericClassifier(_Resource):
+    _endpoint_name: ClassVar[str] = "genericClassifiers"
+    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    name: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    selectorId: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class GenericClassifierType(_Resource):
+    _endpoint_name: ClassVar[str] = "genericClassifierTypes"
+    genericClassifierTypeSeq: int = field(
+        default=None, metadata={"seq": True}, repr=False
+    )
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class GlobalFieldName(_Resource):
+    _endpoint_name: ClassVar[str] = "globalFieldNames"
+    globalFieldNameSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    globalFieldNameDataTypeLength: int = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Group(_Resource):
+    _endpoint_name: ClassVar[str] = "groups"
+    groupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    policy: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Incentive(_Resource):
+    _endpoint_name: ClassVar[str] = "incentives"
+    incentiveSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, repr=False)
+    ruleElementOwnerSeq: str = field(default=None, repr=False)
+    isActive: bool = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    quota: Quota = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    releaseDate: datetime = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    attainment: str = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    position: Position = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class LookUpTable(_Resource):
+    _endpoint_name: ClassVar[str] = "relationalMDLTs"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnit: BusinessUnit = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    returnType: str = field(default=None, repr=False)
+    returnUnitType: UnitType = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    treatNullAsZero: bool = field(default=None, repr=False)
+    expressionTypeCounts: str = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    dimensions: LookUpTableDimension = field(
+        default=None, metadata={"expand": True}, repr=False
+    )
+    indices: LookUpTableIndice = field(
+        default=None, metadata={"expand": True}, repr=False
+    )
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class LookUpTableDimension(_Resource):
+    _endpoint_name: ClassVar[str] = "lookupTableDimension"
+    dimensionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    removeDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    displayOrder: int = field(default=None, repr=False)
+    dimensionType: int = field(default=None, repr=False)
+    dimensionSlot: int = field(default=None, repr=False)
+    dimensionUnitType: UnitType = field(default=None, repr=False)
+    isRanged: bool = field(default=None, repr=False)
+    includeStartInRange: bool = field(default=None, repr=False)
+    includeEndInRange: bool = field(default=None, repr=False)
+    flags: str = field(default=None, repr=False)
+    MDLT: LookUpTable = field(default=None, repr=False)
+    categoryTree: CategoryTree = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class LookUpTableIndice(_Resource):
+    _endpoint_name: ClassVar[str] = "lookuptableIndice"
+    ordinal: int = field(default=None, repr=False)
+    displayOrder: int = field(default=None, repr=False)
+    minString: str = field(default=None, repr=False)
+    maxString: str = field(default=None, repr=False)
+    minValue: str = field(default=None, repr=False)
+    maxValue: str = field(default=None, repr=False)
+    minDate: date = field(default=None, repr=False)
+    maxDate: date = field(default=None, repr=False)
+    validStart: date = field(default=None, repr=False)
+    validEnd: date = field(default=None, repr=False)
+    classifier: str = field(default=None, repr=False)  # TODO Implement Classifier
+    category: str = field(default=None, repr=False)  # TODO Implement Category
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    createDate: datetime = field(default=None, repr=False)
+    removeDate: datetime = field(default=None, repr=False)
+    MDLT: LookUpTable = field(default=None, repr=False)
+    dimensionSeq: LookUpTableDimension = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class LookUpTableVariable(_Resource):
+    _endpoint_name: ClassVar[str] = "lookUpTableVariables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    requiredPeriodType: PeriodType = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    defaultElement: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    referenceClassType: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Measurement(_Resource):
+    _endpoint_name: ClassVar[str] = "measurements"
+    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    numberOfCredits: Value = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PrimaryMeasurement(_Resource):
+    _endpoint_name: ClassVar[str] = "primaryMeasurements"
+    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    numberOfCredits: Value = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class SecondaryMeasurement(_Resource):
+    _endpoint_name: ClassVar[str] = "secondaryMeasurements"
+    measurementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    numberOfCredits: Value = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    isPrivate: bool = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Message(_Resource):
+    _endpoint_name: ClassVar[str] = "messages"
+    messageSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    messageKey: str = field(default=None, metadata={"id": True}, repr=True)
+    messageTimeStamp: datetime = field(default=None, repr=False)
+    argumentCount: int = field(default=None, repr=False)
+    subCategory: str = field(default=None, repr=False)
+    messageLog: MessageLog = field(default=None, repr=False)
+    module: str = field(default=None, repr=False)
+    rule: Rule = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    messageType: str = field(default=None, repr=False)
+    runPeriod: Period = field(default=None, repr=False)
+    objectSeq: str = field(default=None, repr=False)
+    salesTransaction: SalesTransaction = field(default=None, repr=False)
+    position: Position = field(default=None, repr=False)
+    category: str = field(default=None, repr=False)
+    credit: Credit = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class MessageLog(_Resource):
+    _endpoint_name: ClassVar[str] = "messageLogs"
+    messageLogSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    sourceSeq: str = field(default=None, repr=False)
+    componentName: str = field(default=None, repr=False)
+    logDate: datetime = field(default=None, repr=False)
+    logName: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Model(_Resource):
+    _endpoint_name: ClassVar[str] = "models"
+    modelSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    modelName: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    status: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    budgetType: str = field(default=None, repr=False)
+    budgetValue: Value = field(default=None, repr=False)
+    useSourcePeriodAsInput: str = field(default=None, repr=False)
+    sourceAdjustment: Value = field(default=None, repr=False)
+    sourceStartPeriod: Period = field(default=None, repr=False)
+    sourceEndPeriod: Period = field(default=None, repr=False)
+    modelStartPeriod: Period = field(default=None, repr=False)
+    modelEndPeriod: Period = field(default=None, repr=False)
+    modificationDate: datetime = field(default=None, repr=False)
+    budgetPercentValue: Value = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    useNewTransactionAsInput: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Participant(_Resource):
+    _endpoint_name: ClassVar[str] = "participants"
+    payeeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    payeeId: str = field(default=None, metadata={"id": True}, repr=True)
+    firstName: str = field(default=None, repr=False)
+    lastName: str = field(default=None, repr=False)
+    middleName: str = field(default=None, repr=False)
+    prefix: str = field(default=None, repr=False)
+    suffix: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    hireDate: date = field(default=None, repr=False)
+    terminationDate: date = field(default=None, repr=False)
+    salary: Value = field(default=None, repr=False)
+    userId: str = field(default=None, repr=False)
+    participantEmail: str = field(default=None, repr=False)
+    preferredLanguage: str = field(default=None, repr=False)
+    eventCalendar: str = field(default=None, repr=False)
+    taxId: str = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Payment(_Resource):
+    _endpoint_name: ClassVar[str] = "payments"
+    paymentSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    position: Position = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    earningCodeId: str = field(default=None, repr=False)
+    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRunDate: datetime = field(default=None, repr=False)
+    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRunDate: datetime = field(default=None, repr=False)
+    reason: str = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PaymentMapping(_Resource):
+    _endpoint_name: ClassVar[str] = "paymentMappings"
+    paymentMappingSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    sourceTableName: str = field(default=None, repr=False)
+    sourceAttribute: str = field(default=None, repr=False)
+    paymentAttribute: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PaymentSummary(_Resource):
+    _endpoint_name: ClassVar[str] = "paymentSummarys"
+    paymentSummarySeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    position: Position = field(default=None, repr=False)
+    participant: Participant = field(default=None, repr=False)
+    period: Period = field(default=None, repr=False)
+    earningGroupId: str = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    pipelineRunDate: datetime = field(default=None, repr=False)
+    appliedDeposit: Value = field(default=None, repr=False)
+    priorBalance: Value = field(default=None, repr=False)
+    balance: Value = field(default=None, repr=False)
+    payment: Value = field(default=None, repr=False)
+    Deposit: Value = field(default=None, repr=False)
+    outstandingBalance: Value = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Period(_Resource):
+    _endpoint_name: ClassVar[str] = "periods"
+    periodSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    shortName: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    periodType: PeriodType = field(default=None, repr=False)
+    parent: Period = field(default=None, repr=False)
+    startDate: date = field(default=None, repr=False)
+    endDate: date = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PeriodType(_Resource):
+    _endpoint_name: ClassVar[str] = "periodTypes"
+    periodTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    level: int = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Pipeline(_Resource):
+    _endpoint_name: ClassVar[str] = "pipelines"
+    pipelineRunSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    batchName: str = field(default=None, repr=False)
+    command: str = field(default=None, repr=False)
+    dateSubmitted: datetime = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    endDateScheduled: datetime = field(default=None, repr=False)
+    groupName: str = field(default=None, repr=False)
+    isolationLevel: str = field(default=None, repr=False)
+    message: str = field(default=None, repr=False)
+    modelRun: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    numErrors: int = field(default=None, repr=False)
+    numWarnings: int = field(default=None, repr=False)
+    period: str = field(default=None, repr=False)
+    priority: str = field(default=None, repr=False)
+    processingUnit: str = field(default=None, repr=False)
+    productVersion: str = field(default=None, repr=False)
+    removeDate: datetime = field(default=None, repr=False)
+    reportTypeName: str = field(default=None, repr=False)
+    runMode: str = field(default=None, repr=False)
+    runParameters: str = field(default=None, repr=False)
+    runProgress: str = field(default=None, repr=False)
+    scheduleDay: str = field(default=None, repr=False)
+    scheduleFrequency: str = field(default=None, repr=False)
+    schemaVersion: str = field(default=None, repr=False)
+    stageTables: list = field(default=None, metadata={"type": str}, repr=False)
+    stageType: str = field(default=None, repr=False)
+    startDateScheduled: datetime = field(default=None, repr=False)
+    startTime: datetime = field(default=None, repr=False)
+    state: str = field(default=None, repr=False)
+    status: str = field(default=None, repr=False)
+    stopTime: datetime = field(default=None, repr=False)
+    storedProcVersion: str = field(default=None, repr=False)
+    targetDatabase: str = field(default=None, repr=False)
+    traceLevel: str = field(default=None, repr=False)
+    userId: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Plan(_Resource):
+    _endpoint_name: ClassVar[str] = "plans"
+    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    variableAssignments: VariableAssignment = field(
+        default=None, metadata={"expand": True}, repr=False
+    )
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Position(_Resource):
+    _endpoint_name: ClassVar[str] = "positions"
+    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=date(2200, 1, 1), repr=True)
+    creditStartDate: date = field(default=None, repr=False)
+    creditEndDate: date = field(default=None, repr=False)
+    processingStartDate: date = field(default=None, repr=False)
+    processingEndDate: date = field(default=None, repr=False)
+    targetCompensation: Value = field(default=None, repr=False)
+    businessUnits: list[BusinessUnit] = field(default_factory=list, repr=False)
+    manager: Position = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    title: Title = field(default=None, repr=False)
+    positionGroup: PositionGroup = field(default=None, repr=False)
+    payee: Participant = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    plan: Plan = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    variableAssignments: list[VariableAssignment] = field(
+        default_factory=list, metadata={"expand": True}, repr=False
+    )
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PositionGroup(_Resource):
+    _endpoint_name: ClassVar[str] = "positionGroups"
+    positionGroupSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PositionRelation(_Resource):
+    _endpoint_name: ClassVar[str] = "positionRelations"
+    positionRelationSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    parentPosition: Position = field(default=None, repr=False)
+    positionRelationType: PositionRelationType = field(default=None, repr=False)
+    childPosition: Position = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class PositionRelationType(_Resource):
+    _endpoint_name: ClassVar[str] = "positionRelationTypes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    relations: PositionRelation = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class ProcessingUnit(_Resource):
+    _endpoint_name: ClassVar[str] = "processingUnits"
+    processingUnitSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Product(_Resource):
+    _endpoint_name: ClassVar[str] = "products"
+    classifierSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    classifierId: str = field(default=None, metadata={"id": True}, repr=True)
+    name: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    selectorId: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    cost: Value = field(default=None, repr=False)
+    price: Value = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Quota(_Resource):
+    _endpoint_name: ClassVar[str] = "quotas"
+    quotaSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnit: BusinessUnit = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    unitType: UnitType = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class RateTable(_Resource):
+    _endpoint_name: ClassVar[str] = "rateTables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnit: BusinessUnit = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class RateTableVariable(_Resource):
+    _endpoint_name: ClassVar[str] = "rateTableVariables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    requiredPeriodType: PeriodType = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    unitType: UnitType = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    defaultElement: str = field(default=None, repr=False)
+    referenceClassType: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Reason(_Resource):
+    _endpoint_name: ClassVar[str] = "reasons"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    reasonId: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Rule(_Resource):
+    _endpoint_name: ClassVar[str] = "rules"
+    ruleSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    businessUnit: BusinessUnit = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    type: RuleType = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class RuleType(_Resource):
+    _endpoint_name: ClassVar[str] = "ruleType"
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    id: int = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class SalesOrder(_Resource):
+    _endpoint_name: ClassVar[str] = "salesOrders"
+    salesOrderSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    orderId: str = field(default=None, metadata={"id": True}, repr=True)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class SalesTransaction(_Resource):
+    _endpoint_name: ClassVar[str] = "salesTransactions"
+    salesTransactionSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    salesOrder: SalesOrder = field(default=None, repr=False)
+    lineNumber: Value = field(default=None, repr=False)
+    subLineNumber: Value = field(default=None, repr=False)
+    value: Value = field(default=None, repr=False)
+    preadjustedValue: Value = field(default=None, repr=False)
+    isRunnable: bool = field(default=None, repr=False)
+    compensationDate: date = field(default=None, repr=False)
+    eventType: EventType = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modificationDate: datetime = field(default=None, repr=False)
+    reason: Reason = field(default=None, repr=False)
+    channel: str = field(default=None, repr=False)
+    poNumber: str = field(default=None, repr=False)
+    dataSource: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    shipToAddress: Address = field(default=None, repr=False)
+    otherToAddress: Address = field(default=None, repr=False)
+    billToAddress: Address = field(default=None, repr=False)
+    transactionAssignments: TransactionAssignment = field(
+        default=None, metadata={"expand": True}, repr=False
+    )
+    discountType: str = field(default=None, repr=False)
+    productName: str = field(default=None, repr=False)
+    productDescription: str = field(default=None, repr=False)
+    paymentTerms: str = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    unitValue: Value = field(default=None, repr=False)
+    accountingDate: date = field(default=None, repr=False)
+    discountPercent: Value = field(default=None, repr=False)
+    comments: str = field(default=None, repr=False)
+    productId: str = field(default=None, repr=False)
+    numberOfUnits: Value = field(default=None, repr=False)
+    nativeCurrencyAmount: Value = field(default=None, repr=False)
+    nativeCurrency: str = field(default=None, repr=False)
+    pipelineRun: Pipeline = field(default=None, repr=False)
+    alternateOrderNumber: str = field(default=None, repr=False)
+    originTypeId: str = field(default=None, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericAttribute17: str = field(default=None, repr=False)
+    genericAttribute18: str = field(default=None, repr=False)
+    genericAttribute19: str = field(default=None, repr=False)
+    genericAttribute20: str = field(default=None, repr=False)
+    genericAttribute21: str = field(default=None, repr=False)
+    genericAttribute22: str = field(default=None, repr=False)
+    genericAttribute23: str = field(default=None, repr=False)
+    genericAttribute24: str = field(default=None, repr=False)
+    genericAttribute25: str = field(default=None, repr=False)
+    genericAttribute26: str = field(default=None, repr=False)
+    genericAttribute27: str = field(default=None, repr=False)
+    genericAttribute28: str = field(default=None, repr=False)
+    genericAttribute29: str = field(default=None, repr=False)
+    genericAttribute30: str = field(default=None, repr=False)
+    genericAttribute31: str = field(default=None, repr=False)
+    genericAttribute32: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class StatusCode(_Resource):
+    _endpoint_name: ClassVar[str] = "statusCodes"
+    dataTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    type: str = field(default=None, repr=False)
+    isActive: bool = field(default=None, repr=False)
+    status: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Territory(_Resource):
+    _endpoint_name: ClassVar[str] = "territories"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    definition: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    returnType: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class TerritoryVariable(_Resource):
+    _endpoint_name: ClassVar[str] = "territoryVariables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: BusinessUnit = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    defaultElement: str = field(default=None, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    referenceClassType: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    requiredPeriodType: PeriodType = field(default=None, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Title(_Resource):
+    _endpoint_name: ClassVar[str] = "titles"
+    ruleElementOwnerSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
+    plan: str = field(default=None, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    genericAttribute1: str = field(default=None, repr=False)
+    genericAttribute2: str = field(default=None, repr=False)
+    genericAttribute3: str = field(default=None, repr=False)
+    genericAttribute4: str = field(default=None, repr=False)
+    genericAttribute5: str = field(default=None, repr=False)
+    genericAttribute6: str = field(default=None, repr=False)
+    genericAttribute7: str = field(default=None, repr=False)
+    genericAttribute8: str = field(default=None, repr=False)
+    genericAttribute9: str = field(default=None, repr=False)
+    genericAttribute10: str = field(default=None, repr=False)
+    genericAttribute11: str = field(default=None, repr=False)
+    genericAttribute12: str = field(default=None, repr=False)
+    genericAttribute13: str = field(default=None, repr=False)
+    genericAttribute14: str = field(default=None, repr=False)
+    genericAttribute15: str = field(default=None, repr=False)
+    genericAttribute16: str = field(default=None, repr=False)
+    genericNumber1: Value = field(default=None, repr=False)
+    genericNumber2: Value = field(default=None, repr=False)
+    genericNumber3: Value = field(default=None, repr=False)
+    genericNumber4: Value = field(default=None, repr=False)
+    genericNumber5: Value = field(default=None, repr=False)
+    genericNumber6: Value = field(default=None, repr=False)
+    genericDate1: date = field(default=None, repr=False)
+    genericDate2: date = field(default=None, repr=False)
+    genericDate3: date = field(default=None, repr=False)
+    genericDate4: date = field(default=None, repr=False)
+    genericDate5: date = field(default=None, repr=False)
+    genericDate6: date = field(default=None, repr=False)
+    genericBoolean1: bool = field(default=None, repr=False)
+    genericBoolean2: bool = field(default=None, repr=False)
+    genericBoolean3: bool = field(default=None, repr=False)
+    genericBoolean4: bool = field(default=None, repr=False)
+    genericBoolean5: bool = field(default=None, repr=False)
+    genericBoolean6: bool = field(default=None, repr=False)
+    variableAssignments: VariableAssignment = field(
+        default=None, metadata={"expand": True}, repr=False
+    )
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class TransactionAssignment(_Resource):
+    _endpoint_name: ClassVar[str] = "transactionAssignment"
+    titleName: str = field(default=None, repr=False)
+    payeeId: str = field(default=None, repr=False)
+    positionName: str = field(default=None, repr=False)
+    salesOrder: SalesOrder = field(default=None, repr=False)
+    salesTransactionSeq: int = field(default=None, repr=False)
+    setNumber: int = field(default=None, repr=False)
+    compensationDate: date = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class UnitType(_Resource):
+    _endpoint_name: ClassVar[str] = "unitTypes"
+    unitTypeSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    symbol: str = field(default=None, repr=False)
+    currencyLocale: str = field(default=None, repr=False)
+    formatting: str = field(default=None, repr=False)
+    positionOfSymbol: int = field(default=None, repr=False)
+    reportingScale: str = field(default=None, repr=False)
+    scale: int = field(default=None, repr=False)
+    valueClass: dict = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class User(_Resource):
+    _endpoint_name: ClassVar[str] = "users"
+    userSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    id: str = field(default=None, metadata={"id": True}, repr=True)
+    userName: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    readOnlyBusinessUnitList: BusinessUnit = field(default=None, repr=False)
+    fullAccessBusinessUnitList: BusinessUnit = field(default=None, repr=False)
+    groups: Group = field(default=None, repr=False)
+    email: str = field(default=None, repr=False)
+    preferredLanguage: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Value(_Resource):
+    _endpoint_name: ClassVar[str] = "value"
+    value: float = field(default=None, repr=False)
+    unitType: UnitType = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class Variable(_Resource):
+    _endpoint_name: ClassVar[str] = "variables"
+    ruleElementSeq: int = field(default=None, metadata={"seq": True}, repr=False)
+    name: str = field(default=None, metadata={"id": True}, repr=True)
+    description: str = field(default=None, repr=False)
+    calendar: Calendar = field(default=None, repr=False)
+    requiredPeriodType: PeriodType = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    businessUnits: list = field(default=None, metadata={"type": str}, repr=False)
+    plan: str = field(default=None, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modifiedBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    createdBy: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
+    notAllowUpdate: bool = field(default=None, repr=False)
+    defaultElement: str = field(default=None, repr=False)
+    referenceClassType: str = field(default=None, repr=False)
+    returnType: str = field(default=None, repr=False)
+    owningElement: str = field(default=None, repr=False)
+    ruleUsage: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+    inputSignature: str = field(default=None, repr=False)
+    etag: str = field(default=None, metadata={"json_ignore": True}, repr=False)
+
+
+@dataclass
+class VariableAssignment(_Resource):
+    _endpoint_name: ClassVar[str] = "variableAssignment"
+    owner: str = field(default=None, repr=False)
+    variable: str = field(default=None, repr=False)
+    assignment: str = field(default=None, repr=False)
+    effectiveStartDate: date = field(default=None, repr=True)
+    effectiveEndDate: date = field(default=None, repr=False)
+    createDate: datetime = field(
+        default=None, metadata={"json_ignore": True}, repr=False
+    )
+    modelSeq: Model = field(default=None, metadata={"json_ignore": True}, repr=False)
```

### Comparing `python-sapcommissions-1.0.0/tests/test_base.py` & `python-sapcommissions-1.0.1/tests/test_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import unittest
-from dataclasses import asdict
-
-from sapcommissions import Connection
-
-
-class TestConnection(unittest.TestCase):
-    def test_url(self):
-        # Create a connection instance to test
-        conn = Connection(
-            tenant="spam", environment="eggs", username="user", password="pass"
-        )
-
-        # Check that the url property returns the expected value
-        self.assertEqual(conn.url, "https://spam-eggs.callidusondemand.com")
-
-    def test_api_url(self):
-        # Create a connection instance to test
-        conn = Connection(
-            tenant="spam", environment="eggs", username="user", password="pass"
-        )
-
-        # Check that the api_url property returns the expected value
-        self.assertEqual(conn.api_url, "https://spam-eggs.callidusondemand.com/api")
-
-    def test_api_document(self):
-        # Create a connection instance to test
-        conn = Connection(
-            tenant="spam", environment="eggs", username="user", password="pass"
-        )
-
-        # Check that the api_document property returns the expected value
-        self.assertEqual(
-            conn.api_document, "https://spam-eggs.callidusondemand.com/APIDocument"
-        )
-
-    def test_connection_dataclass(self):
-        # Check that the Connection dataclass is defined correctly
-        conn_dict = {
-            "tenant": "spam",
-            "environment": "eggs",
-            "username": "user",
-            "password": "pass",
-            "verify_ssl": True,
-        }
-
-        # Check that the fields of the Connection instance match the values in conn_dict
-        conn = Connection(**conn_dict)
-        self.assertEqual(asdict(conn), conn_dict)
-
-        # Check that the verify_ssl field defaults to True if not provided
-        del conn_dict["verify_ssl"]
-        conn = Connection(**conn_dict)
-        conn_dict["verify_ssl"] = True  # Verify that verify_ssl defaults to True
-        self.assertEqual(asdict(conn), conn_dict)
-
-    def test_hidden_password(self):
-        # Create a connection instance to test
-        conn = Connection(
-            tenant="spam", environment="eggs", username="foo", password="barbaz"
-        )
-
-        # Check that the password property is hidden from the string representation.
-        self.assertNotIn("barbaz", str(conn))
-        self.assertNotIn("barbaz", repr(conn))
+import unittest
+from dataclasses import asdict
+
+from sapcommissions import Connection
+
+
+class TestConnection(unittest.TestCase):
+    def test_url(self):
+        # Create a connection instance to test
+        conn = Connection(
+            tenant="spam", environment="eggs", username="user", password="pass"
+        )
+
+        # Check that the url property returns the expected value
+        self.assertEqual(conn.url, "https://spam-eggs.callidusondemand.com")
+
+    def test_api_url(self):
+        # Create a connection instance to test
+        conn = Connection(
+            tenant="spam", environment="eggs", username="user", password="pass"
+        )
+
+        # Check that the api_url property returns the expected value
+        self.assertEqual(conn.api_url, "https://spam-eggs.callidusondemand.com/api")
+
+    def test_api_document(self):
+        # Create a connection instance to test
+        conn = Connection(
+            tenant="spam", environment="eggs", username="user", password="pass"
+        )
+
+        # Check that the api_document property returns the expected value
+        self.assertEqual(
+            conn.api_document, "https://spam-eggs.callidusondemand.com/APIDocument"
+        )
+
+    def test_connection_dataclass(self):
+        # Check that the Connection dataclass is defined correctly
+        conn_dict = {
+            "tenant": "spam",
+            "environment": "eggs",
+            "username": "user",
+            "password": "pass",
+            "verify_ssl": True,
+        }
+
+        # Check that the fields of the Connection instance match the values in conn_dict
+        conn = Connection(**conn_dict)
+        self.assertEqual(asdict(conn), conn_dict)
+
+        # Check that the verify_ssl field defaults to True if not provided
+        del conn_dict["verify_ssl"]
+        conn = Connection(**conn_dict)
+        conn_dict["verify_ssl"] = True  # Verify that verify_ssl defaults to True
+        self.assertEqual(asdict(conn), conn_dict)
+
+    def test_hidden_password(self):
+        # Create a connection instance to test
+        conn = Connection(
+            tenant="spam", environment="eggs", username="foo", password="barbaz"
+        )
+
+        # Check that the password property is hidden from the string representation.
+        self.assertNotIn("barbaz", str(conn))
+        self.assertNotIn("barbaz", repr(conn))
```

### Comparing `python-sapcommissions-1.0.0/tests/test_resources.py` & `python-sapcommissions-1.0.1/tests/test_resources.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-import unittest
-from dataclasses import dataclass, field
-from datetime import date, datetime
-from typing import ClassVar, List
-
-from sapcommissions.resources import _decode, _encode, _Resource
-
-
-@dataclass
-class DummyResource(_Resource):
-    _endpoint_name: ClassVar[str] = "test"
-    id: str = field(metadata={"id": True})
-    name: str = field(default=None)
-    items: List[str] = field(default_factory=list)
-    expands: bool = field(default=None, metadata={"expand": True})
-
-
-class TestResourceMethods(unittest.TestCase):
-    def setUp(self):
-        self.resource_dict = {
-            "id": "123",
-            "name": "Test Resource",
-            "items": ["item1", "item2"],
-            "expands": False,
-        }
-        self.resource: DummyResource = DummyResource.from_dict(self.resource_dict)
-
-    def test_name_property(self):
-        self.assertEqual(DummyResource._name, "test")
-
-    def test_seq_attr_property(self):
-        self.assertIsNone(DummyResource._seq_attr)
-
-    def test_seq_property(self):
-        self.assertIsNone(self.resource._seq)
-
-    def test_id_attr_property(self):
-        self.assertEqual(DummyResource._id_attr, "id")
-
-    def test_id_property(self):
-        self.assertEqual(self.resource._id, "123")
-
-    def test_expands_property(self):
-        self.assertEqual(DummyResource._expands, ("expands",))
-
-    def test_from_dict_method(self):
-        self.assertIsInstance(self.resource, DummyResource)
-        self.assertEqual(self.resource.id, "123")
-        self.assertEqual(self.resource.name, "Test Resource")
-        self.assertEqual(self.resource.items, ["item1", "item2"])
-        self.assertEqual(self.resource.expands, False)
-
-    def test_to_dict_method(self):
-        expected_dict = {
-            "id": "123",
-            "name": "Test Resource",
-            "items": ["item1", "item2"],
-            "expands": False,
-        }
-        self.assertEqual(self.resource.to_dict(), expected_dict)
-
-
-class TestEncodeDecode(unittest.TestCase):
-    def test_decode_datetime(self):
-        dt_str = "2000-01-02T03:04:05.000-06:00"
-        decoded_dt = _decode(dt_str, datetime)
-        self.assertEqual(decoded_dt, datetime.fromisoformat(dt_str))
-
-    def test_encode_datetime(self):
-        dt = datetime(2000, 1, 2, 3, 4, 5)
-        encoded_dt = _encode(dt, datetime)
-        self.assertEqual(encoded_dt, "2000-01-02T03:04:05")
-
-    def test_decode_date(self):
-        date_str = "2000-01-02T03:04:05.000-06:00"
-        decoded_date = _decode(date_str, date)
-        self.assertEqual(decoded_date, datetime.fromisoformat(date_str).date())
-
-    def test_encode_date(self):
-        dt = date(2000, 1, 2)
-        encoded_dt = _encode(dt, date)
-        self.assertEqual(encoded_dt, "2000-01-02")
-
-    def test_decode_none(self):
-        decoded_none = _decode(None, str)
-        self.assertIs(decoded_none, None)
-
-    def test_encode_none(self):
-        encoded_none = _encode(None, str)
-        self.assertIs(encoded_none, None)
-
-    def test_decode_string(self):
-        test_str = "SPAM"
-        decoded_str = _decode(test_str, str)
-        self.assertEqual(decoded_str, "SPAM")
-
-    def test_encode_string(self):
-        test_str = "SPAM"
-        encoded_str = _encode(test_str, str)
-        self.assertEqual(encoded_str, "SPAM")
-
-    def test_decode_int(self):
-        test_int = 1
-        decoded_int = _decode(test_int, int)
-        self.assertEqual(decoded_int, 1)
-
-    def test_decode_str_int(self):
-        test_int_str = "1"
-        decoded_int_str = _decode(test_int_str, int)
-        self.assertEqual(decoded_int_str, 1)
-
-    def test_encode_int(self):
-        test_int = 1
-        encoded_int = _encode(test_int, int)
-        self.assertEqual(encoded_int, 1)
-
-    def test_decode_list_str(self):
-        test_list = ["SPAM", "EGGS"]
-        decoded_list = _decode(test_list, list[str])
-        self.assertListEqual(decoded_list, test_list)
-
-    def test_decode_list_error(self):
-        test_list = ["SPAM", "EGGS"]
-        with self.assertRaises(TypeError):
-            _decode(test_list, list[str, int])
-        with self.assertRaises(TypeError):
-            _decode(test_list, list)
-        with self.assertRaises(TypeError):
-            _decode(test_list, str)
-
-    def test_decode_unions(self):
-        test_value = 1
-        with self.assertRaises(NotImplementedError):
-            _decode(test_value, int | dict)
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from dataclasses import dataclass, field
+from datetime import date, datetime
+from typing import ClassVar, List
+
+from sapcommissions.resources import _decode, _encode, _Resource
+
+
+@dataclass
+class DummyResource(_Resource):
+    _endpoint_name: ClassVar[str] = "test"
+    id: str = field(metadata={"id": True})
+    name: str = field(default=None)
+    items: List[str] = field(default_factory=list)
+    expands: bool = field(default=None, metadata={"expand": True})
+
+
+class TestResourceMethods(unittest.TestCase):
+    def setUp(self):
+        self.resource_dict = {
+            "id": "123",
+            "name": "Test Resource",
+            "items": ["item1", "item2"],
+            "expands": False,
+        }
+        self.resource: DummyResource = DummyResource.from_dict(self.resource_dict)
+
+    def test_name_property(self):
+        self.assertEqual(DummyResource._name, "test")
+
+    def test_seq_attr_property(self):
+        self.assertIsNone(DummyResource._seq_attr)
+
+    def test_seq_property(self):
+        self.assertIsNone(self.resource._seq)
+
+    def test_id_attr_property(self):
+        self.assertEqual(DummyResource._id_attr, "id")
+
+    def test_id_property(self):
+        self.assertEqual(self.resource._id, "123")
+
+    def test_expands_property(self):
+        self.assertEqual(DummyResource._expands, ("expands",))
+
+    def test_from_dict_method(self):
+        self.assertIsInstance(self.resource, DummyResource)
+        self.assertEqual(self.resource.id, "123")
+        self.assertEqual(self.resource.name, "Test Resource")
+        self.assertEqual(self.resource.items, ["item1", "item2"])
+        self.assertEqual(self.resource.expands, False)
+
+    def test_to_dict_method(self):
+        expected_dict = {
+            "id": "123",
+            "name": "Test Resource",
+            "items": ["item1", "item2"],
+            "expands": False,
+        }
+        self.assertEqual(self.resource.to_dict(), expected_dict)
+
+
+class TestEncodeDecode(unittest.TestCase):
+    def test_decode_datetime(self):
+        dt_str = "2000-01-02T03:04:05.000-06:00"
+        decoded_dt = _decode(dt_str, datetime)
+        self.assertEqual(decoded_dt, datetime.fromisoformat(dt_str))
+
+    def test_encode_datetime(self):
+        dt = datetime(2000, 1, 2, 3, 4, 5)
+        encoded_dt = _encode(dt, datetime)
+        self.assertEqual(encoded_dt, "2000-01-02T03:04:05")
+
+    def test_decode_date(self):
+        date_str = "2000-01-02T03:04:05.000-06:00"
+        decoded_date = _decode(date_str, date)
+        self.assertEqual(decoded_date, datetime.fromisoformat(date_str).date())
+
+    def test_encode_date(self):
+        dt = date(2000, 1, 2)
+        encoded_dt = _encode(dt, date)
+        self.assertEqual(encoded_dt, "2000-01-02")
+
+    def test_decode_none(self):
+        decoded_none = _decode(None, str)
+        self.assertIs(decoded_none, None)
+
+    def test_encode_none(self):
+        encoded_none = _encode(None, str)
+        self.assertIs(encoded_none, None)
+
+    def test_decode_string(self):
+        test_str = "SPAM"
+        decoded_str = _decode(test_str, str)
+        self.assertEqual(decoded_str, "SPAM")
+
+    def test_encode_string(self):
+        test_str = "SPAM"
+        encoded_str = _encode(test_str, str)
+        self.assertEqual(encoded_str, "SPAM")
+
+    def test_decode_int(self):
+        test_int = 1
+        decoded_int = _decode(test_int, int)
+        self.assertEqual(decoded_int, 1)
+
+    def test_decode_str_int(self):
+        test_int_str = "1"
+        decoded_int_str = _decode(test_int_str, int)
+        self.assertEqual(decoded_int_str, 1)
+
+    def test_encode_int(self):
+        test_int = 1
+        encoded_int = _encode(test_int, int)
+        self.assertEqual(encoded_int, 1)
+
+    def test_decode_list_str(self):
+        test_list = ["SPAM", "EGGS"]
+        decoded_list = _decode(test_list, list[str])
+        self.assertListEqual(decoded_list, test_list)
+
+    def test_decode_list_error(self):
+        test_list = ["SPAM", "EGGS"]
+        with self.assertRaises(TypeError):
+            _decode(test_list, list[str, int])
+        with self.assertRaises(TypeError):
+            _decode(test_list, list)
+        with self.assertRaises(TypeError):
+            _decode(test_list, str)
+
+    def test_decode_unions(self):
+        test_value = 1
+        with self.assertRaises(NotImplementedError):
+            _decode(test_value, int | dict)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

