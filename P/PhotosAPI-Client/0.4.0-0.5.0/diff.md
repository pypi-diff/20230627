# Comparing `tmp/PhotosAPI_Client-0.4.0.tar.gz` & `tmp/PhotosAPI_Client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhotosAPI_Client-0.4.0.tar", last modified: Thu Jun 22 12:51:32 2023, max compression
+gzip compressed data, was "PhotosAPI_Client-0.5.0.tar", last modified: Tue Jun 27 12:04:04 2023, max compression
```

## Comparing `PhotosAPI_Client-0.4.0.tar` & `PhotosAPI_Client-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.152751 PhotosAPI_Client-0.4.0/
--rw-rw-rw-   0        0        0     4050 2023-06-22 12:51:32.150756 PhotosAPI_Client-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.974874 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/
--rw-rw-rw-   0        0        0     4050 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2875 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3864 2023-06-22 11:55:39.000000 PhotosAPI_Client-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.987877 PhotosAPI_Client-0.4.0/photosapi_client/
--rw-rw-rw-   0        0        0      166 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.992875 PhotosAPI_Client-0.4.0/photosapi_client/api/
--rw-rw-rw-   0        0        0       48 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.075939 PhotosAPI_Client-0.4.0/photosapi_client/api/default/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/__init__.py
--rw-rw-rw-   0        0        0     5318 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_create_albums_post.py
--rw-rw-rw-   0        0        0     4520 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_delete_album_id_delete.py
--rw-rw-rw-   0        0        0     4781 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_find_albums_get.py
--rw-rw-rw-   0        0        0     6634 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_patch_albums_id_patch.py
--rw-rw-rw-   0        0        0     5961 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_put_albums_id_put.py
--rw-rw-rw-   0        0        0     4712 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/login_for_access_token_token_post.py
--rw-rw-rw-   0        0        0     4529 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_delete_photos_id_delete.py
--rw-rw-rw-   0        0        0     9311 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py
--rw-rw-rw-   0        0        0     4610 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_photos_id_get.py
--rw-rw-rw-   0        0        0     5094 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py
--rw-rw-rw-   0        0        0     5214 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_move_photos_id_put.py
--rw-rw-rw-   0        0        0     5254 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_patch_photos_id_patch.py
--rw-rw-rw-   0        0        0     7878 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py
--rw-rw-rw-   0        0        0     4806 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py
--rw-rw-rw-   0        0        0     4808 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py
--rw-rw-rw-   0        0        0     4483 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_create_users_post.py
--rw-rw-rw-   0        0        0     4608 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_delete_users_me_delete.py
--rw-rw-rw-   0        0        0     3520 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_me_users_me_get.py
--rw-rw-rw-   0        0        0     4529 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_delete_videos_id_delete.py
--rw-rw-rw-   0        0        0     7744 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_find_albums_album_videos_get.py
--rw-rw-rw-   0        0        0     4610 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_get_videos_id_get.py
--rw-rw-rw-   0        0        0     5222 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_move_videos_id_put.py
--rw-rw-rw-   0        0        0     5254 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_patch_videos_id_patch.py
--rw-rw-rw-   0        0        0     6362 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py
--rw-rw-rw-   0        0        0     2883 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/client.py
--rw-rw-rw-   0        0        0      484 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.148751 PhotosAPI_Client-0.4.0/photosapi_client/models/
--rw-rw-rw-   0        0        0     1591 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/__init__.py
--rw-rw-rw-   0        0        0     1666 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/album.py
--rw-rw-rw-   0        0        0     1865 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/album_modified.py
--rw-rw-rw-   0        0        0     2969 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_login_for_access_token_token_post.py
--rw-rw-rw-   0        0        0     2051 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py
--rw-rw-rw-   0        0        0     1828 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_create_users_post.py
--rw-rw-rw-   0        0        0     1543 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_delete_users_me_delete.py
--rw-rw-rw-   0        0        0     2051 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py
--rw-rw-rw-   0        0        0     2205 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/http_validation_error.py
--rw-rw-rw-   0        0        0     1863 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo.py
--rw-rw-rw-   0        0        0     1759 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo_public.py
--rw-rw-rw-   0        0        0     1887 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo_search.py
--rw-rw-rw-   0        0        0     2262 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_album.py
--rw-rw-rw-   0        0        0     2306 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_photo.py
--rw-rw-rw-   0        0        0     2306 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_video.py
--rw-rw-rw-   0        0        0     1667 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/token.py
--rw-rw-rw-   0        0        0     1935 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/user.py
--rw-rw-rw-   0        0        0     2178 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/validation_error.py
--rw-rw-rw-   0        0        0     1863 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video.py
--rw-rw-rw-   0        0        0     1759 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video_public.py
--rw-rw-rw-   0        0        0     1887 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video_search.py
--rw-rw-rw-   0        0        0       25 2023-06-22 12:46:06.000000 PhotosAPI_Client-0.4.0/photosapi_client/py.typed
--rw-rw-rw-   0        0        0     1037 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/types.py
--rw-rw-rw-   0        0        0      215 2023-06-22 11:55:39.000000 PhotosAPI_Client-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 12:51:32.153751 PhotosAPI_Client-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-22 12:46:42.000000 PhotosAPI_Client-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:04.008088 PhotosAPI_Client-0.5.0/
+-rw-rw-rw-   0        0        0     4111 2023-06-27 12:04:04.007082 PhotosAPI_Client-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:03.848524 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/
+-rw-rw-rw-   0        0        0     4111 2023-06-27 12:04:03.000000 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3137 2023-06-27 12:04:03.000000 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:04:03.000000 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-27 12:04:03.000000 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 12:04:03.000000 PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3775 2023-03-23 11:50:59.000000 PhotosAPI_Client-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:03.857042 PhotosAPI_Client-0.5.0/photosapi_client/
+-rw-rw-rw-   0        0        0      166 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:03.859041 PhotosAPI_Client-0.5.0/photosapi_client/api/
+-rw-rw-rw-   0        0        0       48 2023-06-27 12:02:23.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:03.933268 PhotosAPI_Client-0.5.0/photosapi_client/api/default/
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:02:23.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/__init__.py
+-rw-rw-rw-   0        0        0     5318 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_create_albums_post.py
+-rw-rw-rw-   0        0        0     4520 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_delete_album_id_delete.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_find_albums_get.py
+-rw-rw-rw-   0        0        0     6634 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_patch_albums_id_patch.py
+-rw-rw-rw-   0        0        0     5961 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_put_albums_id_put.py
+-rw-rw-rw-   0        0        0     4712 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/login_for_access_token_token_post.py
+-rw-rw-rw-   0        0        0     4529 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_delete_photos_id_delete.py
+-rw-rw-rw-   0        0        0     9311 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py
+-rw-rw-rw-   0        0        0     4610 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_get_photos_id_get.py
+-rw-rw-rw-   0        0        0     5094 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py
+-rw-rw-rw-   0        0        0     5214 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_move_photos_id_put.py
+-rw-rw-rw-   0        0        0     5254 2023-06-27 12:02:26.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_patch_photos_id_patch.py
+-rw-rw-rw-   0        0        0     6479 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_random_albums_album_photos_random_get.py
+-rw-rw-rw-   0        0        0     7878 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py
+-rw-rw-rw-   0        0        0     4806 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py
+-rw-rw-rw-   0        0        0     4808 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py
+-rw-rw-rw-   0        0        0     4483 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_create_users_post.py
+-rw-rw-rw-   0        0        0     4608 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_delete_users_me_delete.py
+-rw-rw-rw-   0        0        0     3520 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_me_users_me_get.py
+-rw-rw-rw-   0        0        0     4529 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_delete_videos_id_delete.py
+-rw-rw-rw-   0        0        0     7744 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_find_albums_album_videos_get.py
+-rw-rw-rw-   0        0        0     4610 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_get_videos_id_get.py
+-rw-rw-rw-   0        0        0     5222 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_move_videos_id_put.py
+-rw-rw-rw-   0        0        0     5254 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_patch_videos_id_patch.py
+-rw-rw-rw-   0        0        0     6479 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_random_albums_album_videos_random_get.py
+-rw-rw-rw-   0        0        0     6362 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py
+-rw-rw-rw-   0        0        0     2883 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/client.py
+-rw-rw-rw-   0        0        0      484 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:04:04.004631 PhotosAPI_Client-0.5.0/photosapi_client/models/
+-rw-rw-rw-   0        0        0     1791 2023-06-27 12:02:23.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/__init__.py
+-rw-rw-rw-   0        0        0     1666 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/album.py
+-rw-rw-rw-   0        0        0     1865 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/album_modified.py
+-rw-rw-rw-   0        0        0     2969 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/body_login_for_access_token_token_post.py
+-rw-rw-rw-   0        0        0     2051 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py
+-rw-rw-rw-   0        0        0     1828 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/body_user_create_users_post.py
+-rw-rw-rw-   0        0        0     1543 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/body_user_delete_users_me_delete.py
+-rw-rw-rw-   0        0        0     2051 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py
+-rw-rw-rw-   0        0        0     2205 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/http_validation_error.py
+-rw-rw-rw-   0        0        0     1863 2023-06-27 12:02:27.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/photo.py
+-rw-rw-rw-   0        0        0     1759 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/photo_public.py
+-rw-rw-rw-   0        0        0     1887 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/photo_search.py
+-rw-rw-rw-   0        0        0     2008 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/random_search_results_photo.py
+-rw-rw-rw-   0        0        0     2008 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/random_search_results_video.py
+-rw-rw-rw-   0        0        0     2262 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_album.py
+-rw-rw-rw-   0        0        0     2306 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_photo.py
+-rw-rw-rw-   0        0        0     2306 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_video.py
+-rw-rw-rw-   0        0        0     1667 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/token.py
+-rw-rw-rw-   0        0        0     1935 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/user.py
+-rw-rw-rw-   0        0        0     2178 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/validation_error.py
+-rw-rw-rw-   0        0        0     1863 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/video.py
+-rw-rw-rw-   0        0        0     1759 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/video_public.py
+-rw-rw-rw-   0        0        0     1887 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/models/video_search.py
+-rw-rw-rw-   0        0        0       25 2023-06-27 12:02:23.000000 PhotosAPI_Client-0.5.0/photosapi_client/py.typed
+-rw-rw-rw-   0        0        0     1037 2023-06-27 12:02:28.000000 PhotosAPI_Client-0.5.0/photosapi_client/types.py
+-rw-rw-rw-   0        0        0      199 2023-03-22 20:58:23.000000 PhotosAPI_Client-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:04:04.008088 PhotosAPI_Client-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-27 12:03:13.000000 PhotosAPI_Client-0.5.0/setup.py
```

### Comparing `PhotosAPI_Client-0.4.0/PKG-INFO` & `PhotosAPI_Client-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: PhotosAPI_Client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A client library for accessing Photos API
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # PhotosAPI_Client
 A client library for accessing Photos API
 
 ## Usage
@@ -90,7 +93,9 @@
 1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
 
 If you want to install this client into another project without publishing it (e.g. for development) then:
 1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
 1. If that project is not using Poetry:
     1. Build a wheel with `poetry build -f wheel`
     1. Install that wheel from the other project `pip install <path-to-wheel>`
+
+
```

### Comparing `PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/PKG-INFO` & `PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: PhotosAPI-Client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A client library for accessing Photos API
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # PhotosAPI_Client
 A client library for accessing Photos API
 
 ## Usage
@@ -90,7 +93,9 @@
 1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
 
 If you want to install this client into another project without publishing it (e.g. for development) then:
 1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
 1. If that project is not using Poetry:
     1. Build a wheel with `poetry build -f wheel`
     1. Install that wheel from the other project `pip install <path-to-wheel>`
+
+
```

### Comparing `PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/SOURCES.txt` & `PhotosAPI_Client-0.5.0/PhotosAPI_Client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,38 +21,42 @@
 photosapi_client/api/default/login_for_access_token_token_post.py
 photosapi_client/api/default/photo_delete_photos_id_delete.py
 photosapi_client/api/default/photo_find_albums_album_photos_get.py
 photosapi_client/api/default/photo_get_photos_id_get.py
 photosapi_client/api/default/photo_get_token_token_photo_token_get.py
 photosapi_client/api/default/photo_move_photos_id_put.py
 photosapi_client/api/default/photo_patch_photos_id_patch.py
+photosapi_client/api/default/photo_random_albums_album_photos_random_get.py
 photosapi_client/api/default/photo_upload_albums_album_photos_post.py
 photosapi_client/api/default/user_confirm_users_user_confirm_get.py
 photosapi_client/api/default/user_confirm_users_user_confirm_patch.py
 photosapi_client/api/default/user_create_users_post.py
 photosapi_client/api/default/user_delete_users_me_delete.py
 photosapi_client/api/default/user_me_users_me_get.py
 photosapi_client/api/default/video_delete_videos_id_delete.py
 photosapi_client/api/default/video_find_albums_album_videos_get.py
 photosapi_client/api/default/video_get_videos_id_get.py
 photosapi_client/api/default/video_move_videos_id_put.py
 photosapi_client/api/default/video_patch_videos_id_patch.py
+photosapi_client/api/default/video_random_albums_album_videos_random_get.py
 photosapi_client/api/default/video_upload_albums_album_videos_post.py
 photosapi_client/models/__init__.py
 photosapi_client/models/album.py
 photosapi_client/models/album_modified.py
 photosapi_client/models/body_login_for_access_token_token_post.py
 photosapi_client/models/body_photo_upload_albums_album_photos_post.py
 photosapi_client/models/body_user_create_users_post.py
 photosapi_client/models/body_user_delete_users_me_delete.py
 photosapi_client/models/body_video_upload_albums_album_videos_post.py
 photosapi_client/models/http_validation_error.py
 photosapi_client/models/photo.py
 photosapi_client/models/photo_public.py
 photosapi_client/models/photo_search.py
+photosapi_client/models/random_search_results_photo.py
+photosapi_client/models/random_search_results_video.py
 photosapi_client/models/search_results_album.py
 photosapi_client/models/search_results_photo.py
 photosapi_client/models/search_results_video.py
 photosapi_client/models/token.py
 photosapi_client/models/user.py
 photosapi_client/models/validation_error.py
 photosapi_client/models/video.py
```

### Comparing `PhotosAPI_Client-0.4.0/README.md` & `PhotosAPI_Client-0.5.0/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# PhotosAPI_Client
-A client library for accessing Photos API
-
-## Usage
-First, create a client:
-
-```python
-from photosapi_client import Client
-
-client = Client(base_url="https://api.example.com")
-```
-
-If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
-
-```python
-from photosapi_client import AuthenticatedClient
-
-client = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")
-```
-
-Now call your endpoint and use your models:
-
-```python
-from photosapi_client.models import MyDataModel
-from photosapi_client.api.my_tag import get_my_data_model
-from photosapi_client.types import Response
-
-my_data: MyDataModel = get_my_data_model.sync(client=client)
-# or if you need more info (e.g. status_code)
-response: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)
-```
-
-Or do the same thing with an async version:
-
-```python
-from photosapi_client.models import MyDataModel
-from photosapi_client.api.my_tag import get_my_data_model
-from photosapi_client.types import Response
-
-my_data: MyDataModel = await get_my_data_model.asyncio(client=client)
-response: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)
-```
-
-By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
-
-```python
-client = AuthenticatedClient(
-    base_url="https://internal_api.example.com", 
-    token="SuperSecretToken",
-    verify_ssl="/path/to/certificate_bundle.pem",
-)
-```
-
-You can also disable certificate validation altogether, but beware that **this is a security risk**.
-
-```python
-client = AuthenticatedClient(
-    base_url="https://internal_api.example.com", 
-    token="SuperSecretToken", 
-    verify_ssl=False
-)
-```
-
-There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info.
-
-Things to know:
-1. Every path/method combo becomes a Python module with four functions:
-    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
-    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
-    1. `asyncio`: Like `sync` but async instead of blocking
-    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
-
-1. All path/query params, and bodies become method arguments.
-1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)
-1. Any endpoint which did not have a tag will be in `photosapi_client.api.default`
-
-## Building / publishing this Client
-This project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:
-1. Update the metadata in pyproject.toml (e.g. authors, version)
-1. If you're using a private repository, configure it with Poetry
-    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`
-    1. `poetry config http-basic.<your-repository-name> <username> <password>`
-1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
-
-If you want to install this client into another project without publishing it (e.g. for development) then:
-1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
-1. If that project is not using Poetry:
-    1. Build a wheel with `poetry build -f wheel`
-    1. Install that wheel from the other project `pip install <path-to-wheel>`
+# PhotosAPI_Client
+A client library for accessing Photos API
+
+## Usage
+First, create a client:
+
+```python
+from photosapi_client import Client
+
+client = Client(base_url="https://api.example.com")
+```
+
+If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
+
+```python
+from photosapi_client import AuthenticatedClient
+
+client = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")
+```
+
+Now call your endpoint and use your models:
+
+```python
+from photosapi_client.models import MyDataModel
+from photosapi_client.api.my_tag import get_my_data_model
+from photosapi_client.types import Response
+
+my_data: MyDataModel = get_my_data_model.sync(client=client)
+# or if you need more info (e.g. status_code)
+response: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)
+```
+
+Or do the same thing with an async version:
+
+```python
+from photosapi_client.models import MyDataModel
+from photosapi_client.api.my_tag import get_my_data_model
+from photosapi_client.types import Response
+
+my_data: MyDataModel = await get_my_data_model.asyncio(client=client)
+response: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)
+```
+
+By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken",
+    verify_ssl="/path/to/certificate_bundle.pem",
+)
+```
+
+You can also disable certificate validation altogether, but beware that **this is a security risk**.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken", 
+    verify_ssl=False
+)
+```
+
+There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info.
+
+Things to know:
+1. Every path/method combo becomes a Python module with four functions:
+    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
+    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
+    1. `asyncio`: Like `sync` but async instead of blocking
+    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
+
+1. All path/query params, and bodies become method arguments.
+1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)
+1. Any endpoint which did not have a tag will be in `photosapi_client.api.default`
+
+## Building / publishing this Client
+This project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:
+1. Update the metadata in pyproject.toml (e.g. authors, version)
+1. If you're using a private repository, configure it with Poetry
+    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`
+    1. `poetry config http-basic.<your-repository-name> <username> <password>`
+1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
+
+If you want to install this client into another project without publishing it (e.g. for development) then:
+1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
+1. If that project is not using Poetry:
+    1. Build a wheel with `poetry build -f wheel`
+    1. Install that wheel from the other project `pip install <path-to-wheel>`
```

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_create_albums_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_create_albums_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_delete_album_id_delete.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_delete_album_id_delete.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_find_albums_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_find_albums_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_patch_albums_id_patch.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_patch_albums_id_patch.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_put_albums_id_put.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/album_put_albums_id_put.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/login_for_access_token_token_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/login_for_access_token_token_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_delete_photos_id_delete.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_delete_photos_id_delete.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_photos_id_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_get_photos_id_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_move_photos_id_put.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_move_photos_id_put.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_patch_photos_id_patch.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_patch_photos_id_patch.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_create_users_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_create_users_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_delete_users_me_delete.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_delete_users_me_delete.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_me_users_me_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/user_me_users_me_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_delete_videos_id_delete.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_delete_videos_id_delete.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_find_albums_album_videos_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_find_albums_album_videos_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_get_videos_id_get.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_get_videos_id_get.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_move_videos_id_put.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_move_videos_id_put.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_patch_videos_id_patch.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_patch_videos_id_patch.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/client.py` & `PhotosAPI_Client-0.5.0/photosapi_client/client.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/__init__.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from .body_user_create_users_post import BodyUserCreateUsersPost
 from .body_user_delete_users_me_delete import BodyUserDeleteUsersMeDelete
 from .body_video_upload_albums_album_videos_post import BodyVideoUploadAlbumsAlbumVideosPost
 from .http_validation_error import HTTPValidationError
 from .photo import Photo
 from .photo_public import PhotoPublic
 from .photo_search import PhotoSearch
+from .random_search_results_photo import RandomSearchResultsPhoto
+from .random_search_results_video import RandomSearchResultsVideo
 from .search_results_album import SearchResultsAlbum
 from .search_results_photo import SearchResultsPhoto
 from .search_results_video import SearchResultsVideo
 from .token import Token
 from .user import User
 from .validation_error import ValidationError
 from .video import Video
@@ -29,14 +31,16 @@
     "BodyUserCreateUsersPost",
     "BodyUserDeleteUsersMeDelete",
     "BodyVideoUploadAlbumsAlbumVideosPost",
     "HTTPValidationError",
     "Photo",
     "PhotoPublic",
     "PhotoSearch",
+    "RandomSearchResultsPhoto",
+    "RandomSearchResultsVideo",
     "SearchResultsAlbum",
     "SearchResultsPhoto",
     "SearchResultsVideo",
     "Token",
     "User",
     "ValidationError",
     "Video",
```

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/album.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/album.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/album_modified.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/album_modified.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/body_login_for_access_token_token_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/body_login_for_access_token_token_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_create_users_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/body_user_create_users_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_delete_users_me_delete.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/body_user_delete_users_me_delete.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/http_validation_error.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/photo.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/photo.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/photo_public.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/photo_public.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/photo_search.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/photo_search.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_album.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_album.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_photo.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_photo.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_video.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/search_results_video.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/token.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/token.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/user.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/user.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/validation_error.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/video.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/video.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/video_public.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/video_public.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/models/video_search.py` & `PhotosAPI_Client-0.5.0/photosapi_client/models/video_search.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/photosapi_client/types.py` & `PhotosAPI_Client-0.5.0/photosapi_client/types.py`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.4.0/setup.py` & `PhotosAPI_Client-0.5.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="PhotosAPI_Client",
-    version="0.4.0",
+    version="0.5.0",
     description="A client library for accessing Photos API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     python_requires=">=3.7, <4",
     install_requires=["httpx >= 0.15.0, < 0.24.0", "attrs >= 21.3.0", "python-dateutil >= 2.8.0, < 3"],
     package_data={"photosapi_client": ["py.typed"]},
```

