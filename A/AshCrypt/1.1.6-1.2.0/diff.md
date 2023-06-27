# Comparing `tmp/AshCrypt-1.1.6.tar.gz` & `tmp/AshCrypt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.1.6.tar", last modified: Sun Jun 18 16:05:00 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.0.tar", last modified: Tue Jun 27 16:08:10 2023, max compression
```

## Comparing `AshCrypt-1.1.6.tar` & `AshCrypt-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.145609 AshCrypt-1.1.6/
-drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.041630 AshCrypt-1.1.6/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0     4407 2023-06-18 16:01:05.000000 AshCrypt-1.1.6/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     3001 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     6000 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    14610 2023-06-18 15:58:49.000000 AshCrypt-1.1.6/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.064401 AshCrypt-1.1.6/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15529 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.1.6/LICENSE
--rw-rw-rw-   0        0        0    15529 2023-06-18 16:05:00.144600 AshCrypt-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    17580 2023-06-18 15:58:49.000000 AshCrypt-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 16:05:00.146604 AshCrypt-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-06-18 16:04:28.000000 AshCrypt-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.136233 AshCrypt-1.1.6/unittestsAC/
--rw-rw-rw-   0        0        0       25 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/unittestsAC/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/unittestsAC/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.045924 AshCrypt-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-27 16:08:09.973736 AshCrypt-1.2.0/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    34125 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     8855 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     4128 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     6450 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    14164 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.028504 AshCrypt-1.2.0/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6435 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/Ash.cpython-310.pyc
+-rw-rw-rw-   0        0        0    19153 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshCryptGUI.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7808 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshDatabase.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3515 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshFileCrypt.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2650 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/AshTextCrypt.cpython-310.pyc
+-rw-rw-rw-   0        0        0      248 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1294 2023-06-27 15:57:46.000000 AshCrypt-1.2.0/AshCrypt/__pycache__/qr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.2.0/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:08:10.037808 AshCrypt-1.2.0/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:08:09.998617 AshCrypt-1.2.0/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15187 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 16:08:09.000000 AshCrypt-1.2.0/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    15187 2023-06-27 16:08:10.043934 AshCrypt-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17100 2023-06-27 15:57:29.000000 AshCrypt-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:08:10.046925 AshCrypt-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-27 16:06:57.000000 AshCrypt-1.2.0/setup.py
```

### Comparing `AshCrypt-1.1.6/AshCrypt/Ash.py` & `AshCrypt-1.2.0/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.6/AshCrypt/AshDatabase.py` & `AshCrypt-1.2.0/AshCrypt/AshDatabase.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,65 +39,67 @@
     def default_routing(self):
         return (f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"')
 
     def query(self, *querys: str) -> list:
         result = []
         for i, query in enumerate(querys):
             if not isinstance(query, str):
-                result.append({f'query{i+1}': (0.0, TypeError)})
+                result.append({f'query {i}': (0.0, TypeError)})
             try:
                 with self.conn:
                     self.c.execute(query)
                     if self.c.rowcount == 1:
-                        result.append({f'query{i+1}': self.c.fetchone()})
+                        result.append({f'query {i}': ['SUCCESS',self.c.fetchone()]})
                     else:
-                        result.append({f'query{i+1}': self.c.fetchall()})
+                        result.append({f'query {i}': ['SUCCESS',self.c.fetchall()]})
 
             except sqlite3.Error as e:
-                result.append({f'query{i+1}': (0, e)})
+                result.append({f'query {i}': ('FAILURE', e.__str__())})
         return result
 
     def addtable(self, optional_tablename=None):
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f"CREATE TABLE IF NOT EXISTS {self.tablename} "
-                                   "(ID INTEGER PRIMARY KEY,Content BLOB ,Key TEXT )")
+                                   "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
                 return 11
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
                     self.c.execute(f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
                                    "(ID INTEGER PRIMARY KEY,"
+                                   "Name TEXT ,"
                                    "Content BLOB ,"
-                                   " Key TEXT )")
+                                   "Key TEXT )")
                     self.tablename = optional_tablename
                 return 1
 
             except sqlite3.Error as e:
                 return (0, e)
 
-    def insert(self, content, key, optional_table_name=None):
+    def insert(self, name , content, key, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
-                    self.c.execute(f"INSERT INTO {self.tablename} (Content ,Key) VALUES (? , ?) ", (content, key))
+                    self.c.execute(f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) "
+                                   , (name,content,key))
 
                 return 11
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f"INSERT INTO {optional_table_name} (Content ,Key) VALUES (? , ?) ",
-                                   (content, key))
+                    self.c.execute(f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
+                                   (name,content,key))
                 return 1
             except sqlite3.Error as e:
                 return (0, e)
 
     def update(self, column_name: str, new_column_val: str, ID: int, optional_table_name=None):
         if optional_table_name is None:
             try:
@@ -136,14 +138,35 @@
                     self.c.execute(f'SELECT * FROM {optional_tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return (0, e)
 
+    def content_by_id(self, id : int ,optional_tablename=None):
+        if optional_tablename is None:
+            try:
+                with self.conn:
+                    self.c.execute(f'SELECT * FROM {self.tablename} WHERE ID = ? ',(id,))
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return (0.0, e)
+
+        else:
+            try:
+                with self.conn:
+                    self.c.execute(f'SELECT * FROM {optional_tablename} WHERE ID = ? ',(id,))
+                    for row in self.c.fetchall():
+                        yield row
+
+            except sqlite3.Error as e:
+                return (0, e)
+
     def show_contents(self, *optional_tablenames):
         if optional_tablenames:
             try:
                 for arg in optional_tablenames:
                     with self.conn:
                         self.c.execute(f'SELECT * FROM {arg} ')
                         for row in self.c.fetchall():
@@ -218,16 +241,19 @@
                     self.c.execute(f'DELETE FROM {optional_table_name} WHERE ID = {ID}')
                 return 1
 
             except sqlite3.Error as e:
                 return (0, e)
 
 if __name__ == '__main__':
-    conn = Database('test.db')
+    conn = Database('post_test.db')
     conn.addtable()
-    key = '#5482A'
-    conn.insert('some encrypted content of bytes or strings',key)
+
+    key = '#5482AF'
+    conn.insert('My Accounts','some encrypted content of bytes or strings',key)
     for e in conn.show_tables():
         print(e)
     print(conn.size)
-    query1 = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
-    print(conn.query(query1))
+    query1 = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482AF" ORDER BY cc DESC '
+    print(conn.query(query1))
+
+
```

### Comparing `AshCrypt-1.1.6/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.2.0/AshCrypt/AshFileCrypt.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,83 +5,109 @@
     def __init__(self):
         self.display = 'Key must be 512 Bit long !'
         super().__init__(self.display)
 
 class CryptFile():
     def __init__(self,filename,key):
         self.filename = filename
+        self.not_512_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
-            raise KeyError()
+            self.not_512_bit_key = 1  # Raise KeyError()
 
     @staticmethod
     def genkey() -> str:
         return Ash.Enc.genMainkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
-        if isinstance(key, str):
-            a = bytes.fromhex(key.strip())
-            if len(a) == 64:
-                return 1
-            else:
-                return 0
-        else:
+        try:
+            if isinstance(key, str):
+                a = bytes.fromhex(key.strip())
+                if len(a) == 64:
+                    return 1
+                else:
+                    return 0
+        except:
             return 2
-    def encrypt(self) -> int :
-        try :
+
+    def encrypt(self) -> int:
+        if os.path.isdir(self.filename):
+            return  7
+        if self.not_512_bit_key == 1:
+            return 5
+        try:
+            go_ahead_rename_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
-            else :
-                with open(self.filename, 'rb') as f:
-                    filecontent = f.read()
-                with open(self.filename, 'wb') as f:
-                    if filecontent:
-                        try:
-                            ins = Ash.Enc(message=filecontent,mainkey=self.key)
-                            new_content= ins.encToBytes()
-                            f.write(new_content)
-                            return 1
-                        except:
+            else:
+                if os.path.splitext(self.filename)[1] == '.crypt':
+                    return 6
+                else:
+                    with open(self.filename, 'rb') as f:
+                        filecontent = f.read()
+                    with open(self.filename, 'wb') as f:
+                        if filecontent:
+                            try:
+                                ins = Ash.Enc(message=filecontent, mainkey=self.key)
+                                new_content = ins.encToBytes()
+                                f.write(new_content)
+                                go_ahead_rename_crypt = 1
+                            except:
+                                f.write(filecontent)
+                                return 0
+                        else:
                             f.write(filecontent)
-                            return 0
-                    else:
-                        f.write(filecontent)
-                        return 2
-        except Exception :
+                            return 2
+                    if go_ahead_rename_crypt == 1:
+                        os.rename(self.filename, self.filename + '.crypt')
+                        return 1
+        except Exception:
             return 4
-    def decrypt(self) -> int :
-        try :
+
+    def decrypt(self) -> int:
+        if os.path.isdir(self.filename):
+            return  7
+        if self.not_512_bit_key == 1:
+            return 5
+        try:
+            go_ahead_remove_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
-            else :
-                with open(self.filename, 'rb') as f:
-                    enc_content = f.read()
-                if enc_content:
+            else:
+                if os.path.splitext(self.filename)[1] != '.crypt':
+                    return 6
+                else:
+                    with open(self.filename, 'rb') as f:
+                        enc_content = f.read()
                     with open(self.filename, 'wb') as f:
-                        try:
-                            ins = Ash.Dec(message=enc_content,mainkey=self.key)
-                            a = ins.decToBytes()
-                            f.write(a)
-                            return 1
-                        except Exception:
+                        if enc_content:
+                            try:
+                                ins = Ash.Dec(message=enc_content, mainkey=self.key)
+                                a = ins.decToBytes()
+                                f.write(a)
+                                go_ahead_remove_crypt = 1
+                            except Exception:
+                                f.write(enc_content)
+                                return 0
+                        else:
                             f.write(enc_content)
-                            return 0
-                else:
-                    f.write(enc_content)
-                    return 2
-        except Exception :
+                            return 2
+                    if go_ahead_remove_crypt == 1:
+                        os.rename(self.filename, os.path.splitext(self.filename)[0])
+                        return 1
+        except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
     def __repr__(self):
         return f'{self.__class__.__name__}({self.filename},{self.key})'
 
 if __name__ == '__main__':
     print(CryptFile.genkey())
     key = 'd5d717f57933ad21725888d3451a9cd7a565dfda677fe92fd8ff9e9c3a36d1496af58c17de2b77d4d3ea6d8791b27350fea0af3ad2610d38c8cb12a29fda4bcf'
-    target = CryptFile('myfile.txt',key)  # if the file is in the current working directory
+    target = CryptFile('hello.txt.crypt',key)
     print(target.decrypt())
```

### Comparing `AshCrypt-1.1.6/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.2.0/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.6/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.0/AshCrypt/CliCrypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -155,16 +155,22 @@
             if a == 2:
                 print('Cannot decrypt the file  when it is already empty')
             if a == 3:
                 print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
                 print('Error in the decryption process. Check if the the file is distorted or it might just be '
                       'decrypted already')
-            elif a == 4 :
+            if a == 4 :
                 print('Unknown Error has occurred\n')
+            if a == 5 :
+                print('ERROR : Key is Not 512-bit')
+            if a == 6:
+                print('ERROR : File is already decrypted')
+            elif a == 7:
+                print('ERROR : Given a directory instead of a file')
 
 
 def file_enc():
     keysetup()
     while file_encFlag :
         print()
         global key
@@ -179,16 +185,21 @@
             if a == 1:
                 print('File successfully encrypted ')
             if a == 2:
                 print('Cannot encrypt the file  when it is already empty')
             if a == 3:
                 print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
-                print('Error in the encryption process. Check if the the file is distorted or it might just be '
-                      'encrypted already')
+                print('Error in the encryption process. Check if the the file is distorted')
             elif a == 4 :
                 print('Unknown Error has occurred\n')
+            if a == 5 :
+                print('ERROR : Key is Not 512-bit')
+            if a == 6:
+                print('ERROR : File is already encrypted')
+            elif a == 7:
+                print('ERROR : Given a directory instead of a file')
 
 
 
 if __name__ == '__main__':
     intro()
```

### Comparing `AshCrypt-1.1.6/AshCrypt/README.md` & `AshCrypt-1.2.0/AshCrypt/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -179,28 +179,18 @@
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ## AshCryptGUI ##
-This is merely a GUI to encrypt and decrypt a text of a maximum of 200 characters and also display the qr representation of the text (encrypted/decrypted) .
+This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
 
-Run the command
-```bash
-python -m AshCryptGUI
-```
-
-**NOTE** : The key is not specified in the GUI its hard-coded, if you want to change the key make sure to change it from within the file `AshCryptGUI.py` itself, it's just a security measure. By default it uses the following key in bytes :
-```python
-import ttkbootstrap as tk
-from AshTextCrypt import *
-import qr
-
-key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
+```shell
+python -m AshCrypt.AshCryptGUI
 ```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
```

### Comparing `AshCrypt-1.1.6/AshCrypt/qr.py` & `AshCrypt-1.2.0/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.6/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.0/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.6
+Version: 1.2.0
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cryptography Library : AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
@@ -200,28 +202,18 @@
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ## AshCryptGUI ##
-This is merely a GUI to encrypt and decrypt a text of a maximum of 200 characters and also display the qr representation of the text (encrypted/decrypted) .
+This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
 
-Run the command
-```bash
-python -m AshCryptGUI
-```
-
-**NOTE** : The key is not specified in the GUI its hard-coded, if you want to change the key make sure to change it from within the file `AshCryptGUI.py` itself, it's just a security measure. By default it uses the following key in bytes :
-```python
-import ttkbootstrap as tk
-from AshTextCrypt import *
-import qr
-
-key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
+```shell
+python -m AshCrypt.AshCryptGUI
 ```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
```

### Comparing `AshCrypt-1.1.6/LICENSE` & `AshCrypt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.6/PKG-INFO` & `AshCrypt-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.6
+Version: 1.2.0
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cryptography Library : AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
@@ -200,28 +202,18 @@
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ## AshCryptGUI ##
-This is merely a GUI to encrypt and decrypt a text of a maximum of 200 characters and also display the qr representation of the text (encrypted/decrypted) .
+This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution. run this command and see for yourself !
 
-Run the command
-```bash
-python -m AshCryptGUI
-```
-
-**NOTE** : The key is not specified in the GUI its hard-coded, if you want to change the key make sure to change it from within the file `AshCryptGUI.py` itself, it's just a security measure. By default it uses the following key in bytes :
-```python
-import ttkbootstrap as tk
-from AshTextCrypt import *
-import qr
-
-key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
+```shell
+python -m AshCrypt.AshCryptGUI
 ```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
```

### Comparing `AshCrypt-1.1.6/README.md` & `AshCrypt-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 <br>The `CliCrypt` will pop off automatically and you can start using it right away.
 
 <br>If you're testing how this works on a Debian based Docker container you can run this command to automatically set the environment before you run the command above
 ```bash
-curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/Apex/docker-build/env-setup.sh | bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/docker-build/env-setup.sh | bash
 ```
 Then run 
 ```bash
 source vvv/bin/activate
 ```
 
 <details>
@@ -243,26 +243,17 @@
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ## AshCryptGUI ##
-This is merely a GUI to encrypt and decrypt a text of a maximum of 200 characters and also display the qr representation of the text (encrypted/decrypted) .
-
+This is a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution
 ![alt text](important/GUI.png)
 
-**NOTE** : The key is not specified in the GUI its hard-coded, if you want to change the key make sure to change it from within the file `AshCryptGUI.py` itself, it's just a security measure. By default it uses the following key in bytes :
-```python
-import ttkbootstrap as tk
-from AshTextCrypt import *
-import qr
-
-key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
-```
 <br>To run the GUI anywhere
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
```

### Comparing `AshCrypt-1.1.6/setup.py` & `AshCrypt-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup , find_packages
 
-
-with open('AshCrypt/README.md','r') as f :
+with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.1.6',
+    version='1.2.0',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
     packages=find_packages(exclude=['important', 'docker-build']),
     package_data={
-        'AshCrypt': ['*'],
-        'unittestsAC': ['*'],
+        'AshCrypt': ['**'],
     },
     exclude_package_data={
         '': ['.gitignore','LICENSE','README'],
     },
     install_requires=[
         'bcrypt==4.0.1',
         'cryptography==40.0.2',
@@ -35,13 +33,15 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords=[
         'Cryptography',
         'AES-256',
     ],
 )
```

### Comparing `AshCrypt-1.1.6/unittestsAC/unittestAsh.py` & `AshCrypt-1.2.0/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

