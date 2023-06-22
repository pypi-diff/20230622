# Comparing `tmp/core_models-0.1.0.tar.gz` & `tmp/core_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_models-0.1.0.tar", last modified: Mon Jun 12 21:43:51 2023, max compression
+gzip compressed data, was "core_models-0.1.1.tar", last modified: Thu Jun 22 05:24:07 2023, max compression
```

## Comparing `core_models-0.1.0.tar` & `core_models-0.1.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.666797 core_models-0.1.0/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.1.0/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-12 21:43:51.666518 core_models-0.1.0/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.1.0/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.656217 core_models-0.1.0/core_models/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.1.0/core_models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.1.0/core_models/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.658078 core_models-0.1.0/core_models/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.1.0/core_models/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     9351 2023-05-22 22:44:46.000000 core_models-0.1.0/core_models/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.1.0/core_models/app/apps.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.1.0/core_models/app/context_processors.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.658512 core_models-0.1.0/core_models/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.1.0/core_models/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6142 2023-06-11 23:14:32.000000 core_models-0.1.0/core_models/app/managers/notification_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.661471 core_models-0.1.0/core_models/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.1.0/core_models/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.1.0/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.1.0/core_models/app/migrations/0003_alter_user_onboarding_stage.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.1.0/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.1.0/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.1.0/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.1.0/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.1.0/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.1.0/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.1.0/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.1.0/core_models/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.664405 core_models-0.1.0/core_models/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.1.0/core_models/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.1.0/core_models/app/models/bank_account.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.1.0/core_models/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2215 2023-05-29 15:03:18.000000 core_models-0.1.0/core_models/app/models/company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.1.0/core_models/app/models/configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.1.0/core_models/app/models/contract.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.1.0/core_models/app/models/currency.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4104 2023-06-12 17:47:17.000000 core_models-0.1.0/core_models/app/models/invoice.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.1.0/core_models/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.1.0/core_models/app/models/transaction.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.1.0/core_models/app/models/user.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.664978 core_models-0.1.0/core_models/app/templates/
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.665970 core_models-0.1.0/core_models/app/templates/core_models/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.1.0/core_models/app/templates/core_models/mail-base.html
--rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.1.0/core_models/app/templates/core_models/mail-base.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.1.0/core_models/app/templates/invoice.html
--rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.1.0/core_models/app/templates/reset.html
--rw-r--r--   0 macbookpro   (501) staff       (20)     3182 2023-06-12 14:08:46.000000 core_models-0.1.0/core_models/base_views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3324 2023-06-11 21:08:48.000000 core_models-0.1.0/core_models/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.1.0/core_models/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7516 2023-06-11 00:16:44.000000 core_models-0.1.0/core_models/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.1.0/core_models/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 21:43:51.657095 core_models-0.1.0/core_models.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-12 21:43:51.000000 core_models-0.1.0/core_models.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-06-12 21:43:51.000000 core_models-0.1.0/core_models.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-06-12 21:43:51.000000 core_models-0.1.0/core_models.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      195 2023-06-12 21:43:51.000000 core_models-0.1.0/core_models.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-06-12 21:43:51.000000 core_models-0.1.0/core_models.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.1.0/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-06-12 21:43:51.666892 core_models-0.1.0/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1257 2023-06-12 21:43:43.000000 core_models-0.1.0/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.892630 core_models-0.1.1/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.1.1/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-22 05:24:07.892408 core_models-0.1.1/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.1.1/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.862339 core_models-0.1.1/core_models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.1.1/core_models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.1.1/core_models/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.864281 core_models-0.1.1/core_models/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.1.1/core_models/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     9351 2023-05-22 22:44:46.000000 core_models-0.1.1/core_models/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.1.1/core_models/app/apps.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.1.1/core_models/app/context_processors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.864715 core_models-0.1.1/core_models/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.1.1/core_models/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6142 2023-06-11 23:14:32.000000 core_models-0.1.1/core_models/app/managers/notification_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.887394 core_models-0.1.1/core_models/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.1.1/core_models/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.1.1/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.1.1/core_models/app/migrations/0003_alter_user_onboarding_stage.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.1.1/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.1.1/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.1.1/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.1.1/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.1.1/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.1.1/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.1.1/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.1.1/core_models/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.890857 core_models-0.1.1/core_models/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      419 2023-06-13 14:55:57.000000 core_models-0.1.1/core_models/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.1.1/core_models/app/models/bank_account.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.1.1/core_models/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2204 2023-06-13 17:30:06.000000 core_models-0.1.1/core_models/app/models/company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.1.1/core_models/app/models/configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.1.1/core_models/app/models/contract.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      624 2023-06-13 14:53:32.000000 core_models-0.1.1/core_models/app/models/country.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.1.1/core_models/app/models/currency.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4104 2023-06-12 17:47:17.000000 core_models-0.1.1/core_models/app/models/invoice.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.1.1/core_models/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.1.1/core_models/app/models/transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.1.1/core_models/app/models/user.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.891426 core_models-0.1.1/core_models/app/templates/
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.892042 core_models-0.1.1/core_models/app/templates/core_models/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.1.1/core_models/app/templates/core_models/mail-base.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.1.1/core_models/app/templates/core_models/mail-base.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.1.1/core_models/app/templates/invoice.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.1.1/core_models/app/templates/reset.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3182 2023-06-12 14:08:46.000000 core_models-0.1.1/core_models/base_views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3324 2023-06-11 21:08:48.000000 core_models-0.1.1/core_models/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.1.1/core_models/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7690 2023-06-13 19:13:14.000000 core_models-0.1.1/core_models/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.1.1/core_models/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-22 05:24:07.863204 core_models-0.1.1/core_models.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-22 05:24:07.000000 core_models-0.1.1/core_models.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2013 2023-06-22 05:24:07.000000 core_models-0.1.1/core_models.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-06-22 05:24:07.000000 core_models-0.1.1/core_models.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      195 2023-06-22 05:24:07.000000 core_models-0.1.1/core_models.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-06-22 05:24:07.000000 core_models-0.1.1/core_models.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.1.1/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-06-22 05:24:07.892693 core_models-0.1.1/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1257 2023-06-19 10:11:46.000000 core_models-0.1.1/setup.py
```

### Comparing `core_models-0.1.0/LICENSE` & `core_models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/README.md` & `core_models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/api_response.py` & `core_models-0.1.1/core_models/api_response.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/admin.py` & `core_models-0.1.1/core_models/app/admin.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/managers/notification_manager.py` & `core_models-0.1.1/core_models/app/managers/notification_manager.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0001_initial.py` & `core_models-0.1.1/core_models/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py` & `core_models-0.1.1/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py` & `core_models-0.1.1/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py` & `core_models-0.1.1/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py` & `core_models-0.1.1/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py` & `core_models-0.1.1/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py` & `core_models-0.1.1/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py` & `core_models-0.1.1/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py` & `core_models-0.1.1/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/base.py` & `core_models-0.1.1/core_models/app/models/base.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/company.py` & `core_models-0.1.1/core_models/app/models/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
-from cities_light.models import Country, Region, City
 from django.db import models
 from django.utils import timezone
 
+from .country import Country, Region, City
 from .base import BaseModelAbstract
 from .user import User
 
 
 class Company(BaseModelAbstract, models.Model):
     created_by = None
     user = models.OneToOneField(User, models.CASCADE, related_name='company')
```

### Comparing `core_models-0.1.0/core_models/app/models/configuration.py` & `core_models-0.1.1/core_models/app/models/configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/contract.py` & `core_models-0.1.1/core_models/app/models/contract.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/currency.py` & `core_models-0.1.1/core_models/app/models/currency.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/invoice.py` & `core_models-0.1.1/core_models/app/models/invoice.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/transaction.py` & `core_models-0.1.1/core_models/app/models/transaction.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/models/user.py` & `core_models-0.1.1/core_models/app/models/user.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/templates/core_models/mail-base.html` & `core_models-0.1.1/core_models/app/templates/core_models/mail-base.html`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/templates/core_models/mail-base.txt` & `core_models-0.1.1/core_models/app/templates/core_models/mail-base.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/templates/invoice.html` & `core_models-0.1.1/core_models/app/templates/invoice.html`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/app/templates/reset.html` & `core_models-0.1.1/core_models/app/templates/reset.html`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/base_views.py` & `core_models-0.1.1/core_models/base_views.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/constants.py` & `core_models-0.1.1/core_models/constants.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/settings.example.py` & `core_models-0.1.1/core_models/settings.example.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models/settings.py` & `core_models-0.1.1/core_models/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,7 +271,13 @@
 
 if FILE_UPLOAD_STORAGE == "gcloud":
     DEFAULT_FILE_STORAGE = 'storages.backends.gcloud.GoogleCloudStorage'
     GS_BUCKET_NAME = env("GS_BUCKET_NAME")
     STATICFILES_STORAGE = 'storages.backends.gcloud.GoogleCloudStorage'
     GS_DEFAULT_ACL = "publicRead"
 
+CITIES_LIGHT_APP_NAME = 'app'
+CITIES_LIGHT_TRANSLATION_LANGUAGES = ('en', )
+# Disable built-in cities_light migrations
+# MIGRATION_MODULES = {
+#     'cities_light': None
+# }
```

### Comparing `core_models-0.1.0/core_models/utils.py` & `core_models-0.1.1/core_models/utils.py`

 * *Files identical despite different names*

### Comparing `core_models-0.1.0/core_models.egg-info/SOURCES.txt` & `core_models-0.1.1/core_models.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 core_models/app/migrations/__init__.py
 core_models/app/models/__init__.py
 core_models/app/models/bank_account.py
 core_models/app/models/base.py
 core_models/app/models/company.py
 core_models/app/models/configuration.py
 core_models/app/models/contract.py
+core_models/app/models/country.py
 core_models/app/models/currency.py
 core_models/app/models/invoice.py
 core_models/app/models/notification.py
 core_models/app/models/transaction.py
 core_models/app/models/user.py
 core_models/app/templates/invoice.html
 core_models/app/templates/reset.html
```

### Comparing `core_models-0.1.0/setup.py` & `core_models-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Liquify core package'
 LONG_DESCRIPTION = 'Package that holds all models and core ' \
                    'functions/classes of Liquify project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
```

