# Comparing `tmp/whoisdomain-1.20230525.9.tar.gz` & `tmp/whoisdomain-1.20230627.2.tar.gz`

## Comparing `whoisdomain-1.20230525.9.tar` & `whoisdomain-1.20230627.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/main.py
--rw-r--r--   0        0        0   131262 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/.gitignore
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/pyproject.toml
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 whoisdomain-1.20230525.9/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/main.py
+-rw-r--r--   0        0        0   131444 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/.gitignore
+-rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/README.md
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/pyproject.toml
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 whoisdomain-1.20230627.2/PKG-INFO
```

### Comparing `whoisdomain-1.20230525.9/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230627.2/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/_1_query.py` & `whoisdomain-1.20230627.2/whoisdomain/_1_query.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/_2_parse.py` & `whoisdomain-1.20230627.2/whoisdomain/_2_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,17 +262,15 @@
         if with_cleanup_results is True and line.startswith("%"):  # only remove if requested
             continue
 
         if withRedacted is False:
             if "REDACTED FOR PRIVACY" in line:  # these lines contibute nothing so ignore
                 continue
 
-        if (
-            "Please query the RDDS service of the Registrar of Record" in line
-        ):  # these lines contibute nothing so ignore
+        if "Please query the RDDS service of the Registrar of Record" in line:  # these lines contibute nothing so ignore
             continue
 
         # regular responses may at the end have meta info starting with a line >>> some texte <<<
         # similar trailing info exists with lines starting with -- but we wil handle them later
         # unfortunalery we have domains (google.st) that have this early at the top
         if 0:
             if line.startswith(">>>"):
```

### Comparing `whoisdomain-1.20230525.9/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230627.2/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/__init__.py` & `whoisdomain-1.20230627.2/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/exceptions.py` & `whoisdomain-1.20230627.2/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/main.py` & `whoisdomain-1.20230627.2/whoisdomain/main.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230627.2/whoisdomain/tld_regexpr.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # when we finally apply the regexes we use IGNORE CASE allways on all matches
 
 # Commercial TLD - Original Big 7
 ZZ["com"] = {
     "extend": None,
     "domain_name": r"Domain Name\s*:\s*(.+)",
     "registrar": r"Registrar:\s?(.+)",
-    "registrant": r"Registrant\s*Organi(?:s|z)ation:\s?(.+)",
+    "registrant": r"Registrant\s*Organi(?:s|z)ation:([^\n]*)",  # this seems to match Registrant Street: if Registrant Organization: is empty
     "registrant_country": r"Registrant Country:\s?(.+)",
     "creation_date": r"Creation Date:[ \t]*([^\n]*)",
     "expiration_date": r"(?:Expiry|Expiration) Date:[ \t]*([^\n]*)",  # Expiration Date
     "updated_date": r"Updated Date:[\t ]*([^\n]*)",
     "name_servers": r"Name Server:\s*(.+)\s*",  # host -t ns <domain> often has more nameservers then the output of whois
     "status": r"Status:\s?(.+)",
     # the trailing domain must have minimal 2 parts firstname.lastname@fld.tld
@@ -1929,16 +1929,21 @@
 ZZ["li"] = {"extend": "_privateReg"}
 ZZ["mp"] = {"extend": "_privateReg"}
 ZZ["my"] = {"extend": "_privateReg"}
 ZZ["pk"] = {"extend": "_privateReg"}
 ZZ["py"] = {"extend": "_privateReg"}  # Paraguay:https://www.iana.org/domains/root/db/py.html
 ZZ["com.py"] = {"extend": "_privateReg"}
 ZZ["sr"] = {"extend": "_privateReg"}
-ZZ["ke"] = {"extend": "_privateReg"}  # Kenia
-ZZ["co.ke"] = {"extend": "_privateReg"}
+
+# Kenia
+ZZ["ke"] = {"extend": "com", "_server": "whois.kenic.or.ke"}
+ZZ["co.ke"] = {"extend": "ke"}
+ZZ["or.ke"] = {"extend": "ke"}
+ZZ["ac.ke"] = {"extend": "ke"}
+ZZ["go.ke"] = {"extend": "ke"}
 
 # https://www.iana.org/domains/root/db/td.html
 # td = {"extend": "_privateReg"} # Chad (French: Tchad) made available for use in 1997.
 
 ZZ["tk"] = {"extend": "_privateReg"}
 ZZ["to"] = {"extend": "_privateReg"}  #
 ZZ["uy"] = {"extend": "_privateReg"}  # Uruguay
@@ -1947,17 +1952,15 @@
 ZZ["vn"] = {"extend": "_privateReg"}
 #
 ZZ["zw"] = {"extend": "_privateReg"}  # Zimbabwe ; # This TLD has no whois server
 ZZ["com.zw"] = {"extend": "zw"}
 ZZ["org.zw"] = {"extend": "zw"}
 
 # Nepal
-ZZ["np"] = {
-    "extend": "_privateReg"
-}  # This TLD has no whois server, but you can access the whois database at https://www.mos.com.np/
+ZZ["np"] = {"extend": "_privateReg"}  # This TLD has no whois server, but you can access the whois database at https://www.mos.com.np/
 ZZ["com.np"] = {"extend": "np"}
 
 # Ecuador
 ZZ["ec"] = {"extend": "_privateReg"}
 ZZ["com.ec"] = {"extend": "ec"}
 ZZ["gob.ec"] = {"extend": "ec"}
```

### Comparing `whoisdomain-1.20230525.9/.gitignore` & `whoisdomain-1.20230627.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230525.9/README.md` & `whoisdomain-1.20230627.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
  * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
  * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
+ * withRedacted: bool = False has been added to query(), if set to True any redacted fields will now be shown also (also supported in the cli whoisdomain as --withRedacted)
+ * a analizer directory is presend in the github repo that will be used to look for new IANA tls's currently unsupported but maching known whois servers
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
 ## Docker
  * docker pull mbootgithub/whoisdomain:latest
  * docker run mbootgithub/whoisdomain -V # show version
```

### Comparing `whoisdomain-1.20230525.9/pyproject.toml` & `whoisdomain-1.20230627.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Makefile",
     ".gitignore",
     "/.gitignore",
 ]
 
 [project]
 name = "whoisdomain"
-version = "1.20230525.9"
+dynamic = ['version']
 
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
   { name="Maarten Boot", email="130295084+mboot-github@users.noreply.github.com" },
@@ -39,22 +39,15 @@
 license = "MIT"
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Environment :: Console",
-
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-
+    "Programming Language :: Python :: 3",
     "Topic :: Internet",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 keywords = [
     "Python",
     "whois",
@@ -64,13 +57,19 @@
     "cctld",
     "registrar",
 ]
 
 [project.scripts]
 whoisdomain = 'whoisdomain.main:main'
 
+[tool.hatch.version]
+path = "whoisdomain/version.py"
+
+[tool.pylama]
+max_line_length = 160
+skip = "*/.pytest_cache/*, */.tox/*, */mypy_cache/*, ./dist, ./docs"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
 "Home Page" = "https://github.com/mboot-github/WhoisDomain/"
 "Repository" = "https://github.com/mboot-github/WhoisDomain/"
```

### Comparing `whoisdomain-1.20230525.9/PKG-INFO` & `whoisdomain-1.20230627.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230525.9
+Version: 1.20230627.2
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
 Keywords: Python,cctld,domain,expiration,registrar,tld,whois
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # whoisdomain
 
@@ -51,14 +46,16 @@
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
  * the module is now 'mypy --strict' clean
  * the module now also exports a cli command domainwhois
  * both the module and the cli now support showing the version with lib:whois.getVersion() or cli:whoisdomain -V
  * the whoisdomain can now output json data (one per domain: e.g 'whoisdomain -d google.com -j' )
+ * withRedacted: bool = False has been added to query(), if set to True any redacted fields will now be shown also (also supported in the cli whoisdomain as --withRedacted)
+ * a analizer directory is presend in the github repo that will be used to look for new IANA tls's currently unsupported but maching known whois servers
 
 ## Dependencies
   * please install also the command line "whois" of your distribution as this library parses the output of the "whois" cli command of your operating system
 
 ## Docker
  * docker pull mbootgithub/whoisdomain:latest
  * docker run mbootgithub/whoisdomain -V # show version
```

