# Comparing `tmp/propan-0.1.3.7.tar.gz` & `tmp/propan-0.1.3.8.tar.gz`

## Comparing `propan-0.1.3.7.tar` & `propan-0.1.3.8.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.7/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/grpc/gen_py_code.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/grpc/grpc_encoding.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/grpc/message.proto
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/grpc/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.7/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/__about__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/__main__.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/security.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    15906 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/app.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/redis.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/classes.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.7/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.7/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.7/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.7/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.7/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.7/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.7/README.md
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 propan-0.1.3.7/pyproject.toml
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 propan-0.1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.8/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/gen_py_code.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/grpc_encoding.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/message.proto
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/grpc/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.8/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__about__.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/__main__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/py.typed
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/app.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/nats.py
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/redis.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/sqs.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 propan-0.1.3.8/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.8/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.8/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.8/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.8/README.md
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 propan-0.1.3.8/pyproject.toml
+-rw-r--r--   0        0        0    17608 2020-02-02 00:00:00.000000 propan-0.1.3.8/PKG-INFO
```

### Comparing `propan-0.1.3.7/CONTRIBUTING.md` & `propan-0.1.3.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/SECURITY.md` & `propan-0.1.3.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.3.8/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.3.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.3.8/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/workflows/documentation.yml` & `propan-0.1.3.8/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/workflows/publish_coverage.yml` & `propan-0.1.3.8/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/workflows/publish_pypi.yml` & `propan-0.1.3.8/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/.github/workflows/tests.yml` & `propan-0.1.3.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/3_lifespan_events.py` & `propan-0.1.3.8/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/4_cli_attributes_promotion.py` & `propan-0.1.3.8/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/5_publishing.py` & `propan-0.1.3.8/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/6_arguments_casting.py` & `propan-0.1.3.8/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/7_handler_errors_processing.py` & `propan-0.1.3.8/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/1_dependency_injection.py` & `propan-0.1.3.8/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.3.8/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.3.8/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.3.8/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.3.8/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/dependencies/7_annotated.py` & `propan-0.1.3.8/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/grpc/grpc_encoding.py` & `propan-0.1.3.8/examples/grpc/grpc_encoding.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/quart.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.3.8/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/rabbit/direct.py` & `propan-0.1.3.8/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/rabbit/fanout.py` & `propan-0.1.3.8/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/rabbit/header.py` & `propan-0.1.3.8/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/rabbit/topic.py` & `propan-0.1.3.8/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/redis/direct.py` & `propan-0.1.3.8/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/examples/redis/pattern.py` & `propan-0.1.3.8/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/__about__.py` & `propan-0.1.3.8/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.3.7"
+__version__ = "0.1.3.8"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.3.7/propan/__init__.py` & `propan-0.1.3.8/propan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 from propan import __about__ as about
 from propan.cli.app import *  # noqa: F403
 from propan.log import *  # noqa: F403
 from propan.utils import *  # noqa: F403
 
 try:
     from propan.brokers.rabbit import RabbitBroker
-except Exception:
+except ImportError:
     RabbitBroker = about.INSTALL_RABBIT  # type: ignore
 
 try:
     from propan.brokers.nats import NatsBroker
-except Exception:
+except ImportError:
     NatsBroker = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.brokers.redis import RedisBroker
-except Exception:
+except ImportError:
     RedisBroker = about.INSTALL_REDIS  # type: ignore
 
 try:
     from propan.brokers.kafka import KafkaBroker
-except Exception:
+except ImportError:
     KafkaBroker = about.INSTALL_KAFKA  # type: ignore
 
 try:
     from propan.brokers.sqs import SQSBroker
-except Exception:
+except ImportError:
     SQSBroker = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitBroker, NatsBroker, RedisBroker, SQSBroker, KafkaBroker)
 ), about.INSTALL_MESSAGE
 
 __all__ = (  # noqa: F405
```

### Comparing `propan-0.1.3.7/propan/annotations.py` & `propan-0.1.3.8/propan/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,62 +21,62 @@
     from propan.brokers.rabbit import RabbitBroker as RB
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
     RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
     Channel = Annotated[
         aio_pika.robust_channel.RobustChannel, ContextField("broker.channel")
     ]
-except Exception:
+except ImportError:
     RabbitBroker = RabbitMessage = Channel = about.INSTALL_RABBIT
 
 
 try:
     from nats.aio.msg import Msg
 
     from propan.brokers.nats import NatsBroker as NB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
-except Exception:
+except ImportError:
     NatsBroker = NatsMessage = about.INSTALL_NATS
 
 
 try:
     from redis.asyncio.client import Redis as R
 
     from propan.brokers.redis import RedisBroker as RedB
 
     RedisBroker = Annotated[RedB, ContextField("broker")]
     Redis = Annotated[R, ContextField("broker._connection")]
-except Exception:
+except ImportError:
     RedisBroker = Redis = about.INSTALL_REDIS
 
 
 try:
     from aiokafka import AIOKafkaProducer
     from aiokafka.structs import ConsumerRecord
 
     from propan.brokers.kafka import KafkaBroker as KB
 
     KafkaBroker = Annotated[KB, ContextField("broker")]
     KafkaMessage = Annotated[ConsumerRecord, ContextField("message")]
     Producer = Annotated[AIOKafkaProducer, ContextField("producer")]
-except Exception:
+except ImportError:
     KafkaBroker = KafkaMessage = Producer = about.INSTALL_KAFKA
 
 
 try:
     from aiobotocore.client import AioBaseClient
 
     from propan.brokers.sqs import SQSBroker as SB
 
     SQSBroker = Annotated[SB, ContextField("broker")]
     client = Annotated[AioBaseClient, ContextField("client")]
     queue_url = Annotated[str, ContextField("queue_url")]
-except Exception:
+except ImportError:
     SQSBroker = client = queue_url = about.INSTALL_SQS
 
 
 assert any(
     (
         all((RabbitBroker, RabbitMessage, Channel)),
         all((NatsBroker, NatsMessage)),
```

### Comparing `propan-0.1.3.7/propan/types.py` & `propan-0.1.3.8/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/asyncapi/__init__.py` & `propan-0.1.3.8/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/asyncapi/channels.py` & `propan-0.1.3.8/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/asyncapi/info.py` & `propan-0.1.3.8/propan/asyncapi/bindings/redis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-import importlib.util
 from typing import Optional
 
-from pydantic import BaseModel, Field, HttpUrl
+from pydantic import BaseModel, Field
+from typing_extensions import Literal
 
-if importlib.util.find_spec("email_validator"):
-    from pydantic import EmailStr
-else:
-    EmailStr = str  # type: ignore
+from propan.types import AnyDict
 
 
-class AsyncAPIContact(BaseModel):
-    name: str
-    url: HttpUrl
-    email: Optional[EmailStr] = None
-
-
-class AsyncAPILicense(BaseModel):
-    name: str
-    url: HttpUrl
+class AsyncAPIRedisChannelBinding(BaseModel):
+    channel: str
+    method: Literal["ssubscribe", "psubscribe", "subscribe"] = "subscribe"
+    version: str = Field(
+        default="custom",
+        alias="bindingVersion",
+    )
 
 
-class AsyncAPIInfo(BaseModel):
-    title: str
-    version: str = "1.0.0"
-    description: str = ""
-    terms: Optional[HttpUrl] = Field(
-        default=None,
-        alias="termsOfService",
+class AsyncAPIRedisOperationBinding(BaseModel):
+    reply_to: Optional[AnyDict] = Field(default=None, alias="replyTo")
+    version: str = Field(
+        default="custom",
+        alias="bindingVersion",
     )
-    contact: Optional[AsyncAPIContact] = None
-    license: Optional[AsyncAPILicense] = None
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/main.py` & `propan-0.1.3.8/propan/asyncapi/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     # correlationIds
     # operationTraits
     # messageTraits
     # serverBindings
     # channelBindings
     # operationBindings
     # messageBindings
-    class Config:
-        allow_population_by_field_name = True
 
 
 class AsyncAPISchema(BaseModel):
     asyncapi: str = ASYNC_API_VERSION
     default_content_type: str = Field(
         default=ContentTypes.json.value,
         alias="defaultContentType",
@@ -48,10 +46,7 @@
         default=None,
         alias="externalDocs",
     )
 
     # TODO:
     # id
     components: Optional[AsyncAPIComponents] = None
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/message.py` & `propan-0.1.3.8/propan/asyncapi/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,10 +37,7 @@
     # traits
 
     tags: Optional[List[AsyncAPITag]] = None
     external_docs: Optional[AsyncAPIExternalDocs] = Field(
         default=None,
         alias="externalDocs",
     )
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/security.py` & `propan-0.1.3.8/propan/asyncapi/security.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,14 @@
         alias="clientCredentials",
     )
     authorization_code: Optional[AsyncAPIOauthFlowObj] = Field(
         default=None,
         alias="authorizationCode",
     )
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 class AsyncAPISecuritySchemeComponent(BaseModel):
     type: Literal[
         "userPassword",
         "apikey",
         "X509",
         "symmetricEncryption",
@@ -64,10 +61,7 @@
         alias="bearerFormat",
     )
     openid_connect_url: Optional[str] = Field(
         default=None,
         alias="openIdConnectUrl",
     )
     flows: Optional[AsyncAPIOauthFlows] = None
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/subscription.py` & `propan-0.1.3.8/propan/asyncapi/subscription.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,10 +26,7 @@
     # traits
 
     tags: Optional[List[AsyncAPITag]] = None
     external_docs: Optional[AsyncAPIExternalDocs] = Field(
         default=None,
         alias="externalDocs",
     )
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/utils.py` & `propan-0.1.3.8/propan/asyncapi/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import sys
 from typing import Optional, Type
 
+from fast_depends._compat import PYDANTIC_V2
 from pydantic import BaseModel, Field
 
 
 class AsyncAPIExternalDocs(BaseModel):
     url: str = ""
     description: str = ""
 
@@ -14,20 +15,17 @@
     name: str
     description: str = ""
     external_docs: Optional[AsyncAPIExternalDocs] = Field(
         default=None,
         alias="externalDocs",
     )
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 def add_example_to_model(model: Type[BaseModel]) -> Type[BaseModel]:
-    if sys.version_info >= (3, 8):
+    if sys.version_info >= (3, 8) and not PYDANTIC_V2:
         from polyfactory.factories.pydantic_factory import ModelFactory
 
         factory = type(
             f"{model.__name__}_factory", (ModelFactory,), {"__model__": model}
         )
 
         return type(
```

### Comparing `propan-0.1.3.7/propan/asyncapi/bindings/amqp.py` & `propan-0.1.3.8/propan/asyncapi/bindings/amqp.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,49 +9,37 @@
 class AsyncAPIAmqpQueue(BaseModel):
     name: str
     durable: bool
     exclusive: bool
     auto_delete: bool = Field(alias="autoDelete")
     vhost: str = "/"
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 class AsyncAPIAmqpExchange(BaseModel):
     name: Optional[str] = None
     type: Literal["default", "direct", "topic", "fanout", "headers"]
     durable: Optional[bool] = None
     auto_delete: Optional[bool] = Field(
         default=None,
         alias="autoDelete",
     )
     vhost: str = "/"
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 class AsyncAPIAmqpChannelBinding(BaseModel):
     is_: Literal["queue", "routingKey"] = Field(..., alias="is")
     version: str = Field(
         default="0.2.0",
         alias="bindingVersion",
     )
     queue: Optional[AsyncAPIAmqpQueue] = None
     exchange: Optional[AsyncAPIAmqpExchange] = None
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 class AsyncAPIAmqpOperationBinding(BaseModel):
     cc: Optional[str] = None
     ack: bool = True
     reply_to: Optional[AnyDict] = Field(default=None, alias="replyTo")
     version: str = Field(
         default="0.2.0",
         alias="bindingVersion",
     )
-
-    class Config:
-        allow_population_by_field_name = True
```

### Comparing `propan-0.1.3.7/propan/asyncapi/bindings/main.py` & `propan-0.1.3.8/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/brokers/push_back_watcher.py` & `propan-0.1.3.8/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/brokers/_model/broker_usecase.py` & `propan-0.1.3.8/propan/brokers/_model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     Dict,
     Generic,
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
-    TypeVar,
     Union,
     cast,
 )
 
-from fast_depends.construct import get_dependant
-from fast_depends.model import Dependant, Depends
+from fast_depends.core import CallModel, build_call_model
+from fast_depends.dependencies import Depends
 from fast_depends.utils import args_to_kwargs
-from typing_extensions import Self, TypeAlias
+from typing_extensions import ParamSpec, Self, TypeAlias, TypeVar
 
 from propan.brokers._model.schemas import BaseHandler, PropanMessage
 from propan.brokers._model.utils import (
     ContentType,
     ContentTypes,
     change_logger_handlers,
     get_watcher,
@@ -59,14 +58,22 @@
             Callable[[PropanMessage[MsgType]], Awaitable[DecodedMessage]],
         ],
         Awaitable[DecodedMessage],
     ]
 ]
 
 
+P = ParamSpec("P")
+R = TypeVar("R")
+
+
+def WRAPPED_BUILDER(path: str, call: Callable[P, R]) -> CallModel[P, R]:
+    return build_call_model(call)
+
+
 class BrokerUsecase(ABC, Generic[MsgType, ConnectionType]):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: Sequence[BaseHandler]
     dependencies: Sequence[Depends]
     _global_parser: CustomParser[MsgType]
     _global_decoder: CustomDecoder[MsgType]
@@ -172,15 +179,18 @@
         *broker_args: Any,
         retry: Union[bool, int] = False,
         dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
         parse_message: CustomParser[MsgType] = None,
         description: str = "",
         _raw: bool = False,
-        _get_dependant: Callable[[Callable[..., Any]], Dependant] = get_dependant,
+        _get_dependant: Callable[
+            ...,
+            CallModel,
+        ] = WRAPPED_BUILDER,
         **broker_kwargs: Any,
     ) -> HandlerWrapper:
         raise NotImplementedError()
 
     @staticmethod
     async def _decode_message(message: PropanMessage[MsgType]) -> DecodedMessage:
         body = message.body
@@ -217,23 +227,24 @@
         self,
         func: Union[Callable[..., T], Callable[..., Awaitable[T]]],
         retry: Union[bool, int] = False,
         extra_dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
         parse_message: CustomParser[MsgType] = None,
         _raw: bool = False,
-        _get_dependant: Callable[..., Dependant] = get_dependant,
+        _get_dependant: Callable[..., CallModel] = WRAPPED_BUILDER,
         **broker_log_context_kwargs: Any,
-    ) -> Tuple[Callable[[MsgType, bool], Awaitable[Optional[T]]], Dependant]:
+    ) -> Tuple[Callable[[MsgType, bool], Awaitable[Optional[T]]], CallModel]:
         dependant = _get_dependant(path="", call=func)
         extra = [
             _get_dependant(path="", call=d.dependency)
             for d in chain(extra_dependencies, self.dependencies)
         ]
-        dependant.dependencies.extend(extra)
+
+        extend_dependencies(extra)(dependant)
 
         if getattr(dependant, "flat_params", None) is None:  # handle FastAPI Dependant
             params = dependant.path_params + dependant.body_params
 
             for d in dependant.dependencies:
                 params.extend(d.path_params + d.body_params)
 
@@ -245,15 +256,15 @@
             dependant.flat_params = params_unique
 
         f = cast(Callable[..., Awaitable[T]], to_async(func))
 
         if self._is_apply_types is True:
             f = apply_types(
                 func=f,
-                wrap_dependant=extend_dependencies(extra),
+                wrap_model=extend_dependencies(extra),
             )
 
         f = self._wrap_decode_message(
             func=f,
             _raw=_raw,
             params=tuple(chain(dependant.flat_params, extra)),
             decoder=decode_message or self._global_decoder,
@@ -361,13 +372,16 @@
     ) -> None:
         if self.logger is not None:
             self.logger.log(
                 level=(log_level or self.log_level), msg=message, extra=extra
             )
 
 
-def extend_dependencies(extra: Sequence[Dependant]) -> Callable[[Dependant], Dependant]:
-    def dependant_wrapper(dependant: Dependant) -> Dependant:
-        dependant.dependencies.extend(extra)
+def extend_dependencies(extra: Sequence[CallModel]) -> Callable[[CallModel], CallModel]:
+    def dependant_wrapper(dependant: CallModel) -> CallModel:
+        if isinstance(dependant, CallModel):
+            dependant.extra_dependencies.extend(extra)
+        else:  # FastAPI dependencies
+            dependant.dependencies.extend(extra)
         return dependant
 
     return dependant_wrapper
```

### Comparing `propan-0.1.3.7/propan/brokers/_model/schemas.py` & `propan-0.1.3.8/propan/brokers/_model/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from abc import abstractmethod
 from dataclasses import dataclass
-from inspect import _empty
-from typing import Any, Dict, Generic, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 from pydantic import BaseModel, Field, Json, create_model
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.utils import add_example_to_model
 from propan.types import AnyDict, DecodedMessage, DecoratedCallable
 
 
 @dataclass
 class BaseHandler:
     callback: DecoratedCallable
-    dependant: Dependant
+    dependant: CallModel
     _description: str
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         _description: str = "",
     ):
         self.callback = callback
         self.dependant = dependant
         self._description = _description
 
     @abstractmethod
@@ -42,89 +41,92 @@
         return self._description or self.callback.__doc__
 
     def get_message_object(self) -> Tuple[str, AnyDict, Optional[AnyDict]]:
         import jsonref  # hide it there to remove docs dependencies from main package
 
         dependant = self.dependant
 
-        if getattr(dependant, "return_field", None) is not None:
-            return_field = dependant.return_field
+        if getattr(dependant, "response_model", None) is not None:
+            response_model: Type[BaseModel] = dependant.response_model
+            return_field = list(response_model.__fields__.values())[0]
+
+            if (
+                return_field.annotation != Any  # NOTE: 3.7-3.10 compatibility
+                and issubclass(return_field.annotation, BaseModel)
+            ):
+                response_model = return_field.annotation
+
+                schema_extra = response_model.Config.schema_extra
+                if not isinstance(schema_extra, dict) or not schema_extra.get(
+                    "example"
+                ):
+                    response_model = add_example_to_model(response_model)
 
-            if return_field.type_ != Any and issubclass(return_field.type_, BaseModel):
-                return_model = return_field.type_
-                if not return_model.Config.schema_extra.get("example"):
-                    return_model = add_example_to_model(return_model)
                 return_info = jsonref.replace_refs(
-                    return_model.schema(), jsonschema=True, proxies=False
+                    response_model.schema(), jsonschema=True, proxies=False
                 )
-                return_info["examples"] = [return_info.pop("example", [])]
+                return_info["examples"] = [return_info.pop("example", None)]
 
             else:
-                return_model = create_model(  # type: ignore
-                    f"{self.title}Reply",
-                    **{return_field.name: (return_field.annotation, ...)},
-                )
-                return_model = add_example_to_model(return_model)
-                return_info = jsonref.replace_refs(
-                    return_model.schema(), jsonschema=True, proxies=False
-                )
-                return_info.pop("required")
-                return_info.update(
-                    {
-                        "type": return_info.pop("properties", {})
-                        .get(return_field.name, {})
-                        .get("type"),
-                        "examples": [
-                            return_info.pop("example", {}).get(return_field.name)
-                        ],
-                    }
+                response_model = add_example_to_model(response_model)
+                response_field_name = "response"
+
+                raw = jsonref.replace_refs(
+                    response_model.schema(),
+                    jsonschema=True,
+                    proxies=False,
                 )
 
+                return_info = raw.get("properties", {}).get(response_field_name)
+                return_info["examples"] = [
+                    raw.pop("example", {}).get(response_field_name)
+                ]
+                return_info["title"] = f"{self.title}Reply"
         else:
             return_info = None
 
         payload_title = f"{self.title}Payload"
         params = dependant.flat_params
         params_number = len(params)
 
         gen_examples: bool
         use_original_model = False
         if params_number == 0:
             model = None
 
         elif params_number == 1:
-            param = params[0]
+            name, param = list(params.items())[0]
+            info = getattr(param, "field_info", param)
 
-            if param.annotation != Any and issubclass(param.annotation, BaseModel):
+            if (
+                param.annotation != Any  # NOTE: 3.7-3.10 compatibility
+                and issubclass(param.annotation, BaseModel)
+            ):
                 model = param.annotation
-                gen_examples = model.Config.schema_extra.get("example") is None
+
+                schema_extra = model.Config.schema_extra
+                if isinstance(schema_extra, dict):
+                    gen_examples = schema_extra.get("example") is None
+                else:
+                    gen_examples = True
+
                 use_original_model = True
 
             else:
-                is_pydantic = param.field_info.default is not _empty
                 model = create_model(  # type: ignore
-                    param.field_info.title or payload_title,
-                    **{
-                        param.name: (
-                            param.annotation,
-                            param.field_info if is_pydantic else ...,
-                        )
-                    },
+                    info.title or payload_title,
+                    **{name: (param.annotation, info)},
                 )
                 gen_examples = True
-
         else:
             model = create_model(  # type: ignore
                 payload_title,
                 **{
-                    p.name: (
-                        p.annotation,
-                        ... if p.field_info.default is _empty else p.field_info,
-                    )
-                    for p in params
+                    i: (j.annotation, getattr(j, "field_info", j))
+                    for i, j in params.items()
                 },
             )
             gen_examples = True
 
         body: AnyDict
         if model is None:
             body = {"title": payload_title, "type": "null"}
```

### Comparing `propan-0.1.3.7/propan/brokers/_model/utils.py` & `propan-0.1.3.8/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.3.8/propan/brokers/kafka/kafka_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Tuple,
     Union,
 )
 from uuid import uuid4
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
```

### Comparing `propan-0.1.3.7/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.3.8/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Union,
 )
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
 from aiokafka.structs import ConsumerRecord
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import (
```

### Comparing `propan-0.1.3.7/propan/brokers/kafka/schemas.py` & `propan-0.1.3.8/propan/brokers/kafka/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional
 
 from aiokafka import AIOKafkaConsumer
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     kafka,
 )
 from propan.asyncapi.channels import AsyncAPIChannel
@@ -25,15 +25,15 @@
     consumer: Optional[AIOKafkaConsumer] = None
     task: Optional["asyncio.Task[Any]"] = None
     consumer_kwargs: AnyDict = field(default_factory=dict)
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         topics: List[str],
         group_id: Optional[str] = None,
         consumer: Optional[AIOKafkaConsumer] = None,
         task: Optional["asyncio.Task[Any]"] = None,
         consumer_kwargs: Optional[AnyDict] = None,
         _description: str = "",
     ):
```

### Comparing `propan-0.1.3.7/propan/brokers/nats/nats_broker.py` & `propan-0.1.3.8/propan/brokers/nats/nats_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
 
 import nats
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from nats.aio.client import Callback, Client, ErrorCallback
 from nats.aio.msg import Msg
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
```

### Comparing `propan-0.1.3.7/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.3.8/propan/brokers/nats/nats_broker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     List,
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
 
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
     DEFAULT_DRAIN_TIMEOUT,
     DEFAULT_INBOX_PREFIX,
     DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
     DEFAULT_MAX_OUTSTANDING_PINGS,
     DEFAULT_MAX_RECONNECT_ATTEMPTS,
```

### Comparing `propan-0.1.3.7/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.3.8/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/brokers/nats/schemas.py` & `propan-0.1.3.8/propan/brokers/nats/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Dict, Optional, Sequence
 
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 from nats.aio.subscription import Subscription
 from nats.js.api import DEFAULT_PREFIX
 from pydantic import BaseModel
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
@@ -24,15 +24,15 @@
     queue: str = ""
 
     subscription: Optional[Subscription] = None
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         subject: str,
         queue: str = "",
         subscription: Optional[Subscription] = None,
         _description: str = "",
     ):
         self.callback = callback
         self.dependant = dependant
```

### Comparing `propan-0.1.3.7/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Union,
 )
 from uuid import uuid4
 
 import aio_pika
 import aiormq
 from aio_pika.abc import DeliveryMode
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 from yarl import URL
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
```

### Comparing `propan-0.1.3.7/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.3.8/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     TypeVar,
     Union,
 )
 
 import aio_pika
 import aiormq
 from aio_pika.message import IncomingMessage
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from pamqp.common import FieldTable
 from typing_extensions import ParamSpec, TypeAlias
 from yarl import URL
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
```

### Comparing `propan-0.1.3.7/propan/brokers/rabbit/schemas.py` & `propan-0.1.3.8/propan/brokers/rabbit/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Any, Dict, Optional
 
 from aio_pika.abc import ExchangeType, TimeoutType
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 from pydantic import Field
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     amqp,
 )
@@ -137,15 +137,15 @@
 class Handler(BaseHandler):
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = field(default=None)
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
         _description: str = "",
     ):
         self.callback = callback
         self.dependant = dependant
         self.queue = queue
@@ -177,34 +177,36 @@
                         correlationId=AsyncAPICorrelationId(
                             location="$message.header#/correlation_id"
                         ),
                     ),
                 ),
                 bindings=AsyncAPIChannelBinding(
                     amqp=amqp.AsyncAPIAmqpChannelBinding(
-                        is_="routingKey",  # type: ignore
-                        queue=None
-                        if (
-                            self.exchange
-                            and self.exchange.type
-                            in (ExchangeType.FANOUT, ExchangeType.HEADERS)
-                        )
-                        else amqp.AsyncAPIAmqpQueue(
-                            name=self.queue.name,
-                            durable=self.queue.durable,
-                            exclusive=self.queue.exclusive,
-                            autoDelete=self.queue.auto_delete,
-                        ),
-                        exchange=(
-                            amqp.AsyncAPIAmqpExchange(type="default")
-                            if self.exchange is None
-                            else amqp.AsyncAPIAmqpExchange(
-                                type=self.exchange.type.value,  # type: ignore
-                                name=self.exchange.name,
-                                durable=self.exchange.durable,
-                                autoDelete=self.exchange.auto_delete,
+                        **{
+                            "is": "routingKey",  # type: ignore
+                            "queue": None
+                            if (
+                                self.exchange
+                                and self.exchange.type
+                                in (ExchangeType.FANOUT, ExchangeType.HEADERS)
                             )
-                        ),
+                            else amqp.AsyncAPIAmqpQueue(
+                                name=self.queue.name,
+                                durable=self.queue.durable,
+                                exclusive=self.queue.exclusive,
+                                autoDelete=self.queue.auto_delete,
+                            ),
+                            "exchange": (
+                                amqp.AsyncAPIAmqpExchange(type="default")
+                                if self.exchange is None
+                                else amqp.AsyncAPIAmqpExchange(
+                                    type=self.exchange.type.value,  # type: ignore
+                                    name=self.exchange.name,
+                                    durable=self.exchange.durable,
+                                    autoDelete=self.exchange.auto_delete,
+                                )
+                            ),
+                        }
                     )
                 ),
             ),
         }
```

### Comparing `propan-0.1.3.7/propan/brokers/redis/redis_broker.py` & `propan-0.1.3.8/propan/brokers/redis/redis_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     NoReturn,
     Optional,
     Sequence,
     TypeVar,
 )
 from uuid import uuid4
 
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from redis.asyncio.client import PubSub, Redis
 from redis.asyncio.connection import ConnectionPool, parse_url
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage, RawDecoced
 from propan.brokers.push_back_watcher import BaseWatcher
```

### Comparing `propan-0.1.3.7/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.3.8/propan/brokers/redis/redis_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
 )
 
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from redis.asyncio.client import Redis
 from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
```

### Comparing `propan-0.1.3.7/propan/brokers/redis/schemas.py` & `propan-0.1.3.8/propan/brokers/redis/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 from pydantic import BaseModel, Field
 from redis.asyncio.client import PubSub
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     redis,
@@ -25,15 +25,15 @@
 
     task: Optional["asyncio.Task[Any]"] = None
     subscription: Optional[PubSub] = None
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         channel: str,
         pattern: bool = False,
         task: Optional["asyncio.Task[Any]"] = None,
         subscription: Optional[PubSub] = None,
         _description: str = "",
     ):
         self.callback = callback
```

### Comparing `propan-0.1.3.7/propan/brokers/sqs/schema.py` & `propan-0.1.3.8/propan/brokers/sqs/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from dataclasses import dataclass
 from dataclasses import field as DField
 from typing import Any, Dict, Optional, Sequence
 
-from fast_depends.model import Dependant
+from fast_depends.core import CallModel
 from pydantic import BaseModel, Field, PositiveInt
 from typing_extensions import Literal
 
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     sqs,
@@ -213,15 +213,15 @@
     consumer_params: AnyDict
 
     task: Optional["asyncio.Task[Any]"] = None
 
     def __init__(
         self,
         callback: DecoratedCallable,
-        dependant: Dependant,
+        dependant: CallModel,
         queue: SQSQueue,
         consumer_params: AnyDict,
         _description: str = "",
         task: Optional["asyncio.Task[Any]"] = None,
     ):
         self.callback = callback
         self.dependant = dependant
```

### Comparing `propan-0.1.3.7/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.3.8/propan/brokers/sqs/sqs_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeVar,
     Union,
 )
 from uuid import uuid4
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.session import get_session
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
```

### Comparing `propan-0.1.3.7/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.3.8/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Sequence,
     TypeVar,
     Union,
 )
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.config import AioConfig
-from fast_depends.model import Depends
+from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.sqs.schema import Handler, SQSQueue
```

### Comparing `propan-0.1.3.7/propan/cli/app.py` & `propan-0.1.3.8/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/main.py` & `propan-0.1.3.8/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/docs/app.py` & `propan-0.1.3.8/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/docs/gen.py` & `propan-0.1.3.8/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/docs/serving.py` & `propan-0.1.3.8/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/core.py` & `propan-0.1.3.8/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/app.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/core.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/nats.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/redis.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.3.8/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/supervisors/basereload.py` & `propan-0.1.3.8/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/supervisors/multiprocess.py` & `propan-0.1.3.8/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/supervisors/utils.py` & `propan-0.1.3.8/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/supervisors/watchfiles.py` & `propan-0.1.3.8/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/utils/imports.py` & `propan-0.1.3.8/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/utils/logs.py` & `propan-0.1.3.8/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/cli/utils/parser.py` & `propan-0.1.3.8/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/__init__.py` & `propan-0.1.3.8/propan/fastapi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from propan import __about__ as about
 
 try:
     from propan.fastapi.rabbit import RabbitRouter
-except Exception:
+except ImportError:
     RabbitRouter = about.INSTALL_RABBIT  # type: ignore
 
 try:
     from propan.fastapi.redis import RedisRouter
-except Exception:
+except ImportError:
     RedisRouter = about.INSTALL_REDIS  # type: ignore
 
 try:
     from propan.fastapi.kafka import KafkaRouter
-except Exception:
+except ImportError:
     KafkaRouter = about.INSTALL_KAFKA  # type: ignore
 
 try:
     from propan.fastapi.nats import NatsRouter
-except Exception:
+except ImportError:
     NatsRouter = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.fastapi.sqs import SQSRouter
-except Exception:
+except ImportError:
     SQSRouter = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitRouter, RedisRouter, KafkaRouter, NatsRouter, SQSRouter)
 ), about.INSTALL_MESSAGE
 
 __all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter", "SQSRouter")
```

### Comparing `propan-0.1.3.7/propan/fastapi/core/route.py` & `propan-0.1.3.8/propan/fastapi/core/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             )
         )
 
         broker.handle(
             path,
             *extra,
             _raw=True,
-            _get_dependant=get_dependant,  # type: ignore
+            _get_dependant=get_dependant,
             **handle_kwargs,  # type: ignore
         )(handler)
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
```

### Comparing `propan-0.1.3.7/propan/fastapi/core/router.py` & `propan-0.1.3.8/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/kafka/router.pyi` & `propan-0.1.3.8/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/nats/router.pyi` & `propan-0.1.3.8/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/rabbit/router.pyi` & `propan-0.1.3.8/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/redis/router.pyi` & `propan-0.1.3.8/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/fastapi/sqs/router.pyi` & `propan-0.1.3.8/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/log/formatter.py` & `propan-0.1.3.8/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/log/logging.py` & `propan-0.1.3.8/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/test/__init__.py` & `propan-0.1.3.8/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/test/kafka.py` & `propan-0.1.3.8/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/test/nats.py` & `propan-0.1.3.8/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/test/rabbit.py` & `propan-0.1.3.8/propan/test/rabbit.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,33 +97,45 @@
     )
 
     for handler in self.handlers:  # pragma: no branch
         if not handler.exchange:
             if not exchange:  # pragma: no branch
                 if handler.queue.name == incoming.routing_key:
                     r = await call_handler(
-                        handler, incoming, callback, callback_timeout, raise_timeout
+                        handler,
+                        incoming,
+                        callback,
+                        callback_timeout,
+                        raise_timeout,
                     )
                     if callback:  # pragma: no branch
                         return r
 
         elif (  # pragma: no branch
             handler.exchange.type == ExchangeType.DIRECT
             or handler.exchange.type == ExchangeType.TOPIC
         ):
             if handler.queue.name == incoming.routing_key:
                 r = await call_handler(
-                    handler, incoming, callback, callback_timeout, raise_timeout
+                    handler,
+                    incoming,
+                    callback,
+                    callback_timeout,
+                    raise_timeout,
                 )
                 if callback:
                     return r
 
         elif handler.exchange.type == ExchangeType.FANOUT:
             r = await call_handler(
-                handler, incoming, callback, callback_timeout, raise_timeout
+                handler,
+                incoming,
+                callback,
+                callback_timeout,
+                raise_timeout,
             )
             if callback:
                 return r
 
 
 def TestRabbitBroker(broker: RabbitBroker) -> RabbitBroker:
     broker._channel = AsyncMock()
```

### Comparing `propan-0.1.3.7/propan/test/redis.py` & `propan-0.1.3.8/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/test/sqs.py` & `propan-0.1.3.8/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/utils/functions.py` & `propan-0.1.3.8/propan/utils/functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import inspect
 from functools import wraps
 from typing import Awaitable, Callable, List, TypeVar, Union, cast
 
-from fast_depends.injector import run_async as call_or_await
+from fast_depends.utils import run_async as call_or_await
 from typing_extensions import ParamSpec
 
 __all__ = (
     "call_or_await",
     "to_async",
 )
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def to_async(
-    func: Union[Callable[P, T], Callable[P, Awaitable[T]]]
+    func: Union[
+        Callable[P, T],
+        Callable[P, Awaitable[T]],
+    ]
 ) -> Callable[P, Awaitable[T]]:
     @wraps(func)
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         r = await call_or_await(func, *args, **kwargs)
         return cast(T, r)
 
     return wrapper
```

### Comparing `propan-0.1.3.7/propan/utils/context/main.py` & `propan-0.1.3.8/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/propan/utils/context/types.py` & `propan-0.1.3.8/propan/utils/context/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,42 @@
 
 from propan.types import AnyDict
 from propan.utils.context import context
 
 
 class Context(CustomField):  # type: ignore
     def __init__(
-        self, real_name: str = "", *, cast: bool = False, default: Any = _empty
+        self,
+        real_name: str = "",
+        *,
+        cast: bool = False,
+        default: Any = _empty,
     ):
         self.name = real_name
         self.default = default
-        super().__init__(cast=cast, required=(default is _empty))
+        super().__init__(
+            cast=cast,
+            required=(default is _empty),
+        )
 
     def use(self, **kwargs: AnyDict) -> AnyDict:
         name = self.name or self.param_name
-        default = None if self.default is _empty else self.default
-        return {**kwargs, self.param_name: resolve_context(name) or default}
+
+        try:
+            kwargs[self.param_name] = resolve_context(name)
+        except (KeyError, AttributeError):
+            if self.required is False:
+                kwargs[self.param_name] = self.default
+
+        return kwargs
 
 
 def resolve_context(argument: str) -> Any:
     keys = argument.split(".")
 
-    v = context.context.get(keys[0])
+    v = context.context[keys[0]]
     for i in keys[1:]:
-        v = getattr(v, i, None)
+        v = getattr(v, i)
         if v is None:
             return v
 
     return v
```

### Comparing `propan-0.1.3.7/LICENSE` & `propan-0.1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/README.md` & `propan-0.1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.7/pyproject.toml` & `propan-0.1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends==1.1.6",
+    "fast-depends==2.0.2",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
@@ -76,15 +76,15 @@
 async-kafka = [
     "aiokafka>=0.8",
 ]
 
 doc = [
     "PyYAML",
     "pydantic[email]",
-    "polyfactory; python_version > '3.7'",
+    "polyfactory>=2.3.0; python_version > '3.7'",
     "jsonref",
     "fastapi",
     "uvicorn",
 ]
 
 async-sqs = [
     "aiobotocore",
@@ -98,15 +98,15 @@
     "propan[async-kafka]",
     "propan[async-sqs]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
 
-    "fastapi",
+    "fastapi==0.100.0b1",
     "python-dotenv",
 
     "asyncmock; python_version < '3.8'",
 ]
 
 dev-doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
```

### Comparing `propan-0.1.3.7/PKG-INFO` & `propan-0.1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.3.7
+Version: 0.1.3.8
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -31,15 +31,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: fast-depends==1.1.6
+Requires-Dist: fast-depends==2.0.2
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-kafka
 Requires-Dist: aiokafka>=0.8; extra == 'async-kafka'
 Provides-Extra: async-nats
 Requires-Dist: nats-py!=2.3.0,>=2; extra == 'async-nats'
@@ -65,22 +65,22 @@
 Requires-Dist: mkdocs-macros-plugin; extra == 'dev-doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'dev-doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'dev-doc'
 Requires-Dist: typer[all]; extra == 'dev-doc'
 Provides-Extra: doc
 Requires-Dist: fastapi; extra == 'doc'
 Requires-Dist: jsonref; extra == 'doc'
-Requires-Dist: polyfactory; python_version > '3.7' and extra == 'doc'
+Requires-Dist: polyfactory>=2.3.0; python_version > '3.7' and extra == 'doc'
 Requires-Dist: pydantic[email]; extra == 'doc'
 Requires-Dist: pyyaml; extra == 'doc'
 Requires-Dist: uvicorn; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
-Requires-Dist: fastapi; extra == 'test'
+Requires-Dist: fastapi==0.100.0b1; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: propan[async-sqs]; extra == 'test'
 Requires-Dist: propan[doc]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
```

