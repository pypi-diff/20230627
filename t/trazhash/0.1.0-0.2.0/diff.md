# Comparing `tmp/trazhash-0.1.0.tar.gz` & `tmp/trazhash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trazhash-0.1.0.tar", last modified: Tue Jun 27 01:57:31 2023, max compression
+gzip compressed data, was "trazhash-0.2.0.tar", last modified: Tue Jun 27 02:05:41 2023, max compression
```

## Comparing `trazhash-0.1.0.tar` & `trazhash-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 01:57:31.138745 trazhash-0.1.0/
--rw-rw-rw-   0        0        0     3343 2023-06-27 01:57:31.135784 trazhash-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2023-06-27 01:57:27.000000 trazhash-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 01:57:31.138745 trazhash-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-06-27 01:55:37.000000 trazhash-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:57:31.132743 trazhash-0.1.0/trazhash.egg-info/
--rw-rw-rw-   0        0        0     3343 2023-06-27 01:57:30.000000 trazhash-0.1.0/trazhash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-06-27 01:57:30.000000 trazhash-0.1.0/trazhash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:57:30.000000 trazhash-0.1.0/trazhash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:57:30.000000 trazhash-0.1.0/trazhash.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 02:05:41.620248 trazhash-0.2.0/
+-rw-rw-rw-   0        0        0     3389 2023-06-27 02:05:41.618245 trazhash-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2023-06-27 02:04:24.000000 trazhash-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 02:05:41.620248 trazhash-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-06-27 02:05:36.000000 trazhash-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:05:41.616244 trazhash-0.2.0/trazhash.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-27 02:05:41.000000 trazhash-0.2.0/trazhash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-06-27 02:05:41.000000 trazhash-0.2.0/trazhash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 02:05:41.000000 trazhash-0.2.0/trazhash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 02:05:41.000000 trazhash-0.2.0/trazhash.egg-info/top_level.txt
```

### Comparing `trazhash-0.1.0/PKG-INFO` & `trazhash-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trazhash
-Version: 0.1.0
+Version: 0.2.0
 Summary: TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions.
 Home-page: https://github.com/traztech/trazhash
 Author: TrazTech
 Author-email: contact@traztech.ca
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -14,15 +14,15 @@
 
 TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions. By incorporating system-specific values such as the system name, node name, release, version, machine, processor, and hostname into the hashing process, the library produces hashes that are tied to the particular system on which the hashing was performed. This can be useful for generating unique identifiers, checksums, or verifying the integrity and origin of data.
 
 The library supports multiple levels of hashing (e.g., hash inside another hash) and allows users to specify the desired cryptographic hash functions (e.g., SHA256, SHA512) for each level.
 
 TrazHash is easy to use, highly configurable, and can be integrated into various Python projects including security applications, data verification tools, and more.
 
-![TrazHash](TRAZHASH.png)
+![TrazHash](https://github.com/traztech/trazhash/raw/main/TRAZHASH.png)
 
 ## Features
 
 - **System-specific Hashing**: Combines data strings or file contents with system-specific values before hashing, ensuring that hashes are unique to the system.
 - **Multi-level Hashing**: Supports hashing data inside another hash, which can be used for additional security and integrity assurance.
 - **Configurable Hash Algorithms**: Allows users to specify which cryptographic hash functions to use at each level.
 - **File Hashing**: Conveniently hash the contents of a file.
```

### Comparing `trazhash-0.1.0/README.md` & `trazhash-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions. By incorporating system-specific values such as the system name, node name, release, version, machine, processor, and hostname into the hashing process, the library produces hashes that are tied to the particular system on which the hashing was performed. This can be useful for generating unique identifiers, checksums, or verifying the integrity and origin of data.
 
 The library supports multiple levels of hashing (e.g., hash inside another hash) and allows users to specify the desired cryptographic hash functions (e.g., SHA256, SHA512) for each level.
 
 TrazHash is easy to use, highly configurable, and can be integrated into various Python projects including security applications, data verification tools, and more.
 
-![TrazHash](TRAZHASH.png)
+![TrazHash](https://github.com/traztech/trazhash/raw/main/TRAZHASH.png)
 
 ## Features
 
 - **System-specific Hashing**: Combines data strings or file contents with system-specific values before hashing, ensuring that hashes are unique to the system.
 - **Multi-level Hashing**: Supports hashing data inside another hash, which can be used for additional security and integrity assurance.
 - **Configurable Hash Algorithms**: Allows users to specify which cryptographic hash functions to use at each level.
 - **File Hashing**: Conveniently hash the contents of a file.
```

### Comparing `trazhash-0.1.0/setup.py` & `trazhash-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trazhash',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         # List your library dependencies here
     ],
     author='TrazTech',
     author_email='contact@traztech.ca',
     description="TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions.",
```

### Comparing `trazhash-0.1.0/trazhash.egg-info/PKG-INFO` & `trazhash-0.2.0/trazhash.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trazhash
-Version: 0.1.0
+Version: 0.2.0
 Summary: TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions.
 Home-page: https://github.com/traztech/trazhash
 Author: TrazTech
 Author-email: contact@traztech.ca
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -14,15 +14,15 @@
 
 TrazHash is a Python library designed to hash data strings or file contents using a combination of your system's specific values and cryptographic hash functions. By incorporating system-specific values such as the system name, node name, release, version, machine, processor, and hostname into the hashing process, the library produces hashes that are tied to the particular system on which the hashing was performed. This can be useful for generating unique identifiers, checksums, or verifying the integrity and origin of data.
 
 The library supports multiple levels of hashing (e.g., hash inside another hash) and allows users to specify the desired cryptographic hash functions (e.g., SHA256, SHA512) for each level.
 
 TrazHash is easy to use, highly configurable, and can be integrated into various Python projects including security applications, data verification tools, and more.
 
-![TrazHash](TRAZHASH.png)
+![TrazHash](https://github.com/traztech/trazhash/raw/main/TRAZHASH.png)
 
 ## Features
 
 - **System-specific Hashing**: Combines data strings or file contents with system-specific values before hashing, ensuring that hashes are unique to the system.
 - **Multi-level Hashing**: Supports hashing data inside another hash, which can be used for additional security and integrity assurance.
 - **Configurable Hash Algorithms**: Allows users to specify which cryptographic hash functions to use at each level.
 - **File Hashing**: Conveniently hash the contents of a file.
```

