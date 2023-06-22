# Comparing `tmp/meliorator-0.9.16.tar.gz` & `tmp/meliorator-0.9.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meliorator-0.9.16.tar", max compression
+gzip compressed data, was "meliorator-0.9.17.tar", max compression
```

## Comparing `meliorator-0.9.16.tar` & `meliorator-0.9.17.tar`

### file list

```diff
@@ -1,147 +1,146 @@
--rw-r--r--   0        0        0     1062 2023-03-10 21:09:44.651085 meliorator-0.9.16/LICENSE
--rw-r--r--   0        0        0    20599 2023-03-10 21:09:44.651085 meliorator-0.9.16/README.rst
--rw-r--r--   0        0        0      298 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-03-10 21:09:44.651085 meliorator-0.9.16/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/__init__.py
--rw-r--r--   0        0        0    15175 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2095 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/connector.py
--rw-r--r--   0        0        0     3886 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2065 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1254 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-03-10 21:09:44.655086 meliorator-0.9.16/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23246 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-03-10 21:09:44.659086 meliorator-0.9.16/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13604 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/__init__.py
--rw-r--r--   0        0        0    43978 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/__init__.py
--rw-r--r--   0        0        0    19840 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7304 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-03-10 21:09:44.663086 meliorator-0.9.16/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-03-10 21:09:44.667086 meliorator-0.9.16/orator/utils/url.py
--rw-r--r--   0        0        0     1282 2023-03-10 21:09:44.667086 meliorator-0.9.16/pyproject.toml
--rw-r--r--   0        0        0    23872 1970-01-01 00:00:00.000000 meliorator-0.9.16/setup.py
--rw-r--r--   0        0        0    22356 1970-01-01 00:00:00.000000 meliorator-0.9.16/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-22 17:37:17.956223 meliorator-0.9.17/LICENSE
+-rw-r--r--   0        0        0    20599 2023-06-22 17:37:17.956223 meliorator-0.9.17/README.rst
+-rw-r--r--   0        0        0      298 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/application.py
+-rw-r--r--   0        0        0     3453 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15175 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2095 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3886 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2065 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-06-22 17:37:17.956223 meliorator-0.9.17/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1254 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-06-22 17:37:17.960223 meliorator-0.9.17/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23246 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13604 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/__init__.py
+-rw-r--r--   0        0        0    43978 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-06-22 17:37:17.964223 meliorator-0.9.17/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19840 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7304 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-06-22 17:37:17.968223 meliorator-0.9.17/orator/utils/url.py
+-rw-r--r--   0        0        0     1283 2023-06-22 17:37:17.968223 meliorator-0.9.17/pyproject.toml
+-rw-r--r--   0        0        0    22163 1970-01-01 00:00:00.000000 meliorator-0.9.17/PKG-INFO
```

### Comparing `meliorator-0.9.16/LICENSE` & `meliorator-0.9.17/LICENSE`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/README.rst` & `meliorator-0.9.17/README.rst`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/application.py` & `meliorator-0.9.17/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/command.py` & `meliorator-0.9.17/orator/commands/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         if not path:
             path = self.option("config")
 
         filename, ext = os.path.splitext(path)
         if ext in [".yml", ".yaml"]:
             with open(path) as fd:
-                config = yaml.load(fd)
+                config = yaml.load(fd, yaml.FullLoader)
         elif ext in [".py"]:
             config = {}
 
             with open(path) as fh:
                 exec(fh.read(), {}, config)
         else:
             raise RuntimeError("Config file [%s] is not supported." % path)
```

### Comparing `meliorator-0.9.16/orator/commands/migrations/install_command.py` & `meliorator-0.9.17/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/make_command.py` & `meliorator-0.9.17/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/migrate_command.py` & `meliorator-0.9.17/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/refresh_command.py` & `meliorator-0.9.17/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/reset_command.py` & `meliorator-0.9.17/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/rollback_command.py` & `meliorator-0.9.17/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/migrations/status_command.py` & `meliorator-0.9.17/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/models/make_command.py` & `meliorator-0.9.17/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/seeds/make_command.py` & `meliorator-0.9.17/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/commands/seeds/seed_command.py` & `meliorator-0.9.17/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connections/connection.py` & `meliorator-0.9.17/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connections/connection_interface.py` & `meliorator-0.9.17/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connections/mysql_connection.py` & `meliorator-0.9.17/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connections/postgres_connection.py` & `meliorator-0.9.17/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connections/sqlite_connection.py` & `meliorator-0.9.17/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connectors/connection_factory.py` & `meliorator-0.9.17/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connectors/connector.py` & `meliorator-0.9.17/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connectors/mysql_connector.py` & `meliorator-0.9.17/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connectors/postgres_connector.py` & `meliorator-0.9.17/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/connectors/sqlite_connector.py` & `meliorator-0.9.17/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/database_manager.py` & `meliorator-0.9.17/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/abstract_asset.py` & `meliorator-0.9.17/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/column.py` & `meliorator-0.9.17/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/column_diff.py` & `meliorator-0.9.17/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/comparator.py` & `meliorator-0.9.17/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/exceptions/__init__.py` & `meliorator-0.9.17/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/foreign_key_constraint.py` & `meliorator-0.9.17/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/index.py` & `meliorator-0.9.17/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/mysql_schema_manager.py` & `meliorator-0.9.17/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/keywords/mysql_keywords.py` & `meliorator-0.9.17/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/keywords/postgresql_keywords.py` & `meliorator-0.9.17/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/keywords/sqlite_keywords.py` & `meliorator-0.9.17/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/mysql57_platform.py` & `meliorator-0.9.17/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/mysql_platform.py` & `meliorator-0.9.17/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/platform.py` & `meliorator-0.9.17/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/postgres_platform.py` & `meliorator-0.9.17/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/platforms/sqlite_platform.py` & `meliorator-0.9.17/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/postgres_schema_manager.py` & `meliorator-0.9.17/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/schema_manager.py` & `meliorator-0.9.17/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/sqlite_schema_manager.py` & `meliorator-0.9.17/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/table.py` & `meliorator-0.9.17/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/dbal/table_diff.py` & `meliorator-0.9.17/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/events/__init__.py` & `meliorator-0.9.17/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/exceptions/connectors.py` & `meliorator-0.9.17/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/exceptions/orm.py` & `meliorator-0.9.17/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/migrations/database_migration_repository.py` & `meliorator-0.9.17/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/migrations/migration_creator.py` & `meliorator-0.9.17/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/migrations/migrator.py` & `meliorator-0.9.17/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/migrations/stubs.py` & `meliorator-0.9.17/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/builder.py` & `meliorator-0.9.17/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/collection.py` & `meliorator-0.9.17/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/factory.py` & `meliorator-0.9.17/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/factory_builder.py` & `meliorator-0.9.17/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/mixins/soft_deletes.py` & `meliorator-0.9.17/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/model.py` & `meliorator-0.9.17/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/belongs_to.py` & `meliorator-0.9.17/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/belongs_to_many.py` & `meliorator-0.9.17/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/has_many.py` & `meliorator-0.9.17/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/has_many_through.py` & `meliorator-0.9.17/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/has_one.py` & `meliorator-0.9.17/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/has_one_or_many.py` & `meliorator-0.9.17/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_many.py` & `meliorator-0.9.17/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_one.py` & `meliorator-0.9.17/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_one_or_many.py` & `meliorator-0.9.17/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_pivot.py` & `meliorator-0.9.17/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_to.py` & `meliorator-0.9.17/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/morph_to_many.py` & `meliorator-0.9.17/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/pivot.py` & `meliorator-0.9.17/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/relation.py` & `meliorator-0.9.17/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/result.py` & `meliorator-0.9.17/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/relations/wrapper.py` & `meliorator-0.9.17/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/scopes/soft_deleting.py` & `meliorator-0.9.17/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/orm/utils.py` & `meliorator-0.9.17/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/pagination/base.py` & `meliorator-0.9.17/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/pagination/length_aware_paginator.py` & `meliorator-0.9.17/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/pagination/paginator.py` & `meliorator-0.9.17/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/builder.py` & `meliorator-0.9.17/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/grammars/grammar.py` & `meliorator-0.9.17/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/grammars/mysql_grammar.py` & `meliorator-0.9.17/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/grammars/postgres_grammar.py` & `meliorator-0.9.17/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/grammars/sqlite_grammar.py` & `meliorator-0.9.17/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/join_clause.py` & `meliorator-0.9.17/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/processors/mysql_processor.py` & `meliorator-0.9.17/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/processors/postgres_processor.py` & `meliorator-0.9.17/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/query/processors/processor.py` & `meliorator-0.9.17/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/blueprint.py` & `meliorator-0.9.17/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/builder.py` & `meliorator-0.9.17/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/grammars/grammar.py` & `meliorator-0.9.17/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/grammars/mysql_grammar.py` & `meliorator-0.9.17/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/grammars/postgres_grammar.py` & `meliorator-0.9.17/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/grammars/sqlite_grammar.py` & `meliorator-0.9.17/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/mysql_builder.py` & `meliorator-0.9.17/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/schema/schema.py` & `meliorator-0.9.17/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/seeds/seeder.py` & `meliorator-0.9.17/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/support/fluent.py` & `meliorator-0.9.17/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/support/grammar.py` & `meliorator-0.9.17/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/utils/__init__.py` & `meliorator-0.9.17/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/utils/command_formatter.py` & `meliorator-0.9.17/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/utils/helpers.py` & `meliorator-0.9.17/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/utils/qmarker.py` & `meliorator-0.9.17/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/orator/utils/url.py` & `meliorator-0.9.17/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `meliorator-0.9.16/pyproject.toml` & `meliorator-0.9.17/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meliorator"
-version = "0.9.16"
+version = "0.9.17"
 description = "This is a fork from Orator ORM used by Méliuz."
 
 license = "MIT"
 
 authors = [
     "Sébastien Eustace <sebastien@eustace.io>"
 ]
@@ -21,24 +21,24 @@
 keywords = ['database', 'orm']
 
 packages = [
     { include = "orator", from = "." }
 ]
 
 [tool.poetry.dependencies]
-python = "~2.7 || ^3.5"
+python = ">=3.6"
 backpack = "^0.1"
 blinker = "^1.4"
 cleo = "^0.6"
 inflection = "^0.3"
 Faker = "^0.8"
 lazy-object-proxy = "^1.2"
 pendulum = "^1.4"
 pyaml = "^16.12"
-pyyaml = "^5.1"
+pyyaml = ">= 5.1, <7.0"
 Pygments = "^2.2"
 simplejson = "^3.10"
 six = "^1.10"
 wrapt = "^1.10"
 
 # Extras
 psycopg2 = { version = "^2.7", optional = true }
```

### Comparing `meliorator-0.9.16/setup.py` & `meliorator-0.9.17/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,911 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: meliorator
+Version: 0.9.17
+Summary: This is a fork from Orator ORM used by Méliuz.
+Home-page: https://orator-orm.com/
+License: MIT
+Keywords: database,orm
+Author: Sébastien Eustace
+Author-email: sebastien@eustace.io
+Maintainer: Matheus Oliveira
+Maintainer-email: mco@meliuz.com.br
+Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: mysql
+Provides-Extra: mysql-python
+Provides-Extra: pgsql
+Requires-Dist: Faker (>=0.8,<0.9)
+Requires-Dist: PyMySQL (>=0.7,<0.8) ; extra == "mysql-python"
+Requires-Dist: Pygments (>=2.2,<3.0)
+Requires-Dist: backpack (>=0.1,<0.2)
+Requires-Dist: blinker (>=1.4,<2.0)
+Requires-Dist: cleo (>=0.6,<0.7)
+Requires-Dist: inflection (>=0.3,<0.4)
+Requires-Dist: lazy-object-proxy (>=1.2,<2.0)
+Requires-Dist: mysqlclient (>=1.3,<2.0) ; extra == "mysql"
+Requires-Dist: pendulum (>=1.4,<2.0)
+Requires-Dist: psycopg2 (>=2.7,<3.0) ; extra == "pgsql"
+Requires-Dist: pyaml (>=16.12,<17.0)
+Requires-Dist: pyyaml (>=5.1,<7.0)
+Requires-Dist: simplejson (>=3.10,<4.0)
+Requires-Dist: six (>=1.10,<2.0)
+Requires-Dist: wrapt (>=1.10,<2.0)
+Project-URL: Repository, https://github.com/meliuz/meliorator
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': '.'}
+Orator
+######
 
-packages = \
-['orator',
- 'orator.commands',
- 'orator.commands.migrations',
- 'orator.commands.models',
- 'orator.commands.seeds',
- 'orator.connections',
- 'orator.connectors',
- 'orator.dbal',
- 'orator.dbal.exceptions',
- 'orator.dbal.platforms',
- 'orator.dbal.platforms.keywords',
- 'orator.dbal.types',
- 'orator.events',
- 'orator.exceptions',
- 'orator.migrations',
- 'orator.orm',
- 'orator.orm.mixins',
- 'orator.orm.relations',
- 'orator.orm.scopes',
- 'orator.pagination',
- 'orator.query',
- 'orator.query.grammars',
- 'orator.query.processors',
- 'orator.schema',
- 'orator.schema.grammars',
- 'orator.seeds',
- 'orator.support',
- 'orator.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Faker>=0.8,<0.9',
- 'Pygments>=2.2,<3.0',
- 'backpack>=0.1,<0.2',
- 'blinker>=1.4,<2.0',
- 'cleo>=0.6,<0.7',
- 'inflection>=0.3,<0.4',
- 'lazy-object-proxy>=1.2,<2.0',
- 'pendulum>=1.4,<2.0',
- 'pyaml>=16.12,<17.0',
- 'pyyaml>=5.1,<6.0',
- 'simplejson>=3.10,<4.0',
- 'six>=1.10,<2.0',
- 'wrapt>=1.10,<2.0']
-
-extras_require = \
-{'mysql': ['mysqlclient>=1.3,<2.0'],
- 'mysql-python': ['PyMySQL>=0.7,<0.8'],
- 'pgsql': ['psycopg2>=2.7,<3.0']}
-
-entry_points = \
-{'console_scripts': ['orator = orator.commands.application:application.run']}
-
-setup_kwargs = {
-    'name': 'meliorator',
-    'version': '0.9.16',
-    'description': 'This is a fork from Orator ORM used by Méliuz.',
-    'long_description': 'Orator\n######\n\n.. image:: https://travis-ci.org/sdispater/orator.png\n   :alt: Orator Build status\n   :target: https://travis-ci.org/sdispater/orator\n\nThe Orator ORM provides a simple yet beautiful ActiveRecord implementation.\n\nIt is inspired by the database part of the `Laravel framework <http://laravel.com>`_,\nbut largely modified to be more pythonic.\n\nThe full documentation is available here: http://orator-orm.com/docs\n\n\nInstallation\n============\n\nYou can install Orator in 2 different ways:\n\n* The easier and more straightforward is to use pip\n\n.. code-block:: bash\n\n    pip install orator\n\n* Install from source using the official repository (https://github.com/sdispater/orator)\n\nThe different dbapi packages are not part of the package dependencies,\nso you must install them in order to connect to corresponding databases:\n\n* Postgres: ``psycopg2``\n* MySQL: ``PyMySQL`` or ``mysqlclient``\n* Sqlite: The ``sqlite3`` module is bundled with Python by default\n\n\nBasic Usage\n===========\n\nConfiguration\n-------------\n\nAll you need to get you started is the configuration describing your database connections\nand passing it to a ``DatabaseManager`` instance.\n\n.. code-block:: python\n\n    from orator import DatabaseManager, Model\n\n    config = {\n        \'mysql\': {\n            \'driver\': \'mysql\',\n            \'host\': \'localhost\',\n            \'database\': \'database\',\n            \'user\': \'root\',\n            \'password\': \'\',\n            \'prefix\': \'\'\n        }\n    }\n\n    db = DatabaseManager(config)\n    Model.set_connection_resolver(db)\n\n\nDefining a model\n----------------\n\n.. code-block:: python\n\n    class User(Model):\n        pass\n\nNote that we did not tell the ORM which table to use for the ``User`` model. The plural "snake case" name of the\nclass name will be used as the table name unless another name is explicitly specified.\nIn this case, the ORM will assume the ``User`` model stores records in the ``users`` table.\nYou can specify a custom table by defining a ``__table__`` property on your model:\n\n.. code-block:: python\n\n    class User(Model):\n\n        __table__ = \'my_users\'\n\nThe ORM will also assume that each table has a primary key column named ``id``.\nYou can define a ``__primary_key__`` property to override this convention.\nLikewise, you can define a ``__connection__`` property to override the name of the database\nconnection that should be used when using the model.\n\nOnce a model is defined, you are ready to start retrieving and creating records in your table.\nNote that you will need to place ``updated_at`` and ``created_at`` columns on your table by default.\nIf you do not wish to have these columns automatically maintained,\nset the ``__timestamps__`` property on your model to ``False``.\n\n\nRetrieving all models\n---------------------\n\n.. code-block:: python\n\n    users = User.all()\n\n\nRetrieving a record by primary key\n----------------------------------\n\n.. code-block:: python\n\n    user = User.find(1)\n\n    print(user.name)\n\n\nQuerying using models\n---------------------\n\n.. code-block:: python\n\n    users = User.where(\'votes\', \'>\', 100).take(10).get()\n\n    for user in users:\n        print(user.name)\n\n\nAggregates\n----------\n\nYou can also use the query builder aggregate functions:\n\n.. code-block:: python\n\n    count = User.where(\'votes\', \'>\', 100).count()\n\nIf you feel limited by the builder\'s fluent interface, you can use the ``where_raw`` method:\n\n.. code-block:: python\n\n    users = User.where_raw(\'age > ? and votes = 100\', [25]).get()\n\n\nChunking Results\n----------------\n\nIf you need to process a lot of records, you can use the ``chunk`` method to avoid\nconsuming a lot of RAM:\n\n.. code-block:: python\n\n    for users in User.chunk(100):\n        for user in users:\n            # ...\n\n\nSpecifying the query connection\n-------------------------------\n\nYou can specify which database connection to use when querying a model by using the ``on`` method:\n\n.. code-block:: python\n\n    user = User.on(\'connection-name\').find(1)\n\nIf you are using read / write connections, you can force the query to use the "write" connection\nwith the following method:\n\n.. code-block:: python\n\n    user = User.on_write_connection().find(1)\n\n\nMass assignment\n===============\n\nWhen creating a new model, you pass attributes to the model constructor.\nThese attributes are then assigned to the model via mass-assignment.\nThough convenient, this can be a serious security concern when passing user input into a model,\nsince the user is then free to modify **any** and **all** of the model\'s attributes.\nFor this reason, all models protect against mass-assignment by default.\n\nTo get started, set the ``__fillable__`` or ``__guarded__`` properties on your model.\n\n\nDefining fillable attributes on a model\n---------------------------------------\n\nThe ``__fillable__`` property specifies which attributes can be mass-assigned.\n\n.. code-block:: python\n\n    class User(Model):\n\n        __fillable__ = [\'first_name\', \'last_name\', \'email\']\n\n\nDefining guarded attributes on a model\n--------------------------------------\n\nThe ``__guarded__`` is the inverse and acts as "blacklist".\n\n.. code-block:: python\n\n    class User(Model):\n\n        __guarded__ = [\'id\', \'password\']\n\n\nYou can also block **all** attributes from mass-assignment:\n\n.. code-block:: python\n\n    __guarded__ = [\'*\']\n\n\nInsert, update and delete\n=========================\n\n\nSaving a new model\n------------------\n\nTo create a new record in the database, simply create a new model instance and call the ``save`` method.\n\n.. code-block:: python\n\n    user = User()\n\n    user.name = \'John\'\n\n    user.save()\n\nYou can also use the ``create`` method to save a model in a single line, but you will need to specify\neither the ``__fillable__`` or ``__guarded__`` property on the model since all models are protected against\nmass-assignment by default.\n\nAfter saving or creating a new model with auto-incrementing IDs, you can retrieve the ID by accessing\nthe object\'s ``id`` attribute:\n\n.. code-block:: python\n\n    inserted_id = user.id\n\n\nUsing the create method\n-----------------------\n\n.. code-block:: python\n\n    # Create a new user in the database\n    user = User.create(name=\'John\')\n\n    # Retrieve the user by attributes, or create it if it does not exist\n    user = User.first_or_create(name=\'John\')\n\n    # Retrieve the user by attributes, or instantiate it if it does not exist\n    user = User.first_or_new(name=\'John\')\n\n\nUpdating a retrieved model\n--------------------------\n\n.. code-block:: python\n\n    user = User.find(1)\n\n    user.name = \'Foo\'\n\n    user.save()\n\nYou can also run updates as queries against a set of models:\n\n.. code-block:: python\n\n    affected_rows = User.where(\'votes\', \'>\', 100).update(status=2)\n\n..\n    TODO: push method\n\n\nDeleting an existing model\n--------------------------\n\nTo delete a model, simply call the ``delete`` model:\n\n.. code-block:: python\n\n    user = User.find(1)\n\n    user.delete()\n\n\nDeleting an existing model by key\n---------------------------------\n\n.. code-block:: python\n\n    User.destroy(1)\n\n    User.destroy(1, 2, 3)\n\nYou can also run a delete query on a set of models:\n\n.. code-block:: python\n\n    affected_rows = User.where(\'votes\', \'>\' 100).delete()\n\n\nUpdating only the model\'s timestamps\n------------------------------------\n\nIf you want to only update the timestamps on a model, you can use the ``touch`` method:\n\n.. code-block:: python\n\n    user.touch()\n\n\nTimestamps\n==========\n\nBy default, the ORM will maintain the ``created_at`` and ``updated_at`` columns on your database table\nautomatically. Simply add these ``timestamp`` columns to your table. If you do not wish for the ORM to maintain\nthese columns, just add the ``__timestamps__`` property:\n\n.. code-block:: python\n\n    class User(Model):\n\n        __timestamps__ = False\n\n\nProviding a custom timestamp format\n-----------------------------------\n\nIf you wish to customize the format of your timestamps (the default is the ISO Format) that will be returned when using the ``to_dict``\nor the ``to_json`` methods, you can override the ``get_date_format`` method:\n\n.. code-block:: python\n\n    class User(Model):\n\n        def get_date_format():\n            return \'DD-MM-YY\'\n\n\nConverting to dictionaries / JSON\n=================================\n\nConverting a model to a dictionary\n----------------------------------\n\nWhen building JSON APIs, you may often need to convert your models and relationships to dictionaries or JSON.\nSo, Orator includes methods for doing so. To convert a model and its loaded relationship to a dictionary,\nyou may use the ``to_dict`` method:\n\n.. code-block:: python\n\n    user = User.with_(\'roles\').first()\n\n    return user.to_dict()\n\nNote that entire collections of models can also be converted to dictionaries:\n\n.. code-block:: python\n\n    return User.all().serailize()\n\n\nConverting a model to JSON\n--------------------------\n\nTo convert a model to JSON, you can use the ``to_json`` method!\n\n.. code-block:: python\n\n    return User.find(1).to_json()\n\n\nQuery Builder\n=============\n\n\nIntroduction\n------------\n\nThe database query builder provides a fluent interface to create and run database queries.\nIt can be used to perform most database operations in your application, and works on all supported database systems.\n\n\nSelects\n-------\n\nRetrieving all row from a table\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').get()\n\n    for user in users:\n        print(user[\'name\'])\n\n\nChunking results from a table\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    for users in db.table(\'users\').chunk(100):\n        for user in users:\n            # ...\n\n\nRetrieving a single row from a table\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    user = db.table(\'users\').where(\'name\', \'John\').first()\n    print(user[\'name\'])\n\nRetrieving a single column from a row\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    user = db.table(\'users\').where(\'name\', \'John\').pluck(\'name\')\n\nRetrieving a list of column values\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    roles = db.table(\'roles\').lists(\'title\')\n\nThis method will return a list of role titles. It can return a dictionary\nif you pass an extra key parameter.\n\n.. code-block:: python\n\n    roles = db.table(\'roles\').lists(\'title\', \'name\')\n\nSpecifying a select clause\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').select(\'name\', \'email\').get()\n\n    users = db.table(\'users\').distinct().get()\n\n    users = db.table(\'users\').select(\'name as user_name\').get()\n\nAdding a select clause to an existing query\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    query = db.table(\'users\').select(\'name\')\n\n    users = query.add_select(\'age\').get()\n\nUsing where operators\n~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where(\'age\', \'>\', 25).get()\n\nOr statements\n~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where(\'age\', \'>\', 25).or_where(\'name\', \'John\').get()\n\nUsing Where Between\n~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where_between(\'age\', [25, 35]).get()\n\nUsing Where Not Between\n~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where_not_between(\'age\', [25, 35]).get()\n\nUsing Where In\n~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where_in(\'id\', [1, 2, 3]).get()\n\n    users = db.table(\'users\').where_not_in(\'id\', [1, 2, 3]).get()\n\nUsing Where Null to find records with null values\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').where_null(\'updated_at\').get()\n\nOrder by, group by and having\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    query = db.table(\'users\').order_by(\'name\', \'desc\')\n    query = query.group_by(\'count\')\n    query = query.having(\'count\', \'>\', 100)\n\n    users = query.get()\n\nOffset and limit\n~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    users = db.table(\'users\').skip(10).take(5).get()\n\n    users = db.table(\'users\').offset(10).limit(5).get()\n\n\nJoins\n-----\n\nThe query builder can also be used to write join statements.\n\nBasic join statement\n~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\') \\\n        .join(\'contacts\', \'users.id\', \'=\', \'contacts.user_id\') \\\n        .join(\'orders\', \'users.id\', \'=\', \'orders.user_id\') \\\n        .select(\'users.id\', \'contacts.phone\', \'orders.price\') \\\n        .get()\n\nLeft join statement\n~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').left_join(\'posts\', \'users.id\', \'=\', \'posts.user_id\').get()\n\nYou can also specify more advance join clauses:\n\n.. code-block:: python\n\n    clause = JoinClause(\'contacts\').on(\'users.id\', \'=\', \'contacts.user_id\').or_on(...)\n\n    db.table(\'users\').join(clause).get()\n\nIf you would like to use a "where" style clause on your joins,\nyou may use the ``where`` and ``or_where`` methods on a join.\nInstead of comparing two columns, these methods will compare the column against a value:\n\n\n.. code-block:: python\n\n    clause = JoinClause(\'contacts\').on(\'users.id\', \'=\', \'contacts.user_id\').where(\'contacts.user_id\', \'>\', 5)\n\n    db.table(\'users\').join(clause).get()\n\n\nAdvanced where\n--------------\n\nSometimes you may need to create more advanced where clauses such as "where exists" or nested parameter groupings.\nIt is pretty easy to do with the Orator query builder\n\nParameter grouping\n~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\') \\\n        .where(\'name\', \'=\', \'John\') \\\n        .or_where(\n            db.query().where(\'votes\', \'>\', 100).where(\'title\', \'!=\', \'admin\')\n        ).get()\n\nThe query above will produce the following SQL:\n\n.. code-block:: sql\n\n    SELECT * FROM users WHERE name = \'John\' OR (votes > 100 AND title != \'Admin\')\n\nExists statement\n~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').where_exists(\n        db.table(\'orders\').select(db.raw(1)).where_raw(\'order.user_id = users.id\')\n    )\n\nThe query above will produce the following SQL:\n\n.. code-block:: sql\n\n    SELECT * FROM users\n    WHERE EXISTS (\n        SELECT 1 FROM orders WHERE orders.user_id = users.id\n    )\n\n\nAggregates\n----------\n\nThe query builder also provides a variety of aggregate methods, `\nsuch as ``count``, ``max``, ``min``, ``avg``, and ``sum``.\n\n.. code-block:: python\n\n    users = db.table(\'users\').count()\n\n    price = db.table(\'orders\').max(\'price\')\n\n    price = db.table(\'orders\').min(\'price\')\n\n    price = db.table(\'orders\').avg(\'price\')\n\n    total = db.table(\'users\').sum(\'votes\')\n\n\nRaw expressions\n---------------\n\nSometimes you may need to use a raw expression in a query.\nThese expressions will be injected into the query as strings, so be careful not to create any SQL injection points!\nTo create a raw expression, you may use the ``raw()`` method:\n\n.. code-block:: python\n\n    db.table(\'users\') \\\n        .select(db.raw(\'count(*) as user_count, status\')) \\\n        .where(\'status\', \'!=\', 1) \\\n        .group_by(\'status\') \\\n        .get()\n\n\nInserts\n-------\n\nInsert records into a table\n~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').insert(email=\'foo@bar.com\', votes=0)\n\n    db.table(\'users\').insert({\n        \'email\': \'foo@bar.com\',\n        \'votes\': 0\n    })\n\n\nIt is important to note that there is two notations available.\nThe reason is quite simple: the dictionary notation, though a little less practical, is here to handle\ncolumns names which cannot be passed as keywords arguments.\n\nInserting records into a table with an auto-incrementing ID\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nIf the table has an auto-incrementing id, use ``insert_get_id`` to insert a record and retrieve the id:\n\n.. code-block:: python\n\n    id = db.table(\'users\').insert_get_id({\n        \'email\': \'foo@bar.com\',\n        \'votes\': 0\n    })\n\nInserting multiple record into a table\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').insert([\n        {\'email\': \'foo@bar.com\', \'votes\': 0},\n        {\'email\': \'bar@baz.com\', \'votes\': 0}\n    ])\n\nUpdates\n-------\n\nUpdating records\n~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').where(\'id\', 1).update(votes=1)\n\n    db.table(\'users\').where(\'id\', 1).update({\'votes\': 1})\n\nLike the ``insert`` statement, there is two notations available.\nThe reason is quite simple: the dictionary notation, though a little less practical, is here to handle\ncolumns names which cannot be passed as keywords arguments.\n\n\nIncrementing or decrementing the value of a column\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').increment(\'votes\')  # Increment the value by 1\n\n    db.table(\'users\').increment(\'votes\', 5)  # Increment the value by 5\n\n    db.table(\'users\').decrement(\'votes\')  # Decrement the value by 1\n\n    db.table(\'users\').decrement(\'votes\', 5)  # Decrement the value by 5\n\nYou can also specify additional columns to update:\n\n.. code-block:: python\n\n    db.table(\'users\').increment(\'votes\', 1, name=\'John\')\n\n\nDeletes\n-------\n\nDeleting records\n~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').where(\'age\', \'<\', 25).delete()\n\nDelete all records\n~~~~~~~~~~~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').delete()\n\nTruncate\n~~~~~~~~\n\n.. code-block:: python\n\n    db.table(\'users\').truncate()\n\n\nUnions\n------\n\nThe query builder provides a quick and easy way to "union" two queries:\n\n.. code-block:: python\n\n    first = db.table(\'users\').where_null(\'first_name\')\n\n    users = db.table(\'users\').where_null(\'last_name\').union(first).get()\n\nThe ``union_all`` method is also available.\n\n\n.. _read_write_connections:\n\nRead / Write connections\n========================\n\nSometimes you may wish to use one database connection for SELECT statements,\nand another for INSERT, UPDATE, and DELETE statements. Orator makes this easy,\nand the proper connections will always be used whether you use raw queries, the query\nbuilder or the actual ORM\n\nHere is an example of how read / write connections should be configured:\n\n.. code-block:: python\n\n    config = {\n        \'mysql\': {\n            \'read\': {\n                \'host\': \'192.168.1.1\'\n            },\n            \'write\': {\n                \'host\': \'192.168.1.2\'\n            },\n            \'driver\': \'mysql\',\n            \'database\': \'database\',\n            \'user\': \'root\',\n            \'password\': \'\',\n            \'prefix\': \'\'\n        }\n    }\n\nNote that two keys have been added to the configuration dictionary: ``read`` and ``write``.\nBoth of these keys have dictionary values containing a single key: ``host``.\nThe rest of the database options for the ``read`` and ``write`` connections\nwill be merged from the main ``mysql`` dictionary. So, you only need to place items\nin the ``read`` and ``write`` dictionaries if you wish to override the values in the main dictionary.\nSo, in this case, ``192.168.1.1`` will be used as the "read" connection, while ``192.168.1.2``\nwill be used as the "write" connection. The database credentials, prefix, character set,\nand all other options in the main ``mysql`` dictionary will be shared across both connections.\n\n\nDatabase transactions\n=====================\n\nTo run a set of operations within a database transaction, you can use the ``transaction`` method\nwhich is a context manager:\n\n.. code-block:: python\n\n    with db.transaction():\n        db.table(\'users\').update({votes: 1})\n        db.table(\'posts\').delete()\n\n.. note::\n\n    Any exception thrown within a transaction block will cause the transaction to be rolled back\n    automatically.\n\nSometimes you may need to start a transaction yourself:\n\n.. code-block:: python\n\n    db.begin_transaction()\n\nYou can rollback a transaction with the ``rollback`` method:\n\n.. code-block:: python\n\n    db.rollback()\n\nYou can also commit a transaction via the ``commit`` method:\n\n.. code-block:: python\n\n    db.commit()\n\nBy default, all underlying DBAPI connections are set to be in autocommit mode\nmeaning that you don\'t need to explicitly commit after each operation.\n\n\nAccessing connections\n=====================\n\nWhen using multiple connections, you can access them via the ``connection()`` method:\n\n.. code-block:: python\n\n    users = db.connection(\'foo\').table(\'users\').get()\n\nYou also can access the raw, underlying dbapi connection instance:\n\n.. code-block:: python\n\n    db.connection().get_connection()\n\nSometimes, you may need to reconnect to a given database:\n\n.. code-block:: python\n\n    db.reconnect(\'foo\')\n\nIf you need to disconnect from the given database, use the ``disconnect`` method:\n\n.. code-block:: python\n\n    db.disconnect(\'foo\')\n',
-    'author': 'Sébastien Eustace',
-    'author_email': 'sebastien@eustace.io',
-    'maintainer': 'Matheus Oliveira',
-    'maintainer_email': 'mco@meliuz.com.br',
-    'url': 'https://orator-orm.com/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
-}
+.. image:: https://travis-ci.org/sdispater/orator.png
+   :alt: Orator Build status
+   :target: https://travis-ci.org/sdispater/orator
 
+The Orator ORM provides a simple yet beautiful ActiveRecord implementation.
+
+It is inspired by the database part of the `Laravel framework <http://laravel.com>`_,
+but largely modified to be more pythonic.
+
+The full documentation is available here: http://orator-orm.com/docs
+
+
+Installation
+============
+
+You can install Orator in 2 different ways:
+
+* The easier and more straightforward is to use pip
+
+.. code-block:: bash
+
+    pip install orator
+
+* Install from source using the official repository (https://github.com/sdispater/orator)
+
+The different dbapi packages are not part of the package dependencies,
+so you must install them in order to connect to corresponding databases:
+
+* Postgres: ``psycopg2``
+* MySQL: ``PyMySQL`` or ``mysqlclient``
+* Sqlite: The ``sqlite3`` module is bundled with Python by default
+
+
+Basic Usage
+===========
+
+Configuration
+-------------
+
+All you need to get you started is the configuration describing your database connections
+and passing it to a ``DatabaseManager`` instance.
+
+.. code-block:: python
+
+    from orator import DatabaseManager, Model
+
+    config = {
+        'mysql': {
+            'driver': 'mysql',
+            'host': 'localhost',
+            'database': 'database',
+            'user': 'root',
+            'password': '',
+            'prefix': ''
+        }
+    }
+
+    db = DatabaseManager(config)
+    Model.set_connection_resolver(db)
+
+
+Defining a model
+----------------
+
+.. code-block:: python
+
+    class User(Model):
+        pass
+
+Note that we did not tell the ORM which table to use for the ``User`` model. The plural "snake case" name of the
+class name will be used as the table name unless another name is explicitly specified.
+In this case, the ORM will assume the ``User`` model stores records in the ``users`` table.
+You can specify a custom table by defining a ``__table__`` property on your model:
+
+.. code-block:: python
+
+    class User(Model):
+
+        __table__ = 'my_users'
+
+The ORM will also assume that each table has a primary key column named ``id``.
+You can define a ``__primary_key__`` property to override this convention.
+Likewise, you can define a ``__connection__`` property to override the name of the database
+connection that should be used when using the model.
+
+Once a model is defined, you are ready to start retrieving and creating records in your table.
+Note that you will need to place ``updated_at`` and ``created_at`` columns on your table by default.
+If you do not wish to have these columns automatically maintained,
+set the ``__timestamps__`` property on your model to ``False``.
+
+
+Retrieving all models
+---------------------
+
+.. code-block:: python
+
+    users = User.all()
+
+
+Retrieving a record by primary key
+----------------------------------
+
+.. code-block:: python
+
+    user = User.find(1)
+
+    print(user.name)
+
+
+Querying using models
+---------------------
+
+.. code-block:: python
+
+    users = User.where('votes', '>', 100).take(10).get()
+
+    for user in users:
+        print(user.name)
+
+
+Aggregates
+----------
+
+You can also use the query builder aggregate functions:
+
+.. code-block:: python
+
+    count = User.where('votes', '>', 100).count()
+
+If you feel limited by the builder's fluent interface, you can use the ``where_raw`` method:
+
+.. code-block:: python
+
+    users = User.where_raw('age > ? and votes = 100', [25]).get()
+
+
+Chunking Results
+----------------
+
+If you need to process a lot of records, you can use the ``chunk`` method to avoid
+consuming a lot of RAM:
+
+.. code-block:: python
+
+    for users in User.chunk(100):
+        for user in users:
+            # ...
+
+
+Specifying the query connection
+-------------------------------
+
+You can specify which database connection to use when querying a model by using the ``on`` method:
+
+.. code-block:: python
+
+    user = User.on('connection-name').find(1)
+
+If you are using read / write connections, you can force the query to use the "write" connection
+with the following method:
+
+.. code-block:: python
+
+    user = User.on_write_connection().find(1)
+
+
+Mass assignment
+===============
+
+When creating a new model, you pass attributes to the model constructor.
+These attributes are then assigned to the model via mass-assignment.
+Though convenient, this can be a serious security concern when passing user input into a model,
+since the user is then free to modify **any** and **all** of the model's attributes.
+For this reason, all models protect against mass-assignment by default.
+
+To get started, set the ``__fillable__`` or ``__guarded__`` properties on your model.
+
+
+Defining fillable attributes on a model
+---------------------------------------
+
+The ``__fillable__`` property specifies which attributes can be mass-assigned.
+
+.. code-block:: python
+
+    class User(Model):
+
+        __fillable__ = ['first_name', 'last_name', 'email']
+
+
+Defining guarded attributes on a model
+--------------------------------------
+
+The ``__guarded__`` is the inverse and acts as "blacklist".
+
+.. code-block:: python
+
+    class User(Model):
+
+        __guarded__ = ['id', 'password']
+
+
+You can also block **all** attributes from mass-assignment:
+
+.. code-block:: python
+
+    __guarded__ = ['*']
+
+
+Insert, update and delete
+=========================
+
+
+Saving a new model
+------------------
+
+To create a new record in the database, simply create a new model instance and call the ``save`` method.
+
+.. code-block:: python
+
+    user = User()
+
+    user.name = 'John'
+
+    user.save()
+
+You can also use the ``create`` method to save a model in a single line, but you will need to specify
+either the ``__fillable__`` or ``__guarded__`` property on the model since all models are protected against
+mass-assignment by default.
+
+After saving or creating a new model with auto-incrementing IDs, you can retrieve the ID by accessing
+the object's ``id`` attribute:
+
+.. code-block:: python
+
+    inserted_id = user.id
+
+
+Using the create method
+-----------------------
+
+.. code-block:: python
+
+    # Create a new user in the database
+    user = User.create(name='John')
+
+    # Retrieve the user by attributes, or create it if it does not exist
+    user = User.first_or_create(name='John')
+
+    # Retrieve the user by attributes, or instantiate it if it does not exist
+    user = User.first_or_new(name='John')
+
+
+Updating a retrieved model
+--------------------------
+
+.. code-block:: python
+
+    user = User.find(1)
+
+    user.name = 'Foo'
+
+    user.save()
+
+You can also run updates as queries against a set of models:
+
+.. code-block:: python
+
+    affected_rows = User.where('votes', '>', 100).update(status=2)
+
+..
+    TODO: push method
+
+
+Deleting an existing model
+--------------------------
+
+To delete a model, simply call the ``delete`` model:
+
+.. code-block:: python
+
+    user = User.find(1)
+
+    user.delete()
+
+
+Deleting an existing model by key
+---------------------------------
+
+.. code-block:: python
+
+    User.destroy(1)
+
+    User.destroy(1, 2, 3)
+
+You can also run a delete query on a set of models:
+
+.. code-block:: python
+
+    affected_rows = User.where('votes', '>' 100).delete()
+
+
+Updating only the model's timestamps
+------------------------------------
+
+If you want to only update the timestamps on a model, you can use the ``touch`` method:
+
+.. code-block:: python
+
+    user.touch()
+
+
+Timestamps
+==========
+
+By default, the ORM will maintain the ``created_at`` and ``updated_at`` columns on your database table
+automatically. Simply add these ``timestamp`` columns to your table. If you do not wish for the ORM to maintain
+these columns, just add the ``__timestamps__`` property:
+
+.. code-block:: python
+
+    class User(Model):
+
+        __timestamps__ = False
+
+
+Providing a custom timestamp format
+-----------------------------------
+
+If you wish to customize the format of your timestamps (the default is the ISO Format) that will be returned when using the ``to_dict``
+or the ``to_json`` methods, you can override the ``get_date_format`` method:
+
+.. code-block:: python
+
+    class User(Model):
+
+        def get_date_format():
+            return 'DD-MM-YY'
+
+
+Converting to dictionaries / JSON
+=================================
+
+Converting a model to a dictionary
+----------------------------------
+
+When building JSON APIs, you may often need to convert your models and relationships to dictionaries or JSON.
+So, Orator includes methods for doing so. To convert a model and its loaded relationship to a dictionary,
+you may use the ``to_dict`` method:
+
+.. code-block:: python
+
+    user = User.with_('roles').first()
+
+    return user.to_dict()
+
+Note that entire collections of models can also be converted to dictionaries:
+
+.. code-block:: python
+
+    return User.all().serailize()
+
+
+Converting a model to JSON
+--------------------------
+
+To convert a model to JSON, you can use the ``to_json`` method!
+
+.. code-block:: python
+
+    return User.find(1).to_json()
+
+
+Query Builder
+=============
+
+
+Introduction
+------------
+
+The database query builder provides a fluent interface to create and run database queries.
+It can be used to perform most database operations in your application, and works on all supported database systems.
+
+
+Selects
+-------
+
+Retrieving all row from a table
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').get()
+
+    for user in users:
+        print(user['name'])
+
+
+Chunking results from a table
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    for users in db.table('users').chunk(100):
+        for user in users:
+            # ...
+
+
+Retrieving a single row from a table
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    user = db.table('users').where('name', 'John').first()
+    print(user['name'])
+
+Retrieving a single column from a row
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    user = db.table('users').where('name', 'John').pluck('name')
+
+Retrieving a list of column values
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    roles = db.table('roles').lists('title')
+
+This method will return a list of role titles. It can return a dictionary
+if you pass an extra key parameter.
+
+.. code-block:: python
+
+    roles = db.table('roles').lists('title', 'name')
+
+Specifying a select clause
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').select('name', 'email').get()
+
+    users = db.table('users').distinct().get()
+
+    users = db.table('users').select('name as user_name').get()
+
+Adding a select clause to an existing query
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    query = db.table('users').select('name')
+
+    users = query.add_select('age').get()
+
+Using where operators
+~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where('age', '>', 25).get()
+
+Or statements
+~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where('age', '>', 25).or_where('name', 'John').get()
+
+Using Where Between
+~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where_between('age', [25, 35]).get()
+
+Using Where Not Between
+~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where_not_between('age', [25, 35]).get()
+
+Using Where In
+~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where_in('id', [1, 2, 3]).get()
+
+    users = db.table('users').where_not_in('id', [1, 2, 3]).get()
+
+Using Where Null to find records with null values
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').where_null('updated_at').get()
+
+Order by, group by and having
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    query = db.table('users').order_by('name', 'desc')
+    query = query.group_by('count')
+    query = query.having('count', '>', 100)
+
+    users = query.get()
+
+Offset and limit
+~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    users = db.table('users').skip(10).take(5).get()
+
+    users = db.table('users').offset(10).limit(5).get()
+
+
+Joins
+-----
+
+The query builder can also be used to write join statements.
+
+Basic join statement
+~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users') \
+        .join('contacts', 'users.id', '=', 'contacts.user_id') \
+        .join('orders', 'users.id', '=', 'orders.user_id') \
+        .select('users.id', 'contacts.phone', 'orders.price') \
+        .get()
+
+Left join statement
+~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').left_join('posts', 'users.id', '=', 'posts.user_id').get()
+
+You can also specify more advance join clauses:
+
+.. code-block:: python
+
+    clause = JoinClause('contacts').on('users.id', '=', 'contacts.user_id').or_on(...)
+
+    db.table('users').join(clause).get()
+
+If you would like to use a "where" style clause on your joins,
+you may use the ``where`` and ``or_where`` methods on a join.
+Instead of comparing two columns, these methods will compare the column against a value:
+
+
+.. code-block:: python
+
+    clause = JoinClause('contacts').on('users.id', '=', 'contacts.user_id').where('contacts.user_id', '>', 5)
+
+    db.table('users').join(clause).get()
+
+
+Advanced where
+--------------
+
+Sometimes you may need to create more advanced where clauses such as "where exists" or nested parameter groupings.
+It is pretty easy to do with the Orator query builder
+
+Parameter grouping
+~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users') \
+        .where('name', '=', 'John') \
+        .or_where(
+            db.query().where('votes', '>', 100).where('title', '!=', 'admin')
+        ).get()
+
+The query above will produce the following SQL:
+
+.. code-block:: sql
+
+    SELECT * FROM users WHERE name = 'John' OR (votes > 100 AND title != 'Admin')
+
+Exists statement
+~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').where_exists(
+        db.table('orders').select(db.raw(1)).where_raw('order.user_id = users.id')
+    )
+
+The query above will produce the following SQL:
+
+.. code-block:: sql
+
+    SELECT * FROM users
+    WHERE EXISTS (
+        SELECT 1 FROM orders WHERE orders.user_id = users.id
+    )
+
+
+Aggregates
+----------
+
+The query builder also provides a variety of aggregate methods, `
+such as ``count``, ``max``, ``min``, ``avg``, and ``sum``.
+
+.. code-block:: python
+
+    users = db.table('users').count()
+
+    price = db.table('orders').max('price')
+
+    price = db.table('orders').min('price')
+
+    price = db.table('orders').avg('price')
+
+    total = db.table('users').sum('votes')
+
+
+Raw expressions
+---------------
+
+Sometimes you may need to use a raw expression in a query.
+These expressions will be injected into the query as strings, so be careful not to create any SQL injection points!
+To create a raw expression, you may use the ``raw()`` method:
+
+.. code-block:: python
+
+    db.table('users') \
+        .select(db.raw('count(*) as user_count, status')) \
+        .where('status', '!=', 1) \
+        .group_by('status') \
+        .get()
+
+
+Inserts
+-------
+
+Insert records into a table
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').insert(email='foo@bar.com', votes=0)
+
+    db.table('users').insert({
+        'email': 'foo@bar.com',
+        'votes': 0
+    })
+
+
+It is important to note that there is two notations available.
+The reason is quite simple: the dictionary notation, though a little less practical, is here to handle
+columns names which cannot be passed as keywords arguments.
+
+Inserting records into a table with an auto-incrementing ID
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If the table has an auto-incrementing id, use ``insert_get_id`` to insert a record and retrieve the id:
+
+.. code-block:: python
+
+    id = db.table('users').insert_get_id({
+        'email': 'foo@bar.com',
+        'votes': 0
+    })
+
+Inserting multiple record into a table
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').insert([
+        {'email': 'foo@bar.com', 'votes': 0},
+        {'email': 'bar@baz.com', 'votes': 0}
+    ])
+
+Updates
+-------
+
+Updating records
+~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').where('id', 1).update(votes=1)
+
+    db.table('users').where('id', 1).update({'votes': 1})
+
+Like the ``insert`` statement, there is two notations available.
+The reason is quite simple: the dictionary notation, though a little less practical, is here to handle
+columns names which cannot be passed as keywords arguments.
+
+
+Incrementing or decrementing the value of a column
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').increment('votes')  # Increment the value by 1
+
+    db.table('users').increment('votes', 5)  # Increment the value by 5
+
+    db.table('users').decrement('votes')  # Decrement the value by 1
+
+    db.table('users').decrement('votes', 5)  # Decrement the value by 5
+
+You can also specify additional columns to update:
+
+.. code-block:: python
+
+    db.table('users').increment('votes', 1, name='John')
+
+
+Deletes
+-------
+
+Deleting records
+~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').where('age', '<', 25).delete()
+
+Delete all records
+~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').delete()
+
+Truncate
+~~~~~~~~
+
+.. code-block:: python
+
+    db.table('users').truncate()
+
+
+Unions
+------
+
+The query builder provides a quick and easy way to "union" two queries:
+
+.. code-block:: python
+
+    first = db.table('users').where_null('first_name')
+
+    users = db.table('users').where_null('last_name').union(first).get()
+
+The ``union_all`` method is also available.
+
+
+.. _read_write_connections:
+
+Read / Write connections
+========================
+
+Sometimes you may wish to use one database connection for SELECT statements,
+and another for INSERT, UPDATE, and DELETE statements. Orator makes this easy,
+and the proper connections will always be used whether you use raw queries, the query
+builder or the actual ORM
+
+Here is an example of how read / write connections should be configured:
+
+.. code-block:: python
+
+    config = {
+        'mysql': {
+            'read': {
+                'host': '192.168.1.1'
+            },
+            'write': {
+                'host': '192.168.1.2'
+            },
+            'driver': 'mysql',
+            'database': 'database',
+            'user': 'root',
+            'password': '',
+            'prefix': ''
+        }
+    }
+
+Note that two keys have been added to the configuration dictionary: ``read`` and ``write``.
+Both of these keys have dictionary values containing a single key: ``host``.
+The rest of the database options for the ``read`` and ``write`` connections
+will be merged from the main ``mysql`` dictionary. So, you only need to place items
+in the ``read`` and ``write`` dictionaries if you wish to override the values in the main dictionary.
+So, in this case, ``192.168.1.1`` will be used as the "read" connection, while ``192.168.1.2``
+will be used as the "write" connection. The database credentials, prefix, character set,
+and all other options in the main ``mysql`` dictionary will be shared across both connections.
+
+
+Database transactions
+=====================
+
+To run a set of operations within a database transaction, you can use the ``transaction`` method
+which is a context manager:
+
+.. code-block:: python
+
+    with db.transaction():
+        db.table('users').update({votes: 1})
+        db.table('posts').delete()
+
+.. note::
+
+    Any exception thrown within a transaction block will cause the transaction to be rolled back
+    automatically.
+
+Sometimes you may need to start a transaction yourself:
+
+.. code-block:: python
+
+    db.begin_transaction()
+
+You can rollback a transaction with the ``rollback`` method:
+
+.. code-block:: python
+
+    db.rollback()
+
+You can also commit a transaction via the ``commit`` method:
+
+.. code-block:: python
+
+    db.commit()
+
+By default, all underlying DBAPI connections are set to be in autocommit mode
+meaning that you don't need to explicitly commit after each operation.
+
+
+Accessing connections
+=====================
+
+When using multiple connections, you can access them via the ``connection()`` method:
+
+.. code-block:: python
+
+    users = db.connection('foo').table('users').get()
+
+You also can access the raw, underlying dbapi connection instance:
+
+.. code-block:: python
+
+    db.connection().get_connection()
+
+Sometimes, you may need to reconnect to a given database:
+
+.. code-block:: python
+
+    db.reconnect('foo')
+
+If you need to disconnect from the given database, use the ``disconnect`` method:
+
+.. code-block:: python
+
+    db.disconnect('foo')
 
-setup(**setup_kwargs)
```

