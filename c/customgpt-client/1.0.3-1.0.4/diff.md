# Comparing `tmp/customgpt_client-1.0.3.tar.gz` & `tmp/customgpt_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customgpt_client-1.0.3.tar", max compression
+gzip compressed data, was "customgpt_client-1.0.4.tar", max compression
```

## Comparing `customgpt_client-1.0.3.tar` & `customgpt_client-1.0.4.tar`

### file list

```diff
@@ -1,84 +1,376 @@
--rw-r--r--   0        0        0     3542 2023-06-08 08:28:24.767137 customgpt_client-1.0.3/README.md
--rw-r--r--   0        0        0      151 2023-06-20 20:40:24.008285 customgpt_client-1.0.3/custom_gpt_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-20 20:40:23.104552 customgpt_client-1.0.3/custom_gpt_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.144540 customgpt_client-1.0.3/custom_gpt_client/api/citations/__init__.py
--rw-r--r--   0        0        0     5325 2023-06-20 20:40:24.116253 customgpt_client-1.0.3/custom_gpt_client/api/citations/get_open_graph_data_for_citation.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.136543 customgpt_client-1.0.3/custom_gpt_client/api/conversations/__init__.py
--rw-r--r--   0        0        0     3498 2023-06-20 20:40:24.100258 customgpt_client-1.0.3/custom_gpt_client/api/conversations/create_project_conversation.py
--rw-r--r--   0        0        0     3222 2023-06-20 20:40:24.084263 customgpt_client-1.0.3/custom_gpt_client/api/conversations/delete_project_conversation.py
--rw-r--r--   0        0        0     4822 2023-06-20 20:40:24.204227 customgpt_client-1.0.3/custom_gpt_client/api/conversations/get_project_conversation_messages.py
--rw-r--r--   0        0        0     7055 2023-06-20 20:40:24.196230 customgpt_client-1.0.3/custom_gpt_client/api/conversations/get_project_conversations.py
--rw-r--r--   0        0        0     7103 2023-06-20 20:40:24.192231 customgpt_client-1.0.3/custom_gpt_client/api/conversations/send_message_to_conversation.py
--rw-r--r--   0        0        0     6060 2023-06-20 20:40:24.152243 customgpt_client-1.0.3/custom_gpt_client/api/conversations/update_project_conversation.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.132544 customgpt_client-1.0.3/custom_gpt_client/api/pages/__init__.py
--rw-r--r--   0        0        0     3270 2023-06-20 20:40:24.084263 customgpt_client-1.0.3/custom_gpt_client/api/pages/delete_project_page.py
--rw-r--r--   0        0        0     2709 2023-06-20 20:40:24.152243 customgpt_client-1.0.3/custom_gpt_client/api/pages/get_preview.py
--rw-r--r--   0        0        0     7272 2023-06-20 20:40:24.240217 customgpt_client-1.0.3/custom_gpt_client/api/pages/get_project_pages.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.136543 customgpt_client-1.0.3/custom_gpt_client/api/project_settings/__init__.py
--rw-r--r--   0        0        0     2985 2023-06-20 20:40:24.184233 customgpt_client-1.0.3/custom_gpt_client/api/project_settings/get_project_settings.py
--rw-r--r--   0        0        0     3581 2023-06-20 20:40:24.196230 customgpt_client-1.0.3/custom_gpt_client/api/project_settings/update_project_settings.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.124546 customgpt_client-1.0.3/custom_gpt_client/api/projects/__init__.py
--rw-r--r--   0        0        0     3297 2023-06-20 20:40:24.292201 customgpt_client-1.0.3/custom_gpt_client/api/projects/create_project.py
--rw-r--r--   0        0        0     2965 2023-06-20 20:40:24.240217 customgpt_client-1.0.3/custom_gpt_client/api/projects/delete_project.py
--rw-r--r--   0        0        0     3864 2023-06-20 20:40:24.304198 customgpt_client-1.0.3/custom_gpt_client/api/projects/get_project.py
--rw-r--r--   0        0        0     2994 2023-06-20 20:40:24.272207 customgpt_client-1.0.3/custom_gpt_client/api/projects/get_project_stats.py
--rw-r--r--   0        0        0     7848 2023-06-20 20:40:24.456153 customgpt_client-1.0.3/custom_gpt_client/api/projects/list_projects.py
--rw-r--r--   0        0        0     3377 2023-06-20 20:40:24.296200 customgpt_client-1.0.3/custom_gpt_client/api/projects/update_project.py
--rw-r--r--   0        0        0        0 2023-06-20 20:40:23.144540 customgpt_client-1.0.3/custom_gpt_client/api/users/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-20 20:40:24.328191 customgpt_client-1.0.3/custom_gpt_client/api/users/get_user_profile.py
--rw-r--r--   0        0        0     5088 2023-06-20 20:40:24.456153 customgpt_client-1.0.3/custom_gpt_client/api/users/update_user_profile.py
--rw-r--r--   0        0        0    15936 2023-06-20 20:40:24.812048 customgpt_client-1.0.3/custom_gpt_client/client.py
--rw-r--r--   0        0        0      470 2023-06-20 20:40:24.284204 customgpt_client-1.0.3/custom_gpt_client/errors.py
--rw-r--r--   0        0        0     5311 2023-06-20 20:40:23.060565 customgpt_client-1.0.3/custom_gpt_client/models/__init__.py
--rw-r--r--   0        0        0     4878 2023-06-20 20:40:24.540128 customgpt_client-1.0.3/custom_gpt_client/models/conversation.py
--rw-r--r--   0        0        0     1604 2023-06-20 20:40:24.452154 customgpt_client-1.0.3/custom_gpt_client/models/create_project_conversation_json_body.py
--rw-r--r--   0        0        0     4400 2023-06-20 20:40:24.468149 customgpt_client-1.0.3/custom_gpt_client/models/create_project_multipart_data.py
--rw-r--r--   0        0        0     3148 2023-06-20 20:40:24.428161 customgpt_client-1.0.3/custom_gpt_client/models/get_open_graph_data_for_citation_response_200.py
--rw-r--r--   0        0        0     2412 2023-06-20 20:40:24.408167 customgpt_client-1.0.3/custom_gpt_client/models/get_open_graph_data_for_citation_response_200_data.py
--rw-r--r--   0        0        0      193 2023-06-20 20:40:23.692379 customgpt_client-1.0.3/custom_gpt_client/models/get_open_graph_data_for_citation_response_200_status.py
--rw-r--r--   0        0        0      174 2023-06-20 20:40:23.692379 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversation_messages_order.py
--rw-r--r--   0        0        0      167 2023-06-20 20:40:23.732367 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_order.py
--rw-r--r--   0        0        0     3017 2023-06-20 20:40:24.540128 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200.py
--rw-r--r--   0        0        0     6843 2023-06-20 20:40:24.660092 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200_data.py
--rw-r--r--   0        0        0     2602 2023-06-20 20:40:24.552124 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200_data_links.py
--rw-r--r--   0        0        0      189 2023-06-20 20:40:23.740364 customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200_status.py
--rw-r--r--   0        0        0      159 2023-06-20 20:40:23.696377 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_order.py
--rw-r--r--   0        0        0     2865 2023-06-20 20:40:24.632101 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200.py
--rw-r--r--   0        0        0     2842 2023-06-20 20:40:24.616106 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data.py
--rw-r--r--   0        0        0     6728 2023-06-20 20:40:24.660092 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data_pages.py
--rw-r--r--   0        0        0     2590 2023-06-20 20:40:24.632101 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data_pages_links.py
--rw-r--r--   0        0        0      181 2023-06-20 20:40:23.704375 customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_status.py
--rw-r--r--   0        0        0     2846 2023-06-20 20:40:24.624103 customgpt_client-1.0.3/custom_gpt_client/models/get_user_profile_response_200.py
--rw-r--r--   0        0        0     1918 2023-06-20 20:40:24.616106 customgpt_client-1.0.3/custom_gpt_client/models/get_user_profile_response_200_data.py
--rw-r--r--   0        0        0      180 2023-06-20 20:40:23.700376 customgpt_client-1.0.3/custom_gpt_client/models/get_user_profile_response_200_status.py
--rw-r--r--   0        0        0      156 2023-06-20 20:40:23.700376 customgpt_client-1.0.3/custom_gpt_client/models/list_projects_order.py
--rw-r--r--   0        0        0     2802 2023-06-20 20:40:24.716076 customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200.py
--rw-r--r--   0        0        0     6635 2023-06-20 20:40:24.975999 customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200_data.py
--rw-r--r--   0        0        0     2544 2023-06-20 20:40:24.716076 customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200_data_links.py
--rw-r--r--   0        0        0      178 2023-06-20 20:40:23.700376 customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200_status.py
--rw-r--r--   0        0        0     4285 2023-06-20 20:40:24.748067 customgpt_client-1.0.3/custom_gpt_client/models/open_graph_cache.py
--rw-r--r--   0        0        0     8656 2023-06-20 20:40:24.999992 customgpt_client-1.0.3/custom_gpt_client/models/page.py
--rw-r--r--   0        0        0      217 2023-06-20 20:40:23.764357 customgpt_client-1.0.3/custom_gpt_client/models/page_crawl_status.py
--rw-r--r--   0        0        0      217 2023-06-20 20:40:23.688380 customgpt_client-1.0.3/custom_gpt_client/models/page_index_status.py
--rw-r--r--   0        0        0     7789 2023-06-20 20:40:24.904020 customgpt_client-1.0.3/custom_gpt_client/models/project.py
--rw-r--r--   0        0        0     3482 2023-06-20 20:40:24.776058 customgpt_client-1.0.3/custom_gpt_client/models/project_plugin.py
--rw-r--r--   0        0        0     4467 2023-06-20 20:40:24.824044 customgpt_client-1.0.3/custom_gpt_client/models/project_settings.py
--rw-r--r--   0        0        0      236 2023-06-20 20:40:23.768356 customgpt_client-1.0.3/custom_gpt_client/models/project_settings_response_source.py
--rw-r--r--   0        0        0      156 2023-06-20 20:40:23.700376 customgpt_client-1.0.3/custom_gpt_client/models/project_type.py
--rw-r--r--   0        0        0     5019 2023-06-20 20:40:24.868031 customgpt_client-1.0.3/custom_gpt_client/models/prompt_history.py
--rw-r--r--   0        0        0     1654 2023-06-20 20:40:24.804050 customgpt_client-1.0.3/custom_gpt_client/models/send_message_to_conversation_json_body.py
--rw-r--r--   0        0        0     1628 2023-06-20 20:40:24.832042 customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_json_body.py
--rw-r--r--   0        0        0     3055 2023-06-20 20:40:24.892024 customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_response_200.py
--rw-r--r--   0        0        0     2305 2023-06-20 20:40:24.884026 customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_response_200_data.py
--rw-r--r--   0        0        0      191 2023-06-20 20:40:23.704375 customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_response_200_status.py
--rw-r--r--   0        0        0     4948 2023-06-20 20:40:24.968002 customgpt_client-1.0.3/custom_gpt_client/models/update_project_multipart_data.py
--rw-r--r--   0        0        0     6861 2023-06-20 20:40:25.023985 customgpt_client-1.0.3/custom_gpt_client/models/update_project_settings_multipart_data.py
--rw-r--r--   0        0        0     3050 2023-06-20 20:40:24.968002 customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_multipart_data.py
--rw-r--r--   0        0        0     2903 2023-06-20 20:40:24.995993 customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_response_200.py
--rw-r--r--   0        0        0     1933 2023-06-20 20:40:24.991994 customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_response_200_data.py
--rw-r--r--   0        0        0      183 2023-06-20 20:40:23.696377 customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_response_200_status.py
--rw-r--r--   0        0        0     3791 2023-06-20 20:40:25.019986 customgpt_client-1.0.3/custom_gpt_client/models/user.py
--rw-r--r--   0        0        0       25 2023-06-20 20:40:22.896614 customgpt_client-1.0.3/custom_gpt_client/py.typed
--rw-r--r--   0        0        0      993 2023-06-20 20:40:24.995993 customgpt_client-1.0.3/custom_gpt_client/types.py
--rw-r--r--   0        0        0      679 2023-06-20 21:04:45.248655 customgpt_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 customgpt_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3542 2023-06-08 08:28:24.767137 customgpt_client-1.0.4/README.md
+-rw-r--r--   0        0        0      105 2023-06-22 11:37:05.439351 customgpt_client-1.0.4/custom_gpt_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-22 11:37:02.875324 customgpt_client-1.0.4/custom_gpt_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.935325 customgpt_client-1.0.4/custom_gpt_client/api/citations/__init__.py
+-rw-r--r--   0        0        0     6513 2023-06-22 11:37:05.555352 customgpt_client-1.0.4/custom_gpt_client/api/citations/get_open_graph_data_for_citation.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.923325 customgpt_client-1.0.4/custom_gpt_client/api/conversations/__init__.py
+-rw-r--r--   0        0        0     7370 2023-06-22 11:37:05.583353 customgpt_client-1.0.4/custom_gpt_client/api/conversations/create_project_conversation.py
+-rw-r--r--   0        0        0     6970 2023-06-22 11:37:05.783355 customgpt_client-1.0.4/custom_gpt_client/api/conversations/delete_project_conversation.py
+-rw-r--r--   0        0        0     8648 2023-06-22 11:37:05.615353 customgpt_client-1.0.4/custom_gpt_client/api/conversations/get_project_conversations.py
+-rw-r--r--   0        0        0     8015 2023-06-22 11:37:05.763354 customgpt_client-1.0.4/custom_gpt_client/api/conversations/messages.py
+-rw-r--r--   0        0        0    12263 2023-06-22 11:43:29.208591 customgpt_client-1.0.4/custom_gpt_client/api/conversations/send_message_to_conversation.py
+-rw-r--r--   0        0        0     7725 2023-06-22 11:37:05.695354 customgpt_client-1.0.4/custom_gpt_client/api/conversations/update_project_conversation.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.911325 customgpt_client-1.0.4/custom_gpt_client/api/pages/__init__.py
+-rw-r--r--   0        0        0     6716 2023-06-22 11:37:05.803355 customgpt_client-1.0.4/custom_gpt_client/api/pages/delete_project_page.py
+-rw-r--r--   0        0        0     8458 2023-06-22 11:37:05.791355 customgpt_client-1.0.4/custom_gpt_client/api/pages/get_project_pages.py
+-rw-r--r--   0        0        0     4706 2023-06-22 11:37:05.699354 customgpt_client-1.0.4/custom_gpt_client/api/pages/preview.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.915325 customgpt_client-1.0.4/custom_gpt_client/api/project_settings/__init__.py
+-rw-r--r--   0        0        0     6233 2023-06-22 11:37:06.011357 customgpt_client-1.0.4/custom_gpt_client/api/project_settings/get_project_settings.py
+-rw-r--r--   0        0        0     7313 2023-06-22 11:37:05.943356 customgpt_client-1.0.4/custom_gpt_client/api/project_settings/update_project_settings.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.899325 customgpt_client-1.0.4/custom_gpt_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     6242 2023-06-22 11:37:05.955356 customgpt_client-1.0.4/custom_gpt_client/api/projects/create_project.py
+-rw-r--r--   0        0        0     5760 2023-06-22 11:37:06.039357 customgpt_client-1.0.4/custom_gpt_client/api/projects/delete_project.py
+-rw-r--r--   0        0        0     7074 2023-06-22 11:37:06.171359 customgpt_client-1.0.4/custom_gpt_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     8489 2023-06-22 11:37:06.235359 customgpt_client-1.0.4/custom_gpt_client/api/projects/list_projects.py
+-rw-r--r--   0        0        0     5767 2023-06-22 11:37:06.075358 customgpt_client-1.0.4/custom_gpt_client/api/projects/stats_project.py
+-rw-r--r--   0        0        0     6358 2023-06-22 11:37:06.239359 customgpt_client-1.0.4/custom_gpt_client/api/projects/update_project.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:02.939325 customgpt_client-1.0.4/custom_gpt_client/api/users/__init__.py
+-rw-r--r--   0        0        0     4857 2023-06-22 11:37:06.179359 customgpt_client-1.0.4/custom_gpt_client/api/users/get_user_profile.py
+-rw-r--r--   0        0        0     5851 2023-06-22 11:37:06.327360 customgpt_client-1.0.4/custom_gpt_client/api/users/update_user_profile.py
+-rw-r--r--   0        0        0    20470 2023-06-22 11:37:06.823366 customgpt_client-1.0.4/custom_gpt_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-22 11:37:06.063358 customgpt_client-1.0.4/custom_gpt_client/errors.py
+-rw-r--r--   0        0        0    42317 2023-06-22 11:37:04.723343 customgpt_client-1.0.4/custom_gpt_client/models/__init__.py
+-rw-r--r--   0        0        0     4878 2023-06-22 11:37:06.479362 customgpt_client-1.0.4/custom_gpt_client/models/conversation.py
+-rw-r--r--   0        0        0     1604 2023-06-22 11:37:06.243359 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_json_body.py
+-rw-r--r--   0        0        0     3055 2023-06-22 11:37:06.387361 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_201.py
+-rw-r--r--   0        0        0     5033 2023-06-22 11:37:06.443362 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_201_data.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.727344 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_201_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.339361 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_401.py
+-rw-r--r--   0        0        0     2456 2023-06-22 11:37:06.335360 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_401_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.367340 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.615342 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_401_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.427361 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404.py
+-rw-r--r--   0        0        0     3034 2023-06-22 11:37:06.503362 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.343340 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.739344 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.735344 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.459362 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_500.py
+-rw-r--r--   0        0        0     2439 2023-06-22 11:37:06.419361 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_500_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.331339 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:05.023347 customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_500_status.py
+-rw-r--r--   0        0        0     4400 2023-06-22 11:37:06.547363 customgpt_client-1.0.4/custom_gpt_client/models/create_project_multipart_data.py
+-rw-r--r--   0        0        0     2821 2023-06-22 11:37:06.579363 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_201.py
+-rw-r--r--   0        0        0     8090 2023-06-22 11:37:06.679364 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_201_data.py
+-rw-r--r--   0        0        0      177 2023-06-22 11:37:04.611342 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_201_data_type.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.491341 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_201_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:06.547363 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_400.py
+-rw-r--r--   0        0        0     2819 2023-06-22 11:37:06.535363 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_400_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.951346 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_400_data_code.py
+-rw-r--r--   0        0        0      362 2023-06-22 11:37:04.523342 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_400_data_message.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.579342 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_400_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:06.659364 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_401.py
+-rw-r--r--   0        0        0     2320 2023-06-22 11:37:06.635364 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.351340 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.595342 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_401_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:06.651364 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_500.py
+-rw-r--r--   0        0        0     2303 2023-06-22 11:37:06.631363 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.895345 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:05.023347 customgpt_client-1.0.4/custom_gpt_client/models/create_project_response_500_status.py
+-rw-r--r--   0        0        0     3055 2023-06-22 11:37:06.695364 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_200.py
+-rw-r--r--   0        0        0     1700 2023-06-22 11:37:06.635364 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_200_data.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.419340 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_200_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.771365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_401.py
+-rw-r--r--   0        0        0     2456 2023-06-22 11:37:06.783365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_401_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.343340 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.579342 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_401_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.747365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_404.py
+-rw-r--r--   0        0        0     3034 2023-06-22 11:37:06.783365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_404_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.727344 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.411340 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.819345 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_404_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:06.823366 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_500.py
+-rw-r--r--   0        0        0     2439 2023-06-22 11:37:06.767365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_500_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.547342 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:05.011347 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_conversation_response_500_status.py
+-rw-r--r--   0        0        0     2903 2023-06-22 11:37:06.811365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_200.py
+-rw-r--r--   0        0        0     1660 2023-06-22 11:37:06.803365 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_200_data.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.683343 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_200_status.py
+-rw-r--r--   0        0        0     3189 2023-06-22 11:37:06.875366 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_401.py
+-rw-r--r--   0        0        0     2368 2023-06-22 11:37:06.843366 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_401_data.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:04.479341 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_401_data_code.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.655343 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_401_status.py
+-rw-r--r--   0        0        0     3189 2023-06-22 11:37:06.955367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_404.py
+-rw-r--r--   0        0        0     2889 2023-06-22 11:37:06.947367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_404_data.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:04.423340 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_404_data_code.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:04.763344 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_404_data_message.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.411340 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_404_status.py
+-rw-r--r--   0        0        0     3189 2023-06-22 11:37:06.987367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_500.py
+-rw-r--r--   0        0        0     2351 2023-06-22 11:37:06.891366 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_500_data.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:05.003347 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_500_data_code.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.563342 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_page_response_500_status.py
+-rw-r--r--   0        0        0     2821 2023-06-22 11:37:06.987367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_200.py
+-rw-r--r--   0        0        0     1637 2023-06-22 11:37:06.951367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_200_data.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.831345 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_200_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:06.979367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_401.py
+-rw-r--r--   0        0        0     2320 2023-06-22 11:37:06.995367 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.555342 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.751344 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_401_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:07.047368 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_404.py
+-rw-r--r--   0        0        0     2816 2023-06-22 11:37:07.027368 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_404_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.579342 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_404_data_code.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.483341 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_404_data_message.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.635343 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_404_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:07.043368 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_500.py
+-rw-r--r--   0        0        0     2303 2023-06-22 11:37:07.031368 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.751344 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.455341 customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_500_status.py
+-rw-r--r--   0        0        0     3148 2023-06-22 11:37:07.119369 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_200.py
+-rw-r--r--   0        0        0     4443 2023-06-22 11:37:07.155369 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_200_data.py
+-rw-r--r--   0        0        0      193 2023-06-22 11:37:04.363340 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_200_status.py
+-rw-r--r--   0        0        0     3422 2023-06-22 11:37:07.139369 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_401.py
+-rw-r--r--   0        0        0     2499 2023-06-22 11:37:07.075368 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_401_data.py
+-rw-r--r--   0        0        0      272 2023-06-22 11:37:04.871345 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_401_data_code.py
+-rw-r--r--   0        0        0      193 2023-06-22 11:37:05.035347 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_401_status.py
+-rw-r--r--   0        0        0     3422 2023-06-22 11:37:07.139369 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_404.py
+-rw-r--r--   0        0        0     3092 2023-06-22 11:37:07.099368 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_404_data.py
+-rw-r--r--   0        0        0      272 2023-06-22 11:37:04.883345 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_404_data_code.py
+-rw-r--r--   0        0        0      272 2023-06-22 11:37:04.939346 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_404_data_message.py
+-rw-r--r--   0        0        0      193 2023-06-22 11:37:05.007346 customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_404_status.py
+-rw-r--r--   0        0        0      167 2023-06-22 11:37:04.795344 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_order.py
+-rw-r--r--   0        0        0     3017 2023-06-22 11:37:07.139369 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200.py
+-rw-r--r--   0        0        0     7137 2023-06-22 11:37:07.307371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_data.py
+-rw-r--r--   0        0        0     5069 2023-06-22 11:37:07.223370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_data_data_item.py
+-rw-r--r--   0        0        0     2602 2023-06-22 11:37:07.179369 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_data_links.py
+-rw-r--r--   0        0        0      189 2023-06-22 11:37:04.875345 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_status.py
+-rw-r--r--   0        0        0     3303 2023-06-22 11:37:07.287371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_401.py
+-rw-r--r--   0        0        0     2434 2023-06-22 11:37:07.207370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_401_data.py
+-rw-r--r--   0        0        0      268 2023-06-22 11:37:04.687343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_401_data_code.py
+-rw-r--r--   0        0        0      189 2023-06-22 11:37:04.347339 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_401_status.py
+-rw-r--r--   0        0        0     3303 2023-06-22 11:37:07.227370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_404.py
+-rw-r--r--   0        0        0     2991 2023-06-22 11:37:07.219370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_404_data.py
+-rw-r--r--   0        0        0      268 2023-06-22 11:37:04.687343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_404_data_code.py
+-rw-r--r--   0        0        0      268 2023-06-22 11:37:04.539342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_404_data_message.py
+-rw-r--r--   0        0        0      189 2023-06-22 11:37:04.775344 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_404_status.py
+-rw-r--r--   0        0        0     3303 2023-06-22 11:37:07.255370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_500.py
+-rw-r--r--   0        0        0     2417 2023-06-22 11:37:07.279370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_500_data.py
+-rw-r--r--   0        0        0      268 2023-06-22 11:37:04.423340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_500_data_code.py
+-rw-r--r--   0        0        0      189 2023-06-22 11:37:04.515341 customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_500_status.py
+-rw-r--r--   0        0        0      159 2023-06-22 11:37:04.387340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_order.py
+-rw-r--r--   0        0        0     2865 2023-06-22 11:37:07.295370 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200.py
+-rw-r--r--   0        0        0     3094 2023-06-22 11:37:07.287371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data.py
+-rw-r--r--   0        0        0     7042 2023-06-22 11:37:07.395372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages.py
+-rw-r--r--   0        0        0     9561 2023-06-22 11:37:07.479372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages_data_item.py
+-rw-r--r--   0        0        0      256 2023-06-22 11:37:05.019347 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages_data_item_crawl_status.py
+-rw-r--r--   0        0        0      256 2023-06-22 11:37:04.671343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages_data_item_index_status.py
+-rw-r--r--   0        0        0     2590 2023-06-22 11:37:07.367371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages_links.py
+-rw-r--r--   0        0        0     8215 2023-06-22 11:37:07.531373 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_project.py
+-rw-r--r--   0        0        0      186 2023-06-22 11:37:04.567342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_project_type.py
+-rw-r--r--   0        0        0      181 2023-06-22 11:37:04.615342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_status.py
+-rw-r--r--   0        0        0     3151 2023-06-22 11:37:07.375371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_401.py
+-rw-r--r--   0        0        0     2346 2023-06-22 11:37:07.359371 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_401_data.py
+-rw-r--r--   0        0        0      260 2023-06-22 11:37:04.919345 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_401_data_code.py
+-rw-r--r--   0        0        0      181 2023-06-22 11:37:04.567342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_401_status.py
+-rw-r--r--   0        0        0     3151 2023-06-22 11:37:07.395372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_404.py
+-rw-r--r--   0        0        0     2855 2023-06-22 11:37:07.379372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_404_data.py
+-rw-r--r--   0        0        0      260 2023-06-22 11:37:04.519341 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_404_data_code.py
+-rw-r--r--   0        0        0      260 2023-06-22 11:37:04.827345 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_404_data_message.py
+-rw-r--r--   0        0        0      181 2023-06-22 11:37:04.463341 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_404_status.py
+-rw-r--r--   0        0        0     3151 2023-06-22 11:37:07.455372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_500.py
+-rw-r--r--   0        0        0     2329 2023-06-22 11:37:07.435372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_500_data.py
+-rw-r--r--   0        0        0      260 2023-06-22 11:37:04.803344 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_500_data_code.py
+-rw-r--r--   0        0        0      181 2023-06-22 11:37:04.627343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_500_status.py
+-rw-r--r--   0        0        0     2764 2023-06-22 11:37:07.459372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_200.py
+-rw-r--r--   0        0        0     8051 2023-06-22 11:37:07.623374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_200_data.py
+-rw-r--r--   0        0        0      174 2023-06-22 11:37:04.523342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_200_data_type.py
+-rw-r--r--   0        0        0      176 2023-06-22 11:37:04.371340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_200_status.py
+-rw-r--r--   0        0        0     3050 2023-06-22 11:37:07.535373 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_401.py
+-rw-r--r--   0        0        0     2287 2023-06-22 11:37:07.471372 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_401_data.py
+-rw-r--r--   0        0        0      255 2023-06-22 11:37:05.011347 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_401_data_code.py
+-rw-r--r--   0        0        0      176 2023-06-22 11:37:04.391340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_401_status.py
+-rw-r--r--   0        0        0     3050 2023-06-22 11:37:07.531373 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_404.py
+-rw-r--r--   0        0        0     2753 2023-06-22 11:37:07.559373 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_404_data.py
+-rw-r--r--   0        0        0      255 2023-06-22 11:37:04.999346 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_404_data_code.py
+-rw-r--r--   0        0        0      255 2023-06-22 11:37:04.959346 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_404_data_message.py
+-rw-r--r--   0        0        0      176 2023-06-22 11:37:04.767344 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_404_status.py
+-rw-r--r--   0        0        0     3050 2023-06-22 11:37:07.559373 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_500.py
+-rw-r--r--   0        0        0     2270 2023-06-22 11:37:07.575374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_500_data.py
+-rw-r--r--   0        0        0      255 2023-06-22 11:37:04.411340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_500_data_code.py
+-rw-r--r--   0        0        0      176 2023-06-22 11:37:04.931346 customgpt_client-1.0.4/custom_gpt_client/models/get_project_response_500_status.py
+-rw-r--r--   0        0        0     2922 2023-06-22 11:37:07.627374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_200.py
+-rw-r--r--   0        0        0     4690 2023-06-22 11:37:07.691375 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_200_data.py
+-rw-r--r--   0        0        0      254 2023-06-22 11:37:04.815344 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_200_data_response_source.py
+-rw-r--r--   0        0        0      184 2023-06-22 11:37:05.031347 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_200_status.py
+-rw-r--r--   0        0        0     3208 2023-06-22 11:37:07.619374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_401.py
+-rw-r--r--   0        0        0     2379 2023-06-22 11:37:07.599374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_401_data.py
+-rw-r--r--   0        0        0      263 2023-06-22 11:37:04.883345 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_401_data_code.py
+-rw-r--r--   0        0        0      184 2023-06-22 11:37:04.671343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_401_status.py
+-rw-r--r--   0        0        0     3208 2023-06-22 11:37:07.715375 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_404.py
+-rw-r--r--   0        0        0     2906 2023-06-22 11:37:07.671374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_404_data.py
+-rw-r--r--   0        0        0      263 2023-06-22 11:37:04.399340 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_404_data_code.py
+-rw-r--r--   0        0        0      263 2023-06-22 11:37:04.623342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_404_data_message.py
+-rw-r--r--   0        0        0      184 2023-06-22 11:37:04.591342 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_404_status.py
+-rw-r--r--   0        0        0     3208 2023-06-22 11:37:07.667374 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_500.py
+-rw-r--r--   0        0        0     2362 2023-06-22 11:37:07.699375 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_500_data.py
+-rw-r--r--   0        0        0      263 2023-06-22 11:37:04.687343 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_500_data_code.py
+-rw-r--r--   0        0        0      184 2023-06-22 11:37:04.511341 customgpt_client-1.0.4/custom_gpt_client/models/get_project_settings_response_500_status.py
+-rw-r--r--   0        0        0     2846 2023-06-22 11:37:07.763375 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_200.py
+-rw-r--r--   0        0        0     3931 2023-06-22 11:37:07.743375 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_200_data.py
+-rw-r--r--   0        0        0      180 2023-06-22 11:37:04.511341 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_200_status.py
+-rw-r--r--   0        0        0     3132 2023-06-22 11:37:07.763375 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_401.py
+-rw-r--r--   0        0        0     2335 2023-06-22 11:37:07.779376 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_401_data.py
+-rw-r--r--   0        0        0      259 2023-06-22 11:37:04.491341 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_401_data_code.py
+-rw-r--r--   0        0        0      180 2023-06-22 11:37:04.515341 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_401_status.py
+-rw-r--r--   0        0        0     3132 2023-06-22 11:37:07.795376 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_500.py
+-rw-r--r--   0        0        0     2318 2023-06-22 11:37:07.767376 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_500_data.py
+-rw-r--r--   0        0        0      259 2023-06-22 11:37:04.427340 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_500_data_code.py
+-rw-r--r--   0        0        0      180 2023-06-22 11:37:04.775344 customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_500_status.py
+-rw-r--r--   0        0        0      156 2023-06-22 11:37:04.551342 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_order.py
+-rw-r--r--   0        0        0     2802 2023-06-22 11:37:07.775375 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200.py
+-rw-r--r--   0        0        0     6843 2023-06-22 11:37:07.887377 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data.py
+-rw-r--r--   0        0        0     8189 2023-06-22 11:37:07.987378 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data_data_item.py
+-rw-r--r--   0        0        0      184 2023-06-22 11:37:04.795344 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data_data_item_type.py
+-rw-r--r--   0        0        0     2544 2023-06-22 11:37:07.835376 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data_links.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.503341 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_status.py
+-rw-r--r--   0        0        0     3088 2023-06-22 11:37:07.859377 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_401.py
+-rw-r--r--   0        0        0     2309 2023-06-22 11:37:07.927377 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_401_data.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:04.379340 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:05.035347 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_401_status.py
+-rw-r--r--   0        0        0     3088 2023-06-22 11:37:07.859377 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_500.py
+-rw-r--r--   0        0        0     2292 2023-06-22 11:37:07.847376 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_500_data.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:05.027347 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.987346 customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_500_status.py
+-rw-r--r--   0        0        0      152 2023-06-22 11:37:04.619342 customgpt_client-1.0.4/custom_gpt_client/models/messages_order.py
+-rw-r--r--   0        0        0     3753 2023-06-22 11:37:07.923377 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200.py
+-rw-r--r--   0        0        0     4982 2023-06-22 11:37:08.035378 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_conversation.py
+-rw-r--r--   0        0        0     6836 2023-06-22 11:37:08.067379 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_messages.py
+-rw-r--r--   0        0        0     5141 2023-06-22 11:37:08.067379 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_messages_data_item.py
+-rw-r--r--   0        0        0     2541 2023-06-22 11:37:07.947377 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_messages_links.py
+-rw-r--r--   0        0        0      174 2023-06-22 11:37:04.755344 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_status.py
+-rw-r--r--   0        0        0     3006 2023-06-22 11:37:07.991378 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_401.py
+-rw-r--r--   0        0        0     2261 2023-06-22 11:37:08.039378 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_401_data.py
+-rw-r--r--   0        0        0      253 2023-06-22 11:37:04.387340 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_401_data_code.py
+-rw-r--r--   0        0        0      174 2023-06-22 11:37:04.963346 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_401_status.py
+-rw-r--r--   0        0        0     3006 2023-06-22 11:37:08.043378 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_404.py
+-rw-r--r--   0        0        0     2714 2023-06-22 11:37:08.035378 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_404_data.py
+-rw-r--r--   0        0        0      253 2023-06-22 11:37:04.647343 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_404_data_code.py
+-rw-r--r--   0        0        0      253 2023-06-22 11:37:04.519341 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_404_data_message.py
+-rw-r--r--   0        0        0      174 2023-06-22 11:37:04.431341 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_404_status.py
+-rw-r--r--   0        0        0     3006 2023-06-22 11:37:08.083379 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_500.py
+-rw-r--r--   0        0        0     2244 2023-06-22 11:37:08.115379 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_500_data.py
+-rw-r--r--   0        0        0      253 2023-06-22 11:37:04.511341 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_500_data_code.py
+-rw-r--r--   0        0        0      174 2023-06-22 11:37:04.755344 customgpt_client-1.0.4/custom_gpt_client/models/messages_response_500_status.py
+-rw-r--r--   0        0        0     4285 2023-06-22 11:37:08.183380 customgpt_client-1.0.4/custom_gpt_client/models/open_graph_cache.py
+-rw-r--r--   0        0        0     8656 2023-06-22 11:37:08.407382 customgpt_client-1.0.4/custom_gpt_client/models/page.py
+-rw-r--r--   0        0        0      217 2023-06-22 11:37:04.991346 customgpt_client-1.0.4/custom_gpt_client/models/page_crawl_status.py
+-rw-r--r--   0        0        0      217 2023-06-22 11:37:04.359340 customgpt_client-1.0.4/custom_gpt_client/models/page_index_status.py
+-rw-r--r--   0        0        0     2987 2023-06-22 11:37:08.347381 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_401.py
+-rw-r--r--   0        0        0     2250 2023-06-22 11:37:08.143379 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_401_data.py
+-rw-r--r--   0        0        0      252 2023-06-22 11:37:04.991346 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_401_data_code.py
+-rw-r--r--   0        0        0      173 2023-06-22 11:37:04.911346 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_401_status.py
+-rw-r--r--   0        0        0     2987 2023-06-22 11:37:08.239380 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_404.py
+-rw-r--r--   0        0        0     2697 2023-06-22 11:37:08.207380 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_404_data.py
+-rw-r--r--   0        0        0      252 2023-06-22 11:37:04.455341 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_404_data_code.py
+-rw-r--r--   0        0        0      252 2023-06-22 11:37:04.915346 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_404_data_message.py
+-rw-r--r--   0        0        0      173 2023-06-22 11:37:04.759344 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_404_status.py
+-rw-r--r--   0        0        0     2987 2023-06-22 11:37:08.235380 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_500.py
+-rw-r--r--   0        0        0     2233 2023-06-22 11:37:08.219380 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_500_data.py
+-rw-r--r--   0        0        0      252 2023-06-22 11:37:04.875345 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_500_data_code.py
+-rw-r--r--   0        0        0      173 2023-06-22 11:37:04.619342 customgpt_client-1.0.4/custom_gpt_client/models/preview_response_500_status.py
+-rw-r--r--   0        0        0     7789 2023-06-22 11:37:08.511383 customgpt_client-1.0.4/custom_gpt_client/models/project.py
+-rw-r--r--   0        0        0     3482 2023-06-22 11:37:08.291381 customgpt_client-1.0.4/custom_gpt_client/models/project_plugin.py
+-rw-r--r--   0        0        0     4467 2023-06-22 11:37:08.367382 customgpt_client-1.0.4/custom_gpt_client/models/project_settings.py
+-rw-r--r--   0        0        0      236 2023-06-22 11:37:05.027347 customgpt_client-1.0.4/custom_gpt_client/models/project_settings_response_source.py
+-rw-r--r--   0        0        0      156 2023-06-22 11:37:04.463341 customgpt_client-1.0.4/custom_gpt_client/models/project_type.py
+-rw-r--r--   0        0        0     5019 2023-06-22 11:37:08.427382 customgpt_client-1.0.4/custom_gpt_client/models/prompt_history.py
+-rw-r--r--   0        0        0     1654 2023-06-22 11:37:08.399382 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_json_body.py
+-rw-r--r--   0        0        0     3061 2023-06-22 11:37:08.379382 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_200.py
+-rw-r--r--   0        0        0     5169 2023-06-22 11:37:08.475383 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_200_data.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.803344 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_200_status.py
+-rw-r--r--   0        0        0     3347 2023-06-22 11:37:08.559384 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_401.py
+-rw-r--r--   0        0        0     2460 2023-06-22 11:37:08.471383 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_401_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.527341 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.555342 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_401_status.py
+-rw-r--r--   0        0        0     3347 2023-06-22 11:37:08.483383 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_404.py
+-rw-r--r--   0        0        0     3039 2023-06-22 11:37:08.559384 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_404_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.959346 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.555342 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.983346 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_404_status.py
+-rw-r--r--   0        0        0     3347 2023-06-22 11:37:08.619384 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_500.py
+-rw-r--r--   0        0        0     2443 2023-06-22 11:37:08.547384 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_500_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.659343 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:05.003347 customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_response_500_status.py
+-rw-r--r--   0        0        0     2802 2023-06-22 11:37:08.571384 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_200.py
+-rw-r--r--   0        0        0     3719 2023-06-22 11:37:08.683385 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_200_data.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.591342 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_200_status.py
+-rw-r--r--   0        0        0     3088 2023-06-22 11:37:08.635385 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_401.py
+-rw-r--r--   0        0        0     2309 2023-06-22 11:37:08.675385 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_401_data.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:04.515341 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.595342 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_401_status.py
+-rw-r--r--   0        0        0     3088 2023-06-22 11:37:08.659385 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_404.py
+-rw-r--r--   0        0        0     2787 2023-06-22 11:37:08.715386 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_404_data.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:04.487341 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_404_data_code.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:04.483341 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.343340 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_404_status.py
+-rw-r--r--   0        0        0     3088 2023-06-22 11:37:08.787386 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_500.py
+-rw-r--r--   0        0        0     2292 2023-06-22 11:37:08.703385 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_500_data.py
+-rw-r--r--   0        0        0      257 2023-06-22 11:37:04.455341 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2023-06-22 11:37:04.407340 customgpt_client-1.0.4/custom_gpt_client/models/stats_project_response_500_status.py
+-rw-r--r--   0        0        0     1628 2023-06-22 11:37:08.683385 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_json_body.py
+-rw-r--r--   0        0        0     3055 2023-06-22 11:37:08.715386 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_200.py
+-rw-r--r--   0        0        0     5033 2023-06-22 11:37:08.851387 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_200_data.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.591342 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_200_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:08.847387 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_401.py
+-rw-r--r--   0        0        0     2456 2023-06-22 11:37:08.787386 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_401_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.735344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.451341 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_401_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:08.867387 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_404.py
+-rw-r--r--   0        0        0     3034 2023-06-22 11:37:08.935388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_404_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.559342 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.467341 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.735344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_404_status.py
+-rw-r--r--   0        0        0     3341 2023-06-22 11:37:08.843387 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_500.py
+-rw-r--r--   0        0        0     2439 2023-06-22 11:37:08.799386 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_500_data.py
+-rw-r--r--   0        0        0      270 2023-06-22 11:37:04.967346 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:37:04.923346 customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_500_status.py
+-rw-r--r--   0        0        0     4948 2023-06-22 11:37:08.943388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_multipart_data.py
+-rw-r--r--   0        0        0     2821 2023-06-22 11:37:08.919388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_200.py
+-rw-r--r--   0        0        0     8090 2023-06-22 11:37:08.975388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_200_data.py
+-rw-r--r--   0        0        0      177 2023-06-22 11:37:04.731344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_200_data_type.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.875345 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_200_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:08.943388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_401.py
+-rw-r--r--   0        0        0     2320 2023-06-22 11:37:08.931388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.643343 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.527341 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_401_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:08.991388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_404.py
+-rw-r--r--   0        0        0     2816 2023-06-22 11:37:08.943388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_404_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.627343 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_404_data_code.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.787344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_404_data_message.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.659343 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_404_status.py
+-rw-r--r--   0        0        0     3107 2023-06-22 11:37:09.147390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_500.py
+-rw-r--r--   0        0        0     2303 2023-06-22 11:37:09.051389 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2023-06-22 11:37:04.351340 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2023-06-22 11:37:04.635343 customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_500_status.py
+-rw-r--r--   0        0        0     6861 2023-06-22 11:37:09.295391 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_multipart_data.py
+-rw-r--r--   0        0        0     2979 2023-06-22 11:37:09.019389 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_200.py
+-rw-r--r--   0        0        0     1680 2023-06-22 11:37:08.995388 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_200_data.py
+-rw-r--r--   0        0        0      187 2023-06-22 11:37:05.031347 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_200_status.py
+-rw-r--r--   0        0        0     3265 2023-06-22 11:37:09.159390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_400.py
+-rw-r--r--   0        0        0     2976 2023-06-22 11:37:09.047389 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_400_data.py
+-rw-r--r--   0        0        0      266 2023-06-22 11:37:04.363340 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_400_data_code.py
+-rw-r--r--   0        0        0      423 2023-06-22 11:37:04.547342 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_400_data_message.py
+-rw-r--r--   0        0        0      187 2023-06-22 11:37:04.775344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_400_status.py
+-rw-r--r--   0        0        0     3265 2023-06-22 11:37:09.187390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_401.py
+-rw-r--r--   0        0        0     2412 2023-06-22 11:37:09.179390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_401_data.py
+-rw-r--r--   0        0        0      266 2023-06-22 11:37:04.467341 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_401_data_code.py
+-rw-r--r--   0        0        0      187 2023-06-22 11:37:04.331339 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_401_status.py
+-rw-r--r--   0        0        0     3265 2023-06-22 11:37:09.115390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_500.py
+-rw-r--r--   0        0        0     2395 2023-06-22 11:37:09.155390 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_500_data.py
+-rw-r--r--   0        0        0      266 2023-06-22 11:37:04.915346 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_500_data_code.py
+-rw-r--r--   0        0        0      187 2023-06-22 11:37:04.755344 customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_response_500_status.py
+-rw-r--r--   0        0        0     3050 2023-06-22 11:37:09.155390 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_multipart_data.py
+-rw-r--r--   0        0        0     2903 2023-06-22 11:37:09.219391 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_200.py
+-rw-r--r--   0        0        0     3946 2023-06-22 11:37:09.311392 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_200_data.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.407340 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_200_status.py
+-rw-r--r--   0        0        0     3189 2023-06-22 11:37:09.255391 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_401.py
+-rw-r--r--   0        0        0     2368 2023-06-22 11:37:09.231391 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_401_data.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:05.035347 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_401_data_code.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.443341 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_401_status.py
+-rw-r--r--   0        0        0     3189 2023-06-22 11:37:09.331392 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_500.py
+-rw-r--r--   0        0        0     2351 2023-06-22 11:37:09.283391 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_500_data.py
+-rw-r--r--   0        0        0      262 2023-06-22 11:37:04.571342 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_500_data_code.py
+-rw-r--r--   0        0        0      183 2023-06-22 11:37:04.667343 customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_500_status.py
+-rw-r--r--   0        0        0     3791 2023-06-22 11:37:09.355392 customgpt_client-1.0.4/custom_gpt_client/models/user.py
+-rw-r--r--   0        0        0       25 2023-06-22 11:37:02.427319 customgpt_client-1.0.4/custom_gpt_client/py.typed
+-rw-r--r--   0        0        0      993 2023-06-22 11:37:09.251391 customgpt_client-1.0.4/custom_gpt_client/types.py
+-rw-r--r--   0        0        0      679 2023-06-22 11:45:59.942889 customgpt_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 customgpt_client-1.0.4/PKG-INFO
```

### Comparing `customgpt_client-1.0.3/README.md` & `customgpt_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/conversations/create_project_conversation.py` & `customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_404.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,95 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
-import httpx
+import attr
 
-from ... import errors
-from ...models.create_project_conversation_json_body import CreateProjectConversationJsonBody
-from ...types import Response
-
-
-def _get_kwargs(
-    project_id: int,
-    *,
-    client: {},
-    json_body: CreateProjectConversationJsonBody,
-) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectId}/conversations".format(client.base_url, projectId=project_id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
-    }
-
-
-def _parse_response(*, client: {}, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.CREATED:
-        return None
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        return None
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        return None
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        return None
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
-
-
-def _build_response(*, client: {}, response: httpx.Response, content: Optional[bytes] = None) -> Response[Any]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content if content is None else content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    project_id: int,
-    *,
-    client: {},
-    json_body: CreateProjectConversationJsonBody,
-):
-    """Create a new conversation.
-
-     Create a new conversation for a project by `projectId`.
-
-    Args:
-        project_id (int):
-        json_body (CreateProjectConversationJsonBody):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+from ..models.create_project_conversation_response_404_status import CreateProjectConversationResponse404Status
+from ..types import UNSET, Unset
 
-    Returns:
-        Response[Any]
-    """
+if TYPE_CHECKING:
+    from ..models.create_project_conversation_response_404_data import CreateProjectConversationResponse404Data
+
+
+T = TypeVar("T", bound="CreateProjectConversationResponse404")
 
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        client=client,
-        json_body=json_body,
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
-async def asyncio_detailed(
-    project_id: int,
-    *,
-    client: {},
-    json_body: CreateProjectConversationJsonBody,
-) -> Response[Any]:
-    """Create a new conversation.
-
-     Create a new conversation for a project by `projectId`.
-
-    Args:
-        project_id (int):
-        json_body (CreateProjectConversationJsonBody):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
-    Returns:
-        Response[Any]
+@attr.s(auto_attribs=True)
+class CreateProjectConversationResponse404:
     """
+    Attributes:
+        status (Union[Unset, CreateProjectConversationResponse404Status]): The status of the response Example: error.
+        url (Union[Unset, str]): The URL of the request Example: https://app.customgpt.ai/api/v1/projects/1.
+        data (Union[Unset, CreateProjectConversationResponse404Data]):
+    """
+
+    status: Union[Unset, CreateProjectConversationResponse404Status] = UNSET
+    url: Union[Unset, str] = UNSET
+    data: Union[Unset, "CreateProjectConversationResponse404Data"] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
+        url = self.url
+        data: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data, Unset):
+            data = self.data.to_dict()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if status is not UNSET:
+            field_dict["status"] = status
+        if url is not UNSET:
+            field_dict["url"] = url
+        if data is not UNSET:
+            field_dict["data"] = data
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.create_project_conversation_response_404_data import CreateProjectConversationResponse404Data
+
+        d = src_dict.copy()
+        _status = d.pop("status", UNSET)
+        status: Union[Unset, CreateProjectConversationResponse404Status]
+        if isinstance(_status, Unset):
+            status = UNSET
+        else:
+            status = CreateProjectConversationResponse404Status(_status)
+
+        url = d.pop("url", UNSET)
+
+        _data = d.pop("data", UNSET)
+        data: Union[Unset, CreateProjectConversationResponse404Data]
+        if isinstance(_data, Unset):
+            data = UNSET
+        else:
+            data = CreateProjectConversationResponse404Data.from_dict(_data)
+
+        create_project_conversation_response_404 = cls(
+            status=status,
+            url=url,
+            data=data,
+        )
+
+        create_project_conversation_response_404.additional_properties = d
+        return create_project_conversation_response_404
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
 
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        client=client,
-        json_body=json_body,
-    )
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
 
-    return _build_response(client=client, response=response)
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/conversations/get_project_conversations.py` & `customgpt_client-1.0.4/custom_gpt_client/api/projects/get_project.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...models.get_project_conversations_order import GetProjectConversationsOrder
-from ...models.get_project_conversations_response_200 import GetProjectConversationsResponse200
+from ...models.get_project_response_200 import GetProjectResponse200
+from ...models.get_project_response_401 import GetProjectResponse401
+from ...models.get_project_response_404 import GetProjectResponse404
+from ...models.get_project_response_500 import GetProjectResponse500
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     project_id: int,
     *,
     client: {},
-    page: Union[Unset, None, int] = 1,
-    order: Union[Unset, None, GetProjectConversationsOrder] = GetProjectConversationsOrder.DESC,
+    width: Union[Unset, None, str] = "100%",
+    height: Union[Unset, None, str] = "auto",
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectId}/conversations".format(client.base_url, projectId=project_id)
+    url = "{}/api/v1/projects/{projectId}".format(client.base_url, projectId=project_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["page"] = page
+    params["width"] = width
 
-    json_order: Union[Unset, None, str] = UNSET
-    if not isinstance(order, Unset):
-        json_order = order.value if order else None
-
-    params["order"] = json_order
+    params["height"] = height
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
@@ -41,178 +39,182 @@
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: {}, response: httpx.Response
-) -> Optional[Union[Any, GetProjectConversationsResponse200]]:
+) -> Optional[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectConversationsResponse200.from_dict(response.json())
+        response_200 = GetProjectResponse200.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
+        response_401 = GetProjectResponse401.from_dict(response.json())
+
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
+        response_404 = GetProjectResponse404.from_dict(response.json())
+
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = cast(Any, None)
+        response_500 = GetProjectResponse500.from_dict(response.json())
+
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: {}, response: httpx.Response, content: Optional[bytes] = None
-) -> Response[Union[Any, GetProjectConversationsResponse200]]:
+) -> Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
 def sync_detailed(
     project_id: int,
     *,
     client: {},
-    page: Union[Unset, None, int] = 1,
-    order: Union[Unset, None, GetProjectConversationsOrder] = GetProjectConversationsOrder.DESC,
+    width: Union[Unset, None, str] = "100%",
+    height: Union[Unset, None, str] = "auto",
 ):
-    """List all conversations for a project
-    Retrieve all conversations for a project by `projectId`.
+    """Show a certain project.
+
+     View a specific project by project ID.
 
     Args:
         project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, GetProjectConversationsOrder]):  Default:
-            GetProjectConversationsOrder.DESC. Example: desc.
+        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
+        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, GetProjectConversationsResponse200]]
+        Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
-        page=page,
-        order=order,
+        width=width,
+        height=height,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_id: int,
     *,
     client: {},
-    page: Union[Unset, None, int] = 1,
-    order: Union[Unset, None, GetProjectConversationsOrder] = GetProjectConversationsOrder.DESC,
-) -> Optional[Union[Any, GetProjectConversationsResponse200]]:
-    """List all conversations for a project
-    Retrieve all conversations for a project by `projectId`.
+    width: Union[Unset, None, str] = "100%",
+    height: Union[Unset, None, str] = "auto",
+) -> Optional[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
+    """Show a certain project.
+
+     View a specific project by project ID.
 
     Args:
         project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, GetProjectConversationsOrder]):  Default:
-            GetProjectConversationsOrder.DESC. Example: desc.
+        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
+        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, GetProjectConversationsResponse200]
+        Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
-        page=page,
-        order=order,
+        width=width,
+        height=height,
     ).parsed
 
 
 async def asyncio_detailed(
     project_id: int,
     *,
     client: {},
-    page: Union[Unset, None, int] = 1,
-    order: Union[Unset, None, GetProjectConversationsOrder] = GetProjectConversationsOrder.DESC,
-) -> Response[Union[Any, GetProjectConversationsResponse200]]:
-    """List all conversations for a project
-    Retrieve all conversations for a project by `projectId`.
+    width: Union[Unset, None, str] = "100%",
+    height: Union[Unset, None, str] = "auto",
+) -> Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
+    """Show a certain project.
+
+     View a specific project by project ID.
 
     Args:
         project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, GetProjectConversationsOrder]):  Default:
-            GetProjectConversationsOrder.DESC. Example: desc.
+        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
+        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, GetProjectConversationsResponse200]]
+        Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
-        page=page,
-        order=order,
+        width=width,
+        height=height,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
     client: {},
-    page: Union[Unset, None, int] = 1,
-    order: Union[Unset, None, GetProjectConversationsOrder] = GetProjectConversationsOrder.DESC,
-) -> Optional[Union[Any, GetProjectConversationsResponse200]]:
-    """List all conversations for a project
-    Retrieve all conversations for a project by `projectId`.
+    width: Union[Unset, None, str] = "100%",
+    height: Union[Unset, None, str] = "auto",
+) -> Optional[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
+    """Show a certain project.
+
+     View a specific project by project ID.
 
     Args:
         project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, GetProjectConversationsOrder]):  Default:
-            GetProjectConversationsOrder.DESC. Example: desc.
+        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
+        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, GetProjectConversationsResponse200]
+        Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
-            page=page,
-            order=order,
+            width=width,
+            height=height,
         )
     ).parsed
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/conversations/send_message_to_conversation.py` & `customgpt_client-1.0.4/custom_gpt_client/api/conversations/create_project_conversation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,238 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...models.send_message_to_conversation_json_body import SendMessageToConversationJsonBody
-from ...types import UNSET, Response, Unset
+from ...models.create_project_conversation_json_body import CreateProjectConversationJsonBody
+from ...models.create_project_conversation_response_201 import CreateProjectConversationResponse201
+from ...models.create_project_conversation_response_401 import CreateProjectConversationResponse401
+from ...models.create_project_conversation_response_404 import CreateProjectConversationResponse404
+from ...models.create_project_conversation_response_500 import CreateProjectConversationResponse500
+from ...types import Response
 
 
 def _get_kwargs(
     project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
+    json_body: CreateProjectConversationJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectId}/conversations/{sessionId}/messages".format(
-        client.base_url, projectId=project_id, sessionId=session_id
-    )
+    url = "{}/api/v1/projects/{projectId}/conversations".format(client.base_url, projectId=project_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["stream"] = stream
-
-    params["lang"] = lang
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     json_json_body = json_body.to_dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
-        "params": params,
     }
 
 
-def _parse_response(*, client: {}, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.OK:
-        return None
+def _parse_response(
+    *, client: {}, response: httpx.Response
+) -> Optional[
+    Union[
+        CreateProjectConversationResponse201,
+        CreateProjectConversationResponse401,
+        CreateProjectConversationResponse404,
+        CreateProjectConversationResponse500,
+    ]
+]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = CreateProjectConversationResponse201.from_dict(response.json())
+
+        return response_201
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        return None
+        response_401 = CreateProjectConversationResponse401.from_dict(response.json())
+
+        return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        return None
+        response_404 = CreateProjectConversationResponse404.from_dict(response.json())
+
+        return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        return None
+        response_500 = CreateProjectConversationResponse500.from_dict(response.json())
+
+        return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: {}, response: httpx.Response, content: Optional[bytes] = None) -> Response[Any]:
+def _build_response(
+    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+) -> Response[
+    Union[
+        CreateProjectConversationResponse201,
+        CreateProjectConversationResponse401,
+        CreateProjectConversationResponse404,
+        CreateProjectConversationResponse500,
+    ]
+]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
-def stream_detailed(
+def sync_detailed(
     project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-) -> Response[Any]:
-    """Send a message to a conversation.
+    json_body: CreateProjectConversationJsonBody,
+):
+    """Create a new conversation.
 
-     Send a message to a conversation by `projectId` and `sessionId`.
+     Create a new conversation for a project by `projectId`.
 
     Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        stream (Union[Unset, None, bool]):
-        lang (Union[Unset, None, str]):  Default: 'en'.
-        json_body (SendMessageToConversationJsonBody):
+        project_id (int):
+        json_body (CreateProjectConversationJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[Union[CreateProjectConversationResponse201, CreateProjectConversationResponse401, CreateProjectConversationResponse404, CreateProjectConversationResponse500]]
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
-        session_id=session_id,
         client=client,
         json_body=json_body,
-        stream=stream,
-        lang=lang,
     )
 
-    response = httpx.request(**kwargs)
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
 
-    lines = response.iter_lines()
-    while True:
-        try:
-            line = next(lines)
-            yield _build_response(client=client, response=response, content=line)
-        except StopIteration:
-            break
+    return _build_response(client=client, response=response)
 
 
-async def astream_detailed(
+def sync(
     project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-):
-    kwargs = _get_kwargs(
+    json_body: CreateProjectConversationJsonBody,
+) -> Optional[
+    Union[
+        CreateProjectConversationResponse201,
+        CreateProjectConversationResponse401,
+        CreateProjectConversationResponse404,
+        CreateProjectConversationResponse500,
+    ]
+]:
+    """Create a new conversation.
+
+     Create a new conversation for a project by `projectId`.
+
+    Args:
+        project_id (int):
+        json_body (CreateProjectConversationJsonBody):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[CreateProjectConversationResponse201, CreateProjectConversationResponse401, CreateProjectConversationResponse404, CreateProjectConversationResponse500]
+    """
+
+    return sync_detailed(
         project_id=project_id,
-        session_id=session_id,
         client=client,
         json_body=json_body,
-        stream=stream,
-        lang=lang,
-    )
-    async with httpx.AsyncClient() as client:
-        async with client.stream(**kwargs) as response:
-            async for chunk in response.aiter_raw():
-                yield _build_response(client=client, response=response, content=chunk)
+    ).parsed
 
 
-def sync_detailed(
+async def asyncio_detailed(
     project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-):
-    if stream:
-        return list(
-            stream_detailed(
-                project_id=project_id,
-                session_id=session_id,
-                client=client,
-                json_body=json_body,
-                stream=stream,
-                lang=lang,
-            )
-        )
-    """ Send a message to a conversation.
+    json_body: CreateProjectConversationJsonBody,
+) -> Response[
+    Union[
+        CreateProjectConversationResponse201,
+        CreateProjectConversationResponse401,
+        CreateProjectConversationResponse404,
+        CreateProjectConversationResponse500,
+    ]
+]:
+    """Create a new conversation.
 
-     Send a message to a conversation by `projectId` and `sessionId`.
+     Create a new conversation for a project by `projectId`.
 
     Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        stream (Union[Unset, None, bool]):
-        lang (Union[Unset, None, str]):  Default: 'en'.
-        json_body (SendMessageToConversationJsonBody):
+        project_id (int):
+        json_body (CreateProjectConversationJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
-     """
+        Response[Union[CreateProjectConversationResponse201, CreateProjectConversationResponse401, CreateProjectConversationResponse404, CreateProjectConversationResponse500]]
+    """
 
     kwargs = _get_kwargs(
         project_id=project_id,
-        session_id=session_id,
         client=client,
         json_body=json_body,
-        stream=stream,
-        lang=lang,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio_detailed(
+async def asyncio(
     project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-) -> Response[Any]:
-    if stream:
-        return astream_detailed(
-            project_id=project_id,
-            session_id=session_id,
-            client=client,
-            json_body=json_body,
-            stream=stream,
-            lang=lang,
-        )
-    """ Send a message to a conversation.
+    json_body: CreateProjectConversationJsonBody,
+) -> Optional[
+    Union[
+        CreateProjectConversationResponse201,
+        CreateProjectConversationResponse401,
+        CreateProjectConversationResponse404,
+        CreateProjectConversationResponse500,
+    ]
+]:
+    """Create a new conversation.
 
-     Send a message to a conversation by `projectId` and `sessionId`.
+     Create a new conversation for a project by `projectId`.
 
     Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        stream (Union[Unset, None, bool]):
-        lang (Union[Unset, None, str]):  Default: 'en'.
-        json_body (SendMessageToConversationJsonBody):
+        project_id (int):
+        json_body (CreateProjectConversationJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
-     """
-
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
-        client=client,
-        json_body=json_body,
-        stream=stream,
-        lang=lang,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+        Union[CreateProjectConversationResponse201, CreateProjectConversationResponse401, CreateProjectConversationResponse404, CreateProjectConversationResponse500]
+    """
 
-    return _build_response(client=client, response=response)
+    return (
+        await asyncio_detailed(
+            project_id=project_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/conversations/update_project_conversation.py` & `customgpt_client-1.0.4/custom_gpt_client/api/projects/create_project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,211 +1,200 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...models.update_project_conversation_json_body import UpdateProjectConversationJsonBody
-from ...models.update_project_conversation_response_200 import UpdateProjectConversationResponse200
+from ...models.create_project_multipart_data import CreateProjectMultipartData
+from ...models.create_project_response_201 import CreateProjectResponse201
+from ...models.create_project_response_400 import CreateProjectResponse400
+from ...models.create_project_response_401 import CreateProjectResponse401
+from ...models.create_project_response_500 import CreateProjectResponse500
 from ...types import Response
 
 
 def _get_kwargs(
-    project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: UpdateProjectConversationJsonBody,
+    multipart_data: CreateProjectMultipartData,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectId}/conversations/{sessionId}".format(
-        client.base_url, projectId=project_id, sessionId=session_id
-    )
+    url = "{}/api/v1/projects".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    multipart_multipart_data = multipart_data.to_multipart()
 
     return {
-        "method": "put",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
+        "files": multipart_multipart_data,
     }
 
 
 def _parse_response(
     *, client: {}, response: httpx.Response
-) -> Optional[Union[Any, UpdateProjectConversationResponse200]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateProjectConversationResponse200.from_dict(response.json())
+) -> Optional[
+    Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
+]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = CreateProjectResponse201.from_dict(response.json())
+
+        return response_201
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = CreateProjectResponse400.from_dict(response.json())
 
-        return response_200
+        return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
+        response_401 = CreateProjectResponse401.from_dict(response.json())
+
         return response_401
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
-        return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = cast(Any, None)
+        response_500 = CreateProjectResponse500.from_dict(response.json())
+
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: {}, response: httpx.Response, content: Optional[bytes] = None
-) -> Response[Union[Any, UpdateProjectConversationResponse200]]:
+) -> Response[
+    Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
+]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
 def sync_detailed(
-    project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: UpdateProjectConversationJsonBody,
+    multipart_data: CreateProjectMultipartData,
 ):
-    """Update a conversation.
+    """Create a new project.
 
-     Update a conversation by `projectId` and `sessionId`.
+     Create a new project from either sitemap or uploaded file.
 
     Args:
-        project_id (int):
-        session_id (str):
-        json_body (UpdateProjectConversationJsonBody):
+        multipart_data (CreateProjectMultipartData):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, UpdateProjectConversationResponse200]]
+        Response[Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]]
     """
 
     kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
         client=client,
-        json_body=json_body,
+        multipart_data=multipart_data,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: UpdateProjectConversationJsonBody,
-) -> Optional[Union[Any, UpdateProjectConversationResponse200]]:
-    """Update a conversation.
+    multipart_data: CreateProjectMultipartData,
+) -> Optional[
+    Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
+]:
+    """Create a new project.
 
-     Update a conversation by `projectId` and `sessionId`.
+     Create a new project from either sitemap or uploaded file.
 
     Args:
-        project_id (int):
-        session_id (str):
-        json_body (UpdateProjectConversationJsonBody):
+        multipart_data (CreateProjectMultipartData):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, UpdateProjectConversationResponse200]
+        Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
     """
 
     return sync_detailed(
-        project_id=project_id,
-        session_id=session_id,
         client=client,
-        json_body=json_body,
+        multipart_data=multipart_data,
     ).parsed
 
 
 async def asyncio_detailed(
-    project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: UpdateProjectConversationJsonBody,
-) -> Response[Union[Any, UpdateProjectConversationResponse200]]:
-    """Update a conversation.
+    multipart_data: CreateProjectMultipartData,
+) -> Response[
+    Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
+]:
+    """Create a new project.
 
-     Update a conversation by `projectId` and `sessionId`.
+     Create a new project from either sitemap or uploaded file.
 
     Args:
-        project_id (int):
-        session_id (str):
-        json_body (UpdateProjectConversationJsonBody):
+        multipart_data (CreateProjectMultipartData):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, UpdateProjectConversationResponse200]]
+        Response[Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]]
     """
 
     kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
         client=client,
-        json_body=json_body,
+        multipart_data=multipart_data,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    project_id: int,
-    session_id: str,
     *,
     client: {},
-    json_body: UpdateProjectConversationJsonBody,
-) -> Optional[Union[Any, UpdateProjectConversationResponse200]]:
-    """Update a conversation.
+    multipart_data: CreateProjectMultipartData,
+) -> Optional[
+    Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
+]:
+    """Create a new project.
 
-     Update a conversation by `projectId` and `sessionId`.
+     Create a new project from either sitemap or uploaded file.
 
     Args:
-        project_id (int):
-        session_id (str):
-        json_body (UpdateProjectConversationJsonBody):
+        multipart_data (CreateProjectMultipartData):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, UpdateProjectConversationResponse200]
+        Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
     """
 
     return (
         await asyncio_detailed(
-            project_id=project_id,
-            session_id=session_id,
             client=client,
-            json_body=json_body,
+            multipart_data=multipart_data,
         )
     ).parsed
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/pages/get_project_pages.py` & `customgpt_client-1.0.4/custom_gpt_client/api/pages/get_project_pages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...models.get_project_pages_order import GetProjectPagesOrder
 from ...models.get_project_pages_response_200 import GetProjectPagesResponse200
+from ...models.get_project_pages_response_401 import GetProjectPagesResponse401
+from ...models.get_project_pages_response_404 import GetProjectPagesResponse404
+from ...models.get_project_pages_response_500 import GetProjectPagesResponse500
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     project_id: int,
     *,
     client: {},
@@ -42,42 +45,56 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: {}, response: httpx.Response) -> Optional[Union[Any, GetProjectPagesResponse200]]:
+def _parse_response(
+    *, client: {}, response: httpx.Response
+) -> Optional[
+    Union[
+        GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
+    ]
+]:
     if response.status_code == HTTPStatus.OK:
         response_200 = GetProjectPagesResponse200.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
+        response_401 = GetProjectPagesResponse401.from_dict(response.json())
+
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = cast(Any, None)
+        response_404 = GetProjectPagesResponse404.from_dict(response.json())
+
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = cast(Any, None)
+        response_500 = GetProjectPagesResponse500.from_dict(response.json())
+
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: {}, response: httpx.Response, content: Optional[bytes] = None
-) -> Response[Union[Any, GetProjectPagesResponse200]]:
+) -> Response[
+    Union[
+        GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
+    ]
+]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
 def sync_detailed(
     project_id: int,
     *,
     client: {},
@@ -96,15 +113,15 @@
         order (Union[Unset, None, GetProjectPagesOrder]):  Default: GetProjectPagesOrder.DESC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, GetProjectPagesResponse200]]
+        Response[Union[GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500]]
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         page=page,
         duration=duration,
@@ -122,15 +139,19 @@
 def sync(
     project_id: int,
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, GetProjectPagesOrder] = GetProjectPagesOrder.DESC,
-) -> Optional[Union[Any, GetProjectPagesResponse200]]:
+) -> Optional[
+    Union[
+        GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
+    ]
+]:
     """List all pages that belong to a project.
 
      Get a list of all pages that belong to a project.
 
     Args:
         project_id (int):  Example: 1.
         page (Union[Unset, None, int]):  Default: 1.
@@ -138,15 +159,15 @@
         order (Union[Unset, None, GetProjectPagesOrder]):  Default: GetProjectPagesOrder.DESC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, GetProjectPagesResponse200]
+        Union[GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500]
     """
 
     return sync_detailed(
         project_id=project_id,
         client=client,
         page=page,
         duration=duration,
@@ -157,15 +178,19 @@
 async def asyncio_detailed(
     project_id: int,
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, GetProjectPagesOrder] = GetProjectPagesOrder.DESC,
-) -> Response[Union[Any, GetProjectPagesResponse200]]:
+) -> Response[
+    Union[
+        GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
+    ]
+]:
     """List all pages that belong to a project.
 
      Get a list of all pages that belong to a project.
 
     Args:
         project_id (int):  Example: 1.
         page (Union[Unset, None, int]):  Default: 1.
@@ -173,15 +198,15 @@
         order (Union[Unset, None, GetProjectPagesOrder]):  Default: GetProjectPagesOrder.DESC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, GetProjectPagesResponse200]]
+        Response[Union[GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500]]
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         page=page,
         duration=duration,
@@ -197,15 +222,19 @@
 async def asyncio(
     project_id: int,
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, GetProjectPagesOrder] = GetProjectPagesOrder.DESC,
-) -> Optional[Union[Any, GetProjectPagesResponse200]]:
+) -> Optional[
+    Union[
+        GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
+    ]
+]:
     """List all pages that belong to a project.
 
      Get a list of all pages that belong to a project.
 
     Args:
         project_id (int):  Example: 1.
         page (Union[Unset, None, int]):  Default: 1.
@@ -213,15 +242,15 @@
         order (Union[Unset, None, GetProjectPagesOrder]):  Default: GetProjectPagesOrder.DESC.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, GetProjectPagesResponse200]
+        Union[GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500]
     """
 
     return (
         await asyncio_detailed(
             project_id=project_id,
             client=client,
             page=page,
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/projects/list_projects.py` & `customgpt_client-1.0.4/custom_gpt_client/api/projects/list_projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...models.list_projects_order import ListProjectsOrder
 from ...models.list_projects_response_200 import ListProjectsResponse200
+from ...models.list_projects_response_401 import ListProjectsResponse401
+from ...models.list_projects_response_500 import ListProjectsResponse500
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
@@ -47,39 +49,44 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: {}, response: httpx.Response) -> Optional[Union[Any, ListProjectsResponse200]]:
+def _parse_response(
+    *, client: {}, response: httpx.Response
+) -> Optional[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = ListProjectsResponse200.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
+        response_401 = ListProjectsResponse401.from_dict(response.json())
+
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = cast(Any, None)
+        response_500 = ListProjectsResponse500.from_dict(response.json())
+
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: {}, response: httpx.Response, content: Optional[bytes] = None
-) -> Response[Union[Any, ListProjectsResponse200]]:
+) -> Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
 def sync_detailed(
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
@@ -100,15 +107,15 @@
         height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ListProjectsResponse200]]
+        Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         page=page,
         duration=duration,
         order=order,
@@ -128,15 +135,15 @@
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, ListProjectsOrder] = ListProjectsOrder.DESC,
     width: Union[Unset, None, str] = "100%",
     height: Union[Unset, None, str] = "auto",
-) -> Optional[Union[Any, ListProjectsResponse200]]:
+) -> Optional[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     """List all projects.
 
      Get a list of all projects that belong to the user.
 
     Args:
         page (Union[Unset, None, int]):  Default: 1.
         duration (Union[Unset, None, int]):  Default: 90.
@@ -145,15 +152,15 @@
         height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, ListProjectsResponse200]
+        Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]
     """
 
     return sync_detailed(
         client=client,
         page=page,
         duration=duration,
         order=order,
@@ -166,15 +173,15 @@
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, ListProjectsOrder] = ListProjectsOrder.DESC,
     width: Union[Unset, None, str] = "100%",
     height: Union[Unset, None, str] = "auto",
-) -> Response[Union[Any, ListProjectsResponse200]]:
+) -> Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     """List all projects.
 
      Get a list of all projects that belong to the user.
 
     Args:
         page (Union[Unset, None, int]):  Default: 1.
         duration (Union[Unset, None, int]):  Default: 90.
@@ -183,15 +190,15 @@
         height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ListProjectsResponse200]]
+        Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         page=page,
         duration=duration,
         order=order,
@@ -209,15 +216,15 @@
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, ListProjectsOrder] = ListProjectsOrder.DESC,
     width: Union[Unset, None, str] = "100%",
     height: Union[Unset, None, str] = "auto",
-) -> Optional[Union[Any, ListProjectsResponse200]]:
+) -> Optional[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     """List all projects.
 
      Get a list of all projects that belong to the user.
 
     Args:
         page (Union[Unset, None, int]):  Default: 1.
         duration (Union[Unset, None, int]):  Default: 90.
@@ -226,15 +233,15 @@
         height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, ListProjectsResponse200]
+        Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             page=page,
             duration=duration,
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/api/users/update_user_profile.py` & `customgpt_client-1.0.4/custom_gpt_client/api/pages/preview.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,178 +1,173 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...models.update_user_profile_multipart_data import UpdateUserProfileMultipartData
-from ...models.update_user_profile_response_200 import UpdateUserProfileResponse200
+from ...models.preview_response_401 import PreviewResponse401
+from ...models.preview_response_404 import PreviewResponse404
+from ...models.preview_response_500 import PreviewResponse500
 from ...types import Response
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: {},
-    multipart_data: UpdateUserProfileMultipartData,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/user".format(client.base_url)
+    url = "{}/api/v1/preview/{id}".format(client.base_url, id=id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    multipart_multipart_data = multipart_data.to_multipart()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "files": multipart_multipart_data,
     }
 
 
-def _parse_response(*, client: {}, response: httpx.Response) -> Optional[Union[Any, UpdateUserProfileResponse200]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateUserProfileResponse200.from_dict(response.json())
-
-        return response_200
+def _parse_response(
+    *, client: {}, response: httpx.Response
+) -> Optional[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = cast(Any, None)
+        response_401 = PreviewResponse401.from_dict(response.json())
+
         return response_401
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = PreviewResponse404.from_dict(response.json())
+
+        return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = cast(Any, None)
+        response_500 = PreviewResponse500.from_dict(response.json())
+
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: {}, response: httpx.Response, content: Optional[bytes] = None
-) -> Response[Union[Any, UpdateUserProfileResponse200]]:
+) -> Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
+        parsed=parse,
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: {},
-    multipart_data: UpdateUserProfileMultipartData,
 ):
-    """Update the user's profile.
-
-     Update the current user's profile.
+    """Preview file from citation.
 
     Args:
-        multipart_data (UpdateUserProfileMultipartData):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, UpdateUserProfileResponse200]]
+        Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
-        multipart_data=multipart_data,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    id: str,
     *,
     client: {},
-    multipart_data: UpdateUserProfileMultipartData,
-) -> Optional[Union[Any, UpdateUserProfileResponse200]]:
-    """Update the user's profile.
-
-     Update the current user's profile.
+) -> Optional[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
+    """Preview file from citation.
 
     Args:
-        multipart_data (UpdateUserProfileMultipartData):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, UpdateUserProfileResponse200]
+        Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]
     """
 
     return sync_detailed(
+        id=id,
         client=client,
-        multipart_data=multipart_data,
     ).parsed
 
 
 async def asyncio_detailed(
+    id: str,
     *,
     client: {},
-    multipart_data: UpdateUserProfileMultipartData,
-) -> Response[Union[Any, UpdateUserProfileResponse200]]:
-    """Update the user's profile.
-
-     Update the current user's profile.
+) -> Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
+    """Preview file from citation.
 
     Args:
-        multipart_data (UpdateUserProfileMultipartData):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, UpdateUserProfileResponse200]]
+        Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]
     """
 
     kwargs = _get_kwargs(
+        id=id,
         client=client,
-        multipart_data=multipart_data,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    id: str,
     *,
     client: {},
-    multipart_data: UpdateUserProfileMultipartData,
-) -> Optional[Union[Any, UpdateUserProfileResponse200]]:
-    """Update the user's profile.
-
-     Update the current user's profile.
+) -> Optional[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
+    """Preview file from citation.
 
     Args:
-        multipart_data (UpdateUserProfileMultipartData):
+        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Any, UpdateUserProfileResponse200]
+        Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]
     """
 
     return (
         await asyncio_detailed(
+            id=id,
             client=client,
-            multipart_data=multipart_data,
         )
     ).parsed
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/conversation.py` & `customgpt_client-1.0.4/custom_gpt_client/models/conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/create_project_conversation_json_body.py` & `customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/create_project_multipart_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/create_project_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_open_graph_data_for_citation_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_open_graph_data_for_citation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_open_graph_data_for_citation_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_200_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.open_graph_cache import OpenGraphCache
-
-
-T = TypeVar("T", bound="GetOpenGraphDataForCitationResponse200Data")
+T = TypeVar("T", bound="DeleteProjectResponse200Data")
 
 
 @attr.s(auto_attribs=True)
-class GetOpenGraphDataForCitationResponse200Data:
+class DeleteProjectResponse200Data:
     """
     Attributes:
-        open_graph_cache_schema (Union[Unset, OpenGraphCache]):
+        deleted (Union[Unset, bool]): Whether the project was deleted successfully or not Example: True.
     """
 
-    open_graph_cache_schema: Union[Unset, "OpenGraphCache"] = UNSET
+    deleted: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        open_graph_cache_schema: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.open_graph_cache_schema, Unset):
-            open_graph_cache_schema = self.open_graph_cache_schema.to_dict()
+        deleted = self.deleted
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if open_graph_cache_schema is not UNSET:
-            field_dict["OpenGraphCacheSchema"] = open_graph_cache_schema
+        if deleted is not UNSET:
+            field_dict["deleted"] = deleted
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.open_graph_cache import OpenGraphCache
-
         d = src_dict.copy()
-        _open_graph_cache_schema = d.pop("OpenGraphCacheSchema", UNSET)
-        open_graph_cache_schema: Union[Unset, OpenGraphCache]
-        if isinstance(_open_graph_cache_schema, Unset):
-            open_graph_cache_schema = UNSET
-        else:
-            open_graph_cache_schema = OpenGraphCache.from_dict(_open_graph_cache_schema)
+        deleted = d.pop("deleted", UNSET)
 
-        get_open_graph_data_for_citation_response_200_data = cls(
-            open_graph_cache_schema=open_graph_cache_schema,
+        delete_project_response_200_data = cls(
+            deleted=deleted,
         )
 
-        get_open_graph_data_for_citation_response_200_data.additional_properties = d
-        return get_open_graph_data_for_citation_response_200_data
+        delete_project_response_200_data.additional_properties = d
+        return delete_project_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.conversation import Conversation
+    from ..models.get_project_conversations_response_200_data_data_item import (
+        GetProjectConversationsResponse200DataDataItem,
+    )
     from ..models.get_project_conversations_response_200_data_links import GetProjectConversationsResponse200DataLinks
 
 
 T = TypeVar("T", bound="GetProjectConversationsResponse200Data")
 
 
 @attr.s(auto_attribs=True)
 class GetProjectConversationsResponse200Data:
     """
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
-        data (Union[Unset, List['Conversation']]):
+        data (Union[Unset, List['GetProjectConversationsResponse200DataDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         links (Union[Unset, GetProjectConversationsResponse200DataLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
-    data: Union[Unset, List["Conversation"]] = UNSET
+    data: Union[Unset, List["GetProjectConversationsResponse200DataDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
     links: Union[Unset, "GetProjectConversationsResponse200DataLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
@@ -102,26 +104,28 @@
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.conversation import Conversation
+        from ..models.get_project_conversations_response_200_data_data_item import (
+            GetProjectConversationsResponse200DataDataItem,
+        )
         from ..models.get_project_conversations_response_200_data_links import (
             GetProjectConversationsResponse200DataLinks,
         )
 
         d = src_dict.copy()
         current_page = d.pop("current_page", UNSET)
 
         data = []
         _data = d.pop("data", UNSET)
         for data_item_data in _data or []:
-            data_item = Conversation.from_dict(data_item_data)
+            data_item = GetProjectConversationsResponse200DataDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
         first_page_url = d.pop("first_page_url", UNSET)
 
         from_ = d.pop("from", UNSET)
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_conversations_response_200_data_links.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_200_data_links.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/create_project_conversation_response_401_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.create_project_conversation_response_401_data_code import CreateProjectConversationResponse401DataCode
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.get_project_pages_response_200_data_pages import GetProjectPagesResponse200DataPages
-    from ..models.project import Project
-
-
-T = TypeVar("T", bound="GetProjectPagesResponse200Data")
+T = TypeVar("T", bound="CreateProjectConversationResponse401Data")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectPagesResponse200Data:
+class CreateProjectConversationResponse401Data:
     """
     Attributes:
-        project (Union[Unset, Project]):
-        pages (Union[Unset, GetProjectPagesResponse200DataPages]):
+        code (Union[Unset, CreateProjectConversationResponse401DataCode]): The error status code Example: 401.
+        message (Union[Unset, str]):  Example: API Token is either missing or invalid.
     """
 
-    project: Union[Unset, "Project"] = UNSET
-    pages: Union[Unset, "GetProjectPagesResponse200DataPages"] = UNSET
+    code: Union[Unset, CreateProjectConversationResponse401DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        project: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.project, Unset):
-            project = self.project.to_dict()
-
-        pages: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.pages, Unset):
-            pages = self.pages.to_dict()
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if project is not UNSET:
-            field_dict["project"] = project
-        if pages is not UNSET:
-            field_dict["pages"] = pages
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.get_project_pages_response_200_data_pages import GetProjectPagesResponse200DataPages
-        from ..models.project import Project
-
         d = src_dict.copy()
-        _project = d.pop("project", UNSET)
-        project: Union[Unset, Project]
-        if isinstance(_project, Unset):
-            project = UNSET
+        _code = d.pop("code", UNSET)
+        code: Union[Unset, CreateProjectConversationResponse401DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
         else:
-            project = Project.from_dict(_project)
+            code = CreateProjectConversationResponse401DataCode(_code)
 
-        _pages = d.pop("pages", UNSET)
-        pages: Union[Unset, GetProjectPagesResponse200DataPages]
-        if isinstance(_pages, Unset):
-            pages = UNSET
-        else:
-            pages = GetProjectPagesResponse200DataPages.from_dict(_pages)
+        message = d.pop("message", UNSET)
 
-        get_project_pages_response_200_data = cls(
-            project=project,
-            pages=pages,
+        create_project_conversation_response_401_data = cls(
+            code=code,
+            message=message,
         )
 
-        get_project_pages_response_200_data.additional_properties = d
-        return get_project_pages_response_200_data
+        create_project_conversation_response_401_data.additional_properties = d
+        return create_project_conversation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data_pages.py` & `customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.get_project_pages_response_200_data_pages_links import GetProjectPagesResponse200DataPagesLinks
-    from ..models.page import Page
+    from ..models.list_projects_response_200_data_data_item import ListProjectsResponse200DataDataItem
+    from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
 
 
-T = TypeVar("T", bound="GetProjectPagesResponse200DataPages")
+T = TypeVar("T", bound="ListProjectsResponse200Data")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectPagesResponse200DataPages:
+class ListProjectsResponse200Data:
     """
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
-        data (Union[Unset, List['Page']]):
+        data (Union[Unset, List['ListProjectsResponse200DataDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, GetProjectPagesResponse200DataPagesLinks]):
+        links (Union[Unset, ListProjectsResponse200DataLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
-    data: Union[Unset, List["Page"]] = UNSET
+    data: Union[Unset, List["ListProjectsResponse200DataDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "GetProjectPagesResponse200DataPagesLinks"] = UNSET
+    links: Union[Unset, "ListProjectsResponse200DataLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -102,55 +102,55 @@
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.get_project_pages_response_200_data_pages_links import GetProjectPagesResponse200DataPagesLinks
-        from ..models.page import Page
+        from ..models.list_projects_response_200_data_data_item import ListProjectsResponse200DataDataItem
+        from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
 
         d = src_dict.copy()
         current_page = d.pop("current_page", UNSET)
 
         data = []
         _data = d.pop("data", UNSET)
         for data_item_data in _data or []:
-            data_item = Page.from_dict(data_item_data)
+            data_item = ListProjectsResponse200DataDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
         first_page_url = d.pop("first_page_url", UNSET)
 
         from_ = d.pop("from", UNSET)
 
         last_page = d.pop("last_page", UNSET)
 
         last_page_url = d.pop("last_page_url", UNSET)
 
         _links = d.pop("links", UNSET)
-        links: Union[Unset, GetProjectPagesResponse200DataPagesLinks]
+        links: Union[Unset, ListProjectsResponse200DataLinks]
         if isinstance(_links, Unset):
             links = UNSET
         else:
-            links = GetProjectPagesResponse200DataPagesLinks.from_dict(_links)
+            links = ListProjectsResponse200DataLinks.from_dict(_links)
 
         next_page_url = d.pop("next_page_url", UNSET)
 
         path = d.pop("path", UNSET)
 
         per_page = d.pop("per_page", UNSET)
 
         prev_page_url = d.pop("prev_page_url", UNSET)
 
         to = d.pop("to", UNSET)
 
         total = d.pop("total", UNSET)
 
-        get_project_pages_response_200_data_pages = cls(
+        list_projects_response_200_data = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
             links=links,
@@ -158,16 +158,16 @@
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        get_project_pages_response_200_data_pages.additional_properties = d
-        return get_project_pages_response_200_data_pages
+        list_projects_response_200_data.additional_properties = d
+        return list_projects_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_project_pages_response_200_data_pages_links.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_pages_response_200_data_pages_links.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_user_profile_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_user_profile_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/get_user_profile_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_json_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.user import User
-
-
-T = TypeVar("T", bound="GetUserProfileResponse200Data")
+T = TypeVar("T", bound="UpdateProjectConversationJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class GetUserProfileResponse200Data:
+class UpdateProjectConversationJsonBody:
     """
     Attributes:
-        user (Union[Unset, User]):
+        name (Union[Unset, str]): The new name of the conversation Example: My new conversation name.
     """
 
-    user: Union[Unset, "User"] = UNSET
+    name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.user, Unset):
-            user = self.user.to_dict()
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if user is not UNSET:
-            field_dict["user"] = user
+        if name is not UNSET:
+            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.user import User
-
         d = src_dict.copy()
-        _user = d.pop("user", UNSET)
-        user: Union[Unset, User]
-        if isinstance(_user, Unset):
-            user = UNSET
-        else:
-            user = User.from_dict(_user)
+        name = d.pop("name", UNSET)
 
-        get_user_profile_response_200_data = cls(
-            user=user,
+        update_project_conversation_json_body = cls(
+            name=name,
         )
 
-        get_user_profile_response_200_data.additional_properties = d
-        return get_user_profile_response_200_data
+        update_project_conversation_json_body.additional_properties = d
+        return update_project_conversation_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/messages_response_200_messages.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
-    from ..models.project import Project
+    from ..models.messages_response_200_messages_data_item import MessagesResponse200MessagesDataItem
+    from ..models.messages_response_200_messages_links import MessagesResponse200MessagesLinks
 
 
-T = TypeVar("T", bound="ListProjectsResponse200Data")
+T = TypeVar("T", bound="MessagesResponse200Messages")
 
 
 @attr.s(auto_attribs=True)
-class ListProjectsResponse200Data:
+class MessagesResponse200Messages:
     """
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
-        data (Union[Unset, List['Project']]):
+        data (Union[Unset, List['MessagesResponse200MessagesDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, ListProjectsResponse200DataLinks]):
+        links (Union[Unset, MessagesResponse200MessagesLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
-    data: Union[Unset, List["Project"]] = UNSET
+    data: Union[Unset, List["MessagesResponse200MessagesDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "ListProjectsResponse200DataLinks"] = UNSET
+    links: Union[Unset, "MessagesResponse200MessagesLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -102,55 +102,55 @@
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
-        from ..models.project import Project
+        from ..models.messages_response_200_messages_data_item import MessagesResponse200MessagesDataItem
+        from ..models.messages_response_200_messages_links import MessagesResponse200MessagesLinks
 
         d = src_dict.copy()
         current_page = d.pop("current_page", UNSET)
 
         data = []
         _data = d.pop("data", UNSET)
         for data_item_data in _data or []:
-            data_item = Project.from_dict(data_item_data)
+            data_item = MessagesResponse200MessagesDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
         first_page_url = d.pop("first_page_url", UNSET)
 
         from_ = d.pop("from", UNSET)
 
         last_page = d.pop("last_page", UNSET)
 
         last_page_url = d.pop("last_page_url", UNSET)
 
         _links = d.pop("links", UNSET)
-        links: Union[Unset, ListProjectsResponse200DataLinks]
+        links: Union[Unset, MessagesResponse200MessagesLinks]
         if isinstance(_links, Unset):
             links = UNSET
         else:
-            links = ListProjectsResponse200DataLinks.from_dict(_links)
+            links = MessagesResponse200MessagesLinks.from_dict(_links)
 
         next_page_url = d.pop("next_page_url", UNSET)
 
         path = d.pop("path", UNSET)
 
         per_page = d.pop("per_page", UNSET)
 
         prev_page_url = d.pop("prev_page_url", UNSET)
 
         to = d.pop("to", UNSET)
 
         total = d.pop("total", UNSET)
 
-        list_projects_response_200_data = cls(
+        messages_response_200_messages = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
             links=links,
@@ -158,16 +158,16 @@
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        list_projects_response_200_data.additional_properties = d
-        return list_projects_response_200_data
+        messages_response_200_messages.additional_properties = d
+        return messages_response_200_messages
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/list_projects_response_200_data_links.py` & `customgpt_client-1.0.4/custom_gpt_client/models/list_projects_response_200_data_links.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/open_graph_cache.py` & `customgpt_client-1.0.4/custom_gpt_client/models/open_graph_cache.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/page.py` & `customgpt_client-1.0.4/custom_gpt_client/models/page.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/project.py` & `customgpt_client-1.0.4/custom_gpt_client/models/project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/project_plugin.py` & `customgpt_client-1.0.4/custom_gpt_client/models/project_plugin.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/project_settings.py` & `customgpt_client-1.0.4/custom_gpt_client/models/project_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/prompt_history.py` & `customgpt_client-1.0.4/custom_gpt_client/models/prompt_history.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/send_message_to_conversation_json_body.py` & `customgpt_client-1.0.4/custom_gpt_client/models/send_message_to_conversation_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_json_body.py` & `customgpt_client-1.0.4/custom_gpt_client/models/delete_project_response_401_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.delete_project_response_401_data_code import DeleteProjectResponse401DataCode
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateProjectConversationJsonBody")
+T = TypeVar("T", bound="DeleteProjectResponse401Data")
 
 
 @attr.s(auto_attribs=True)
-class UpdateProjectConversationJsonBody:
+class DeleteProjectResponse401Data:
     """
     Attributes:
-        name (Union[Unset, str]): The new name of the conversation Example: My new conversation name.
+        code (Union[Unset, DeleteProjectResponse401DataCode]): The error status code Example: 401.
+        message (Union[Unset, str]):  Example: API Token is either missing or invalid.
     """
 
-    name: Union[Unset, str] = UNSET
+    code: Union[Unset, DeleteProjectResponse401DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if name is not UNSET:
-            field_dict["name"] = name
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name", UNSET)
-
-        update_project_conversation_json_body = cls(
-            name=name,
+        _code = d.pop("code", UNSET)
+        code: Union[Unset, DeleteProjectResponse401DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
+        else:
+            code = DeleteProjectResponse401DataCode(_code)
+
+        message = d.pop("message", UNSET)
+
+        delete_project_response_401_data = cls(
+            code=code,
+            message=message,
         )
 
-        update_project_conversation_json_body.additional_properties = d
-        return update_project_conversation_json_body
+        delete_project_response_401_data.additional_properties = d
+        return delete_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_project_conversation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_project_conversation_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/get_project_conversations_response_500_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,65 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.get_project_conversations_response_500_data_code import GetProjectConversationsResponse500DataCode
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.conversation import Conversation
-
-
-T = TypeVar("T", bound="UpdateProjectConversationResponse200Data")
+T = TypeVar("T", bound="GetProjectConversationsResponse500Data")
 
 
 @attr.s(auto_attribs=True)
-class UpdateProjectConversationResponse200Data:
+class GetProjectConversationsResponse500Data:
     """
     Attributes:
-        conversation_schema (Union[Unset, Conversation]):
+        code (Union[Unset, GetProjectConversationsResponse500DataCode]): The error status code Example: 500.
+        message (Union[Unset, str]):  Example: Internal Server Error.
     """
 
-    conversation_schema: Union[Unset, "Conversation"] = UNSET
+    code: Union[Unset, GetProjectConversationsResponse500DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        conversation_schema: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.conversation_schema, Unset):
-            conversation_schema = self.conversation_schema.to_dict()
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if conversation_schema is not UNSET:
-            field_dict["ConversationSchema"] = conversation_schema
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.conversation import Conversation
-
         d = src_dict.copy()
-        _conversation_schema = d.pop("ConversationSchema", UNSET)
-        conversation_schema: Union[Unset, Conversation]
-        if isinstance(_conversation_schema, Unset):
-            conversation_schema = UNSET
+        _code = d.pop("code", UNSET)
+        code: Union[Unset, GetProjectConversationsResponse500DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
         else:
-            conversation_schema = Conversation.from_dict(_conversation_schema)
+            code = GetProjectConversationsResponse500DataCode(_code)
+
+        message = d.pop("message", UNSET)
 
-        update_project_conversation_response_200_data = cls(
-            conversation_schema=conversation_schema,
+        get_project_conversations_response_500_data = cls(
+            code=code,
+            message=message,
         )
 
-        update_project_conversation_response_200_data.additional_properties = d
-        return update_project_conversation_response_200_data
+        get_project_conversations_response_500_data.additional_properties = d
+        return get_project_conversations_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_project_multipart_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_project_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_project_settings_multipart_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_project_settings_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_multipart_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_response_200.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_user_profile_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/update_user_profile_response_200_data.py` & `customgpt_client-1.0.4/custom_gpt_client/models/update_project_response_500_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,65 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.update_project_response_500_data_code import UpdateProjectResponse500DataCode
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.user import User
-
-
-T = TypeVar("T", bound="UpdateUserProfileResponse200Data")
+T = TypeVar("T", bound="UpdateProjectResponse500Data")
 
 
 @attr.s(auto_attribs=True)
-class UpdateUserProfileResponse200Data:
+class UpdateProjectResponse500Data:
     """
     Attributes:
-        user (Union[Unset, User]):
+        code (Union[Unset, UpdateProjectResponse500DataCode]): The error status code Example: 500.
+        message (Union[Unset, str]):  Example: Internal Server Error.
     """
 
-    user: Union[Unset, "User"] = UNSET
+    code: Union[Unset, UpdateProjectResponse500DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.user, Unset):
-            user = self.user.to_dict()
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if user is not UNSET:
-            field_dict["user"] = user
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.user import User
-
         d = src_dict.copy()
-        _user = d.pop("user", UNSET)
-        user: Union[Unset, User]
-        if isinstance(_user, Unset):
-            user = UNSET
+        _code = d.pop("code", UNSET)
+        code: Union[Unset, UpdateProjectResponse500DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
         else:
-            user = User.from_dict(_user)
+            code = UpdateProjectResponse500DataCode(_code)
+
+        message = d.pop("message", UNSET)
 
-        update_user_profile_response_200_data = cls(
-            user=user,
+        update_project_response_500_data = cls(
+            code=code,
+            message=message,
         )
 
-        update_user_profile_response_200_data.additional_properties = d
-        return update_user_profile_response_200_data
+        update_project_response_500_data.additional_properties = d
+        return update_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `customgpt_client-1.0.3/custom_gpt_client/models/user.py` & `customgpt_client-1.0.4/custom_gpt_client/models/user.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/custom_gpt_client/types.py` & `customgpt_client-1.0.4/custom_gpt_client/types.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.0.3/pyproject.toml` & `customgpt_client-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "customgpt-client"
-version = "1.0.3"
+version = "1.0.4"
 description = "A client library for accessing CustomGPT"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "custom_gpt_client"},
```

### Comparing `customgpt_client-1.0.3/PKG-INFO` & `customgpt_client-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A client library for accessing CustomGPT
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

