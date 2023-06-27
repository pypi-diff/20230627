# Comparing `tmp/checkdmarc-4.6.0.tar.gz` & `tmp/checkdmarc-4.7.0.tar.gz`

## Comparing `checkdmarc-4.6.0.tar` & `checkdmarc-4.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0   116311 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/checkdmarc.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/LICENSE
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0   117153 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/checkdmarc.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/LICENSE
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/README.md
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 checkdmarc-4.7.0/PKG-INFO
```

### Comparing `checkdmarc-4.6.0/checkdmarc.py` & `checkdmarc-4.7.0/checkdmarc.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License."""
 
-__version__ = "4.6.0"
+__version__ = "4.7.0"
 
 DMARC_VERSION_REGEX_STRING = r"v *= *DMARC1;"
 BIMI_VERSION_REGEX_STRING = r"v=BIMI1;"
 DMARC_TAG_VALUE_REGEX_STRING = r"([a-z]{1,5}) *= *([\w.:@/+!,_\- ]+)"
 BIMI_TAG_VALUE_REGEX_STRING = r"([a-z]{1}) *= *(.*)"
 MAILTO_REGEX_STRING = r"^(mailto):" \
                       r"([\w\-!#$%&'*+-/=?^_`{|}~]" \
@@ -2427,109 +2427,165 @@
         domains.remove(domain)
     while "" in domains:
         domains.remove("")
     results = []
     for domain in domains:
         domain = domain.lower()
         logging.debug("Checking: {0}".format(domain))
+
         domain_results = OrderedDict(
             [("domain", domain), ("base_domain", get_base_domain(domain)),
              ("dnssec", None), ("ns", []), ("mx", [])])
-        domain_results["spf"] = OrderedDict(
-            [("record", None), ("valid", True), ("dns_lookups", None),
-             ("dns_void_lookups", None)])
-        domain_results["dnssec"] = test_dnssec(domain,
-                                               nameservers=nameservers,
-                                               timeout=timeout)
-        try:
-            domain_results["ns"] = get_nameservers(
-                domain,
-                approved_nameservers=approved_nameservers,
-                nameservers=nameservers, resolver=resolver,
-                timeout=timeout)
-        except DNSException as error:
-            domain_results["ns"] = OrderedDict([("hostnames", []),
-                                                ("error", error.__str__())])
-        try:
-            domain_results["mx"] = get_mx_hosts(
-                domain,
-                skip_tls=skip_tls,
-                approved_hostnames=approved_mx_hostnames,
-                nameservers=nameservers, resolver=resolver,
-                timeout=timeout)
-        except DNSException as error:
-            domain_results["mx"] = OrderedDict([("hosts", []),
-                                                ("error", error.__str__())])
-        try:
-            spf_query = query_spf_record(
-                domain,
-                nameservers=nameservers, resolver=resolver,
-                timeout=timeout)
-            domain_results["spf"]["record"] = spf_query["record"]
-            domain_results["spf"]["warnings"] = spf_query["warnings"]
-            parsed_spf = parse_spf_record(domain_results["spf"]["record"],
-                                          domain_results["domain"],
-                                          parked=parked,
-                                          nameservers=nameservers,
-                                          resolver=resolver,
-                                          timeout=timeout)
-
-            domain_results["spf"]["dns_lookups"] = parsed_spf[
-                "dns_lookups"]
-            domain_results["spf"]["dns_void_lookups"] = parsed_spf[
-                "dns_void_lookups"]
-            domain_results["spf"]["parsed"] = parsed_spf["parsed"]
-            domain_results["spf"]["warnings"] += parsed_spf["warnings"]
-        except SPFError as error:
-            domain_results["spf"]["error"] = str(error)
-            del domain_results["spf"]["dns_lookups"]
-            domain_results["spf"]["valid"] = False
-            if hasattr(error, "data") and error.data:
-                for key in error.data:
-                    domain_results["spf"][key] = error.data[key]
-
-        # DMARC
-        domain_results["dmarc"] = OrderedDict([("record", None),
-                                               ("valid", True),
-                                               ("location", None)])
-        try:
-            dmarc_query = query_dmarc_record(domain,
-                                             nameservers=nameservers,
-                                             resolver=resolver,
-                                             timeout=timeout)
-            domain_results["dmarc"]["record"] = dmarc_query["record"]
-            domain_results["dmarc"]["location"] = dmarc_query["location"]
-            parsed_dmarc_record = parse_dmarc_record(
-                dmarc_query["record"],
-                dmarc_query["location"],
-                parked=parked,
-                include_tag_descriptions=include_dmarc_tag_descriptions,
-                nameservers=nameservers, resolver=resolver,
-                timeout=timeout)
-            domain_results["dmarc"]["warnings"] = dmarc_query["warnings"]
-
-            domain_results["dmarc"]["tags"] = parsed_dmarc_record["tags"]
-            domain_results["dmarc"]["warnings"] += parsed_dmarc_record[
-                "warnings"]
-        except DMARCError as error:
-            domain_results["dmarc"]["error"] = str(error)
-            domain_results["dmarc"]["valid"] = False
-            if hasattr(error, "data") and error.data:
-                for key in error.data:
-                    domain_results["dmarc"][key] = error.data[key]
+
+        domain_results["dnssec"] = test_dnssec(
+            domain,
+            nameservers=nameservers,
+            timeout=timeout
+            )
+
+        domain_results["ns"] = check_ns(
+            domain,
+            approved_nameservers=approved_nameservers,
+            nameservers=nameservers,
+            resolver=resolver, timeout=timeout
+            )
+
+        domain_results["mx"] = check_mx(
+            domain,
+            approved_mx_hostnames=approved_mx_hostnames,
+            skip_tls=skip_tls,
+            nameservers=nameservers,
+            resolver=resolver,
+            timeout=timeout
+            )
+
+        domain_results["spf"] = check_spf(
+            domain,
+            parked=parked,
+            nameservers=nameservers,
+            resolver=resolver,
+            timeout=timeout
+            )
+
+        domain_results["dmarc"] = check_dmarc(
+            domain,
+            parked=parked,
+            include_dmarc_tag_descriptions=include_dmarc_tag_descriptions,
+            nameservers=nameservers,
+            resolver=resolver,
+            timeout=timeout
+            )
+
         results.append(domain_results)
         if wait > 0.0:
             logging.debug("Sleeping for {0} seconds".format(wait))
             sleep(wait)
     if len(results) == 1:
         results = results[0]
 
     return results
 
 
+def check_ns(domain, approved_nameservers=None,
+             nameservers=None, resolver=None, timeout=2.0):
+    try:
+        ns_results = get_nameservers(
+            domain,
+            approved_nameservers=approved_nameservers,
+            nameservers=nameservers, resolver=resolver,
+            timeout=timeout)
+    except DNSException as error:
+        ns_results = OrderedDict([("hostnames", []),
+                                  ("error", error.__str__())])
+    return ns_results
+
+
+def check_mx(domain, approved_mx_hostnames=None, skip_tls=False,
+             nameservers=None, resolver=None, timeout=2.0):
+    try:
+        mx_results = get_mx_hosts(
+            domain,
+            skip_tls=skip_tls,
+            approved_hostnames=approved_mx_hostnames,
+            nameservers=nameservers, resolver=resolver,
+            timeout=timeout)
+    except DNSException as error:
+        mx_results = OrderedDict([("hosts", []),
+                                  ("error", error.__str__())])
+    return mx_results
+
+
+def check_dmarc(domain, parked=False,
+                include_dmarc_tag_descriptions=False,
+                nameservers=None, resolver=None, timeout=2.0):
+    dmarc_results = OrderedDict([("record", None), ("valid", True),
+                                 ("location", None)])
+    try:
+        dmarc_query = query_dmarc_record(domain,
+                                         nameservers=nameservers,
+                                         resolver=resolver,
+                                         timeout=timeout)
+        dmarc_results["record"] = dmarc_query["record"]
+        dmarc_results["location"] = dmarc_query["location"]
+        parsed_dmarc_record = parse_dmarc_record(
+            dmarc_query["record"],
+            dmarc_query["location"],
+            parked=parked,
+            include_tag_descriptions=include_dmarc_tag_descriptions,
+            nameservers=nameservers, resolver=resolver,
+            timeout=timeout)
+        dmarc_results["warnings"] = dmarc_query["warnings"]
+
+        dmarc_results["tags"] = parsed_dmarc_record["tags"]
+        dmarc_results["warnings"] += parsed_dmarc_record[
+            "warnings"]
+    except DMARCError as error:
+        dmarc_results["error"] = str(error)
+        dmarc_results["valid"] = False
+        if hasattr(error, "data") and error.data:
+            for key in error.data:
+                dmarc_results[key] = error.data[key]
+    return dmarc_results
+
+
+def check_spf(domain, parked=False, nameservers=None, resolver=None,
+              timeout=2.0):
+    spf_results = OrderedDict(
+        [("record", None), ("valid", True), ("dns_lookups", None),
+         ("dns_void_lookups", None)])
+    try:
+        spf_query = query_spf_record(
+            domain,
+            nameservers=nameservers, resolver=resolver,
+            timeout=timeout)
+        spf_results["record"] = spf_query["record"]
+        spf_results["warnings"] = spf_query["warnings"]
+        parsed_spf = parse_spf_record(spf_results["record"],
+                                      domain,
+                                      parked=parked,
+                                      nameservers=nameservers,
+                                      resolver=resolver,
+                                      timeout=timeout)
+
+        spf_results["dns_lookups"] = parsed_spf[
+            "dns_lookups"]
+        spf_results["dns_void_lookups"] = parsed_spf[
+            "dns_void_lookups"]
+        spf_results["parsed"] = parsed_spf["parsed"]
+        spf_results["warnings"] += parsed_spf["warnings"]
+    except SPFError as error:
+        spf_results["error"] = str(error)
+        del spf_results["dns_lookups"]
+        spf_results["valid"] = False
+        if hasattr(error, "data") and error.data:
+            for key in error.data:
+                spf_results[key] = error.data[key]
+    return spf_results
+
+
 def results_to_json(results):
     """
     Converts a dictionary of results to a JSON string
 
     Args:
         results (dict): A dictionary of results
```

### Comparing `checkdmarc-4.6.0/.gitignore` & `checkdmarc-4.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.6.0/LICENSE` & `checkdmarc-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.6.0/README.md` & `checkdmarc-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.6.0/pyproject.toml` & `checkdmarc-4.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.6.0/PKG-INFO` & `checkdmarc-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkdmarc
-Version: 4.6.0
+Version: 4.7.0
 Summary: A Python module and command line parser for SPF and DMARC records
 Project-URL: Homepage, https://github.com/domainaware/checkdmarc
 Project-URL: Documentation, https://domainaware.github.io/checkdmarc/
 Project-URL: Issues, https://github.com/domainaware/checkdmarc/issues
 Project-URL: Changelog, https://github.com/domainaware/checkdmarc/blob/master/CHANGELOG.md
 Author-email: Sean Whalen <whalenster@gmail.com>
 License-Expression: Apache-2.0
```

