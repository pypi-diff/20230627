# Comparing `tmp/abejacli-2.2.0rc1-py3-none-any.whl.zip` & `tmp/abejacli-2.2.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 80412 bytes, number of entries: 50
+Zip file size: 84302 bytes, number of entries: 52
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/__init__.py
 -rw-r--r--  2.0 unx     3756 b- defN 80-Jan-01 00:00 abejacli/bucket/__init__.py
 -rw-r--r--  2.0 unx     4355 b- defN 80-Jan-01 00:00 abejacli/bucket/download_job.py
 -rw-r--r--  2.0 unx     6484 b- defN 80-Jan-01 00:00 abejacli/bucket/process_file_job.py
 -rw-r--r--  2.0 unx     3200 b- defN 80-Jan-01 00:00 abejacli/bucket/upload_job.py
 -rw-r--r--  2.0 unx     5354 b- defN 80-Jan-01 00:00 abejacli/click_custom.py
 -rw-r--r--  2.0 unx     5278 b- defN 80-Jan-01 00:00 abejacli/common/__init__.py
@@ -18,35 +18,37 @@
 -rw-r--r--  2.0 unx     4339 b- defN 80-Jan-01 00:00 abejacli/dataset/__init__.py
 -rw-r--r--  2.0 unx     9753 b- defN 80-Jan-01 00:00 abejacli/dataset/commands.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/docker/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/docker/commands/__init__.py
 -rw-r--r--  2.0 unx     8452 b- defN 80-Jan-01 00:00 abejacli/docker/commands/run.py
 -rw-r--r--  2.0 unx     9155 b- defN 80-Jan-01 00:00 abejacli/docker/container_run.py
 -rw-r--r--  2.0 unx      746 b- defN 80-Jan-01 00:00 abejacli/docker/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/dx_template/__init__.py
+-rw-r--r--  2.0 unx    10530 b- defN 80-Jan-01 00:00 abejacli/dx_template/commands.py
 -rw-r--r--  2.0 unx      282 b- defN 80-Jan-01 00:00 abejacli/exceptions.py
 -rw-r--r--  2.0 unx     6964 b- defN 80-Jan-01 00:00 abejacli/fs_utils.py
 -rw-r--r--  2.0 unx     1228 b- defN 80-Jan-01 00:00 abejacli/logger.py
 -rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 abejacli/model/__init__.py
 -rw-r--r--  2.0 unx     6405 b- defN 80-Jan-01 00:00 abejacli/model/docker_handler.py
 -rw-r--r--  2.0 unx     1731 b- defN 80-Jan-01 00:00 abejacli/model/local_server_manager.py
 -rw-r--r--  2.0 unx      831 b- defN 80-Jan-01 00:00 abejacli/model/runtime_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/registry/__init__.py
 -rw-r--r--  2.0 unx     5703 b- defN 80-Jan-01 00:00 abejacli/registry/commands.py
--rwxr-xr-x  2.0 unx    76654 b- defN 80-Jan-01 00:00 abejacli/run.py
+-rwxr-xr-x  2.0 unx    76738 b- defN 80-Jan-01 00:00 abejacli/run.py
 -rw-r--r--  2.0 unx     4623 b- defN 80-Jan-01 00:00 abejacli/session.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/startapp/__init__.py
 -rw-r--r--  2.0 unx     3343 b- defN 80-Jan-01 00:00 abejacli/startapp/commands.py
 -rw-r--r--  2.0 unx     1804 b- defN 80-Jan-01 00:00 abejacli/task/__init__.py
 -rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 abejacli/template/predict.py-tpl
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 abejacli/template/requirements-local.txt-tpl
 -rw-r--r--  2.0 unx     1432 b- defN 80-Jan-01 00:00 abejacli/template/train.py-tpl
 -rw-r--r--  2.0 unx     6891 b- defN 80-Jan-01 00:00 abejacli/training/__init__.py
 -rw-r--r--  2.0 unx      905 b- defN 80-Jan-01 00:00 abejacli/training/client.py
 -rw-r--r--  2.0 unx    59110 b- defN 80-Jan-01 00:00 abejacli/training/commands.py
 -rw-r--r--  2.0 unx    17869 b- defN 80-Jan-01 00:00 abejacli/training/jobs.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 abejacli/version.py
--rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4239 b- defN 16-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/RECORD
-50 files, 315588 bytes uncompressed, 73654 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     4415 b- defN 16-Jan-01 00:00 abejacli-2.2.0rc2.dist-info/RECORD
+52 files, 326378 bytes uncompressed, 77264 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -63,14 +63,20 @@
 
 Filename: abejacli/docker/container_run.py
 Comment: 
 
 Filename: abejacli/docker/utils.py
 Comment: 
 
+Filename: abejacli/dx_template/__init__.py
+Comment: 
+
+Filename: abejacli/dx_template/commands.py
+Comment: 
+
 Filename: abejacli/exceptions.py
 Comment: 
 
 Filename: abejacli/fs_utils.py
 Comment: 
 
 Filename: abejacli/logger.py
@@ -129,23 +135,23 @@
 
 Filename: abejacli/training/jobs.py
 Comment: 
 
 Filename: abejacli/version.py
 Comment: 
 
-Filename: abejacli-2.2.0rc1.dist-info/LICENSE
+Filename: abejacli-2.2.0rc2.dist-info/LICENSE
 Comment: 
 
-Filename: abejacli-2.2.0rc1.dist-info/METADATA
+Filename: abejacli-2.2.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: abejacli-2.2.0rc1.dist-info/WHEEL
+Filename: abejacli-2.2.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: abejacli-2.2.0rc1.dist-info/entry_points.txt
+Filename: abejacli-2.2.0rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: abejacli-2.2.0rc1.dist-info/RECORD
+Filename: abejacli-2.2.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abejacli/run.py

```diff
@@ -61,14 +61,15 @@
     generate_channel_file_iter_by_id,
     generate_channel_file_iter_by_period,
     upload_to_datalake
 )
 from abejacli.dataset.commands import dataset
 from abejacli.docker.commands.run import ModelRunCommand
 from abejacli.docker.utils import check_docker_installation
+from abejacli.dx_template.commands import dx_template
 from abejacli.fs_utils import (
     InvalidPathException,
     UploadBucketFile,
     UploadFile,
     generate_upload_bucket_iter,
     generate_upload_file_iter,
     get_compressed_file
@@ -1894,11 +1895,12 @@
 
 
 # add subcommands
 main.add_command(training)
 main.add_command(registry)
 main.add_command(startapp)
 main.add_command(dataset)
+main.add_command(dx_template)
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `abejacli-2.2.0rc1.dist-info/LICENSE` & `abejacli-2.2.0rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abejacli-2.2.0rc1.dist-info/METADATA` & `abejacli-2.2.0rc2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abejacli
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: ABEJA Platform Command line tool
 License: Apache-2.0
 Author: ABEJA Inc.
 Author-email: platform-support@abejainc.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `abejacli-2.2.0rc1.dist-info/RECORD` & `abejacli-2.2.0rc2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,36 @@
 abejacli/dataset/__init__.py,sha256=pAsg3XaP7io6A6o9_KzXVmjrduu6keKt0GMtd5fsdtw,4339
 abejacli/dataset/commands.py,sha256=gWtysraygVHBy19pxk0OQWAJpF12PX5BtpOMdLaxJP8,9753
 abejacli/docker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/docker/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/docker/commands/run.py,sha256=plvtD0m5sHL2IzmpGMNc4SOH_ed1SL9lJ9qEav1Nhrk,8452
 abejacli/docker/container_run.py,sha256=9xZ3Y4hwszpLST1MUnf5tseZ2h2Eoc9vrdB9Q2rR-e0,9155
 abejacli/docker/utils.py,sha256=nCTlrvmWreW9jf5gg5ZCotFxq8k2-EWY2jtijkdrd60,746
+abejacli/dx_template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+abejacli/dx_template/commands.py,sha256=T8SHxk30uHqJKTQD99DftQDLMjjkXagycYNGY-XLGW0,10530
 abejacli/exceptions.py,sha256=BOSeNT7GgQMQ0-IVdbzCKtflAqWfQUT58LydccKCMIY,282
 abejacli/fs_utils.py,sha256=V6uWQ1knu0OOxGdG2XHGwOEeUTwFpMd1T9a_eF85GkA,6964
 abejacli/logger.py,sha256=skvYF-qmkGVBbs6rzDvqibz91xoxKLh54NQGWUb8PbE,1228
 abejacli/model/__init__.py,sha256=yn_QtqimDjul0PCLa2Ps4guoDzoZcZzo4twuPuuaE-o,217
 abejacli/model/docker_handler.py,sha256=Oh5QrGHzQMwFeqea4-XuEIBf9goSPtDKU72DWa4uGqE,6405
 abejacli/model/local_server_manager.py,sha256=TRGOVSLNYbZooTNppBoKHJcoJQBqcakJNjQCFTXonnY,1731
 abejacli/model/runtime_utils.py,sha256=GsCmE-Avb4oOrreSRh_YNc-KQ4M-G5Vi370gAERgkQk,831
 abejacli/registry/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/registry/commands.py,sha256=1Ea-XdLUY2Smmjj2-1zRv7vVrR8xtomgtJnHEYapINw,5703
-abejacli/run.py,sha256=0T3CS2jjTxmm9uiFlCIktMCF2SY5A0-PMjRPMyqW874,76654
+abejacli/run.py,sha256=uWVEZ5-FQGWHQJ8bUZQk_KDcC7NkluTTyYGJQpqPaD0,76738
 abejacli/session.py,sha256=M6JxGW30YvZzREv3VDPSiqGV0ND8h6COE4P3TH3IlkU,4623
 abejacli/startapp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/startapp/commands.py,sha256=rkoSo_Ky6X5NfTCjvaYesUQRA3_I4cozKYDf-MlpKn4,3343
 abejacli/task/__init__.py,sha256=FWyS657o-AKHdHzK6t3_XYUYerTjvn76JneNjgvz43E,1804
 abejacli/template/predict.py-tpl,sha256=XQaP8Q6748QVtT7Vr3s2jzB9HE0ZkOq2m_WJXiiNJMo,3233
 abejacli/template/requirements-local.txt-tpl,sha256=i_YQz8eFRWEs7hEWL-ww8UyVhLAzQcasrROGjVWp0nk,25
 abejacli/template/train.py-tpl,sha256=fTqep3aHzojqX664KExwotET8WihoqLMlSZhpybQZTc,1432
 abejacli/training/__init__.py,sha256=G8P-bJOy0Hjb-C_EA7NfP-M884PWlIAKLXwf53B9E54,6891
 abejacli/training/client.py,sha256=CLjI_UojbGLiTJg-mPFIcAv4-2npGCM3Se1TniB6hp8,905
 abejacli/training/commands.py,sha256=3WpVkEEnHT5GAkhSFnCa3lrsSN7xhFgJbSg7YAfFf9A,59110
 abejacli/training/jobs.py,sha256=PN1oW40dZNoJbdcxmyeF_8tlbNFog8RpKOQZvnGHegA,17869
 abejacli/version.py,sha256=g4QC6oBBD54l5EAZFkxCrEY9h47YON2VDCA9PItYOQM,83
-abejacli-2.2.0rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
-abejacli-2.2.0rc1.dist-info/METADATA,sha256=Pt0MU1tNhUBuOu2nRcTmSz2Re-OPXBxo9MKb80vIsH8,1107
-abejacli-2.2.0rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-abejacli-2.2.0rc1.dist-info/entry_points.txt,sha256=0sfIdUU9v0_JsInKJ7Qf5pVUSL9wbAlOOXp7qCHDDjg,43
-abejacli-2.2.0rc1.dist-info/RECORD,,
+abejacli-2.2.0rc2.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
+abejacli-2.2.0rc2.dist-info/METADATA,sha256=kkl7QjH2qjjq8fqOZC7xS7LLx6flLcS9b3BfK9oMQA0,1107
+abejacli-2.2.0rc2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+abejacli-2.2.0rc2.dist-info/entry_points.txt,sha256=0sfIdUU9v0_JsInKJ7Qf5pVUSL9wbAlOOXp7qCHDDjg,43
+abejacli-2.2.0rc2.dist-info/RECORD,,
```

