# Comparing `tmp/castor_extractor-0.3.8.tar.gz` & `tmp/castor_extractor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor_extractor-0.3.8.tar", max compression
+gzip compressed data, was "castor_extractor-0.4.0.tar", max compression
```

## Comparing `castor_extractor-0.3.8.tar` & `castor_extractor-0.4.0.tar`

### file list

```diff
@@ -1,266 +1,277 @@
--rw-r--r--   0        0        0     5004 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     8254 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/LICENCE
--rw-r--r--   0        0        0     3423 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/README.md
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.402721 castor_extractor-0.3.8/castor_extractor/__init__.py
--rw-r--r--   0        0        0      116 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/__init__.py
--rw-r--r--   0        0        0     1252 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/extract_bigquery.py
--rwxr-xr-x   0        0        0     1075 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/extract_looker.py
--rwxr-xr-x   0        0        0      761 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/extract_metabase_api.py
--rwxr-xr-x   0        0        0     1235 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/extract_metabase_db.py
--rwxr-xr-x   0        0        0      919 2023-06-05 10:01:55.260722 castor_extractor-0.3.8/castor_extractor/commands/extract_mode.py
--rw-r--r--   0        0        0     1154 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_postgres.py
--rw-r--r--   0        0        0      850 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_powerbi.py
--rw-r--r--   0        0        0      989 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_qlik.py
--rwxr-xr-x   0        0        0     1155 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_redshift.py
--rwxr-xr-x   0        0        0     1799 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_snowflake.py
--rwxr-xr-x   0        0        0     1390 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/extract_tableau.py
--rw-r--r--   0        0        0     2667 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/file_check.py
--rwxr-xr-x   0        0        0     1930 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/commands/upload.py
--rw-r--r--   0        0        0      119 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/column.py
--rw-r--r--   0        0        0     1935 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/column_test.py
--rw-r--r--   0        0        0      289 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/constants.py
--rw-r--r--   0        0        0      536 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/enums.py
--rw-r--r--   0        0        0     6537 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/file.py
--rw-r--r--   0        0        0     2082 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/file_test.py
--rw-r--r--   0        0        0      547 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/file_test_users.csv
--rw-r--r--   0        0        0      286 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/file_test_users_valid.csv
--rw-r--r--   0        0        0       60 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/templates/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/file_checker/templates/generic_warehouse.py
--rw-r--r--   0        0        0      886 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/logger.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.402721 castor_extractor-0.3.8/castor_extractor/transformation/__init__.py
--rw-r--r--   0        0        0       91 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/transformation/dbt/__init__.py
--rw-r--r--   0        0        0       94 2023-06-05 10:01:55.261722 castor_extractor-0.3.8/castor_extractor/transformation/dbt/assets.py
--rw-r--r--   0        0        0       86 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/transformation/dbt/client/__init__.py
--rw-r--r--   0        0        0     2938 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/transformation/dbt/client/client.py
--rw-r--r--   0        0        0      746 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/transformation/dbt/client/credentials.py
--rw-r--r--   0        0        0      181 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/types.py
--rw-r--r--   0        0        0       75 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/__init__.py
--rw-r--r--   0        0        0      718 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/constant.py
--rw-r--r--   0        0        0      878 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/env.py
--rw-r--r--   0        0        0      472 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/env_test.py
--rw-r--r--   0        0        0     3353 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/upload.py
--rw-r--r--   0        0        0      329 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/upload_test.py
--rw-r--r--   0        0        0      478 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/uploader/utils.py
--rw-r--r--   0        0        0      918 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/__init__.py
--rw-r--r--   0        0        0      417 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/collection.py
--rw-r--r--   0        0        0       39 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/constants.py
--rw-r--r--   0        0        0      843 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/deprecate.py
--rw-r--r--   0        0        0      608 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/env.py
--rw-r--r--   0        0        0     1545 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/files.py
--rw-r--r--   0        0        0     1514 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/files_test.py
--rw-r--r--   0        0        0     4616 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/formatter.py
--rw-r--r--   0        0        0     3802 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/formatter_test.csv
--rw-r--r--   0        0        0    12527 2023-06-05 10:01:55.262722 castor_extractor-0.3.8/castor_extractor/utils/formatter_test.json
--rw-r--r--   0        0        0     1543 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/formatter_test.py
--rw-r--r--   0        0        0      265 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/load.py
--rw-r--r--   0        0        0     1813 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/object.py
--rw-r--r--   0        0        0     2487 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/object_test.py
--rw-r--r--   0        0        0     3894 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/pager.py
--rw-r--r--   0        0        0     3245 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/pager_test.py
--rw-r--r--   0        0        0     2664 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/retry.py
--rw-r--r--   0        0        0     1635 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/retry_test.py
--rw-r--r--   0        0        0     1966 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/safe.py
--rw-r--r--   0        0        0     2160 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/safe_test.py
--rw-r--r--   0        0        0     2092 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/store.py
--rw-r--r--   0        0        0     1961 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/string.py
--rw-r--r--   0        0        0     2206 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/string_test.py
--rw-r--r--   0        0        0      430 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/time.py
--rw-r--r--   0        0        0      313 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/type.py
--rw-r--r--   0        0        0      150 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/uri.py
--rw-r--r--   0        0        0      259 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/uri_test.py
--rw-r--r--   0        0        0     1904 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/validation.py
--rw-r--r--   0        0        0     1181 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/validation_test.py
--rw-r--r--   0        0        0     2135 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/utils/write.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.406721 castor_extractor-0.3.8/castor_extractor/visualization/__init__.py
--rw-r--r--   0        0        0      191 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/visualization/looker/__init__.py
--rw-r--r--   0        0        0      181 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/__init__.py
--rw-r--r--   0        0        0     7137 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/client.py
--rw-r--r--   0        0        0      816 2023-06-05 10:01:55.263723 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/client_test.py
--rw-r--r--   0        0        0     3895 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/constants.py
--rw-r--r--   0        0        0     3526 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/sdk.py
--rw-r--r--   0        0        0     1742 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/sdk_test.py
--rw-r--r--   0        0        0     1320 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/api/utils.py
--rw-r--r--   0        0        0      364 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/assets.py
--rw-r--r--   0        0        0      467 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/constant.py
--rw-r--r--   0        0        0      864 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/env.py
--rw-r--r--   0        0        0     3514 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/extract.py
--rw-r--r--   0        0        0      636 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/fields.py
--rw-r--r--   0        0        0      782 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/fields_test.py
--rw-r--r--   0        0        0     1527 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/looker/parameters.py
--rw-r--r--   0        0        0      125 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/__init__.py
--rw-r--r--   0        0        0     2814 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/assets.py
--rw-r--r--   0        0        0       52 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/__init__.py
--rw-r--r--   0        0        0       30 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/api/__init__.py
--rw-r--r--   0        0        0     5609 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/api/client.py
--rw-r--r--   0        0        0     1334 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/api/credentials.py
--rw-r--r--   0        0        0       29 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/__init__.py
--rw-r--r--   0        0        0     4095 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/client.py
--rw-r--r--   0        0        0     1863 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/credentials.py
--rw-r--r--   0        0        0       76 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
--rw-r--r--   0        0        0       79 2023-06-05 10:01:55.264722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
--rw-r--r--   0        0        0      419 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/card.sql
--rw-r--r--   0        0        0       42 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/collection.sql
--rw-r--r--   0        0        0      439 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
--rw-r--r--   0        0        0       52 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
--rw-r--r--   0        0        0       49 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/database.sql
--rw-r--r--   0        0        0       46 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/table.sql
--rw-r--r--   0        0        0       41 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/queries/user.sql
--rw-r--r--   0        0        0     1076 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/decryption.py
--rw-r--r--   0        0        0      591 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/decryption_test.py
--rw-r--r--   0        0        0      389 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/shared.py
--rw-r--r--   0        0        0     1006 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/errors.py
--rw-r--r--   0        0        0     1773 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/extract.py
--rw-r--r--   0        0        0       45 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/metabase/types.py
--rw-r--r--   0        0        0      117 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/assets.py
--rw-r--r--   0        0        0       27 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/__init__.py
--rw-r--r--   0        0        0     7803 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client.py
--rw-r--r--   0        0        0     2087 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client_test.json
--rw-r--r--   0        0        0     1400 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client_test.py
--rw-r--r--   0        0        0      453 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/constants.py
--rw-r--r--   0        0        0     1622 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/client/credentials.py
--rw-r--r--   0        0        0     1495 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/errors.py
--rw-r--r--   0        0        0     1559 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/mode/extract.py
--rw-r--r--   0        0        0      106 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/__init__.py
--rw-r--r--   0        0        0      449 2023-06-05 10:01:55.265722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/assets.py
--rw-r--r--   0        0        0       62 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/__init__.py
--rw-r--r--   0        0        0     2142 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/constants.py
--rw-r--r--   0        0        0      501 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/credentials.py
--rw-r--r--   0        0        0      720 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/credentials_test.py
--rw-r--r--   0        0        0     7084 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/rest.py
--rw-r--r--   0        0        0     6142 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/rest_test.py
--rw-r--r--   0        0        0      541 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/utils.py
--rw-r--r--   0        0        0      719 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/utils_test.py
--rw-r--r--   0        0        0     1616 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/powerbi/extract.py
--rw-r--r--   0        0        0      143 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/assets.py
--rw-r--r--   0        0        0       94 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/__init__.py
--rw-r--r--   0        0        0      786 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/constants.py
--rw-r--r--   0        0        0       36 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/__init__.py
--rw-r--r--   0        0        0     2512 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/client.py
--rw-r--r--   0        0        0      707 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/constants.py
--rw-r--r--   0        0        0     1229 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/error.py
--rw-r--r--   0        0        0     1005 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/error_test.py
--rw-r--r--   0        0        0     1386 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/json_rpc.py
--rw-r--r--   0        0        0     1305 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
--rw-r--r--   0        0        0     2032 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/websocket.py
--rw-r--r--   0        0        0     3209 2023-06-05 10:01:55.266722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/master.py
--rw-r--r--   0        0        0     5966 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/rest.py
--rw-r--r--   0        0        0     1676 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/rest_test.py
--rw-r--r--   0        0        0       95 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/constants.py
--rw-r--r--   0        0        0     2397 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/qlik/extract.py
--rw-r--r--   0        0        0      114 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/__init__.py
--rw-r--r--   0        0        0      762 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/assets.py
--rw-r--r--   0        0        0       78 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/__init__.py
--rw-r--r--   0        0        0     6824 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/client.py
--rw-r--r--   0        0        0     2077 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/client_utils.py
--rw-r--r--   0        0        0     3335 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/credentials.py
--rw-r--r--   0        0        0      803 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/project.py
--rw-r--r--   0        0        0     2036 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/safe_mode.py
--rw-r--r--   0        0        0      126 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/constants.py
--rw-r--r--   0        0        0       91 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/errors.py
--rw-r--r--   0        0        0     2873 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/extract.py
--rw-r--r--   0        0        0     4728 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/gql_fields.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.412721 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.412721 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/__init__.py
--rw-r--r--   0        0        0      446 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
--rw-r--r--   0        0        0      447 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
--rw-r--r--   0        0        0      450 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
--rw-r--r--   0        0        0     1018 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
--rw-r--r--   0        0        0      679 2023-06-05 10:01:55.267722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
--rw-r--r--   0        0        0     1415 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
--rw-r--r--   0        0        0     1325 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.412721 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
--rw-r--r--   0        0        0     1917 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.412721 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
--rw-r--r--   0        0        0     1134 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
--rw-r--r--   0        0        0      422 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
--rw-r--r--   0        0        0     1779 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
--rw-r--r--   0        0        0     1384 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
--rw-r--r--   0        0        0     1499 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
--rw-r--r--   0        0        0     1979 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
--rw-r--r--   0        0        0       26 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
--rw-r--r--   0        0        0      966 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/tsc_fields.py
--rw-r--r--   0        0        0      322 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/types.py
--rw-r--r--   0        0        0      427 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/visualization/tableau/usage.py
--rw-r--r--   0        0        0        0 2023-06-05 10:01:55.412721 castor_extractor-0.3.8/castor_extractor/warehouse/__init__.py
--rw-r--r--   0        0        0      386 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/asset.py
--rw-r--r--   0        0        0     1947 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/client.py
--rw-r--r--   0        0        0     2885 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/extract.py
--rw-r--r--   0        0        0     2640 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/query.py
--rw-r--r--   0        0        0      935 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/time_filter.py
--rw-r--r--   0        0        0      449 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/abstract/time_filter_test.py
--rw-r--r--   0        0        0      125 2023-06-05 10:01:55.268722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/client.py
--rw-r--r--   0        0        0     1567 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/client_test.py
--rw-r--r--   0        0        0     2800 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/extract.py
--rw-r--r--   0        0        0       30 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/.sqlfluff
--rw-r--r--   0        0        0     1815 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/column.sql
--rw-r--r--   0        0        0     1347 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
--rw-r--r--   0        0        0      207 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/database.sql
--rw-r--r--   0        0        0      660 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/query.sql
--rw-r--r--   0        0        0      284 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/schema.sql
--rw-r--r--   0        0        0     1508 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/table.sql
--rw-r--r--   0        0        0     2660 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
--rw-r--r--   0        0        0      189 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/user.sql
--rw-r--r--   0        0        0      326 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
--rw-r--r--   0        0        0     4147 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/query.py
--rw-r--r--   0        0        0      140 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/types.py
--rw-r--r--   0        0        0      125 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/__init__.py
--rw-r--r--   0        0        0      871 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/client.py
--rw-r--r--   0        0        0     2099 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/extract.py
--rw-r--r--   0        0        0       30 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/.sqlfluff
--rw-r--r--   0        0        0     1632 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/column.sql
--rw-r--r--   0        0        0      241 2023-06-05 10:01:55.269722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/database.sql
--rw-r--r--   0        0        0      101 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/group.sql
--rw-r--r--   0        0        0      592 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/schema.sql
--rw-r--r--   0        0        0     1489 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/table.sql
--rw-r--r--   0        0        0      170 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/user.sql
--rw-r--r--   0        0        0      540 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/postgres/query.py
--rw-r--r--   0        0        0      125 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/__init__.py
--rw-r--r--   0        0        0      764 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/client.py
--rw-r--r--   0        0        0     1028 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/client_test.py
--rw-r--r--   0        0        0     2238 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/extract.py
--rw-r--r--   0        0        0       30 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/.sqlfluff
--rw-r--r--   0        0        0     7044 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/column.sql
--rw-r--r--   0        0        0      299 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/database.sql
--rw-r--r--   0        0        0      101 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/group.sql
--rw-r--r--   0        0        0     3258 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/query.sql
--rw-r--r--   0        0        0      585 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/schema.sql
--rw-r--r--   0        0        0     2645 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/table.sql
--rw-r--r--   0        0        0      726 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/table_freshness.sql
--rw-r--r--   0        0        0      170 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/user.sql
--rw-r--r--   0        0        0      719 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/view_ddl.sql
--rw-r--r--   0        0        0      540 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/redshift/query.py
--rw-r--r--   0        0        0      128 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/__init__.py
--rw-r--r--   0        0        0     4128 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/client.py
--rw-r--r--   0        0        0     1434 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/client_test.py
--rw-r--r--   0        0        0     2443 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/extract.py
--rw-r--r--   0        0        0       31 2023-06-05 10:01:55.270722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/.sqlfluff
--rw-r--r--   0        0        0     1130 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/column.sql
--rw-r--r--   0        0        0     1179 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
--rw-r--r--   0        0        0      483 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/database.sql
--rw-r--r--   0        0        0      272 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
--rw-r--r--   0        0        0      143 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
--rw-r--r--   0        0        0     1779 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/query.sql
--rw-r--r--   0        0        0       96 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/role.sql
--rw-r--r--   0        0        0      730 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/schema.sql
--rw-r--r--   0        0        0     1378 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/table.sql
--rw-r--r--   0        0        0      570 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/user.sql
--rw-r--r--   0        0        0      673 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
--rw-r--r--   0        0        0     1769 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/query.py
--rw-r--r--   0        0        0       36 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/__init__.py
--rw-r--r--   0        0        0      517 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/extract.py
--rw-r--r--   0        0        0       26 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/.sqlfluff
--rw-r--r--   0        0        0     1392 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/column.sql
--rw-r--r--   0        0        0      138 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/database.sql
--rw-r--r--   0        0        0     1110 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/query.sql
--rw-r--r--   0        0        0      250 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/schema.sql
--rw-r--r--   0        0        0     1049 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/table.sql
--rw-r--r--   0        0        0       67 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/user.sql
--rw-r--r--   0        0        0      249 2023-06-05 10:01:55.271722 castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/view_ddl.sql
--rw-r--r--   0        0        0     5150 2023-06-05 10:01:55.272722 castor_extractor-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6414 1970-01-01 00:00:00.000000 castor_extractor-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     5054 2023-06-22 07:53:23.677088 castor_extractor-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     8254 2023-06-22 07:53:23.677088 castor_extractor-0.4.0/LICENCE
+-rw-r--r--   0        0        0     3423 2023-06-22 07:53:23.677088 castor_extractor-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.816088 castor_extractor-0.4.0/castor_extractor/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/__init__.py
+-rw-r--r--   0        0        0     1252 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_bigquery.py
+-rwxr-xr-x   0        0        0     1075 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_looker.py
+-rwxr-xr-x   0        0        0      761 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_metabase_api.py
+-rwxr-xr-x   0        0        0     1235 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_metabase_db.py
+-rwxr-xr-x   0        0        0      919 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_mode.py
+-rw-r--r--   0        0        0     1154 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_postgres.py
+-rw-r--r--   0        0        0      850 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_powerbi.py
+-rw-r--r--   0        0        0      989 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_qlik.py
+-rwxr-xr-x   0        0        0     1155 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_redshift.py
+-rw-r--r--   0        0        0      703 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_sigma.py
+-rwxr-xr-x   0        0        0     1799 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_snowflake.py
+-rwxr-xr-x   0        0        0     1390 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/extract_tableau.py
+-rw-r--r--   0        0        0     2667 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/file_check.py
+-rwxr-xr-x   0        0        0     1930 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/commands/upload.py
+-rw-r--r--   0        0        0      119 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/column.py
+-rw-r--r--   0        0        0     1935 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/column_test.py
+-rw-r--r--   0        0        0      289 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/constants.py
+-rw-r--r--   0        0        0      536 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/enums.py
+-rw-r--r--   0        0        0     6537 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/file.py
+-rw-r--r--   0        0        0     2082 2023-06-22 07:53:23.678088 castor_extractor-0.4.0/castor_extractor/file_checker/file_test.py
+-rw-r--r--   0        0        0      547 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/file_checker/file_test_users.csv
+-rw-r--r--   0        0        0      286 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/file_checker/file_test_users_valid.csv
+-rw-r--r--   0        0        0       60 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/file_checker/templates/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/file_checker/templates/generic_warehouse.py
+-rw-r--r--   0        0        0      886 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/logger.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.816088 castor_extractor-0.4.0/castor_extractor/transformation/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/transformation/dbt/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/transformation/dbt/assets.py
+-rw-r--r--   0        0        0       86 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/transformation/dbt/client/__init__.py
+-rw-r--r--   0        0        0     2938 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/transformation/dbt/client/client.py
+-rw-r--r--   0        0        0      746 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/transformation/dbt/client/credentials.py
+-rw-r--r--   0        0        0      181 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/types.py
+-rw-r--r--   0        0        0       75 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/__init__.py
+-rw-r--r--   0        0        0      718 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/constant.py
+-rw-r--r--   0        0        0      878 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/env.py
+-rw-r--r--   0        0        0      472 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/env_test.py
+-rw-r--r--   0        0        0     3353 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/upload.py
+-rw-r--r--   0        0        0      329 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/upload_test.py
+-rw-r--r--   0        0        0      478 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/uploader/utils.py
+-rw-r--r--   0        0        0      918 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/utils/__init__.py
+-rw-r--r--   0        0        0      417 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/utils/collection.py
+-rw-r--r--   0        0        0       39 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/utils/constants.py
+-rw-r--r--   0        0        0      843 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/utils/deprecate.py
+-rw-r--r--   0        0        0      608 2023-06-22 07:53:23.679088 castor_extractor-0.4.0/castor_extractor/utils/env.py
+-rw-r--r--   0        0        0     1545 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/files.py
+-rw-r--r--   0        0        0     1514 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/files_test.py
+-rw-r--r--   0        0        0     4616 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/formatter.py
+-rw-r--r--   0        0        0     3802 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/formatter_test.csv
+-rw-r--r--   0        0        0    12527 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/formatter_test.json
+-rw-r--r--   0        0        0     1543 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/formatter_test.py
+-rw-r--r--   0        0        0      265 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/load.py
+-rw-r--r--   0        0        0     1987 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/object.py
+-rw-r--r--   0        0        0     2487 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/object_test.py
+-rw-r--r--   0        0        0     3894 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/pager.py
+-rw-r--r--   0        0        0     3245 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/pager_test.py
+-rw-r--r--   0        0        0     2664 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/retry.py
+-rw-r--r--   0        0        0     1635 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/retry_test.py
+-rw-r--r--   0        0        0     1966 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/safe.py
+-rw-r--r--   0        0        0     2160 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/safe_test.py
+-rw-r--r--   0        0        0     2092 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/store.py
+-rw-r--r--   0        0        0     1961 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/string.py
+-rw-r--r--   0        0        0     2206 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/string_test.py
+-rw-r--r--   0        0        0      430 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/time.py
+-rw-r--r--   0        0        0      313 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/type.py
+-rw-r--r--   0        0        0      150 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/uri.py
+-rw-r--r--   0        0        0      259 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/uri_test.py
+-rw-r--r--   0        0        0     1904 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/validation.py
+-rw-r--r--   0        0        0     1181 2023-06-22 07:53:23.680088 castor_extractor-0.4.0/castor_extractor/utils/validation_test.py
+-rw-r--r--   0        0        0     2135 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/utils/write.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.830088 castor_extractor-0.4.0/castor_extractor/visualization/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/__init__.py
+-rw-r--r--   0        0        0     7137 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/client.py
+-rw-r--r--   0        0        0      816 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/client_test.py
+-rw-r--r--   0        0        0     3895 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/constants.py
+-rw-r--r--   0        0        0     3526 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/sdk.py
+-rw-r--r--   0        0        0     1742 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/sdk_test.py
+-rw-r--r--   0        0        0     1320 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/api/utils.py
+-rw-r--r--   0        0        0      364 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/assets.py
+-rw-r--r--   0        0        0      467 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/constant.py
+-rw-r--r--   0        0        0      864 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/env.py
+-rw-r--r--   0        0        0     3514 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/extract.py
+-rw-r--r--   0        0        0      636 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/fields.py
+-rw-r--r--   0        0        0      782 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/fields_test.py
+-rw-r--r--   0        0        0     1527 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/looker/parameters.py
+-rw-r--r--   0        0        0      125 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/assets.py
+-rw-r--r--   0        0        0       52 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/api/__init__.py
+-rw-r--r--   0        0        0     5609 2023-06-22 07:53:23.681088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/api/client.py
+-rw-r--r--   0        0        0     1334 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/api/credentials.py
+-rw-r--r--   0        0        0       29 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/__init__.py
+-rw-r--r--   0        0        0     4095 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/client.py
+-rw-r--r--   0        0        0     1863 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/credentials.py
+-rw-r--r--   0        0        0       76 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
+-rw-r--r--   0        0        0       79 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
+-rw-r--r--   0        0        0      419 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/card.sql
+-rw-r--r--   0        0        0       42 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/collection.sql
+-rw-r--r--   0        0        0      439 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
+-rw-r--r--   0        0        0       52 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
+-rw-r--r--   0        0        0       49 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/database.sql
+-rw-r--r--   0        0        0       46 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/table.sql
+-rw-r--r--   0        0        0       41 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/queries/user.sql
+-rw-r--r--   0        0        0     1076 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/decryption.py
+-rw-r--r--   0        0        0      591 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/decryption_test.py
+-rw-r--r--   0        0        0      389 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/shared.py
+-rw-r--r--   0        0        0     1006 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/errors.py
+-rw-r--r--   0        0        0     1773 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/extract.py
+-rw-r--r--   0        0        0       45 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/metabase/types.py
+-rw-r--r--   0        0        0      117 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/assets.py
+-rw-r--r--   0        0        0       27 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/__init__.py
+-rw-r--r--   0        0        0     7803 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client.py
+-rw-r--r--   0        0        0     2087 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client_test.json
+-rw-r--r--   0        0        0     1400 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client_test.py
+-rw-r--r--   0        0        0      453 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/constants.py
+-rw-r--r--   0        0        0     1622 2023-06-22 07:53:23.682088 castor_extractor-0.4.0/castor_extractor/visualization/mode/client/credentials.py
+-rw-r--r--   0        0        0     1495 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/mode/errors.py
+-rw-r--r--   0        0        0     1559 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/mode/extract.py
+-rw-r--r--   0        0        0      106 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/assets.py
+-rw-r--r--   0        0        0       62 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/__init__.py
+-rw-r--r--   0        0        0     2142 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/constants.py
+-rw-r--r--   0        0        0      501 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/credentials.py
+-rw-r--r--   0        0        0      720 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/credentials_test.py
+-rw-r--r--   0        0        0     7084 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/rest.py
+-rw-r--r--   0        0        0     6142 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/rest_test.py
+-rw-r--r--   0        0        0      541 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/utils.py
+-rw-r--r--   0        0        0      719 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/utils_test.py
+-rw-r--r--   0        0        0     1616 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/powerbi/extract.py
+-rw-r--r--   0        0        0      143 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/assets.py
+-rw-r--r--   0        0        0       94 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/constants.py
+-rw-r--r--   0        0        0       36 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/__init__.py
+-rw-r--r--   0        0        0     2512 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/client.py
+-rw-r--r--   0        0        0      707 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/constants.py
+-rw-r--r--   0        0        0     1229 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/error.py
+-rw-r--r--   0        0        0     1005 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/error_test.py
+-rw-r--r--   0        0        0     1386 2023-06-22 07:53:23.683088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/json_rpc.py
+-rw-r--r--   0        0        0     1305 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
+-rw-r--r--   0        0        0     2032 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/websocket.py
+-rw-r--r--   0        0        0     3209 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/master.py
+-rw-r--r--   0        0        0     5966 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/rest.py
+-rw-r--r--   0        0        0     1676 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/rest_test.py
+-rw-r--r--   0        0        0       95 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/constants.py
+-rw-r--r--   0        0        0     2397 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/qlik/extract.py
+-rw-r--r--   0        0        0      130 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/assets.py
+-rw-r--r--   0        0        0       90 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/__init__.py
+-rw-r--r--   0        0        0     6307 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/client.py
+-rw-r--r--   0        0        0     1529 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/client_test.py
+-rw-r--r--   0        0        0      769 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/credentials.py
+-rw-r--r--   0        0        0     1157 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/endpoints.py
+-rw-r--r--   0        0        0      667 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/client/pagination.py
+-rw-r--r--   0        0        0      130 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/constants.py
+-rw-r--r--   0        0        0     2661 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/sigma/extract.py
+-rw-r--r--   0        0        0      114 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/__init__.py
+-rw-r--r--   0        0        0      762 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/assets.py
+-rw-r--r--   0        0        0       78 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/__init__.py
+-rw-r--r--   0        0        0     6824 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/client.py
+-rw-r--r--   0        0        0     2077 2023-06-22 07:53:23.684088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/client_utils.py
+-rw-r--r--   0        0        0     3335 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/credentials.py
+-rw-r--r--   0        0        0      803 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/project.py
+-rw-r--r--   0        0        0     2036 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/safe_mode.py
+-rw-r--r--   0        0        0      126 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/constants.py
+-rw-r--r--   0        0        0       91 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/errors.py
+-rw-r--r--   0        0        0     2873 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/extract.py
+-rw-r--r--   0        0        0     4728 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/gql_fields.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.830088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.830088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/__init__.py
+-rw-r--r--   0        0        0      446 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
+-rw-r--r--   0        0        0      447 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
+-rw-r--r--   0        0        0      450 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
+-rw-r--r--   0        0        0     1018 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
+-rw-r--r--   0        0        0      679 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
+-rw-r--r--   0        0        0     1415 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
+-rw-r--r--   0        0        0     1325 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.830088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
+-rw-r--r--   0        0        0     1917 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.831088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
+-rw-r--r--   0        0        0     1134 2023-06-22 07:53:23.685088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
+-rw-r--r--   0        0        0      422 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
+-rw-r--r--   0        0        0     1779 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
+-rw-r--r--   0        0        0     1384 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
+-rw-r--r--   0        0        0     1499 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
+-rw-r--r--   0        0        0     1979 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
+-rw-r--r--   0        0        0       26 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
+-rw-r--r--   0        0        0      966 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/tsc_fields.py
+-rw-r--r--   0        0        0      322 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/types.py
+-rw-r--r--   0        0        0      427 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/visualization/tableau/usage.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:53:23.831088 castor_extractor-0.4.0/castor_extractor/warehouse/__init__.py
+-rw-r--r--   0        0        0      386 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/asset.py
+-rw-r--r--   0        0        0     1947 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/client.py
+-rw-r--r--   0        0        0     2885 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/extract.py
+-rw-r--r--   0        0        0     2640 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/query.py
+-rw-r--r--   0        0        0      935 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/time_filter.py
+-rw-r--r--   0        0        0      449 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/abstract/time_filter_test.py
+-rw-r--r--   0        0        0      125 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/__init__.py
+-rw-r--r--   0        0        0     3125 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/client.py
+-rw-r--r--   0        0        0     1567 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/client_test.py
+-rw-r--r--   0        0        0     2800 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/extract.py
+-rw-r--r--   0        0        0       30 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/.sqlfluff
+-rw-r--r--   0        0        0     1815 2023-06-22 07:53:23.686088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/column.sql
+-rw-r--r--   0        0        0     1347 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
+-rw-r--r--   0        0        0      207 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/database.sql
+-rw-r--r--   0        0        0      660 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/query.sql
+-rw-r--r--   0        0        0      284 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/schema.sql
+-rw-r--r--   0        0        0     1508 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/table.sql
+-rw-r--r--   0        0        0     2660 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
+-rw-r--r--   0        0        0      189 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/user.sql
+-rw-r--r--   0        0        0      326 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
+-rw-r--r--   0        0        0     4147 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/query.py
+-rw-r--r--   0        0        0      140 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/types.py
+-rw-r--r--   0        0        0      125 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/__init__.py
+-rw-r--r--   0        0        0      871 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/client.py
+-rw-r--r--   0        0        0     2099 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/extract.py
+-rw-r--r--   0        0        0       30 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/.sqlfluff
+-rw-r--r--   0        0        0     1632 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/column.sql
+-rw-r--r--   0        0        0      241 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/group.sql
+-rw-r--r--   0        0        0      592 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/schema.sql
+-rw-r--r--   0        0        0     1489 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/table.sql
+-rw-r--r--   0        0        0      170 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/user.sql
+-rw-r--r--   0        0        0      540 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/postgres/query.py
+-rw-r--r--   0        0        0      125 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/__init__.py
+-rw-r--r--   0        0        0      764 2023-06-22 07:53:23.687088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/client.py
+-rw-r--r--   0        0        0     1028 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/client_test.py
+-rw-r--r--   0        0        0     2238 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/extract.py
+-rw-r--r--   0        0        0       30 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/.sqlfluff
+-rw-r--r--   0        0        0     7044 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/column.sql
+-rw-r--r--   0        0        0      299 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/group.sql
+-rw-r--r--   0        0        0     3258 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/query.sql
+-rw-r--r--   0        0        0      585 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/schema.sql
+-rw-r--r--   0        0        0     2645 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/table.sql
+-rw-r--r--   0        0        0      726 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/table_freshness.sql
+-rw-r--r--   0        0        0      170 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/user.sql
+-rw-r--r--   0        0        0      719 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/view_ddl.sql
+-rw-r--r--   0        0        0      540 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/redshift/query.py
+-rw-r--r--   0        0        0      128 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/__init__.py
+-rw-r--r--   0        0        0     4128 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/client.py
+-rw-r--r--   0        0        0     1434 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/client_test.py
+-rw-r--r--   0        0        0     2443 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/extract.py
+-rw-r--r--   0        0        0       31 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/.sqlfluff
+-rw-r--r--   0        0        0     1130 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/column.sql
+-rw-r--r--   0        0        0     1179 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
+-rw-r--r--   0        0        0      483 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/database.sql
+-rw-r--r--   0        0        0      272 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
+-rw-r--r--   0        0        0      143 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
+-rw-r--r--   0        0        0     1779 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/query.sql
+-rw-r--r--   0        0        0       96 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/role.sql
+-rw-r--r--   0        0        0      730 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/schema.sql
+-rw-r--r--   0        0        0     1378 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/table.sql
+-rw-r--r--   0        0        0      570 2023-06-22 07:53:23.688088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/user.sql
+-rw-r--r--   0        0        0      673 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
+-rw-r--r--   0        0        0     1769 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/query.py
+-rw-r--r--   0        0        0       36 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/extract.py
+-rw-r--r--   0        0        0       26 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/.sqlfluff
+-rw-r--r--   0        0        0     1392 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/column.sql
+-rw-r--r--   0        0        0      138 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/database.sql
+-rw-r--r--   0        0        0     1110 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/query.sql
+-rw-r--r--   0        0        0      250 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/schema.sql
+-rw-r--r--   0        0        0     1049 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/table.sql
+-rw-r--r--   0        0        0       67 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/user.sql
+-rw-r--r--   0        0        0      249 2023-06-22 07:53:23.689088 castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/view_ddl.sql
+-rw-r--r--   0        0        0     5611 2023-06-22 07:53:23.690088 castor_extractor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 castor_extractor-0.4.0/PKG-INFO
```

### Comparing `castor_extractor-0.3.8/CHANGELOG.md` & `castor_extractor-0.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.4.0 - 2023-06-12
+
+* Added support for Sigma
+
 ## 0.3.8 - 2023-05-02
 
 * Added support for PowerBI datasets and fields
 
 ## 0.3.7 - 2023-04-28
 
 * Warning message to deprecate python < 3.8
```

### Comparing `castor_extractor-0.3.8/LICENCE` & `castor_extractor-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/README.md` & `castor_extractor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_bigquery.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_bigquery.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_looker.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_looker.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_metabase_api.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_metabase_api.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_metabase_db.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_metabase_db.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_mode.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_postgres.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_postgres.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_powerbi.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_powerbi.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_qlik.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_qlik.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_redshift.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_redshift.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_snowflake.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_snowflake.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/extract_tableau.py` & `castor_extractor-0.4.0/castor_extractor/commands/extract_tableau.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/file_check.py` & `castor_extractor-0.4.0/castor_extractor/commands/file_check.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/commands/upload.py` & `castor_extractor-0.4.0/castor_extractor/commands/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/column.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/column.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/column_test.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/column_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/enums.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/enums.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/file.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/file.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/file_test.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/file_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/file_test_users.csv` & `castor_extractor-0.4.0/castor_extractor/file_checker/file_test_users.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/file_checker/templates/generic_warehouse.py` & `castor_extractor-0.4.0/castor_extractor/file_checker/templates/generic_warehouse.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/logger.py` & `castor_extractor-0.4.0/castor_extractor/logger.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/transformation/dbt/client/client.py` & `castor_extractor-0.4.0/castor_extractor/transformation/dbt/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/transformation/dbt/client/credentials.py` & `castor_extractor-0.4.0/castor_extractor/transformation/dbt/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/uploader/constant.py` & `castor_extractor-0.4.0/castor_extractor/uploader/constant.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/uploader/env.py` & `castor_extractor-0.4.0/castor_extractor/uploader/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/uploader/upload.py` & `castor_extractor-0.4.0/castor_extractor/uploader/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/__init__.py` & `castor_extractor-0.4.0/castor_extractor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/deprecate.py` & `castor_extractor-0.4.0/castor_extractor/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/env.py` & `castor_extractor-0.4.0/castor_extractor/utils/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/files.py` & `castor_extractor-0.4.0/castor_extractor/utils/files.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/files_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/formatter.py` & `castor_extractor-0.4.0/castor_extractor/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/formatter_test.csv` & `castor_extractor-0.4.0/castor_extractor/utils/formatter_test.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/formatter_test.json` & `castor_extractor-0.4.0/castor_extractor/utils/formatter_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/formatter_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/formatter_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/object.py` & `castor_extractor-0.4.0/castor_extractor/utils/object.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, datetime
 from enum import Enum
-from typing import Any, Union, overload
+from typing import Any, Iterator, Union, overload
 from uuid import UUID
 
 from .type import Getter
 
 
 @overload
 def deep_serialize(__value: None) -> None:
@@ -32,14 +32,19 @@
 
 
 @overload
 def deep_serialize(__value: dict) -> dict:
     ...
 
 
+@overload
+def deep_serialize(__value: Iterator) -> Iterator:
+    ...
+
+
 def deep_serialize(value: Any) -> Any:
     """Deep serialize any data to primitive"""
     if isinstance(value, (float, int, str)) or value is None:
         return value
 
     if isinstance(value, (date, datetime)):
         return value.isoformat()
@@ -52,14 +57,17 @@
 
     if isinstance(value, (tuple, list, set)):
         return [deep_serialize(el) for el in value]
 
     if isinstance(value, dict):
         return {k: deep_serialize(v) for k, v in value.items()}
 
+    if isinstance(value, Iterator):
+        return (deep_serialize(item) for item in value)
+
     try:
         items = dict(value).items()
         return {k: deep_serialize(v) for k, v in items}
     except TypeError:
         raise ValueError(f"Value {str(value)} is not serializable")
```

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/object_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/pager.py` & `castor_extractor-0.4.0/castor_extractor/utils/pager.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/pager_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/pager_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/retry.py` & `castor_extractor-0.4.0/castor_extractor/utils/retry.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/retry_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/retry_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/safe.py` & `castor_extractor-0.4.0/castor_extractor/utils/safe.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/safe_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/safe_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/store.py` & `castor_extractor-0.4.0/castor_extractor/utils/store.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/string.py` & `castor_extractor-0.4.0/castor_extractor/utils/string.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/string_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/string_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/validation.py` & `castor_extractor-0.4.0/castor_extractor/utils/validation.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/validation_test.py` & `castor_extractor-0.4.0/castor_extractor/utils/validation_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/utils/write.py` & `castor_extractor-0.4.0/castor_extractor/utils/write.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/client_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/constants.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/sdk.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/sdk.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/sdk_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/sdk_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/api/utils.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/api/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/env.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/fields.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/fields_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/fields_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/looker/parameters.py` & `castor_extractor-0.4.0/castor_extractor/visualization/looker/parameters.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/assets.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/api/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/api/credentials.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/api/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/db/credentials.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/db/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/decryption.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/decryption.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/client/decryption_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/client/decryption_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/errors.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/metabase/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/metabase/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/assets.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client_test.json` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/client/client_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/client/credentials.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/errors.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/mode/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/mode/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/constants.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/credentials_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/credentials_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/rest.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/rest_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/utils.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/client/utils_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/client/utils_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/powerbi/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/powerbi/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/assets.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/constants.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/constants.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/error.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/error.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/error_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/error_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/json_rpc.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/json_rpc.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/engine/websocket.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/engine/websocket.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/master.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/master.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/rest.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/client/rest_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/qlik/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/qlik/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/assets.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/client.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/client_utils.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/credentials.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/project.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/project.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/client/safe_mode.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/client/safe_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/extract.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/gql_fields.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/gql_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/visualization/tableau/tsc_fields.py` & `castor_extractor-0.4.0/castor_extractor/visualization/tableau/tsc_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/abstract/asset.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/abstract/asset.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/abstract/client.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/abstract/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/abstract/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/abstract/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/abstract/query.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/abstract/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/abstract/time_filter.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/abstract/time_filter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/client.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/client_test.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/column.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/query.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/table.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/bigquery/query.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/bigquery/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/client.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/column.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/schema.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/queries/table.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/postgres/query.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/postgres/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/client.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/client_test.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/column.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/query.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/schema.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/table.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/table_freshness.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/table_freshness.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/queries/view_ddl.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/redshift/query.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/redshift/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/client.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/client_test.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/column.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/column_lineage.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/column_lineage.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/query.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/schema.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/table.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/user.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/user.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/queries/view_ddl.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/snowflake/query.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/synapse/extract.py` & `castor_extractor-0.4.0/castor_extractor/warehouse/synapse/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/column.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/query.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/castor_extractor/warehouse/synapse/queries/table.sql` & `castor_extractor-0.4.0/castor_extractor/warehouse/synapse/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.3.8/pyproject.toml` & `castor_extractor-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 
 [tool.poetry]
 name = "castor-extractor"
-version = "0.3.8"
+version = "0.4.0"
 description = "Extract your metadata assets."
 authors = ["Castor <support@castordoc.com>"]
 license = "EULA"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
@@ -78,33 +78,43 @@
   "snowflake-sqlalchemy",
 ]
 
 [tool.poetry.group.test.dependencies]
 black = "^22"
 flakehell = "^0.9.0"
 isort = "^5.8.0"
+pytest = "^6.1.2"
+pytest-freezegun = "^0.4.2"
+requests-mock = "^1.9.3"
 
 [tool.poetry.scripts]
 castor-extract-bigquery = "castor_extractor.commands.extract_bigquery:main"
 castor-extract-looker = "castor_extractor.commands.extract_looker:main"
 castor-extract-metabase-api = "castor_extractor.commands.extract_metabase_api:main"
 castor-extract-metabase-db = "castor_extractor.commands.extract_metabase_db:main"
 castor-extract-mode = "castor_extractor.commands.extract_mode:main"
 castor-extract-powerbi = "castor_extractor.commands.extract_powerbi:main"
 castor-extract-qlik = "castor_extractor.commands.extract_qlik:main"
 castor-extract-postgres = "castor_extractor.commands.extract_postgres:main"
 castor-extract-redshift = "castor_extractor.commands.extract_redshift:main"
 castor-extract-snowflake = "castor_extractor.commands.extract_snowflake:main"
+castor-extract-sigma = "castor_extractor.commands.extract_sigma:main"
 castor-extract-tableau = "castor_extractor.commands.extract_tableau:main"
 castor-file-check = "castor_extractor.commands.file_check:main"
 castor-upload = "castor_extractor.commands.upload:main"
 
 [[tool.poetry.source]]
 name = "test-pypi"
 url = "https://test.pypi.org/legacy/"
+priority = "primary"
+
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [tool.black]
 line-length = 80
 include = '\.pyi?$'
 exclude = '''
 (
   /(
@@ -125,14 +135,15 @@
 
 [tool.flakehell]
 format = "grouped"   # make output nice
 max_line_length = 80
 show_source = true   # show line of source code in output
 # the following is needed otherwise flake8 crashes
 extended_default_ignore = []
+exclude = [".venv/"]
 
 # list of plugins and rules for them
 [tool.flakehell.plugins]
 # include everything in pyflakes except F401
 pyflakes = ["+*", "-F401"]
 # enable only codes from S100 to S199
 flake8-bandit = ["-*", "+S1??"]
@@ -148,14 +159,23 @@
 combine_as_imports = true
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 80
 
+[tool.pytest.ini_options]
+log_level = "INFO"
+filterwarnings = [
+  "ignore:The Session.close_all",
+  "ignore:the imp module is deprecated",
+  "ignore:invalid escape sequence",
+  "ignore:Using or importing the ABCs",
+]
+
 [tool.sqlfluff.core]
 sql_file_exts = ".sql"
 exclude_rules = "L023,L025,L031,L032,L034"
 dialect = "postgres"
 
 [tool.sqlfluff.rules]
 max_line_length = 120
```

### Comparing `castor_extractor-0.3.8/PKG-INFO` & `castor_extractor-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: castor-extractor
-Version: 0.3.8
+Version: 0.4.0
 Summary: Extract your metadata assets.
 Home-page: https://www.castordoc.com/
 License: EULA
 Author: Castor
 Author-email: support@castordoc.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
 Provides-Extra: bigquery
 Provides-Extra: looker
 Provides-Extra: metabase
 Provides-Extra: qlik
 Provides-Extra: redshift
 Provides-Extra: snowflake
```

