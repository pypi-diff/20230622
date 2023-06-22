# Comparing `tmp/iparapheur-provisioning-1.6.8.tar.gz` & `tmp/iparapheur-provisioning-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.6.8.tar", last modified: Tue Jun 20 11:38:13 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.7.0.tar", last modified: Thu Jun 22 14:40:21 2023, max compression
```

## Comparing `iparapheur-provisioning-1.6.8.tar` & `iparapheur-provisioning-1.7.0.tar`

### file list

```diff
@@ -1,241 +1,264 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.223655 iparapheur-provisioning-1.6.8/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-06-20 11:36:57.000000 iparapheur-provisioning-1.6.8/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-20 11:38:13.223655 iparapheur-provisioning-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17323 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.191654 iparapheur-provisioning-1.6.8/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.191654 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.195654 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.195654 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-06-20 11:36:26.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-06-20 11:36:27.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-20 11:36:28.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-06-20 11:36:28.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4891 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    28616 2023-06-20 11:36:33.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     3645 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-06-20 11:36:44.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-06-20 11:36:44.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-06-20 11:36:41.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-06-20 11:36:40.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-20 11:36:40.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-06-20 11:36:41.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-06-20 11:36:40.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.203655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-06-20 11:36:54.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-06-20 11:36:52.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-20 11:36:53.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-06-20 11:36:53.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-06-20 11:36:54.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-06-20 11:36:52.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-06-20 11:36:53.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-06-20 11:36:53.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-06-20 11:36:54.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-06-20 11:36:47.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-06-20 11:36:46.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-06-20 11:36:48.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-06-20 11:36:47.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-06-20 11:36:50.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-06-20 11:36:38.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.207655 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-06-20 11:36:38.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-06-20 11:36:38.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.191654 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-20 11:38:13.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13497 2023-06-20 11:38:13.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:38:13.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-20 11:38:13.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 11:38:13.000000 iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-20 11:38:13.223655 iparapheur-provisioning-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.187654 iparapheur-provisioning-1.6.8/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.215655 iparapheur-provisioning-1.6.8/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:56.000000 iparapheur-provisioning-1.6.8/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 11:36:26.000000 iparapheur-provisioning-1.6.8/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:36:28.000000 iparapheur-provisioning-1.6.8/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:36:28.000000 iparapheur-provisioning-1.6.8/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-06-20 11:36:29.000000 iparapheur-provisioning-1.6.8/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:36:30.000000 iparapheur-provisioning-1.6.8/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:36:31.000000 iparapheur-provisioning-1.6.8/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-20 11:36:32.000000 iparapheur-provisioning-1.6.8/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-20 11:36:33.000000 iparapheur-provisioning-1.6.8/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-20 11:36:34.000000 iparapheur-provisioning-1.6.8/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-20 11:36:35.000000 iparapheur-provisioning-1.6.8/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-20 11:36:36.000000 iparapheur-provisioning-1.6.8/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-20 11:36:37.000000 iparapheur-provisioning-1.6.8/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.215655 iparapheur-provisioning-1.6.8/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.215655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.215655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-20 11:36:45.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.215655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-20 11:36:42.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-20 11:36:55.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-20 11:36:51.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.219655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:38:13.223655 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-20 11:36:39.000000 iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18391 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.047867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5602 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.055867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-06-22 14:38:57.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-06-22 14:38:59.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    28616 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+-rw-r--r--   0 root         (0) root         (0)    16907 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11413 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-06-22 14:39:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-06-22 14:39:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.071868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15193 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.043867 iparapheur-provisioning-1.7.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.075868 iparapheur-provisioning-1.7.0/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-22 14:38:57.000000 iparapheur-provisioning-1.7.0/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:38:59.000000 iparapheur-provisioning-1.7.0/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.075868 iparapheur-provisioning-1.7.0/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.8/LICENSE.md` & `iparapheur-provisioning-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/README.md` & `iparapheur-provisioning-1.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.6.8
+- Package version: 1.7.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
@@ -189,14 +189,19 @@
 *AdminAllUsersApi* | [**list_users_as_super_admin**](docs/apis/tags/AdminAllUsersApi.md#list_users_as_super_admin) | **get** /api/provisioning/v1/admin/user | List all users on the instance
 *AdminAllUsersApi* | [**update_user_as_super_admin**](docs/apis/tags/AdminAllUsersApi.md#update_user_as_super_admin) | **put** /api/provisioning/v1/admin/user/{userId} | Edit a user
 *AdminDeskApi* | [**create_desk**](docs/apis/tags/AdminDeskApi.md#create_desk) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/desk | Create a desk
 *AdminDeskApi* | [**delete_desk**](docs/apis/tags/AdminDeskApi.md#delete_desk) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Delete a desk
 *AdminDeskApi* | [**edit_desk**](docs/apis/tags/AdminDeskApi.md#edit_desk) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Edit a desk
 *AdminDeskApi* | [**get_desk_as_admin**](docs/apis/tags/AdminDeskApi.md#get_desk_as_admin) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Get a full desk description
 *AdminDeskApi* | [**list_desks**](docs/apis/tags/AdminDeskApi.md#list_desks) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk | List desks
+*AdminMetadataApi* | [**create_metadata**](docs/apis/tags/AdminMetadataApi.md#create_metadata) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/metadata | Create a metadata
+*AdminMetadataApi* | [**delete_metadata**](docs/apis/tags/AdminMetadataApi.md#delete_metadata) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Delete a metadata
+*AdminMetadataApi* | [**get_metadata**](docs/apis/tags/AdminMetadataApi.md#get_metadata) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Get a full metadata description
+*AdminMetadataApi* | [**list_metadata**](docs/apis/tags/AdminMetadataApi.md#list_metadata) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/metadata | List all metadata associated with the tenant
+*AdminMetadataApi* | [**update_metadata**](docs/apis/tags/AdminMetadataApi.md#update_metadata) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Edit a metadata
 *AdminTenantApi* | [**create_tenant**](docs/apis/tags/AdminTenantApi.md#create_tenant) | **post** /api/provisioning/v1/admin/tenant | Create a new tenant
 *AdminTenantApi* | [**delete_tenant**](docs/apis/tags/AdminTenantApi.md#delete_tenant) | **delete** /api/provisioning/v1/admin/tenant/{tenantId} | Delete a tenant
 *AdminTenantApi* | [**get_tenant**](docs/apis/tags/AdminTenantApi.md#get_tenant) | **get** /api/provisioning/v1/admin/tenant/{tenantId} | Get a full tenant description
 *AdminTenantApi* | [**update_tenant**](docs/apis/tags/AdminTenantApi.md#update_tenant) | **put** /api/provisioning/v1/admin/tenant/{tenantId} | Edit a tenant
 *AdminTenantUserApi* | [**create_user**](docs/apis/tags/AdminTenantUserApi.md#create_user) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/user | Create a new user
 *AdminTenantUserApi* | [**get_user**](docs/apis/tags/AdminTenantUserApi.md#get_user) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Get a full user description
 *AdminTenantUserApi* | [**list_tenant_users**](docs/apis/tags/AdminTenantUserApi.md#list_tenant_users) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user | List all users associated with the tenant
@@ -227,14 +232,15 @@
  - [LayerRepresentation](docs/models/LayerRepresentation.md)
  - [LayerSortBy](docs/models/LayerSortBy.md)
  - [MetadataDto](docs/models/MetadataDto.md)
  - [MetadataRepresentation](docs/models/MetadataRepresentation.md)
  - [MetadataSortBy](docs/models/MetadataSortBy.md)
  - [MetadataType](docs/models/MetadataType.md)
  - [PageDeskRepresentation](docs/models/PageDeskRepresentation.md)
+ - [PageMetadataRepresentation](docs/models/PageMetadataRepresentation.md)
  - [PageSubtypeRepresentation](docs/models/PageSubtypeRepresentation.md)
  - [PageTypeRepresentation](docs/models/PageTypeRepresentation.md)
  - [PageUserRepresentation](docs/models/PageUserRepresentation.md)
  - [PageableObject](docs/models/PageableObject.md)
  - [PdfSignaturePosition](docs/models/PdfSignaturePosition.md)
  - [SealCertificateSortBy](docs/models/SealCertificateSortBy.md)
  - [SignatureFormat](docs/models/SignatureFormat.md)
@@ -271,14 +277,15 @@
 ## Author
 
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
+iparapheur@libriciel.coop
 
 ## Notes for Large OpenAPI documents
 If the OpenAPI document is large, imports in iparapheur_provisioning.apis and iparapheur_provisioning.models may fail with a
 RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
 
 Solution 1:
 Use specific imports for apis and models like:
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.6.8"
+__version__ = "1.7.0"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.7.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/path_to_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,49 +2,55 @@
 
 from iparapheur_provisioning.paths import PathValues
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_user_user_id import ApiProvisioningV1AdminUserUserId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id import ApiProvisioningV1AdminTenantTenantId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import ApiProvisioningV1AdminTenantTenantIdUserUserId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import ApiProvisioningV1AdminTenantTenantIdDeskDeskId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant import ApiProvisioningV1AdminTenant
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_user import ApiProvisioningV1AdminTenantTenantIdUser
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import ApiProvisioningV1AdminTenantTenantIdTypologyType
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import ApiProvisioningV1AdminTenantTenantIdMetadata
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import ApiProvisioningV1AdminTenantTenantIdDesk
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_user import ApiProvisioningV1AdminUser
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID: ApiProvisioningV1AdminTenantTenantIdUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID: ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdMetadata,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID: ApiProvisioningV1AdminTenantTenantIdUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID: ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdMetadata,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
     }
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import typing_extensions
 
 from iparapheur_provisioning.apis.tags import TagValues
 from iparapheur_provisioning.apis.tags.admin_tenant_user_api import AdminTenantUserApi
 from iparapheur_provisioning.apis.tags.admin_desk_api import AdminDeskApi
+from iparapheur_provisioning.apis.tags.admin_metadata_api import AdminMetadataApi
 from iparapheur_provisioning.apis.tags.admin_typology_api import AdminTypologyApi
 from iparapheur_provisioning.apis.tags.admin_tenant_api import AdminTenantApi
 from iparapheur_provisioning.apis.tags.admin_all_users_api import AdminAllUsersApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi',
     {
         TagValues.ADMINTENANTUSER: AdminTenantUserApi,
         TagValues.ADMINDESK: AdminDeskApi,
+        TagValues.ADMINMETADATA: AdminMetadataApi,
         TagValues.ADMINTYPOLOGY: AdminTypologyApi,
         TagValues.ADMINTENANT: AdminTenantApi,
         TagValues.ADMINALLUSERS: AdminAllUsersApi,
     }
 )
 
 tag_to_api = TagToApi(
     {
         TagValues.ADMINTENANTUSER: AdminTenantUserApi,
         TagValues.ADMINDESK: AdminDeskApi,
+        TagValues.ADMINMETADATA: AdminMetadataApi,
         TagValues.ADMINTYPOLOGY: AdminTypologyApi,
         TagValues.ADMINTENANT: AdminTenantApi,
         TagValues.ADMINALLUSERS: AdminAllUsersApi,
     }
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.6.8".\
+               "SDK Package Version: 1.7.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 class MetadataDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    body
     """
 
 
     class MetaOapg:
         required = {
             "name",
             "key",
@@ -93,34 +95,54 @@
         
             @staticmethod
             def type() -> typing.Type['MetadataType']:
                 return MetadataType
             
             
             class restrictedValues(
-                schemas.ListSchema
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'restrictedValues':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
             __annotations__ = {
                 "name": name,
                 "key": key,
                 "id": id,
                 "index": index,
                 "type": type,
                 "restrictedValues": restrictedValues,
@@ -184,15 +206,15 @@
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         key: typing.Union[MetaOapg.properties.key, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         index: typing.Union[MetaOapg.properties.index, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         type: typing.Union['MetadataType', schemas.Unset] = schemas.unset,
-        restrictedValues: typing.Union[MetaOapg.properties.restrictedValues, list, tuple, schemas.Unset] = schemas.unset,
+        restrictedValues: typing.Union[MetaOapg.properties.restrictedValues, list, tuple, None, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'MetadataDto':
         return super().__new__(
             cls,
             *_args,
             name=name,
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from iparapheur_provisioning.model.layer_representation import LayerRepresentation
 from iparapheur_provisioning.model.layer_sort_by import LayerSortBy
 from iparapheur_provisioning.model.metadata_dto import MetadataDto
 from iparapheur_provisioning.model.metadata_representation import MetadataRepresentation
 from iparapheur_provisioning.model.metadata_sort_by import MetadataSortBy
 from iparapheur_provisioning.model.metadata_type import MetadataType
 from iparapheur_provisioning.model.page_desk_representation import PageDeskRepresentation
+from iparapheur_provisioning.model.page_metadata_representation import PageMetadataRepresentation
 from iparapheur_provisioning.model.page_subtype_representation import PageSubtypeRepresentation
 from iparapheur_provisioning.model.page_type_representation import PageTypeRepresentation
 from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.pdf_signature_position import PdfSignaturePosition
 from iparapheur_provisioning.model.seal_certificate_sort_by import SealCertificateSortBy
 from iparapheur_provisioning.model.signature_format import SignatureFormat
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 class PathValues(str, enum.Enum):
     API_PROVISIONING_V1_ADMIN_USER_USER_ID = "/api/provisioning/v1/admin/user/{userId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID = "/api/provisioning/v1/admin/tenant/{tenantId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/user/{userId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId}"
     API_PROVISIONING_V1_ADMIN_TENANT = "/api/provisioning/v1/admin/tenant"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER = "/api/provisioning/v1/admin/tenant/{tenantId}/user"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA = "/api/provisioning/v1/admin/tenant/{tenantId}/metadata"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK = "/api/provisioning/v1/admin/tenant/{tenantId}/desk"
     API_PROVISIONING_V1_ADMIN_USER = "/api/provisioning/v1/admin/user"
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,115 +40,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TenantDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
+    '401': _response_for_401,
+    '400': _response_for_400,
     '201': _response_for_201,
     '403': _response_for_403,
-    '400': _response_for_400,
-    '401': _response_for_401,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -125,16 +125,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,69 +55,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -132,17 +132,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -123,31 +123,31 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -162,18 +162,18 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,50 +143,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,135 +66,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '401': _response_for_401,
     '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -74,50 +74,50 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -133,16 +133,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,69 +63,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -140,17 +140,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,69 +135,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -212,17 +212,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '401': _response_for_401,
     '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,50 +74,50 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -133,16 +133,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,69 +63,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -140,17 +140,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,69 +74,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -151,17 +151,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,69 +143,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -220,17 +220,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '401': _response_for_401,
     '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,50 +82,50 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -141,16 +141,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,69 +71,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -148,17 +148,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,50 +101,50 @@
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor204ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -179,16 +179,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,50 +151,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -208,31 +208,31 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -247,18 +247,18 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '401': _response_for_401,
     '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,69 +63,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -140,17 +140,17 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,88 +74,88 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -170,18 +170,18 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '406': _response_for_406,
+    '401': _response_for_401,
     '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,50 +117,50 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -174,38 +174,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -104,38 +104,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,50 +55,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -112,31 +112,31 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -151,18 +151,18 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -123,31 +123,31 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -162,18 +162,18 @@
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
+    '403': _response_for_403,
     '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 iparapheur_provisioning/apis/path_to_api.py
 iparapheur_provisioning/apis/tag_to_api.py
 iparapheur_provisioning/apis/paths/__init__.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
 iparapheur_provisioning/apis/tags/__init__.py
 iparapheur_provisioning/apis/tags/admin_all_users_api.py
 iparapheur_provisioning/apis/tags/admin_desk_api.py
+iparapheur_provisioning/apis/tags/admin_metadata_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
 iparapheur_provisioning/apis/tags/admin_typology_api.py
 iparapheur_provisioning/model/__init__.py
 iparapheur_provisioning/model/delegation_sort_by.py
 iparapheur_provisioning/model/desk_dto.py
 iparapheur_provisioning/model/desk_representation.py
@@ -48,14 +51,15 @@
 iparapheur_provisioning/model/layer_representation.py
 iparapheur_provisioning/model/layer_sort_by.py
 iparapheur_provisioning/model/metadata_dto.py
 iparapheur_provisioning/model/metadata_representation.py
 iparapheur_provisioning/model/metadata_sort_by.py
 iparapheur_provisioning/model/metadata_type.py
 iparapheur_provisioning/model/page_desk_representation.py
+iparapheur_provisioning/model/page_metadata_representation.py
 iparapheur_provisioning/model/page_subtype_representation.py
 iparapheur_provisioning/model/page_type_representation.py
 iparapheur_provisioning/model/page_user_representation.py
 iparapheur_provisioning/model/pageable_object.py
 iparapheur_provisioning/model/pdf_signature_position.py
 iparapheur_provisioning/model/seal_certificate_sort_by.py
 iparapheur_provisioning/model/signature_format.py
@@ -88,14 +92,21 @@
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
@@ -132,14 +143,15 @@
 test/test_models/test_layer_representation.py
 test/test_models/test_layer_sort_by.py
 test/test_models/test_metadata_dto.py
 test/test_models/test_metadata_representation.py
 test/test_models/test_metadata_sort_by.py
 test/test_models/test_metadata_type.py
 test/test_models/test_page_desk_representation.py
+test/test_models/test_page_metadata_representation.py
 test/test_models/test_page_subtype_representation.py
 test/test_models/test_page_type_representation.py
 test/test_models/test_page_user_representation.py
 test/test_models/test_pageable_object.py
 test/test_models/test_pdf_signature_position.py
 test/test_models/test_seal_certificate_sort_by.py
 test/test_models/test_signature_format.py
@@ -171,14 +183,21 @@
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.8/setup.py` & `iparapheur-provisioning-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.6.8"
+VERSION = "1.7.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.0/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/__init__.py` & `iparapheur-provisioning-1.7.0/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Edit a desk  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        Create a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        Create a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 406
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Edit a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
+        Edit a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 406
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.8/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

