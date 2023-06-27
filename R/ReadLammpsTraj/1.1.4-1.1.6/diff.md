# Comparing `tmp/ReadLammpsTraj-1.1.4.tar.gz` & `tmp/ReadLammpsTraj-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadLammpsTraj-1.1.4.tar", last modified: Wed May 31 14:35:19 2023, max compression
+gzip compressed data, was "ReadLammpsTraj-1.1.6.tar", last modified: Tue Jun 27 06:39:27 2023, max compression
```

## Comparing `ReadLammpsTraj-1.1.4.tar` & `ReadLammpsTraj-1.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.161053 ReadLammpsTraj-1.1.4/
--rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      132 2023-05-31 14:29:01.000000 ReadLammpsTraj-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2684 2023-05-31 14:35:19.160053 ReadLammpsTraj-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2401 2023-05-31 14:34:42.000000 ReadLammpsTraj-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.143533 ReadLammpsTraj-1.1.4/demo/
--rw-rw-rw-   0        0        0  2026571 2022-07-19 02:19:38.000000 ReadLammpsTraj-1.1.4/demo/1000.lammpstrj
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.146056 ReadLammpsTraj-1.1.4/demo/__pycache__/
--rw-rw-rw-   0        0        0    15185 2023-05-31 05:24:15.000000 ReadLammpsTraj-1.1.4/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc
--rw-rw-rw-   0        0        0     1966 2023-05-31 14:26:43.000000 ReadLammpsTraj-1.1.4/demo/cal_density.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.147055 ReadLammpsTraj-1.1.4/demo/imgs/
--rw-rw-rw-   0        0        0   307101 2023-05-31 14:26:47.000000 ReadLammpsTraj-1.1.4/demo/imgs/density.png
--rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:35:19.161053 ReadLammpsTraj-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-05-31 14:35:10.000000 ReadLammpsTraj-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.149054 ReadLammpsTraj-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.158054 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/
--rw-rw-rw-   0        0        0     2684 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-31 14:35:19.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.954986 ReadLammpsTraj-1.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-05-31 14:29:01.000000 ReadLammpsTraj-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2684 2023-06-27 06:39:27.953986 ReadLammpsTraj-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2401 2023-05-31 14:34:42.000000 ReadLammpsTraj-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.937910 ReadLammpsTraj-1.1.6/demo/
+-rw-rw-rw-   0        0        0  2026571 2022-07-19 02:19:38.000000 ReadLammpsTraj-1.1.6/demo/1000.lammpstrj
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.938909 ReadLammpsTraj-1.1.6/demo/__pycache__/
+-rw-rw-rw-   0        0        0    20996 2023-06-21 01:10:23.000000 ReadLammpsTraj-1.1.6/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1968 2023-06-21 01:01:32.000000 ReadLammpsTraj-1.1.6/demo/cal_density.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.940909 ReadLammpsTraj-1.1.6/demo/imgs/
+-rw-rw-rw-   0        0        0   307101 2023-05-31 14:26:47.000000 ReadLammpsTraj-1.1.6/demo/imgs/density.png
+-rw-rw-rw-   0        0        0       13 2023-06-21 01:20:36.000000 ReadLammpsTraj-1.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 06:39:27.954986 ReadLammpsTraj-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-06-27 05:23:51.000000 ReadLammpsTraj-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.943909 ReadLammpsTraj-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 06:39:27.951984 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/
+-rw-rw-rw-   0        0        0     2684 2023-06-27 06:39:27.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-27 06:39:27.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 06:39:27.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 06:39:27.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-27 06:39:27.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12030 2023-06-27 06:39:22.000000 ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.py
```

### Comparing `ReadLammpsTraj-1.1.4/LICENSE` & `ReadLammpsTraj-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.4/PKG-INFO` & `ReadLammpsTraj-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.4
+Version: 1.1.6
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.4/README.md` & `ReadLammpsTraj-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.4/demo/1000.lammpstrj` & `ReadLammpsTraj-1.1.6/demo/1000.lammpstrj`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.4/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc` & `ReadLammpsTraj-1.1.6/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,114 +1,526 @@
 magic:    0xa70d0d0a
-moddate:  0xfdd97664 (Wed May 31 05:24:13 2023 UTC)
-files sz: 8088
+moddate:  0xfd4d9264 (Wed Jun 21 01:10:21 2023 UTC)
+files sz: 11359
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a01640064016c025a030200470064028400640365
-      04a6030000ab0300000000000000005a0564015300
+      0x9700640064016c005a01640064016c025a0364025a04640384005a0502
+      006505a6000000ab0000000000000000000100640484005a060200470064
+      05840064066507a6030000ab0300000000000000005a0864015300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (numpy)
                  8 STORE_NAME               1 (np)
    
      4          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              2 (pandas)
                 16 STORE_NAME               3 (pd)
    
-     6          18 PUSH_NULL
-                20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               2 (<code object ReadLammpsTraj, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 6>)
+     6          18 LOAD_CONST               2 ('1.1.4')
+                20 STORE_NAME               4 (version)
+   
+     8          22 LOAD_CONST               3 (<code object print_ReadLammpsTraj, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 8>)
                 24 MAKE_FUNCTION            0
-                26 LOAD_CONST               3 ('ReadLammpsTraj')
-                28 LOAD_NAME                4 (object)
-                30 PRECALL                  3
-                34 CALL                     3
-                44 STORE_NAME               5 (ReadLammpsTraj)
-                46 LOAD_CONST               1 (None)
-                48 RETURN_VALUE
+                26 STORE_NAME               5 (print_ReadLammpsTraj)
+   
+    30          28 PUSH_NULL
+                30 LOAD_NAME                5 (print_ReadLammpsTraj)
+                32 PRECALL                  0
+                36 CALL                     0
+                46 POP_TOP
+   
+    32          48 LOAD_CONST               4 (<code object read_mass, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 32>)
+                50 MAKE_FUNCTION            0
+                52 STORE_NAME               6 (read_mass)
+   
+    66          54 PUSH_NULL
+                56 LOAD_BUILD_CLASS
+                58 LOAD_CONST               5 (<code object ReadLammpsTraj, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 66>)
+                60 MAKE_FUNCTION            0
+                62 LOAD_CONST               6 ('ReadLammpsTraj')
+                64 LOAD_NAME                7 (object)
+                66 PRECALL                  3
+                70 CALL                     3
+                80 STORE_NAME               8 (ReadLammpsTraj)
+                82 LOAD_CONST               1 (None)
+                84 RETURN_VALUE
    consts
       0
       None
+      '1.1.4'
+      code
+         argcount  : 0
+         nlocals   : 3
+         stacksize : 4
+         flags     : 3
+         code
+            0x970067006401a2017d0064027d017401000000000000000000006403a6
+            010000ab01000000000000000001007401000000000000000000007c0164
+            047a050000a6010000ab0100000000000000000100740100000000000000
+            0000007c0164057a050000a6010000ab01000000000000000001007c0044
+            005d117d027401000000000000000000007c02a6010000ab010000000000
+            00000001008c127401000000000000000000006406740200000000000000
+            0000007a0000006407a6020000ab02000000000000000001007401000000
+            000000000000007c0164057a050000a6010000ab01000000000000000001
+            007401000000000000000000007c0164047a050000a6010000ab01000000
+            0000000000010064005300
+           8           0 RESUME                   0
+         
+           9           2 BUILD_LIST               0
+                       4 LOAD_CONST               1 (('______                   _    _       _____                 _ ', '| ___ \\                 | |  | |     |_   _|               (_)', '| |_/ /  ___   __ _   __| |  | |       | |   _ __   __ _    _ ', "|    /  / _ \\ / _` | / _` |  | |       | |  | '__| / _` |  | |", '| |\\ \\ |  __/| (_| || (_| |  | |____   | |  | |   | (_| |  | |', '\\_| \\_| \\___| \\__,_| \\__,_|  \\_____/   \\_/  |_|    \\__,_|  | |', '                                                          _/ |', '                                                         |__/ '))
+                       6 LIST_EXTEND              1
+                       8 STORE_FAST               0 (cloud)
+         
+          19          10 LOAD_CONST               2 (32)
+                      12 STORE_FAST               1 (n)
+         
+          20          14 LOAD_GLOBAL              1 (NULL + print)
+                      26 LOAD_CONST               3 ('\n')
+                      28 PRECALL                  1
+                      32 CALL                     1
+                      42 POP_TOP
+         
+          21          44 LOAD_GLOBAL              1 (NULL + print)
+                      56 LOAD_FAST                1 (n)
+                      58 LOAD_CONST               4 ('- ')
+                      60 BINARY_OP                5 (*)
+                      64 PRECALL                  1
+                      68 CALL                     1
+                      78 POP_TOP
+         
+          22          80 LOAD_GLOBAL              1 (NULL + print)
+                      92 LOAD_FAST                1 (n)
+                      94 LOAD_CONST               5 ('. ')
+                      96 BINARY_OP                5 (*)
+                     100 PRECALL                  1
+                     104 CALL                     1
+                     114 POP_TOP
+         
+          23         116 LOAD_FAST                0 (cloud)
+                     118 GET_ITER
+                 >>  120 FOR_ITER                17 (to 156)
+                     122 STORE_FAST               2 (line)
+         
+          24         124 LOAD_GLOBAL              1 (NULL + print)
+                     136 LOAD_FAST                2 (line)
+                     138 PRECALL                  1
+                     142 CALL                     1
+                     152 POP_TOP
+                     154 JUMP_BACKWARD           18 (to 120)
+         
+          25     >>  156 LOAD_GLOBAL              1 (NULL + print)
+                     168 LOAD_CONST               6 ('@ReadLammpsTraj-')
+                     170 LOAD_GLOBAL              2 (version)
+                     182 BINARY_OP                0 (+)
+                     186 LOAD_CONST               7 (', Good Luck!')
+                     188 PRECALL                  2
+                     192 CALL                     2
+                     202 POP_TOP
+         
+          26         204 LOAD_GLOBAL              1 (NULL + print)
+                     216 LOAD_FAST                1 (n)
+                     218 LOAD_CONST               5 ('. ')
+                     220 BINARY_OP                5 (*)
+                     224 PRECALL                  1
+                     228 CALL                     1
+                     238 POP_TOP
+         
+          27         240 LOAD_GLOBAL              1 (NULL + print)
+                     252 LOAD_FAST                1 (n)
+                     254 LOAD_CONST               4 ('- ')
+                     256 BINARY_OP                5 (*)
+                     260 PRECALL                  1
+                     264 CALL                     1
+                     274 POP_TOP
+         
+          28         276 LOAD_CONST               0 (None)
+                     278 RETURN_VALUE
+         consts
+            None
+            ('______                   _    _       _____                 _ ', '| ___ \\                 | |  | |     |_   _|               (_)', '| |_/ /  ___   __ _   __| |  | |       | |   _ __   __ _    _ ', "|    /  / _ \\ / _` | / _` |  | |       | |  | '__| / _` |  | |", '| |\\ \\ |  __/| (_| || (_| |  | |____   | |  | |   | (_| |  | |', '\\_| \\_| \\___| \\__,_| \\__,_|  \\_____/   \\_/  |_|    \\__,_|  | |', '                                                          _/ |', '                                                         |__/ ')
+            32
+            '\n'
+            '- '
+            '. '
+            '@ReadLammpsTraj-'
+            ', Good Luck!'
+         names      ('print', 'version')
+         varnames   ('cloud', 'n', 'line')
+         freevars   ()
+         cellvars   ()
+         filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
+         name       'print_ReadLammpsTraj'
+         firstlineno 8
+         lnotab 0x0201080a04011e012401240108012001300124012401
+      code
+         argcount  : 1
+         nlocals   : 13
+         stacksize : 7
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006401a6020000ab020000000000
+            0000007d017c01a0010000000000000000000000000000000000000000a6
+            000000ab0000000000000000007d0267007d037c02a00200000000000000
+            000000000000000000000000006402a6010000ab0100000000000000005c
+            0200007d047d050900090009007c05a00200000000000000000000000000
+            000000000000006403a6010000ab0100000000000000005c0200007d037d
+            066e1f230001007c05a00200000000000000000000000000000000000000
+            006404a6010000ab0100000000000000005c0200007d037d0659006e0378
+            03590077016e1f230001007c05a002000000000000000000000000000000
+            00000000006405a6010000ab0100000000000000005c0200007d037d0659
+            006e037803590077016e1f230001007c05a0020000000000000000000000
+            0000000000000000006406a6010000ab0100000000000000005c0200007d
+            037d0659006e037803590077017407000000000000000000007c03a00200
+            000000000000000000000000000000000000006407a6010000ab01000000
+            0000000000a6010000ab0100000000000000007d03740700000000000000
+            00000074090000000000000000000064087c03a6020000ab020000000000
+            000000a6010000ab0100000000000000007d03670067007d087d07740b00
+            000000000000000000740d000000000000000000007c03a6010000ab0100
+            00000000000000a6010000ab01000000000000000044005d807d097c037c
+            0919000000000000000000a0070000000000000000000000000000000000
+            0000006409a6010000ab010000000000000000a002000000000000000000
+            00000000000000000000006409a6010000ab0100000000000000007d0a7c
+            07a008000000000000000000000000000000000000000074130000000000
+            00000000007c0a640a19000000000000000000a6010000ab010000000000
+            000000a6010000ab01000000000000000001007c08a00800000000000000
+            000000000000000000000000007415000000000000000000007c0a640b19
+            000000000000000000a6010000ab010000000000000000a6010000ab0100
+            0000000000000001008c817417000000000000000000007c077c08a60200
+            00ab0200000000000000007d0b640c84007c0b4400a6000000ab00000000
+            00000000007d0c7c0c5300
+          32           0 RESUME                   0
+         
+          36           2 LOAD_GLOBAL              1 (NULL + open)
+                      14 LOAD_FAST                0 (lammpsdata)
+                      16 LOAD_CONST               1 ('r')
+                      18 PRECALL                  2
+                      22 CALL                     2
+                      32 STORE_FAST               1 (data)
+         
+          37          34 LOAD_FAST                1 (data)
+                      36 LOAD_METHOD              1 (read)
+                      58 PRECALL                  0
+                      62 CALL                     0
+                      72 STORE_FAST               2 (lines)
+         
+          38          74 BUILD_LIST               0
+                      76 STORE_FAST               3 (mass)
+         
+          39          78 LOAD_FAST                2 (lines)
+                      80 LOAD_METHOD              2 (split)
+                     102 LOAD_CONST               2 ('\n\nMasses\n\n')
+                     104 PRECALL                  1
+                     108 CALL                     1
+                     118 UNPACK_SEQUENCE          2
+                     122 STORE_FAST               4 (header)
+                     124 STORE_FAST               5 (mass_other)
+         
+          40         126 NOP
+         
+          41         128 NOP
+         
+          42         130 NOP
+         
+          43         132 LOAD_FAST                5 (mass_other)
+                     134 LOAD_METHOD              2 (split)
+                     156 LOAD_CONST               3 ('\n\nPair Coeffs ')
+                     158 PRECALL                  1
+                     162 CALL                     1
+                     172 UNPACK_SEQUENCE          2
+                     176 STORE_FAST               3 (mass)
+                     178 STORE_FAST               6 (other)
+                     180 JUMP_FORWARD            31 (to 244)
+                 >>  182 PUSH_EXC_INFO
+         
+          44         184 POP_TOP
+         
+          45         186 LOAD_FAST                5 (mass_other)
+                     188 LOAD_METHOD              2 (split)
+                     210 LOAD_CONST               4 ('\n\nBond Coeffs ')
+                     212 PRECALL                  1
+                     216 CALL                     1
+                     226 UNPACK_SEQUENCE          2
+                     230 STORE_FAST               3 (mass)
+                     232 STORE_FAST               6 (other)
+                     234 POP_EXCEPT
+                     236 JUMP_FORWARD             3 (to 244)
+                 >>  238 COPY                     3
+                     240 POP_EXCEPT
+                     242 RERAISE                  1
+                 >>  244 JUMP_FORWARD            31 (to 308)
+                 >>  246 PUSH_EXC_INFO
+         
+          46         248 POP_TOP
+         
+          47         250 LOAD_FAST                5 (mass_other)
+                     252 LOAD_METHOD              2 (split)
+                     274 LOAD_CONST               5 ('\n\nAngle Coeffs ')
+                     276 PRECALL                  1
+                     280 CALL                     1
+                     290 UNPACK_SEQUENCE          2
+                     294 STORE_FAST               3 (mass)
+                     296 STORE_FAST               6 (other)
+                     298 POP_EXCEPT
+                     300 JUMP_FORWARD             3 (to 308)
+                 >>  302 COPY                     3
+                     304 POP_EXCEPT
+                     306 RERAISE                  1
+                 >>  308 JUMP_FORWARD            31 (to 372)
+                 >>  310 PUSH_EXC_INFO
+         
+          48         312 POP_TOP
+         
+          49         314 LOAD_FAST                5 (mass_other)
+                     316 LOAD_METHOD              2 (split)
+                     338 LOAD_CONST               6 ('\n\nAtoms # ')
+                     340 PRECALL                  1
+                     344 CALL                     1
+                     354 UNPACK_SEQUENCE          2
+                     358 STORE_FAST               3 (mass)
+                     360 STORE_FAST               6 (other)
+                     362 POP_EXCEPT
+                     364 JUMP_FORWARD             3 (to 372)
+                 >>  366 COPY                     3
+                     368 POP_EXCEPT
+                     370 RERAISE                  1
+         
+          51     >>  372 LOAD_GLOBAL              7 (NULL + list)
+                     384 LOAD_FAST                3 (mass)
+                     386 LOAD_METHOD              2 (split)
+                     408 LOAD_CONST               7 ('\n')
+                     410 PRECALL                  1
+                     414 CALL                     1
+                     424 PRECALL                  1
+                     428 CALL                     1
+                     438 STORE_FAST               3 (mass)
+         
+          52         440 LOAD_GLOBAL              7 (NULL + list)
+                     452 LOAD_GLOBAL              9 (NULL + filter)
+                     464 LOAD_CONST               8 (None)
+                     466 LOAD_FAST                3 (mass)
+                     468 PRECALL                  2
+                     472 CALL                     2
+                     482 PRECALL                  1
+                     486 CALL                     1
+                     496 STORE_FAST               3 (mass)
+         
+          53         498 BUILD_LIST               0
+                     500 BUILD_LIST               0
+                     502 STORE_FAST               8 (mass_sub)
+                     504 STORE_FAST               7 (mass_id)
+         
+          54         506 LOAD_GLOBAL             11 (NULL + range)
+                     518 LOAD_GLOBAL             13 (NULL + len)
+                     530 LOAD_FAST                3 (mass)
+                     532 PRECALL                  1
+                     536 CALL                     1
+                     546 PRECALL                  1
+                     550 CALL                     1
+                     560 GET_ITER
+                 >>  562 FOR_ITER               128 (to 820)
+                     564 STORE_FAST               9 (i)
+         
+          55         566 LOAD_FAST                3 (mass)
+                     568 LOAD_FAST                9 (i)
+                     570 BINARY_SUBSCR
+                     580 LOAD_METHOD              7 (strip)
+                     602 LOAD_CONST               9 (' ')
+                     604 PRECALL                  1
+                     608 CALL                     1
+                     618 LOAD_METHOD              2 (split)
+                     640 LOAD_CONST               9 (' ')
+                     642 PRECALL                  1
+                     646 CALL                     1
+                     656 STORE_FAST              10 (mass_uu)
+         
+          56         658 LOAD_FAST                7 (mass_id)
+                     660 LOAD_METHOD              8 (append)
+                     682 LOAD_GLOBAL             19 (NULL + int)
+                     694 LOAD_FAST               10 (mass_uu)
+                     696 LOAD_CONST              10 (0)
+                     698 BINARY_SUBSCR
+                     708 PRECALL                  1
+                     712 CALL                     1
+                     722 PRECALL                  1
+                     726 CALL                     1
+                     736 POP_TOP
+         
+          57         738 LOAD_FAST                8 (mass_sub)
+                     740 LOAD_METHOD              8 (append)
+                     762 LOAD_GLOBAL             21 (NULL + float)
+                     774 LOAD_FAST               10 (mass_uu)
+                     776 LOAD_CONST              11 (1)
+                     778 BINARY_SUBSCR
+                     788 PRECALL                  1
+                     792 CALL                     1
+                     802 PRECALL                  1
+                     806 CALL                     1
+                     816 POP_TOP
+                     818 JUMP_BACKWARD          129 (to 562)
+         
+          59     >>  820 LOAD_GLOBAL             23 (NULL + zip)
+                     832 LOAD_FAST                7 (mass_id)
+                     834 LOAD_FAST                8 (mass_sub)
+                     836 PRECALL                  2
+                     840 CALL                     2
+                     850 STORE_FAST              11 (pairs)
+         
+          60         852 LOAD_CONST              12 (<code object <dictcomp>, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 60>)
+                     854 MAKE_FUNCTION            0
+                     856 LOAD_FAST               11 (pairs)
+                     858 GET_ITER
+                     860 PRECALL                  0
+                     864 CALL                     0
+                     874 STORE_FAST              12 (mass_dict)
+         
+          62         876 LOAD_FAST               12 (mass_dict)
+                     878 RETURN_VALUE
+         ExceptionTable:
+           132 to 178 -> 182 [0]
+           180 to 180 -> 246 [0]
+           182 to 232 -> 238 [1] lasti
+           234 to 242 -> 246 [0]
+           244 to 244 -> 310 [0]
+           246 to 296 -> 302 [1] lasti
+           298 to 306 -> 310 [0]
+           310 to 360 -> 366 [1] lasti
+         consts
+            '\n\tread atomic mass from lammps data. \n\t'
+            'r'
+            '\n\nMasses\n\n'
+            '\n\nPair Coeffs '
+            '\n\nBond Coeffs '
+            '\n\nAngle Coeffs '
+            '\n\nAtoms # '
+            '\n'
+            None
+            ' '
+            0
+            1
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 4
+               flags     : 19
+               code 0x970069007c005d085c0200007d017d027c017c0293028c095300
+                60           0 RESUME                   0
+                             2 BUILD_MAP                0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                 8 (to 24)
+                             8 UNPACK_SEQUENCE          2
+                            12 STORE_FAST               1 (k)
+                            14 STORE_FAST               2 (v)
+                            16 LOAD_FAST                1 (k)
+                            18 LOAD_FAST                2 (v)
+                            20 MAP_ADD                  2
+                            22 JUMP_BACKWARD            9 (to 6)
+                       >>   24 RETURN_VALUE
+               consts
+               names      ()
+               varnames   ('.0', 'k', 'v')
+               freevars   ()
+               cellvars   ()
+               filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
+               name       '<dictcomp>'
+               firstlineno 60
+               lnotab 0x
+         names      ('open', 'read', 'split', 'list', 'filter', 'range', 'len', 'strip', 'append', 'int', 'float', 'zip')
+         varnames   ('lammpsdata', 'data', 'lines', 'mass', 'header', 'mass_other', 'other', 'mass_id', 'mass_sub', 'i', 'mass_uu', 'pairs', 'mass_dict')
+         freevars   ()
+         cellvars   ()
+         filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
+         name       'read_mass'
+         firstlineno 32
+         lnotab
+            0x02042001280104013001020102010201340102013e0102013e0102013a
+            0244013a0108013c015c015001520220011802
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 4
          flags     : 0
          code
-            0x8700970065005a0164005a0264015a03640f88006601640384095a0464
-            0484005a05640584005a06640684005a07640784005a08640884005a0964
-            10640a84015a0a6411640c84015a0b6412640d84015a0c640e84005a0d88
-            0078015a0e5300
+            0x8700970065005a0164005a0264015a03641088006601640384095a0464
+            0484005a05640584005a06640684005a07640784005a08640884005a0969
+            006409640a6603640b84015a0a6900640c6409640a6604640d84015a0b64
+            11640e84015a0c640f84005a0d880078015a0e5300
                        0 MAKE_CELL                0 (__class__)
          
-           6           2 RESUME                   0
+          66           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ReadLammpsTraj')
                       10 STORE_NAME               2 (__qualname__)
          
-           7          12 LOAD_CONST               1 ('docstring for ClassName')
+          67          12 LOAD_CONST               1 ('docstring for ClassName')
                       14 STORE_NAME               3 (__doc__)
          
-           8          16 LOAD_CONST              15 ((1,))
+          68          16 LOAD_CONST              16 ((1,))
                       18 LOAD_CLOSURE             0 (__class__)
                       20 BUILD_TUPLE              1
-                      22 LOAD_CONST               3 (<code object __init__, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 8>)
+                      22 LOAD_CONST               3 (<code object __init__, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 68>)
                       24 MAKE_FUNCTION            9 (defaults, closure)
                       26 STORE_NAME               4 (__init__)
          
-          14          28 LOAD_CONST               4 (<code object read_info, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 14>)
+          74          28 LOAD_CONST               4 (<code object read_info, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 74>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (read_info)
          
-          50          34 LOAD_CONST               5 (<code object read_header, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 50>)
+         110          34 LOAD_CONST               5 (<code object read_header, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 110>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (read_header)
          
-          61          40 LOAD_CONST               6 (<code object read_vol, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 61>)
+         121          40 LOAD_CONST               6 (<code object read_vol, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 121>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (read_vol)
          
-          76          46 LOAD_CONST               7 (<code object read_mxyz, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 76>)
+         136          46 LOAD_CONST               7 (<code object read_mxyz, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 136>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (read_mxyz)
          
-         102          52 LOAD_CONST               8 (<code object read_traj, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 102>)
+         165          52 LOAD_CONST               8 (<code object read_traj, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 165>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME               9 (read_traj)
          
-         111          58 LOAD_CONST              16 (('mass',))
-                      60 LOAD_CONST              10 (<code object oneframe_alldensity, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 111>)
-                      62 MAKE_FUNCTION            1 (defaults)
-                      64 STORE_NAME              10 (oneframe_alldensity)
-         
-         151          66 LOAD_CONST              17 (('mol', 'mass'))
-                      68 LOAD_CONST              12 (<code object oneframe_moldensity, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 151>)
-                      70 MAKE_FUNCTION            1 (defaults)
-                      72 STORE_NAME              11 (oneframe_moldensity)
-         
-         194          74 LOAD_CONST              18 ((1, 1, 1, 'mass'))
-                      76 LOAD_CONST              13 (<code object TwoD_Density, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 194>)
-                      78 MAKE_FUNCTION            1 (defaults)
-                      80 STORE_NAME              12 (TwoD_Density)
-         
-         268          82 LOAD_CONST              14 (<code object unwrap, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 268>)
-                      84 MAKE_FUNCTION            0
-                      86 STORE_NAME              13 (unwrap)
-                      88 LOAD_CLOSURE             0 (__class__)
-                      90 COPY                     1
-                      92 STORE_NAME              14 (__classcell__)
-                      94 RETURN_VALUE
+         177          58 BUILD_MAP                0
+                      60 LOAD_CONST               9 ('mass')
+                      62 LOAD_CONST              10 ('z')
+                      64 BUILD_TUPLE              3
+                      66 LOAD_CONST              11 (<code object oneframe_alldensity, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 177>)
+                      68 MAKE_FUNCTION            1 (defaults)
+                      70 STORE_NAME              10 (oneframe_alldensity)
+         
+         238          72 BUILD_MAP                0
+                      74 LOAD_CONST              12 ('mol')
+                      76 LOAD_CONST               9 ('mass')
+                      78 LOAD_CONST              10 ('z')
+                      80 BUILD_TUPLE              4
+                      82 LOAD_CONST              13 (<code object oneframe_moldensity, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 238>)
+                      84 MAKE_FUNCTION            1 (defaults)
+                      86 STORE_NAME              11 (oneframe_moldensity)
+         
+         306          88 LOAD_CONST              17 ((1, 1, 1, 'mass'))
+                      90 LOAD_CONST              14 (<code object TwoD_Density, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 306>)
+                      92 MAKE_FUNCTION            1 (defaults)
+                      94 STORE_NAME              12 (TwoD_Density)
+         
+         380          96 LOAD_CONST              15 (<code object unwrap, file "E:\DongshengChen\OneDrive - student.cup.edu.cn\Github\MyRepos\ReadLammpsTraj\demo\ReadLammpsTraj.py", line 380>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              13 (unwrap)
+                     102 LOAD_CLOSURE             0 (__class__)
+                     104 COPY                     1
+                     106 STORE_NAME              14 (__classcell__)
+                     108 RETURN_VALUE
          consts
             'ReadLammpsTraj'
             'docstring for ClassName'
             1
             code
                argcount  : 3
                nlocals   : 3
@@ -118,54 +530,54 @@
                   0x950197007401000000000000000000007402000000000000000000007c
                   00a6020000ab020000000000000000a00200000000000000000000000000
                   00000000000000a6000000ab00000000000000000001007c017c005f0300
                   0000000000000064017c005f04000000000000000064027c005f05000000
                   00000000007c027c005f06000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                 8           2 RESUME                   0
+                68           2 RESUME                   0
                
-                 9           4 LOAD_GLOBAL              1 (NULL + super)
+                69           4 LOAD_GLOBAL              1 (NULL + super)
                             16 LOAD_GLOBAL              2 (ReadLammpsTraj)
                             28 LOAD_FAST                0 (self)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_METHOD              2 (__init__)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 POP_TOP
                
-                10          82 LOAD_FAST                1 (f)
+                70          82 LOAD_FAST                1 (f)
                             84 LOAD_FAST                0 (self)
                             86 STORE_ATTR               3 (f)
                
-                11          96 LOAD_CONST               1 (6.02214076208112e+23)
+                71          96 LOAD_CONST               1 (6.02214076208112e+23)
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               4 (amu2g)
                
-                12         110 LOAD_CONST               2 (1e-08)
+                72         110 LOAD_CONST               2 (1e-08)
                            112 LOAD_FAST                0 (self)
                            114 STORE_ATTR               5 (A2CM)
                
-                13         124 LOAD_FAST                2 (timestep)
+                73         124 LOAD_FAST                2 (timestep)
                            126 LOAD_FAST                0 (self)
                            128 STORE_ATTR               6 (timestep)
                            138 LOAD_CONST               0 (None)
                            140 RETURN_VALUE
                consts
                   None
                   6.02214076208112e+23
                   1e-08
                names      ('super', 'ReadLammpsTraj', '__init__', 'f', 'amu2g', 'A2CM', 'timestep')
                varnames   ('self', 'f', 'timestep')
                freevars   ('__class__',)
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       '__init__'
-               firstlineno 8
+               firstlineno 68
                lnotab 0x04014e010e010e010e01
             code
                argcount  : 1
                nlocals   : 15
                stacksize : 9
                flags     : 3
                code
@@ -229,74 +641,74 @@
                   110000000000000000a6060000ab06000000000000000001006e1d230001
                   0064037c005f140000000000000000742b000000000000000000006410a6
                   010000ab010000000000000000010059006e037803590077016400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   00770101005900010001007c006a1400000000000000007c006a07000000
                   00000000007c006a0f00000000000000007c006a1000000000000000007c
                   006a11000000000000000066055300
-                14           0 RESUME                   0
+                74           0 RESUME                   0
                
-                15           2 LOAD_GLOBAL              1 (NULL + open)
+                75           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (f)
                             26 LOAD_CONST               1 ('r')
                             28 PRECALL                  2
                             32 CALL                     2
                             42 BEFORE_WITH
                             44 STORE_FAST               1 (f)
                
-                16          46 LOAD_FAST                1 (f)
+                76          46 LOAD_FAST                1 (f)
                             48 LOAD_METHOD              2 (readline)
                             70 PRECALL                  0
                             74 CALL                     0
                             84 STORE_FAST               2 (L1)
                
-                17          86 LOAD_FAST                1 (f)
+                77          86 LOAD_FAST                1 (f)
                             88 LOAD_METHOD              2 (readline)
                            110 PRECALL                  0
                            114 CALL                     0
                            124 STORE_FAST               3 (L2)
                
-                18         126 LOAD_FAST                1 (f)
+                78         126 LOAD_FAST                1 (f)
                            128 LOAD_METHOD              2 (readline)
                            150 PRECALL                  0
                            154 CALL                     0
                            164 STORE_FAST               4 (L3)
                
-                19         166 LOAD_FAST                1 (f)
+                79         166 LOAD_FAST                1 (f)
                            168 LOAD_METHOD              2 (readline)
                            190 PRECALL                  0
                            194 CALL                     0
                            204 STORE_FAST               5 (L4)
                
-                20         206 LOAD_FAST                1 (f)
+                80         206 LOAD_FAST                1 (f)
                            208 LOAD_METHOD              2 (readline)
                            230 PRECALL                  0
                            234 CALL                     0
                            244 STORE_FAST               6 (L5)
                
-                21         246 LOAD_FAST                1 (f)
+                81         246 LOAD_FAST                1 (f)
                            248 LOAD_METHOD              2 (readline)
                            270 PRECALL                  0
                            274 CALL                     0
                            284 STORE_FAST               7 (L6)
                
-                22         286 LOAD_FAST                1 (f)
+                82         286 LOAD_FAST                1 (f)
                            288 LOAD_METHOD              2 (readline)
                            310 PRECALL                  0
                            314 CALL                     0
                            324 STORE_FAST               8 (L7)
                
-                23         326 LOAD_FAST                1 (f)
+                83         326 LOAD_FAST                1 (f)
                            328 LOAD_METHOD              2 (readline)
                            350 PRECALL                  0
                            354 CALL                     0
                            364 STORE_FAST               9 (L8)
                
-                24         366 LOAD_FAST                1 (f)
+                84         366 LOAD_FAST                1 (f)
                            368 LOAD_METHOD              2 (readline)
                            390 PRECALL                  0
                            394 CALL                     0
                            404 LOAD_METHOD              3 (strip)
                            426 PRECALL                  0
                            430 CALL                     0
                            440 LOAD_METHOD              4 (split)
@@ -304,32 +716,32 @@
                            466 CALL                     0
                            476 LOAD_CONST               2 (2)
                            478 LOAD_CONST               0 (None)
                            480 BUILD_SLICE              2
                            482 BINARY_SUBSCR
                            492 STORE_FAST              10 (L9)
                
-                25         494 LOAD_FAST               10 (L9)
+                85         494 LOAD_FAST               10 (L9)
                            496 LOAD_FAST                0 (self)
                            498 STORE_ATTR               5 (col)
                
-                26         508 LOAD_GLOBAL             13 (NULL + int)
+                86         508 LOAD_GLOBAL             13 (NULL + int)
                            520 LOAD_FAST                3 (L2)
                            522 PRECALL                  1
                            526 CALL                     1
                            536 STORE_FAST              11 (step1)
                
-                27         538 LOAD_GLOBAL             13 (NULL + int)
+                87         538 LOAD_GLOBAL             13 (NULL + int)
                            550 LOAD_FAST                5 (L4)
                            552 PRECALL                  1
                            556 CALL                     1
                            566 LOAD_FAST                0 (self)
                            568 STORE_ATTR               7 (atom_n)
                
-                28         578 LOAD_GLOBAL             17 (NULL + float)
+                88         578 LOAD_GLOBAL             17 (NULL + float)
                            590 LOAD_FAST                7 (L6)
                            592 LOAD_METHOD              4 (split)
                            614 PRECALL                  0
                            618 CALL                     0
                            628 LOAD_CONST               3 (0)
                            630 BINARY_SUBSCR
                            640 PRECALL                  1
@@ -345,15 +757,15 @@
                            720 CALL                     1
                            730 SWAP                     2
                            732 LOAD_FAST                0 (self)
                            734 STORE_ATTR               9 (xlo)
                            744 LOAD_FAST                0 (self)
                            746 STORE_ATTR              10 (xhi)
                
-                29         756 LOAD_GLOBAL             17 (NULL + float)
+                89         756 LOAD_GLOBAL             17 (NULL + float)
                            768 LOAD_FAST                8 (L7)
                            770 LOAD_METHOD              4 (split)
                            792 PRECALL                  0
                            796 CALL                     0
                            806 LOAD_CONST               3 (0)
                            808 BINARY_SUBSCR
                            818 PRECALL                  1
@@ -369,15 +781,15 @@
                            898 CALL                     1
                            908 SWAP                     2
                            910 LOAD_FAST                0 (self)
                            912 STORE_ATTR              11 (ylo)
                            922 LOAD_FAST                0 (self)
                            924 STORE_ATTR              12 (yhi)
                
-                30         934 LOAD_GLOBAL             17 (NULL + float)
+                90         934 LOAD_GLOBAL             17 (NULL + float)
                            946 LOAD_FAST                9 (L8)
                            948 LOAD_METHOD              4 (split)
                            970 PRECALL                  0
                            974 CALL                     0
                            984 LOAD_CONST               3 (0)
                            986 BINARY_SUBSCR
                            996 PRECALL                  1
@@ -393,124 +805,124 @@
                           1076 CALL                     1
                           1086 SWAP                     2
                           1088 LOAD_FAST                0 (self)
                           1090 STORE_ATTR              13 (zlo)
                           1100 LOAD_FAST                0 (self)
                           1102 STORE_ATTR              14 (zhi)
                
-                31        1112 LOAD_FAST                0 (self)
+                91        1112 LOAD_FAST                0 (self)
                           1114 LOAD_ATTR               10 (xhi)
                           1124 LOAD_FAST                0 (self)
                           1126 LOAD_ATTR                9 (xlo)
                           1136 BINARY_OP               10 (-)
                           1140 LOAD_FAST                0 (self)
                           1142 STORE_ATTR              15 (Lx)
                
-                32        1152 LOAD_FAST                0 (self)
+                92        1152 LOAD_FAST                0 (self)
                           1154 LOAD_ATTR               12 (yhi)
                           1164 LOAD_FAST                0 (self)
                           1166 LOAD_ATTR               11 (ylo)
                           1176 BINARY_OP               10 (-)
                           1180 LOAD_FAST                0 (self)
                           1182 STORE_ATTR              16 (Ly)
                
-                33        1192 LOAD_FAST                0 (self)
+                93        1192 LOAD_FAST                0 (self)
                           1194 LOAD_ATTR               14 (zhi)
                           1204 LOAD_FAST                0 (self)
                           1206 LOAD_ATTR               13 (zlo)
                           1216 BINARY_OP               10 (-)
                           1220 LOAD_FAST                0 (self)
                           1222 STORE_ATTR              17 (Lz)
                
-                34        1232 LOAD_FAST                0 (self)
+                94        1232 LOAD_FAST                0 (self)
                           1234 LOAD_ATTR               15 (Lx)
                           1244 LOAD_FAST                0 (self)
                           1246 LOAD_ATTR               16 (Ly)
                           1256 BINARY_OP                5 (*)
                           1260 LOAD_FAST                0 (self)
                           1262 LOAD_ATTR               17 (Lz)
                           1272 BINARY_OP                5 (*)
                           1276 LOAD_FAST                0 (self)
                           1278 STORE_ATTR              18 (vlo)
                
-                35        1288 LOAD_GLOBAL             39 (NULL + range)
+                95        1288 LOAD_GLOBAL             39 (NULL + range)
                           1300 LOAD_FAST                0 (self)
                           1302 LOAD_ATTR                7 (atom_n)
                           1312 LOAD_CONST               4 (1)
                           1314 BINARY_OP                0 (+)
                           1318 PRECALL                  1
                           1322 CALL                     1
                           1332 GET_ITER
                        >> 1334 FOR_ITER                22 (to 1380)
                           1336 STORE_FAST              12 (i)
                
-                36        1338 LOAD_FAST                1 (f)
+                96        1338 LOAD_FAST                1 (f)
                           1340 LOAD_METHOD              2 (readline)
                           1362 PRECALL                  0
                           1366 CALL                     0
                           1376 STORE_FAST              13 (Li)
                           1378 JUMP_BACKWARD           23 (to 1334)
                
-                38     >> 1380 NOP
+                98     >> 1380 NOP
                
-                39        1382 LOAD_GLOBAL             13 (NULL + int)
+                99        1382 LOAD_GLOBAL             13 (NULL + int)
                           1394 LOAD_FAST                1 (f)
                           1396 LOAD_METHOD              2 (readline)
                           1418 PRECALL                  0
                           1422 CALL                     0
                           1432 PRECALL                  1
                           1436 CALL                     1
                           1446 STORE_FAST              14 (step2)
                
-                40        1448 LOAD_FAST               14 (step2)
+               100        1448 LOAD_FAST               14 (step2)
                           1450 LOAD_FAST               11 (step1)
                           1452 BINARY_OP               10 (-)
                           1456 LOAD_FAST                0 (self)
                           1458 STORE_ATTR              20 (step_inter)
                
-                41        1468 LOAD_GLOBAL             43 (NULL + print)
+               101        1468 LOAD_GLOBAL             43 (NULL + print)
                           1480 LOAD_CONST               5 ('Step interval:')
                           1482 LOAD_FAST                0 (self)
                           1484 LOAD_ATTR               20 (step_inter)
                           1494 LOAD_CONST               6 ('\nAtom number:')
                           1496 LOAD_FAST                0 (self)
                           1498 LOAD_ATTR                7 (atom_n)
                           1508 PRECALL                  4
                           1512 CALL                     4
                           1522 POP_TOP
                
-                42        1524 LOAD_GLOBAL             43 (NULL + print)
+               102        1524 LOAD_GLOBAL             43 (NULL + print)
                           1536 LOAD_CONST               7 ('xlo:')
                           1538 LOAD_FAST                0 (self)
                           1540 LOAD_ATTR                9 (xlo)
                           1550 LOAD_CONST               8 ('xhi:')
                           1552 LOAD_FAST                0 (self)
                           1554 LOAD_ATTR               10 (xhi)
                           1564 LOAD_CONST               9 ('Lx:')
                           1566 LOAD_FAST                0 (self)
                           1568 LOAD_ATTR               15 (Lx)
                           1578 PRECALL                  6
                           1582 CALL                     6
                           1592 POP_TOP
                
-                43        1594 LOAD_GLOBAL             43 (NULL + print)
+               103        1594 LOAD_GLOBAL             43 (NULL + print)
                           1606 LOAD_CONST              10 ('ylo:')
                           1608 LOAD_FAST                0 (self)
                           1610 LOAD_ATTR               11 (ylo)
                           1620 LOAD_CONST              11 ('yhi:')
                           1622 LOAD_FAST                0 (self)
                           1624 LOAD_ATTR               12 (yhi)
                           1634 LOAD_CONST              12 ('Ly:')
                           1636 LOAD_FAST                0 (self)
                           1638 LOAD_ATTR               16 (Ly)
                           1648 PRECALL                  6
                           1652 CALL                     6
                           1662 POP_TOP
                
-                44        1664 LOAD_GLOBAL             43 (NULL + print)
+               104        1664 LOAD_GLOBAL             43 (NULL + print)
                           1676 LOAD_CONST              13 ('zlo:')
                           1678 LOAD_FAST                0 (self)
                           1680 LOAD_ATTR               13 (zlo)
                           1690 LOAD_CONST              14 ('zhi:')
                           1692 LOAD_FAST                0 (self)
                           1694 LOAD_ATTR               14 (zhi)
                           1704 LOAD_CONST              15 ('Lz:')
@@ -518,32 +930,32 @@
                           1708 LOAD_ATTR               17 (Lz)
                           1718 PRECALL                  6
                           1722 CALL                     6
                           1732 POP_TOP
                           1734 JUMP_FORWARD            29 (to 1794)
                        >> 1736 PUSH_EXC_INFO
                
-                45        1738 POP_TOP
+               105        1738 POP_TOP
                
-                46        1740 LOAD_CONST               3 (0)
+               106        1740 LOAD_CONST               3 (0)
                           1742 LOAD_FAST                0 (self)
                           1744 STORE_ATTR              20 (step_inter)
                
-                47        1754 LOAD_GLOBAL             43 (NULL + print)
+               107        1754 LOAD_GLOBAL             43 (NULL + print)
                           1766 LOAD_CONST              16 ('pass')
                           1768 PRECALL                  1
                           1772 CALL                     1
                           1782 POP_TOP
                           1784 POP_EXCEPT
                           1786 JUMP_FORWARD             3 (to 1794)
                        >> 1788 COPY                     3
                           1790 POP_EXCEPT
                           1792 RERAISE                  1
                
-                15     >> 1794 LOAD_CONST               0 (None)
+                75     >> 1794 LOAD_CONST               0 (None)
                           1796 LOAD_CONST               0 (None)
                           1798 LOAD_CONST               0 (None)
                           1800 PRECALL                  2
                           1804 CALL                     2
                           1814 POP_TOP
                           1816 JUMP_FORWARD            11 (to 1840)
                        >> 1818 PUSH_EXC_INFO
@@ -554,15 +966,15 @@
                           1828 POP_EXCEPT
                           1830 RERAISE                  1
                        >> 1832 POP_TOP
                           1834 POP_EXCEPT
                           1836 POP_TOP
                           1838 POP_TOP
                
-                48     >> 1840 LOAD_FAST                0 (self)
+               108     >> 1840 LOAD_FAST                0 (self)
                           1842 LOAD_ATTR               20 (step_inter)
                           1852 LOAD_FAST                0 (self)
                           1854 LOAD_ATTR                7 (atom_n)
                           1864 LOAD_FAST                0 (self)
                           1866 LOAD_ATTR               15 (Lx)
                           1876 LOAD_FAST                0 (self)
                           1878 LOAD_ATTR               16 (Ly)
@@ -598,15 +1010,15 @@
                   'pass'
                names      ('open', 'f', 'readline', 'strip', 'split', 'col', 'int', 'atom_n', 'float', 'xlo', 'xhi', 'ylo', 'yhi', 'zlo', 'zhi', 'Lx', 'Ly', 'Lz', 'vlo', 'range', 'step_inter', 'print')
                varnames   ('self', 'f', 'L1', 'L2', 'L3', 'L4', 'L5', 'L6', 'L7', 'L8', 'L9', 'step1', 'i', 'Li', 'step2')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'read_info'
-               firstlineno 14
+               firstlineno 74
                lnotab
                   0x02012c012801280128012801280128012801280180010e011e012801b2
                   01b201b201280128012801380132012a020201420114013801460146014a
                   0102010e0128e02e21
             code
                argcount  : 2
                nlocals   : 6
@@ -619,40 +1031,40 @@
                   047d057c0464027c006a03000000000000000064037a0000007c017a0500
                   007a0000006b050000000072297c0464037c006a03000000000000000064
                   037a0000007c017a0500007a0000006b010000000072157c03a004000000
                   00000000000000000000000000000000007c05a6010000ab010000000000
                   00000001008c437c037d03640064006400a6020000ab0200000000000000
                   0001006e0b230031007304770278035900770101005900010001007c0353
                   00
-                50           0 RESUME                   0
+               110           0 RESUME                   0
                
-                51           2 LOAD_GLOBAL              1 (NULL + open)
+               111           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (f)
                             26 LOAD_CONST               1 ('r')
                             28 PRECALL                  2
                             32 CALL                     2
                             42 BEFORE_WITH
                             44 STORE_FAST               2 (f)
                
-                52          46 BUILD_LIST               0
+               112          46 BUILD_LIST               0
                             48 STORE_FAST               3 (header)
                
-                53          50 LOAD_GLOBAL              5 (NULL + enumerate)
+               113          50 LOAD_GLOBAL              5 (NULL + enumerate)
                             62 LOAD_FAST                2 (f)
                             64 LOAD_CONST               2 (1)
                             66 PRECALL                  2
                             70 CALL                     2
                             80 GET_ITER
                        >>   82 FOR_ITER                66 (to 216)
                             84 UNPACK_SEQUENCE          2
                             88 STORE_FAST               4 (index)
                             90 STORE_FAST               5 (line)
                
-                54          92 LOAD_FAST                4 (index)
+               114          92 LOAD_FAST                4 (index)
                             94 LOAD_CONST               2 (1)
                             96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                3 (atom_n)
                            108 LOAD_CONST               3 (9)
                            110 BINARY_OP                0 (+)
                            114 LOAD_FAST                1 (nframe)
                            116 BINARY_OP                5 (*)
@@ -667,26 +1079,26 @@
                            150 BINARY_OP                0 (+)
                            154 LOAD_FAST                1 (nframe)
                            156 BINARY_OP                5 (*)
                            160 BINARY_OP                0 (+)
                            164 COMPARE_OP               1 (<=)
                            170 POP_JUMP_FORWARD_IF_FALSE    21 (to 214)
                
-                56         172 LOAD_FAST                3 (header)
+               116         172 LOAD_FAST                3 (header)
                            174 LOAD_METHOD              4 (append)
                            196 LOAD_FAST                5 (line)
                            198 PRECALL                  1
                            202 CALL                     1
                            212 POP_TOP
                        >>  214 JUMP_BACKWARD           67 (to 82)
                
-                57     >>  216 LOAD_FAST                3 (header)
+               117     >>  216 LOAD_FAST                3 (header)
                            218 STORE_FAST               3 (header)
                
-                51         220 LOAD_CONST               0 (None)
+               111         220 LOAD_CONST               0 (None)
                            222 LOAD_CONST               0 (None)
                            224 LOAD_CONST               0 (None)
                            226 PRECALL                  2
                            230 CALL                     2
                            240 POP_TOP
                            242 JUMP_FORWARD            11 (to 266)
                        >>  244 PUSH_EXC_INFO
@@ -697,15 +1109,15 @@
                            254 POP_EXCEPT
                            256 RERAISE                  1
                        >>  258 POP_TOP
                            260 POP_EXCEPT
                            262 POP_TOP
                            264 POP_TOP
                
-                59     >>  266 LOAD_FAST                3 (header)
+               119     >>  266 LOAD_FAST                3 (header)
                            268 RETURN_VALUE
                ExceptionTable:
                  44 to 218 -> 244 [1] lasti
                  244 to 250 -> 252 [3] lasti
                  258 to 258 -> 252 [3] lasti
                consts
                   None
@@ -714,15 +1126,15 @@
                   9
                names      ('open', 'f', 'enumerate', 'atom_n', 'append')
                varnames   ('self', 'nframe', 'f', 'header', 'index', 'line')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'read_header'
-               firstlineno 50
+               firstlineno 110
                lnotab 0x02012c0104012a0150022c0104fa2e08
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 5
                flags     : 3
                code
@@ -730,76 +1142,76 @@
                   0164037a0a00007a0500007a0000007d027403000000000000000000006a
                   0200000000000000007c006a0300000000000000007c026404ac05a60300
                   00ab0300000000000000007d037c036406190000000000000000007c0364
                   07190000000000000000007a0a00007d047c036408190000000000000000
                   007c036409190000000000000000007a0a00007d057c03640a1900000000
                   00000000007c03640b190000000000000000007a0a00007d067c047c057a
                   0500007c067a0500007d077c075300
-                61           0 RESUME                   0
+               121           0 RESUME                   0
                
-                67           2 LOAD_CONST               1 (5)
+               127           2 LOAD_CONST               1 (5)
                              4 LOAD_FAST                1 (nframe)
                              6 BINARY_OP                5 (*)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (atom_n)
                             22 LOAD_CONST               2 (4)
                             24 BINARY_OP                0 (+)
                             28 LOAD_FAST                1 (nframe)
                             30 LOAD_CONST               3 (1)
                             32 BINARY_OP               10 (-)
                             36 BINARY_OP                5 (*)
                             40 BINARY_OP                0 (+)
                             44 STORE_FAST               2 (skip)
                
-                68          46 LOAD_GLOBAL              3 (NULL + np)
+               128          46 LOAD_GLOBAL              3 (NULL + np)
                             58 LOAD_ATTR                2 (loadtxt)
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                3 (f)
                             80 LOAD_FAST                2 (skip)
                             82 LOAD_CONST               4 (3)
                             84 KW_NAMES                 5
                             86 PRECALL                  3
                             90 CALL                     3
                            100 STORE_FAST               3 (vol_xyz)
                
-                70         102 LOAD_FAST                3 (vol_xyz)
+               130         102 LOAD_FAST                3 (vol_xyz)
                            104 LOAD_CONST               6 ((0, 1))
                            106 BINARY_SUBSCR
                            116 LOAD_FAST                3 (vol_xyz)
                            118 LOAD_CONST               7 ((0, 0))
                            120 BINARY_SUBSCR
                            130 BINARY_OP               10 (-)
                            134 STORE_FAST               4 (xL)
                
-                71         136 LOAD_FAST                3 (vol_xyz)
+               131         136 LOAD_FAST                3 (vol_xyz)
                            138 LOAD_CONST               8 ((1, 1))
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                3 (vol_xyz)
                            152 LOAD_CONST               9 ((1, 0))
                            154 BINARY_SUBSCR
                            164 BINARY_OP               10 (-)
                            168 STORE_FAST               5 (yL)
                
-                72         170 LOAD_FAST                3 (vol_xyz)
+               132         170 LOAD_FAST                3 (vol_xyz)
                            172 LOAD_CONST              10 ((2, 1))
                            174 BINARY_SUBSCR
                            184 LOAD_FAST                3 (vol_xyz)
                            186 LOAD_CONST              11 ((2, 0))
                            188 BINARY_SUBSCR
                            198 BINARY_OP               10 (-)
                            202 STORE_FAST               6 (zL)
                
-                73         204 LOAD_FAST                4 (xL)
+               133         204 LOAD_FAST                4 (xL)
                            206 LOAD_FAST                5 (yL)
                            208 BINARY_OP                5 (*)
                            212 LOAD_FAST                6 (zL)
                            214 BINARY_OP                5 (*)
                            218 STORE_FAST               7 (vol)
                
-                74         220 LOAD_FAST                7 (vol)
+               134         220 LOAD_FAST                7 (vol)
                            222 RETURN_VALUE
                consts
                   '\n\t\tcalculate the volume by traj file\n\t\tnframe: n_th frame, nframe>=1 and int type\n\t\tvol: volume of system, unit: A^3\n\t\t'
                   5
                   4
                   1
                   3
@@ -812,213 +1224,214 @@
                   (2, 0)
                names      ('atom_n', 'np', 'loadtxt', 'f')
                varnames   ('self', 'nframe', 'skip', 'vol_xyz', 'xL', 'yL', 'zL', 'vol')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'read_vol'
-               firstlineno 61
+               firstlineno 121
                lnotab 0x02062c0138022201220122011001
             code
                argcount  : 2
                nlocals   : 7
                stacksize : 6
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007d0209007c026a01000000000000000064
-                  006400850264016602190000000000000000006a020000000000000000a0
+                  016401850264026602190000000000000000006a020000000000000000a0
                   030000000000000000000000000000000000000000740800000000000000
                   0000006a050000000000000000a6010000ab0100000000000000007c005f
-                  0600000000000000006e1623000100740f000000000000000000006402a6
+                  0600000000000000006e1623000100740f000000000000000000006403a6
                   010000ab010000000000000000010059006e0378035900770109007c026a
-                  01000000000000000064006400850264036602190000000000000000006a
+                  01000000000000000064016401850264046602190000000000000000006a
                   020000000000000000a00300000000000000000000000000000000000000
                   007408000000000000000000006a050000000000000000a6010000ab0100
                   000000000000007c005f0800000000000000006e1623000100740f000000
-                  000000000000006404a6010000ab010000000000000000010059006e0378
-                  03590077017c026a01000000000000000064006400850264056406850266
+                  000000000000006405a6010000ab010000000000000000010059006e0378
+                  03590077017c026a01000000000000000064016401850264066407850266
                   02190000000000000000006a020000000000000000a00300000000000000
                   000000000000000000000000007408000000000000000000006a09000000
                   0000000000a6010000ab0100000000000000007d0309007c026a01000000
-                  000000000064006400850264076602190000000000000000006a02000000
+                  000000000064016401850264086602190000000000000000006a02000000
                   0000000000a0030000000000000000000000000000000000000000740800
                   0000000000000000006a090000000000000000a6010000ab010000000000
-                  0000007d046e3723000100740f000000000000000000006408a6010000ab
+                  0000007d046e3723000100740f000000000000000000006409a6010000ab
                   01000000000000000001007409000000000000000000006a0a0000000000
                   0000007417000000000000000000007c03a6010000ab0100000000000000
                   00a6010000ab0100000000000000007d0459006e03780359007701740900
                   0000000000000000006a0c00000000000000007c04a00d00000000000000
-                  000000000000000000000000006409640aa6020000ab0200000000000000
+                  00000000000000000000000000640a640ba6020000ab0200000000000000
                   007c036602a6010000ab0100000000000000007d057c057d067c065300
-                76           0 RESUME                   0
+               136           0 RESUME                   0
                
-                78           2 LOAD_FAST                0 (self)
+               141           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (read_traj)
                             26 LOAD_FAST                1 (nframe)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               2 (traj)
                
-                79          44 NOP
+               142          44 NOP
                
-                80          46 LOAD_FAST                2 (traj)
+               143          46 LOAD_FAST                2 (traj)
                             48 LOAD_ATTR                1 (loc)
-                            58 LOAD_CONST               0 (None)
-                            60 LOAD_CONST               0 (None)
+                            58 LOAD_CONST               1 (None)
+                            60 LOAD_CONST               1 (None)
                             62 BUILD_SLICE              2
-                            64 LOAD_CONST               1 ('mol')
+                            64 LOAD_CONST               2 ('mol')
                             66 BUILD_TUPLE              2
                             68 BINARY_SUBSCR
                             78 LOAD_ATTR                2 (values)
                             88 LOAD_METHOD              3 (astype)
                            110 LOAD_GLOBAL              8 (np)
                            122 LOAD_ATTR                5 (int64)
                            132 PRECALL                  1
                            136 CALL                     1
                            146 LOAD_FAST                0 (self)
                            148 STORE_ATTR               6 (mol)
                            158 JUMP_FORWARD            22 (to 204)
                        >>  160 PUSH_EXC_INFO
                
-                81         162 POP_TOP
+               144         162 POP_TOP
                
-                82         164 LOAD_GLOBAL             15 (NULL + print)
-                           176 LOAD_CONST               2 ('No molecule types in traj...')
+               145         164 LOAD_GLOBAL             15 (NULL + print)
+                           176 LOAD_CONST               3 ('No molecule types in traj...')
                            178 PRECALL                  1
                            182 CALL                     1
                            192 POP_TOP
                            194 POP_EXCEPT
                            196 JUMP_FORWARD             3 (to 204)
                        >>  198 COPY                     3
                            200 POP_EXCEPT
                            202 RERAISE                  1
                
-                84     >>  204 NOP
+               147     >>  204 NOP
                
-                85         206 LOAD_FAST                2 (traj)
+               148         206 LOAD_FAST                2 (traj)
                            208 LOAD_ATTR                1 (loc)
-                           218 LOAD_CONST               0 (None)
-                           220 LOAD_CONST               0 (None)
+                           218 LOAD_CONST               1 (None)
+                           220 LOAD_CONST               1 (None)
                            222 BUILD_SLICE              2
-                           224 LOAD_CONST               3 ('type')
+                           224 LOAD_CONST               4 ('type')
                            226 BUILD_TUPLE              2
                            228 BINARY_SUBSCR
                            238 LOAD_ATTR                2 (values)
                            248 LOAD_METHOD              3 (astype)
                            270 LOAD_GLOBAL              8 (np)
                            282 LOAD_ATTR                5 (int64)
                            292 PRECALL                  1
                            296 CALL                     1
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR               8 (atom)
                            318 JUMP_FORWARD            22 (to 364)
                        >>  320 PUSH_EXC_INFO
                
-                86         322 POP_TOP
+               149         322 POP_TOP
                
-                87         324 LOAD_GLOBAL             15 (NULL + print)
-                           336 LOAD_CONST               4 ('No atom types in traj...')
+               150         324 LOAD_GLOBAL             15 (NULL + print)
+                           336 LOAD_CONST               5 ('No atom types in traj...')
                            338 PRECALL                  1
                            342 CALL                     1
                            352 POP_TOP
                            354 POP_EXCEPT
                            356 JUMP_FORWARD             3 (to 364)
                        >>  358 COPY                     3
                            360 POP_EXCEPT
                            362 RERAISE                  1
                
-                89     >>  364 LOAD_FAST                2 (traj)
+               152     >>  364 LOAD_FAST                2 (traj)
                            366 LOAD_ATTR                1 (loc)
-                           376 LOAD_CONST               0 (None)
-                           378 LOAD_CONST               0 (None)
+                           376 LOAD_CONST               1 (None)
+                           378 LOAD_CONST               1 (None)
                            380 BUILD_SLICE              2
-                           382 LOAD_CONST               5 ('x')
-                           384 LOAD_CONST               6 ('z')
+                           382 LOAD_CONST               6 ('x')
+                           384 LOAD_CONST               7 ('z')
                            386 BUILD_SLICE              2
                            388 BUILD_TUPLE              2
                            390 BINARY_SUBSCR
                            400 LOAD_ATTR                2 (values)
                            410 LOAD_METHOD              3 (astype)
                            432 LOAD_GLOBAL              8 (np)
                            444 LOAD_ATTR                9 (float64)
                            454 PRECALL                  1
                            458 CALL                     1
                            468 STORE_FAST               3 (xyz)
                
-                91         470 NOP
+               154         470 NOP
                
-                92         472 LOAD_FAST                2 (traj)
+               155         472 LOAD_FAST                2 (traj)
                            474 LOAD_ATTR                1 (loc)
-                           484 LOAD_CONST               0 (None)
-                           486 LOAD_CONST               0 (None)
+                           484 LOAD_CONST               1 (None)
+                           486 LOAD_CONST               1 (None)
                            488 BUILD_SLICE              2
-                           490 LOAD_CONST               7 ('mass')
+                           490 LOAD_CONST               8 ('mass')
                            492 BUILD_TUPLE              2
                            494 BINARY_SUBSCR
                            504 LOAD_ATTR                2 (values)
                            514 LOAD_METHOD              3 (astype)
                            536 LOAD_GLOBAL              8 (np)
                            548 LOAD_ATTR                9 (float64)
                            558 PRECALL                  1
                            562 CALL                     1
                            572 STORE_FAST               4 (mass)
                            574 JUMP_FORWARD            55 (to 686)
                        >>  576 PUSH_EXC_INFO
                
-                93         578 POP_TOP
+               156         578 POP_TOP
                
-                94         580 LOAD_GLOBAL             15 (NULL + print)
-                           592 LOAD_CONST               8 ('No mass out in traj...')
+               157         580 LOAD_GLOBAL             15 (NULL + print)
+                           592 LOAD_CONST               9 ('No mass out in traj...')
                            594 PRECALL                  1
                            598 CALL                     1
                            608 POP_TOP
                
-                95         610 LOAD_GLOBAL              9 (NULL + np)
+               158         610 LOAD_GLOBAL              9 (NULL + np)
                            622 LOAD_ATTR               10 (zeros)
                            632 LOAD_GLOBAL             23 (NULL + len)
                            644 LOAD_FAST                3 (xyz)
                            646 PRECALL                  1
                            650 CALL                     1
                            660 PRECALL                  1
                            664 CALL                     1
                            674 STORE_FAST               4 (mass)
                            676 POP_EXCEPT
                            678 JUMP_FORWARD             3 (to 686)
                        >>  680 COPY                     3
                            682 POP_EXCEPT
                            684 RERAISE                  1
                
-                96     >>  686 LOAD_GLOBAL              9 (NULL + np)
+               159     >>  686 LOAD_GLOBAL              9 (NULL + np)
                            698 LOAD_ATTR               12 (hstack)
                            708 LOAD_FAST                4 (mass)
                            710 LOAD_METHOD             13 (reshape)
-                           732 LOAD_CONST               9 (-1)
-                           734 LOAD_CONST              10 (1)
+                           732 LOAD_CONST              10 (-1)
+                           734 LOAD_CONST              11 (1)
                            736 PRECALL                  2
                            740 CALL                     2
                            750 LOAD_FAST                3 (xyz)
                            752 BUILD_TUPLE              2
                            754 PRECALL                  1
                            758 CALL                     1
                            768 STORE_FAST               5 (mxyz)
                
-                98         770 LOAD_FAST                5 (mxyz)
+               161         770 LOAD_FAST                5 (mxyz)
                            772 STORE_FAST               6 (position)
                
-               100         774 LOAD_FAST                6 (position)
+               163         774 LOAD_FAST                6 (position)
                            776 RETURN_VALUE
                ExceptionTable:
                  46 to 156 -> 160 [0]
                  160 to 192 -> 198 [1] lasti
                  206 to 316 -> 320 [0]
                  320 to 352 -> 358 [1] lasti
                  472 to 572 -> 576 [0]
                  576 to 674 -> 680 [1] lasti
                consts
+                  '\n\t\tread mass, and x, y, z coordinates of nth frame from traj...\n\t\tnframe: number of frame \n\t\t'
                   None
                   'mol'
                   'No molecule types in traj...'
                   'type'
                   'No atom types in traj...'
                   'x'
                   'z'
@@ -1028,17 +1441,17 @@
                   1
                names      ('read_traj', 'loc', 'values', 'astype', 'np', 'int64', 'mol', 'print', 'atom', 'float64', 'zeros', 'len', 'hstack', 'reshape')
                varnames   ('self', 'nframe', 'traj', 'xyz', 'mass', 'mxyz', 'position')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'read_mxyz'
-               firstlineno 76
+               firstlineno 136
                lnotab
-                  0x02022a01020174010201280202017401020128026a0202016a0102011e
+                  0x02052a01020174010201280202017401020128026a0202016a0102011e
                   014c0154020402
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
@@ -1046,630 +1459,981 @@
                   007a0500007a0000007d027403000000000000000000006a020000000000
                   0000007c006a0300000000000000007c027c006a00000000000000000064
                   03ac04a6040000ab0400000000000000007d037409000000000000000000
                   0064057c006a050000000000000000a6020000ab02000000000000000001
                   00740d000000000000000000006a0700000000000000007c037c006a0500
                   00000000000000ac06a6020000ab0200000000000000007d037409000000
                   000000000000007c03a6010000ab01000000000000000001007c035300
-               102           0 RESUME                   0
+               165           0 RESUME                   0
                
-               104           2 LOAD_CONST               1 (9)
+               170           2 LOAD_CONST               1 (9)
                              4 LOAD_FAST                1 (nframe)
                              6 BINARY_OP                5 (*)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (atom_n)
                             22 LOAD_FAST                1 (nframe)
                             24 LOAD_CONST               2 (1)
                             26 BINARY_OP               10 (-)
                             30 BINARY_OP                5 (*)
                             34 BINARY_OP                0 (+)
                             38 STORE_FAST               2 (skip)
                
-               105          40 LOAD_GLOBAL              3 (NULL + np)
+               171          40 LOAD_GLOBAL              3 (NULL + np)
                             52 LOAD_ATTR                2 (loadtxt)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (f)
                             74 LOAD_FAST                2 (skip)
                             76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                0 (atom_n)
                             88 LOAD_CONST               3 ('str')
                             90 KW_NAMES                 4
                             92 PRECALL                  4
                             96 CALL                     4
                            106 STORE_FAST               3 (traj)
                
-               106         108 LOAD_GLOBAL              9 (NULL + print)
+               172         108 LOAD_GLOBAL              9 (NULL + print)
                            120 LOAD_CONST               5 ('Labels in traj is:')
                            122 LOAD_FAST                0 (self)
                            124 LOAD_ATTR                5 (col)
                            134 PRECALL                  2
                            138 CALL                     2
                            148 POP_TOP
                
-               107         150 LOAD_GLOBAL             13 (NULL + pd)
+               173         150 LOAD_GLOBAL             13 (NULL + pd)
                            162 LOAD_ATTR                7 (DataFrame)
                            172 LOAD_FAST                3 (traj)
                            174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                5 (col)
                            186 KW_NAMES                 6
                            188 PRECALL                  2
                            192 CALL                     2
                            202 STORE_FAST               3 (traj)
                
-               108         204 LOAD_GLOBAL              9 (NULL + print)
+               174         204 LOAD_GLOBAL              9 (NULL + print)
                            216 LOAD_FAST                3 (traj)
                            218 PRECALL                  1
                            222 CALL                     1
                            232 POP_TOP
                
-               109         234 LOAD_FAST                3 (traj)
+               175         234 LOAD_FAST                3 (traj)
                            236 RETURN_VALUE
                consts
-                  None
+                  '\n\t\tread data of nth frame from traj...\n\t\tnframe: number of frame \n\t\t'
                   9
                   1
                   'str'
                   ('skiprows', 'max_rows', 'dtype')
                   'Labels in traj is:'
                   ('columns',)
                names      ('atom_n', 'np', 'loadtxt', 'f', 'print', 'col', 'pd', 'DataFrame')
                varnames   ('self', 'nframe', 'skip', 'traj')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'read_traj'
-               firstlineno 102
-               lnotab 0x0202260144012a0136011e01
+               firstlineno 165
+               lnotab 0x0205260144012a0136011e01
             'mass'
+            'z'
             code
-               argcount  : 4
-               nlocals   : 18
-               stacksize : 5
+               argcount  : 6
+               nlocals   : 23
+               stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a01000000000000000064017a
-                  0800007a0500007d047c006a0200000000000000007c027a0b00007d057c
-                  0164006400850264026602190000000000000000007d0674070000000000
-                  00000000006a0400000000000000007c0664026b0200000000a6010000ab
-                  010000000000000000721264037d03740b000000000000000000006404a6
-                  010000ab01000000000000000001006e0264057d037c0164006400850264
-                  016602190000000000000000007d0767007d0867007d09740d0000000000
-                  00000000007c02a6010000ab01000000000000000044005db37d0a64027d
-                  0b7c006a0700000000000000007c057c0a7a0500007a0000007d0c7c006a
-                  0700000000000000007c057c0a64067a0000007a0500007a0000007d0d7c
-                  0c7c0d7a00000064077a0500007d0e740d000000000000000000007c006a
-                  080000000000000000a6010000ab01000000000000000044005d317d0f7c
-                  077c0f190000000000000000007c0c6b050000000072237c077c0f190000
-                  000000000000007c0d6b010000000072177c0364056b0200000000720c7c
-                  067c0f190000000000000000007c0b7a0000007d0b8c2c7c0b64067a0000
-                  007d0b8c327c006a0900000000000000007c006a0a00000000000000007a
-                  0500007c057a0500007c047a0500007d107c0b7c107a0b00007d117c08a0
-                  0b00000000000000000000000000000000000000007c11a6010000ab0100
-                  0000000000000001007c09a00b0000000000000000000000000000000000
-                  0000007c0ea6010000ab01000000000000000001008cb474070000000000
-                  00000000006a0c00000000000000007c09a6010000ab0100000000000000
-                  00a00d000000000000000000000000000000000000000064086406a60200
-                  00ab0200000000000000007d097407000000000000000000006a0c000000
-                  00000000007c08a6010000ab010000000000000000a00d00000000000000
-                  0000000000000000000000000064086406a6020000ab0200000000000000
-                  007d087c097c0866025300
-               111           0 RESUME                   0
+                  0800007a0500007d067c0564026b020000000073067c0564036b02000000
+                  0072337c006a0200000000000000007c027a0b00007d077c016404640485
+                  0264016602190000000000000000007d087c006a0300000000000000007d
+                  097c006a0400000000000000007c006a0500000000000000007a0500007c
+                  077a0500007c067a0500007d0a6e7d7c0564056b020000000073067c0564
+                  066b020000000072337c006a0500000000000000007c027a0b00007d077c
+                  0164046404850264076602190000000000000000007d087c006a06000000
+                  00000000007d097c006a0400000000000000007c006a0200000000000000
+                  007a0500007c077a0500007c067a0500007d0a6e3e7c0564086b02000000
+                  0073067c0564096b020000000072327c006a0400000000000000007c027a
+                  0b00007d077c01640464048502640a6602190000000000000000007d087c
+                  006a0700000000000000007d097c006a0500000000000000007c006a0200
+                  000000000000007a0500007c077a0500007c067a0500007d0a7411000000
+                  000000000000007c03a00900000000000000000000000000000000000000
+                  00a6000000ab000000000000000000a6010000ab0100000000000000007d
+                  0b7415000000000000000000007417000000000000000000007c006a0c00
+                  00000000000000a6010000ab010000000000000000a6010000ab01000000
+                  000000000044005d4b7d0c74150000000000000000000074170000000000
+                  00000000007c0ba6010000ab010000000000000000a6010000ab01000000
+                  000000000044005d2c7d0d7c006a0c00000000000000007c0c1900000000
+                  00000000007c0b7c0d190000000000000000006b020000000072137c037c
+                  0b7c0d19000000000000000000190000000000000000007c017c0c640b66
+                  023c0000008c2d8c4c7c01640464048502640b6602190000000000000000
+                  007d0e741b000000000000000000006a0e00000000000000007c0e640b6b
+                  0200000000a6010000ab0100000000000000007212640c7d04741f000000
+                  00000000000000640da6010000ab01000000000000000001006e02640e7d
+                  0467007d0f67007d107415000000000000000000007c02a6010000ab0100
+                  0000000000000044005d947d11640b7d127c097c077c117a0500007a0000
+                  007d137c097c077c11640a7a0000007a0500007a0000007d147c137c147a
+                  000000640f7a0500007d157415000000000000000000007c006a10000000
+                  0000000000a6010000ab01000000000000000044005d317d0c7c087c0c19
+                  0000000000000000007c136b050000000072237c087c0c19000000000000
+                  0000007c146b010000000072177c04640e6b0200000000720c7c0e7c0c19
+                  0000000000000000007c127a0000007d128c2c7c12640a7a0000007d128c
+                  327c127c0a7a0b00007d167c0fa011000000000000000000000000000000
+                  00000000007c16a6010000ab01000000000000000001007c10a011000000
+                  00000000000000000000000000000000007c15a6010000ab010000000000
+                  00000001008c95741b000000000000000000006a1200000000000000007c
+                  10a6010000ab010000000000000000a01300000000000000000000000000
+                  000000000000006410640aa6020000ab0200000000000000007d10741b00
+                  0000000000000000006a1200000000000000007c0fa6010000ab01000000
+                  0000000000a0130000000000000000000000000000000000000000641064
+                  0aa6020000ab0200000000000000007d0f7c107c0f66025300
+               177           0 RESUME                   0
                
-               113           2 LOAD_FAST                0 (self)
+               186           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (amu2g)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (A2CM)
                             26 LOAD_CONST               1 (3)
                             28 BINARY_OP                8 (**)
                             32 BINARY_OP                5 (*)
-                            36 STORE_FAST               4 (unitconvert)
-               
-               114          38 LOAD_FAST                0 (self)
-                            40 LOAD_ATTR                2 (Lz)
-                            50 LOAD_FAST                2 (Nz)
-                            52 BINARY_OP               11 (/)
-                            56 STORE_FAST               5 (dZ)
-               
-               115          58 LOAD_FAST                1 (mxyz)
-                            60 LOAD_CONST               0 (None)
-                            62 LOAD_CONST               0 (None)
-                            64 BUILD_SLICE              2
-                            66 LOAD_CONST               2 (0)
-                            68 BUILD_TUPLE              2
-                            70 BINARY_SUBSCR
-                            80 STORE_FAST               6 (MW)
-               
-               116          82 LOAD_GLOBAL              7 (NULL + np)
-                            94 LOAD_ATTR                4 (all)
-                           104 LOAD_FAST                6 (MW)
-                           106 LOAD_CONST               2 (0)
-                           108 COMPARE_OP               2 (==)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 POP_JUMP_FORWARD_IF_FALSE    18 (to 166)
-               
-               117         130 LOAD_CONST               3 ('number')
-                           132 STORE_FAST               3 (density_type)
-               
-               118         134 LOAD_GLOBAL             11 (NULL + print)
-                           146 LOAD_CONST               4 ('\nNo provided mass, will calculate number density!\n')
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 POP_TOP
-                           164 JUMP_FORWARD             2 (to 170)
-               
-               120     >>  166 LOAD_CONST               5 ('mass')
-                           168 STORE_FAST               3 (density_type)
-               
-               122     >>  170 LOAD_FAST                1 (mxyz)
-                           172 LOAD_CONST               0 (None)
-                           174 LOAD_CONST               0 (None)
-                           176 BUILD_SLICE              2
-                           178 LOAD_CONST               1 (3)
-                           180 BUILD_TUPLE              2
-                           182 BINARY_SUBSCR
-                           192 STORE_FAST               7 (Z)
+                            36 STORE_FAST               6 (unitconvert)
                
-               123         194 BUILD_LIST               0
-                           196 STORE_FAST               8 (rho_n)
+               187          38 LOAD_FAST                5 (direction)
+                            40 LOAD_CONST               2 ('z')
+                            42 COMPARE_OP               2 (==)
+                            48 POP_JUMP_FORWARD_IF_TRUE     6 (to 62)
+                            50 LOAD_FAST                5 (direction)
+                            52 LOAD_CONST               3 ('Z')
+                            54 COMPARE_OP               2 (==)
+                            60 POP_JUMP_FORWARD_IF_FALSE    51 (to 164)
+               
+               188     >>   62 LOAD_FAST                0 (self)
+                            64 LOAD_ATTR                2 (Lz)
+                            74 LOAD_FAST                2 (Nbin)
+                            76 BINARY_OP               11 (/)
+                            80 STORE_FAST               7 (dr)
+               
+               189          82 LOAD_FAST                1 (mxyz)
+                            84 LOAD_CONST               4 (None)
+                            86 LOAD_CONST               4 (None)
+                            88 BUILD_SLICE              2
+                            90 LOAD_CONST               1 (3)
+                            92 BUILD_TUPLE              2
+                            94 BINARY_SUBSCR
+                           104 STORE_FAST               8 (L)
+               
+               190         106 LOAD_FAST                0 (self)
+                           108 LOAD_ATTR                3 (zlo)
+                           118 STORE_FAST               9 (lo)
+               
+               191         120 LOAD_FAST                0 (self)
+                           122 LOAD_ATTR                4 (Lx)
+                           132 LOAD_FAST                0 (self)
+                           134 LOAD_ATTR                5 (Ly)
+                           144 BINARY_OP                5 (*)
+                           148 LOAD_FAST                7 (dr)
+                           150 BINARY_OP                5 (*)
+                           154 LOAD_FAST                6 (unitconvert)
+                           156 BINARY_OP                5 (*)
+                           160 STORE_FAST              10 (vlo)
+                           162 JUMP_FORWARD           125 (to 414)
                
-               124         198 BUILD_LIST               0
-                           200 STORE_FAST               9 (zc_n)
+               192     >>  164 LOAD_FAST                5 (direction)
+                           166 LOAD_CONST               5 ('y')
+                           168 COMPARE_OP               2 (==)
+                           174 POP_JUMP_FORWARD_IF_TRUE     6 (to 188)
+                           176 LOAD_FAST                5 (direction)
+                           178 LOAD_CONST               6 ('Y')
+                           180 COMPARE_OP               2 (==)
+                           186 POP_JUMP_FORWARD_IF_FALSE    51 (to 290)
+               
+               193     >>  188 LOAD_FAST                0 (self)
+                           190 LOAD_ATTR                5 (Ly)
+                           200 LOAD_FAST                2 (Nbin)
+                           202 BINARY_OP               11 (/)
+                           206 STORE_FAST               7 (dr)
+               
+               194         208 LOAD_FAST                1 (mxyz)
+                           210 LOAD_CONST               4 (None)
+                           212 LOAD_CONST               4 (None)
+                           214 BUILD_SLICE              2
+                           216 LOAD_CONST               7 (2)
+                           218 BUILD_TUPLE              2
+                           220 BINARY_SUBSCR
+                           230 STORE_FAST               8 (L)
+               
+               195         232 LOAD_FAST                0 (self)
+                           234 LOAD_ATTR                6 (ylo)
+                           244 STORE_FAST               9 (lo)
+               
+               196         246 LOAD_FAST                0 (self)
+                           248 LOAD_ATTR                4 (Lx)
+                           258 LOAD_FAST                0 (self)
+                           260 LOAD_ATTR                2 (Lz)
+                           270 BINARY_OP                5 (*)
+                           274 LOAD_FAST                7 (dr)
+                           276 BINARY_OP                5 (*)
+                           280 LOAD_FAST                6 (unitconvert)
+                           282 BINARY_OP                5 (*)
+                           286 STORE_FAST              10 (vlo)
+                           288 JUMP_FORWARD            62 (to 414)
+               
+               197     >>  290 LOAD_FAST                5 (direction)
+                           292 LOAD_CONST               8 ('x')
+                           294 COMPARE_OP               2 (==)
+                           300 POP_JUMP_FORWARD_IF_TRUE     6 (to 314)
+                           302 LOAD_FAST                5 (direction)
+                           304 LOAD_CONST               9 ('X')
+                           306 COMPARE_OP               2 (==)
+                           312 POP_JUMP_FORWARD_IF_FALSE    50 (to 414)
+               
+               198     >>  314 LOAD_FAST                0 (self)
+                           316 LOAD_ATTR                4 (Lx)
+                           326 LOAD_FAST                2 (Nbin)
+                           328 BINARY_OP               11 (/)
+                           332 STORE_FAST               7 (dr)
+               
+               199         334 LOAD_FAST                1 (mxyz)
+                           336 LOAD_CONST               4 (None)
+                           338 LOAD_CONST               4 (None)
+                           340 BUILD_SLICE              2
+                           342 LOAD_CONST              10 (1)
+                           344 BUILD_TUPLE              2
+                           346 BINARY_SUBSCR
+                           356 STORE_FAST               8 (L)
+               
+               200         358 LOAD_FAST                0 (self)
+                           360 LOAD_ATTR                7 (xlo)
+                           370 STORE_FAST               9 (lo)
+               
+               201         372 LOAD_FAST                0 (self)
+                           374 LOAD_ATTR                5 (Ly)
+                           384 LOAD_FAST                0 (self)
+                           386 LOAD_ATTR                2 (Lz)
+                           396 BINARY_OP                5 (*)
+                           400 LOAD_FAST                7 (dr)
+                           402 BINARY_OP                5 (*)
+                           406 LOAD_FAST                6 (unitconvert)
+                           408 BINARY_OP                5 (*)
+                           412 STORE_FAST              10 (vlo)
+               
+               203     >>  414 LOAD_GLOBAL             17 (NULL + list)
+                           426 LOAD_FAST                3 (mass_dict)
+                           428 LOAD_METHOD              9 (keys)
+                           450 PRECALL                  0
+                           454 CALL                     0
+                           464 PRECALL                  1
+                           468 CALL                     1
+                           478 STORE_FAST              11 (mass_key)
+               
+               204         480 LOAD_GLOBAL             21 (NULL + range)
+                           492 LOAD_GLOBAL             23 (NULL + len)
+                           504 LOAD_FAST                0 (self)
+                           506 LOAD_ATTR               12 (atom)
+                           516 PRECALL                  1
+                           520 CALL                     1
+                           530 PRECALL                  1
+                           534 CALL                     1
+                           544 GET_ITER
+                       >>  546 FOR_ITER                75 (to 698)
+                           548 STORE_FAST              12 (i)
+               
+               205         550 LOAD_GLOBAL             21 (NULL + range)
+                           562 LOAD_GLOBAL             23 (NULL + len)
+                           574 LOAD_FAST               11 (mass_key)
+                           576 PRECALL                  1
+                           580 CALL                     1
+                           590 PRECALL                  1
+                           594 CALL                     1
+                           604 GET_ITER
+                       >>  606 FOR_ITER                44 (to 696)
+                           608 STORE_FAST              13 (j)
+               
+               206         610 LOAD_FAST                0 (self)
+                           612 LOAD_ATTR               12 (atom)
+                           622 LOAD_FAST               12 (i)
+                           624 BINARY_SUBSCR
+                           634 LOAD_FAST               11 (mass_key)
+                           636 LOAD_FAST               13 (j)
+                           638 BINARY_SUBSCR
+                           648 COMPARE_OP               2 (==)
+                           654 POP_JUMP_FORWARD_IF_FALSE    19 (to 694)
+               
+               207         656 LOAD_FAST                3 (mass_dict)
+                           658 LOAD_FAST               11 (mass_key)
+                           660 LOAD_FAST               13 (j)
+                           662 BINARY_SUBSCR
+                           672 BINARY_SUBSCR
+                           682 LOAD_FAST                1 (mxyz)
+                           684 LOAD_FAST               12 (i)
+                           686 LOAD_CONST              11 (0)
+                           688 BUILD_TUPLE              2
+                           690 STORE_SUBSCR
+                       >>  694 JUMP_BACKWARD           45 (to 606)
+               
+               205     >>  696 JUMP_BACKWARD           76 (to 546)
+               
+               208     >>  698 LOAD_FAST                1 (mxyz)
+                           700 LOAD_CONST               4 (None)
+                           702 LOAD_CONST               4 (None)
+                           704 BUILD_SLICE              2
+                           706 LOAD_CONST              11 (0)
+                           708 BUILD_TUPLE              2
+                           710 BINARY_SUBSCR
+                           720 STORE_FAST              14 (MW)
+               
+               210         722 LOAD_GLOBAL             27 (NULL + np)
+                           734 LOAD_ATTR               14 (all)
+                           744 LOAD_FAST               14 (MW)
+                           746 LOAD_CONST              11 (0)
+                           748 COMPARE_OP               2 (==)
+                           754 PRECALL                  1
+                           758 CALL                     1
+                           768 POP_JUMP_FORWARD_IF_FALSE    18 (to 806)
                
-               126         202 LOAD_GLOBAL             13 (NULL + range)
-                           214 LOAD_FAST                2 (Nz)
-                           216 PRECALL                  1
-                           220 CALL                     1
-                           230 GET_ITER
-                       >>  232 FOR_ITER               179 (to 592)
-                           234 STORE_FAST              10 (n)
-               
-               127         236 LOAD_CONST               2 (0)
-                           238 STORE_FAST              11 (mass_n)
-               
-               128         240 LOAD_FAST                0 (self)
-                           242 LOAD_ATTR                7 (zlo)
-                           252 LOAD_FAST                5 (dZ)
-                           254 LOAD_FAST               10 (n)
-                           256 BINARY_OP                5 (*)
-                           260 BINARY_OP                0 (+)
-                           264 STORE_FAST              12 (z0)
-               
-               129         266 LOAD_FAST                0 (self)
-                           268 LOAD_ATTR                7 (zlo)
-                           278 LOAD_FAST                5 (dZ)
-                           280 LOAD_FAST               10 (n)
-                           282 LOAD_CONST               6 (1)
-                           284 BINARY_OP                0 (+)
-                           288 BINARY_OP                5 (*)
-                           292 BINARY_OP                0 (+)
-                           296 STORE_FAST              13 (z1)
-               
-               130         298 LOAD_FAST               12 (z0)
-                           300 LOAD_FAST               13 (z1)
-                           302 BINARY_OP                0 (+)
-                           306 LOAD_CONST               7 (0.5)
-                           308 BINARY_OP                5 (*)
-                           312 STORE_FAST              14 (zc)
-               
-               132         314 LOAD_GLOBAL             13 (NULL + range)
-                           326 LOAD_FAST                0 (self)
-                           328 LOAD_ATTR                8 (atom_n)
-                           338 PRECALL                  1
-                           342 CALL                     1
-                           352 GET_ITER
-                       >>  354 FOR_ITER                49 (to 454)
-                           356 STORE_FAST              15 (i)
-               
-               134         358 LOAD_FAST                7 (Z)
-                           360 LOAD_FAST               15 (i)
-                           362 BINARY_SUBSCR
-                           372 LOAD_FAST               12 (z0)
-                           374 COMPARE_OP               5 (>=)
-                           380 POP_JUMP_FORWARD_IF_FALSE    35 (to 452)
-                           382 LOAD_FAST                7 (Z)
-                           384 LOAD_FAST               15 (i)
-                           386 BINARY_SUBSCR
-                           396 LOAD_FAST               13 (z1)
-                           398 COMPARE_OP               1 (<=)
-                           404 POP_JUMP_FORWARD_IF_FALSE    23 (to 452)
-               
-               135         406 LOAD_FAST                3 (density_type)
-                           408 LOAD_CONST               5 ('mass')
-                           410 COMPARE_OP               2 (==)
-                           416 POP_JUMP_FORWARD_IF_FALSE    12 (to 442)
-               
-               136         418 LOAD_FAST                6 (MW)
-                           420 LOAD_FAST               15 (i)
-                           422 BINARY_SUBSCR
-                           432 LOAD_FAST               11 (mass_n)
-                           434 BINARY_OP                0 (+)
-                           438 STORE_FAST              11 (mass_n)
-                           440 JUMP_BACKWARD           44 (to 354)
-               
-               138     >>  442 LOAD_FAST               11 (mass_n)
-                           444 LOAD_CONST               6 (1)
-                           446 BINARY_OP                0 (+)
-                           450 STORE_FAST              11 (mass_n)
-                       >>  452 JUMP_BACKWARD           50 (to 354)
-               
-               140     >>  454 LOAD_FAST                0 (self)
-                           456 LOAD_ATTR                9 (Lx)
-                           466 LOAD_FAST                0 (self)
-                           468 LOAD_ATTR               10 (Ly)
-                           478 BINARY_OP                5 (*)
-                           482 LOAD_FAST                5 (dZ)
-                           484 BINARY_OP                5 (*)
-                           488 LOAD_FAST                4 (unitconvert)
-                           490 BINARY_OP                5 (*)
-                           494 STORE_FAST              16 (vlo)
-               
-               142         496 LOAD_FAST               11 (mass_n)
-                           498 LOAD_FAST               16 (vlo)
-                           500 BINARY_OP               11 (/)
-                           504 STORE_FAST              17 (rho)
-               
-               144         506 LOAD_FAST                8 (rho_n)
-                           508 LOAD_METHOD             11 (append)
-                           530 LOAD_FAST               17 (rho)
-                           532 PRECALL                  1
-                           536 CALL                     1
-                           546 POP_TOP
+               211         770 LOAD_CONST              12 ('number')
+                           772 STORE_FAST               4 (density_type)
                
-               145         548 LOAD_FAST                9 (zc_n)
-                           550 LOAD_METHOD             11 (append)
-                           572 LOAD_FAST               14 (zc)
-                           574 PRECALL                  1
-                           578 CALL                     1
-                           588 POP_TOP
-                           590 JUMP_BACKWARD          180 (to 232)
-               
-               146     >>  592 LOAD_GLOBAL              7 (NULL + np)
-                           604 LOAD_ATTR               12 (array)
-                           614 LOAD_FAST                9 (zc_n)
-                           616 PRECALL                  1
-                           620 CALL                     1
-                           630 LOAD_METHOD             13 (reshape)
-                           652 LOAD_CONST               8 (-1)
-                           654 LOAD_CONST               6 (1)
-                           656 PRECALL                  2
-                           660 CALL                     2
-                           670 STORE_FAST               9 (zc_n)
-               
-               147         672 LOAD_GLOBAL              7 (NULL + np)
-                           684 LOAD_ATTR               12 (array)
-                           694 LOAD_FAST                8 (rho_n)
-                           696 PRECALL                  1
-                           700 CALL                     1
-                           710 LOAD_METHOD             13 (reshape)
-                           732 LOAD_CONST               8 (-1)
-                           734 LOAD_CONST               6 (1)
-                           736 PRECALL                  2
-                           740 CALL                     2
-                           750 STORE_FAST               8 (rho_n)
+               212         774 LOAD_GLOBAL             31 (NULL + print)
+                           786 LOAD_CONST              13 ('\nNo provided mass, will calculate number density!\n')
+                           788 PRECALL                  1
+                           792 CALL                     1
+                           802 POP_TOP
+                           804 JUMP_FORWARD             2 (to 810)
+               
+               214     >>  806 LOAD_CONST              14 ('mass')
+                           808 STORE_FAST               4 (density_type)
+               
+               216     >>  810 BUILD_LIST               0
+                           812 STORE_FAST              15 (rho_n)
+               
+               217         814 BUILD_LIST               0
+                           816 STORE_FAST              16 (lc_n)
+               
+               218         818 LOAD_GLOBAL             21 (NULL + range)
+                           830 LOAD_FAST                2 (Nbin)
+                           832 PRECALL                  1
+                           836 CALL                     1
+                           846 GET_ITER
+                       >>  848 FOR_ITER               148 (to 1146)
+                           850 STORE_FAST              17 (n)
+               
+               219         852 LOAD_CONST              11 (0)
+                           854 STORE_FAST              18 (mass_n)
+               
+               220         856 LOAD_FAST                9 (lo)
+                           858 LOAD_FAST                7 (dr)
+                           860 LOAD_FAST               17 (n)
+                           862 BINARY_OP                5 (*)
+                           866 BINARY_OP                0 (+)
+                           870 STORE_FAST              19 (l0)
+               
+               221         872 LOAD_FAST                9 (lo)
+                           874 LOAD_FAST                7 (dr)
+                           876 LOAD_FAST               17 (n)
+                           878 LOAD_CONST              10 (1)
+                           880 BINARY_OP                0 (+)
+                           884 BINARY_OP                5 (*)
+                           888 BINARY_OP                0 (+)
+                           892 STORE_FAST              20 (l1)
+               
+               222         894 LOAD_FAST               19 (l0)
+                           896 LOAD_FAST               20 (l1)
+                           898 BINARY_OP                0 (+)
+                           902 LOAD_CONST              15 (0.5)
+                           904 BINARY_OP                5 (*)
+                           908 STORE_FAST              21 (lc)
                
-               149         752 LOAD_FAST                9 (zc_n)
-                           754 LOAD_FAST                8 (rho_n)
-                           756 BUILD_TUPLE              2
-                           758 RETURN_VALUE
+               223         910 LOAD_GLOBAL             21 (NULL + range)
+                           922 LOAD_FAST                0 (self)
+                           924 LOAD_ATTR               16 (atom_n)
+                           934 PRECALL                  1
+                           938 CALL                     1
+                           948 GET_ITER
+                       >>  950 FOR_ITER                49 (to 1050)
+                           952 STORE_FAST              12 (i)
+               
+               224         954 LOAD_FAST                8 (L)
+                           956 LOAD_FAST               12 (i)
+                           958 BINARY_SUBSCR
+                           968 LOAD_FAST               19 (l0)
+                           970 COMPARE_OP               5 (>=)
+                           976 POP_JUMP_FORWARD_IF_FALSE    35 (to 1048)
+                           978 LOAD_FAST                8 (L)
+                           980 LOAD_FAST               12 (i)
+                           982 BINARY_SUBSCR
+                           992 LOAD_FAST               20 (l1)
+                           994 COMPARE_OP               1 (<=)
+                          1000 POP_JUMP_FORWARD_IF_FALSE    23 (to 1048)
+               
+               225        1002 LOAD_FAST                4 (density_type)
+                          1004 LOAD_CONST              14 ('mass')
+                          1006 COMPARE_OP               2 (==)
+                          1012 POP_JUMP_FORWARD_IF_FALSE    12 (to 1038)
+               
+               226        1014 LOAD_FAST               14 (MW)
+                          1016 LOAD_FAST               12 (i)
+                          1018 BINARY_SUBSCR
+                          1028 LOAD_FAST               18 (mass_n)
+                          1030 BINARY_OP                0 (+)
+                          1034 STORE_FAST              18 (mass_n)
+                          1036 JUMP_BACKWARD           44 (to 950)
+               
+               228     >> 1038 LOAD_FAST               18 (mass_n)
+                          1040 LOAD_CONST              10 (1)
+                          1042 BINARY_OP                0 (+)
+                          1046 STORE_FAST              18 (mass_n)
+                       >> 1048 JUMP_BACKWARD           50 (to 950)
+               
+               229     >> 1050 LOAD_FAST               18 (mass_n)
+                          1052 LOAD_FAST               10 (vlo)
+                          1054 BINARY_OP               11 (/)
+                          1058 STORE_FAST              22 (rho)
+               
+               231        1060 LOAD_FAST               15 (rho_n)
+                          1062 LOAD_METHOD             17 (append)
+                          1084 LOAD_FAST               22 (rho)
+                          1086 PRECALL                  1
+                          1090 CALL                     1
+                          1100 POP_TOP
+               
+               232        1102 LOAD_FAST               16 (lc_n)
+                          1104 LOAD_METHOD             17 (append)
+                          1126 LOAD_FAST               21 (lc)
+                          1128 PRECALL                  1
+                          1132 CALL                     1
+                          1142 POP_TOP
+                          1144 JUMP_BACKWARD          149 (to 848)
+               
+               233     >> 1146 LOAD_GLOBAL             27 (NULL + np)
+                          1158 LOAD_ATTR               18 (array)
+                          1168 LOAD_FAST               16 (lc_n)
+                          1170 PRECALL                  1
+                          1174 CALL                     1
+                          1184 LOAD_METHOD             19 (reshape)
+                          1206 LOAD_CONST              16 (-1)
+                          1208 LOAD_CONST              10 (1)
+                          1210 PRECALL                  2
+                          1214 CALL                     2
+                          1224 STORE_FAST              16 (lc_n)
+               
+               234        1226 LOAD_GLOBAL             27 (NULL + np)
+                          1238 LOAD_ATTR               18 (array)
+                          1248 LOAD_FAST               15 (rho_n)
+                          1250 PRECALL                  1
+                          1254 CALL                     1
+                          1264 LOAD_METHOD             19 (reshape)
+                          1286 LOAD_CONST              16 (-1)
+                          1288 LOAD_CONST              10 (1)
+                          1290 PRECALL                  2
+                          1294 CALL                     2
+                          1304 STORE_FAST              15 (rho_n)
+               
+               236        1306 LOAD_FAST               16 (lc_n)
+                          1308 LOAD_FAST               15 (rho_n)
+                          1310 BUILD_TUPLE              2
+                          1312 RETURN_VALUE
                consts
-                  None
+                  '\n\t\tcalculating density of all atoms......\n\t\tmxyz: array of mass, x, y, and z;\n\t\tNbin: number of bins in x/y/z-axis\n\t\tmass_dict: masses of atoms ,default={} \n\t\tdensity_type: calculated type of density \n\t\t'
                   3
+                  'z'
+                  'Z'
+                  None
+                  'y'
+                  'Y'
+                  2
+                  'x'
+                  'X'
+                  1
                   0
                   'number'
                   '\nNo provided mass, will calculate number density!\n'
                   'mass'
-                  1
                   0.5
                   -1
-               names      ('amu2g', 'A2CM', 'Lz', 'np', 'all', 'print', 'range', 'zlo', 'atom_n', 'Lx', 'Ly', 'append', 'array', 'reshape')
-               varnames   ('self', 'mxyz', 'Nz', 'density_type', 'unitconvert', 'dZ', 'MW', 'Z', 'rho_n', 'zc_n', 'n', 'mass_n', 'z0', 'z1', 'zc', 'i', 'vlo', 'rho')
+               names      ('amu2g', 'A2CM', 'Lz', 'zlo', 'Lx', 'Ly', 'ylo', 'xlo', 'list', 'keys', 'range', 'len', 'atom', 'np', 'all', 'print', 'atom_n', 'append', 'array', 'reshape')
+               varnames   ('self', 'mxyz', 'Nbin', 'mass_dict', 'density_type', 'direction', 'unitconvert', 'dr', 'L', 'lo', 'vlo', 'mass_key', 'i', 'j', 'MW', 'rho_n', 'lc_n', 'n', 'mass_n', 'l0', 'l1', 'lc', 'rho')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'oneframe_alldensity'
-               firstlineno 111
+               firstlineno 177
                lnotab
-                  0x02022401140118013001040120020402180104010402220104011a0120
-                  0110022c0230010c0118020c022a020a022a012c0150015002
+                  0x020924011801140118010e012c011801140118010e012c011801140118
+                  010e012a02420146013c012e0128fe020318023001040120020402040104
+                  01220104011001160110012c0130010c0118020c010a022a012c01500150
+                  02
             'mol'
             code
-               argcount  : 6
-               nlocals   : 21
-               stacksize : 5
+               argcount  : 8
+               nlocals   : 26
+               stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a01000000000000000064017a
-                  0800007a0500007d067c006a0200000000000000007c027a0b00007d077c
-                  0164006400850264026602190000000000000000007d0874070000000000
-                  00000000006a0400000000000000007c0864026b0200000000a6010000ab
-                  010000000000000000721264037d05740b000000000000000000006404a6
-                  010000ab01000000000000000001006e0264057d057c0164006400850264
-                  016602190000000000000000007d0967007d0a67007d0b7c0464066b0200
-                  00000072087c006a0600000000000000007d0c6e0d7c0464076b02000000
-                  0072077c006a0700000000000000007d0c7411000000000000000000007c
-                  02a6010000ab01000000000000000044005dd77d0d64027d0e7c006a0900
-                  000000000000007c077c0d7a0500007a0000007d0f7c006a090000000000
-                  0000007c077c0d64087a0000007a0500007a0000007d107c0f7c107a0000
-                  0064097a0500007d117411000000000000000000007c006a0a0000000000
-                  000000a6010000ab01000000000000000044005d557d127c0c7c12190000
-                  000000000000007c036402190000000000000000006b050000000072417c
-                  0c7c12190000000000000000007c036408190000000000000000006b0100
-                  000000722f7c097c12190000000000000000007c0f6b050000000072237c
-                  097c12190000000000000000007c106b010000000072177c0564056b0200
-                  000000720c7c087c12190000000000000000007c0e7a0000007d0e8c507c
-                  0e64087a0000007d0e8c567c006a0b00000000000000007c006a0c000000
-                  00000000007a0500007c077a0500007c067a0500007d137c0e7c137a0b00
-                  007d147c0aa00d00000000000000000000000000000000000000007c14a6
-                  010000ab01000000000000000001007c0ba00d0000000000000000000000
-                  0000000000000000007c11a6010000ab01000000000000000001008cd874
-                  07000000000000000000006a0e00000000000000007c0ba6010000ab0100
-                  00000000000000a00f000000000000000000000000000000000000000064
-                  0a6408a6020000ab0200000000000000007d0b7407000000000000000000
-                  006a0e00000000000000007c0aa6010000ab010000000000000000a00f00
-                  00000000000000000000000000000000000000640a6408a6020000ab0200
-                  000000000000007d0a7c0b7c0a66025300
-               151           0 RESUME                   0
+                  0800007a0500007d087c0764026b020000000073067c0764036b02000000
+                  0072337c006a0200000000000000007c027a0b00007d097c016404640485
+                  0264016602190000000000000000007d0a7c006a0300000000000000007d
+                  0b7c006a0400000000000000007c006a0500000000000000007a0500007c
+                  097a0500007c087a0500007d0c6e7d7c0764056b020000000073067c0764
+                  066b020000000072337c006a0500000000000000007c027a0b00007d097c
+                  0164046404850264076602190000000000000000007d0a7c006a06000000
+                  00000000007d0b7c006a0400000000000000007c006a0200000000000000
+                  007a0500007c097a0500007c087a0500007d0c6e3e7c0764086b02000000
+                  0073067c0764096b020000000072327c006a0400000000000000007c027a
+                  0b00007d097c01640464048502640a6602190000000000000000007d0a7c
+                  006a0700000000000000007d0b7c006a0500000000000000007c006a0200
+                  000000000000007a0500007c097a0500007c087a0500007d0c7411000000
+                  000000000000007c04a00900000000000000000000000000000000000000
+                  00a6000000ab000000000000000000a6010000ab0100000000000000007d
+                  0d7415000000000000000000007417000000000000000000007c006a0c00
+                  00000000000000a6010000ab010000000000000000a6010000ab01000000
+                  000000000044005d4b7d0e74150000000000000000000074170000000000
+                  00000000007c0da6010000ab010000000000000000a6010000ab01000000
+                  000000000044005d2c7d0f7c006a0c00000000000000007c0e1900000000
+                  00000000007c0d7c0f190000000000000000006b020000000072137c047c
+                  0d7c0f19000000000000000000190000000000000000007c017c0e640b66
+                  023c0000008c2d8c4c7c01640464048502640b6602190000000000000000
+                  007d10741b000000000000000000006a0e00000000000000007c10640b6b
+                  0200000000a6010000ab0100000000000000007212640c7d06741f000000
+                  00000000000000640da6010000ab01000000000000000001006e02640e7d
+                  0667007d1167007d127c05640f6b020000000072087c006a100000000000
+                  0000007d136e0d7c0564106b020000000072077c006a0c00000000000000
+                  007d137415000000000000000000007c02a6010000ab0100000000000000
+                  0044005db87d14640b7d157c0b7c097c147a0500007a0000007d167c0b7c
+                  097c14640a7a0000007a0500007a0000007d177c167c177a00000064117a
+                  0500007d187415000000000000000000007c006a110000000000000000a6
+                  010000ab01000000000000000044005d557d0e7c137c0e19000000000000
+                  0000007c03640b190000000000000000006b050000000072417c137c0e19
+                  0000000000000000007c03640a190000000000000000006b010000000072
+                  2f7c0a7c0e190000000000000000007c166b050000000072237c0a7c0e19
+                  0000000000000000007c176b010000000072177c06640e6b020000000072
+                  0c7c107c0e190000000000000000007c157a0000007d158c507c15640a7a
+                  0000007d158c567c157c0c7a0b00007d197c11a012000000000000000000
+                  00000000000000000000007c19a6010000ab01000000000000000001007c
+                  12a01200000000000000000000000000000000000000007c18a6010000ab
+                  01000000000000000001008cb9741b000000000000000000006a13000000
+                  00000000007c12a6010000ab010000000000000000a01400000000000000
+                  000000000000000000000000006412640aa6020000ab0200000000000000
+                  007d12741b000000000000000000006a1300000000000000007c11a60100
+                  00ab010000000000000000a0140000000000000000000000000000000000
+                  0000006412640aa6020000ab0200000000000000007d117c127c11660253
+                  00
+               238           0 RESUME                   0
                
-               153           2 LOAD_FAST                0 (self)
+               248           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (amu2g)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (A2CM)
                             26 LOAD_CONST               1 (3)
                             28 BINARY_OP                8 (**)
                             32 BINARY_OP                5 (*)
-                            36 STORE_FAST               6 (unitconvert)
+                            36 STORE_FAST               8 (unitconvert)
                
-               154          38 LOAD_FAST                0 (self)
-                            40 LOAD_ATTR                2 (Lz)
-                            50 LOAD_FAST                2 (Nz)
-                            52 BINARY_OP               11 (/)
-                            56 STORE_FAST               7 (dZ)
+               249          38 LOAD_FAST                7 (direction)
+                            40 LOAD_CONST               2 ('z')
+                            42 COMPARE_OP               2 (==)
+                            48 POP_JUMP_FORWARD_IF_TRUE     6 (to 62)
+                            50 LOAD_FAST                7 (direction)
+                            52 LOAD_CONST               3 ('Z')
+                            54 COMPARE_OP               2 (==)
+                            60 POP_JUMP_FORWARD_IF_FALSE    51 (to 164)
+               
+               250     >>   62 LOAD_FAST                0 (self)
+                            64 LOAD_ATTR                2 (Lz)
+                            74 LOAD_FAST                2 (Nbin)
+                            76 BINARY_OP               11 (/)
+                            80 STORE_FAST               9 (dr)
+               
+               251          82 LOAD_FAST                1 (mxyz)
+                            84 LOAD_CONST               4 (None)
+                            86 LOAD_CONST               4 (None)
+                            88 BUILD_SLICE              2
+                            90 LOAD_CONST               1 (3)
+                            92 BUILD_TUPLE              2
+                            94 BINARY_SUBSCR
+                           104 STORE_FAST              10 (L)
+               
+               252         106 LOAD_FAST                0 (self)
+                           108 LOAD_ATTR                3 (zlo)
+                           118 STORE_FAST              11 (lo)
+               
+               253         120 LOAD_FAST                0 (self)
+                           122 LOAD_ATTR                4 (Lx)
+                           132 LOAD_FAST                0 (self)
+                           134 LOAD_ATTR                5 (Ly)
+                           144 BINARY_OP                5 (*)
+                           148 LOAD_FAST                9 (dr)
+                           150 BINARY_OP                5 (*)
+                           154 LOAD_FAST                8 (unitconvert)
+                           156 BINARY_OP                5 (*)
+                           160 STORE_FAST              12 (vlo)
+                           162 JUMP_FORWARD           125 (to 414)
                
-               155          58 LOAD_FAST                1 (mxyz)
-                            60 LOAD_CONST               0 (None)
-                            62 LOAD_CONST               0 (None)
-                            64 BUILD_SLICE              2
-                            66 LOAD_CONST               2 (0)
-                            68 BUILD_TUPLE              2
-                            70 BINARY_SUBSCR
-                            80 STORE_FAST               8 (MW)
-               
-               156          82 LOAD_GLOBAL              7 (NULL + np)
-                            94 LOAD_ATTR                4 (all)
-                           104 LOAD_FAST                8 (MW)
-                           106 LOAD_CONST               2 (0)
-                           108 COMPARE_OP               2 (==)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 POP_JUMP_FORWARD_IF_FALSE    18 (to 166)
-               
-               157         130 LOAD_CONST               3 ('number')
-                           132 STORE_FAST               5 (density_type)
-               
-               158         134 LOAD_GLOBAL             11 (NULL + print)
-                           146 LOAD_CONST               4 ('\nNo provided mass, will calculate number density!\n')
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 POP_TOP
-                           164 JUMP_FORWARD             2 (to 170)
-               
-               160     >>  166 LOAD_CONST               5 ('mass')
-                           168 STORE_FAST               5 (density_type)
-               
-               161     >>  170 LOAD_FAST                1 (mxyz)
-                           172 LOAD_CONST               0 (None)
-                           174 LOAD_CONST               0 (None)
-                           176 BUILD_SLICE              2
-                           178 LOAD_CONST               1 (3)
-                           180 BUILD_TUPLE              2
-                           182 BINARY_SUBSCR
-                           192 STORE_FAST               9 (Z)
+               254     >>  164 LOAD_FAST                7 (direction)
+                           166 LOAD_CONST               5 ('y')
+                           168 COMPARE_OP               2 (==)
+                           174 POP_JUMP_FORWARD_IF_TRUE     6 (to 188)
+                           176 LOAD_FAST                7 (direction)
+                           178 LOAD_CONST               6 ('Y')
+                           180 COMPARE_OP               2 (==)
+                           186 POP_JUMP_FORWARD_IF_FALSE    51 (to 290)
+               
+               255     >>  188 LOAD_FAST                0 (self)
+                           190 LOAD_ATTR                5 (Ly)
+                           200 LOAD_FAST                2 (Nbin)
+                           202 BINARY_OP               11 (/)
+                           206 STORE_FAST               9 (dr)
+               
+               256         208 LOAD_FAST                1 (mxyz)
+                           210 LOAD_CONST               4 (None)
+                           212 LOAD_CONST               4 (None)
+                           214 BUILD_SLICE              2
+                           216 LOAD_CONST               7 (2)
+                           218 BUILD_TUPLE              2
+                           220 BINARY_SUBSCR
+                           230 STORE_FAST              10 (L)
+               
+               257         232 LOAD_FAST                0 (self)
+                           234 LOAD_ATTR                6 (ylo)
+                           244 STORE_FAST              11 (lo)
+               
+               258         246 LOAD_FAST                0 (self)
+                           248 LOAD_ATTR                4 (Lx)
+                           258 LOAD_FAST                0 (self)
+                           260 LOAD_ATTR                2 (Lz)
+                           270 BINARY_OP                5 (*)
+                           274 LOAD_FAST                9 (dr)
+                           276 BINARY_OP                5 (*)
+                           280 LOAD_FAST                8 (unitconvert)
+                           282 BINARY_OP                5 (*)
+                           286 STORE_FAST              12 (vlo)
+                           288 JUMP_FORWARD            62 (to 414)
+               
+               259     >>  290 LOAD_FAST                7 (direction)
+                           292 LOAD_CONST               8 ('x')
+                           294 COMPARE_OP               2 (==)
+                           300 POP_JUMP_FORWARD_IF_TRUE     6 (to 314)
+                           302 LOAD_FAST                7 (direction)
+                           304 LOAD_CONST               9 ('X')
+                           306 COMPARE_OP               2 (==)
+                           312 POP_JUMP_FORWARD_IF_FALSE    50 (to 414)
+               
+               260     >>  314 LOAD_FAST                0 (self)
+                           316 LOAD_ATTR                4 (Lx)
+                           326 LOAD_FAST                2 (Nbin)
+                           328 BINARY_OP               11 (/)
+                           332 STORE_FAST               9 (dr)
+               
+               261         334 LOAD_FAST                1 (mxyz)
+                           336 LOAD_CONST               4 (None)
+                           338 LOAD_CONST               4 (None)
+                           340 BUILD_SLICE              2
+                           342 LOAD_CONST              10 (1)
+                           344 BUILD_TUPLE              2
+                           346 BINARY_SUBSCR
+                           356 STORE_FAST              10 (L)
+               
+               262         358 LOAD_FAST                0 (self)
+                           360 LOAD_ATTR                7 (xlo)
+                           370 STORE_FAST              11 (lo)
+               
+               263         372 LOAD_FAST                0 (self)
+                           374 LOAD_ATTR                5 (Ly)
+                           384 LOAD_FAST                0 (self)
+                           386 LOAD_ATTR                2 (Lz)
+                           396 BINARY_OP                5 (*)
+                           400 LOAD_FAST                9 (dr)
+                           402 BINARY_OP                5 (*)
+                           406 LOAD_FAST                8 (unitconvert)
+                           408 BINARY_OP                5 (*)
+                           412 STORE_FAST              12 (vlo)
+               
+               265     >>  414 LOAD_GLOBAL             17 (NULL + list)
+                           426 LOAD_FAST                4 (mass_dict)
+                           428 LOAD_METHOD              9 (keys)
+                           450 PRECALL                  0
+                           454 CALL                     0
+                           464 PRECALL                  1
+                           468 CALL                     1
+                           478 STORE_FAST              13 (mass_key)
+               
+               266         480 LOAD_GLOBAL             21 (NULL + range)
+                           492 LOAD_GLOBAL             23 (NULL + len)
+                           504 LOAD_FAST                0 (self)
+                           506 LOAD_ATTR               12 (atom)
+                           516 PRECALL                  1
+                           520 CALL                     1
+                           530 PRECALL                  1
+                           534 CALL                     1
+                           544 GET_ITER
+                       >>  546 FOR_ITER                75 (to 698)
+                           548 STORE_FAST              14 (i)
+               
+               267         550 LOAD_GLOBAL             21 (NULL + range)
+                           562 LOAD_GLOBAL             23 (NULL + len)
+                           574 LOAD_FAST               13 (mass_key)
+                           576 PRECALL                  1
+                           580 CALL                     1
+                           590 PRECALL                  1
+                           594 CALL                     1
+                           604 GET_ITER
+                       >>  606 FOR_ITER                44 (to 696)
+                           608 STORE_FAST              15 (j)
+               
+               268         610 LOAD_FAST                0 (self)
+                           612 LOAD_ATTR               12 (atom)
+                           622 LOAD_FAST               14 (i)
+                           624 BINARY_SUBSCR
+                           634 LOAD_FAST               13 (mass_key)
+                           636 LOAD_FAST               15 (j)
+                           638 BINARY_SUBSCR
+                           648 COMPARE_OP               2 (==)
+                           654 POP_JUMP_FORWARD_IF_FALSE    19 (to 694)
+               
+               269         656 LOAD_FAST                4 (mass_dict)
+                           658 LOAD_FAST               13 (mass_key)
+                           660 LOAD_FAST               15 (j)
+                           662 BINARY_SUBSCR
+                           672 BINARY_SUBSCR
+                           682 LOAD_FAST                1 (mxyz)
+                           684 LOAD_FAST               14 (i)
+                           686 LOAD_CONST              11 (0)
+                           688 BUILD_TUPLE              2
+                           690 STORE_SUBSCR
+                       >>  694 JUMP_BACKWARD           45 (to 606)
+               
+               267     >>  696 JUMP_BACKWARD           76 (to 546)
+               
+               270     >>  698 LOAD_FAST                1 (mxyz)
+                           700 LOAD_CONST               4 (None)
+                           702 LOAD_CONST               4 (None)
+                           704 BUILD_SLICE              2
+                           706 LOAD_CONST              11 (0)
+                           708 BUILD_TUPLE              2
+                           710 BINARY_SUBSCR
+                           720 STORE_FAST              16 (MW)
+               
+               271         722 LOAD_GLOBAL             27 (NULL + np)
+                           734 LOAD_ATTR               14 (all)
+                           744 LOAD_FAST               16 (MW)
+                           746 LOAD_CONST              11 (0)
+                           748 COMPARE_OP               2 (==)
+                           754 PRECALL                  1
+                           758 CALL                     1
+                           768 POP_JUMP_FORWARD_IF_FALSE    18 (to 806)
                
-               162         194 BUILD_LIST               0
-                           196 STORE_FAST              10 (rho_n)
+               272         770 LOAD_CONST              12 ('number')
+                           772 STORE_FAST               6 (density_type)
                
-               163         198 BUILD_LIST               0
-                           200 STORE_FAST              11 (zc_n)
+               273         774 LOAD_GLOBAL             31 (NULL + print)
+                           786 LOAD_CONST              13 ('\nNo provided mass, will calculate number density!\n')
+                           788 PRECALL                  1
+                           792 CALL                     1
+                           802 POP_TOP
+                           804 JUMP_FORWARD             2 (to 810)
+               
+               275     >>  806 LOAD_CONST              14 ('mass')
+                           808 STORE_FAST               6 (density_type)
+               
+               277     >>  810 BUILD_LIST               0
+                           812 STORE_FAST              17 (rho_n)
+               
+               278         814 BUILD_LIST               0
+                           816 STORE_FAST              18 (lc_n)
+               
+               280         818 LOAD_FAST                5 (id_type)
+                           820 LOAD_CONST              15 ('mol')
+                           822 COMPARE_OP               2 (==)
+                           828 POP_JUMP_FORWARD_IF_FALSE     8 (to 846)
+               
+               281         830 LOAD_FAST                0 (self)
+                           832 LOAD_ATTR               16 (mol)
+                           842 STORE_FAST              19 (id_know)
+                           844 JUMP_FORWARD            13 (to 872)
+               
+               282     >>  846 LOAD_FAST                5 (id_type)
+                           848 LOAD_CONST              16 ('atom')
+                           850 COMPARE_OP               2 (==)
+                           856 POP_JUMP_FORWARD_IF_FALSE     7 (to 872)
+               
+               283         858 LOAD_FAST                0 (self)
+                           860 LOAD_ATTR               12 (atom)
+                           870 STORE_FAST              19 (id_know)
+               
+               284     >>  872 LOAD_GLOBAL             21 (NULL + range)
+                           884 LOAD_FAST                2 (Nbin)
+                           886 PRECALL                  1
+                           890 CALL                     1
+                           900 GET_ITER
+                       >>  902 FOR_ITER               184 (to 1272)
+                           904 STORE_FAST              20 (n)
+               
+               285         906 LOAD_CONST              11 (0)
+                           908 STORE_FAST              21 (mass_n)
+               
+               286         910 LOAD_FAST               11 (lo)
+                           912 LOAD_FAST                9 (dr)
+                           914 LOAD_FAST               20 (n)
+                           916 BINARY_OP                5 (*)
+                           920 BINARY_OP                0 (+)
+                           924 STORE_FAST              22 (l0)
+               
+               287         926 LOAD_FAST               11 (lo)
+                           928 LOAD_FAST                9 (dr)
+                           930 LOAD_FAST               20 (n)
+                           932 LOAD_CONST              10 (1)
+                           934 BINARY_OP                0 (+)
+                           938 BINARY_OP                5 (*)
+                           942 BINARY_OP                0 (+)
+                           946 STORE_FAST              23 (l1)
+               
+               288         948 LOAD_FAST               22 (l0)
+                           950 LOAD_FAST               23 (l1)
+                           952 BINARY_OP                0 (+)
+                           956 LOAD_CONST              17 (0.5)
+                           958 BINARY_OP                5 (*)
+                           962 STORE_FAST              24 (lc)
+               
+               290         964 LOAD_GLOBAL             21 (NULL + range)
+                           976 LOAD_FAST                0 (self)
+                           978 LOAD_ATTR               17 (atom_n)
+                           988 PRECALL                  1
+                           992 CALL                     1
+                          1002 GET_ITER
+                       >> 1004 FOR_ITER                85 (to 1176)
+                          1006 STORE_FAST              14 (i)
+               
+               291        1008 LOAD_FAST               19 (id_know)
+                          1010 LOAD_FAST               14 (i)
+                          1012 BINARY_SUBSCR
+                          1022 LOAD_FAST                3 (id_range)
+                          1024 LOAD_CONST              11 (0)
+                          1026 BINARY_SUBSCR
+                          1036 COMPARE_OP               5 (>=)
+                          1042 POP_JUMP_FORWARD_IF_FALSE    65 (to 1174)
+                          1044 LOAD_FAST               19 (id_know)
+                          1046 LOAD_FAST               14 (i)
+                          1048 BINARY_SUBSCR
+                          1058 LOAD_FAST                3 (id_range)
+                          1060 LOAD_CONST              10 (1)
+                          1062 BINARY_SUBSCR
+                          1072 COMPARE_OP               1 (<=)
+                          1078 POP_JUMP_FORWARD_IF_FALSE    47 (to 1174)
                
-               165         202 LOAD_FAST                4 (id_type)
-                           204 LOAD_CONST               6 ('mol')
-                           206 COMPARE_OP               2 (==)
-                           212 POP_JUMP_FORWARD_IF_FALSE     8 (to 230)
-               
-               166         214 LOAD_FAST                0 (self)
-                           216 LOAD_ATTR                6 (mol)
-                           226 STORE_FAST              12 (id_know)
-                           228 JUMP_FORWARD            13 (to 256)
-               
-               167     >>  230 LOAD_FAST                4 (id_type)
-                           232 LOAD_CONST               7 ('atom')
-                           234 COMPARE_OP               2 (==)
-                           240 POP_JUMP_FORWARD_IF_FALSE     7 (to 256)
-               
-               168         242 LOAD_FAST                0 (self)
-                           244 LOAD_ATTR                7 (atom)
-                           254 STORE_FAST              12 (id_know)
-               
-               169     >>  256 LOAD_GLOBAL             17 (NULL + range)
-                           268 LOAD_FAST                2 (Nz)
-                           270 PRECALL                  1
-                           274 CALL                     1
-                           284 GET_ITER
-                       >>  286 FOR_ITER               215 (to 718)
-                           288 STORE_FAST              13 (n)
-               
-               170         290 LOAD_CONST               2 (0)
-                           292 STORE_FAST              14 (mass_n)
-               
-               171         294 LOAD_FAST                0 (self)
-                           296 LOAD_ATTR                9 (zlo)
-                           306 LOAD_FAST                7 (dZ)
-                           308 LOAD_FAST               13 (n)
-                           310 BINARY_OP                5 (*)
-                           314 BINARY_OP                0 (+)
-                           318 STORE_FAST              15 (z0)
-               
-               172         320 LOAD_FAST                0 (self)
-                           322 LOAD_ATTR                9 (zlo)
-                           332 LOAD_FAST                7 (dZ)
-                           334 LOAD_FAST               13 (n)
-                           336 LOAD_CONST               8 (1)
-                           338 BINARY_OP                0 (+)
-                           342 BINARY_OP                5 (*)
-                           346 BINARY_OP                0 (+)
-                           350 STORE_FAST              16 (z1)
-               
-               173         352 LOAD_FAST               15 (z0)
-                           354 LOAD_FAST               16 (z1)
-                           356 BINARY_OP                0 (+)
-                           360 LOAD_CONST               9 (0.5)
-                           362 BINARY_OP                5 (*)
-                           366 STORE_FAST              17 (zc)
-               
-               175         368 LOAD_GLOBAL             17 (NULL + range)
-                           380 LOAD_FAST                0 (self)
-                           382 LOAD_ATTR               10 (atom_n)
-                           392 PRECALL                  1
-                           396 CALL                     1
-                           406 GET_ITER
-                       >>  408 FOR_ITER                85 (to 580)
-                           410 STORE_FAST              18 (i)
-               
-               176         412 LOAD_FAST               12 (id_know)
-                           414 LOAD_FAST               18 (i)
-                           416 BINARY_SUBSCR
-                           426 LOAD_FAST                3 (mol_n)
-                           428 LOAD_CONST               2 (0)
-                           430 BINARY_SUBSCR
-                           440 COMPARE_OP               5 (>=)
-                           446 POP_JUMP_FORWARD_IF_FALSE    65 (to 578)
-                           448 LOAD_FAST               12 (id_know)
-                           450 LOAD_FAST               18 (i)
-                           452 BINARY_SUBSCR
-                           462 LOAD_FAST                3 (mol_n)
-                           464 LOAD_CONST               8 (1)
-                           466 BINARY_SUBSCR
-                           476 COMPARE_OP               1 (<=)
-                           482 POP_JUMP_FORWARD_IF_FALSE    47 (to 578)
-               
-               178         484 LOAD_FAST                9 (Z)
-                           486 LOAD_FAST               18 (i)
-                           488 BINARY_SUBSCR
-                           498 LOAD_FAST               15 (z0)
-                           500 COMPARE_OP               5 (>=)
-                           506 POP_JUMP_FORWARD_IF_FALSE    35 (to 578)
-                           508 LOAD_FAST                9 (Z)
-                           510 LOAD_FAST               18 (i)
-                           512 BINARY_SUBSCR
-                           522 LOAD_FAST               16 (z1)
-                           524 COMPARE_OP               1 (<=)
-                           530 POP_JUMP_FORWARD_IF_FALSE    23 (to 578)
-               
-               179         532 LOAD_FAST                5 (density_type)
-                           534 LOAD_CONST               5 ('mass')
-                           536 COMPARE_OP               2 (==)
-                           542 POP_JUMP_FORWARD_IF_FALSE    12 (to 568)
-               
-               180         544 LOAD_FAST                8 (MW)
-                           546 LOAD_FAST               18 (i)
-                           548 BINARY_SUBSCR
-                           558 LOAD_FAST               14 (mass_n)
-                           560 BINARY_OP                0 (+)
-                           564 STORE_FAST              14 (mass_n)
-                           566 JUMP_BACKWARD           80 (to 408)
-               
-               182     >>  568 LOAD_FAST               14 (mass_n)
-                           570 LOAD_CONST               8 (1)
-                           572 BINARY_OP                0 (+)
-                           576 STORE_FAST              14 (mass_n)
-                       >>  578 JUMP_BACKWARD           86 (to 408)
-               
-               184     >>  580 LOAD_FAST                0 (self)
-                           582 LOAD_ATTR               11 (Lx)
-                           592 LOAD_FAST                0 (self)
-                           594 LOAD_ATTR               12 (Ly)
-                           604 BINARY_OP                5 (*)
-                           608 LOAD_FAST                7 (dZ)
-                           610 BINARY_OP                5 (*)
-                           614 LOAD_FAST                6 (unitconvert)
-                           616 BINARY_OP                5 (*)
-                           620 STORE_FAST              19 (vlo)
-               
-               186         622 LOAD_FAST               14 (mass_n)
-                           624 LOAD_FAST               19 (vlo)
-                           626 BINARY_OP               11 (/)
-                           630 STORE_FAST              20 (rho)
-               
-               188         632 LOAD_FAST               10 (rho_n)
-                           634 LOAD_METHOD             13 (append)
-                           656 LOAD_FAST               20 (rho)
-                           658 PRECALL                  1
-                           662 CALL                     1
-                           672 POP_TOP
-               
-               189         674 LOAD_FAST               11 (zc_n)
-                           676 LOAD_METHOD             13 (append)
-                           698 LOAD_FAST               17 (zc)
-                           700 PRECALL                  1
-                           704 CALL                     1
-                           714 POP_TOP
-                           716 JUMP_BACKWARD          216 (to 286)
-               
-               190     >>  718 LOAD_GLOBAL              7 (NULL + np)
-                           730 LOAD_ATTR               14 (array)
-                           740 LOAD_FAST               11 (zc_n)
-                           742 PRECALL                  1
-                           746 CALL                     1
-                           756 LOAD_METHOD             15 (reshape)
-                           778 LOAD_CONST              10 (-1)
-                           780 LOAD_CONST               8 (1)
-                           782 PRECALL                  2
-                           786 CALL                     2
-                           796 STORE_FAST              11 (zc_n)
-               
-               191         798 LOAD_GLOBAL              7 (NULL + np)
-                           810 LOAD_ATTR               14 (array)
-                           820 LOAD_FAST               10 (rho_n)
-                           822 PRECALL                  1
-                           826 CALL                     1
-                           836 LOAD_METHOD             15 (reshape)
-                           858 LOAD_CONST              10 (-1)
-                           860 LOAD_CONST               8 (1)
-                           862 PRECALL                  2
-                           866 CALL                     2
-                           876 STORE_FAST              10 (rho_n)
-               
-               192         878 LOAD_FAST               11 (zc_n)
-                           880 LOAD_FAST               10 (rho_n)
-                           882 BUILD_TUPLE              2
-                           884 RETURN_VALUE
+               293        1080 LOAD_FAST               10 (L)
+                          1082 LOAD_FAST               14 (i)
+                          1084 BINARY_SUBSCR
+                          1094 LOAD_FAST               22 (l0)
+                          1096 COMPARE_OP               5 (>=)
+                          1102 POP_JUMP_FORWARD_IF_FALSE    35 (to 1174)
+                          1104 LOAD_FAST               10 (L)
+                          1106 LOAD_FAST               14 (i)
+                          1108 BINARY_SUBSCR
+                          1118 LOAD_FAST               23 (l1)
+                          1120 COMPARE_OP               1 (<=)
+                          1126 POP_JUMP_FORWARD_IF_FALSE    23 (to 1174)
+               
+               294        1128 LOAD_FAST                6 (density_type)
+                          1130 LOAD_CONST              14 ('mass')
+                          1132 COMPARE_OP               2 (==)
+                          1138 POP_JUMP_FORWARD_IF_FALSE    12 (to 1164)
+               
+               295        1140 LOAD_FAST               16 (MW)
+                          1142 LOAD_FAST               14 (i)
+                          1144 BINARY_SUBSCR
+                          1154 LOAD_FAST               21 (mass_n)
+                          1156 BINARY_OP                0 (+)
+                          1160 STORE_FAST              21 (mass_n)
+                          1162 JUMP_BACKWARD           80 (to 1004)
+               
+               297     >> 1164 LOAD_FAST               21 (mass_n)
+                          1166 LOAD_CONST              10 (1)
+                          1168 BINARY_OP                0 (+)
+                          1172 STORE_FAST              21 (mass_n)
+                       >> 1174 JUMP_BACKWARD           86 (to 1004)
+               
+               298     >> 1176 LOAD_FAST               21 (mass_n)
+                          1178 LOAD_FAST               12 (vlo)
+                          1180 BINARY_OP               11 (/)
+                          1184 STORE_FAST              25 (rho)
+               
+               300        1186 LOAD_FAST               17 (rho_n)
+                          1188 LOAD_METHOD             18 (append)
+                          1210 LOAD_FAST               25 (rho)
+                          1212 PRECALL                  1
+                          1216 CALL                     1
+                          1226 POP_TOP
+               
+               301        1228 LOAD_FAST               18 (lc_n)
+                          1230 LOAD_METHOD             18 (append)
+                          1252 LOAD_FAST               24 (lc)
+                          1254 PRECALL                  1
+                          1258 CALL                     1
+                          1268 POP_TOP
+                          1270 JUMP_BACKWARD          185 (to 902)
+               
+               302     >> 1272 LOAD_GLOBAL             27 (NULL + np)
+                          1284 LOAD_ATTR               19 (array)
+                          1294 LOAD_FAST               18 (lc_n)
+                          1296 PRECALL                  1
+                          1300 CALL                     1
+                          1310 LOAD_METHOD             20 (reshape)
+                          1332 LOAD_CONST              18 (-1)
+                          1334 LOAD_CONST              10 (1)
+                          1336 PRECALL                  2
+                          1340 CALL                     2
+                          1350 STORE_FAST              18 (lc_n)
+               
+               303        1352 LOAD_GLOBAL             27 (NULL + np)
+                          1364 LOAD_ATTR               19 (array)
+                          1374 LOAD_FAST               17 (rho_n)
+                          1376 PRECALL                  1
+                          1380 CALL                     1
+                          1390 LOAD_METHOD             20 (reshape)
+                          1412 LOAD_CONST              18 (-1)
+                          1414 LOAD_CONST              10 (1)
+                          1416 PRECALL                  2
+                          1420 CALL                     2
+                          1430 STORE_FAST              17 (rho_n)
+               
+               304        1432 LOAD_FAST               18 (lc_n)
+                          1434 LOAD_FAST               17 (rho_n)
+                          1436 BUILD_TUPLE              2
+                          1438 RETURN_VALUE
                consts
-                  None
+                  '\n\t\tcalculating density of some molecules......\n\t\tmxyz: array of mass, x, y, and z;\n\t\tNbin: number of bins in x/y/z-axis\n\t\tid_range: range of molecule/atom id;\n\t\tmass_dict: masses of atoms ,default={} \n\t\tid_type: according to the molecule/atom id, to recognize atoms, args: mol, atom\n\t\tdensity_type: calculated type of density \n\t\t'
                   3
+                  'z'
+                  'Z'
+                  None
+                  'y'
+                  'Y'
+                  2
+                  'x'
+                  'X'
+                  1
                   0
                   'number'
                   '\nNo provided mass, will calculate number density!\n'
                   'mass'
                   'mol'
                   'atom'
-                  1
                   0.5
                   -1
-               names      ('amu2g', 'A2CM', 'Lz', 'np', 'all', 'print', 'mol', 'atom', 'range', 'zlo', 'atom_n', 'Lx', 'Ly', 'append', 'array', 'reshape')
-               varnames   ('self', 'mxyz', 'Nz', 'mol_n', 'id_type', 'density_type', 'unitconvert', 'dZ', 'MW', 'Z', 'rho_n', 'zc_n', 'id_know', 'n', 'mass_n', 'z0', 'z1', 'zc', 'i', 'vlo', 'rho')
+               names      ('amu2g', 'A2CM', 'Lz', 'zlo', 'Lx', 'Ly', 'ylo', 'xlo', 'list', 'keys', 'range', 'len', 'atom', 'np', 'all', 'print', 'mol', 'atom_n', 'append', 'array', 'reshape')
+               varnames   ('self', 'mxyz', 'Nbin', 'id_range', 'mass_dict', 'id_type', 'density_type', 'direction', 'unitconvert', 'dr', 'L', 'lo', 'vlo', 'mass_key', 'i', 'j', 'MW', 'rho_n', 'lc_n', 'id_know', 'n', 'mass_n', 'l0', 'l1', 'lc', 'rho')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'oneframe_moldensity'
-               firstlineno 151
+               firstlineno 238
                lnotab
-                  0x020224011401180130010401200204011801040104020c0110010c010e
-                  01220104011a01200110022c01480230010c0118020c022a020a022a012c
-                  0150015001
+                  0x020a24011801140118010e012c011801140118010e012c011801140118
+                  010e012a02420146013c012e0128fe020318013001040120020402040104
+                  020c0110010c010e01220104011001160110022c01480230010c0118020c
+                  010a022a012c0150015001
             code
                argcount  : 7
                nlocals   : 39
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a01000000000000000064017a
@@ -1726,252 +2490,252 @@
                   0000000000a00e00000000000000000000000000000000000000007c037c
                   047c056603a6010000ab0100000000000000007d23741f00000000000000
                   0000007c0fa6010000ab0100000000000000007d24741f00000000000000
                   0000007c10a6010000ab0100000000000000007d25741f00000000000000
                   0000007c11a6010000ab0100000000000000007d267c0f7c247a0a00007d
                   0f7c107c257a0a00007d107c117c267a0a00007d117c0f7c107c117c2366
                   045300
-               194           0 RESUME                   0
+               306           0 RESUME                   0
                
-               203           2 LOAD_FAST                0 (self)
+               315           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (amu2g)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (A2CM)
                             26 LOAD_CONST               1 (3)
                             28 BINARY_OP                8 (**)
                             32 BINARY_OP                5 (*)
                             36 STORE_FAST               7 (unitconvert)
                
-               204          38 LOAD_FAST                0 (self)
+               316          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (Lz)
                             50 LOAD_FAST                3 (Nx)
                             52 BINARY_OP               11 (/)
                             56 STORE_FAST               8 (dX)
                
-               205          58 LOAD_FAST                0 (self)
+               317          58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (Lz)
                             70 LOAD_FAST                4 (Ny)
                             72 BINARY_OP               11 (/)
                             76 STORE_FAST               9 (dY)
                
-               206          78 LOAD_FAST                0 (self)
+               318          78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                2 (Lz)
                             90 LOAD_FAST                5 (Nz)
                             92 BINARY_OP               11 (/)
                             96 STORE_FAST              10 (dZ)
                
-               207          98 LOAD_FAST                1 (mxyz)
+               319          98 LOAD_FAST                1 (mxyz)
                            100 LOAD_CONST               2 (None)
                            102 LOAD_CONST               2 (None)
                            104 BUILD_SLICE              2
                            106 LOAD_CONST               3 (0)
                            108 BUILD_TUPLE              2
                            110 BINARY_SUBSCR
                            120 STORE_FAST              11 (MW)
                
-               208         122 LOAD_FAST                1 (mxyz)
+               320         122 LOAD_FAST                1 (mxyz)
                            124 LOAD_CONST               2 (None)
                            126 LOAD_CONST               2 (None)
                            128 BUILD_SLICE              2
                            130 LOAD_CONST               4 (1)
                            132 BUILD_TUPLE              2
                            134 BINARY_SUBSCR
                            144 STORE_FAST              12 (X)
                
-               209         146 LOAD_FAST                1 (mxyz)
+               321         146 LOAD_FAST                1 (mxyz)
                            148 LOAD_CONST               2 (None)
                            150 LOAD_CONST               2 (None)
                            152 BUILD_SLICE              2
                            154 LOAD_CONST               5 (2)
                            156 BUILD_TUPLE              2
                            158 BINARY_SUBSCR
                            168 STORE_FAST              13 (Y)
                
-               210         170 LOAD_FAST                1 (mxyz)
+               322         170 LOAD_FAST                1 (mxyz)
                            172 LOAD_CONST               2 (None)
                            174 LOAD_CONST               2 (None)
                            176 BUILD_SLICE              2
                            178 LOAD_CONST               1 (3)
                            180 BUILD_TUPLE              2
                            182 BINARY_SUBSCR
                            192 STORE_FAST              14 (Z)
                
-               211         194 BUILD_LIST               0
+               323         194 BUILD_LIST               0
                            196 BUILD_LIST               0
                            198 BUILD_LIST               0
                            200 STORE_FAST              17 (zc_n)
                            202 STORE_FAST              16 (yc_n)
                            204 STORE_FAST              15 (xc_n)
                
-               212         206 BUILD_LIST               0
+               324         206 BUILD_LIST               0
                            208 STORE_FAST              18 (rho_n)
                
-               213         210 LOAD_GLOBAL              7 (NULL + range)
+               325         210 LOAD_GLOBAL              7 (NULL + range)
                            222 LOAD_FAST                3 (Nx)
                            224 PRECALL                  1
                            228 CALL                     1
                            238 GET_ITER
                        >>  240 EXTENDED_ARG             1
                            242 FOR_ITER               443 (to 1130)
                            244 STORE_FAST              19 (xi)
                
-               214         246 LOAD_FAST                0 (self)
+               326         246 LOAD_FAST                0 (self)
                            248 LOAD_ATTR                4 (xlo)
                            258 LOAD_FAST                8 (dX)
                            260 LOAD_FAST               19 (xi)
                            262 BINARY_OP                5 (*)
                            266 BINARY_OP                0 (+)
                            270 STORE_FAST              20 (x0)
                
-               215         272 LOAD_FAST                0 (self)
+               327         272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                4 (xlo)
                            284 LOAD_FAST                8 (dX)
                            286 LOAD_FAST               19 (xi)
                            288 LOAD_CONST               4 (1)
                            290 BINARY_OP                0 (+)
                            294 BINARY_OP                5 (*)
                            298 BINARY_OP                0 (+)
                            302 STORE_FAST              21 (x1)
                
-               216         304 LOAD_FAST               20 (x0)
+               328         304 LOAD_FAST               20 (x0)
                            306 LOAD_FAST               21 (x1)
                            308 BINARY_OP                0 (+)
                            312 LOAD_CONST               6 (0.5)
                            314 BINARY_OP                5 (*)
                            318 STORE_FAST              22 (xc)
                
-               217         320 LOAD_FAST               15 (xc_n)
+               329         320 LOAD_FAST               15 (xc_n)
                            322 LOAD_METHOD              5 (append)
                            344 LOAD_FAST               22 (xc)
                            346 PRECALL                  1
                            350 CALL                     1
                            360 POP_TOP
                
-               218         362 LOAD_GLOBAL             13 (NULL + print)
+               330         362 LOAD_GLOBAL             13 (NULL + print)
                            374 LOAD_FAST               19 (xi)
                            376 LOAD_CONST               7 ('---Nx:---')
                            378 LOAD_FAST                3 (Nx)
                            380 PRECALL                  3
                            384 CALL                     3
                            394 POP_TOP
                
-               219         396 LOAD_GLOBAL              7 (NULL + range)
+               331         396 LOAD_GLOBAL              7 (NULL + range)
                            408 LOAD_FAST                4 (Ny)
                            410 PRECALL                  1
                            414 CALL                     1
                            424 GET_ITER
                        >>  426 EXTENDED_ARG             1
                            428 FOR_ITER               348 (to 1126)
                            430 STORE_FAST              23 (yi)
                
-               221         432 LOAD_FAST                0 (self)
+               333         432 LOAD_FAST                0 (self)
                            434 LOAD_ATTR                7 (ylo)
                            444 LOAD_FAST                9 (dY)
                            446 LOAD_FAST               23 (yi)
                            448 BINARY_OP                5 (*)
                            452 BINARY_OP                0 (+)
                            456 STORE_FAST              24 (y0)
                
-               222         458 LOAD_FAST                0 (self)
+               334         458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                7 (ylo)
                            470 LOAD_FAST                9 (dY)
                            472 LOAD_FAST               23 (yi)
                            474 LOAD_CONST               4 (1)
                            476 BINARY_OP                0 (+)
                            480 BINARY_OP                5 (*)
                            484 BINARY_OP                0 (+)
                            488 STORE_FAST              25 (y1)
                
-               223         490 LOAD_FAST               24 (y0)
+               335         490 LOAD_FAST               24 (y0)
                            492 LOAD_FAST               25 (y1)
                            494 BINARY_OP                0 (+)
                            498 LOAD_CONST               6 (0.5)
                            500 BINARY_OP                5 (*)
                            504 STORE_FAST              26 (yc)
                
-               224         506 LOAD_FAST               16 (yc_n)
+               336         506 LOAD_FAST               16 (yc_n)
                            508 LOAD_METHOD              5 (append)
                            530 LOAD_FAST               26 (yc)
                            532 PRECALL                  1
                            536 CALL                     1
                            546 POP_TOP
                
-               225         548 LOAD_GLOBAL              7 (NULL + range)
+               337         548 LOAD_GLOBAL              7 (NULL + range)
                            560 LOAD_FAST                5 (Nz)
                            562 PRECALL                  1
                            566 CALL                     1
                            576 GET_ITER
                        >>  578 EXTENDED_ARG             1
                            580 FOR_ITER               270 (to 1122)
                            582 STORE_FAST              27 (zi)
                
-               227         584 LOAD_FAST                0 (self)
+               339         584 LOAD_FAST                0 (self)
                            586 LOAD_ATTR                8 (zlo)
                            596 LOAD_FAST               10 (dZ)
                            598 LOAD_FAST               27 (zi)
                            600 BINARY_OP                5 (*)
                            604 BINARY_OP                0 (+)
                            608 STORE_FAST              28 (z0)
                
-               228         610 LOAD_FAST                0 (self)
+               340         610 LOAD_FAST                0 (self)
                            612 LOAD_ATTR                8 (zlo)
                            622 LOAD_FAST               10 (dZ)
                            624 LOAD_FAST               27 (zi)
                            626 LOAD_CONST               4 (1)
                            628 BINARY_OP                0 (+)
                            632 BINARY_OP                5 (*)
                            636 BINARY_OP                0 (+)
                            640 STORE_FAST              29 (z1)
                
-               229         642 LOAD_FAST               28 (z0)
+               341         642 LOAD_FAST               28 (z0)
                            644 LOAD_FAST               29 (z1)
                            646 BINARY_OP                0 (+)
                            650 LOAD_CONST               6 (0.5)
                            652 BINARY_OP                5 (*)
                            656 STORE_FAST              30 (zc)
                
-               230         658 LOAD_FAST               17 (zc_n)
+               342         658 LOAD_FAST               17 (zc_n)
                            660 LOAD_METHOD              5 (append)
                            682 LOAD_FAST               30 (zc)
                            684 PRECALL                  1
                            688 CALL                     1
                            698 POP_TOP
                
-               232         700 LOAD_CONST               3 (0)
+               344         700 LOAD_CONST               3 (0)
                            702 STORE_FAST              31 (n)
                
-               234         704 LOAD_GLOBAL              7 (NULL + range)
+               346         704 LOAD_GLOBAL              7 (NULL + range)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                9 (atom_n)
                            728 PRECALL                  1
                            732 CALL                     1
                            742 GET_ITER
                        >>  744 FOR_ITER               149 (to 1044)
                            746 STORE_FAST              32 (i)
                
-               236         748 LOAD_FAST                0 (self)
+               348         748 LOAD_FAST                0 (self)
                            750 LOAD_ATTR               10 (mol)
                            760 LOAD_FAST               32 (i)
                            762 BINARY_SUBSCR
-                           772 LOAD_FAST                2 (mol_n)
+                           772 LOAD_FAST                2 (id_range)
                            774 LOAD_CONST               3 (0)
                            776 BINARY_SUBSCR
                            786 COMPARE_OP               5 (>=)
                            792 POP_JUMP_FORWARD_IF_FALSE   124 (to 1042)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               10 (mol)
                            806 LOAD_FAST               32 (i)
                            808 BINARY_SUBSCR
-                           818 LOAD_FAST                2 (mol_n)
+                           818 LOAD_FAST                2 (id_range)
                            820 LOAD_CONST               4 (1)
                            822 BINARY_SUBSCR
                            832 COMPARE_OP               1 (<=)
                            838 POP_JUMP_FORWARD_IF_FALSE   101 (to 1042)
                
-               237         840 LOAD_FAST               12 (X)
+               349         840 LOAD_FAST               12 (X)
                            842 LOAD_FAST               32 (i)
                            844 BINARY_SUBSCR
                            854 LOAD_FAST               20 (x0)
                            856 COMPARE_OP               5 (>=)
                            862 POP_JUMP_FORWARD_IF_FALSE    89 (to 1042)
                            864 LOAD_FAST               12 (X)
                            866 LOAD_FAST               32 (i)
@@ -2000,198 +2764,198 @@
                            960 LOAD_FAST               14 (Z)
                            962 LOAD_FAST               32 (i)
                            964 BINARY_SUBSCR
                            974 LOAD_FAST               29 (z1)
                            976 COMPARE_OP               1 (<=)
                            982 POP_JUMP_FORWARD_IF_FALSE    29 (to 1042)
                
-               238         984 LOAD_FAST                6 (mass_or_number)
+               350         984 LOAD_FAST                6 (mass_or_number)
                            986 LOAD_CONST               8 ('mass')
                            988 COMPARE_OP               2 (==)
                            994 POP_JUMP_FORWARD_IF_FALSE    12 (to 1020)
                
-               239         996 LOAD_FAST               11 (MW)
+               351         996 LOAD_FAST               11 (MW)
                            998 LOAD_FAST               32 (i)
                           1000 BINARY_SUBSCR
                           1010 LOAD_FAST               31 (n)
                           1012 BINARY_OP                0 (+)
                           1016 STORE_FAST              31 (n)
                           1018 JUMP_BACKWARD          138 (to 744)
                
-               240     >> 1020 LOAD_FAST                6 (mass_or_number)
+               352     >> 1020 LOAD_FAST                6 (mass_or_number)
                           1022 LOAD_CONST               9 ('number')
                           1024 COMPARE_OP               2 (==)
                           1030 POP_JUMP_FORWARD_IF_FALSE     5 (to 1042)
                
-               241        1032 LOAD_FAST               31 (n)
+               353        1032 LOAD_FAST               31 (n)
                           1034 LOAD_CONST               4 (1)
                           1036 BINARY_OP                0 (+)
                           1040 STORE_FAST              31 (n)
                        >> 1042 JUMP_BACKWARD          150 (to 744)
                
-               243     >> 1044 LOAD_FAST                8 (dX)
+               355     >> 1044 LOAD_FAST                8 (dX)
                           1046 LOAD_FAST                9 (dY)
                           1048 BINARY_OP                5 (*)
                           1052 LOAD_FAST               10 (dZ)
                           1054 BINARY_OP                5 (*)
                           1058 LOAD_FAST                7 (unitconvert)
                           1060 BINARY_OP                5 (*)
                           1064 STORE_FAST              33 (vlo)
                
-               244        1066 LOAD_FAST               31 (n)
+               356        1066 LOAD_FAST               31 (n)
                           1068 LOAD_FAST               33 (vlo)
                           1070 BINARY_OP               11 (/)
                           1074 STORE_FAST              34 (rho)
                
-               245        1076 LOAD_FAST               18 (rho_n)
+               357        1076 LOAD_FAST               18 (rho_n)
                           1078 LOAD_METHOD              5 (append)
                           1100 LOAD_FAST               34 (rho)
                           1102 PRECALL                  1
                           1106 CALL                     1
                           1116 POP_TOP
                           1118 EXTENDED_ARG             1
                           1120 JUMP_BACKWARD          272 (to 578)
                
-               225     >> 1122 EXTENDED_ARG             1
+               337     >> 1122 EXTENDED_ARG             1
                           1124 JUMP_BACKWARD          350 (to 426)
                
-               219     >> 1126 EXTENDED_ARG             1
+               331     >> 1126 EXTENDED_ARG             1
                           1128 JUMP_BACKWARD          445 (to 240)
                
-               247     >> 1130 LOAD_GLOBAL             23 (NULL + np)
+               359     >> 1130 LOAD_GLOBAL             23 (NULL + np)
                           1142 LOAD_ATTR               12 (array)
                           1152 LOAD_FAST               15 (xc_n)
                           1154 PRECALL                  1
                           1158 CALL                     1
                           1168 STORE_FAST              15 (xc_n)
                
-               248        1170 LOAD_GLOBAL             23 (NULL + np)
+               360        1170 LOAD_GLOBAL             23 (NULL + np)
                           1182 LOAD_ATTR               13 (unique)
                           1192 LOAD_FAST               15 (xc_n)
                           1194 PRECALL                  1
                           1198 CALL                     1
                           1208 LOAD_METHOD             14 (reshape)
                           1230 LOAD_FAST                3 (Nx)
                           1232 LOAD_CONST               4 (1)
                           1234 BUILD_TUPLE              2
                           1236 PRECALL                  1
                           1240 CALL                     1
                           1250 STORE_FAST              15 (xc_n)
                
-               250        1252 LOAD_GLOBAL             23 (NULL + np)
+               362        1252 LOAD_GLOBAL             23 (NULL + np)
                           1264 LOAD_ATTR               12 (array)
                           1274 LOAD_FAST               16 (yc_n)
                           1276 PRECALL                  1
                           1280 CALL                     1
                           1290 STORE_FAST              16 (yc_n)
                
-               251        1292 LOAD_GLOBAL             23 (NULL + np)
+               363        1292 LOAD_GLOBAL             23 (NULL + np)
                           1304 LOAD_ATTR               13 (unique)
                           1314 LOAD_FAST               16 (yc_n)
                           1316 PRECALL                  1
                           1320 CALL                     1
                           1330 LOAD_METHOD             14 (reshape)
                           1352 LOAD_FAST                4 (Ny)
                           1354 LOAD_CONST               4 (1)
                           1356 BUILD_TUPLE              2
                           1358 PRECALL                  1
                           1362 CALL                     1
                           1372 STORE_FAST              16 (yc_n)
                
-               253        1374 LOAD_GLOBAL             23 (NULL + np)
+               365        1374 LOAD_GLOBAL             23 (NULL + np)
                           1386 LOAD_ATTR               12 (array)
                           1396 LOAD_FAST               17 (zc_n)
                           1398 PRECALL                  1
                           1402 CALL                     1
                           1412 STORE_FAST              17 (zc_n)
                
-               254        1414 LOAD_GLOBAL             23 (NULL + np)
+               366        1414 LOAD_GLOBAL             23 (NULL + np)
                           1426 LOAD_ATTR               13 (unique)
                           1436 LOAD_FAST               17 (zc_n)
                           1438 PRECALL                  1
                           1442 CALL                     1
                           1452 LOAD_METHOD             14 (reshape)
                           1474 LOAD_FAST                5 (Nz)
                           1476 LOAD_CONST               4 (1)
                           1478 BUILD_TUPLE              2
                           1480 PRECALL                  1
                           1484 CALL                     1
                           1494 STORE_FAST              17 (zc_n)
                
-               255        1496 LOAD_GLOBAL             23 (NULL + np)
+               367        1496 LOAD_GLOBAL             23 (NULL + np)
                           1508 LOAD_ATTR               12 (array)
                           1518 LOAD_FAST               18 (rho_n)
                           1520 PRECALL                  1
                           1524 CALL                     1
                           1534 LOAD_METHOD             14 (reshape)
                           1556 LOAD_FAST                3 (Nx)
                           1558 LOAD_FAST                4 (Ny)
                           1560 LOAD_FAST                5 (Nz)
                           1562 BUILD_TUPLE              3
                           1564 PRECALL                  1
                           1568 CALL                     1
                           1578 STORE_FAST              35 (rho_nxyz)
                
-               257        1580 LOAD_GLOBAL             31 (NULL + min)
+               369        1580 LOAD_GLOBAL             31 (NULL + min)
                           1592 LOAD_FAST               15 (xc_n)
                           1594 PRECALL                  1
                           1598 CALL                     1
                           1608 STORE_FAST              36 (minx)
                
-               258        1610 LOAD_GLOBAL             31 (NULL + min)
+               370        1610 LOAD_GLOBAL             31 (NULL + min)
                           1622 LOAD_FAST               16 (yc_n)
                           1624 PRECALL                  1
                           1628 CALL                     1
                           1638 STORE_FAST              37 (miny)
                
-               259        1640 LOAD_GLOBAL             31 (NULL + min)
+               371        1640 LOAD_GLOBAL             31 (NULL + min)
                           1652 LOAD_FAST               17 (zc_n)
                           1654 PRECALL                  1
                           1658 CALL                     1
                           1668 STORE_FAST              38 (minz)
                
-               260        1670 LOAD_FAST               15 (xc_n)
+               372        1670 LOAD_FAST               15 (xc_n)
                           1672 LOAD_FAST               36 (minx)
                           1674 BINARY_OP               10 (-)
                           1678 STORE_FAST              15 (xc_n)
                
-               261        1680 LOAD_FAST               16 (yc_n)
+               373        1680 LOAD_FAST               16 (yc_n)
                           1682 LOAD_FAST               37 (miny)
                           1684 BINARY_OP               10 (-)
                           1688 STORE_FAST              16 (yc_n)
                
-               262        1690 LOAD_FAST               17 (zc_n)
+               374        1690 LOAD_FAST               17 (zc_n)
                           1692 LOAD_FAST               38 (minz)
                           1694 BINARY_OP               10 (-)
                           1698 STORE_FAST              17 (zc_n)
                
-               266        1700 LOAD_FAST               15 (xc_n)
+               378        1700 LOAD_FAST               15 (xc_n)
                           1702 LOAD_FAST               16 (yc_n)
                           1704 LOAD_FAST               17 (zc_n)
                           1706 LOAD_FAST               35 (rho_nxyz)
                           1708 BUILD_TUPLE              4
                           1710 RETURN_VALUE
                consts
-                  '\n\t\tmxyz: mass x y z\n\t\tatom_n: tot number of atoms\n\t\tmol_n: type of molecules,list,mol_n=[1,36], the 1 is the first mol type and 36 is the last one mol type\n\t\tNx,Ny,Nz: layer number of x , y, z for calculating density, which is relate to the precision of density,\n\t\tand default is 1, that is, the total density.\n\t\tmass_or_number: "mass: mass density; number: number density"\n\t\t'
+                  '\n\t\tmxyz: mass x y z\n\t\tatom_n: tot number of atoms\n\t\tid_range: type of molecules,list,id_range=[1,36], the 1 is the first mol type and 36 is the last one mol type\n\t\tNx,Ny,Nz: layer number of x , y, z for calculating density, which is relate to the precision of density,\n\t\tand default is 1, that is, the total density.\n\t\tmass_or_number: "mass: mass density; number: number density"\n\t\t'
                   3
                   None
                   0
                   1
                   2
                   0.5
                   '---Nx:---'
                   'mass'
                   'number'
                names      ('amu2g', 'A2CM', 'Lz', 'range', 'xlo', 'append', 'print', 'ylo', 'zlo', 'atom_n', 'mol', 'np', 'array', 'unique', 'reshape', 'min')
-               varnames   ('self', 'mxyz', 'mol_n', 'Nx', 'Ny', 'Nz', 'mass_or_number', 'unitconvert', 'dX', 'dY', 'dZ', 'MW', 'X', 'Y', 'Z', 'xc_n', 'yc_n', 'zc_n', 'rho_n', 'xi', 'x0', 'x1', 'xc', 'yi', 'y0', 'y1', 'yc', 'zi', 'z0', 'z1', 'zc', 'n', 'i', 'vlo', 'rho', 'rho_nxyz', 'minx', 'miny', 'minz')
+               varnames   ('self', 'mxyz', 'id_range', 'Nx', 'Ny', 'Nz', 'mass_or_number', 'unitconvert', 'dX', 'dY', 'dZ', 'MW', 'X', 'Y', 'Z', 'xc_n', 'yc_n', 'zc_n', 'rho_n', 'xi', 'x0', 'x1', 'xc', 'yi', 'y0', 'y1', 'yc', 'zi', 'z0', 'z1', 'zc', 'n', 'i', 'vlo', 'rho', 'rho_nxyz', 'minx', 'miny', 'minz')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'TwoD_Density'
-               firstlineno 194
+               firstlineno 306
                lnotab
                   0x0209240114011401140118011801180118010c01040124011a01200110
                   012a01220124021a01200110012a0124021a01200110012a0204022c025c
                   0190010c0118010c010c0216010a012eec04fa041c280152022801520228
                   01520154021e011e011e010a010a010a04
             code
                argcount  : 4
@@ -2199,73 +2963,71 @@
                stacksize : 5
                flags     : 3
                code
                   0x97007c017c027a0a00007d047401000000000000000000007c04a60100
                   00ab01000000000000000064017c037a0500006b0400000000721b7c047c
                   037403000000000000000000006a0200000000000000007c04a6010000ab
                   0100000000000000007a0500007a0a00007d046e027c047d047c045300
-               268           0 RESUME                   0
+               380           0 RESUME                   0
                
-               269           2 LOAD_FAST                1 (dn)
+               381           2 LOAD_FAST                1 (dn)
                              4 LOAD_FAST                2 (dm)
                              6 BINARY_OP               10 (-)
                             10 STORE_FAST               4 (dr)
                
-               270          12 LOAD_GLOBAL              1 (NULL + abs)
+               382          12 LOAD_GLOBAL              1 (NULL + abs)
                             24 LOAD_FAST                4 (dr)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (0.5)
                             42 LOAD_FAST                3 (Lr)
                             44 BINARY_OP                5 (*)
                             48 COMPARE_OP               4 (>)
                             54 POP_JUMP_FORWARD_IF_FALSE    27 (to 110)
                
-               271          56 LOAD_FAST                4 (dr)
+               383          56 LOAD_FAST                4 (dr)
                             58 LOAD_FAST                3 (Lr)
                             60 LOAD_GLOBAL              3 (NULL + np)
                             72 LOAD_ATTR                2 (sign)
                             82 LOAD_FAST                4 (dr)
                             84 PRECALL                  1
                             88 CALL                     1
                             98 BINARY_OP                5 (*)
                            102 BINARY_OP               10 (-)
                            106 STORE_FAST               4 (dr)
                            108 JUMP_FORWARD             2 (to 114)
                
-               273     >>  110 LOAD_FAST                4 (dr)
+               385     >>  110 LOAD_FAST                4 (dr)
                            112 STORE_FAST               4 (dr)
                
-               274     >>  114 LOAD_FAST                4 (dr)
+               386     >>  114 LOAD_FAST                4 (dr)
                            116 RETURN_VALUE
                consts
                   None
                   0.5
                names      ('abs', 'np', 'sign')
                varnames   ('self', 'dn', 'dm', 'Lr', 'dr')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
                name       'unwrap'
-               firstlineno 268
+               firstlineno 380
                lnotab 0x02010a012c0136020401
             (1,)
-            ('mass',)
-            ('mol', 'mass')
             (1, 1, 1, 'mass')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'read_info', 'read_header', 'read_vol', 'read_mxyz', 'read_traj', 'oneframe_alldensity', 'oneframe_moldensity', 'TwoD_Density', 'unwrap', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
          name       'ReadLammpsTraj'
-         firstlineno 6
-         lnotab 0x0c0104010c060624060b060f061a06090828082b084a
+         firstlineno 66
+         lnotab 0x0c0104010c060624060b060f061d060c0e3d1044084a
       'ReadLammpsTraj'
-   names      ('numpy', 'np', 'pandas', 'pd', 'object', 'ReadLammpsTraj')
+   names      ('numpy', 'np', 'pandas', 'pd', 'version', 'print_ReadLammpsTraj', 'read_mass', 'object', 'ReadLammpsTraj')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\ReadLammpsTraj\\demo\\ReadLammpsTraj.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020308010802
+   lnotab 0x00ff0203080108020402061614020622
```

### Comparing `ReadLammpsTraj-1.1.4/demo/cal_density.py` & `ReadLammpsTraj-1.1.6/demo/cal_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 	# ax.legend(loc="center")
 	ax.legend(loc="best")
 
 	ax.set_ylabel('Density(g/mL)',fontweight='bold',size=32)
 	ax.set_xlabel('z(Å)',fontweight='bold',size=32)	
 	# ax.set_ylim(-0.05,1.5)
 
-	plt.savefig(path+"imgs/density.png",dpi=300)
+	# plt.savefig(path+"imgs/density.png",dpi=300)
 	plt.show()
 
 
 if __name__ == '__main__':
 	cal_density()
```

### Comparing `ReadLammpsTraj-1.1.4/demo/imgs/density.png` & `ReadLammpsTraj-1.1.6/demo/imgs/density.png`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.4/setup.py` & `ReadLammpsTraj-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'ReadLammpsTraj',
-version      = '1.1.4',
+version      = '1.1.6',
 py_modules   = ['ReadLammpsTraj'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/ReadLammpsTraj',
```

### Comparing `ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/PKG-INFO` & `ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.4
+Version: 1.1.6
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.py` & `ReadLammpsTraj-1.1.6/src/ReadLammpsTraj.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,37 @@
 # calculating the density,msd and rdf from lammps traj
 # id mol type mass x y z vx vy vz fx fy fz q
 import numpy as np 
 import pandas as pd
 
+version = "1.1.5"
+
+def print_ReadLammpsTraj():
+    cloud = [
+			"______                   _    _       _____                 _ ",
+			"| ___ \                 | |  | |     |_   _|               (_)",
+			"| |_/ /  ___   __ _   __| |  | |       | |   _ __   __ _    _ ",
+			"|    /  / _ \ / _` | / _` |  | |       | |  | '__| / _` |  | |",
+			"| |\ \ |  __/| (_| || (_| |  | |____   | |  | |   | (_| |  | |",
+			"\_| \_| \___| \__,_| \__,_|  \_____/   \_/  |_|    \__,_|  | |",
+			"                                                          _/ |",
+			"                                                         |__/ ",
+    ]
+    n = 32
+    print("\n")
+    print(n*"- ")
+    print(n*". ")
+    for line in cloud:
+        print(line)
+    print('@ReadLammpsTraj-'+version,", Good Luck!")
+    print(n*". ")
+    print(n*"- ")
+    return None
+
+print_ReadLammpsTraj()
 
 def read_mass(lammpsdata):
 	"""
 	read atomic mass from lammps data. 
 	"""
 	data = open(lammpsdata,"r")
 	lines = data.read()
@@ -133,14 +158,33 @@
 			mass = np.zeros(len(xyz))
 		mxyz = np.hstack((mass.reshape(-1,1),xyz))
 
 		position = mxyz
 
 		return position
 
+
+
+	def read_mxyz_add_mass(self,nframe,atomtype_list,mass_list):
+		# 不区分分子类型，计算所有的密度所需
+		traj = self.read_traj(nframe)
+		# print(traj)
+		self.mol = traj.loc[:,"mol"].values.astype(np.int64)#id mol type
+		self.atom = traj.loc[:,"type"].values.astype(np.int64)#id atom type
+		xyz = traj.loc[:,"x":"z"].values.astype(np.float64) # x y z
+		# print(xyz.shape)
+		mass_array = np.zeros(len(xyz)).reshape(-1,1)
+		for i in range(len(xyz)):
+			for j in range(len(mass_list)):
+				if self.atom[i] == atomtype_list[j]:
+					mass_array[i] = mass_list[j]
+		mxyz = np.hstack((mass_array,xyz))
+		return mxyz
+
+
 	def read_traj(self,nframe):
 		"""
 		read data of nth frame from traj...
 		nframe: number of frame 
 		"""
 		skip = 9*nframe+self.atom_n*(nframe-1)
 		traj = np.loadtxt(self.f,skiprows=skip,max_rows=self.atom_n,dtype="str")
@@ -274,57 +318,58 @@
 			# print(rho)
 			rho_n.append(rho)
 			lc_n.append(lc)
 		lc_n = np.array(lc_n).reshape(-1,1)
 		rho_n = np.array(rho_n).reshape(-1,1)	
 		return lc_n,rho_n
 
-	def TwoD_Density(self,mxyz,id_range,Nx=1,Ny=1,Nz=1,mass_or_number="mass"):
+	def TwoD_Density(self,mxyz,atomtype_n,Nx=1,Ny=1,Nz=1,mass_or_number="mass"):
 		'''
 		mxyz: mass x y z
 		atom_n: tot number of atoms
-		id_range: type of molecules,list,id_range=[1,36], the 1 is the first mol type and 36 is the last one mol type
+		atomtype_n: type of molecules,list,atom_n=[1,36], the 1 is the first atom type and 36 is the last one atom type
 		Nx,Ny,Nz: layer number of x , y, z for calculating density, which is relate to the precision of density,
 		and default is 1, that is, the total density.
 		mass_or_number: "mass: mass density; number: number density"
 		'''
 		unitconvert = self.amu2g*(self.A2CM)**3
-		dX = self.Lz/Nx #x方向bin
-		dY = self.Lz/Ny #y方向bin
+		dX = self.Lx/Nx #x方向bin
+		dY = self.Ly/Ny #y方向bin
 		dZ = self.Lz/Nz #z方向bin
 		MW = mxyz[:,0] #相对分子质量
 		X = mxyz[:,1] #x
 		Y = mxyz[:,2] #y
 		Z = mxyz[:,3] #z
 		xc_n,yc_n,zc_n = [],[],[]
 		rho_n = [] #average density list in every bins
 		for xi in range(Nx):
 			x0 = self.xlo+dX*xi #down coord of bin
 			x1 = self.xlo+dX*(xi+1) #down coord of bin
 			xc = (x0+x1)*0.5
 			xc_n.append(xc)
 			print(xi,'---Nx:---',Nx)
 			for yi in range(Ny):
-				# print(yi,'---Ny:---',Ny)
+				print(yi,'---Ny:---',Ny)
 				y0 = self.ylo+dY*yi #down coord of bin
 				y1 = self.ylo+dY*(yi+1) #down coord of bin
 				yc = (y0+y1)*0.5
+				# print(yc)
 				yc_n.append(yc)
 				for zi in range(Nz):
 					# print(zi,'---Nz:---',Nz)
 					z0 = self.zlo+dZ*zi #down coord of bin
 					z1 = self.zlo+dZ*(zi+1) #down coord of bin
 					zc = (z0+z1)*0.5
 					zc_n.append(zc)
 		
 					n=0 #tot mass or number in bin
 
 					for i in range(self.atom_n):
 						
-						if self.mol[i]>=id_range[0] and self.mol[i]<=id_range[1]:
+						if self.atom[i]>=atomtype_n[0] and self.atom[i]<=atomtype_n[1]:
 							if X[i]>=x0 and X[i]<=x1 and Y[i]>=y0 and Y[i]<=y1 and Z[i]>=z0 and Z[i]<=z1:
 								if mass_or_number == "mass":
 									n = MW[i]+n
 								elif mass_or_number == "number":
 									n = n+1
 									# print(i,'---',self.atom_n,MW[i])
 					vlo = (dX*dY*dZ)*unitconvert
```

