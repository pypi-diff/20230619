# Comparing `tmp/propan-0.1.3.5.tar.gz` & `tmp/propan-0.1.3.6.tar.gz`

## Comparing `propan-0.1.3.5.tar` & `propan-0.1.3.6.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.5/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/grpc/gen_py_code.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/grpc/grpc_encoding.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/grpc/message.proto
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/grpc/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.5/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/__about__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/__main__.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/security.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    15906 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/app.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/redis.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/classes.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.5/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.5/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.5/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.5/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.5/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.5/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.5/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.5/README.md
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 propan-0.1.3.5/pyproject.toml
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 propan-0.1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.6/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/grpc/gen_py_code.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/grpc/grpc_encoding.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/grpc/message.proto
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/grpc/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.6/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/__about__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/__main__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    15906 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/app.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/redis.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/classes.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.6/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.6/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.6/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.6/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.6/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.6/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.6/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.6/README.md
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 propan-0.1.3.6/pyproject.toml
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 propan-0.1.3.6/PKG-INFO
```

### Comparing `propan-0.1.3.5/CONTRIBUTING.md` & `propan-0.1.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/SECURITY.md` & `propan-0.1.3.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.3.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.3.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.3.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/workflows/documentation.yml` & `propan-0.1.3.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/workflows/publish_coverage.yml` & `propan-0.1.3.6/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/workflows/publish_pypi.yml` & `propan-0.1.3.6/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/.github/workflows/tests.yml` & `propan-0.1.3.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/3_lifespan_events.py` & `propan-0.1.3.6/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/4_cli_attributes_promotion.py` & `propan-0.1.3.6/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/5_publishing.py` & `propan-0.1.3.6/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/6_arguments_casting.py` & `propan-0.1.3.6/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/7_handler_errors_processing.py` & `propan-0.1.3.6/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/1_dependency_injection.py` & `propan-0.1.3.6/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.3.6/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.3.6/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.3.6/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.3.6/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/dependencies/7_annotated.py` & `propan-0.1.3.6/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/grpc/grpc_encoding.py` & `propan-0.1.3.6/examples/grpc/grpc_encoding.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/quart.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.3.6/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/rabbit/direct.py` & `propan-0.1.3.6/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/rabbit/fanout.py` & `propan-0.1.3.6/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/rabbit/header.py` & `propan-0.1.3.6/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/rabbit/topic.py` & `propan-0.1.3.6/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/redis/direct.py` & `propan-0.1.3.6/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/examples/redis/pattern.py` & `propan-0.1.3.6/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/__about__.py` & `propan-0.1.3.6/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.3.5"
+__version__ = "0.1.3.6"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.3.5/propan/__init__.py` & `propan-0.1.3.6/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/annotations.py` & `propan-0.1.3.6/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/types.py` & `propan-0.1.3.6/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/__init__.py` & `propan-0.1.3.6/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/channels.py` & `propan-0.1.3.6/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/info.py` & `propan-0.1.3.6/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/main.py` & `propan-0.1.3.6/propan/asyncapi/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseModel, Field
 
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.info import AsyncAPIInfo
 from propan.asyncapi.message import AsyncAPIMessage
 from propan.asyncapi.servers import AsyncAPIServer
 from propan.asyncapi.utils import AsyncAPIExternalDocs, AsyncAPITag
-from propan.brokers._model.schemas import ContentTypes
+from propan.brokers._model import ContentTypes
 from propan.types import AnyDict
 
 ASYNC_API_VERSION = "2.6.0"
 
 
 class AsyncAPIComponents(BaseModel):
     # TODO
```

### Comparing `propan-0.1.3.5/propan/asyncapi/message.py` & `propan-0.1.3.6/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/security.py` & `propan-0.1.3.6/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/servers.py` & `propan-0.1.3.6/propan/asyncapi/servers.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/subscription.py` & `propan-0.1.3.6/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/utils.py` & `propan-0.1.3.6/propan/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/amqp.py` & `propan-0.1.3.6/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/kafka.py` & `propan-0.1.3.6/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/main.py` & `propan-0.1.3.6/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/nats.py` & `propan-0.1.3.6/propan/asyncapi/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/redis.py` & `propan-0.1.3.6/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/asyncapi/bindings/sqs.py` & `propan-0.1.3.6/propan/asyncapi/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/push_back_watcher.py` & `propan-0.1.3.6/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/_model/broker_usecase.py` & `propan-0.1.3.6/propan/brokers/_model/broker_usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,26 +20,23 @@
 )
 
 from fast_depends.construct import get_dependant
 from fast_depends.model import Dependant, Depends
 from fast_depends.utils import args_to_kwargs
 from typing_extensions import Self, TypeAlias
 
-from propan.brokers._model.schemas import (
-    BaseHandler,
+from propan.brokers._model.schemas import BaseHandler, PropanMessage
+from propan.brokers._model.utils import (
     ContentType,
     ContentTypes,
-    PropanMessage,
-    SendableModel,
-)
-from propan.brokers._model.utils import (
     change_logger_handlers,
     get_watcher,
     set_message_context,
     suppress_decor,
+    to_send,
 )
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import AnyDict, DecodedMessage, HandlerWrapper, SendableMessage
 from propan.utils import apply_types, context
 from propan.utils.functions import get_function_positional_arguments, to_async
@@ -193,15 +190,15 @@
                 m = body.decode()
             elif ContentTypes.json.value in message.content_type:  # pragma: no branch
                 m = json.loads(body.decode())
         return m
 
     @staticmethod
     def _encode_message(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
-        return SendableModel.to_send(msg)
+        return to_send(msg)
 
     @property
     def fmt(self) -> str:  # pragma: no cover
         return self._fmt or ""
 
     async def start(self) -> None:
         if self.logger is not None:
```

### Comparing `propan-0.1.3.5/propan/brokers/_model/schemas.py` & `propan-0.1.3.6/propan/brokers/_model/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-import json
 from abc import abstractmethod
 from dataclasses import dataclass
-from enum import Enum
 from inspect import _empty
-from typing import Any, Dict, Generic, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Any, Dict, Generic, Optional, Tuple, TypeVar, Union
 from uuid import uuid4
 
 from fast_depends.model import Dependant
 from pydantic import BaseModel, Field, Json, create_model
 from pydantic.dataclasses import dataclass as pydantic_dataclass
-from typing_extensions import TypeAlias, assert_never
 
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.utils import add_example_to_model
-from propan.types import AnyDict, DecodedMessage, DecoratedCallable, SendableMessage
-
-ContentType: TypeAlias = str
-
-Msg = TypeVar("Msg")
+from propan.types import AnyDict, DecodedMessage, DecoratedCallable
 
 
 @dataclass
 class BaseHandler:
     callback: DecoratedCallable
     dependant: Dependant
     _description: str
@@ -156,59 +149,35 @@
             )
             param_body["example"] = body.get("example", {}).get(key)
             body = param_body
 
         return f"{self.title}Message", body, return_info
 
 
-class ContentTypes(str, Enum):
-    text = "text/plain"
-    json = "application/json"
-
-
 class NameRequired(BaseModel):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
 
 class Queue(NameRequired):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
 
-class SendableModel(BaseModel):
-    message: DecodedMessage
-
-    @classmethod
-    def to_send(cls, msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
-        if msg is None:
-            return b"", None
-
-        if isinstance(msg, bytes):
-            return msg, None
-
-        m = cls(message=msg).message  # type: ignore
-
-        if isinstance(m, str):
-            return m.encode(), ContentTypes.text.value
-
-        if isinstance(m, (Dict, Sequence)):
-            return json.dumps(m).encode(), ContentTypes.json.value
-
-        assert_never()  # pragma: no cover
-
-
 class RawDecoced(BaseModel):
     message: Union[Json[Any], str]
 
 
+Msg = TypeVar("Msg")
+
+
 @pydantic_dataclass
 class PropanMessage(Generic[Msg]):
     body: Union[bytes, Any]
     raw_message: Msg
     content_type: Optional[str] = None
     reply_to: str = ""
     headers: AnyDict = Field(default_factory=dict)
```

### Comparing `propan-0.1.3.5/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.3.6/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.3.6/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/kafka/schemas.py` & `propan-0.1.3.6/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/nats/nats_broker.py` & `propan-0.1.3.6/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.3.6/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.3.6/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/nats/schemas.py` & `propan-0.1.3.6/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.3.6/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.3.6/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/rabbit/schemas.py` & `propan-0.1.3.6/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/redis/redis_broker.py` & `propan-0.1.3.6/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.3.6/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/redis/schemas.py` & `propan-0.1.3.6/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/sqs/schema.py` & `propan-0.1.3.6/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.3.6/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.3.6/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/app.py` & `propan-0.1.3.6/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/main.py` & `propan-0.1.3.6/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/docs/app.py` & `propan-0.1.3.6/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/docs/gen.py` & `propan-0.1.3.6/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/docs/serving.py` & `propan-0.1.3.6/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/core.py` & `propan-0.1.3.6/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/app.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/core.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/nats.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/redis.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.3.6/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/supervisors/basereload.py` & `propan-0.1.3.6/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/supervisors/multiprocess.py` & `propan-0.1.3.6/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/supervisors/utils.py` & `propan-0.1.3.6/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/supervisors/watchfiles.py` & `propan-0.1.3.6/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/utils/imports.py` & `propan-0.1.3.6/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/utils/logs.py` & `propan-0.1.3.6/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/cli/utils/parser.py` & `propan-0.1.3.6/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/__init__.py` & `propan-0.1.3.6/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/core/route.py` & `propan-0.1.3.6/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/core/router.py` & `propan-0.1.3.6/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/kafka/router.pyi` & `propan-0.1.3.6/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/nats/router.pyi` & `propan-0.1.3.6/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/rabbit/router.pyi` & `propan-0.1.3.6/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/redis/router.pyi` & `propan-0.1.3.6/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/fastapi/sqs/router.pyi` & `propan-0.1.3.6/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/log/formatter.py` & `propan-0.1.3.6/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/log/logging.py` & `propan-0.1.3.6/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/__init__.py` & `propan-0.1.3.6/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/kafka.py` & `propan-0.1.3.6/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/nats.py` & `propan-0.1.3.6/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/rabbit.py` & `propan-0.1.3.6/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/redis.py` & `propan-0.1.3.6/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/sqs.py` & `propan-0.1.3.6/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/test/utils.py` & `propan-0.1.3.6/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/utils/functions.py` & `propan-0.1.3.6/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/utils/context/main.py` & `propan-0.1.3.6/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/propan/utils/context/types.py` & `propan-0.1.3.6/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/LICENSE` & `propan-0.1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/README.md` & `propan-0.1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/pyproject.toml` & `propan-0.1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.5/PKG-INFO` & `propan-0.1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.3.5
+Version: 0.1.3.6
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

