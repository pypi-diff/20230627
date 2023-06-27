# Comparing `tmp/dopplrSDK-2.6.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4895 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    10779 b- defN 23-Jun-26 12:17 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-27 07:58 dopplrSDK-2.6.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-27 07:58 dopplrSDK-2.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 07:58 dopplrSDK-2.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-27 07:58 dopplrSDK-2.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jun-27 07:58 dopplrSDK-2.6.0.dist-info/RECORD
-6 files, 13058 bytes uncompressed, 4029 bytes compressed:  69.1%
+Zip file size: 4941 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    11035 b- defN 23-Jun-27 08:59 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/RECORD
+6 files, 13314 bytes uncompressed, 4075 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.6.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.6.0.dist-info/METADATA
+Filename: dopplrSDK-2.7.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.6.0.dist-info/WHEEL
+Filename: dopplrSDK-2.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.6.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.6.0.dist-info/RECORD
+Filename: dopplrSDK-2.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -172,15 +172,15 @@
             print('folder exists')
         else:
             os.mkdir(destination)
         if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
             response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
             destination=destination+'/'+fileName
             for obj in response['Contents']:
-                key = obj['Key']               
+                key = obj['Key']
                 is_same = is_file_name_same(key, fileName)
                 if(is_same):                
                     client.download_file(ContainerName, key, destination)
                     print("download")
         else:
             container_client = client.get_container_client(ContainerName)
 
@@ -198,46 +198,48 @@
                         
     except Exception as error:
         print("Error : ",error)
 
 def getWorkspaceFolderFiles(folder,destination,loginName,de_key):
     try:
         keys,db,client=decrypt_keys(de_key)
-
-        query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
+        query="select DOR.\"OrgName\",Du.\"UserKey\",DL.\"ConnectionString\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" join doppler.\"DopplerLake\" DL on DL.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"="+"'"+loginName+"'"+" and \"TableName\"='"+folder+"'"
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         UserKey=results[1]
         OrgName=results[0]
-        folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
+        folder_prefix = results[2]
+        folder_prefix=folder_prefix.replace('/'+folder,'')
         ContainerName = keys['Bucket']
+        if os.path.exists(destination):
+            print('folder exists')
+        else:
+            os.mkdir(destination)
         if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
             response = client.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
             for obj in response['Contents']:
                 key = obj['Key']
                 if not key.endswith('/'):  # Exclude subdirectories
                     file_name = os.path.join(destination, os.path.basename(key))
                     client.download_file(ContainerName, key, file_name)  # Download the file
             print("downloaded")
         else:
             
             folder_prefix = OrgName+'/'+loginName.upper()+'/'+folder
             container_client = client.get_container_client(ContainerName)
             blobs = container_client.list_blobs(name_starts_with=folder_prefix)
-
             for blob in blobs:
                 blob_client = container_client.get_blob_client(blob.name)
                 file_path = os.path.join(destination, os.path.basename(blob.name))
                 os.makedirs(os.path.dirname(file_path), exist_ok=True)
                 with open(file_path, "wb") as file:
                     file.write(blob_client.download_blob().readall())
             print("downloaded")
 
         
     except Exception as error:
         print("Error : ",error)
 
 
 
-
```

## Comparing `dopplrSDK-2.6.0.dist-info/LICENSE.txt` & `dopplrSDK-2.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.6.0.dist-info/METADATA` & `dopplrSDK-2.7.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.6.0
+Version: 2.7.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

