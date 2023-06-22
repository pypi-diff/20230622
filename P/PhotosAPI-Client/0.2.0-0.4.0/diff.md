# Comparing `tmp/PhotosAPI_Client-0.2.0.tar.gz` & `tmp/PhotosAPI_Client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhotosAPI_Client-0.2.0.tar", last modified: Thu Mar 23 11:51:29 2023, max compression
+gzip compressed data, was "PhotosAPI_Client-0.4.0.tar", last modified: Thu Jun 22 12:51:32 2023, max compression
```

## Comparing `PhotosAPI_Client-0.2.0.tar` & `PhotosAPI_Client-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.720724 PhotosAPI_Client-0.2.0/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     3954 2023-03-23 11:51:29.719361 PhotosAPI_Client-0.2.0/PKG-INFO
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.559503 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     3954 2023-03-23 11:51:29.000000 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/PKG-INFO
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2875 2023-03-23 11:51:29.000000 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/SOURCES.txt
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)        1 2023-03-23 11:51:29.000000 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/dependency_links.txt
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)       62 2023-03-23 11:51:29.000000 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/requires.txt
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)       17 2023-03-23 11:51:29.000000 PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/top_level.txt
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     3775 2023-03-23 11:50:59.000000 PhotosAPI_Client-0.2.0/README.md
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.569821 PhotosAPI_Client-0.2.0/photosapi_client/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)      159 2023-03-23 11:48:23.000000 PhotosAPI_Client-0.2.0/photosapi_client/__init__.py
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.572077 PhotosAPI_Client-0.2.0/photosapi_client/api/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)       47 2023-03-23 11:47:38.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/__init__.py
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.646239 PhotosAPI_Client-0.2.0/photosapi_client/api/default/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:47:38.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/__init__.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     5097 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_create_albums_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4325 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_delete_album_id_delete.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4577 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_find_albums_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     6381 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_patch_albums_id_patch.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     5708 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_put_albums_id_put.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4533 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/login_for_access_token_token_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4334 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_delete_photos_id_delete.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     8986 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4310 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_get_photos_id_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4877 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4994 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_move_photos_id_put.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     5034 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_patch_photos_id_patch.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     7612 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4600 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4602 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4306 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_create_users_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4431 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_delete_users_me_delete.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     3360 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_me_users_me_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4334 2023-03-23 11:48:24.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_delete_videos_id_delete.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     7464 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_find_albums_album_videos_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     4310 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_get_videos_id_get.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     5002 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_move_videos_id_put.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     5034 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_patch_videos_id_patch.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     6129 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2673 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/client.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)      282 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/errors.py
-drwxrwxr--   0 profitroll  (1000) profitroll  (1000)        0 2023-03-23 11:51:29.713060 PhotosAPI_Client-0.2.0/photosapi_client/models/
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1546 2023-03-23 11:47:38.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/__init__.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1595 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/album.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1791 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/album_modified.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2871 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/body_login_for_access_token_token_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1976 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1757 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/body_user_create_users_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1486 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/body_user_delete_users_me_delete.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1976 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2131 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/http_validation_error.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1785 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/photo.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1688 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/photo_public.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1813 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/photo_search.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2179 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_album.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2223 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_photo.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2223 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_video.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1603 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/token.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1860 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/user.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     2091 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/validation_error.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1785 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/video.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1688 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/video_public.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)     1813 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/models/video_search.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)       25 2023-03-23 11:47:38.000000 PhotosAPI_Client-0.2.0/photosapi_client/py.typed
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)      974 2023-03-23 11:48:25.000000 PhotosAPI_Client-0.2.0/photosapi_client/types.py
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)      199 2023-03-22 20:58:23.000000 PhotosAPI_Client-0.2.0/pyproject.toml
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)       38 2023-03-23 11:51:29.721267 PhotosAPI_Client-0.2.0/setup.cfg
--rwxrwxr--   0 profitroll  (1000) profitroll  (1000)      607 2023-03-23 11:43:51.000000 PhotosAPI_Client-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.152751 PhotosAPI_Client-0.4.0/
+-rw-rw-rw-   0        0        0     4050 2023-06-22 12:51:32.150756 PhotosAPI_Client-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.974874 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/
+-rw-rw-rw-   0        0        0     4050 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2875 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 12:51:31.000000 PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3864 2023-06-22 11:55:39.000000 PhotosAPI_Client-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.987877 PhotosAPI_Client-0.4.0/photosapi_client/
+-rw-rw-rw-   0        0        0      166 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:31.992875 PhotosAPI_Client-0.4.0/photosapi_client/api/
+-rw-rw-rw-   0        0        0       48 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.075939 PhotosAPI_Client-0.4.0/photosapi_client/api/default/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/__init__.py
+-rw-rw-rw-   0        0        0     5318 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_create_albums_post.py
+-rw-rw-rw-   0        0        0     4520 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_delete_album_id_delete.py
+-rw-rw-rw-   0        0        0     4781 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_find_albums_get.py
+-rw-rw-rw-   0        0        0     6634 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_patch_albums_id_patch.py
+-rw-rw-rw-   0        0        0     5961 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_put_albums_id_put.py
+-rw-rw-rw-   0        0        0     4712 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/login_for_access_token_token_post.py
+-rw-rw-rw-   0        0        0     4529 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_delete_photos_id_delete.py
+-rw-rw-rw-   0        0        0     9311 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py
+-rw-rw-rw-   0        0        0     4610 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_photos_id_get.py
+-rw-rw-rw-   0        0        0     5094 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py
+-rw-rw-rw-   0        0        0     5214 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_move_photos_id_put.py
+-rw-rw-rw-   0        0        0     5254 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_patch_photos_id_patch.py
+-rw-rw-rw-   0        0        0     7878 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py
+-rw-rw-rw-   0        0        0     4806 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py
+-rw-rw-rw-   0        0        0     4808 2023-06-22 12:46:21.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py
+-rw-rw-rw-   0        0        0     4483 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_create_users_post.py
+-rw-rw-rw-   0        0        0     4608 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_delete_users_me_delete.py
+-rw-rw-rw-   0        0        0     3520 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_me_users_me_get.py
+-rw-rw-rw-   0        0        0     4529 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_delete_videos_id_delete.py
+-rw-rw-rw-   0        0        0     7744 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_find_albums_album_videos_get.py
+-rw-rw-rw-   0        0        0     4610 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_get_videos_id_get.py
+-rw-rw-rw-   0        0        0     5222 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_move_videos_id_put.py
+-rw-rw-rw-   0        0        0     5254 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_patch_videos_id_patch.py
+-rw-rw-rw-   0        0        0     6362 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py
+-rw-rw-rw-   0        0        0     2883 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/client.py
+-rw-rw-rw-   0        0        0      484 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:51:32.148751 PhotosAPI_Client-0.4.0/photosapi_client/models/
+-rw-rw-rw-   0        0        0     1591 2023-06-22 12:46:07.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/__init__.py
+-rw-rw-rw-   0        0        0     1666 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/album.py
+-rw-rw-rw-   0        0        0     1865 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/album_modified.py
+-rw-rw-rw-   0        0        0     2969 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_login_for_access_token_token_post.py
+-rw-rw-rw-   0        0        0     2051 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py
+-rw-rw-rw-   0        0        0     1828 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_create_users_post.py
+-rw-rw-rw-   0        0        0     1543 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_user_delete_users_me_delete.py
+-rw-rw-rw-   0        0        0     2051 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py
+-rw-rw-rw-   0        0        0     2205 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/http_validation_error.py
+-rw-rw-rw-   0        0        0     1863 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo.py
+-rw-rw-rw-   0        0        0     1759 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo_public.py
+-rw-rw-rw-   0        0        0     1887 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/photo_search.py
+-rw-rw-rw-   0        0        0     2262 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_album.py
+-rw-rw-rw-   0        0        0     2306 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_photo.py
+-rw-rw-rw-   0        0        0     2306 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_video.py
+-rw-rw-rw-   0        0        0     1667 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/token.py
+-rw-rw-rw-   0        0        0     1935 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/user.py
+-rw-rw-rw-   0        0        0     2178 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/validation_error.py
+-rw-rw-rw-   0        0        0     1863 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video.py
+-rw-rw-rw-   0        0        0     1759 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video_public.py
+-rw-rw-rw-   0        0        0     1887 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/models/video_search.py
+-rw-rw-rw-   0        0        0       25 2023-06-22 12:46:06.000000 PhotosAPI_Client-0.4.0/photosapi_client/py.typed
+-rw-rw-rw-   0        0        0     1037 2023-06-22 12:46:22.000000 PhotosAPI_Client-0.4.0/photosapi_client/types.py
+-rw-rw-rw-   0        0        0      215 2023-06-22 11:55:39.000000 PhotosAPI_Client-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:51:32.153751 PhotosAPI_Client-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-22 12:46:42.000000 PhotosAPI_Client-0.4.0/setup.py
```

### Comparing `PhotosAPI_Client-0.2.0/PKG-INFO` & `PhotosAPI_Client-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,89 @@
-Metadata-Version: 2.1
-Name: PhotosAPI_Client
-Version: 0.2.0
-Summary: A client library for accessing Photos API
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-
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

### Comparing `PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/PKG-INFO` & `PhotosAPI_Client-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: PhotosAPI-Client
-Version: 0.2.0
-Summary: A client library for accessing Photos API
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-
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
+Metadata-Version: 2.1
+Name: PhotosAPI_Client
+Version: 0.4.0
+Summary: A client library for accessing Photos API
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+
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

### Comparing `PhotosAPI_Client-0.2.0/PhotosAPI_Client.egg-info/SOURCES.txt` & `PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PhotosAPI_Client-0.2.0/README.md` & `PhotosAPI_Client-0.4.0/PhotosAPI_Client.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,96 @@
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
+Metadata-Version: 2.1
+Name: PhotosAPI-Client
+Version: 0.4.0
+Summary: A client library for accessing Photos API
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+
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

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_create_albums_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_patch_photos_id_patch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.album import Album
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-) -> Dict[str, Any]:
-    url = "{}/albums".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["name"] = name
-
-    params["title"] = title
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Album, Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Album.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_ACCEPTABLE:
-        response_406 = cast(Any, None)
-        return response_406
-    if response.status_code == HTTPStatus.CONFLICT:
-        response_409 = cast(Any, None)
-        return response_409
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Album, Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-) -> Response[Union[Album, Any, HTTPValidationError]]:
-    """Album Create
-
-     Create album with name and title
-
-    Args:
-        name (str):
-        title (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Album, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        name=name,
-        title=title,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-) -> Optional[Union[Album, Any, HTTPValidationError]]:
-    """Album Create
-
-     Create album with name and title
-
-    Args:
-        name (str):
-        title (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Album, Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        client=client,
-        name=name,
-        title=title,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-) -> Response[Union[Album, Any, HTTPValidationError]]:
-    """Album Create
-
-     Create album with name and title
-
-    Args:
-        name (str):
-        title (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Album, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        name=name,
-        title=title,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-) -> Optional[Union[Album, Any, HTTPValidationError]]:
-    """Album Create
-
-     Create album with name and title
-
-    Args:
-        name (str):
-        title (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Album, Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            name=name,
-            title=title,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...models.photo_public import PhotoPublic
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Dict[str, Any]:
+    url = "{}/photos/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["caption"] = caption
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "patch",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = PhotoPublic.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
+    """Photo Patch
+
+     Change properties of a photo
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, PhotoPublic]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        caption=caption,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
+    """Photo Patch
+
+     Change properties of a photo
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, PhotoPublic]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+        caption=caption,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
+    """Photo Patch
+
+     Change properties of a photo
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, PhotoPublic]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        caption=caption,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
+    """Photo Patch
+
+     Change properties of a photo
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, PhotoPublic]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+            caption=caption,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_delete_album_id_delete.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_photos_id_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,175 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
-    url = "{}/album/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Album Delete
-
-     Delete album by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Album Delete
-
-     Delete album by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Album Delete
-
-     Delete album by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Album Delete
-
-     Delete album by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-        )
-    ).parsed
+from http import HTTPStatus
+from io import BytesIO
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import File, Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Dict[str, Any]:
+    url = "{}/photos/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, File, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = File(payload=BytesIO(response.content))
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, File, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, File, HTTPValidationError]]:
+    """Photo Get
+
+     Get a photo by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, File, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, File, HTTPValidationError]]:
+    """Photo Get
+
+     Get a photo by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, File, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, File, HTTPValidationError]]:
+    """Photo Get
+
+     Get a photo by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, File, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, File, HTTPValidationError]]:
+    """Photo Get
+
+     Get a photo by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, File, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_find_albums_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_find_albums_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,181 +1,182 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...models.search_results_album import SearchResultsAlbum
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    q: str,
-) -> Dict[str, Any]:
-    url = "{}/albums".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["q"] = q
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = SearchResultsAlbum.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    q: str,
-) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
-    """Album Find
-
-     Find album by name
-
-    Args:
-        q (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[HTTPValidationError, SearchResultsAlbum]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        q=q,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    q: str,
-) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
-    """Album Find
-
-     Find album by name
-
-    Args:
-        q (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[HTTPValidationError, SearchResultsAlbum]]
-    """
-
-    return sync_detailed(
-        client=client,
-        q=q,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    q: str,
-) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
-    """Album Find
-
-     Find album by name
-
-    Args:
-        q (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[HTTPValidationError, SearchResultsAlbum]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        q=q,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    q: str,
-) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
-    """Album Find
-
-     Find album by name
-
-    Args:
-        q (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[HTTPValidationError, SearchResultsAlbum]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            q=q,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...models.search_results_album import SearchResultsAlbum
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    q: str,
+) -> Dict[str, Any]:
+    url = "{}/albums".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["q"] = q
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = SearchResultsAlbum.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    q: str,
+) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
+    """Album Find
+
+     Find album by name
+
+    Args:
+        q (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[HTTPValidationError, SearchResultsAlbum]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        q=q,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    q: str,
+) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
+    """Album Find
+
+     Find album by name
+
+    Args:
+        q (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[HTTPValidationError, SearchResultsAlbum]
+    """
+
+    return sync_detailed(
+        client=client,
+        q=q,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    q: str,
+) -> Response[Union[HTTPValidationError, SearchResultsAlbum]]:
+    """Album Find
+
+     Find album by name
+
+    Args:
+        q (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[HTTPValidationError, SearchResultsAlbum]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        q=q,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    q: str,
+) -> Optional[Union[HTTPValidationError, SearchResultsAlbum]]:
+    """Album Find
+
+     Find album by name
+
+    Args:
+        q (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[HTTPValidationError, SearchResultsAlbum]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            q=q,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_patch_albums_id_patch.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_patch_albums_id_patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,230 +1,231 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.album_modified import AlbumModified
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: Union[Unset, None, str] = UNSET,
-    title: Union[Unset, None, str] = UNSET,
-    cover: Union[Unset, None, str] = UNSET,
-) -> Dict[str, Any]:
-    url = "{}/albums/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["name"] = name
-
-    params["title"] = title
-
-    params["cover"] = cover
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "patch",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = AlbumModified.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.NOT_ACCEPTABLE:
-        response_406 = cast(Any, None)
-        return response_406
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: Union[Unset, None, str] = UNSET,
-    title: Union[Unset, None, str] = UNSET,
-    cover: Union[Unset, None, str] = UNSET,
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Patch
-
-     Modify album's name or title by id
-
-    Args:
-        id (str):
-        name (Union[Unset, None, str]):
-        title (Union[Unset, None, str]):
-        cover (Union[Unset, None, str]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: Union[Unset, None, str] = UNSET,
-    title: Union[Unset, None, str] = UNSET,
-    cover: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Patch
-
-     Modify album's name or title by id
-
-    Args:
-        id (str):
-        name (Union[Unset, None, str]):
-        title (Union[Unset, None, str]):
-        cover (Union[Unset, None, str]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: Union[Unset, None, str] = UNSET,
-    title: Union[Unset, None, str] = UNSET,
-    cover: Union[Unset, None, str] = UNSET,
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Patch
-
-     Modify album's name or title by id
-
-    Args:
-        id (str):
-        name (Union[Unset, None, str]):
-        title (Union[Unset, None, str]):
-        cover (Union[Unset, None, str]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: Union[Unset, None, str] = UNSET,
-    title: Union[Unset, None, str] = UNSET,
-    cover: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Patch
-
-     Modify album's name or title by id
-
-    Args:
-        id (str):
-        name (Union[Unset, None, str]):
-        title (Union[Unset, None, str]):
-        cover (Union[Unset, None, str]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-            name=name,
-            title=title,
-            cover=cover,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.album_modified import AlbumModified
+from ...models.http_validation_error import HTTPValidationError
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    name: Union[Unset, None, str] = UNSET,
+    title: Union[Unset, None, str] = UNSET,
+    cover: Union[Unset, None, str] = UNSET,
+) -> Dict[str, Any]:
+    url = "{}/albums/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["name"] = name
+
+    params["title"] = title
+
+    params["cover"] = cover
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "patch",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = AlbumModified.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.NOT_ACCEPTABLE:
+        response_406 = cast(Any, None)
+        return response_406
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    name: Union[Unset, None, str] = UNSET,
+    title: Union[Unset, None, str] = UNSET,
+    cover: Union[Unset, None, str] = UNSET,
+) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
+    """Album Patch
+
+     Modify album's name or title by id
+
+    Args:
+        id (str):
+        name (Union[Unset, None, str]):
+        title (Union[Unset, None, str]):
+        cover (Union[Unset, None, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[AlbumModified, Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        name=name,
+        title=title,
+        cover=cover,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    name: Union[Unset, None, str] = UNSET,
+    title: Union[Unset, None, str] = UNSET,
+    cover: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
+    """Album Patch
+
+     Modify album's name or title by id
+
+    Args:
+        id (str):
+        name (Union[Unset, None, str]):
+        title (Union[Unset, None, str]):
+        cover (Union[Unset, None, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[AlbumModified, Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+        name=name,
+        title=title,
+        cover=cover,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    name: Union[Unset, None, str] = UNSET,
+    title: Union[Unset, None, str] = UNSET,
+    cover: Union[Unset, None, str] = UNSET,
+) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
+    """Album Patch
+
+     Modify album's name or title by id
+
+    Args:
+        id (str):
+        name (Union[Unset, None, str]):
+        title (Union[Unset, None, str]):
+        cover (Union[Unset, None, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[AlbumModified, Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        name=name,
+        title=title,
+        cover=cover,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    name: Union[Unset, None, str] = UNSET,
+    title: Union[Unset, None, str] = UNSET,
+    cover: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
+    """Album Patch
+
+     Modify album's name or title by id
+
+    Args:
+        id (str):
+        name (Union[Unset, None, str]):
+        title (Union[Unset, None, str]):
+        cover (Union[Unset, None, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[AlbumModified, Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+            name=name,
+            title=title,
+            cover=cover,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/album_put_albums_id_put.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,230 +1,195 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.album_modified import AlbumModified
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-    cover: str,
-) -> Dict[str, Any]:
-    url = "{}/albums/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["name"] = name
-
-    params["title"] = title
-
-    params["cover"] = cover
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "put",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = AlbumModified.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.NOT_ACCEPTABLE:
-        response_406 = cast(Any, None)
-        return response_406
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-    cover: str,
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Put
-
-     Modify album's name and title by id
-
-    Args:
-        id (str):
-        name (str):
-        title (str):
-        cover (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-    cover: str,
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Put
-
-     Modify album's name and title by id
-
-    Args:
-        id (str):
-        name (str):
-        title (str):
-        cover (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-    cover: str,
-) -> Response[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Put
-
-     Modify album's name and title by id
-
-    Args:
-        id (str):
-        name (str):
-        title (str):
-        cover (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        name=name,
-        title=title,
-        cover=cover,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    name: str,
-    title: str,
-    cover: str,
-) -> Optional[Union[AlbumModified, Any, HTTPValidationError]]:
-    """Album Put
-
-     Modify album's name and title by id
-
-    Args:
-        id (str):
-        name (str):
-        title (str):
-        cover (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[AlbumModified, Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-            name=name,
-            title=title,
-            cover=cover,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    token: str,
+    *,
+    client: Client,
+    id: int,
+) -> Dict[str, Any]:
+    url = "{}/token/photo/{token}".format(client.base_url, token=token)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["id"] = id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = cast(Any, response.json())
+        return response_200
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = cast(Any, None)
+        return response_401
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    token: str,
+    *,
+    client: Client,
+    id: int,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Photo Get Token
+
+     Get a photo by its duplicate token
+
+    Args:
+        token (str):
+        id (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        token=token,
+        client=client,
+        id=id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    token: str,
+    *,
+    client: Client,
+    id: int,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Photo Get Token
+
+     Get a photo by its duplicate token
+
+    Args:
+        token (str):
+        id (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        token=token,
+        client=client,
+        id=id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    token: str,
+    *,
+    client: Client,
+    id: int,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Photo Get Token
+
+     Get a photo by its duplicate token
+
+    Args:
+        token (str):
+        id (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        token=token,
+        client=client,
+        id=id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    token: str,
+    *,
+    client: Client,
+    id: int,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Photo Get Token
+
+     Get a photo by its duplicate token
+
+    Args:
+        token (str):
+        id (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            token=token,
+            client=client,
+            id=id,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_delete_photos_id_delete.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_create_users_post.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,155 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
-    url = "{}/photos/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Delete
-
-     Delete a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Delete
-
-     Delete a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Delete
-
-     Delete a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Delete
-
-     Delete a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import Client
+from ...models.body_user_create_users_post import BodyUserCreateUsersPost
+from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+
+def _get_kwargs(
+    *,
+    client: Client,
+    form_data: BodyUserCreateUsersPost,
+) -> Dict[str, Any]:
+    url = "{}/users".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "post",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "data": form_data.to_dict(),
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.CONFLICT:
+        response_409 = cast(Any, None)
+        return response_409
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: Client,
+    form_data: BodyUserCreateUsersPost,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Create
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        form_data=form_data,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    *,
+    client: Client,
+    form_data: BodyUserCreateUsersPost,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Create
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        client=client,
+        form_data=form_data,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: Client,
+    form_data: BodyUserCreateUsersPost,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Create
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        form_data=form_data,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+    form_data: BodyUserCreateUsersPost,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Create
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            form_data=form_data,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_find_albums_album_photos_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_find_albums_album_videos_get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,302 +1,258 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.search_results_photo import SearchResultsPhoto
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    q: Union[Unset, None, str] = UNSET,
-    caption: Union[Unset, None, str] = UNSET,
-    token: Union[Unset, None, str] = UNSET,
-    page: Union[Unset, None, int] = 1,
-    page_size: Union[Unset, None, int] = 100,
-    lat: Union[Unset, None, float] = UNSET,
-    lng: Union[Unset, None, float] = UNSET,
-    radius: Union[Unset, None, int] = UNSET,
-) -> Dict[str, Any]:
-    url = "{}/albums/{album}/photos".format(client.base_url, album=album)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["q"] = q
-
-    params["caption"] = caption
-
-    params["token"] = token
-
-    params["page"] = page
-
-    params["page_size"] = page_size
-
-    params["lat"] = lat
-
-    params["lng"] = lng
-
-    params["radius"] = radius
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, SearchResultsPhoto]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = SearchResultsPhoto.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = cast(Any, None)
-        return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
-        return response_401
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = cast(Any, None)
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, SearchResultsPhoto]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    q: Union[Unset, None, str] = UNSET,
-    caption: Union[Unset, None, str] = UNSET,
-    token: Union[Unset, None, str] = UNSET,
-    page: Union[Unset, None, int] = 1,
-    page_size: Union[Unset, None, int] = 100,
-    lat: Union[Unset, None, float] = UNSET,
-    lng: Union[Unset, None, float] = UNSET,
-    radius: Union[Unset, None, int] = UNSET,
-) -> Response[Union[Any, SearchResultsPhoto]]:
-    """Photo Find
-
-     Find a photo by filename, caption, location or token
-
-    Args:
-        album (str):
-        q (Union[Unset, None, str]):
-        caption (Union[Unset, None, str]):
-        token (Union[Unset, None, str]):
-        page (Union[Unset, None, int]):  Default: 1.
-        page_size (Union[Unset, None, int]):  Default: 100.
-        lat (Union[Unset, None, float]):
-        lng (Union[Unset, None, float]):
-        radius (Union[Unset, None, int]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, SearchResultsPhoto]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        q=q,
-        caption=caption,
-        token=token,
-        page=page,
-        page_size=page_size,
-        lat=lat,
-        lng=lng,
-        radius=radius,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    q: Union[Unset, None, str] = UNSET,
-    caption: Union[Unset, None, str] = UNSET,
-    token: Union[Unset, None, str] = UNSET,
-    page: Union[Unset, None, int] = 1,
-    page_size: Union[Unset, None, int] = 100,
-    lat: Union[Unset, None, float] = UNSET,
-    lng: Union[Unset, None, float] = UNSET,
-    radius: Union[Unset, None, int] = UNSET,
-) -> Optional[Union[Any, SearchResultsPhoto]]:
-    """Photo Find
-
-     Find a photo by filename, caption, location or token
-
-    Args:
-        album (str):
-        q (Union[Unset, None, str]):
-        caption (Union[Unset, None, str]):
-        token (Union[Unset, None, str]):
-        page (Union[Unset, None, int]):  Default: 1.
-        page_size (Union[Unset, None, int]):  Default: 100.
-        lat (Union[Unset, None, float]):
-        lng (Union[Unset, None, float]):
-        radius (Union[Unset, None, int]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, SearchResultsPhoto]]
-    """
-
-    return sync_detailed(
-        album=album,
-        client=client,
-        q=q,
-        caption=caption,
-        token=token,
-        page=page,
-        page_size=page_size,
-        lat=lat,
-        lng=lng,
-        radius=radius,
-    ).parsed
-
-
-async def asyncio_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    q: Union[Unset, None, str] = UNSET,
-    caption: Union[Unset, None, str] = UNSET,
-    token: Union[Unset, None, str] = UNSET,
-    page: Union[Unset, None, int] = 1,
-    page_size: Union[Unset, None, int] = 100,
-    lat: Union[Unset, None, float] = UNSET,
-    lng: Union[Unset, None, float] = UNSET,
-    radius: Union[Unset, None, int] = UNSET,
-) -> Response[Union[Any, SearchResultsPhoto]]:
-    """Photo Find
-
-     Find a photo by filename, caption, location or token
-
-    Args:
-        album (str):
-        q (Union[Unset, None, str]):
-        caption (Union[Unset, None, str]):
-        token (Union[Unset, None, str]):
-        page (Union[Unset, None, int]):  Default: 1.
-        page_size (Union[Unset, None, int]):  Default: 100.
-        lat (Union[Unset, None, float]):
-        lng (Union[Unset, None, float]):
-        radius (Union[Unset, None, int]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, SearchResultsPhoto]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        q=q,
-        caption=caption,
-        token=token,
-        page=page,
-        page_size=page_size,
-        lat=lat,
-        lng=lng,
-        radius=radius,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    q: Union[Unset, None, str] = UNSET,
-    caption: Union[Unset, None, str] = UNSET,
-    token: Union[Unset, None, str] = UNSET,
-    page: Union[Unset, None, int] = 1,
-    page_size: Union[Unset, None, int] = 100,
-    lat: Union[Unset, None, float] = UNSET,
-    lng: Union[Unset, None, float] = UNSET,
-    radius: Union[Unset, None, int] = UNSET,
-) -> Optional[Union[Any, SearchResultsPhoto]]:
-    """Photo Find
-
-     Find a photo by filename, caption, location or token
-
-    Args:
-        album (str):
-        q (Union[Unset, None, str]):
-        caption (Union[Unset, None, str]):
-        token (Union[Unset, None, str]):
-        page (Union[Unset, None, int]):  Default: 1.
-        page_size (Union[Unset, None, int]):  Default: 100.
-        lat (Union[Unset, None, float]):
-        lng (Union[Unset, None, float]):
-        radius (Union[Unset, None, int]):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, SearchResultsPhoto]]
-    """
-
-    return (
-        await asyncio_detailed(
-            album=album,
-            client=client,
-            q=q,
-            caption=caption,
-            token=token,
-            page=page,
-            page_size=page_size,
-            lat=lat,
-            lng=lng,
-            radius=radius,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.search_results_video import SearchResultsVideo
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    q: Union[Unset, None, str] = UNSET,
+    caption: Union[Unset, None, str] = UNSET,
+    token: Union[Unset, None, str] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    page_size: Union[Unset, None, int] = 100,
+) -> Dict[str, Any]:
+    url = "{}/albums/{album}/videos".format(client.base_url, album=album)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["q"] = q
+
+    params["caption"] = caption
+
+    params["token"] = token
+
+    params["page"] = page
+
+    params["page_size"] = page_size
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, SearchResultsVideo]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = SearchResultsVideo.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = cast(Any, None)
+        return response_400
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = cast(Any, None)
+        return response_401
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = cast(Any, None)
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, SearchResultsVideo]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    q: Union[Unset, None, str] = UNSET,
+    caption: Union[Unset, None, str] = UNSET,
+    token: Union[Unset, None, str] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    page_size: Union[Unset, None, int] = 100,
+) -> Response[Union[Any, SearchResultsVideo]]:
+    """Video Find
+
+     Find a video by filename, caption or token
+
+    Args:
+        album (str):
+        q (Union[Unset, None, str]):
+        caption (Union[Unset, None, str]):
+        token (Union[Unset, None, str]):
+        page (Union[Unset, None, int]):  Default: 1.
+        page_size (Union[Unset, None, int]):  Default: 100.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, SearchResultsVideo]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        q=q,
+        caption=caption,
+        token=token,
+        page=page,
+        page_size=page_size,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    q: Union[Unset, None, str] = UNSET,
+    caption: Union[Unset, None, str] = UNSET,
+    token: Union[Unset, None, str] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    page_size: Union[Unset, None, int] = 100,
+) -> Optional[Union[Any, SearchResultsVideo]]:
+    """Video Find
+
+     Find a video by filename, caption or token
+
+    Args:
+        album (str):
+        q (Union[Unset, None, str]):
+        caption (Union[Unset, None, str]):
+        token (Union[Unset, None, str]):
+        page (Union[Unset, None, int]):  Default: 1.
+        page_size (Union[Unset, None, int]):  Default: 100.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, SearchResultsVideo]
+    """
+
+    return sync_detailed(
+        album=album,
+        client=client,
+        q=q,
+        caption=caption,
+        token=token,
+        page=page,
+        page_size=page_size,
+    ).parsed
+
+
+async def asyncio_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    q: Union[Unset, None, str] = UNSET,
+    caption: Union[Unset, None, str] = UNSET,
+    token: Union[Unset, None, str] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    page_size: Union[Unset, None, int] = 100,
+) -> Response[Union[Any, SearchResultsVideo]]:
+    """Video Find
+
+     Find a video by filename, caption or token
+
+    Args:
+        album (str):
+        q (Union[Unset, None, str]):
+        caption (Union[Unset, None, str]):
+        token (Union[Unset, None, str]):
+        page (Union[Unset, None, int]):  Default: 1.
+        page_size (Union[Unset, None, int]):  Default: 100.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, SearchResultsVideo]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        q=q,
+        caption=caption,
+        token=token,
+        page=page,
+        page_size=page_size,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    q: Union[Unset, None, str] = UNSET,
+    caption: Union[Unset, None, str] = UNSET,
+    token: Union[Unset, None, str] = UNSET,
+    page: Union[Unset, None, int] = 1,
+    page_size: Union[Unset, None, int] = 100,
+) -> Optional[Union[Any, SearchResultsVideo]]:
+    """Video Find
+
+     Find a video by filename, caption or token
+
+    Args:
+        album (str):
+        q (Union[Unset, None, str]):
+        caption (Union[Unset, None, str]):
+        token (Union[Unset, None, str]):
+        page (Union[Unset, None, int]):  Default: 1.
+        page_size (Union[Unset, None, int]):  Default: 100.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, SearchResultsVideo]
+    """
+
+    return (
+        await asyncio_detailed(
+            album=album,
+            client=client,
+            q=q,
+            caption=caption,
+            token=token,
+            page=page,
+            page_size=page_size,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_get_photos_id_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_delete_users_me_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,155 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
-    url = "{}/photos/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Get
-
-     Get a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Get
-
-     Get a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Get
-
-     Get a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Get
-
-     Get a photo by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.body_user_delete_users_me_delete import BodyUserDeleteUsersMeDelete
+from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    form_data: BodyUserDeleteUsersMeDelete,
+) -> Dict[str, Any]:
+    url = "{}/users/me/".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "data": form_data.to_dict(),
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = cast(Any, None)
+        return response_401
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    form_data: BodyUserDeleteUsersMeDelete,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Delete
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        form_data=form_data,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    form_data: BodyUserDeleteUsersMeDelete,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Delete
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        client=client,
+        form_data=form_data,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    form_data: BodyUserDeleteUsersMeDelete,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Delete
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        form_data=form_data,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    form_data: BodyUserDeleteUsersMeDelete,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Delete
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            form_data=form_data,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_get_token_token_photo_token_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_patch_videos_id_patch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,198 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    token: str,
-    *,
-    client: Client,
-    id: int,
-) -> Dict[str, Any]:
-    url = "{}/token/photo/{token}".format(client.base_url, token=token)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["id"] = id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
-        return response_401
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    token: str,
-    *,
-    client: Client,
-    id: int,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Get Token
-
-     Get a photo by its duplicate token
-
-    Args:
-        token (str):
-        id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        token=token,
-        client=client,
-        id=id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    token: str,
-    *,
-    client: Client,
-    id: int,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Get Token
-
-     Get a photo by its duplicate token
-
-    Args:
-        token (str):
-        id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        token=token,
-        client=client,
-        id=id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    token: str,
-    *,
-    client: Client,
-    id: int,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Photo Get Token
-
-     Get a photo by its duplicate token
-
-    Args:
-        token (str):
-        id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        token=token,
-        client=client,
-        id=id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    token: str,
-    *,
-    client: Client,
-    id: int,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Photo Get Token
-
-     Get a photo by its duplicate token
-
-    Args:
-        token (str):
-        id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            token=token,
-            client=client,
-            id=id,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...models.video_public import VideoPublic
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Dict[str, Any]:
+    url = "{}/videos/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["caption"] = caption
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "patch",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, VideoPublic]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = VideoPublic.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, VideoPublic]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Response[Union[Any, HTTPValidationError, VideoPublic]]:
+    """Video Patch
+
+     Change properties of a video
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, VideoPublic]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        caption=caption,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Optional[Union[Any, HTTPValidationError, VideoPublic]]:
+    """Video Patch
+
+     Change properties of a video
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, VideoPublic]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+        caption=caption,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Response[Union[Any, HTTPValidationError, VideoPublic]]:
+    """Video Patch
+
+     Change properties of a video
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, VideoPublic]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+        caption=caption,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+    caption: str,
+) -> Optional[Union[Any, HTTPValidationError, VideoPublic]]:
+    """Video Patch
+
+     Change properties of a video
+
+    Args:
+        id (str):
+        caption (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, VideoPublic]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+            caption=caption,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_move_photos_id_put.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/album_delete_album_id_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,197 +1,173 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...models.photo_public import PhotoPublic
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    album: str,
-) -> Dict[str, Any]:
-    url = "{}/photos/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["album"] = album
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "put",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = PhotoPublic.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    album: str,
-) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
-    """Photo Move
-
-     Move a photo to another album
-
-    Args:
-        id (str):
-        album (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, PhotoPublic]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        album=album,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    album: str,
-) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
-    """Photo Move
-
-     Move a photo to another album
-
-    Args:
-        id (str):
-        album (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, PhotoPublic]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-        album=album,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    album: str,
-) -> Response[Union[Any, HTTPValidationError, PhotoPublic]]:
-    """Photo Move
-
-     Move a photo to another album
-
-    Args:
-        id (str):
-        album (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, PhotoPublic]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-        album=album,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-    album: str,
-) -> Optional[Union[Any, HTTPValidationError, PhotoPublic]]:
-    """Photo Move
-
-     Move a photo to another album
-
-    Args:
-        id (str):
-        album (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, PhotoPublic]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-            album=album,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Dict[str, Any]:
+    url = "{}/album/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Album Delete
+
+     Delete album by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Album Delete
+
+     Delete album by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Album Delete
+
+     Delete album by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Album Delete
+
+     Delete album by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/photo_upload_albums_album_photos_post.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,243 +1,244 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.body_photo_upload_albums_album_photos_post import BodyPhotoUploadAlbumsAlbumPhotosPost
-from ...models.http_validation_error import HTTPValidationError
-from ...models.photo import Photo
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
-    ignore_duplicates: Union[Unset, None, bool] = False,
-    compress: Union[Unset, None, bool] = True,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Dict[str, Any]:
-    url = "{}/albums/{album}/photos".format(client.base_url, album=album)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["ignore_duplicates"] = ignore_duplicates
-
-    params["compress"] = compress
-
-    params["caption"] = caption
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    multipart_multipart_data = multipart_data.to_multipart()
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "files": multipart_multipart_data,
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, Photo]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Photo.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.CONFLICT:
-        response_409 = cast(Any, None)
-        return response_409
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, Photo]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
-    ignore_duplicates: Union[Unset, None, bool] = False,
-    compress: Union[Unset, None, bool] = True,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Response[Union[Any, HTTPValidationError, Photo]]:
-    """Photo Upload
-
-     Upload a photo to album
-
-    Args:
-        album (str):
-        ignore_duplicates (Union[Unset, None, bool]):
-        compress (Union[Unset, None, bool]):  Default: True.
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Photo]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        ignore_duplicates=ignore_duplicates,
-        compress=compress,
-        caption=caption,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
-    ignore_duplicates: Union[Unset, None, bool] = False,
-    compress: Union[Unset, None, bool] = True,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[Any, HTTPValidationError, Photo]]:
-    """Photo Upload
-
-     Upload a photo to album
-
-    Args:
-        album (str):
-        ignore_duplicates (Union[Unset, None, bool]):
-        compress (Union[Unset, None, bool]):  Default: True.
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Photo]]
-    """
-
-    return sync_detailed(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        ignore_duplicates=ignore_duplicates,
-        compress=compress,
-        caption=caption,
-    ).parsed
-
-
-async def asyncio_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
-    ignore_duplicates: Union[Unset, None, bool] = False,
-    compress: Union[Unset, None, bool] = True,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Response[Union[Any, HTTPValidationError, Photo]]:
-    """Photo Upload
-
-     Upload a photo to album
-
-    Args:
-        album (str):
-        ignore_duplicates (Union[Unset, None, bool]):
-        compress (Union[Unset, None, bool]):  Default: True.
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Photo]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        ignore_duplicates=ignore_duplicates,
-        compress=compress,
-        caption=caption,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
-    ignore_duplicates: Union[Unset, None, bool] = False,
-    compress: Union[Unset, None, bool] = True,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[Any, HTTPValidationError, Photo]]:
-    """Photo Upload
-
-     Upload a photo to album
-
-    Args:
-        album (str):
-        ignore_duplicates (Union[Unset, None, bool]):
-        compress (Union[Unset, None, bool]):  Default: True.
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Photo]]
-    """
-
-    return (
-        await asyncio_detailed(
-            album=album,
-            client=client,
-            multipart_data=multipart_data,
-            ignore_duplicates=ignore_duplicates,
-            compress=compress,
-            caption=caption,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.body_photo_upload_albums_album_photos_post import BodyPhotoUploadAlbumsAlbumPhotosPost
+from ...models.http_validation_error import HTTPValidationError
+from ...models.photo import Photo
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
+    ignore_duplicates: Union[Unset, None, bool] = False,
+    compress: Union[Unset, None, bool] = True,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Dict[str, Any]:
+    url = "{}/albums/{album}/photos".format(client.base_url, album=album)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["ignore_duplicates"] = ignore_duplicates
+
+    params["compress"] = compress
+
+    params["caption"] = caption
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    multipart_multipart_data = multipart_data.to_multipart()
+
+    return {
+        "method": "post",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "files": multipart_multipart_data,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, Photo]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Photo.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.CONFLICT:
+        response_409 = cast(Any, None)
+        return response_409
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, Photo]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
+    ignore_duplicates: Union[Unset, None, bool] = False,
+    compress: Union[Unset, None, bool] = True,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError, Photo]]:
+    """Photo Upload
+
+     Upload a photo to album
+
+    Args:
+        album (str):
+        ignore_duplicates (Union[Unset, None, bool]):
+        compress (Union[Unset, None, bool]):  Default: True.
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, Photo]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        ignore_duplicates=ignore_duplicates,
+        compress=compress,
+        caption=caption,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
+    ignore_duplicates: Union[Unset, None, bool] = False,
+    compress: Union[Unset, None, bool] = True,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError, Photo]]:
+    """Photo Upload
+
+     Upload a photo to album
+
+    Args:
+        album (str):
+        ignore_duplicates (Union[Unset, None, bool]):
+        compress (Union[Unset, None, bool]):  Default: True.
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, Photo]
+    """
+
+    return sync_detailed(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        ignore_duplicates=ignore_duplicates,
+        compress=compress,
+        caption=caption,
+    ).parsed
+
+
+async def asyncio_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
+    ignore_duplicates: Union[Unset, None, bool] = False,
+    compress: Union[Unset, None, bool] = True,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError, Photo]]:
+    """Photo Upload
+
+     Upload a photo to album
+
+    Args:
+        album (str):
+        ignore_duplicates (Union[Unset, None, bool]):
+        compress (Union[Unset, None, bool]):  Default: True.
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, Photo]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        ignore_duplicates=ignore_duplicates,
+        compress=compress,
+        caption=caption,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyPhotoUploadAlbumsAlbumPhotosPost,
+    ignore_duplicates: Union[Unset, None, bool] = False,
+    compress: Union[Unset, None, bool] = True,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError, Photo]]:
+    """Photo Upload
+
+     Upload a photo to album
+
+    Args:
+        album (str):
+        ignore_duplicates (Union[Unset, None, bool]):
+        compress (Union[Unset, None, bool]):  Default: True.
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyPhotoUploadAlbumsAlbumPhotosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, Photo]
+    """
+
+    return (
+        await asyncio_detailed(
+            album=album,
+            client=client,
+            multipart_data=multipart_data,
+            ignore_duplicates=ignore_duplicates,
+            compress=compress,
+            caption=caption,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,184 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Dict[str, Any]:
-    url = "{}/users/{user}/confirm".format(client.base_url, user=user)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["code"] = code
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = cast(Any, None)
-        return response_400
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        user=user,
-        client=client,
-        code=code,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        user=user,
-        client=client,
-        code=code,
-    ).parsed
-
-
-async def asyncio_detailed(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        user=user,
-        client=client,
-        code=code,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            user=user,
-            client=client,
-            code=code,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Dict[str, Any]:
+    url = "{}/users/{user}/confirm".format(client.base_url, user=user)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["code"] = code
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "patch",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = cast(Any, response.json())
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = cast(Any, None)
+        return response_400
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        user=user,
+        client=client,
+        code=code,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        user=user,
+        client=client,
+        code=code,
+    ).parsed
+
+
+async def asyncio_detailed(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        user=user,
+        client=client,
+        code=code,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            user=user,
+            client=client,
+            code=code,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_confirm_users_user_confirm_patch.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/user_confirm_users_user_confirm_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,183 +1,184 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Dict[str, Any]:
-    url = "{}/users/{user}/confirm".format(client.base_url, user=user)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["code"] = code
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "patch",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = cast(Any, None)
-        return response_400
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        user=user,
-        client=client,
-        code=code,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        user=user,
-        client=client,
-        code=code,
-    ).parsed
-
-
-async def asyncio_detailed(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        user=user,
-        client=client,
-        code=code,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    user: str,
-    *,
-    client: Client,
-    code: str,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Confirm
-
-    Args:
-        user (str):
-        code (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            user=user,
-            client=client,
-            code=code,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Dict[str, Any]:
+    url = "{}/users/{user}/confirm".format(client.base_url, user=user)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["code"] = code
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = cast(Any, response.json())
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = cast(Any, None)
+        return response_400
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        user=user,
+        client=client,
+        code=code,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        user=user,
+        client=client,
+        code=code,
+    ).parsed
+
+
+async def asyncio_detailed(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        user=user,
+        client=client,
+        code=code,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    user: str,
+    *,
+    client: Client,
+    code: str,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """User Confirm
+
+    Args:
+        user (str):
+        code (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            user=user,
+            client=client,
+            code=code,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/user_delete_users_me_delete.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_delete_videos_id_delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,173 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.body_user_delete_users_me_delete import BodyUserDeleteUsersMeDelete
-from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    form_data: BodyUserDeleteUsersMeDelete,
-) -> Dict[str, Any]:
-    url = "{}/users/me/".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "data": form_data.to_dict(),
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
-        return response_401
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    form_data: BodyUserDeleteUsersMeDelete,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Delete
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        form_data=form_data,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    form_data: BodyUserDeleteUsersMeDelete,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Delete
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        client=client,
-        form_data=form_data,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    form_data: BodyUserDeleteUsersMeDelete,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """User Delete
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        form_data=form_data,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    form_data: BodyUserDeleteUsersMeDelete,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """User Delete
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            form_data=form_data,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Dict[str, Any]:
+    url = "{}/videos/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Video Delete
+
+     Delete a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Video Delete
+
+     Delete a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Video Delete
+
+     Delete a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Video Delete
+
+     Delete a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_get_videos_id_get.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_get_videos_id_get.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,172 +1,175 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
-
-
-def _get_kwargs(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Dict[str, Any]:
-    url = "{}/videos/{id}".format(client.base_url, id=id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Video Get
-
-     Get a video by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Video Get
-
-     Get a video by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return sync_detailed(
-        id=id,
-        client=client,
-    ).parsed
-
-
-async def asyncio_detailed(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Video Get
-
-     Get a video by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    kwargs = _get_kwargs(
-        id=id,
-        client=client,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    id: str,
-    *,
-    client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Video Get
-
-     Get a video by id
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError]]
-    """
-
-    return (
-        await asyncio_detailed(
-            id=id,
-            client=client,
-        )
-    ).parsed
+from http import HTTPStatus
+from io import BytesIO
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.http_validation_error import HTTPValidationError
+from ...types import File, Response
+
+
+def _get_kwargs(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Dict[str, Any]:
+    url = "{}/videos/{id}".format(client.base_url, id=id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, File, HTTPValidationError]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = File(payload=BytesIO(response.content))
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, File, HTTPValidationError]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, File, HTTPValidationError]]:
+    """Video Get
+
+     Get a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, File, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, File, HTTPValidationError]]:
+    """Video Get
+
+     Get a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, File, HTTPValidationError]
+    """
+
+    return sync_detailed(
+        id=id,
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Response[Union[Any, File, HTTPValidationError]]:
+    """Video Get
+
+     Get a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, File, HTTPValidationError]]
+    """
+
+    kwargs = _get_kwargs(
+        id=id,
+        client=client,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    id: str,
+    *,
+    client: AuthenticatedClient,
+) -> Optional[Union[Any, File, HTTPValidationError]]:
+    """Video Get
+
+     Get a video by id
+
+    Args:
+        id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, File, HTTPValidationError]
+    """
+
+    return (
+        await asyncio_detailed(
+            id=id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/api/default/video_upload_albums_album_videos_post.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,211 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.body_video_upload_albums_album_videos_post import BodyVideoUploadAlbumsAlbumVideosPost
-from ...models.http_validation_error import HTTPValidationError
-from ...models.video import Video
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Dict[str, Any]:
-    url = "{}/albums/{album}/videos".format(client.base_url, album=album)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["caption"] = caption
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    multipart_multipart_data = multipart_data.to_multipart()
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "files": multipart_multipart_data,
-        "params": params,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, Video]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Video.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
-    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        response_422 = HTTPValidationError.from_dict(response.json())
-
-        return response_422
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(f"Unexpected status code: {response.status_code}")
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, Video]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Response[Union[Any, HTTPValidationError, Video]]:
-    """Video Upload
-
-     Upload a video to album
-
-    Args:
-        album (str):
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Video]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        caption=caption,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[Any, HTTPValidationError, Video]]:
-    """Video Upload
-
-     Upload a video to album
-
-    Args:
-        album (str):
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Video]]
-    """
-
-    return sync_detailed(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        caption=caption,
-    ).parsed
-
-
-async def asyncio_detailed(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Response[Union[Any, HTTPValidationError, Video]]:
-    """Video Upload
-
-     Upload a video to album
-
-    Args:
-        album (str):
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Video]]
-    """
-
-    kwargs = _get_kwargs(
-        album=album,
-        client=client,
-        multipart_data=multipart_data,
-        caption=caption,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    album: str,
-    *,
-    client: AuthenticatedClient,
-    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
-    caption: Union[Unset, None, str] = UNSET,
-) -> Optional[Union[Any, HTTPValidationError, Video]]:
-    """Video Upload
-
-     Upload a video to album
-
-    Args:
-        album (str):
-        caption (Union[Unset, None, str]):
-        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, Video]]
-    """
-
-    return (
-        await asyncio_detailed(
-            album=album,
-            client=client,
-            multipart_data=multipart_data,
-            caption=caption,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.body_video_upload_albums_album_videos_post import BodyVideoUploadAlbumsAlbumVideosPost
+from ...models.http_validation_error import HTTPValidationError
+from ...models.video import Video
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Dict[str, Any]:
+    url = "{}/albums/{album}/videos".format(client.base_url, album=album)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["caption"] = caption
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    multipart_multipart_data = multipart_data.to_multipart()
+
+    return {
+        "method": "post",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "files": multipart_multipart_data,
+        "params": params,
+    }
+
+
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, Video]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = Video.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = cast(Any, None)
+        return response_404
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = HTTPValidationError.from_dict(response.json())
+
+        return response_422
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, Video]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError, Video]]:
+    """Video Upload
+
+     Upload a video to album
+
+    Args:
+        album (str):
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, Video]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        caption=caption,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError, Video]]:
+    """Video Upload
+
+     Upload a video to album
+
+    Args:
+        album (str):
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, Video]
+    """
+
+    return sync_detailed(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        caption=caption,
+    ).parsed
+
+
+async def asyncio_detailed(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError, Video]]:
+    """Video Upload
+
+     Upload a video to album
+
+    Args:
+        album (str):
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, Video]]
+    """
+
+    kwargs = _get_kwargs(
+        album=album,
+        client=client,
+        multipart_data=multipart_data,
+        caption=caption,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    album: str,
+    *,
+    client: AuthenticatedClient,
+    multipart_data: BodyVideoUploadAlbumsAlbumVideosPost,
+    caption: Union[Unset, None, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError, Video]]:
+    """Video Upload
+
+     Upload a video to album
+
+    Args:
+        album (str):
+        caption (Union[Unset, None, str]):
+        multipart_data (BodyVideoUploadAlbumsAlbumVideosPost):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[Any, HTTPValidationError, Video]
+    """
+
+    return (
+        await asyncio_detailed(
+            album=album,
+            client=client,
+            multipart_data=multipart_data,
+            caption=caption,
+        )
+    ).parsed
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/client.py` & `PhotosAPI_Client-0.4.0/photosapi_client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-import ssl
-from typing import Dict, Union
-
-import attr
-
-
-@attr.s(auto_attribs=True)
-class Client:
-    """A class for keeping track of data related to the API
-
-    Attributes:
-        base_url: The base URL for the API, all requests are made to a relative path to this URL
-        cookies: A dictionary of cookies to be sent with every request
-        headers: A dictionary of headers to be sent with every request
-        timeout: The maximum amount of a time in seconds a request can take. API functions will raise
-            httpx.TimeoutException if this is exceeded.
-        verify_ssl: Whether or not to verify the SSL certificate of the API server. This should be True in production,
-            but can be set to False for testing purposes.
-        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
-            status code that was not documented in the source OpenAPI document.
-    """
-
-    base_url: str
-    cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    timeout: float = attr.ib(5.0, kw_only=True)
-    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
-    raise_on_unexpected_status: bool = attr.ib(False, kw_only=True)
-
-    def get_headers(self) -> Dict[str, str]:
-        """Get headers to be used in all endpoints"""
-        return {**self.headers}
-
-    def with_headers(self, headers: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional headers"""
-        return attr.evolve(self, headers={**self.headers, **headers})
-
-    def get_cookies(self) -> Dict[str, str]:
-        return {**self.cookies}
-
-    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional cookies"""
-        return attr.evolve(self, cookies={**self.cookies, **cookies})
-
-    def get_timeout(self) -> float:
-        return self.timeout
-
-    def with_timeout(self, timeout: float) -> "Client":
-        """Get a new client matching this one with a new timeout (in seconds)"""
-        return attr.evolve(self, timeout=timeout)
-
-
-@attr.s(auto_attribs=True)
-class AuthenticatedClient(Client):
-    """A Client which has been authenticated for use on secured endpoints"""
-
-    token: str
-    prefix: str = "Bearer"
-    auth_header_name: str = "Authorization"
-
-    def get_headers(self) -> Dict[str, str]:
-        """Get headers to be used in authenticated endpoints"""
-        auth_header_value = f"{self.prefix} {self.token}" if self.prefix else self.token
-        return {self.auth_header_name: auth_header_value, **self.headers}
+import ssl
+from typing import Dict, Union
+
+import attr
+
+
+@attr.s(auto_attribs=True)
+class Client:
+    """A class for keeping track of data related to the API
+
+    Attributes:
+        base_url: The base URL for the API, all requests are made to a relative path to this URL
+        cookies: A dictionary of cookies to be sent with every request
+        headers: A dictionary of headers to be sent with every request
+        timeout: The maximum amount of a time in seconds a request can take. API functions will raise
+            httpx.TimeoutException if this is exceeded.
+        verify_ssl: Whether or not to verify the SSL certificate of the API server. This should be True in production,
+            but can be set to False for testing purposes.
+        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
+            status code that was not documented in the source OpenAPI document.
+        follow_redirects: Whether or not to follow redirects. Default value is False.
+    """
+
+    base_url: str
+    cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
+    headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
+    timeout: float = attr.ib(5.0, kw_only=True)
+    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
+    raise_on_unexpected_status: bool = attr.ib(False, kw_only=True)
+    follow_redirects: bool = attr.ib(False, kw_only=True)
+
+    def get_headers(self) -> Dict[str, str]:
+        """Get headers to be used in all endpoints"""
+        return {**self.headers}
+
+    def with_headers(self, headers: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional headers"""
+        return attr.evolve(self, headers={**self.headers, **headers})
+
+    def get_cookies(self) -> Dict[str, str]:
+        return {**self.cookies}
+
+    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional cookies"""
+        return attr.evolve(self, cookies={**self.cookies, **cookies})
+
+    def get_timeout(self) -> float:
+        return self.timeout
+
+    def with_timeout(self, timeout: float) -> "Client":
+        """Get a new client matching this one with a new timeout (in seconds)"""
+        return attr.evolve(self, timeout=timeout)
+
+
+@attr.s(auto_attribs=True)
+class AuthenticatedClient(Client):
+    """A Client which has been authenticated for use on secured endpoints"""
+
+    token: str
+    prefix: str = "Bearer"
+    auth_header_name: str = "Authorization"
+
+    def get_headers(self) -> Dict[str, str]:
+        """Get headers to be used in authenticated endpoints"""
+        auth_header_value = f"{self.prefix} {self.token}" if self.prefix else self.token
+        return {self.auth_header_name: auth_header_value, **self.headers}
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/__init__.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-""" Contains all the data models used in inputs/outputs """
-
-from .album import Album
-from .album_modified import AlbumModified
-from .body_login_for_access_token_token_post import BodyLoginForAccessTokenTokenPost
-from .body_photo_upload_albums_album_photos_post import BodyPhotoUploadAlbumsAlbumPhotosPost
-from .body_user_create_users_post import BodyUserCreateUsersPost
-from .body_user_delete_users_me_delete import BodyUserDeleteUsersMeDelete
-from .body_video_upload_albums_album_videos_post import BodyVideoUploadAlbumsAlbumVideosPost
-from .http_validation_error import HTTPValidationError
-from .photo import Photo
-from .photo_public import PhotoPublic
-from .photo_search import PhotoSearch
-from .search_results_album import SearchResultsAlbum
-from .search_results_photo import SearchResultsPhoto
-from .search_results_video import SearchResultsVideo
-from .token import Token
-from .user import User
-from .validation_error import ValidationError
-from .video import Video
-from .video_public import VideoPublic
-from .video_search import VideoSearch
-
-__all__ = (
-    "Album",
-    "AlbumModified",
-    "BodyLoginForAccessTokenTokenPost",
-    "BodyPhotoUploadAlbumsAlbumPhotosPost",
-    "BodyUserCreateUsersPost",
-    "BodyUserDeleteUsersMeDelete",
-    "BodyVideoUploadAlbumsAlbumVideosPost",
-    "HTTPValidationError",
-    "Photo",
-    "PhotoPublic",
-    "PhotoSearch",
-    "SearchResultsAlbum",
-    "SearchResultsPhoto",
-    "SearchResultsVideo",
-    "Token",
-    "User",
-    "ValidationError",
-    "Video",
-    "VideoPublic",
-    "VideoSearch",
-)
+""" Contains all the data models used in inputs/outputs """
+
+from .album import Album
+from .album_modified import AlbumModified
+from .body_login_for_access_token_token_post import BodyLoginForAccessTokenTokenPost
+from .body_photo_upload_albums_album_photos_post import BodyPhotoUploadAlbumsAlbumPhotosPost
+from .body_user_create_users_post import BodyUserCreateUsersPost
+from .body_user_delete_users_me_delete import BodyUserDeleteUsersMeDelete
+from .body_video_upload_albums_album_videos_post import BodyVideoUploadAlbumsAlbumVideosPost
+from .http_validation_error import HTTPValidationError
+from .photo import Photo
+from .photo_public import PhotoPublic
+from .photo_search import PhotoSearch
+from .search_results_album import SearchResultsAlbum
+from .search_results_photo import SearchResultsPhoto
+from .search_results_video import SearchResultsVideo
+from .token import Token
+from .user import User
+from .validation_error import ValidationError
+from .video import Video
+from .video_public import VideoPublic
+from .video_search import VideoSearch
+
+__all__ = (
+    "Album",
+    "AlbumModified",
+    "BodyLoginForAccessTokenTokenPost",
+    "BodyPhotoUploadAlbumsAlbumPhotosPost",
+    "BodyUserCreateUsersPost",
+    "BodyUserDeleteUsersMeDelete",
+    "BodyVideoUploadAlbumsAlbumVideosPost",
+    "HTTPValidationError",
+    "Photo",
+    "PhotoPublic",
+    "PhotoSearch",
+    "SearchResultsAlbum",
+    "SearchResultsPhoto",
+    "SearchResultsVideo",
+    "Token",
+    "User",
+    "ValidationError",
+    "Video",
+    "VideoPublic",
+    "VideoSearch",
+)
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/album.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/album.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="Album")
-
-
-@attr.s(auto_attribs=True)
-class Album:
-    """
-    Attributes:
-        id (str):
-        name (str):
-        title (str):
-    """
-
-    id: str
-    name: str
-    title: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
-        title = self.title
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "name": name,
-                "title": title,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        name = d.pop("name")
-
-        title = d.pop("title")
-
-        album = cls(
-            id=id,
-            name=name,
-            title=title,
-        )
-
-        album.additional_properties = d
-        return album
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="Album")
+
+
+@attr.s(auto_attribs=True)
+class Album:
+    """
+    Attributes:
+        id (str):
+        name (str):
+        title (str):
+    """
+
+    id: str
+    name: str
+    title: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        name = self.name
+        title = self.title
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "name": name,
+                "title": title,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        name = d.pop("name")
+
+        title = d.pop("title")
+
+        album = cls(
+            id=id,
+            name=name,
+            title=title,
+        )
+
+        album.additional_properties = d
+        return album
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/album_modified.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/album_modified.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="AlbumModified")
-
-
-@attr.s(auto_attribs=True)
-class AlbumModified:
-    """
-    Attributes:
-        name (str):
-        title (str):
-        cover (Union[Unset, str]):
-    """
-
-    name: str
-    title: str
-    cover: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        title = self.title
-        cover = self.cover
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "name": name,
-                "title": title,
-            }
-        )
-        if cover is not UNSET:
-            field_dict["cover"] = cover
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name")
-
-        title = d.pop("title")
-
-        cover = d.pop("cover", UNSET)
-
-        album_modified = cls(
-            name=name,
-            title=title,
-            cover=cover,
-        )
-
-        album_modified.additional_properties = d
-        return album_modified
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="AlbumModified")
+
+
+@attr.s(auto_attribs=True)
+class AlbumModified:
+    """
+    Attributes:
+        name (str):
+        title (str):
+        cover (Union[Unset, str]):
+    """
+
+    name: str
+    title: str
+    cover: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+        title = self.title
+        cover = self.cover
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "name": name,
+                "title": title,
+            }
+        )
+        if cover is not UNSET:
+            field_dict["cover"] = cover
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        name = d.pop("name")
+
+        title = d.pop("title")
+
+        cover = d.pop("cover", UNSET)
+
+        album_modified = cls(
+            name=name,
+            title=title,
+            cover=cover,
+        )
+
+        album_modified.additional_properties = d
+        return album_modified
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/body_login_for_access_token_token_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/body_login_for_access_token_token_post.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="BodyLoginForAccessTokenTokenPost")
-
-
-@attr.s(auto_attribs=True)
-class BodyLoginForAccessTokenTokenPost:
-    """
-    Attributes:
-        username (str):
-        password (str):
-        grant_type (Union[Unset, str]):
-        scope (Union[Unset, str]):  Default: ''.
-        client_id (Union[Unset, str]):
-        client_secret (Union[Unset, str]):
-    """
-
-    username: str
-    password: str
-    grant_type: Union[Unset, str] = UNSET
-    scope: Union[Unset, str] = ""
-    client_id: Union[Unset, str] = UNSET
-    client_secret: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        username = self.username
-        password = self.password
-        grant_type = self.grant_type
-        scope = self.scope
-        client_id = self.client_id
-        client_secret = self.client_secret
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "username": username,
-                "password": password,
-            }
-        )
-        if grant_type is not UNSET:
-            field_dict["grant_type"] = grant_type
-        if scope is not UNSET:
-            field_dict["scope"] = scope
-        if client_id is not UNSET:
-            field_dict["client_id"] = client_id
-        if client_secret is not UNSET:
-            field_dict["client_secret"] = client_secret
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        username = d.pop("username")
-
-        password = d.pop("password")
-
-        grant_type = d.pop("grant_type", UNSET)
-
-        scope = d.pop("scope", UNSET)
-
-        client_id = d.pop("client_id", UNSET)
-
-        client_secret = d.pop("client_secret", UNSET)
-
-        body_login_for_access_token_token_post = cls(
-            username=username,
-            password=password,
-            grant_type=grant_type,
-            scope=scope,
-            client_id=client_id,
-            client_secret=client_secret,
-        )
-
-        body_login_for_access_token_token_post.additional_properties = d
-        return body_login_for_access_token_token_post
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="BodyLoginForAccessTokenTokenPost")
+
+
+@attr.s(auto_attribs=True)
+class BodyLoginForAccessTokenTokenPost:
+    """
+    Attributes:
+        username (str):
+        password (str):
+        grant_type (Union[Unset, str]):
+        scope (Union[Unset, str]):  Default: ''.
+        client_id (Union[Unset, str]):
+        client_secret (Union[Unset, str]):
+    """
+
+    username: str
+    password: str
+    grant_type: Union[Unset, str] = UNSET
+    scope: Union[Unset, str] = ""
+    client_id: Union[Unset, str] = UNSET
+    client_secret: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        username = self.username
+        password = self.password
+        grant_type = self.grant_type
+        scope = self.scope
+        client_id = self.client_id
+        client_secret = self.client_secret
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "username": username,
+                "password": password,
+            }
+        )
+        if grant_type is not UNSET:
+            field_dict["grant_type"] = grant_type
+        if scope is not UNSET:
+            field_dict["scope"] = scope
+        if client_id is not UNSET:
+            field_dict["client_id"] = client_id
+        if client_secret is not UNSET:
+            field_dict["client_secret"] = client_secret
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        username = d.pop("username")
+
+        password = d.pop("password")
+
+        grant_type = d.pop("grant_type", UNSET)
+
+        scope = d.pop("scope", UNSET)
+
+        client_id = d.pop("client_id", UNSET)
+
+        client_secret = d.pop("client_secret", UNSET)
+
+        body_login_for_access_token_token_post = cls(
+            username=username,
+            password=password,
+            grant_type=grant_type,
+            scope=scope,
+            client_id=client_id,
+            client_secret=client_secret,
+        )
+
+        body_login_for_access_token_token_post.additional_properties = d
+        return body_login_for_access_token_token_post
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/body_photo_upload_albums_album_photos_post.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from io import BytesIO
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from ..types import File
-
-T = TypeVar("T", bound="BodyPhotoUploadAlbumsAlbumPhotosPost")
-
-
-@attr.s(auto_attribs=True)
-class BodyPhotoUploadAlbumsAlbumPhotosPost:
-    """
-    Attributes:
-        file (File):
-    """
-
-    file: File
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        file = self.file.to_tuple()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "file": file,
-            }
-        )
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        file = self.file.to_tuple()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "file": file,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        file = File(payload=BytesIO(d.pop("file")))
-
-        body_photo_upload_albums_album_photos_post = cls(
-            file=file,
-        )
-
-        body_photo_upload_albums_album_photos_post.additional_properties = d
-        return body_photo_upload_albums_album_photos_post
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from io import BytesIO
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from ..types import File
+
+T = TypeVar("T", bound="BodyPhotoUploadAlbumsAlbumPhotosPost")
+
+
+@attr.s(auto_attribs=True)
+class BodyPhotoUploadAlbumsAlbumPhotosPost:
+    """
+    Attributes:
+        file (File):
+    """
+
+    file: File
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        file = self.file.to_tuple()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "file": file,
+            }
+        )
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        file = self.file.to_tuple()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update(
+            {
+                "file": file,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        file = File(payload=BytesIO(d.pop("file")))
+
+        body_photo_upload_albums_album_photos_post = cls(
+            file=file,
+        )
+
+        body_photo_upload_albums_album_photos_post.additional_properties = d
+        return body_photo_upload_albums_album_photos_post
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/body_user_delete_users_me_delete.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/validation_error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,87 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="BodyUserDeleteUsersMeDelete")
-
-
-@attr.s(auto_attribs=True)
-class BodyUserDeleteUsersMeDelete:
-    """
-    Attributes:
-        password (str):
-    """
-
-    password: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        password = self.password
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "password": password,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        password = d.pop("password")
-
-        body_user_delete_users_me_delete = cls(
-            password=password,
-        )
-
-        body_user_delete_users_me_delete.additional_properties = d
-        return body_user_delete_users_me_delete
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+T = TypeVar("T", bound="ValidationError")
+
+
+@attr.s(auto_attribs=True)
+class ValidationError:
+    """
+    Attributes:
+        loc (List[Union[int, str]]):
+        msg (str):
+        type (str):
+    """
+
+    loc: List[Union[int, str]]
+    msg: str
+    type: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        loc = []
+        for loc_item_data in self.loc:
+            loc_item: Union[int, str]
+
+            loc_item = loc_item_data
+
+            loc.append(loc_item)
+
+        msg = self.msg
+        type = self.type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "loc": loc,
+                "msg": msg,
+                "type": type,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        loc = []
+        _loc = d.pop("loc")
+        for loc_item_data in _loc:
+
+            def _parse_loc_item(data: object) -> Union[int, str]:
+                return cast(Union[int, str], data)
+
+            loc_item = _parse_loc_item(loc_item_data)
+
+            loc.append(loc_item)
+
+        msg = d.pop("msg")
+
+        type = d.pop("type")
+
+        validation_error = cls(
+            loc=loc,
+            msg=msg,
+            type=type,
+        )
+
+        validation_error.additional_properties = d
+        return validation_error
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_photo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,83 @@
-from io import BytesIO
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from ..types import File
-
-T = TypeVar("T", bound="BodyVideoUploadAlbumsAlbumVideosPost")
-
-
-@attr.s(auto_attribs=True)
-class BodyVideoUploadAlbumsAlbumVideosPost:
-    """
-    Attributes:
-        file (File):
-    """
-
-    file: File
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        file = self.file.to_tuple()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "file": file,
-            }
-        )
-
-        return field_dict
-
-    def to_multipart(self) -> Dict[str, Any]:
-        file = self.file.to_tuple()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
-        )
-        field_dict.update(
-            {
-                "file": file,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        file = File(payload=BytesIO(d.pop("file")))
-
-        body_video_upload_albums_album_videos_post = cls(
-            file=file,
-        )
-
-        body_video_upload_albums_album_videos_post.additional_properties = d
-        return body_video_upload_albums_album_videos_post
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.photo_search import PhotoSearch
+
+
+T = TypeVar("T", bound="SearchResultsPhoto")
+
+
+@attr.s(auto_attribs=True)
+class SearchResultsPhoto:
+    """
+    Attributes:
+        results (List['PhotoSearch']):
+        next_page (Union[Unset, str]):
+    """
+
+    results: List["PhotoSearch"]
+    next_page: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
+        next_page = self.next_page
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "results": results,
+            }
+        )
+        if next_page is not UNSET:
+            field_dict["next_page"] = next_page
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.photo_search import PhotoSearch
+
+        d = src_dict.copy()
+        results = []
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = PhotoSearch.from_dict(results_item_data)
+
+            results.append(results_item)
+
+        next_page = d.pop("next_page", UNSET)
+
+        search_results_photo = cls(
+            results=results,
+            next_page=next_page,
+        )
+
+        search_results_photo.additional_properties = d
+        return search_results_photo
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/photo.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/photo_public.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,71 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="Photo")
-
-
-@attr.s(auto_attribs=True)
-class Photo:
-    """
-    Attributes:
-        id (str):
-        album (str):
-        hash_ (str):
-        filename (str):
-    """
-
-    id: str
-    album: str
-    hash_: str
-    filename: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        album = self.album
-        hash_ = self.hash_
-        filename = self.filename
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "album": album,
-                "hash": hash_,
-                "filename": filename,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        album = d.pop("album")
-
-        hash_ = d.pop("hash")
-
-        filename = d.pop("filename")
-
-        photo = cls(
-            id=id,
-            album=album,
-            hash_=hash_,
-            filename=filename,
-        )
-
-        photo.additional_properties = d
-        return photo
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="PhotoPublic")
+
+
+@attr.s(auto_attribs=True)
+class PhotoPublic:
+    """
+    Attributes:
+        id (str):
+        caption (str):
+        filename (str):
+    """
+
+    id: str
+    caption: str
+    filename: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        caption = self.caption
+        filename = self.filename
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "caption": caption,
+                "filename": filename,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        caption = d.pop("caption")
+
+        filename = d.pop("filename")
+
+        photo_public = cls(
+            id=id,
+            caption=caption,
+            filename=filename,
+        )
+
+        photo_public.additional_properties = d
+        return photo_public
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/photo_public.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/video_public.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="PhotoPublic")
-
-
-@attr.s(auto_attribs=True)
-class PhotoPublic:
-    """
-    Attributes:
-        id (str):
-        caption (str):
-        filename (str):
-    """
-
-    id: str
-    caption: str
-    filename: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        caption = self.caption
-        filename = self.filename
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "caption": caption,
-                "filename": filename,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        caption = d.pop("caption")
-
-        filename = d.pop("filename")
-
-        photo_public = cls(
-            id=id,
-            caption=caption,
-            filename=filename,
-        )
-
-        photo_public.additional_properties = d
-        return photo_public
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="VideoPublic")
+
+
+@attr.s(auto_attribs=True)
+class VideoPublic:
+    """
+    Attributes:
+        id (str):
+        caption (str):
+        filename (str):
+    """
+
+    id: str
+    caption: str
+    filename: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        caption = self.caption
+        filename = self.filename
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "caption": caption,
+                "filename": filename,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        caption = d.pop("caption")
+
+        filename = d.pop("filename")
+
+        video_public = cls(
+            id=id,
+            caption=caption,
+            filename=filename,
+        )
+
+        video_public.additional_properties = d
+        return video_public
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_album.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_video.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.album import Album
-
-
-T = TypeVar("T", bound="SearchResultsAlbum")
-
-
-@attr.s(auto_attribs=True)
-class SearchResultsAlbum:
-    """
-    Attributes:
-        results (List['Album']):
-        next_page (Union[Unset, str]):
-    """
-
-    results: List["Album"]
-    next_page: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        next_page = self.next_page
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "results": results,
-            }
-        )
-        if next_page is not UNSET:
-            field_dict["next_page"] = next_page
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.album import Album
-
-        d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = Album.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        next_page = d.pop("next_page", UNSET)
-
-        search_results_album = cls(
-            results=results,
-            next_page=next_page,
-        )
-
-        search_results_album.additional_properties = d
-        return search_results_album
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.video_search import VideoSearch
+
+
+T = TypeVar("T", bound="SearchResultsVideo")
+
+
+@attr.s(auto_attribs=True)
+class SearchResultsVideo:
+    """
+    Attributes:
+        results (List['VideoSearch']):
+        next_page (Union[Unset, str]):
+    """
+
+    results: List["VideoSearch"]
+    next_page: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
+        next_page = self.next_page
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "results": results,
+            }
+        )
+        if next_page is not UNSET:
+            field_dict["next_page"] = next_page
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.video_search import VideoSearch
+
+        d = src_dict.copy()
+        results = []
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = VideoSearch.from_dict(results_item_data)
+
+            results.append(results_item)
+
+        next_page = d.pop("next_page", UNSET)
+
+        search_results_video = cls(
+            results=results,
+            next_page=next_page,
+        )
+
+        search_results_video.additional_properties = d
+        return search_results_video
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_photo.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/search_results_album.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.photo_search import PhotoSearch
-
-
-T = TypeVar("T", bound="SearchResultsPhoto")
-
-
-@attr.s(auto_attribs=True)
-class SearchResultsPhoto:
-    """
-    Attributes:
-        results (List['PhotoSearch']):
-        next_page (Union[Unset, str]):
-    """
-
-    results: List["PhotoSearch"]
-    next_page: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        next_page = self.next_page
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "results": results,
-            }
-        )
-        if next_page is not UNSET:
-            field_dict["next_page"] = next_page
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.photo_search import PhotoSearch
-
-        d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = PhotoSearch.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        next_page = d.pop("next_page", UNSET)
-
-        search_results_photo = cls(
-            results=results,
-            next_page=next_page,
-        )
-
-        search_results_photo.additional_properties = d
-        return search_results_photo
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.album import Album
+
+
+T = TypeVar("T", bound="SearchResultsAlbum")
+
+
+@attr.s(auto_attribs=True)
+class SearchResultsAlbum:
+    """
+    Attributes:
+        results (List['Album']):
+        next_page (Union[Unset, str]):
+    """
+
+    results: List["Album"]
+    next_page: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
+        next_page = self.next_page
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "results": results,
+            }
+        )
+        if next_page is not UNSET:
+            field_dict["next_page"] = next_page
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.album import Album
+
+        d = src_dict.copy()
+        results = []
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Album.from_dict(results_item_data)
+
+            results.append(results_item)
+
+        next_page = d.pop("next_page", UNSET)
+
+        search_results_album = cls(
+            results=results,
+            next_page=next_page,
+        )
+
+        search_results_album.additional_properties = d
+        return search_results_album
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/search_results_video.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/video.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,78 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.video_search import VideoSearch
-
-
-T = TypeVar("T", bound="SearchResultsVideo")
-
-
-@attr.s(auto_attribs=True)
-class SearchResultsVideo:
-    """
-    Attributes:
-        results (List['VideoSearch']):
-        next_page (Union[Unset, str]):
-    """
-
-    results: List["VideoSearch"]
-    next_page: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        next_page = self.next_page
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "results": results,
-            }
-        )
-        if next_page is not UNSET:
-            field_dict["next_page"] = next_page
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.video_search import VideoSearch
-
-        d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = VideoSearch.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        next_page = d.pop("next_page", UNSET)
-
-        search_results_video = cls(
-            results=results,
-            next_page=next_page,
-        )
-
-        search_results_video.additional_properties = d
-        return search_results_video
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="Video")
+
+
+@attr.s(auto_attribs=True)
+class Video:
+    """
+    Attributes:
+        id (str):
+        album (str):
+        hash_ (str):
+        filename (str):
+    """
+
+    id: str
+    album: str
+    hash_: str
+    filename: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        album = self.album
+        hash_ = self.hash_
+        filename = self.filename
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "album": album,
+                "hash": hash_,
+                "filename": filename,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        album = d.pop("album")
+
+        hash_ = d.pop("hash")
+
+        filename = d.pop("filename")
+
+        video = cls(
+            id=id,
+            album=album,
+            hash_=hash_,
+            filename=filename,
+        )
+
+        video.additional_properties = d
+        return video
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/user.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/user.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="User")
-
-
-@attr.s(auto_attribs=True)
-class User:
-    """
-    Attributes:
-        user (str):
-        email (Union[Unset, str]):
-        disabled (Union[Unset, bool]):
-    """
-
-    user: str
-    email: Union[Unset, str] = UNSET
-    disabled: Union[Unset, bool] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        user = self.user
-        email = self.email
-        disabled = self.disabled
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "user": user,
-            }
-        )
-        if email is not UNSET:
-            field_dict["email"] = email
-        if disabled is not UNSET:
-            field_dict["disabled"] = disabled
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        user = d.pop("user")
-
-        email = d.pop("email", UNSET)
-
-        disabled = d.pop("disabled", UNSET)
-
-        user = cls(
-            user=user,
-            email=email,
-            disabled=disabled,
-        )
-
-        user.additional_properties = d
-        return user
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="User")
+
+
+@attr.s(auto_attribs=True)
+class User:
+    """
+    Attributes:
+        user (str):
+        email (Union[Unset, str]):
+        disabled (Union[Unset, bool]):
+    """
+
+    user: str
+    email: Union[Unset, str] = UNSET
+    disabled: Union[Unset, bool] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        user = self.user
+        email = self.email
+        disabled = self.disabled
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "user": user,
+            }
+        )
+        if email is not UNSET:
+            field_dict["email"] = email
+        if disabled is not UNSET:
+            field_dict["disabled"] = disabled
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        user = d.pop("user")
+
+        email = d.pop("email", UNSET)
+
+        disabled = d.pop("disabled", UNSET)
+
+        user = cls(
+            user=user,
+            email=email,
+            disabled=disabled,
+        )
+
+        user.additional_properties = d
+        return user
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/video.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/body_video_upload_albums_album_videos_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,75 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="Video")
-
-
-@attr.s(auto_attribs=True)
-class Video:
-    """
-    Attributes:
-        id (str):
-        album (str):
-        hash_ (str):
-        filename (str):
-    """
-
-    id: str
-    album: str
-    hash_: str
-    filename: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        album = self.album
-        hash_ = self.hash_
-        filename = self.filename
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "album": album,
-                "hash": hash_,
-                "filename": filename,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        album = d.pop("album")
-
-        hash_ = d.pop("hash")
-
-        filename = d.pop("filename")
-
-        video = cls(
-            id=id,
-            album=album,
-            hash_=hash_,
-            filename=filename,
-        )
-
-        video.additional_properties = d
-        return video
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from io import BytesIO
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from ..types import File
+
+T = TypeVar("T", bound="BodyVideoUploadAlbumsAlbumVideosPost")
+
+
+@attr.s(auto_attribs=True)
+class BodyVideoUploadAlbumsAlbumVideosPost:
+    """
+    Attributes:
+        file (File):
+    """
+
+    file: File
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        file = self.file.to_tuple()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "file": file,
+            }
+        )
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        file = self.file.to_tuple()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update(
+            {
+                "file": file,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        file = File(payload=BytesIO(d.pop("file")))
+
+        body_video_upload_albums_album_videos_post = cls(
+            file=file,
+        )
+
+        body_video_upload_albums_album_videos_post.additional_properties = d
+        return body_video_upload_albums_album_videos_post
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/video_public.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/photo_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,74 @@
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="VideoPublic")
-
-
-@attr.s(auto_attribs=True)
-class VideoPublic:
-    """
-    Attributes:
-        id (str):
-        caption (str):
-        filename (str):
-    """
-
-    id: str
-    caption: str
-    filename: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        caption = self.caption
-        filename = self.filename
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "caption": caption,
-                "filename": filename,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        caption = d.pop("caption")
-
-        filename = d.pop("filename")
-
-        video_public = cls(
-            id=id,
-            caption=caption,
-            filename=filename,
-        )
-
-        video_public.additional_properties = d
-        return video_public
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="PhotoSearch")
+
+
+@attr.s(auto_attribs=True)
+class PhotoSearch:
+    """
+    Attributes:
+        id (str):
+        filename (str):
+        caption (Union[Unset, str]):
+    """
+
+    id: str
+    filename: str
+    caption: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        filename = self.filename
+        caption = self.caption
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "filename": filename,
+            }
+        )
+        if caption is not UNSET:
+            field_dict["caption"] = caption
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        filename = d.pop("filename")
+
+        caption = d.pop("caption", UNSET)
+
+        photo_search = cls(
+            id=id,
+            filename=filename,
+            caption=caption,
+        )
+
+        photo_search.additional_properties = d
+        return photo_search
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/models/video_search.py` & `PhotosAPI_Client-0.4.0/photosapi_client/models/video_search.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="VideoSearch")
-
-
-@attr.s(auto_attribs=True)
-class VideoSearch:
-    """
-    Attributes:
-        id (str):
-        filename (str):
-        caption (Union[Unset, str]):
-    """
-
-    id: str
-    filename: str
-    caption: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        filename = self.filename
-        caption = self.caption
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "filename": filename,
-            }
-        )
-        if caption is not UNSET:
-            field_dict["caption"] = caption
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id")
-
-        filename = d.pop("filename")
-
-        caption = d.pop("caption", UNSET)
-
-        video_search = cls(
-            id=id,
-            filename=filename,
-            caption=caption,
-        )
-
-        video_search.additional_properties = d
-        return video_search
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="VideoSearch")
+
+
+@attr.s(auto_attribs=True)
+class VideoSearch:
+    """
+    Attributes:
+        id (str):
+        filename (str):
+        caption (Union[Unset, str]):
+    """
+
+    id: str
+    filename: str
+    caption: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        filename = self.filename
+        caption = self.caption
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "id": id,
+                "filename": filename,
+            }
+        )
+        if caption is not UNSET:
+            field_dict["caption"] = caption
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id")
+
+        filename = d.pop("filename")
+
+        caption = d.pop("caption", UNSET)
+
+        video_search = cls(
+            id=id,
+            filename=filename,
+            caption=caption,
+        )
+
+        video_search.additional_properties = d
+        return video_search
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `PhotosAPI_Client-0.2.0/photosapi_client/types.py` & `PhotosAPI_Client-0.4.0/photosapi_client/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-""" Contains some shared types for properties """
-from http import HTTPStatus
-from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
-
-import attr
-
-
-class Unset:
-    def __bool__(self) -> bool:
-        return False
-
-
-UNSET: Unset = Unset()
-
-FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
-
-
-@attr.s(auto_attribs=True)
-class File:
-    """Contains information for file uploads"""
-
-    payload: BinaryIO
-    file_name: Optional[str] = None
-    mime_type: Optional[str] = None
-
-    def to_tuple(self) -> FileJsonType:
-        """Return a tuple representation that httpx will accept for multipart/form-data"""
-        return self.file_name, self.payload, self.mime_type
-
-
-T = TypeVar("T")
-
-
-@attr.s(auto_attribs=True)
-class Response(Generic[T]):
-    """A response from an endpoint"""
-
-    status_code: HTTPStatus
-    content: bytes
-    headers: MutableMapping[str, str]
-    parsed: Optional[T]
-
-
-__all__ = ["File", "Response", "FileJsonType"]
+""" Contains some shared types for properties """
+from http import HTTPStatus
+from typing import BinaryIO, Generic, Literal, MutableMapping, Optional, Tuple, TypeVar
+
+import attr
+
+
+class Unset:
+    def __bool__(self) -> Literal[False]:
+        return False
+
+
+UNSET: Unset = Unset()
+
+FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
+
+
+@attr.s(auto_attribs=True)
+class File:
+    """Contains information for file uploads"""
+
+    payload: BinaryIO
+    file_name: Optional[str] = None
+    mime_type: Optional[str] = None
+
+    def to_tuple(self) -> FileJsonType:
+        """Return a tuple representation that httpx will accept for multipart/form-data"""
+        return self.file_name, self.payload, self.mime_type
+
+
+T = TypeVar("T")
+
+
+@attr.s(auto_attribs=True)
+class Response(Generic[T]):
+    """A response from an endpoint"""
+
+    status_code: HTTPStatus
+    content: bytes
+    headers: MutableMapping[str, str]
+    parsed: Optional[T]
+
+
+__all__ = ["File", "Response", "FileJsonType"]
```

