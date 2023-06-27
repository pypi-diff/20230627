# Comparing `tmp/malwoverview-5.2.tar.gz` & `tmp/malwoverview-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malwoverview-5.2.tar", last modified: Tue Jun 20 05:07:40 2023, max compression
+gzip compressed data, was "malwoverview-5.3.tar", last modified: Tue Jun 27 02:19:50 2023, max compression
```

## Comparing `malwoverview-5.2.tar` & `malwoverview-5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.941765 malwoverview-5.2/
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-20 05:02:57.000000 malwoverview-5.2/.malwapi.conf
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-20 05:02:57.000000 malwoverview-5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    34611 2023-06-20 05:07:40.937765 malwoverview-5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34086 2023-06-20 05:04:04.000000 malwoverview-5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.937765 malwoverview-5.2/malwoverview/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:02:57.000000 malwoverview-5.2/malwoverview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)   610320 2023-06-20 05:02:57.000000 malwoverview-5.2/malwoverview/malwoverview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.937765 malwoverview-5.2/malwoverview.egg-info/
--rw-r--r--   0 root         (0) root         (0)    34611 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 05:07:40.941765 malwoverview-5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-20 05:02:57.000000 malwoverview-5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.669625 malwoverview-5.3/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-27 01:55:55.000000 malwoverview-5.3/.malwapi.conf
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-27 01:55:55.000000 malwoverview-5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    35430 2023-06-27 02:19:50.669625 malwoverview-5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34905 2023-06-27 01:57:01.000000 malwoverview-5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.665625 malwoverview-5.3/malwoverview/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 01:55:55.000000 malwoverview-5.3/malwoverview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   612059 2023-06-27 01:55:55.000000 malwoverview-5.3/malwoverview/malwoverview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.669625 malwoverview-5.3/malwoverview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    35430 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 02:19:50.669625 malwoverview-5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-27 01:55:55.000000 malwoverview-5.3/setup.py
```

### Comparing `malwoverview-5.2/LICENSE` & `malwoverview-5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `malwoverview-5.2/PKG-INFO` & `malwoverview-5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: malwoverview
-Version: 5.2
-Summary: Malwoverview is a first response tool for threat hunting.
-Home-page: https://github.com/alexandreborges/malwoverview
-Author: Alexandre Borges
-Author-email: alexandreborges@blackstormsecurity.com
-License: GNU GPL v3.0
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Malwoverview
 
       Copyright (C)  2018-2023 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
 
       This program is free software: you can redistribute it and/or modify
       it under the terms of the GNU General Public License as published by
       the Free Software Foundation, either version 3 of the License, or
@@ -25,15 +11,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.2
+# Current Version: 5.3
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -84,31 +70,45 @@
 
       Alexandre Borges (project owner)
       Corey Forman (https://github.com/digitalsleuth)
       Christian Clauss (https://github.com/cclauss)
 
 # INSTALLATION 
 
-This tool has been tested on REMnux, Ubuntu, Kali Linux and macOS only. Malwoverview 
+This tool has been tested on REMnux, Ubuntu, Kali Linux, macOS and Windows. Malwoverview 
 can be installed by executing the following command:
 
-      * pip3.9 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
+      * pip3.11 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
       
       or...
       
       * python -m pip install -U malwoverview
       
       or...
       
       * git clone https://github.com/alexandreborges/malwoverview
 
-If you are using macOS, so you should install libmagic before installing Malwoverview:
+If you are installing Malwoverview on  macOS, you must execute the following commands:
 
+      * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
       * brew install libmagic
-      * pip3.9 install -U malwoverview
+      * pip install urllib3==1.26.6
+      * pip3 install -U malwoverview
+      * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
+        directory. Example:
+
+          export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
+
+      * Execute: . ./.bash_profile
+
+If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
+installing Malwoverview:
+
+      * python -m pip uninstall python-magic
+      * python -m pip install python-magic-bin 
 
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
@@ -216,49 +216,49 @@
 If you want to perform the manual steps (usually, it is not necessary), so few steps 
 should be executed:
 
 ## REMnux / Ubuntu (manual steps)
 
 1. Python version 3.8 or later (Only Python 3.x !!! It does NOT work using Python 2.7) 
 
-       $ apt-get install python3.9  (for example)
+       $ apt-get install python3.11  (for example)
 
 2. Python-magic.  
 
       To install python-magic package you can execute the following command:
 
-       $ pip3.9 install python-magic
+       $ pip3.11 install python-magic
 
       Or compiling it from the github repository:
 
        $ git clone https://github.com/ahupp/python-magic
        $ cd python-magic/
-       $ python3.9 setup.py build
-       $ python3.9 setup.py install
+       $ python3.11 setup.py build
+       $ python3.11 setup.py install
 
       As there are serious problems about existing two versions of python-magic package, my 
       recommendation is to install it from github (second procedure above) and copy the magic.py 
       file to the SAME directory of malwoverview tool. 
       
 3. Install several Python packages: 
 
-       $ pip3.9 install -r requirements.txt
+       $ pip3.11 install -r requirements.txt
 
        OR
 
-       $ pip3.9 install -U pefile
-       $ pip3.9 install -U colorama
-       $ pip3.9 install -U simplejson
-       $ pip3.9 install -U python-magic
-       $ pip3.9 install -U requests
-       $ pip3.9 install -U validators
-       $ pip3.9 install -U geocoder
-       $ pip3.9 install -U polyswarm-api
-       $ pip3.9 install -U pathlib
-       $ pip3.9 install -U configparser
+       $ pip3.11 install -U pefile
+       $ pip3.11 install -U colorama
+       $ pip3.11 install -U simplejson
+       $ pip3.11 install -U python-magic
+       $ pip3.11 install -U requests
+       $ pip3.11 install -U validators
+       $ pip3.11 install -U geocoder
+       $ pip3.11 install -U polyswarm-api
+       $ pip3.11 install -U pathlib
+       $ pip3.11 install -U configparser
 
 4. To check an Android mobile you need to install the "adb" program by executing the following command:
 
        # apt get install adb
 
    PS: before trying Android's options, check:
 
@@ -373,14 +373,22 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.3:
+
+      This version:
+
+            * Fixes issues related to Malshare (-l and -L options).
+            * Adds a new Malshare option (-l 7) to list all samples 
+              from last 24 hours.
+
 Version 5.2:
 
       This version:
 
             * Multiple issues related to Hybrid Analysis have been fixed.
 
 Version 5.1.1:
```

### Comparing `malwoverview-5.2/README.md` & `malwoverview-5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: malwoverview
+Version: 5.3
+Summary: Malwoverview is a first response tool for threat hunting.
+Home-page: https://github.com/alexandreborges/malwoverview
+Author: Alexandre Borges
+Author-email: alexandreborges@blackstormsecurity.com
+License: GNU GPL v3.0
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Malwoverview
 
       Copyright (C)  2018-2023 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
 
       This program is free software: you can redistribute it and/or modify
       it under the terms of the GNU General Public License as published by
       the Free Software Foundation, either version 3 of the License, or
@@ -11,15 +25,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.2
+# Current Version: 5.3
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -70,31 +84,45 @@
 
       Alexandre Borges (project owner)
       Corey Forman (https://github.com/digitalsleuth)
       Christian Clauss (https://github.com/cclauss)
 
 # INSTALLATION 
 
-This tool has been tested on REMnux, Ubuntu, Kali Linux and macOS only. Malwoverview 
+This tool has been tested on REMnux, Ubuntu, Kali Linux, macOS and Windows. Malwoverview 
 can be installed by executing the following command:
 
-      * pip3.9 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
+      * pip3.11 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
       
       or...
       
       * python -m pip install -U malwoverview
       
       or...
       
       * git clone https://github.com/alexandreborges/malwoverview
 
-If you are using macOS, so you should install libmagic before installing Malwoverview:
+If you are installing Malwoverview on  macOS, you must execute the following commands:
 
+      * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
       * brew install libmagic
-      * pip3.9 install -U malwoverview
+      * pip install urllib3==1.26.6
+      * pip3 install -U malwoverview
+      * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
+        directory. Example:
+
+          export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
+
+      * Execute: . ./.bash_profile
+
+If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
+installing Malwoverview:
+
+      * python -m pip uninstall python-magic
+      * python -m pip install python-magic-bin 
 
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
@@ -202,49 +230,49 @@
 If you want to perform the manual steps (usually, it is not necessary), so few steps 
 should be executed:
 
 ## REMnux / Ubuntu (manual steps)
 
 1. Python version 3.8 or later (Only Python 3.x !!! It does NOT work using Python 2.7) 
 
-       $ apt-get install python3.9  (for example)
+       $ apt-get install python3.11  (for example)
 
 2. Python-magic.  
 
       To install python-magic package you can execute the following command:
 
-       $ pip3.9 install python-magic
+       $ pip3.11 install python-magic
 
       Or compiling it from the github repository:
 
        $ git clone https://github.com/ahupp/python-magic
        $ cd python-magic/
-       $ python3.9 setup.py build
-       $ python3.9 setup.py install
+       $ python3.11 setup.py build
+       $ python3.11 setup.py install
 
       As there are serious problems about existing two versions of python-magic package, my 
       recommendation is to install it from github (second procedure above) and copy the magic.py 
       file to the SAME directory of malwoverview tool. 
       
 3. Install several Python packages: 
 
-       $ pip3.9 install -r requirements.txt
+       $ pip3.11 install -r requirements.txt
 
        OR
 
-       $ pip3.9 install -U pefile
-       $ pip3.9 install -U colorama
-       $ pip3.9 install -U simplejson
-       $ pip3.9 install -U python-magic
-       $ pip3.9 install -U requests
-       $ pip3.9 install -U validators
-       $ pip3.9 install -U geocoder
-       $ pip3.9 install -U polyswarm-api
-       $ pip3.9 install -U pathlib
-       $ pip3.9 install -U configparser
+       $ pip3.11 install -U pefile
+       $ pip3.11 install -U colorama
+       $ pip3.11 install -U simplejson
+       $ pip3.11 install -U python-magic
+       $ pip3.11 install -U requests
+       $ pip3.11 install -U validators
+       $ pip3.11 install -U geocoder
+       $ pip3.11 install -U polyswarm-api
+       $ pip3.11 install -U pathlib
+       $ pip3.11 install -U configparser
 
 4. To check an Android mobile you need to install the "adb" program by executing the following command:
 
        # apt get install adb
 
    PS: before trying Android's options, check:
 
@@ -359,14 +387,22 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.3:
+
+      This version:
+
+            * Fixes issues related to Malshare (-l and -L options).
+            * Adds a new Malshare option (-l 7) to list all samples 
+              from last 24 hours.
+
 Version 5.2:
 
       This version:
 
             * Multiple issues related to Hybrid Analysis have been fixed.
 
 Version 5.1.1:
```

### Comparing `malwoverview-5.2/malwoverview/malwoverview.py` & `malwoverview-5.3/malwoverview/malwoverview.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #CONTRIBUTORS
 
 # Alexandre Borges (project owner)
 # Corey Forman (https://github.com/digitalsleuth)
 # Christian Clauss (https://github.com/cclauss)
 
-# Malwoverview.py: version 5.2
+# Malwoverview.py: version 5.3
 
 import os
 import sys
 import re
 import pefile
 import peutils
 import magic
@@ -58,15 +58,15 @@
 from requests import Request, Session, exceptions
 
 # On Windows systems, it is necessary to install python-magic-bin: pip install python-magic-bin
 
 __author__ = "Alexandre Borges"
 __copyright__ = "Copyright 2018-2021, Alexandre Borges"
 __license__ = "GNU General Public License v3.0"
-__version__ = "5.2"
+__version__ = "5.3"
 __email__ = "alexandreborges at blackstormsecurity.com"
 
 haurl = 'https://www.hybrid-analysis.com/api/v2'
 urlfilevt3 = 'https://www.virustotal.com/api/v3/files'
 urlurlvt3 = 'https://www.virustotal.com/api/v3/urls'
 urlipvt3 = 'https://www.virustotal.com/api/v3/ip_addresses'
 urldomainvt3 = 'https://www.virustotal.com/api/v3/domains'
@@ -3109,18 +3109,19 @@
 
         resource = filehash
         requestsession3 = requests.Session( )
         finalurl3 = ''.join([urlmalshare, MALSHAREAPI, '&action=getfile&hash=', resource])
         malresponse3 = requestsession3.get(url=finalurl3, allow_redirects=True)
         if (b'Sample not found by hash' in malresponse3.content):
             if(bkg == 1):
-                print((mycolors.foreground.lightred + "\nSample not found by the given hash.\n"))
+                print((mycolors.foreground.lightred + "\nSample not found by the provided hash.\n"))
             else:
-                print((mycolors.foreground.red + "\nSample not found by the given hash.\n"))
-                exit(1)
+                print((mycolors.foreground.red + "\nSample not found by the provided hash.\n"))
+            print(mycolors.reset)
+            exit(1)
 
         open(resource, 'wb').write(malresponse3.content)
 
         print("\n")
         print((mycolors.reset + "MALWARE SAMPLE SAVED! "))
         print((mycolors.reset))
 
@@ -3198,40 +3199,74 @@
         filetype = 'PE32'
     elif (maltype == 3):
         filetype = 'ELF'
     elif (maltype == 4):
         filetype = 'Java'
     elif (maltype == 5):
         filetype = 'PDF'
+    elif (maltype == 5):
+        filetype = 'PDF'
+    elif (maltype == 6):
+        filetype = 'PDF'
     else:
-        filetype = 'Composite'
+        filetype = 'all'
 
     try:
 
-        print("\n")
-        print((mycolors.reset + "SHA256 hash".center(75)), end='')
-        print((mycolors.reset + "MD5 hash".center(38)), end='')
-        print((mycolors.reset + "File type".center(8)), end='')
-        print("\n" + (126*'-').center(59))
-        print((mycolors.reset))
+        if (filetype != "all"):
+            print("\n")
+            print((mycolors.reset + "SHA256 hash".center(75)), end='')
+            print((mycolors.reset + "MD5 hash".center(38)), end='')
+            print((mycolors.reset + "File type".center(8)), end='')
+            print("\n" + (126*'-').center(59))
+            print((mycolors.reset))
 
-        requestsession = requests.Session( )
-        requestsession.headers.update({'accept': 'application/json'})
-        finalurl = ''.join([urlmalshare, MALSHAREAPI, '&action=type&type=', filetype])
-        malresponse = requestsession.get(url=finalurl)
-        maltext = json.loads(malresponse.text)
+            requestsession = requests.Session( )
+            requestsession.headers.update({'accept': 'application/json'})
+            finalurl = ''.join([urlmalshare, MALSHAREAPI, '&action=type&type=', filetype])
+            malresponse = requestsession.get(url=finalurl)
+            maltext = json.loads(malresponse.text)
+        
+        if (filetype == "all"):
+            print("\n")
+            print((mycolors.reset + "SHA256 hash".center(75)), end='')
+            print((mycolors.reset + "MD5 hash".center(38)), end='')
+            print("\n" + (112*'-').center(56))
+            print((mycolors.reset))
+
+            requestsession = requests.Session( )
+            requestsession.headers.update({'accept': 'application/json'})
+            finalurl = ''.join([urlmalshare, MALSHAREAPI, '&action=getlist'])
+            malresponse = requestsession.get(url=finalurl)
+            maltext = json.loads(malresponse.text)
 
-        if ((maltext)):
+        if ((maltext) and filetype!="all"):
             try:
                 for i in range(0, len(maltext)):
                     if (maltext[i].get('sha256')):
                         if (bkg == 1):
                             print((mycolors.reset + "sha256: " + mycolors.foreground.yellow + "%s" % maltext[i]['sha256'] + mycolors.reset + "  md5: " + mycolors.foreground.lightcyan + "%s" % maltext[i]['md5'] + mycolors.reset + "  type: " + mycolors.foreground.lightred + "%s" % filetype))
                         else:
                             print((mycolors.reset + "sha256: " + mycolors.foreground.red + "%s" % maltext[i]['sha256'] + mycolors.reset + "  md5: " + mycolors.foreground.blue + "%s" % maltext[i]['md5'] + mycolors.reset + "   type: " + mycolors.foreground.purple + "%s" % filetype))
+            
+            except KeyError as e:
+                pass
+
+            except (BrokenPipeError, IOError):
+                print(mycolors.reset, file=sys.stderr)
+                exit(1)
+
+        if ((maltext) and filetype=="all"):
+            try:
+                for i in range(0, len(maltext)):
+                    if (maltext[i].get('sha256')):
+                        if (bkg == 1):
+                            print((mycolors.reset + "sha256: " + mycolors.foreground.yellow + "%s" % maltext[i]['sha256'] + mycolors.reset + "  md5: " + mycolors.foreground.lightcyan + "%s" % maltext[i]['md5'] + mycolors.reset))
+                        else:
+                            print((mycolors.reset + "sha256: " + mycolors.foreground.red + "%s" % maltext[i]['sha256'] + mycolors.reset + "  md5: " + mycolors.foreground.blue + "%s" % maltext[i]['md5'] + mycolors.reset))
 
             except KeyError as e:
                 pass
 
             except (BrokenPipeError, IOError):
                 print(mycolors.reset, file=sys.stderr)
                 exit(1)
@@ -10326,24 +10361,24 @@
     bazaararg = ''
     triage = 0
     triagearg = ''
     virustotalarg = ''
     ipaddrvtx = ''
     ffpname = ''
 
-    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.2", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-6> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
+    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.3", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-7> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
     parser.add_argument('-c', '--config', dest='config', type=str, metavar = "CONFIG FILE", default = (USER_HOME_DIR + '.malwapi.conf'), help='Use a custom config file to specify API\'s.')
     parser.add_argument('-d', '--directory', dest='direct',type=str, metavar = "DIRECTORY", help='Specifies the directory containing malware samples to be checked against VIRUS TOTAL. Use the option -D to decide whether you are being using a public VT API or a Premium VT API.')
     parser.add_argument('-o', '--background', dest='backg', type=int,default = 1, metavar = "BACKGROUND", help='Adapts the output colors to a light background color terminal. The default is dark background color terminal.')
     parser.add_argument('-v', '--virustotal_option', dest='virustotaloption', type=int,default = 0, metavar = "VIRUSTOTAL", help='-v 1: given a file using -V option, it queries the VIRUS TOTAL database (API v.3) to get the report for the given file through -V option.; -v 2: it shows an antivirus report for a given file using -V option (API v.3); -v 3: equal to -v2, but the binary\'s IAT and EAT are also shown (API v.3); -v 4: it extracts the overlay; -v 5: submits an URL to VT scanning; -v 6: submits an IP address to Virus Total; -v 7: this options gets a report on the provided domain from Virus Total; -v 8: verifies a given hash against Virus Total; -v 9: submits a sample to VT (up to 32 MB). Use forward slash to specify the target file on Windows systems. Demands passing sample file with -V option; -v 10: verifies hashes from a provided file through option -V. This option uses public VT API v.3; -v 11: verifies hashes from a provided file through option -V. This option uses Premium API v.3; -v 12: it shows behaviour information of a sample given a hash through option -V. This option uses VT API v.3; -v 13: it submits LARGE files (above 32 MB) to VT using API v.3;')
     parser.add_argument('-V', '--virustotal_arg', dest='virustotalarg', type=str, metavar = "VIRUSTOTAL_ARG", help='Provides arguments for -v option.')
     parser.add_argument('-a', '--hybrid_option', dest='haoption', type=int,default = 0, metavar = "HYBRID_ANALYSIS", help='This parameter fetches reports from HYBRID ANALYSIS, download samples and submits samples to be analyzed. The possible values are: 1: gets a report for a given hash or sample from a Windows 7 32-bit environment; 2: gets a report for a given hash or sample from a Windows 7 32-bit environment (HWP Support); 3: gets a report for given hash or sample from a Windows 64-bit environment; 4: gets a report for a given hash or sample from an Android environment; 5: gets a report for a given hash or sample from a Linux 64-bit environment; 6: submits a sample to Windows 7 32-bit environment; 7. submits a sample to Windows 7 32-bit environment with HWP support environment; 8. submits a sample to Windows 7 64-bit environment ; 9. submits a sample to an Android environment ; 10. submits a sample to a Linux 64-bit environment; 11. downloads a sample from a Windows 7 32-bit environment; 12. downloads a sample from a Windows 7 32-bit HWP environment; 13. downloads a sample from a Windows 7 64-bit environment; 14. downloads a sample from an Android environment; 15. downloads a sample from a Linux 64-bit environment.')
     parser.add_argument('-A', '--ha_arg', dest='haarg', type=str, metavar = "SUBMIT_HA", help='Provides an argument for -a option from HYBRID ANALYSIS.')
     parser.add_argument('-D', '--vtpubpremium', dest='vtpubpremium', type=int,default = 0, metavar = "VT_PUBLIC_PREMIUM", help='This option must be used with -d option. Possible values: <0> it uses the Premium VT API v3 (default); <1> it uses the Public VT API v3.')
-    parser.add_argument('-l', '--malsharelist', dest='malsharelist', type=int,default = 0, metavar = "MALSHARE_HASHES", help='This option performs download a sample and shows hashes of a specific type from the last 24 hours from MALSHARE repository. Possible values are: 1: Download a sample; 2: PE32 (default) ; 3: ELF ; 4: Java; 5: PDF ; 6: Composite(OLE).')
+    parser.add_argument('-l', '--malsharelist', dest='malsharelist', type=int,default = 0, metavar = "MALSHARE_HASHES", help='This option performs download a sample and shows hashes of a specific type from the last 24 hours from MALSHARE repository. Possible values are: 1: Download a sample; 2: PE32 (default) ; 3: ELF ; 4: Java; 5: PDF ; 6: Composite(OLE); 7: List of hashes from past 24 hours.')
     parser.add_argument('-L', '--malshare_hash', dest='malsharehash', type=str, metavar = "MALSHARE_HASH_SEARCH", help='Provides a hash as argument for downloading a sample from MALSHARE repository.')
     parser.add_argument('-j', '--haus_option', dest='hausoption', type=int, default = 0,  metavar = "HAUS_OPTION", help='This option fetches information from URLHaus depending of the value passed as argument: 1: performs download of the given sample; 2: queries information about a provided hash ; 3: searches information about a given URL; 4: searches a malicious URL by a given tag (case sensitive); 5: searches for payloads given a tag; 6: retrives a list of downloadable links to recent payloads; 7: retrives a list of recent malicious URLs.')
     parser.add_argument('-J', '--haus_arg', dest='hausarg', type=str, metavar = "HAUS_ARG", help='Provides argument to -j option from URLHaus.')
     parser.add_argument('-p', '--poly_option', dest='polyoption', type=int,default = 0, metavar = "POLY_OPTION", help='(Only for Linux) This option is related to POLYSWARM operations: 1. searches information related to a given hash provided using -P option; 2. submits a sample provided by -P option to be analyzed by Polyswarm engine ; 3. Downloads a sample from Polyswarm by providing the hash throught option -P .Attention: Polyswarm enforces a maximum of 20 samples per month; 4. searches for similar samples given a sample file thought option -P; 5. searches for samples related to a provided IP address through option -P; 6. searches for samples related to a given domain provided by option -P; 7. searches for samples related to a provided URL throught option -P; 8. searches for samples related to a provided malware family given by option -P.')
     parser.add_argument('-P', '--poly_arg', dest='polyarg', type=str, metavar = "POLYSWARM_ARG", help='(Only for Linux) Provides an argument for -p option from POLYSWARM.')
     parser.add_argument('-y', '--android_option', dest='androidoption', type=int, default = 0, metavar = "ANDROID_OPTION", help='This ANDROID option has multiple possible values: <1>: Check all third-party APK packages from the USB-connected Android device against Hybrid Analysis using multithreads. Notes: the Android device does not need to be rooted and the system does need to have the adb tool in the PATH environment variable; <2>: Check all third-party APK packages from the USB-connected Android device against VirusTotal using Public API (slower because of 60 seconds delay for each 4 hashes). Notes: the Android device does not need to be rooted and the system does need to have adb tool in the PATH environment variable; <3>: Check all third-party APK packages from the USB-connected Android device against VirusTotal using multithreads (only for Private Virus API). Notes: the Android device does not need to be rooted and the system needs to have adb tool in the PATH environment variable; <4> Sends an third-party APK from your USB-connected Android device to Hybrid Analysis; 5. Sends an third-party APK from your USB-connected Android device to Virus-Total.')
     parser.add_argument('-Y', '--android_arg', dest='androidarg', type=str, metavar = "ANDROID_ARG", help='This option provides the argument for -y from ANDROID.')
@@ -10569,15 +10604,15 @@
         exit(0)
 
     if (args.backg) not in optval:
         parser.print_help()
         print(mycolors.reset)
         sys.exit(0)
 
-    if (args.malsharelist) not in optval3:
+    if (args.malsharelist) not in optval8:
         parser.print_help()
         print(mycolors.reset)
         sys.exit(0)
 
     if (Q == 1):
         if ((virustotaloptionx == 0) and (haoptionx == 0)):
             parser.print_help()
```

### Comparing `malwoverview-5.2/malwoverview.egg-info/PKG-INFO` & `malwoverview-5.3/malwoverview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malwoverview
-Version: 5.2
+Version: 5.3
 Summary: Malwoverview is a first response tool for threat hunting.
 Home-page: https://github.com/alexandreborges/malwoverview
 Author: Alexandre Borges
 Author-email: alexandreborges@blackstormsecurity.com
 License: GNU GPL v3.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,15 +25,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.2
+# Current Version: 5.3
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -84,31 +84,45 @@
 
       Alexandre Borges (project owner)
       Corey Forman (https://github.com/digitalsleuth)
       Christian Clauss (https://github.com/cclauss)
 
 # INSTALLATION 
 
-This tool has been tested on REMnux, Ubuntu, Kali Linux and macOS only. Malwoverview 
+This tool has been tested on REMnux, Ubuntu, Kali Linux, macOS and Windows. Malwoverview 
 can be installed by executing the following command:
 
-      * pip3.9 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
+      * pip3.11 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
       
       or...
       
       * python -m pip install -U malwoverview
       
       or...
       
       * git clone https://github.com/alexandreborges/malwoverview
 
-If you are using macOS, so you should install libmagic before installing Malwoverview:
+If you are installing Malwoverview on  macOS, you must execute the following commands:
 
+      * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
       * brew install libmagic
-      * pip3.9 install -U malwoverview
+      * pip install urllib3==1.26.6
+      * pip3 install -U malwoverview
+      * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
+        directory. Example:
+
+          export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
+
+      * Execute: . ./.bash_profile
+
+If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
+installing Malwoverview:
+
+      * python -m pip uninstall python-magic
+      * python -m pip install python-magic-bin 
 
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
@@ -216,49 +230,49 @@
 If you want to perform the manual steps (usually, it is not necessary), so few steps 
 should be executed:
 
 ## REMnux / Ubuntu (manual steps)
 
 1. Python version 3.8 or later (Only Python 3.x !!! It does NOT work using Python 2.7) 
 
-       $ apt-get install python3.9  (for example)
+       $ apt-get install python3.11  (for example)
 
 2. Python-magic.  
 
       To install python-magic package you can execute the following command:
 
-       $ pip3.9 install python-magic
+       $ pip3.11 install python-magic
 
       Or compiling it from the github repository:
 
        $ git clone https://github.com/ahupp/python-magic
        $ cd python-magic/
-       $ python3.9 setup.py build
-       $ python3.9 setup.py install
+       $ python3.11 setup.py build
+       $ python3.11 setup.py install
 
       As there are serious problems about existing two versions of python-magic package, my 
       recommendation is to install it from github (second procedure above) and copy the magic.py 
       file to the SAME directory of malwoverview tool. 
       
 3. Install several Python packages: 
 
-       $ pip3.9 install -r requirements.txt
+       $ pip3.11 install -r requirements.txt
 
        OR
 
-       $ pip3.9 install -U pefile
-       $ pip3.9 install -U colorama
-       $ pip3.9 install -U simplejson
-       $ pip3.9 install -U python-magic
-       $ pip3.9 install -U requests
-       $ pip3.9 install -U validators
-       $ pip3.9 install -U geocoder
-       $ pip3.9 install -U polyswarm-api
-       $ pip3.9 install -U pathlib
-       $ pip3.9 install -U configparser
+       $ pip3.11 install -U pefile
+       $ pip3.11 install -U colorama
+       $ pip3.11 install -U simplejson
+       $ pip3.11 install -U python-magic
+       $ pip3.11 install -U requests
+       $ pip3.11 install -U validators
+       $ pip3.11 install -U geocoder
+       $ pip3.11 install -U polyswarm-api
+       $ pip3.11 install -U pathlib
+       $ pip3.11 install -U configparser
 
 4. To check an Android mobile you need to install the "adb" program by executing the following command:
 
        # apt get install adb
 
    PS: before trying Android's options, check:
 
@@ -373,14 +387,22 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.3:
+
+      This version:
+
+            * Fixes issues related to Malshare (-l and -L options).
+            * Adds a new Malshare option (-l 7) to list all samples 
+              from last 24 hours.
+
 Version 5.2:
 
       This version:
 
             * Multiple issues related to Hybrid Analysis have been fixed.
 
 Version 5.1.1:
```

### Comparing `malwoverview-5.2/setup.py` & `malwoverview-5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 USER_HOME_DIR = str(Path.home()) + os.sep
 
 with open("README.md", encoding='utf8') as readme:
     long_description = readme.read()
 
 setup(
     name="malwoverview",
-    version="5.2",
+    version="5.3",
     author="Alexandre Borges",
     author_email="alexandreborges@blackstormsecurity.com",
     license="GNU GPL v3.0",
     url="https://github.com/alexandreborges/malwoverview",
     description=("Malwoverview is a first response tool for threat hunting."),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

