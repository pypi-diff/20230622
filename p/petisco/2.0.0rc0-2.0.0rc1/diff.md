# Comparing `tmp/petisco-2.0.0rc0.tar.gz` & `tmp/petisco-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-2.0.0rc0.tar", last modified: Thu May 25 14:20:09 2023, max compression
+gzip compressed data, was "petisco-2.0.0rc1.tar", last modified: Thu Jun 22 11:48:07 2023, max compression
```

## Comparing `petisco-2.0.0rc0.tar` & `petisco-2.0.0rc1.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/chaos_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/check_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/async_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/meta_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/handlers/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/async_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/async_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/meta_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/async_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/async_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/persistence_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/sql_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/async_elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/is_elastic_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/legacy_elastic_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/elastic_apm/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/is_elastic_apm_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/application/fastapi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/as_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/loguru_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/not_implemented_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/is_redis_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/base_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/threading/pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.920963 petisco-2.0.0rc1/petisco/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.924963 petisco-2.0.0rc1/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.924963 petisco-2.0.0rc1/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.924963 petisco-2.0.0rc1/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.924963 petisco-2.0.0rc1/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.928963 petisco-2.0.0rc1/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.932963 petisco-2.0.0rc1/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.932963 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.936963 petisco-2.0.0rc1/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.936963 petisco-2.0.0rc1/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.936963 petisco-2.0.0rc1/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.936963 petisco-2.0.0rc1/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/legacy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/legacy_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/persistence_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/domain/persistence/sql_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/is_elastic_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic/legacy_elastic_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.940963 petisco-2.0.0rc1/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/application/fastapi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.944963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.948963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.948963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.952963 petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.956963 petisco-2.0.0rc1/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.956963 petisco-2.0.0rc1/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.956963 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.956963 petisco-2.0.0rc1/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/base_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.924963 petisco-2.0.0rc1/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 11:48:07.000000 petisco-2.0.0rc1/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-22 11:48:07.964963 petisco-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:07.960963 petisco-2.0.0rc1/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:48:01.000000 petisco-2.0.0rc1/tests/modules/__init__.py
```

### Comparing `petisco-2.0.0rc0/LICENSE` & `petisco-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/PKG-INFO` & `petisco-2.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
@@ -37,17 +37,21 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![license](https://img.shields.io/github/license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/petisco/blob/main/LICENSE)
 [![versions](https://img.shields.io/pypi/pyversions/petisco.svg)](https://github.com/alice-biometrics/petisco)
 
 <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true" width=auto>
 
 > **Warning**
-> Disclaimer:
-> Current version now is v1 (not stable yet). 
-> v0 is now deprecated (legacy branch)
+> 
+> Current version now is v1 (*v1 branch*). 
+> 
+> v0 is now deprecated (*legacy branch*)
+> 
+> v2 is about to be release (*main branch*). 1 release candidate
+
 
 ---
 
 **Documentation**: <a href="https://alice-biometrics.github.io/petisco/" target="_blank">https://alice-biometrics.github.io/petisco/</a>
 
 **Source Code**: <a href="https://github.com/alice-biometrics/petisco" target="_blank">https://github.com/alice-biometrics/petisco</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc0 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc1 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -23,20 +23,21 @@
 000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) [![license](https://img.shields.io/github/
 license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/
 petisco/blob/main/LICENSE) [![versions](https://img.shields.io/pypi/pyversions/
 petisco.svg)](https://github.com/alice-biometrics/petisco) [https://github.com/
 alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true] >
-**Warning** > Disclaimer: > Current version now is v1 (not stable yet). > v0 is
-now deprecated (legacy branch) --- **Documentation**: https://alice-
-biometrics.github.io/petisco/ **Source Code**: https://github.com/alice-
-biometrics/petisco --- ## What is petisco? ðª petisco is a framework for
-helping Python developers to build clean Applications in Python. ## How could
-petisco help me? ðª petisco provides several handy classes to help you on
-defining your domain with hexagonal architecture, event streaming and CQRS. ##
-Installation ð» ```console pip install petisco ``` Installation with Extras
-```console pip install petisco[fastapi,sqlalchemy,elastic,elastic-
-apm,rabbitmq,slack,redis] ``` ## Contribute We'd love you to contribute to
-*petisco* ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our
-[documentation](https://alice-biometrics.github.io/petisco/contributing/) ##
-Contact ð¬ support@alicebiometrics.com
+**Warning** > > Current version now is v1 (*v1 branch*). > > v0 is now
+deprecated (*legacy branch*) > > v2 is about to be release (*main branch*). 1
+release candidate --- **Documentation**: https://alice-biometrics.github.io/
+petisco/ **Source Code**: https://github.com/alice-biometrics/petisco --- ##
+What is petisco? ðª petisco is a framework for helping Python developers to
+build clean Applications in Python. ## How could petisco help me? ðª petisco
+provides several handy classes to help you on defining your domain with
+hexagonal architecture, event streaming and CQRS. ## Installation ð»
+```console pip install petisco ``` Installation with Extras ```console pip
+install petisco[fastapi,sqlalchemy,elastic,elastic-apm,rabbitmq,slack,redis]
+``` ## Contribute We'd love you to contribute to *petisco*
+ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our [documentation]
+(https://alice-biometrics.github.io/petisco/contributing/) ## Contact ð¬
+support@alicebiometrics.com
```

### Comparing `petisco-2.0.0rc0/README.md` & `petisco-2.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![license](https://img.shields.io/github/license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/petisco/blob/main/LICENSE)
 [![versions](https://img.shields.io/pypi/pyversions/petisco.svg)](https://github.com/alice-biometrics/petisco)
 
 <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true" width=auto>
 
 > **Warning**
-> Disclaimer:
-> Current version now is v1 (not stable yet). 
-> v0 is now deprecated (legacy branch)
+> 
+> Current version now is v1 (*v1 branch*). 
+> 
+> v0 is now deprecated (*legacy branch*)
+> 
+> v2 is about to be release (*main branch*). 1 release candidate
+
 
 ---
 
 **Documentation**: <a href="https://alice-biometrics.github.io/petisco/" target="_blank">https://alice-biometrics.github.io/petisco/</a>
 
 **Source Code**: <a href="https://github.com/alice-biometrics/petisco" target="_blank">https://github.com/alice-biometrics/petisco</a>
```

#### html2text {}

```diff
@@ -9,20 +9,21 @@
 000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) [![license](https://img.shields.io/github/
 license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/
 petisco/blob/main/LICENSE) [![versions](https://img.shields.io/pypi/pyversions/
 petisco.svg)](https://github.com/alice-biometrics/petisco) [https://github.com/
 alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true] >
-**Warning** > Disclaimer: > Current version now is v1 (not stable yet). > v0 is
-now deprecated (legacy branch) --- **Documentation**: https://alice-
-biometrics.github.io/petisco/ **Source Code**: https://github.com/alice-
-biometrics/petisco --- ## What is petisco? ðª petisco is a framework for
-helping Python developers to build clean Applications in Python. ## How could
-petisco help me? ðª petisco provides several handy classes to help you on
-defining your domain with hexagonal architecture, event streaming and CQRS. ##
-Installation ð» ```console pip install petisco ``` Installation with Extras
-```console pip install petisco[fastapi,sqlalchemy,elastic,elastic-
-apm,rabbitmq,slack,redis] ``` ## Contribute We'd love you to contribute to
-*petisco* ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our
-[documentation](https://alice-biometrics.github.io/petisco/contributing/) ##
-Contact ð¬ support@alicebiometrics.com
+**Warning** > > Current version now is v1 (*v1 branch*). > > v0 is now
+deprecated (*legacy branch*) > > v2 is about to be release (*main branch*). 1
+release candidate --- **Documentation**: https://alice-biometrics.github.io/
+petisco/ **Source Code**: https://github.com/alice-biometrics/petisco --- ##
+What is petisco? ðª petisco is a framework for helping Python developers to
+build clean Applications in Python. ## How could petisco help me? ðª petisco
+provides several handy classes to help you on defining your domain with
+hexagonal architecture, event streaming and CQRS. ## Installation ð»
+```console pip install petisco ``` Installation with Extras ```console pip
+install petisco[fastapi,sqlalchemy,elastic,elastic-apm,rabbitmq,slack,redis]
+``` ## Contribute We'd love you to contribute to *petisco*
+ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our [documentation]
+(https://alice-biometrics.github.io/petisco/contributing/) ## Contact ð¬
+support@alicebiometrics.com
```

### Comparing `petisco-2.0.0rc0/petisco/base/application/application.py` & `petisco-2.0.0rc1/petisco/base/application/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from datetime import datetime, timedelta
-from typing import Any, Callable, Dict, List
+from typing import Any, Callable, Dict, List, Union
 
 from loguru import logger
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from pydantic_settings import BaseSettings
 
 from petisco.base.application.application_configurer import ApplicationConfigurer
 from petisco.base.application.application_info import ApplicationInfo
+from petisco.base.application.controller.error_map import ErrorMap
 from petisco.base.application.dependency_injection.container import Container
 from petisco.base.application.dependency_injection.dependency import Dependency
 from petisco.base.application.notifier.notifier import Notifier
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.message.domain_event_bus import DomainEventBus
 from petisco.extra.rabbitmq.dependencies import get_default_message_dependencies
@@ -20,22 +22,24 @@
     name: str
     version: str
     organization: str
     deployed_at: datetime
     environment: str = Field("local", env="ENVIRONMENT")
     dependencies_provider: Callable[..., List[Dependency]] = lambda: []
     configurers: List[ApplicationConfigurer] = []
+    shared_error_map: Union[ErrorMap, None] = Field(default=dict())
 
     def __init__(self, **data: Any) -> None:
         info = ApplicationInfo(
             name=data["name"],
             organization=data["organization"],
             version=data["version"],
             deployed_at=data.get("deployed_at"),
             force_recreation=True,
+            shared_error_map=data.get("shared_error_map", dict()),
         )
         deployed_at = info.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
         logger.info(
             f"Application: {info.name} {info.version} ({info.organization}) deployed at {deployed_at}"
         )
         super().__init__(**data)
 
@@ -81,16 +85,14 @@
 
     def get_dependencies(self) -> List[Dependency]:
         # TODO: review default dependencies in v2
 
         default_dependencies = (
             get_default_message_dependencies() + get_default_notifier_dependencies()
         )
-        # TODO: the `dependency.type if not dependency.name else dependency.name` will be deprecated in v2 -> use
-        #  just `dependency.type` as key
         default_dependencies_dict = {
             dependency.get_key(): dependency for dependency in default_dependencies
         }
         provided_dependencies = self.dependencies_provider()
         provided_dependencies_dict = {
             dependency.get_key(): dependency for dependency in provided_dependencies
         }
@@ -103,21 +105,21 @@
 
     def clear(self) -> None:
         Container.clear()
 
     def info(self) -> Dict[str, Any]:
         info = self.dict()
         info["deployed_at"] = self.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
-
         info["dependencies"] = {
             dependency.type.__name__: dependency.get_instance().info()
             for dependency in self.get_dependencies()
         }
         del info["dependencies_provider"]
         del info["configurers"]
+        del info["shared_error_map"]
         return info
 
     def was_deploy_few_minutes_ago(self, minutes: int = 25) -> bool:
         return datetime.utcnow() < self.deployed_at + timedelta(minutes=minutes)
 
     def publish_domain_event(self, domain_event: DomainEvent) -> None:
         try:
```

### Comparing `petisco-2.0.0rc0/petisco/base/application/chaos/chaos_config.py` & `petisco-2.0.0rc1/petisco/base/application/chaos/chaos_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from pydantic import BaseSettings, Field, confloat
+from typing import Union
+
+from pydantic import Field, confloat
+from pydantic_settings import BaseSettings
 
 
 class ChaosConfig(BaseSettings):
     percentage_invalid_message_publication: confloat(ge=0.0, le=1.0) = Field(
         default=0,
         env="PETISCO_CHAOS_PERCENTAGE_INVALID_MESSAGE_PUBLICATION",
         description="Percentage of invalid message publication. Where 1.0 means rejecting all the publishing messages.",
@@ -18,15 +21,15 @@
         description="Delay message handler execution for a given number of seconds",
     )
     percentage_simulate_failures: confloat(ge=0.0, le=1.0) = Field(
         default=0,
         env="PETISCO_CHAOS_DELAY_AFTER_OPERATION_SECONDS",
         description="Percentage of simulate failures. Where 1.0 simulate always a failure on handlers",
     )
-    protected_routing_keys: str = Field(
+    protected_routing_keys: Union[str, None] = Field(
         default=None,
         env="PETISCO_CHAOS_PROTECTED_ROUTING_KEYS",
         description="Routing keys where chaos will not be applied",
     )
 
 
 chaos_config = ChaosConfig()
```

### Comparing `petisco-2.0.0rc0/petisco/base/application/controller/async_controller.py` & `petisco-2.0.0rc1/petisco/base/application/controller/async_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/controller/meta_controller.py` & `petisco-2.0.0rc1/petisco/base/application/controller/meta_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/dependency_injection/container.py` & `petisco-2.0.0rc1/petisco/base/application/dependency_injection/container.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/dependency_injection/dependency.py` & `petisco-2.0.0rc1/petisco/base/application/dependency_injection/dependency.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/handlers/message_handler.py` & `petisco-2.0.0rc1/petisco/base/application/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/middleware/middleware.py` & `petisco-2.0.0rc1/petisco/base/application/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.0.0rc1/petisco/base/application/middleware/notifier_middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/notifier/notifier.py` & `petisco-2.0.0rc1/petisco/base/application/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-2.0.0rc1/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/patterns/crud_repository.py` & `petisco-2.0.0rc1/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.0.0rc1/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/application/use_case/meta_use_case.py` & `petisco-2.0.0rc1/petisco/base/application/use_case/meta_use_case.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.0.0rc1/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.0.0rc1/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.0.0rc1/petisco/base/domain/errors/defaults/not_found.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/errors/domain_error.py` & `petisco-2.0.0rc1/petisco/base/domain/errors/domain_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/errors/unknown_error.py` & `petisco-2.0.0rc1/petisco/base/domain/errors/unknown_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-2.0.0rc1/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/command.py` & `petisco-2.0.0rc1/petisco/base/domain/message/command.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/command_bus.py` & `petisco-2.0.0rc1/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/command_subscriber.py` & `petisco-2.0.0rc1/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/domain_event.py` & `petisco-2.0.0rc1/petisco/base/domain/message/domain_event.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.0.0rc1/petisco/base/domain/message/domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-2.0.0rc1/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_bus.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_configurer.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_consumer.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_handler_returns_none_error.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_handler_returns_none_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber_info.py` & `petisco-2.0.0rc1/petisco/base/domain/message/message_subscriber_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_command_bus.py` & `petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.0.0rc1/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/model/aggregate_root.py` & `petisco-2.0.0rc1/petisco/base/domain/model/aggregate_root.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from abc import ABC
 from copy import copy
 from typing import List, Union
 
-from pydantic import BaseModel, Field, NonNegativeInt, PrivateAttr, validator
+from pydantic import (
+    BaseModel,
+    Field,
+    NonNegativeInt,
+    PrivateAttr,
+    field_serializer,
+    field_validator,
+)
 
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.model.uuid import Uuid
 
 DEFAULT_VERSION = 1
 
 
@@ -17,20 +24,24 @@
     It is a cluster of associated entities that are treated as a unit for the purpose of data changes.
     """
 
     aggregate_id: Uuid = Field(default=Uuid.v4())
     aggregate_version: NonNegativeInt = Field(default=DEFAULT_VERSION)
     _domain_events: List[DomainEvent] = PrivateAttr(default=[])
 
-    @validator("aggregate_id", pre=True, always=True)
+    @field_serializer("aggregate_id")
+    def serialize_aggregate_id(self, aggregate_id: Uuid):
+        return aggregate_id.value
+
+    @field_validator("aggregate_id", mode="before")
     def set_aggregate_id(cls, v: Union[str, Uuid]) -> Uuid:
         v = Uuid(v) if isinstance(v, str) else v
         return v or Uuid.v4()
 
-    @validator("aggregate_version", pre=True, always=True)
+    @field_validator("aggregate_version", mode="before")
     def set_aggregate_version(cls, v: NonNegativeInt) -> NonNegativeInt:
         return v or DEFAULT_VERSION
 
     def record(self, domain_event: DomainEvent) -> None:
         """
         Record something that happened is our domain related with the aggregate (a DomainEvent).
         """
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/model/uuid.py` & `petisco-2.0.0rc1/petisco/base/domain/model/uuid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from uuid import uuid4
 
 import validators
-from pydantic import validator
+from pydantic import field_validator
 
 from petisco.base.domain.errors.defaults.invalid_uuid import InvalidUuid
 from petisco.base.domain.model.value_object import ValueObject
 
 
 class Uuid(ValueObject):
     """
     A base class to define Uuid
 
     Use it to identify domain entities
     """
 
     value: str
 
-    @validator("value")
+    @field_validator("value")
     def validate_value(cls, value: str) -> str:
         if value is None or not validators.uuid(value):
             raise InvalidUuid(uuid_value=value)
         return value
 
     @classmethod
     def v4(cls) -> "Uuid":
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/model/value_object.py` & `petisco-2.0.0rc1/petisco/base/domain/model/value_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, NoReturn, Type, TypeVar
 
-from pydantic import validator
+from pydantic import field_validator
 from pydantic.main import BaseModel
 
 from petisco.base.domain.errors.defaults.invalid_value_object import InvalidValueObject
 
 TypeValueObject = TypeVar("TypeValueObject", bound="ValueObject")
 
 
@@ -29,12 +29,12 @@
     def __hash__(self) -> int:
         return hash(self.value)
 
     @classmethod
     def from_value(cls: Type[TypeValueObject], value: Any) -> TypeValueObject:
         return cls(value=value)
 
-    @validator("value")
+    @field_validator("value")
     def validate_value(cls, value: Any) -> Any:
         if value is None:
             raise InvalidValueObject()
         return value
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/database.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/legacy_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from __future__ import annotations
-
 from abc import ABC, abstractmethod
-from typing import Any, Callable, ContextManager, Generic, TypeVar
-
-T = TypeVar("T")
+from typing import Any, Dict, List, Union
 
 
-class Database(Generic[T], ABC):
-    def __init__(self, name: str):
+class LegacyDatabase(ABC):
+    def __init__(self, name: str, models: Union[Dict[str, Any], None] = None):
         self.name = name
+        self.models = models if models else {}
 
-    def info(self) -> dict[str, Any]:
-        return {"name": self.name}
+    def info(self) -> Dict[str, Any]:
+        _info: Dict[str, Any] = {"name": self.name}
+        if self.models:
+            _info["models"] = self.models
+        return _info
 
     @abstractmethod
-    def initialize(self, *args: Any, **kwargs: Any) -> None:
+    def create(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def delete(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def clear_data(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def is_available(self) -> bool:
+    def get_model(self, model_name: str) -> Any:
         raise NotImplementedError
 
     @abstractmethod
-    def get_session_scope(self) -> Callable[..., ContextManager[T]]:
+    def get_model_names(self) -> List[str]:
         raise NotImplementedError
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/databases.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/persistence.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,162 +1,164 @@
-from __future__ import annotations
-
 import inspect
 from dataclasses import dataclass
-from typing import Any, Callable
+from typing import Any, Callable, Dict, List, Union
 
 from loguru import logger
 
-from petisco.base.domain.persistence.async_database import AsyncDatabase
-from petisco.base.domain.persistence.database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.base.misc.singleton import Singleton
 
 
 @dataclass
-class Databases(metaclass=Singleton):
+class Persistence(metaclass=Singleton):
     def __init__(self) -> None:
-        self._databases: dict[str, Any] = {}
+        self._databases: Dict[str, Any] = {}
 
     def __repr__(self) -> str:
-        return f"Databases: {str(self.get_info())}"
+        return f"Persistence: {str(self.get_info())}"
+
+    def get_info(self) -> Dict[str, Any]:
+        return {name: database.info() for name, database in self._databases.items()}
 
     @staticmethod
-    def get_instance() -> Databases:
+    def info() -> Dict[str, Any]:
+        return Persistence.get_instance().get_info()
+
+    @staticmethod
+    def get_instance() -> "Persistence":
         try:
-            return Databases()
+            return Persistence()
         except Exception as e:  # noqa E722
             frame_info = inspect.stack()[1]
             raise ImportError(
-                f"Databases must be configured. If not, you cannot obtain models\n"
-                f"Following code must be executed after Databases initialization:\n"
+                f"Persistence must be configured. If not, you cannot obtain models\n"
+                f"Following code must be executed after Persistence initialization:\n"
                 f"\tfilename: {frame_info.filename}\n"
                 f"\tlineno: {frame_info.lineno}\n"
                 f"\tfunction: {frame_info.function}\n"
                 f"\tcode_context: {frame_info.code_context}\n\n"
             )
 
+    def add(self, database: LegacyDatabase, skip_if_exist: bool = False) -> None:
+        if database.name in self._databases:
+            if skip_if_exist is False:
+                raise NameError(
+                    f"Database {database.name} is already added to Persistence"
+                )
+        else:
+            self._databases[database.name] = database
+
+    def remove(self, database_name: str, skip_if_not_exist: bool = False) -> None:
+        if database_name in self._databases:
+            self._databases[database_name].delete()
+            del self._databases[database_name]
+        else:
+            if skip_if_not_exist is False:
+                raise IndexError(
+                    f"Database cannot be removed. {database_name} not exists"
+                )
+
+    def create(self) -> None:
+        for database in self._databases.values():
+            database.create()
+
+    def delete(self) -> None:
+        for database in self._databases.values():
+            database.delete()
+
+    def clear_data(self, database_name: Union[str, None] = None) -> None:
+        databases = self._databases
+        if database_name is not None:
+            if database_name not in self._databases:
+                raise IndexError(
+                    f"Database cannot clear the data. {database_name} not exists"
+                )
+            databases = [self._databases.get(database_name)]
+        for database in databases.values():
+            database.clear_data()
+
     @staticmethod
-    def info() -> dict[str, Any]:
-        return Databases.get_instance().get_info()
+    def exist() -> bool:
+        databases = Persistence.get_instance()._databases
+        if len(databases) < 1:
+            return False
+        else:
+            return True
 
     @staticmethod
-    def _get_databases(database_name: str | None = None) -> dict[str, Database] | None:
-        databases = Databases.get_instance()._databases
+    def is_available(database_name: Union[str, None] = None) -> bool:
+        def log_warning(message: str) -> None:
+            logger.debug(message)
+
+        databases = Persistence.get_instance()._databases
         if database_name is not None:
             if database_name not in databases:
                 raise IndexError(
                     f"Database cannot return is_available. {database_name} not exists"
                 )
             databases = {database_name: databases.get(database_name)}
         if len(databases) < 1:
-            logger.warning("Databases databases are empty")
-            return None
-        return databases
-
-    @staticmethod
-    def are_available(database_name: str | None = None) -> bool:
-        databases = Databases._get_databases(database_name)
-        if databases is None:
+            log_warning("Persistence databases are empty")
             return False
-
         for database_name, database in databases.items():
-            if isinstance(database, AsyncDatabase):
-                continue
             if not database.is_available():
-                logger.warning(f"Database {database_name} is not available")
+                log_warning(f"Database {database_name} is not available")
                 return False
         return True
 
     @staticmethod
-    async def async_are_available(database_name: str | None = None) -> bool:
-        databases = Databases._get_databases(database_name)
-        if databases is None:
-            return False
+    def get_base(database_name: str) -> Any:
+        database = Persistence.get_instance()._databases.get(database_name)
+        if not database:
+            raise IndexError(f"Database name ({database_name}) not exists.")
 
-        for database_name, database in databases.items():
-            if not isinstance(database, AsyncDatabase):
-                continue
-            if not await database.is_available():
-                logger.warning(f"Database {database_name} is not available")
-                return False
-        return True
+        if not hasattr(database, "get_base"):
+            raise IndexError(f"Database ({database_name}) has not get_base method. ")
+
+        return database.get_base()
 
     @staticmethod
-    def get_databases() -> list[Database]:
-        return list(Databases.get_instance()._databases.values())
+    def get_databases() -> List[LegacyDatabase]:
+        return list(Persistence.get_instance()._databases.values())
 
     @staticmethod
-    def get_available_databases() -> list[str]:
-        return list(Databases.get_instance()._databases.keys())
+    def get_available_databases() -> List[str]:
+        return list(Persistence.get_instance()._databases.keys())
+
+    @staticmethod
+    def get_available_models_for_database(database_name: str) -> List[str]:
+        database = Persistence.get_instance()._databases.get(database_name)
+        if not database:
+            raise IndexError(f"Database name ({database_name}) not exists.")
+
+        return list(database.get_model_names())
+
+    @staticmethod
+    def get_model(database_name: str, model_name: str) -> Any:
+        database = Persistence.get_instance()._databases.get(database_name)
+        if not database:
+            raise IndexError(f"Database name ({database_name}) not exists.")
+        return database.get_model(model_name)
 
     @staticmethod
     def get_session(database_name: str) -> Any:
-        database = Databases.get_instance()._databases.get(database_name)
+        database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         if not hasattr(database, "get_session"):
             raise IndexError(f"Database ({database_name}) has not get_session method. ")
 
         return database.get_session()
 
     @staticmethod
     def get_session_scope(database_name: str) -> Callable[..., Any]:
-        database = Databases.get_instance()._databases.get(database_name)
+        database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         if not hasattr(database, "get_session_scope"):
             raise IndexError(
                 f"Database ({database_name}) has not get_session_scope method. "
             )
 
         return database.get_session_scope()
-
-    @staticmethod
-    def exist() -> bool:
-        databases = Databases.get_instance()._databases
-        if len(databases) < 1:
-            return False
-        else:
-            return True
-
-    def get_info(self) -> dict[str, Any]:
-        return {name: database.info() for name, database in self._databases.items()}
-
-    def add(self, database: Database, skip_if_exist: bool = False) -> None:
-        if database.name in self._databases:
-            if skip_if_exist is False:
-                raise NameError(
-                    f"Database {database.name} is already added to Databases"
-                )
-        else:
-            self._databases[database.name] = database
-
-    def remove(self, database_name: str, skip_if_not_exist: bool = False) -> None:
-        if database_name in self._databases:
-            self._databases[database_name].delete()
-            del self._databases[database_name]
-        else:
-            if skip_if_not_exist is False:
-                raise IndexError(
-                    f"Database cannot be removed. {database_name} not exists"
-                )
-
-    def initialize(self) -> None:
-        for database in self._databases.values():
-            database.initialize()
-
-    def delete(self) -> None:
-        for database in self._databases.values():
-            database.delete()
-
-    def clear_data(self, database_name: str | None = None) -> None:
-        databases = self._databases
-        if database_name is not None:
-            if database_name not in self._databases:
-                raise IndexError(
-                    f"Database cannot clear the data. {database_name} not exists"
-                )
-            databases = [self._databases.get(database_name)]
-        for database in databases.values():
-            database.clear_data()
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/fake_database.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/async_fake_database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 from typing import Any, Callable, ContextManager
 
-from petisco.base.domain.persistence.database import Database, T
+from petisco.base.domain.persistence.async_database import AsyncDatabase
+from petisco.base.domain.persistence.database import T
 
 
-class FakeDatabase(Database):
-    def __init__(self, name: str):
-        super().__init__(name)
-
+class AsyncFakeDatabase(AsyncDatabase):
     def initialize(self, *args: Any, **kwargs: Any) -> None:
         pass
 
     def delete(self) -> None:
         pass
 
     def clear_data(self) -> None:
         pass
 
-    def is_available(self) -> bool:
+    async def is_available(self) -> bool:
         pass
 
     def get_session_scope(self) -> Callable[..., ContextManager[T]]:
         pass
```

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_fake_database.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/legacy_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/persistence_models.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/persistence_models.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/domain/persistence/sql_base.py` & `petisco-2.0.0rc1/petisco/base/domain/persistence/sql_base.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/misc/async_wrapper.py` & `petisco-2.0.0rc1/petisco/base/misc/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/misc/builder.py` & `petisco-2.0.0rc1/petisco/base/misc/builder.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/misc/result_mapper.py` & `petisco-2.0.0rc1/petisco/base/misc/result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/misc/singleton.py` & `petisco-2.0.0rc1/petisco/base/misc/singleton.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/base/misc/wrapper.py` & `petisco-2.0.0rc1/petisco/base/misc/wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/cli/petisco.py` & `petisco-2.0.0rc1/petisco/cli/petisco.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/cli/petisco_dev.py` & `petisco-2.0.0rc1/petisco/cli/petisco_dev.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/cli/petisco_rabbitmq.py` & `petisco-2.0.0rc1/petisco/cli/petisco_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/__init__.py` & `petisco-2.0.0rc1/petisco/extra/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/async_elastic_database.py` & `petisco-2.0.0rc1/petisco/extra/elastic/async_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/elastic_connection.py` & `petisco-2.0.0rc1/petisco/extra/elastic/elastic_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/elastic_database.py` & `petisco-2.0.0rc1/petisco/extra/elastic/elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.0.0rc1/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic/legacy_elastic_database.py` & `petisco-2.0.0rc1/petisco/extra/elastic/legacy_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py` & `petisco-2.0.0rc1/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/fastapi/__init__.py` & `petisco-2.0.0rc1/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.0.0rc1/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/fastapi/testing/assert_http_exception.py` & `petisco-2.0.0rc1/petisco/extra/fastapi/testing/assert_http_exception.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/logger/__init__.py` & `petisco-2.0.0rc1/petisco/extra/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/logger/log_message.py` & `petisco-2.0.0rc1/petisco/extra/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/logger/logging_based_logger.py` & `petisco-2.0.0rc1/petisco/extra/logger/logging_based_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/logger/loguru_logger.py` & `petisco-2.0.0rc1/petisco/extra/logger/loguru_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/__init__.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 from petisco.extra.rabbitmq.shared.rabbitmq_exchange_name_formatter import (
     RabbitMqExchangeNameFormatter,
 )
 
 MAX_ATTEMPTS_TO_RECONNECT = int(
-    os.getenv("PETISCO_RABBITMQ_MAX_ATTEMPTS_TO_RECONNECT_CONSUMER", "20")
+    os.getenv("PETISCO_RABBITMQ_MAX_ATTEMPTS_TO_RECONNECT_CONSUMER", "30")
 )
 WAIT_SECONDS_TO_RECONNECT = int(
     os.getenv("PETISCO_RABBITMQ_WAIT_SECONDS_TO_RECONNECT_CONSUMER", "5")
 )
 
 
 @dataclass
```

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.0.0rc1/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_command_bus.py` & `petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py` & `petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_message_bus.py` & `petisco-2.0.0rc1/petisco/extra/redis/application/message/bus/redis_message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/__init__.py` & `petisco-2.0.0rc1/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc1/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc1/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.0.0rc1/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-2.0.0rc1/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/slack/dependencies.py` & `petisco-2.0.0rc1/petisco/extra/slack/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_database.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/async_sql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/base_sql_repository.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/base_sql_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_database.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 class SqlDatabase(Database[Session]):
 
     session_factory: sessionmaker | None = None
 
     def __init__(
         self,
-        name: str,
         connection: SqliteConnection | MySqlConnection,
         *,
+        alias: str | None = None,
         print_sql_statements: bool = False,
         use_scoped_session: bool = True,
         initial_statements_filename: str = None,
     ):
         self.connection = connection
         self.print_sql_statements = print_sql_statements
         self.use_scoped_session = use_scoped_session
         self.initial_statements_filename = initial_statements_filename
         self._check_connection()
-        super().__init__(name)
+        super().__init__(alias)
 
     def _check_connection(self) -> None:
         if not self.connection or not isinstance(
             self.connection, (SqliteConnection, MySqlConnection)
         ):
             raise ConnectionError(
                 "SqlDatabase needs a valid SqliteConnection or MySqlConnection connection"
@@ -94,24 +94,26 @@
                 for table in reversed(base.metadata.sorted_tables):
                     session.execute(table.delete())
         else:
             logger.warning(
                 "SqlDatabase do not implement clear_data to mitigate possible problems in production"
             )
 
-    def get_session_scope(self) -> Callable[..., ContextManager[Session]]:
+    def get_session_scope(self) -> Callable[..., ContextManager[T]]:
         if self.session_factory is None:
             raise RuntimeError(
                 "SqlDatabase must run initialize() before get_session_scope()"
             )
 
         if self.use_scoped_session:
-            Session = scoped_session(self.session_factory)  # noqa
+            Session: Callable[..., Session] = scoped_session(
+                self.session_factory
+            )  # noqa
         else:
-            Session = self.session_factory  # noqa
+            Session: Callable[..., Session] = self.session_factory  # noqa
         return sql_session_scope_provider(Session)
 
     def is_available(self):
         try:
             context = self.get_session_scope()
             with context() as session:
                 session.execute(text("SELECT 1"))
```

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py` & `petisco-2.0.0rc1/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.0.0rc1/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/extra/threading/pool_executor.py` & `petisco-2.0.0rc1/petisco/extra/threading/pool_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/petisco/public_api.py` & `petisco-2.0.0rc1/petisco/public_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from petisco.base.domain.message.not_implemented_message_configurer import (
     NotImplementedMessageConfigurer,
 )
 from petisco.base.domain.model.aggregate_root import AggregateRoot
 from petisco.base.domain.model.uuid import Uuid
 from petisco.base.domain.model.value_object import ValueObject
 from petisco.base.domain.persistence.database import Database
-from petisco.base.domain.persistence.databases import Databases
+from petisco.base.domain.persistence.databases import databases
 from petisco.base.domain.persistence.persistence import Persistence
 from petisco.base.domain.persistence.persistence_models import PersistenceModels
 from petisco.base.domain.persistence.sql_base import SqlBase
 from petisco.base.misc.builder import Builder
 from petisco.base.misc.interface import Interface
 from petisco.base.misc.result_mapper import ResultMapper
 from petisco.base.misc.singleton import Singleton
@@ -132,15 +132,15 @@
     "Uuid",
     "Interface",
     "DomainEventSubscriber",
     "CommandSubscriber",
     "AllMessageSubscriber",
     "Persistence",
     "PersistenceModels",
-    "Databases",
+    "databases",
     "Database",
     "SqlBase",
     "Repository",
     "CrudRepository",
     "InmemoryCrudRepository",
     "AppService",
     "AsyncAppService",
```

### Comparing `petisco-2.0.0rc0/petisco.egg-info/PKG-INFO` & `petisco-2.0.0rc1/petisco.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
@@ -37,17 +37,21 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![license](https://img.shields.io/github/license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/petisco/blob/main/LICENSE)
 [![versions](https://img.shields.io/pypi/pyversions/petisco.svg)](https://github.com/alice-biometrics/petisco)
 
 <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true" width=auto>
 
 > **Warning**
-> Disclaimer:
-> Current version now is v1 (not stable yet). 
-> v0 is now deprecated (legacy branch)
+> 
+> Current version now is v1 (*v1 branch*). 
+> 
+> v0 is now deprecated (*legacy branch*)
+> 
+> v2 is about to be release (*main branch*). 1 release candidate
+
 
 ---
 
 **Documentation**: <a href="https://alice-biometrics.github.io/petisco/" target="_blank">https://alice-biometrics.github.io/petisco/</a>
 
 **Source Code**: <a href="https://github.com/alice-biometrics/petisco" target="_blank">https://github.com/alice-biometrics/petisco</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc0 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc1 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -23,20 +23,21 @@
 000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) [![license](https://img.shields.io/github/
 license/alice-biometrics/petisco.svg)](https://github.com/alice-biometrics/
 petisco/blob/main/LICENSE) [![versions](https://img.shields.io/pypi/pyversions/
 petisco.svg)](https://github.com/alice-biometrics/petisco) [https://github.com/
 alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true] >
-**Warning** > Disclaimer: > Current version now is v1 (not stable yet). > v0 is
-now deprecated (legacy branch) --- **Documentation**: https://alice-
-biometrics.github.io/petisco/ **Source Code**: https://github.com/alice-
-biometrics/petisco --- ## What is petisco? ðª petisco is a framework for
-helping Python developers to build clean Applications in Python. ## How could
-petisco help me? ðª petisco provides several handy classes to help you on
-defining your domain with hexagonal architecture, event streaming and CQRS. ##
-Installation ð» ```console pip install petisco ``` Installation with Extras
-```console pip install petisco[fastapi,sqlalchemy,elastic,elastic-
-apm,rabbitmq,slack,redis] ``` ## Contribute We'd love you to contribute to
-*petisco* ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our
-[documentation](https://alice-biometrics.github.io/petisco/contributing/) ##
-Contact ð¬ support@alicebiometrics.com
+**Warning** > > Current version now is v1 (*v1 branch*). > > v0 is now
+deprecated (*legacy branch*) > > v2 is about to be release (*main branch*). 1
+release candidate --- **Documentation**: https://alice-biometrics.github.io/
+petisco/ **Source Code**: https://github.com/alice-biometrics/petisco --- ##
+What is petisco? ðª petisco is a framework for helping Python developers to
+build clean Applications in Python. ## How could petisco help me? ðª petisco
+provides several handy classes to help you on defining your domain with
+hexagonal architecture, event streaming and CQRS. ## Installation ð»
+```console pip install petisco ``` Installation with Extras ```console pip
+install petisco[fastapi,sqlalchemy,elastic,elastic-apm,rabbitmq,slack,redis]
+``` ## Contribute We'd love you to contribute to *petisco*
+ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our [documentation]
+(https://alice-biometrics.github.io/petisco/contributing/) ## Contact ð¬
+support@alicebiometrics.com
```

### Comparing `petisco-2.0.0rc0/petisco.egg-info/SOURCES.txt` & `petisco-2.0.0rc1/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/setup.cfg` & `petisco-2.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc0/setup.py` & `petisco-2.0.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,11 +56,11 @@
         "rabbitmq": ["pika==1.3.2"],
         "slack": ["slack_sdk<4.0.0,>=3.20.2"],
         "elastic": [
             "elasticsearch[async]<8.0.0,>=7.13.1",
             "elastic-apm<7.0.0,>=6.15.1",
         ],
         "elastic-apm": ["elastic-apm<7.0.0,>=6.15.1"],
-        "fastapi": ["fastapi<1.0.0,>=0.95.2"],
+        "fastapi": ["fastapi<1.0.0,>=0.100.0b1"],
         "rich": ["rich"],
     },
 )
```

### Comparing `petisco-2.0.0rc0/tests/fixtures.py` & `petisco-2.0.0rc1/tests/fixtures.py`

 * *Files identical despite different names*

