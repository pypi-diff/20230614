# Comparing `tmp/propan-0.1.2.9.tar.gz` & `tmp/propan-0.1.3.0.tar.gz`

## Comparing `propan-0.1.2.9.tar` & `propan-0.1.3.0.tar`

### file list

```diff
@@ -1,146 +1,170 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.9/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.9/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.9/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__about__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/__main__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/app.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.9/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.9/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.2.9/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.9/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.9/README.md
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 propan-0.1.2.9/pyproject.toml
--rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 propan-0.1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.0/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/grpc/gen_py_code.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/grpc/grpc_encoding.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/grpc/message.proto
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/grpc/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.0/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/__about__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/__main__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/app.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/redis.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.3.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.0/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.0/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.0/README.md
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 propan-0.1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 propan-0.1.3.0/PKG-INFO
```

### Comparing `propan-0.1.2.9/CONTRIBUTING.md` & `propan-0.1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/SECURITY.md` & `propan-0.1.3.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.3.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/workflows/documentation.yml` & `propan-0.1.3.0/.github/workflows/documentation.yml`

 * *Files 17% similar despite different names*

```diff
@@ -19,10 +19,10 @@
       - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
-      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-macros-plugin
+      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-macros-plugin mkdocs-glightbox
       - working-directory: ./docs
         run: mkdocs gh-deploy --force
```

### Comparing `propan-0.1.2.9/.github/workflows/publish_coverage.yml` & `propan-0.1.3.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/workflows/publish_pypi.yml` & `propan-0.1.3.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/.github/workflows/tests.yml` & `propan-0.1.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/3_lifespan_events.py` & `propan-0.1.3.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/4_cli_attributes_promotion.py` & `propan-0.1.3.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/5_publishing.py` & `propan-0.1.3.0/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/6_arguments_casting.py` & `propan-0.1.3.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/7_handler_errors_processing.py` & `propan-0.1.3.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/1_dependency_injection.py` & `propan-0.1.3.0/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.3.0/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.3.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.3.0/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.3.0/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/dependencies/7_annotated.py` & `propan-0.1.3.0/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/quart.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.3.0/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/rabbit/direct.py` & `propan-0.1.3.0/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/rabbit/fanout.py` & `propan-0.1.3.0/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/rabbit/header.py` & `propan-0.1.3.0/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/rabbit/topic.py` & `propan-0.1.3.0/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/redis/direct.py` & `propan-0.1.3.0/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/examples/redis/pattern.py` & `propan-0.1.3.0/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/__about__.py` & `propan-0.1.3.0/propan/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.2.9"
+__version__ = "0.1.3.0"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.2.9/propan/__init__.py` & `propan-0.1.3.0/propan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
     "access_logger",
     # utils
     ## types
     "apply_types",
     ## context
     "context",
     "Context",
-    "ContextRepo" "Alias",
+    "ContextRepo",
     "Depends",
     # brokers
+    "PropanMessage",
     "NatsBroker",
     "RabbitBroker",
     "RedisBroker",
     "KafkaBroker",
     "SQSBroker",
 )
```

### Comparing `propan-0.1.2.9/propan/annotations.py` & `propan-0.1.3.0/propan/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import logging
 
-from typing_extensions import Annotated
+from typing_extensions import Annotated, TypeVar
 
 from propan import __about__ as about
 from propan.cli.app import PropanApp
 from propan.utils.context import Context as ContextField
 from propan.utils.context import ContextRepo as CR
+from propan.utils.no_cast import NoCast as NC
 
 Logger = Annotated[logging.Logger, ContextField("logger")]
 App = Annotated[PropanApp, ContextField("app")]
 ContextRepo = Annotated[CR, ContextField("context")]
 
+NoCastType = TypeVar("NoCastType")
+NoCast = Annotated[NoCastType, NC()]
 
 try:
     import aio_pika
 
     from propan.brokers.rabbit import RabbitBroker as RB
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
     RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
     Channel = Annotated[
-        aio_pika.robust_channel.RobustChannel, ContextField("broker._channel")
+        aio_pika.robust_channel.RobustChannel, ContextField("broker.channel")
     ]
 except Exception:
     RabbitBroker = RabbitMessage = Channel = about.INSTALL_RABBIT
 
 
 try:
     from nats.aio.msg import Msg
@@ -54,15 +57,15 @@
 
     from propan.brokers.kafka import KafkaBroker as KB
 
     KafkaBroker = Annotated[KB, ContextField("broker")]
     KafkaMessage = Annotated[ConsumerRecord, ContextField("message")]
     Producer = Annotated[AIOKafkaProducer, ContextField("producer")]
 except Exception:
-    KafkaBroker = KafkaMessage = about.INSTALL_KAFKA
+    KafkaBroker = KafkaMessage = Producer = about.INSTALL_KAFKA
 
 
 try:
     from aiobotocore.client import AioBaseClient
 
     from propan.brokers.sqs import SQSBroker as SB
```

### Comparing `propan-0.1.2.9/propan/types.py` & `propan-0.1.3.0/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/brokers/push_back_watcher.py` & `propan-0.1.3.0/propan/brokers/push_back_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         if not exc_type:
             await call_or_await(self.on_success)
             self.watcher.remove(self._message_id)
 
-        elif isinstance(exc_val, SkipMessage) is True:
+        elif isinstance(exc_val, SkipMessage):
             self.watcher.remove(self._message_id)
 
         elif self.watcher.is_max(self._message_id):
             await call_or_await(self.on_max)
             self.watcher.remove(self._message_id)
 
         else:
```

### Comparing `propan-0.1.2.9/propan/brokers/_model/broker_usecase.py` & `propan-0.1.3.0/propan/brokers/redis/redis_broker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,286 +1,293 @@
-import json
+import asyncio
 import logging
-from abc import ABC, abstractmethod
 from functools import wraps
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
-    Mapping,
+    NoReturn,
     Optional,
     Sequence,
-    Tuple,
     TypeVar,
-    Union,
 )
+from uuid import uuid4
 
-from fast_depends.construct import get_dependant
-from fast_depends.model import Dependant
-from pydantic.fields import ModelField
-from typing_extensions import Self
-
-from propan.brokers._model.schemas import (
-    ContentType,
-    ContentTypes,
-    PropanMessage,
-    SendableModel,
-)
-from propan.brokers._model.utils import (
-    change_logger_handlers,
-    get_watcher,
-    set_message_context,
-    suppress_decor,
-)
-from propan.brokers.exceptions import SkipMessage
+from fast_depends.model import Depends
+from redis.asyncio.client import PubSub, Redis
+from redis.asyncio.connection import ConnectionPool, parse_url
+from typing_extensions import TypeAlias
+
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage, RawDecoced
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.log import access_logger
+from propan.brokers.redis.schemas import Handler
+from propan.brokers.redis.schemas import RedisMessage as RM
 from propan.types import (
     AnyCallable,
     AnyDict,
     DecodedMessage,
-    DecoratedAsync,
+    DecoratedCallable,
     HandlerWrapper,
     SendableMessage,
-    Wrapper,
 )
-from propan.utils import apply_types, context
-from propan.utils.functions import to_async
+from propan.utils import context
 
 T = TypeVar("T")
+RedisMessage: TypeAlias = PropanMessage[AnyDict]
 
 
-class BrokerUsecase(ABC):
-    logger: Optional[logging.Logger]
-    log_level: int
-    handlers: List[Any]
-    _connection: Any
-    _fmt: Optional[str]
+class RedisBroker(BrokerUsecase):
+    handlers: List[Handler]
+    _connection: Redis
+    __max_channel_len: int
+    _polling_interval: float
 
     def __init__(
         self,
-        *args: Any,
-        apply_types: bool = True,
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = "%(asctime)s %(levelname)s - %(message)s",
+        url: str = "redis://localhost:6379",
+        *,
+        polling_interval: float = 1.0,
+        log_fmt: Optional[str] = None,
+        protocol: str = "redis",
         **kwargs: Any,
     ) -> None:
-        self.logger = logger
-        self.log_level = log_level
-        self._fmt = log_fmt
-
-        self._connection = None
-        self._is_apply_types = apply_types
-        self.handlers = []
-
-        self._connection_args = args
-        self._connection_kwargs = kwargs
-
-        context.set_global("logger", logger)
-        context.set_global("broker", self)
-
-    async def connect(self, *args: Any, **kwargs: Any) -> Any:
-        if self._connection is None:
-            _args = args or self._connection_args
-            _kwargs = kwargs or self._connection_kwargs
-            self._connection = await self._connect(*_args, **_kwargs)
-        return self._connection
-
-    @abstractmethod
-    async def _connect(self, *args: Any, **kwargs: Any) -> Any:
-        raise NotImplementedError()
+        super().__init__(
+            url,
+            log_fmt=log_fmt,
+            url_=url,
+            protocol=protocol,
+            **kwargs,
+        )
+        self.__max_channel_len = 0
+        self._polling_interval = polling_interval
 
-    @abstractmethod
-    async def publish(
+    async def _connect(
         self,
-        message: SendableMessage,
-        *args: Any,
-        reply_to: str = "",
-        callback: bool = False,
-        callback_timeout: Optional[float] = None,
-        raise_timeout: bool = False,
+        url: str,
         **kwargs: Any,
-    ) -> Optional[DecodedMessage]:
-        raise NotImplementedError()
+    ) -> Redis:
+        url_options = parse_url(url)
+        url_options.update(kwargs)
+        pool = ConnectionPool(**url_options)
+        return Redis(connection_pool=pool)
 
-    @abstractmethod
     async def close(self) -> None:
-        raise NotImplementedError()
-
-    @abstractmethod
-    async def _parse_message(self, message: Any) -> PropanMessage:
-        raise NotImplementedError()
+        for h in self.handlers:
+            if h.task is not None:  # pragma: no branch
+                h.task.cancel()
+                h.task = None
+
+            if h.subscription is not None:  # pragma: no branch
+                await h.subscription.unsubscribe()
+                await h.subscription.reset()
+                h.subscription = None
+
+        if self._connection is not None:  # pragma: no branch
+            await self._connection.close()
+            self._connection = None
 
-    @abstractmethod
     def _process_message(
         self,
-        func: Callable[[PropanMessage], T],
+        func: Callable[[RedisMessage], Awaitable[T]],
         watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]:
-        raise NotImplementedError()
+    ) -> Callable[[RedisMessage], Awaitable[T]]:
+        @wraps(func)
+        async def wrapper(message: RedisMessage) -> T:
+            r = await func(message)
 
-    def _get_log_context(
-        self,
-        message: Optional[PropanMessage],
-        **kwargs: Dict[str, str],
-    ) -> Dict[str, Any]:
-        return {
-            "message_id": message.message_id[:10] if message else "",
-        }
+            msg = message.raw_message
+            if isinstance(msg, RM) and message.reply_to:
+                await self.publish(r or "", message.reply_to)
+
+            return r
+
+        return wrapper
 
-    @abstractmethod
     def handle(
         self,
-        *broker_args: Any,
-        retry: Union[bool, int] = False,
-        _raw: bool = False,
-        **broker_kwargs: Any,
+        channel: str = "",
+        *,
+        pattern: bool = False,
+        dependencies: Sequence[Depends] = (),
+        description: str = "",
+        **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
-        raise NotImplementedError()
+        self.__max_channel_len = max(self.__max_channel_len, len(channel))
 
-    @staticmethod
-    async def _decode_message(message: PropanMessage) -> DecodedMessage:
-        body = message.body
-        m: DecodedMessage = body
-        if message.content_type is not None:
-            if ContentTypes.text.value in message.content_type:
-                m = body.decode()
-            elif ContentTypes.json.value in message.content_type:  # pragma: no branch
-                m = json.loads(body.decode())
-        return m
+        def wrapper(func: AnyCallable) -> DecoratedCallable:
+            func, dependant = self._wrap_handler(
+                func,
+                channel=channel,
+                extra_dependencies=dependencies,
+                **original_kwargs,
+            )
+            handler = Handler(
+                callback=func,
+                channel=channel,
+                pattern=pattern,
+                _description=description,
+                dependant=dependant,
+            )
+            self.handlers.append(handler)
 
-    @staticmethod
-    def _encode_message(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
-        return SendableModel.to_send(msg)
+            return func
 
-    @property
-    def fmt(self) -> str:  # pragma: no cover
-        return self._fmt or ""
+        return wrapper
 
     async def start(self) -> None:
-        if self.logger is not None:
-            change_logger_handlers(self.logger, self.fmt)
-
-        await self.connect()
-
-    async def __aenter__(self) -> Self:
-        await self.connect()
-        return self
-
-    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
-        await self.close()
-
-    def _wrap_handler(
-        self,
-        func: AnyCallable,
-        retry: Union[bool, int] = False,
-        _raw: bool = False,
-        **broker_args: Any,
-    ) -> DecoratedAsync:
-        dependant: Dependant = get_dependant(path="", call=func)
-
-        f = to_async(func)
-
-        if self._is_apply_types is True:
-            f = apply_types(f)
-
-        f = self._wrap_decode_message(
-            f,
-            _raw=_raw,
-            params=dependant.real_params,
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, ""),
         )
 
-        if self.logger is not None:
-            f = self._log_execution(**broker_args)(f)
-
-        f = self._process_message(f, get_watcher(self.logger, retry))
+        await super().start()
 
-        f = self._wrap_parse_message(f)
+        for handler in self.handlers:  # pragma: no branch
+            c = self._get_log_context(None, handler.channel)
+            self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
+
+            psub = self._connection.pubsub()
+            if handler.pattern is True:
+                await psub.psubscribe(handler.channel)
+            else:
+                await psub.subscribe(handler.channel)
 
-        f = set_message_context(f)
+            handler.subscription = psub
+            handler.task = asyncio.create_task(self._consume(handler, psub))
 
-        f = suppress_decor(f)
+    async def publish(
+        self,
+        message: SendableMessage = "",
+        channel: str = "",
+        *,
+        reply_to: str = "",
+        headers: Optional[Dict[str, Any]] = None,
+        callback: bool = False,
+        callback_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
+    ) -> Optional[DecodedMessage]:
+        if self._connection is None:
+            raise ValueError("Redis connection not established yet")
 
-        return f
+        msg, content_type = self._encode_message(message)
 
-    def _wrap_decode_message(
-        self,
-        func: Callable[..., Awaitable[T]],
-        params: Sequence[ModelField] = (),
-        _raw: bool = False,
-    ) -> Callable[[PropanMessage], Awaitable[T]]:
-        decode: Callable[
-            [PropanMessage], Awaitable[Union[PropanMessage, DecodedMessage]]
-        ]
-        if _raw is True:
-            decode = _fake_decode
+        if callback is True:
+            callback_channel = str(uuid4())
+            psub = self._connection.pubsub()
+            response_queue = asyncio.Queue(maxsize=1)
+            await psub.subscribe(callback_channel)
+            task = asyncio.create_task(_consume_one(response_queue, psub))
         else:
-            decode = self._decode_message
-
-        is_unwrap = len(params) > 1
+            callback_channel = reply_to
+            psub = None
+            response_queue = None
+            task = None
+
+        await self._connection.publish(
+            channel,
+            RM(
+                data=msg,
+                headers={
+                    "content-type": content_type or "",
+                    **(headers or {}),
+                },
+                reply_to=callback_channel,
+            ).json(),
+        )
 
-        @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
-            msg = await decode(message)
-            if is_unwrap is True and isinstance(msg, Mapping):
-                return await func(**msg)
+        if psub and response_queue and task:
+            try:
+                response = await asyncio.wait_for(
+                    response_queue.get(), callback_timeout
+                )
+            except asyncio.TimeoutError as e:
+                if raise_timeout is True:
+                    raise e
+                return None
             else:
-                return await func(msg)
-
-        return wrapper
+                return await self._decode_message(await self._parse_message(response))
+            finally:
+                await psub.unsubscribe(callback_channel)
+                await psub.reset()
+                task.cancel()
 
-    def _wrap_parse_message(
-        self, func: Callable[[PropanMessage], Awaitable[T]]
-    ) -> Callable[[Any], Awaitable[T]]:
-        @wraps(func)
-        async def parse_wrapper(message: Any) -> T:
-            return await func(await self._parse_message(message))
+    @staticmethod
+    async def _parse_message(message: AnyCallable) -> RedisMessage:
+        data = message.get("data", b"")
 
-        return parse_wrapper
+        try:
+            obj = RM.parse_raw(data)
+        except Exception:
+            msg = RedisMessage(
+                body=data,
+                raw_message=message,
+            )
+        else:
+            msg = RedisMessage(
+                body=obj.data,
+                content_type=obj.headers.get("content-type", ""),
+                reply_to=obj.reply_to,
+                headers=obj.headers,
+                raw_message=obj,
+            )
 
-    def _log_execution(
-        self,
-        **broker_args: Any,
-    ) -> Wrapper:
-        def decor(
-            func: Callable[[PropanMessage], Awaitable[T]]
-        ) -> Callable[[PropanMessage], Awaitable[T]]:
-            @wraps(func)
-            async def log_wrapper(message: PropanMessage) -> T:
-                log_context = self._get_log_context(message=message, **broker_args)
-
-                with context.scope("log_context", log_context):
-                    self._log("Received", extra=log_context)
-
-                    try:
-                        r = await func(message)
-                    except SkipMessage as e:
-                        self._log("Skipped", extra=log_context)
-                        raise e
-                    except Exception as e:
-                        self._log(repr(e), logging.ERROR)
-                        raise e
-                    else:
-                        self._log("Processed", extra=log_context)
-                        return r
+        return msg
 
-            return log_wrapper
+    async def _decode_message(self, message: RedisMessage) -> DecodedMessage:
+        if message.headers.get("content-type") is not None:
+            return await super()._decode_message(message)
+        else:
+            return RawDecoced(message=message.body).message
 
-        return decor
+    def _get_log_context(
+        self, message: Optional[RedisMessage], channel: str
+    ) -> Dict[str, Any]:
+        context = {
+            "channel": channel,
+            **super()._get_log_context(message),
+        }
+        return context
 
-    def _log(
-        self,
-        message: str,
-        log_level: Optional[int] = None,
-        extra: Optional[AnyDict] = None,
-    ) -> None:
-        if self.logger is not None:
-            self.logger.log(
-                level=(log_level or self.log_level), msg=message, extra=extra
-            )
+    @property
+    def fmt(self) -> str:
+        return self._fmt or (
+            "%(asctime)s %(levelname)s - "
+            f"%(channel)-{self.__max_channel_len}s | "
+            "%(message_id)-10s "
+            "- %(message)s"
+        )
 
+    async def _consume(self, handler: Handler, psub: PubSub) -> NoReturn:
+        c = self._get_log_context(None, handler.channel)
 
-async def _fake_decode(message: PropanMessage) -> PropanMessage:
-    return message
+        connected = True
+        while True:
+            try:
+                m = await psub.get_message(
+                    ignore_subscribe_messages=True,
+                    timeout=self._polling_interval,
+                )
+            except Exception:
+                if connected is True:
+                    self._log("Connection broken", logging.WARNING, c)
+                    connected = False
+                await asyncio.sleep(5)
+            else:
+                if connected is False:
+                    self._log("Connection established", logging.INFO, c)
+                    connected = True
+
+                if m:  # pragma: no branch
+                    await handler.callback(m)
+            finally:
+                await asyncio.sleep(0.01)
+
+
+async def _consume_one(queue: asyncio.Queue, psub: PubSub) -> NoReturn:
+    async for m in psub.listen():
+        t = m.get("type")
+        if t and "message" in t:  # pragma: no branch
+            await queue.put(m)
+            break
```

### Comparing `propan-0.1.2.9/propan/brokers/_model/utils.py` & `propan-0.1.3.0/propan/brokers/_model/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from functools import wraps
-from typing import Any, Awaitable, Callable, Optional, TypeVar, Union
+from typing import Awaitable, Callable, Optional, TypeVar, Union
 
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.utils import context
@@ -36,30 +36,30 @@
         watcher = None
     else:
         watcher = PushBackWatcher(logger=logger, max_tries=try_number)
     return watcher
 
 
 def suppress_decor(
-    func: Callable[[Any], Awaitable[T]]
-) -> Callable[[Any, bool], Awaitable[Optional[T]]]:
+    func: Callable[[T], Awaitable[P]]
+) -> Callable[[T, bool], Awaitable[Optional[P]]]:
     @wraps(func)
-    async def wrapper(message: Any, reraise_exc: bool = False) -> Optional[T]:
+    async def wrapper(message: T, reraise_exc: bool = False) -> Optional[P]:
         try:
             return await func(message)
         except Exception as e:
             if reraise_exc is True:
                 raise e
             return None
 
     return wrapper
 
 
 def set_message_context(
-    func: Callable[[Any], Awaitable[T]]
-) -> Callable[[Any], Awaitable[T]]:
+    func: Callable[[T], Awaitable[P]]
+) -> Callable[[T], Awaitable[P]]:
     @wraps(func)
-    async def wrapper(message: Any) -> T:
+    async def wrapper(message: T) -> P:
         with context.scope("message", message):
             return await func(message)
 
     return wrapper
```

### Comparing `propan-0.1.2.9/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.3.0/propan/brokers/kafka/kafka_broker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 import asyncio
 import logging
 from functools import partial, wraps
-from typing import Any, Callable, Dict, List, NoReturn, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    NoReturn,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 from uuid import uuid4
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord
-from typing_extensions import TypeAlias, TypeVar
+from fast_depends.model import Depends
+from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
+from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.kafka.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
@@ -22,45 +36,54 @@
     SendableMessage,
     Wrapper,
 )
 from propan.utils.context import context
 
 T = TypeVar("T")
 CorrelationId: TypeAlias = str
+KafkaMessage: TypeAlias = PropanMessage[ConsumerRecord]
 
 
-class KafkaBroker(BrokerUsecase):
+class KafkaBroker(
+    BrokerUsecase[ConsumerRecord, Callable[[Tuple[str, ...]], AIOKafkaConsumer]]
+):
     _publisher: Optional[AIOKafkaProducer]
-    _connection: Callable[[Tuple[str, ...]], AIOKafkaConsumer]
     __max_topic_len: int
     response_topic: str
     response_callbacks: Dict[CorrelationId, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
         response_topic: str = "",
         log_fmt: Optional[str] = None,
+        protocol: str = "kafka",
+        api_version: str = "auto",
         **kwargs: AnyDict,
     ) -> None:
-        super().__init__(bootstrap_servers, log_fmt=log_fmt, **kwargs)
+        super().__init__(
+            bootstrap_servers,
+            log_fmt=log_fmt,
+            url_=bootstrap_servers,
+            protocol=protocol,
+            protocol_version=api_version,
+            **kwargs,
+        )
         self.__max_topic_len = 4
         self._publisher = None
         self.response_topic = response_topic
         self.response_callbacks = {}
 
     async def _connect(
         self,
-        bootstrap_servers: Union[str, List[str]] = "localhost",
         **kwargs: Any,
     ) -> AIOKafkaConsumer:
         kwargs["client_id"] = kwargs.get("client_id", "propan-" + __version__)
-        kwargs["bootstrap_servers"] = bootstrap_servers
 
         producer = AIOKafkaProducer(**kwargs)
         context.set_global("producer", producer)
         await producer.start()
         self._publisher = producer
         consumer_kwargs = {
             k: v
@@ -104,26 +127,84 @@
         if self._publisher is not None:
             await self._publisher.stop()
             self._publisher = None
 
     def handle(
         self,
         *topics: str,
-        _raw: bool = False,
-        **kwargs: AnyDict,
+        group_id: Optional[str] = None,
+        key_deserializer: Optional[Callable[[bytes], Any]] = None,
+        value_deserializer: Optional[Callable[[bytes], Any]] = None,
+        fetch_max_wait_ms: int = 500,
+        fetch_max_bytes: int = 52428800,
+        fetch_min_bytes: int = 1,
+        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
+        auto_offset_reset: Literal[
+            "latest",
+            "earliest",
+            "none",
+        ] = "latest",
+        enable_auto_commit: bool = True,
+        auto_commit_interval_ms: int = 5000,
+        check_crcs: bool = True,
+        partition_assignment_strategy: Sequence[AbstractPartitionAssignor] = (
+            RoundRobinPartitionAssignor,
+        ),
+        max_poll_interval_ms: int = 300000,
+        rebalance_timeout_ms: Optional[int] = None,
+        session_timeout_ms: int = 10000,
+        heartbeat_interval_ms: int = 3000,
+        consumer_timeout_ms: int = 200,
+        max_poll_records: Optional[int] = None,
+        exclude_internal_topics: bool = True,
+        isolation_level: Literal[
+            "read_uncommitted",
+            "read_committed",
+        ] = "read_uncommitted",
+        ## broker
+        dependencies: Sequence[Depends] = (),
+        description: str = "",
+        **original_kwargs: AnyDict,
     ) -> Wrapper:
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             for t in topics:
                 self.__max_topic_len = max((self.__max_topic_len, len(t)))
 
-            func = self._wrap_handler(func, _raw=_raw)
+            func, dependant = self._wrap_handler(
+                func,
+                extra_dependencies=dependencies,
+                **original_kwargs,
+            )
             handler = Handler(
                 callback=func,
                 topics=topics,
-                consumer_kwargs=kwargs,
+                _description=description,
+                group_id=group_id,
+                consumer_kwargs={
+                    "key_deserializer": key_deserializer,
+                    "value_deserializer": value_deserializer,
+                    "fetch_max_wait_ms": fetch_max_wait_ms,
+                    "fetch_max_bytes": fetch_max_bytes,
+                    "fetch_min_bytes": fetch_min_bytes,
+                    "max_partition_fetch_bytes": max_partition_fetch_bytes,
+                    "auto_offset_reset": auto_offset_reset,
+                    "enable_auto_commit": enable_auto_commit,
+                    "auto_commit_interval_ms": auto_commit_interval_ms,
+                    "check_crcs": check_crcs,
+                    "partition_assignment_strategy": partition_assignment_strategy,
+                    "max_poll_interval_ms": max_poll_interval_ms,
+                    "rebalance_timeout_ms": rebalance_timeout_ms,
+                    "session_timeout_ms": session_timeout_ms,
+                    "heartbeat_interval_ms": heartbeat_interval_ms,
+                    "consumer_timeout_ms": consumer_timeout_ms,
+                    "max_poll_records": max_poll_records,
+                    "exclude_internal_topics": exclude_internal_topics,
+                    "isolation_level": isolation_level,
+                },
+                dependant=dependant,
             )
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
@@ -142,36 +223,42 @@
 
         await super().start()
 
         for handler in self.handlers:  # pragma: no branch
             c = self._get_log_context(None, handler.topics)
             self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
 
-            consumer = self._connection(*handler.topics, **handler.consumer_kwargs)
+            consumer = self._connection(
+                *handler.topics,
+                group_id=handler.group_id,
+                **handler.consumer_kwargs,
+            )
             await consumer.start()
             handler.consumer = consumer
             handler.task = asyncio.create_task(self._consume(handler))
 
     @staticmethod
-    async def _parse_message(message: ConsumerRecord) -> PropanMessage:
+    async def _parse_message(message: ConsumerRecord) -> KafkaMessage:
         headers = {i: j.decode() for i, j in message.headers}
         return PropanMessage(
             body=message.value,
             raw_message=message,
             message_id=f"{message.offset}-{message.timestamp}",
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             headers=headers,
         )
 
     def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
-    ) -> Callable[[PropanMessage], T]:
+        self,
+        func: Callable[[KafkaMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[KafkaMessage], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
+        async def wrapper(message: KafkaMessage) -> T:
             r = await func(message)
 
             if message.reply_to:
                 await self.publish(
                     message=r or "",
                     headers={"correlation_id": message.headers.get("correlation_id")},
                     topic=message.reply_to,
@@ -253,15 +340,15 @@
             f"%(topic)-{self.__max_topic_len}s | "
             "%(message_id)-10s "
             "- %(message)s"
         )
 
     def _get_log_context(
         self,
-        message: Optional[PropanMessage],
+        message: Optional[KafkaMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]:
         if topics:
             topic = ", ".join(topics)
         elif message is not None:
             topic = message.raw_message.topic
         else:
@@ -271,23 +358,33 @@
             "topic": topic,
             **super()._get_log_context(message),
         }
 
     async def _consume(self, handler: Handler) -> NoReturn:
         c = self._get_log_context(None, handler.topics)
 
+        connected = True
         while True:
             try:
                 msg = await handler.consumer.getone()
+
             except Exception as e:
-                self._log(e, logging.WATNING, c)
+                if connected is True:
+                    self._log(e, logging.WATNING, c)
+                    connected = False
+                await asyncio.sleep(5)
+
             else:
+                if connected is False:
+                    self._log("Connection established", logging.INFO, c)
+                    connected = True
+
                 await handler.callback(msg)
 
-    async def _consume_response(self, message: PropanMessage):
+    async def _consume_response(self, message: KafkaMessage):
         correlation_id = message.headers.get("correlation_id")
         if correlation_id is not None:
             callback = self.response_callbacks.pop(correlation_id, None)
             if callback is not None:
                 callback.set_result(await self._decode_message(message))
 
         raise SkipMessage()
```

### Comparing `propan-0.1.2.9/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.3.0/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 import logging
 from asyncio import AbstractEventLoop, Future
 from ssl import SSLContext
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
 from aiokafka.structs import ConsumerRecord
+from fast_depends.model import Depends
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
-from propan.brokers._model.broker_usecase import BrokerUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerUsecase,
+    CustomDecoder,
+    CustomParser,
+)
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.kafka.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
-from propan.types import DecodedMessage, SendableMessage, Wrapper
+from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 Partition = TypeVar("Partition")
 CorrelationId: TypeAlias = str
+KafkaMessage: TypeAlias = PropanMessage[ConsumerRecord]
 
-class KafkaBroker(BrokerUsecase):
+class KafkaBroker(
+    BrokerUsecase[ConsumerRecord, Callable[[Tuple[str, ...]], AIOKafkaConsumer]]
+):
     _publisher: Optional[AIOKafkaProducer]
-    _connection: Callable[[Tuple[str, ...]], AIOKafkaConsumer]
     __max_topic_len: int
     response_topic: str
     response_callbacks: Dict[CorrelationId, "Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
@@ -76,22 +93,26 @@
         ssl_context: Optional[SSLContext] = None,
         enable_idempotence: bool = False,
         transactional_id: Optional[str] = None,
         transaction_timeout_ms: int = 60000,
         loop: Optional[AbstractEventLoop] = None,
         # broker
         logger: Optional[logging.Logger] = access_logger,
+        decode_message: CustomDecoder[ConsumerRecord] = None,
+        parse_message: CustomParser[ConsumerRecord] = None,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        dependencies: Sequence[Depends] = (),
+        protocol: str = "kafka",
     ) -> None: ...
     async def connect(
         self,
-        bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
+        bootstrap_servers: Union[str, List[str]] = "localhost",
         # both
         loop: Optional[AbstractEventLoop] = None,
         client_id: str = "propan-" + __version__,
         request_timeout_ms: int = 40 * 1000,
         retry_backoff_ms: int = 100,
         metadata_max_age_ms: int = 5 * 60 * 1000,
         security_protocol: Literal[
@@ -161,35 +182,40 @@
         max_poll_records: Optional[int] = None,
         exclude_internal_topics: bool = True,
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
         retry: Union[bool, int] = False,
-    ) -> Wrapper: ...
-    async def start(self) -> None: ...
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[ConsumerRecord] = None,
+        parse_message: CustomParser[ConsumerRecord] = None,
+        description: str = "",
+    ) -> HandlerWrapper: ...
     @staticmethod
-    async def _parse_message(message: ConsumerRecord) -> PropanMessage: ...
-    def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
-    ) -> Callable[[PropanMessage], T]: ...
+    async def _parse_message(
+        message: ConsumerRecord,
+    ) -> KafkaMessage: ...
     async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
         topic: str,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         *,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
     ) -> Optional[DecodedMessage]: ...
-    @property
-    def fmt(self) -> str: ...
     def _get_log_context(  # type: ignore[override]
         self,
-        message: Optional[PropanMessage],
+        message: Optional[KafkaMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]: ...
+    def _process_message(
+        self,
+        func: Callable[[KafkaMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[KafkaMessage], Awaitable[T]]: ...
```

### Comparing `propan-0.1.2.9/propan/brokers/nats/nats_broker.py` & `propan-0.1.3.0/propan/brokers/nats/nats_broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,108 @@
 import asyncio
 import logging
 from functools import wraps
 from secrets import token_hex
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
 import nats
+from fast_depends.model import Depends
 from nats.aio.client import Callback, Client, ErrorCallback
 from nats.aio.msg import Msg
+from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.types import AnyDict, DecodedMessage, DecoratedCallable, SendableMessage
 from propan.utils import context
 
 T = TypeVar("T")
+NatsMessage: TypeAlias = PropanMessage[Msg]
 
 
-class NatsBroker(BrokerUsecase):
+class NatsBroker(BrokerUsecase[Msg, Client]):
     handlers: List[Handler]
-    _connection: Optional[Client]
 
     __max_queue_len: int
     __max_subject_len: int
     __is_connected: bool
 
     def __init__(
         self,
-        *args: Any,
+        servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
+        *,
         log_fmt: Optional[str] = None,
+        protocol: str = "nats",
         **kwargs: AnyDict,
-    ):
-        super().__init__(*args, log_fmt=log_fmt, **kwargs)
+    ) -> None:
+        super().__init__(
+            servers, log_fmt=log_fmt, url_=servers, protocol=protocol, **kwargs
+        )
 
         self._connection = None
 
         self.__max_queue_len = 0
         self.__max_subject_len = 4
         self.__is_connected = True
 
     async def _connect(
         self,
-        *args: Any,
+        *,
         url: Optional[str] = None,
         error_cb: Optional[ErrorCallback] = None,
         reconnected_cb: Optional[Callback] = None,
         **kwargs: Any,
     ) -> Client:
         if url is not None:
             kwargs["servers"] = kwargs.pop("servers", []) + [url]
         return await nats.connect(
-            *args,
             error_cb=self.log_connection_broken(error_cb),
             reconnected_cb=self.log_reconnected(reconnected_cb),
             **kwargs,
         )
 
     def handle(
         self,
         subject: str,
         queue: str = "",
         *,
-        retry: Union[bool, int] = False,
-        _raw: bool = False,
+        dependencies: Sequence[Depends] = (),
+        description: str = "",
+        **original_kwargs: AnyDict,
     ) -> Callable[[DecoratedCallable], None]:
         self.__max_subject_len = max((self.__max_subject_len, len(subject)))
         self.__max_queue_len = max((self.__max_queue_len, len(queue)))
 
         def wrapper(func: DecoratedCallable) -> None:
-            func = self._wrap_handler(
+            func, dependant = self._wrap_handler(
                 func,
                 queue=queue,
                 subject=subject,
-                retry=retry,
-                _raw=_raw,
+                extra_dependencies=dependencies,
+                **original_kwargs,
+            )
+            handler = Handler(
+                callback=func,
+                subject=subject,
+                queue=queue,
+                _description=description,
+                dependant=dependant,
             )
-            handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
@@ -93,15 +115,19 @@
 
         for handler in self.handlers:
             func = handler.callback
 
             c = self._get_log_context(None, handler.subject, handler.queue)
             self._log(f"`{func.__name__}` waiting for messages", extra=c)
 
-            sub = await self._connection.subscribe(handler.subject, cb=func)
+            sub = await self._connection.subscribe(
+                subject=handler.subject,
+                queue=handler.queue,
+                cb=func,
+            )
             handler.subscription = sub
 
     async def publish(
         self,
         message: SendableMessage,
         subject: str,
         *,
@@ -164,15 +190,15 @@
 
         if self._connection is not None:
             await self._connection.drain()
             self._connection = None
 
     def _get_log_context(
         self,
-        message: Optional[PropanMessage],
+        message: Optional[NatsMessage],
         subject: str,
         queue: str = "",
     ) -> Dict[str, Any]:
         context = {
             "subject": subject,
             "queue": queue,
             **super()._get_log_context(message),
@@ -185,28 +211,30 @@
             "%(asctime)s %(levelname)s - "
             f"%(subject)-{self.__max_subject_len}s | "
             + (f"%(queue)-{self.__max_queue_len}s | " if self.__max_queue_len else "")
             + "%(message_id)-10s "
             "- %(message)s"
         )
 
-    async def _parse_message(self, message: Msg) -> PropanMessage:
+    async def _parse_message(self, message: Msg) -> NatsMessage:
         return PropanMessage(
             body=message.data,
             content_type=message.header.get("content-type", ""),
             headers=message.header,
             reply_to=message.reply,
             raw_message=message,
         )
 
     def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher] = None
-    ) -> Callable[[PropanMessage], T]:
+        self,
+        func: Callable[[NatsMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher] = None,
+    ) -> Callable[[NatsMessage], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
+        async def wrapper(message: NatsMessage) -> T:
             r = await func(message)
 
             if message.reply_to:
                 await self.publish(r, message.reply_to)
 
             return r
```

### Comparing `propan-0.1.2.9/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.3.0/propan/brokers/nats/nats_broker.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import logging
 import ssl
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
+from fast_depends.model import Depends
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
     DEFAULT_DRAIN_TIMEOUT,
     DEFAULT_INBOX_PREFIX,
     DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
     DEFAULT_MAX_OUTSTANDING_PINGS,
     DEFAULT_MAX_RECONNECT_ATTEMPTS,
@@ -16,32 +27,35 @@
     Client,
     Credentials,
     ErrorCallback,
     JWTCallback,
     SignatureCallback,
 )
 from nats.aio.msg import Msg
+from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
+NatsMessage: TypeAlias = PropanMessage[Msg]
 
-class NatsBroker(BrokerUsecase):
+class NatsBroker(BrokerUsecase[Msg, Client]):
     logger: logging.Logger
     handlers: List[Handler]
-    _connection: Optional[Client]
 
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
+        *,
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
         discovered_server_cb: Optional[Callback] = None,
         reconnected_cb: Optional[Callback] = None,
         name: Optional[str] = None,
         pedantic: bool = False,
@@ -64,22 +78,26 @@
         signature_cb: Optional[SignatureCallback] = None,
         user_jwt_cb: Optional[JWTCallback] = None,
         user_credentials: Optional[Credentials] = None,
         nkeys_seed: Optional[str] = None,
         inbox_prefix: Union[str, bytes] = DEFAULT_INBOX_PREFIX,
         pending_size: int = DEFAULT_PENDING_SIZE,
         flush_timeout: Optional[float] = None,
-        *,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[Msg] = None,
+        parse_message: CustomParser[Msg] = None,
+        protocol: str = "nats",
     ) -> None: ...
     async def connect(
         self,
+        *,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
         discovered_server_cb: Optional[Callback] = None,
         reconnected_cb: Optional[Callback] = None,
         name: Optional[str] = None,
@@ -121,23 +139,33 @@
     ) -> Optional[DecodedMessage]: ...
     def handle(  # type: ignore[override]
         self,
         subject: str,
         queue: str = "",
         *,
         retry: Union[bool, int] = False,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[Msg] = None,
+        parse_message: CustomParser[Msg] = None,
+        description: str = "",
     ) -> HandlerWrapper: ...
-    async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
-    async def close(self) -> None: ...
     def _get_log_context(  # type: ignore[override]
         self,
-        message: Optional[PropanMessage],
+        message: Optional[NatsMessage],
         subject: str,
         queue: str = "",
     ) -> Dict[str, Any]: ...
+    async def _connect(
+        self,
+        *,
+        url: Optional[str] = None,
+        error_cb: Optional[ErrorCallback] = None,
+        reconnected_cb: Optional[Callback] = None,
+        **kwargs: Any,
+    ) -> Client: ...
+    async def close(self) -> None: ...
+    async def _parse_message(self, message: Msg) -> NatsMessage: ...
     def _process_message(
         self,
-        func: Callable[[PropanMessage], T],
-        watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]: ...
-    @staticmethod
-    async def _parse_message(message: Msg) -> PropanMessage: ...
+        func: Callable[[NatsMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher] = None,
+    ) -> Callable[[NatsMessage], Awaitable[T]]: ...
```

### Comparing `propan-0.1.2.9/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.3.0/propan/brokers/nats/nats_js_broker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # TODO: remove mypy ignore at complete
 # type: ignore
 from functools import wraps
-from typing import Any, Optional
+from typing import Any, Awaitable, Callable, Optional, TypeVar
 
 import nats
-from nats.aio.msg import Msg
 from nats.js.client import JetStreamContext
 
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.nats_broker import NatsBroker
 from propan.brokers.nats.schemas import JetStream
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
-from propan.types import AnyDict, DecoratedCallable
+from propan.types import AnyDict
+
+T = TypeVar("T")
 
 
 class NatsJSBroker(NatsBroker):
     _js: Optional[JetStream] = None
     _connection: Optional[JetStreamContext] = None
 
     def __init__(self, *args: Any, jetstream: JetStream, **kwargs: AnyDict):
@@ -30,25 +32,26 @@
             **self._js.dict(include={"prefix", "domain", "timeout"})
         )
 
         return stream
 
     @staticmethod
     def _process_message(
-        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> DecoratedCallable:
+        func: Callable[[PropanMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher] = None,
+    ) -> Callable[[PropanMessage], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: Msg) -> Any:
+        async def wrapper(message: PropanMessage) -> T:
             if watcher is None:
                 return await func(message)
             else:
                 async with WatcherContext(
                     watcher,
                     message.message_id,
-                    on_success=message.ack,
-                    on_error=message.nak,
-                    on_max=message.term,
+                    on_success=message.raw_message.ack,
+                    on_error=message.raw_message.nak,
+                    on_max=message.raw_message.term,
                 ):
                     await message.in_progress()
                     return await func(message)
 
         return wrapper
```

### Comparing `propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.3.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,99 @@
 import asyncio
+import warnings
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 from uuid import uuid4
 
 import aio_pika
 import aiormq
 from aio_pika.abc import DeliveryMode
+from fast_depends.model import Depends
+from typing_extensions import TypeAlias
+from yarl import URL
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, HandlerWrapper, SendableMessage
 from propan.utils import context
 
 TimeoutType = Optional[Union[int, float]]
-PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
+PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
+RabbitMessage: TypeAlias = PropanMessage[aio_pika.message.IncomingMessage]
 T = TypeVar("T")
 
 
 class RabbitBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
+    _queues: Dict[RabbitQueue, aio_pika.RobustQueue]
+    _exchanges: Dict[RabbitExchange, aio_pika.RobustExchange]
 
     __max_queue_len: int
     __max_exchange_len: int
 
     def __init__(
         self,
-        *args: Tuple[Any, ...],
-        consumers: Optional[int] = None,
+        url: Union[str, URL, None] = None,
+        *,
         log_fmt: Optional[str] = None,
+        consumers: Optional[int] = None,
+        protocol: str = "amqp",
+        protocol_version: str = "0.9.1",
         **kwargs: AnyDict,
     ) -> None:
-        super().__init__(*args, log_fmt=log_fmt, **kwargs)
+        super().__init__(
+            url,
+            log_fmt=log_fmt,
+            url_=url or "amqp://guest:guest@localhost:5672/",
+            protocol=protocol,
+            protocol_version=protocol_version,
+            **kwargs,
+        )
         self._max_consumers = consumers
 
         self._channel = None
 
         self.__max_queue_len = 4
         self.__max_exchange_len = 4
+        self._queues = {}
+        self._exchanges = {}
 
     async def close(self) -> None:
         if self._channel is not None:
             await self._channel.close()
             self._channel = None
 
         if self._connection is not None:
             await self._connection.close()
             self._connection = None
 
+        self._queues = {}
+        self._exchanges = {}
+
     async def _connect(
         self,
-        *args: Any,
         **kwargs: Any,
     ) -> aio_pika.RobustConnection:
         connection = await aio_pika.connect_robust(
-            *args, **kwargs, loop=asyncio.get_event_loop()
+            **kwargs, loop=asyncio.get_event_loop()
         )
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             self._channel = await connection.channel()
 
             if max_consumers:
@@ -72,30 +104,37 @@
         return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
-        retry: Union[bool, int] = False,
-        _raw: bool = False,
+        dependencies: Sequence[Depends] = (),
+        description: str = "",
+        **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
-            func = self._wrap_handler(
+            func, dependant = self._wrap_handler(
                 func,
                 queue=queue,
                 exchange=exchange,
-                retry=retry,
-                _raw=_raw,
+                extra_dependencies=dependencies,
+                **original_kwargs,
+            )
+            handler = Handler(
+                callback=func,
+                queue=queue,
+                exchange=exchange,
+                _description=description,
+                dependant=dependant,
             )
-            handler = Handler(callback=func, queue=queue, exchange=exchange)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
@@ -141,15 +180,15 @@
             callback_queue = await self._channel.declare_queue(exclusive=True)
         else:
             callback_queue = None
 
         if exchange is None:
             exchange_obj = self._channel.default_exchange
         else:
-            exchange_obj = await self._init_exchange(exchange)
+            exchange_obj = await self.declare_exchange(exchange)
 
         message = self._validate_message(
             message=message,
             callback_queue=callback_queue,
             persist=persist,
             **message_kwargs,
         )
@@ -175,53 +214,59 @@
             else:
                 return await self._decode_message(msg)
 
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue:
-        queue = await self._init_queue(handler.queue)
+        queue = await self.declare_queue(handler.queue)
         if handler.exchange is not None and handler.exchange.name != "default":
-            exchange = await self._init_exchange(handler.exchange)
+            exchange = await self.declare_exchange(handler.exchange)
             await queue.bind(
                 exchange,
                 routing_key=handler.queue.routing,
                 arguments=handler.queue.bind_arguments,
             )
         return queue
 
-    async def _init_queue(
-        self,
-        queue: RabbitQueue,
-    ) -> aio_pika.abc.AbstractRobustQueue:
-        return await self._channel.declare_queue(**queue.dict())
-
-    async def _init_exchange(
-        self,
-        exchange: RabbitExchange,
-    ) -> aio_pika.abc.AbstractRobustExchange:
-        original = await self._channel.declare_exchange(**exchange.dict())
-
-        current = exchange
-        current_exch = original
-        while current.bind_to is not None:
-            parent_exch = await self._channel.declare_exchange(**current.bind_to.dict())
-            await current_exch.bind(
-                exchange=parent_exch,
-                routing_key=current.routing_key,
-                arguments=current.bind_arguments,
-            )
-            current = current.bind_to
-            current_exch = parent_exch
+    async def declare_queue(self, queue: RabbitQueue) -> aio_pika.RobustQueue:
+        q = self._queues.get(queue)
+        if q is None:
+            q = await self._channel.declare_queue(**queue.dict())
+            self._queues[queue] = q
+        return q
+
+    async def declare_exchange(
+        self, exchange: RabbitExchange
+    ) -> aio_pika.RobustExchange:
+        exch = self._exchanges.get(exchange)
+
+        if exch is None:
+            exch = await self._channel.declare_exchange(**exchange.dict())
+            self._exchanges[exchange] = exch
+
+            current = exchange
+            current_exch = exch
+            while current.bind_to is not None:
+                parent_exch = await self._channel.declare_exchange(
+                    **current.bind_to.dict()
+                )
+                await current_exch.bind(
+                    exchange=parent_exch,
+                    routing_key=current.routing_key,
+                    arguments=current.bind_arguments,
+                )
+                current = current.bind_to
+                current_exch = parent_exch
 
-        return original
+        return exch
 
     def _get_log_context(
         self,
-        message: Optional[PropanMessage],
+        message: Optional[RabbitMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
     ) -> Dict[str, Any]:
         context = {
             "queue": queue.name,
             "exchange": exchange.name if exchange else "default",
             **super()._get_log_context(message),
@@ -237,29 +282,31 @@
             f"%(message_id)-10s "
             "- %(message)s"
         )
 
     @staticmethod
     async def _parse_message(
         message: aio_pika.message.IncomingMessage,
-    ) -> PropanMessage:
-        return PropanMessage(
+    ) -> RabbitMessage:
+        return RabbitMessage(
             body=message.body,
             headers=message.headers,
             reply_to=message.reply_to or "",
             message_id=message.message_id,
             content_type=message.content_type or "",
             raw_message=message,
         )
 
     def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
-    ) -> Callable[[PropanMessage], T]:
+        self,
+        func: Callable[[RabbitMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[RabbitMessage], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
+        async def wrapper(message: RabbitMessage) -> T:
             pika_message = message.raw_message
             if watcher is None:
                 context = pika_message.process()
             else:
                 context = WatcherContext(
                     watcher,
                     message.message_id,
@@ -316,14 +363,69 @@
     ) -> None:
         if exchange is not None:
             self.__max_exchange_len = max(self.__max_exchange_len, len(exchange.name))
 
         if queue is not None:  # pragma: no branch
             self.__max_queue_len = max(self.__max_queue_len, len(queue.name))
 
+    @property
+    def channel(self) -> aio_pika.RobustChannel:
+        return self._channel
+
+    async def _init_queue(
+        self,
+        queue: RabbitQueue,
+    ) -> aio_pika.abc.AbstractRobustQueue:
+        warnings.warn(
+            "The `_init_queue` method is deprecated, "  # noqa: E501
+            "and will be removed in version 1.4.0. "  # noqa: E501
+            "Use `declare_queue` instead.",  # noqa: E501
+            category=DeprecationWarning,
+            stacklevel=1,
+        )
+        q = self._queues.get(queue)
+        if q is None:
+            q = await self._channel.declare_queue(**queue.dict())
+            self._queues[queue] = q
+        return q
+
+    async def _init_exchange(
+        self,
+        exchange: RabbitExchange,
+    ) -> aio_pika.abc.AbstractRobustExchange:
+        warnings.warn(
+            "The `_init_exchange` method is deprecated, "  # noqa: E501
+            "and will be removed in version 1.4.0. "  # noqa: E501
+            "Use `declare_exchange` instead.",  # noqa: E501
+            category=DeprecationWarning,
+            stacklevel=1,
+        )
+
+        exch = self._exchanges.get(exchange)
+
+        if exch is None:
+            exch = await self._channel.declare_exchange(**exchange.dict())
+            self._exchanges[exchange] = exch
+
+            current = exchange
+            current_exch = exch
+            while current.bind_to is not None:
+                parent_exch = await self._channel.declare_exchange(
+                    **current.bind_to.dict()
+                )
+                await current_exch.bind(
+                    exchange=parent_exch,
+                    routing_key=current.routing_key,
+                    arguments=current.bind_arguments,
+                )
+                current = current.bind_to
+                current_exch = parent_exch
+
+        return exch
+
 
 def _validate_exchange(
     exchange: Union[str, RabbitExchange, None] = None,
 ) -> Optional[RabbitExchange]:
     if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
             exchange = RabbitExchange(name=exchange)
```

### Comparing `propan-0.1.2.9/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.3.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,76 @@
 import logging
 from ssl import SSLContext
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Type, TypeVar, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import aio_pika
 import aiormq
+from aio_pika.message import IncomingMessage
+from fast_depends.model import Depends
 from pamqp.common import FieldTable
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, TypeAlias
 from yarl import URL
 
 from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
 from propan.types import DecodedMessage, SendableMessage
 
 P = ParamSpec("P")
 T = TypeVar("T")
-PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
+PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
+RabbitMessage: TypeAlias = PropanMessage[IncomingMessage]
 
-class RabbitBroker(BrokerUsecase):
+class RabbitBroker(BrokerUsecase[IncomingMessage, aio_pika.RobustConnection]):
     handlers: List[Handler]
-    _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
 
     __max_queue_len: int
     __max_exchange_len: int
 
     def __init__(
         self,
         url: Union[str, URL, None] = None,
+        *,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
         virtualhost: str = "/",
         ssl: bool = False,
         ssl_options: Optional[aio_pika.abc.SSLOptions] = None,
         ssl_context: Optional[SSLContext] = None,
         timeout: aio_pika.abc.TimeoutType = None,
         client_properties: Optional[FieldTable] = None,
-        *,
+        # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         consumers: Optional[int] = None,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[IncomingMessage] = None,
+        parse_message: CustomParser[IncomingMessage] = None,
+        # AsyncAPI
+        protocol: str = "amqp",
+        protocol_version: str = "0.9.1",
     ) -> None:
         """RabbitMQ Propan broker
 
         URL string might be contain ssl parameters e.g.
         `amqps://user:pass@host:port/vhost?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
 
         Args:
@@ -66,32 +87,36 @@
             timeout: connection timeout in seconds
             ssl_context: ssl.SSLContext instance
             logger: logger to use inside broker
             log_level: broker inner messages log level
             log_fmt: custom log formatting string
             apply_types: wrap brokers handlers to FastDepends decorator
             consumers: max messages to proccess at the same time
+            dependencies: dependencies applied to all broker hadlers
+            decode_message: custom RabbitMessage decoder
+            parse_message: custom IncomingMessage to RabbitMessage parser
 
         .. _RFC3986: https://goo.gl/MzgYAs
         .. _official Python documentation: https://goo.gl/pty9xA
         """
     async def connect(
         self,
+        *,
         url: Union[str, URL, None] = None,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
         virtualhost: str = "/",
         ssl: bool = False,
         ssl_options: Optional[aio_pika.abc.SSLOptions] = None,
         ssl_context: Optional[SSLContext] = None,
         timeout: aio_pika.abc.TimeoutType = None,
         client_properties: Optional[FieldTable] = None,
-    ) -> aio_pika.Connection:
+    ) -> aio_pika.RobustConnection:
         """Connect to RabbitMQ
 
         URL string might be contain ssl parameters e.g.
         `amqps://user:pass@host:port/vhost?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
 
         Args:
             url: RFC3986_ formatted broker address. If `None`
@@ -180,66 +205,79 @@
         """
     def handle(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         retry: Union[bool, int] = False,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[IncomingMessage] = None,
+        parse_message: CustomParser[IncomingMessage] = None,
+        # AsyncAPI
+        description: str = "",
     ) -> Callable[
         [
-            Callable[
-                P, Union[PikaSendableMessage, Coroutine[Any, Any, PikaSendableMessage]]
+            Union[
+                Callable[P, PikaSendableMessage],
+                Callable[P, Awaitable[PikaSendableMessage]],
             ]
         ],
         Callable[P, PikaSendableMessage],
     ]:
         """Register queue consumer method
 
         Args:
             queue: queue to consume messages
             exchange: exchange to bind queue
             retry: at message exception will returns to queue `int` times or endless if `True`
+            dependencies: wrap handler dependencies
+            decode_message: custom RabbitMessage decoder
+            parse_message: custom IncomingMessage to RabbitMessage parser
+            description: AsyncAPI channel object description
 
         Returns:
             Async or sync function decorator
         """
     async def start(self) -> None:
         """Initialize RabbitMQ connection and startup all consumers"""
     async def close(self) -> None:
         """Close RabbitMQ connection"""
+    async def declare_queue(self, queue: RabbitQueue) -> aio_pika.RobustQueue:
+        """Check existence or create RabbitMQ queue"""
+    async def declare_exchange(
+        self, exchange: RabbitExchange
+    ) -> aio_pika.RobustExchange:
+        """Check existence or create RabbitMQ exchange"""
+    @property
+    def channel(self) -> aio_pika.RobustChannel:
+        """Access to brokers' aio-pika channel object"""
     def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
-    ) -> Callable[[PropanMessage], T]: ...
+        self,
+        func: Callable[[RabbitMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[RabbitMessage], Awaitable[T]]: ...
     def _get_log_context(  # type: ignore[override]
         self,
-        message: Optional[PropanMessage],
+        message: Optional[RabbitMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
     ) -> Dict[str, Any]: ...
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue: ...
-    async def _init_queue(
-        self,
-        queue: RabbitQueue,
-    ) -> aio_pika.abc.AbstractRobustQueue: ...
-    async def _init_exchange(
-        self,
-        exchange: RabbitExchange,
-    ) -> aio_pika.abc.AbstractRobustExchange: ...
     @classmethod
     def _validate_message(
         cls: Type["RabbitBroker"],
         message: PikaSendableMessage,
         callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
         **message_kwargs: Dict[str, Any],
     ) -> aio_pika.Message: ...
     @staticmethod
     async def _parse_message(
-        message: aio_pika.message.IncomingMessage,
-    ) -> PropanMessage: ...
+        message: IncomingMessage,
+    ) -> RabbitMessage: ...
     async def _connect(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> aio_pika.RobustConnection: ...
```

### Comparing `propan-0.1.2.9/propan/brokers/redis/redis_broker.py` & `propan-0.1.3.0/propan/brokers/redis/redis_broker.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,272 +1,201 @@
-import asyncio
 import logging
-from functools import wraps
-from typing import Any, Callable, Coroutine, Dict, List, NoReturn, Optional, TypeVar
-from uuid import uuid4
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 
-from redis.asyncio.client import PubSub, Redis
-from redis.asyncio.connection import ConnectionPool, parse_url
+from fast_depends.model import Depends
+from redis.asyncio.client import Redis
+from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
+from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
-from propan.brokers._model.schemas import PropanMessage, RawDecoced
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.brokers.redis.schemas import Handler, RedisMessage
-from propan.types import (
-    AnyCallable,
-    DecodedMessage,
-    DecoratedCallable,
-    HandlerWrapper,
-    SendableMessage,
-)
-from propan.utils import context
+from propan.brokers.redis.schemas import Handler
+from propan.log import access_logger
+from propan.types import AnyDict, DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
+RedisMessage: TypeAlias = PropanMessage[AnyDict]
 
-
-class RedisBroker(BrokerUsecase):
+class RedisBroker(BrokerUsecase[AnyDict, Redis[bytes]]):
     handlers: List[Handler]
-    _connection: Redis
     __max_channel_len: int
-    _polling_interval: float
 
     def __init__(
         self,
         url: str = "redis://localhost:6379",
-        polling_interval: float = 1.0,
         *,
+        polling_interval: float = 1.0,
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        db: Union[str, int] = 0,
+        client_name: Optional[str] = None,
+        health_check_interval: float = 0,
+        max_connections: Optional[int] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_read_size: int = 65536,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        connection_class: Type[Connection] = Connection,
+        encoder_class: Type[Encoder] = Encoder,
+        # broker kwargs
+        logger: Optional[logging.Logger] = access_logger,
+        log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
-        **kwargs: Any,
+        apply_types: bool = True,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        protocol: str = "redis",
     ) -> None:
-        super().__init__(url=url, log_fmt=log_fmt, **kwargs)
-        self.__max_channel_len = 0
-        self._polling_interval = polling_interval
-
-    async def _connect(
-        self,
-        url: str,
-        **kwargs: Any,
-    ) -> Redis:
-        url_options = parse_url(url)
-        url_options.update(kwargs)
-        pool = ConnectionPool(**url_options)
-        return Redis(connection_pool=pool)
-
-    async def connect(
-        self,
-        url: Optional[str] = None,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Coroutine[Any, Any, Any]:
-        if url is not None:
-            kwargs["url"] = url
-        return await super().connect(*args, **kwargs)
+        """Redis Pub/sub Propan broker
 
-    async def close(self) -> None:
-        for h in self.handlers:
-            if h.task is not None:  # pragma: no branch
-                h.task.cancel()
-                h.task = None
-
-            if h.subscription is not None:  # pragma: no branch
-                await h.subscription.unsubscribe()
-                await h.subscription.reset()
-                h.subscription = None
-
-        if self._connection is not None:  # pragma: no branch
-            await self._connection.close()
-            self._connection = None
+        URL examples:
 
-    def _process_message(
-        self,
-        func: Callable[[PropanMessage], T],
-        watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]:
-        @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
-            r = await func(message)
+        - redis://[[username]:[password]]@localhost:6379/0
+        - rediss://[[username]:[password]]@localhost:6379/0
+        - unix://[username@]/path/to/socket.sock?db=0[&password=password]
 
-            msg = message.raw_message
-            if isinstance(msg, RedisMessage) and message.reply_to:
-                await self.publish(r or "", message.reply_to)
+        Three URL schemes are supported:
 
-            return r
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - `unix://`: creates a Unix Domain Socket connection.
 
-        return wrapper
-
-    def handle(
+        Url will be parsed to kwargs and partially replaced by keywords arguments if they specified.
+        """
+    async def connect(
         self,
-        channel: str = "",
+        *,
+        url: str = "redis://localhost:6379",
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        db: Union[str, int] = 0,
+        client_name: Optional[str] = None,
+        health_check_interval: float = 0,
+        max_connections: Optional[int] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_read_size: int = 65536,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        connection_class: Type[Connection] = Connection,
+        encoder_class: Type[Encoder] = Encoder,
+    ) -> Redis[bytes]:
+        """Connect to Redis
+
+        URL examples:
+
+        - redis://[[username]:[password]]@localhost:6379/0
+        - rediss://[[username]:[password]]@localhost:6379/0
+        - unix://[username@]/path/to/socket.sock?db=0[&password=password]
+
+        Three URL schemes are supported:
+
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - `unix://`: creates a Unix Domain Socket connection.
+
+        Url will be parsed to kwargs and partially replaced by keywords arguments if they specified.
+        """
+    async def _connect(self, *args: Any, **kwargs: Any) -> Redis[bytes]: ...
+    async def start(self) -> None:
+        """Initialize Redis connection and startup all consumers"""
+    async def close(self) -> None:
+        """Cancel all consumers tasks and subscribtions, close Redis connection"""
+    def handle(  # type: ignore[override]
+        self,
+        channel: str,
         *,
         pattern: bool = False,
-        _raw: bool = False,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> HandlerWrapper:
-        self.__max_channel_len = max(self.__max_channel_len, len(channel))
-
-        def wrapper(func: AnyCallable) -> DecoratedCallable:
-            func = self._wrap_handler(
-                func,
-                channel=channel,
-                _raw=_raw,
-            )
-            handler = Handler(callback=func, channel=channel, pattern=pattern)
-            self.handlers.append(handler)
-
-            return func
-
-        return wrapper
-
-    async def start(self) -> None:
-        context.set_local(
-            "log_context",
-            self._get_log_context(None, ""),
-        )
-
-        await super().start()
-
-        for handler in self.handlers:  # pragma: no branch
-            c = self._get_log_context(None, handler.channel)
-            self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
-
-            psub = self._connection.pubsub()
-            if handler.pattern is True:
-                await psub.psubscribe(handler.channel)
-            else:
-                await psub.subscribe(handler.channel)
+        """Register channel consumer method
 
-            handler.subscription = psub
-            handler.task = asyncio.create_task(self._consume(handler, psub))
-
-    async def publish(
+        Args:
+            channel: channel to consume messages
+            pattern: use psubscribe or subscribe method
+            dependencies: wrap handler dependencies
+            decode_message: custom PropanMessage[AnyDict] decoder
+            parse_message: custom redis message to PropanMessage[AnyDict] parser
+            description: AsyncAPI channel object description
+
+        Returns:
+            Async or sync function decorator
+        """
+    async def publish(  # type: ignore[override]
         self,
         message: SendableMessage = "",
         channel: str = "",
         *,
         reply_to: str = "",
         headers: Optional[Dict[str, Any]] = None,
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[DecodedMessage]:
-        if self._connection is None:
-            raise ValueError("Redis connection not established yet")
-
-        msg, content_type = self._encode_message(message)
-
-        if callback is True:
-            callback_channel = str(uuid4())
-            psub = self._connection.pubsub()
-            response_queue = asyncio.Queue(maxsize=1)
-            await psub.subscribe(callback_channel)
-            task = asyncio.create_task(_consume_one(response_queue, psub))
-        else:
-            callback_channel = reply_to
-            psub = None
-            response_queue = None
-            task = None
-
-        await self._connection.publish(
-            channel,
-            RedisMessage(
-                data=msg,
-                headers={
-                    "content-type": content_type or "",
-                    **(headers or {}),
-                },
-                reply_to=callback_channel,
-            ).json(),
-        )
-
-        if psub and response_queue and task:
-            try:
-                response = await asyncio.wait_for(
-                    response_queue.get(), callback_timeout
-                )
-            except asyncio.TimeoutError as e:
-                if raise_timeout is True:
-                    raise e
-                return None
-            else:
-                return await self._decode_message(await self._parse_message(response))
-            finally:
-                await psub.unsubscribe(callback_channel)
-                await psub.reset()
-                task.cancel()
+        """Publish the message to the channel.
 
+        Args:
+            message: encodable message to send
+            channel: channel to publish message
+            reply_to: queue to send response
+            headers: message headers (for consumers)
+            callback: wait for response
+            callback_timeout: response waiting time
+            raise_timeout: if False timeout returns None instead asyncio.TimeoutError
+
+        Returns:
+            `None` if you are not waiting for response
+            (reply_to and callback are not specified)
+
+            `DecodedMessage` | `None` if response is expected
+        """
+    def _get_log_context(  # type: ignore[override]
+        self, message: Optional[RedisMessage], channel: str
+    ) -> Dict[str, Any]: ...
     @staticmethod
-    async def _parse_message(message: Any) -> PropanMessage:
-        data = message.get("data", b"")
-
-        try:
-            obj = RedisMessage.parse_raw(data)
-        except Exception:
-            msg = PropanMessage(
-                body=data,
-                raw_message=message,
-            )
-        else:
-            msg = PropanMessage(
-                body=obj.data,
-                content_type=obj.headers.get("content-type", ""),
-                reply_to=obj.reply_to,
-                headers=obj.headers,
-                raw_message=obj,
-            )
-
-        return msg
-
-    async def _decode_message(self, message: PropanMessage) -> DecodedMessage:
-        if message.headers.get("content-type") is not None:
-            return await super()._decode_message(message)
-        else:
-            return RawDecoced(message=message.body).message
-
-    def _get_log_context(
-        self, message: Optional[PropanMessage], channel: str
-    ) -> Dict[str, Any]:
-        context = {
-            "channel": channel,
-            **super()._get_log_context(message),
-        }
-        return context
-
-    @property
-    def fmt(self) -> str:
-        return self._fmt or (
-            "%(asctime)s %(levelname)s - "
-            f"%(channel)-{self.__max_channel_len}s | "
-            "%(message_id)-10s "
-            "- %(message)s"
-        )
-
-    async def _consume(self, handler: Handler, psub: PubSub) -> NoReturn:
-        c = self._get_log_context(None, handler.channel)
-
-        connected = True
-        while True:
-            try:
-                m = await psub.get_message(
-                    ignore_subscribe_messages=True,
-                    timeout=self._polling_interval,
-                )
-            except Exception:
-                if connected is True:
-                    self._log("Connection broken", logging.WARNING, c)
-                    connected = False
-                await asyncio.sleep(5)
-            else:
-                if connected is False:
-                    self._log("Connection established", logging.INFO, c)
-                    connected = True
-
-                if m:  # pragma: no branch
-                    await handler.callback(m)
-            finally:
-                await asyncio.sleep(0.01)
-
-
-async def _consume_one(queue: asyncio.Queue, psub: PubSub) -> NoReturn:
-    async for m in psub.listen():
-        t = m.get("type")
-        if t and "message" in t:  # pragma: no branch
-            await queue.put(m)
-            break
+    async def _decode_message(message: RedisMessage) -> DecodedMessage: ...
+    @staticmethod
+    async def _parse_message(message: AnyDict) -> RedisMessage: ...
+    def _process_message(
+        self,
+        func: Callable[[RedisMessage], Awaitable[T]],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[RedisMessage], Awaitable[T]]: ...
```

### Comparing `propan-0.1.2.9/propan/brokers/sqs/schema.py` & `propan-0.1.3.0/propan/brokers/sqs/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import asyncio
 from dataclasses import dataclass
 from dataclasses import field as DField
 from typing import Any, Dict, Optional, Sequence
 
+from fast_depends.model import Dependant
 from pydantic import BaseModel, Field, PositiveInt
 from typing_extensions import Literal
 
+from propan.asyncapi.bindings import (
+    AsyncAPIChannelBinding,
+    AsyncAPIOperationBinding,
+    sqs,
+)
+from propan.asyncapi.channels import AsyncAPIChannel
+from propan.asyncapi.message import AsyncAPICorrelationId, AsyncAPIMessage
+from propan.asyncapi.subscription import AsyncAPISubscription
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import BaseHandler, Queue
-from propan.types import SendableMessage
+from propan.types import AnyDict, DecoratedCallable, SendableMessage
 
 
 class RedrivePolicy(BaseModel):
     """SQS Queue RedrivePolicy attribute details"""
 
     dead_letter_target: str = Field(
         default="",
@@ -197,30 +206,74 @@
 
 
 @dataclass
 class Handler(BaseHandler):
     """Store SQSBroker hanlder information and runtime objects"""
 
     queue: SQSQueue
-    consumer_params: Dict[str, Any]
+    consumer_params: AnyDict
 
     task: Optional["asyncio.Task[Any]"] = None
 
+    def __init__(
+        self,
+        callback: DecoratedCallable,
+        dependant: Dependant,
+        queue: SQSQueue,
+        consumer_params: AnyDict,
+        _description: str = "",
+        task: Optional["asyncio.Task[Any]"] = None,
+    ):
+        self.callback = callback
+        self.dependant = dependant
+        self._description = _description
+        self.queue = queue
+        self.consumer_params = consumer_params
+        self.task = task
+
+    def get_schema(self) -> Dict[str, AsyncAPIChannel]:
+        message_title, body, reply_to = self.get_message_object()
+
+        return {
+            self.title: AsyncAPIChannel(
+                subscribe=AsyncAPISubscription(
+                    description=self.description,
+                    bindings=AsyncAPIOperationBinding(
+                        sqs=sqs.AsyncAPISQSOperationBinding(
+                            replyTo=reply_to,
+                        ),
+                    ),
+                    message=AsyncAPIMessage(
+                        title=message_title,
+                        correlationId=AsyncAPICorrelationId(
+                            location="$message.header#/correlation_id"
+                        ),
+                        payload=body,
+                    ),
+                ),
+                bindings=AsyncAPIChannelBinding(
+                    sqs=sqs.AsyncAPISQSChannelBinding(
+                        queue=self.queue.dict(include={"name", "fifo"}),
+                    )
+                ),
+            ),
+        }
+
 
 @dataclass
 class SQSMessage:
     message: SendableMessage
     delay_seconds: int = 0
     deduplication_id: Optional[str] = None
     group_id: Optional[str] = None
     headers: Dict[str, str] = DField(default_factory=dict)
-    message_attributes: Dict[str, Any] = DField(default_factory=dict)
-    message_system_attributes: Dict[str, Any] = DField(default_factory=dict)
+    message_attributes: AnyDict = DField(default_factory=dict)
+    message_system_attributes: AnyDict = DField(default_factory=dict)
 
-    def to_params(self, **extra_headers: Any) -> Dict[str, Any]:
+    def to_params(self, **extra_headers: Any) -> AnyDict:
         msg, content_type = BrokerUsecase._encode_message(self.message)
 
         headers = {**extra_headers, "content-type": content_type, **self.headers}
 
         params = {
             "MessageBody": msg.decode(),
             "DelaySeconds": self.delay_seconds,
```

### Comparing `propan-0.1.2.9/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.3.0/propan/brokers/sqs/sqs_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import asyncio
 import logging
 from functools import wraps
 from typing import (
     Any,
+    Awaitable,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
 from uuid import uuid4
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.session import get_session
+from fast_depends.model import Depends
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     NotPushBackWatcher,
     WatcherContext,
 )
-from propan.brokers.sqs.schema import Handler, SQSMessage, SQSQueue
+from propan.brokers.sqs.schema import Handler
+from propan.brokers.sqs.schema import SQSMessage as SM
+from propan.brokers.sqs.schema import SQSQueue
 from propan.types import (
     AnyCallable,
+    AnyDict,
     DecodedMessage,
     DecoratedCallable,
     HandlerWrapper,
     SendableMessage,
 )
 from propan.utils import context
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
 CorrelationId: TypeAlias = str
+SQSMessage: TypeAlias = PropanMessage[AnyDict]
 
 
 class SQSBroker(BrokerUsecase):
     _connection: AioBaseClient
     _queues: Dict[str, QueueUrl]
     __max_queue_len: int
     response_queue: str
@@ -51,23 +57,30 @@
 
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         log_fmt: Optional[str] = None,
         response_queue: str = "",
+        protocol: str = "sqs",
         **kwargs: Any,
     ) -> None:
-        super().__init__(url, log_fmt=log_fmt, **kwargs)
+        super().__init__(
+            url,
+            log_fmt=log_fmt,
+            url_=url,
+            protocol=protocol,
+            **kwargs,
+        )
         self._queues = {}
         self.__max_queue_len = 4
         self.response_queue = response_queue
         self.response_callbacks = {}
 
-    async def _connect(self, url: Optional[str] = None, **kwargs: Any) -> AioBaseClient:
+    async def _connect(self, *, url: str, **kwargs: Any) -> AioBaseClient:
         session = get_session()
         client: AioBaseClient = await session._create_client(
             service_name="sqs", endpoint_url=url, **kwargs
         )
         context.set_global("client", client)
         await client.__aenter__()
         return client
@@ -82,38 +95,38 @@
                 h.task.cancel()
                 h.task = None
 
         if self._connection is not None:
             await self._connection.__aexit__(None, None, None)
             self._connection = None
 
-    async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage:
+    async def _parse_message(self, message: Dict[str, Any]) -> SQSMessage:
         attributes = message.get("MessageAttributes", {})
 
         headers = {i: j.get("StringValue") for i, j in attributes.items()}
 
-        return PropanMessage(
+        return SQSMessage(
             body=message.get("Body", "").encode(),
             message_id=message.get("MessageId"),
             content_type=headers.pop("content-type", None),
             reply_to=headers.pop("reply_to", None) or "",
             headers=headers,
             raw_message=message,
         )
 
     def _process_message(
         self,
-        func: Callable[[PropanMessage], T],
+        func: Callable[[SQSMessage], Awaitable[T]],
         watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]:
+    ) -> Callable[[SQSMessage], Awaitable[T]]:
         if watcher is None:
             watcher = NotPushBackWatcher()
 
         @wraps(func)
-        async def process_wrapper(message: PropanMessage) -> T:
+        async def process_wrapper(message: SQSMessage) -> T:
             context = WatcherContext(
                 watcher,
                 message.message_id,
                 on_success=self.delete_message,
                 on_max=self.delete_message,
             )
 
@@ -139,16 +152,17 @@
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
-        retry: Union[bool, int] = False,
-        _raw: bool = False,
+        dependencies: Sequence[Depends] = (),
+        description: str = "",
+        **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
         if isinstance(queue, str):
             queue = SQSQueue(queue)
 
         self.__max_queue_len = max((self.__max_queue_len, len(queue.name)))
 
         params = {
@@ -163,21 +177,27 @@
                 *message_attributes,
             ),
         }
         if request_attempt_id is not None:
             params["ReceiveRequestAttemptId"] = request_attempt_id
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
-            func = self._wrap_handler(
+            func, dependant = self._wrap_handler(
                 func,
                 queue=queue.name,
-                retry=retry,
-                _raw=_raw,
+                extra_dependencies=dependencies,
+                **original_kwargs,
+            )
+            handler = Handler(
+                callback=func,
+                queue=queue,
+                consumer_params=params,
+                _description=description,
+                dependant=dependant,
             )
-            handler = Handler(callback=func, queue=queue, consumer_params=params)
             self.handlers.append(handler)
             return func
 
         return wrapper
 
     async def start(self) -> None:
         if self.response_queue:
@@ -235,15 +255,15 @@
         response_future: Optional["asyncio.Future[DecodedMessage]"]
         if callback is True:
             response_future = asyncio.Future()
             self.response_callbacks[correlation_id] = response_future
         else:
             response_future = None
 
-        params = SQSMessage(
+        params = SM(
             message=message,
             headers=headers or {},
             delay_seconds=delay_seconds,
             message_attributes=message_attributes or {},
             message_system_attributes=message_system_attributes or {},
             deduplication_id=deduplication_id,
             group_id=group_id,
@@ -343,15 +363,15 @@
                             has_trash_messages = False
 
                     if has_trash_messages is True:
                         await asyncio.sleep(
                             handler.consumer_params.get("WaitTimeSeconds", 1.0)
                         )
 
-    async def _consume_response(self, message: PropanMessage):
+    async def _consume_response(self, message: SQSMessage):
         correlation_id = message.headers.get("correlation_id")
         if correlation_id is not None:
             callback = self.response_callbacks.pop(correlation_id, None)
             if callback is not None:
                 callback.set_result(await self._decode_message(message))
                 return
 
@@ -363,14 +383,14 @@
             "%(asctime)s %(levelname)s - "
             f"%(queue)-{self.__max_queue_len}s | "
             "%(message_id)-10s "
             "- %(message)s"
         )
 
     def _get_log_context(
-        self, message: Optional[PropanMessage], queue: str
+        self, message: Optional[SQSMessage], queue: str
     ) -> Dict[str, Any]:
         context = {
             "queue": queue,
             **super()._get_log_context(message),
         }
         return context
```

### Comparing `propan-0.1.2.9/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.3.0/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,30 @@
     Sequence,
     TypeVar,
     Union,
 )
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.config import AioConfig
+from fast_depends.model import Depends
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.sqs.schema import Handler, SQSQueue
 from propan.log import access_logger
-from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
+from propan.types import AnyDict, DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
+SQSMessage: TypeAlias = PropanMessage[AnyDict]
 
-class SQSBroker(BrokerUsecase):
-    _connection: AioBaseClient
+class SQSBroker(BrokerUsecase[AnyDict, AioBaseClient]):
     _queues: Dict[str, QueueUrl]
     response_queue: str
     response_callbacks: Dict[str, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
@@ -47,20 +49,24 @@
         aws_session_token: Optional[str] = None,
         config: Optional[AioConfig] = None,
         # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        protocol: str = "sqs",
     ) -> None:
         """"""
     async def connect(
         self,
-        url: str = "http://localhost:9324/",
         *,
+        url: str = "http://localhost:9324/",
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
         verify: Optional[bool] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
@@ -93,14 +99,18 @@
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
+        dependencies: Sequence[Depends] = (),
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> HandlerWrapper:
         """"""
     async def start(self) -> None:
         """"""
     async def create_queue(self, queue: str) -> QueueUrl:
         """"""
     async def delete_queue(self, queue: str) -> None:
@@ -109,15 +119,15 @@
         """"""
     async def delete_message(self) -> None:
         """"""
     async def _consume(self, queue_url: str, handler: Handler) -> NoReturn: ...
     @property
     def fmt(self) -> str: ...
     def _get_log_context(  # type: ignore[override]
-        self, message: Optional[PropanMessage], queue: str
+        self, message: Optional[SQSMessage], queue: str
     ) -> Dict[str, Any]: ...
     @classmethod
     def _build_message(
         cls,
         message: SendableMessage,
         queue_url: str,
         *,
@@ -127,14 +137,14 @@
         message_system_attributes: Optional[Dict[str, Any]] = None,
         # FIFO only
         deduplication_id: Optional[str] = None,
         group_id: Optional[str] = None,
         # broker
         reply_to: str = "",
     ) -> Dict[str, Any]: ...
-    async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage: ...
+    async def _parse_message(self, message: Dict[str, Any]) -> SQSMessage: ...
     def _process_message(
         self,
-        func: Callable[[PropanMessage], T],
+        func: Callable[[SQSMessage], T],
         watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]: ...
+    ) -> Callable[[SQSMessage], T]: ...
     async def _connect(self, *args: Any, **kwargs: Any) -> AioBaseClient: ...
```

### Comparing `propan-0.1.2.9/propan/cli/app.py` & `propan-0.1.3.0/propan/cli/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from typing import Dict, List, Optional
 
 from anyio import create_memory_object_stream, create_task_group
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 from typing_extensions import Protocol
 
+from propan.asyncapi.info import AsyncAPIContact, AsyncAPILicense
 from propan.cli.supervisors.utils import set_exit
 from propan.cli.utils.parser import SettingField
 from propan.log import logger
 from propan.types import AnyCallable, AsyncFunc
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
@@ -26,33 +27,47 @@
     _on_startup_calling: List[AsyncFunc]
     _after_startup_calling: List[AsyncFunc]
     _on_shutdown_calling: List[AsyncFunc]
     _after_shutdown_calling: List[AsyncFunc]
 
     _stop_stream: Optional[MemoryObjectSendStream[bool]]
     _receive_stream: Optional[MemoryObjectReceiveStream[bool]]
+    license: Optional[AsyncAPILicense]
+    contact: Optional[AsyncAPIContact]
 
     def __init__(
         self,
         broker: Optional[Runnable] = None,
         logger: Optional[logging.Logger] = logger,
+        # AsyncAPI args,
+        title: str = "Propan",
+        version: str = "0.1.0",
+        description: str = "",
+        license: Optional[AsyncAPILicense] = None,
+        contact: Optional[AsyncAPIContact] = None,
     ):
         self.broker = broker
         self.logger = logger
         self.context = context
         context.set_global("app", self)
 
         self._on_startup_calling = []
         self._after_startup_calling = []
         self._on_shutdown_calling = []
         self._after_shutdown_calling = []
         self._stop_stream = None
         self._receive_stream = None
         self._command_line_options: Dict[str, SettingField] = {}
 
+        self.title = title
+        self.version = version
+        self.description = description
+        self.license = license
+        self.contact = contact
+
     def set_broker(self, broker: Runnable) -> None:
         self.broker = broker
 
     def on_startup(self, func: AnyCallable) -> AnyCallable:
         return _set_async_hook(self._on_startup_calling, func)
 
     def on_shutdown(self, func: AnyCallable) -> AnyCallable:
```

### Comparing `propan-0.1.2.9/propan/cli/main.py` & `propan-0.1.3.0/propan/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import sys
 from pathlib import Path
 from typing import Dict, Optional
 
 import typer
 
 from propan.__about__ import __version__
-from propan.cli.app import PropanApp
+from propan.cli.docs import docs_app
 from propan.cli.startproject import create_app
-from propan.cli.utils.imports import get_app_path, import_object
+from propan.cli.utils.imports import get_app_path, try_import_propan
 from propan.cli.utils.logs import LogLevels, get_log_level, set_log_level
 from propan.cli.utils.parser import SettingField, parse_cli_args
 from propan.log import logger
 
 cli = typer.Typer(pretty_exceptions_short=True)
 cli.add_typer(
     create_app, name="create", help="Create a new Propan project at [APPNAME] directory"
 )
+cli.add_typer(docs_app, name="docs", help="AsyncAPI scheme commands")
 
 
 def version_callback(version: bool) -> None:
     if version is True:
         import platform
 
         typer.echo(
@@ -102,32 +103,21 @@
 def _run(
     module: Path,
     app: str,
     extra_options: Dict[str, SettingField],
     log_level: int = logging.INFO,
     app_level: int = logging.INFO,
 ) -> None:
-    try:
-        propan_app = import_object(module, app)
+    propan_app = try_import_propan(module, app)
+    set_log_level(log_level, propan_app)
 
-        if not isinstance(propan_app, PropanApp):
-            raise FileNotFoundError(f"{propan_app} is not a PropanApp")
+    propan_app._command_line_options = extra_options
 
-    except (FileNotFoundError, AttributeError) as e:
-        logger.error(e)
-        logger.error("Please, input module like [python_file:propan_app_name]")
-        exit()
+    if sys.platform not in ("win32", "cygwin", "cli"):
+        try:
+            import uvloop
+        except Exception:
+            logger.warning("You have no installed `uvloop`")
+        else:
+            uvloop.install()
 
-    else:
-        set_log_level(log_level, propan_app)
-
-        propan_app._command_line_options = extra_options
-
-        if sys.platform not in ("win32", "cygwin", "cli"):
-            try:
-                import uvloop
-            except Exception:
-                logger.warning("You have no installed `uvloop`")
-            else:
-                uvloop.install()
-
-        asyncio.run(propan_app.run(log_level=app_level))
+    asyncio.run(propan_app.run(log_level=app_level))
```

### Comparing `propan-0.1.2.9/propan/cli/startproject/core.py` & `propan-0.1.3.0/propan/cli/startproject/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,11 +138,11 @@
 
 
 def create_apps_dir(apps: Path) -> Path:
     apps_dir = touch_dir(apps)
 
     write_file(
         apps_dir / "__init__.py",
-        "from .handlers import base_handler",
+        "from .handlers import *",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/app.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/core.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 def create_app_file(
     app_dir: Path,
     broker_annotation: str,
     imports: Sequence[str] = (),
     broker_init: Sequence[str] = ("    await broker.connect(settings.broker.url)",),
 ) -> None:
+    write_file(app_dir / "__init__.py")
+
     write_file(
         app_dir / "serve.py",
         "import logging",
         "from typing import Optional",
         "",
         *imports,
         "from propan import PropanApp",
```

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/nats.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/redis.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.3.0/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/supervisors/basereload.py` & `propan-0.1.3.0/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/supervisors/multiprocess.py` & `propan-0.1.3.0/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/supervisors/utils.py` & `propan-0.1.3.0/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/supervisors/watchfiles.py` & `propan-0.1.3.0/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/utils/imports.py` & `propan-0.1.3.0/propan/cli/utils/imports.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from typing import Any, Tuple
 
+import typer
+
+from propan.cli.app import PropanApp
+
+
+def try_import_propan(module: Path, app: str) -> PropanApp:
+    try:
+        propan_app = import_object(module, app)
+
+    except (ValueError, FileNotFoundError, AttributeError) as e:
+        typer.echo(e, err=True)
+        raise typer.BadParameter(
+            "Please, input module like [python_file:propan_app_name]"
+        ) from e
+
+    else:
+        return propan_app  # type: ignore
+
 
 def import_object(module: Path, app: str) -> Any:
-    spec = spec_from_file_location("mode", f"{module}.py")
+    spec = spec_from_file_location(
+        "mode",
+        f"{module}.py",
+        submodule_search_locations=[str(module.parent.absolute())],
+    )
 
     if spec is None:  # pragma: no cover
         raise FileNotFoundError(module)
 
     mod = module_from_spec(spec)
     loader = spec.loader
 
     if loader is None:  # pragma: no cover
         raise ValueError(f"{spec} has no loader")
 
     loader.exec_module(mod)
     obj = getattr(mod, app)
-
     return obj
 
 
 def get_app_path(app: str) -> Tuple[Path, str]:
     if ":" not in app:
         raise ValueError(f"{app} is not a PropanApp")
```

### Comparing `propan-0.1.2.9/propan/cli/utils/logs.py` & `propan-0.1.3.0/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/cli/utils/parser.py` & `propan-0.1.3.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/fastapi/__init__.py` & `propan-0.1.3.0/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/fastapi/core/route.py` & `propan-0.1.3.0/propan/fastapi/core/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 import asyncio
 import inspect
+from functools import wraps
 from itertools import dropwhile
 from typing import Any, Callable, Coroutine, Optional, Union
 
 from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_dependant, solve_dependencies
 from fastapi.routing import run_endpoint_function
 from pydantic import ValidationError, create_model
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage as NativeMessage
+from propan.brokers._model.schemas import Queue
 from propan.types import AnyDict
 
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
-        path: str,
+        path: Union[Queue, str],
+        *extra: Union[Queue, str],
         endpoint: Callable[..., Any],
-        broker: BrokerUsecase,
-        *,
+        broker: BrokerUsecase[Any, Any],
         dependency_overrides_provider: Optional[Any] = None,
         **handle_kwargs: AnyDict,
     ) -> None:
         self.path = path
         self.broker = broker
-        self.dependant = get_dependant(path=path, call=endpoint)
+        self.dependant = get_dependant(
+            path=(path if isinstance(path, str) else path.name) or "",
+            call=endpoint,
+        )
 
-        handler = PropanMessage.get_session(
-            self.dependant, dependency_overrides_provider
+        handler = wraps(endpoint)(
+            PropanMessage.get_session(
+                self.dependant,
+                dependency_overrides_provider,
+            )
         )
-        broker.handle(path, _raw=True, **handle_kwargs)(handler)  # type: ignore
+
+        broker.handle(
+            path,
+            *extra,
+            _raw=True,
+            _get_dependant=get_dependant,  # type: ignore
+            **handle_kwargs,  # type: ignore
+        )(handler)
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
     _headers: AnyDict  # type: ignore
     _body: AnyDict  # type: ignore
@@ -54,30 +69,30 @@
         self._query_params = self._body
 
     @classmethod
     def get_session(
         cls,
         dependant: Dependant,
         dependency_overrides_provider: Optional[Any] = None,
-    ) -> Callable[[NativeMessage], Any]:
+    ) -> Callable[[NativeMessage[Any]], Any]:
         assert dependant.call
         func = get_app(dependant, dependency_overrides_provider)
 
         dependencies_names = tuple(i.name for i in dependant.dependencies)
 
         first_arg = next(
             dropwhile(
                 lambda i: i in dependencies_names,
                 inspect.signature(dependant.call).parameters,
             ),
             None,
         )
 
-        async def app(message: NativeMessage) -> Any:
-            body: Union[AnyDict, bytes] = message.body
+        async def app(message: NativeMessage[Any]) -> Any:
+            body = message.decoded_body
             if first_arg is not None:
                 if not isinstance(body, dict):  # pragma: no branch
                     body = {first_arg: body}
 
                 session = cls(body, message.headers)
             else:
                 session = cls()
```

### Comparing `propan-0.1.2.9/propan/fastapi/kafka/router.pyi` & `propan-0.1.3.0/propan/fastapi/kafka/router.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from asyncio import AbstractEventLoop
 from enum import Enum
 from ssl import SSLContext
 from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
 
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
+from aiokafka.structs import ConsumerRecord
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 from typing_extensions import Literal, TypeVar
 
 from propan import KafkaBroker
 from propan.__about__ import __version__
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 Partition = TypeVar("Partition")
 
 class KafkaRouter(PropanRouter[KafkaBroker]):
@@ -88,18 +90,22 @@
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
         loop: Optional[AbstractEventLoop] = None,
         # Broker kwargs
+        schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        decode_message: CustomDecoder[ConsumerRecord] = None,
+        parse_message: CustomParser[ConsumerRecord] = None,
+        protocol: str = "kafka",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         *topics: str,
         endpoint: AnyCallable,
         group_id: Optional[str] = None,
@@ -127,15 +133,19 @@
         consumer_timeout_ms: int = 200,
         max_poll_records: Optional[int] = None,
         exclude_internal_topics: bool = True,
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
+        # broker kwargs
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[ConsumerRecord] = None,
+        parse_message: CustomParser[ConsumerRecord] = None,
+        description: str = "",
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         *topics: str,
         group_id: Optional[str] = None,
         key_deserializer: Optional[Callable[[bytes], Any]] = None,
@@ -162,10 +172,14 @@
         consumer_timeout_ms: int = 200,
         max_poll_records: Optional[int] = None,
         exclude_internal_topics: bool = True,
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
+        # broker kwargs
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[ConsumerRecord] = None,
+        parse_message: CustomParser[ConsumerRecord] = None,
+        description: str = "",
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.9/propan/fastapi/nats/router.pyi` & `propan-0.1.3.0/propan/fastapi/nats/router.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     DEFAULT_RECONNECT_TIME_WAIT,
     Callback,
     Credentials,
     ErrorCallback,
     JWTCallback,
     SignatureCallback,
 )
+from nats.aio.msg import Msg
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import NatsBroker
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class NatsRouter(PropanRouter[NatsBroker]):
     def __init__(
         self,
@@ -82,30 +84,40 @@
         on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
         # Broker kwargs
+        schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        decode_message: CustomDecoder[Msg] = None,
+        parse_message: CustomParser[Msg] = None,
+        protocol: str = "nats",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         subject: str,
         *,
         queue: str = "",
         endpoint: AnyCallable,
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[Msg] = None,
+        parse_message: CustomParser[Msg] = None,
+        description: str = "",
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         subject: str,
         *,
         queue: str = "",
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[Msg] = None,
+        parse_message: CustomParser[Msg] = None,
+        description: str = "",
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.9/propan/fastapi/rabbit/router.pyi` & `propan-0.1.3.0/propan/fastapi/rabbit/router.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 from enum import Enum
 from ssl import SSLContext
 from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
 
 import aio_pika
+from aio_pika.message import IncomingMessage
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from pamqp.common import FieldTable
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import RabbitBroker
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class RabbitRouter(PropanRouter[RabbitBroker]):
     def __init__(
@@ -53,26 +55,37 @@
         ),
         # Broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         consumers: Optional[int] = None,
+        decode_message: CustomDecoder[IncomingMessage] = None,
+        parse_message: CustomParser[IncomingMessage] = None,
+        schema_url: str = "/asyncapi",
+        protocol: str = "amqp",
+        protocol_version: str = "0.9.1",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         endpoint: AnyCallable,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[IncomingMessage] = None,
+        parse_message: CustomParser[IncomingMessage] = None,
+        description: str = "",
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[IncomingMessage] = None,
+        parse_message: CustomParser[IncomingMessage] = None,
+        description: str = "",
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.9/propan/fastapi/redis/router.pyi` & `propan-0.1.3.0/propan/fastapi/redis/router.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from fastapi.utils import generate_unique_id
 from redis.asyncio.connection import BaseParser, DefaultParser, Encoder
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import RedisBroker
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable
+from propan.types import AnyCallable, AnyDict
 
 class RedisRouter(PropanRouter[RedisBroker]):
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: float = 1.0,
         host: str = "localhost",
@@ -56,28 +57,38 @@
         on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
         # Broker kwargs
+        schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        protocol: str = "redis",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         channel: str,
         *,
         endpoint: AnyCallable,
         pattern: bool = False,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.9/propan/fastapi/sqs/router.pyi` & `propan-0.1.3.0/propan/fastapi/sqs/router.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import SQSBroker
+from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers.sqs.schema import SQSQueue
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable
+from propan.types import AnyCallable, AnyDict
 
 class SQSRouter(PropanRouter[SQSBroker]):
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
@@ -46,40 +47,50 @@
         on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
         # Broker kwargs
+        schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        protocol: str = "sqs",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
         endpoint: AnyCallable,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
+        decode_message: CustomDecoder[AnyDict] = None,
+        parse_message: CustomParser[AnyDict] = None,
+        description: str = "",
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.9/propan/log/formatter.py` & `propan-0.1.3.0/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/log/logging.py` & `propan-0.1.3.0/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/__init__.py` & `propan-0.1.3.0/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/kafka.py` & `propan-0.1.3.0/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/nats.py` & `propan-0.1.3.0/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/rabbit.py` & `propan-0.1.3.0/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/redis.py` & `propan-0.1.3.0/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/test/sqs.py` & `propan-0.1.3.0/propan/test/sqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
 from propan import SQSBroker
-from propan.brokers.sqs import SQSMessage
+from propan.brokers.sqs.schema import SQSMessage
 from propan.test.utils import call_handler
 from propan.types import SendableMessage
 
 __all__ = (
     "build_message",
     "TestSQSBroker",
 )
```

### Comparing `propan-0.1.2.9/propan/test/utils.py` & `propan-0.1.3.0/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/propan/utils/context/main.py` & `propan-0.1.3.0/propan/utils/context/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from contextlib import contextmanager
 from contextvars import ContextVar, Token
 from typing import Any, Dict, Iterator, TypeVar
 
-from propan.utils.classes import Singlethon
+from propan.utils.classes import Singleton
 
 T = TypeVar("T")
 
 
-class ContextRepo(Singlethon):
+class ContextRepo(Singleton):
     _global_context: Dict[str, Any]
     _scope_context: Dict[str, ContextVar[Any]]
 
     def __init__(self) -> None:
         self._global_context = {}
         self._scope_context = {}
```

### Comparing `propan-0.1.2.9/propan/utils/context/types.py` & `propan-0.1.3.0/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/LICENSE` & `propan-0.1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.9/README.md` & `propan-0.1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
   * **SQS** (based on <a href="https://aiobotocore.readthedocs.io/en/latest/" target="_blank">aiobotocore</a>)
   * **Nats** (based on <a href="https://github.com/nats-io/nats.py" target="_blank">nats-py</a>)
 * <a href="https://lancetnik.github.io/Propan/getting_started/4_broker/5_rpc/" target="_blank">**RPC**</a>: The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Great to develop**](#cli-power): CLI tool provides great development experience:
   * framework-independent way to manage the project environment
   * application code *hot reload*
   * robust application templates
+* [**Documentation**](#project-documentation): **Propan** automatically generates and presents an interactive <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> documentation for your project
 * <a href="https://lancetnik.github.io/Propan/getting_started/7_testing" target="_blank">**Testability**</a>: **Propan** allows you to test your app without external dependencies: you do not have to set up a Message Broker, you can use a virtual one!
 
 ### Supported MQ brokers
 
 |                   | async                                                   | sync                 |
 |-------------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
@@ -234,14 +235,24 @@
                        broker: RabbitBroker = Context()):
     assert dep is True
     assert broker is rabbit_broker
 ```
 
 ---
 
+## Project Documentation
+
+**Propan** automatically generates documentation for your project according to the <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> specification. You can work with both generated artifacts and place a Web view of your documentation on resources available to related teams.
+
+The availability of such documentation significantly simplifies the integration of services: you can immediately see what channels and message format the application works with. And most importantly, it doesn't cost you anything - **Propan** has already done everything for you!
+
+![HTML-page](https://lancetnik.github.io/Propan/assets/img/docs-html-short.png)
+
+---
+
 ## CLI power
 
 **Propan** has its own CLI tool that provided the following features:
 
 * project generation
 * multiprocessing workers
 * project hot reloading
@@ -332,18 +343,18 @@
 using the `@event` decorator. This decorator is similar to the decorator `@handle` for the corresponding brokers.
 
 ```python
 from fastapi import Depends, FastAPI
 from pydantic import BaseModel
 from propan.fastapi import RabbitRouter
 
-app = FastAPI()
-
 router = RabbitRouter("amqp://guest:guest@localhost:5672")
 
+app = FastAPI(lifespan=router.lifespan_context)
+
 class Incoming(BaseModel):
     m: dict
 
 def call():
     return True
 
 @router.event("test")
```

#### html2text {}

```diff
@@ -16,15 +16,17 @@
 framework you want * **MQ independent**: Single interface to popular MQ: *
 **Redis** (based on redis-py) * **RabbitMQ** (based on aio-pika) * **Kafka**
 (based on aiokafka) * **SQS** (based on aiobotocore) * **Nats** (based on nats-
 py) * **RPC**: The framework supports RPC requests over MQ, which will allow
 performing long operations on remote services asynchronously. * [**Great to
 develop**](#cli-power): CLI tool provides great development experience: *
 framework-independent way to manage the project environment * application code
-*hot reload* * robust application templates * **Testability**: **Propan**
+*hot reload* * robust application templates * [**Documentation**](#project-
+documentation): **Propan** automatically generates and presents an interactive
+**AsyncAPI** documentation for your project * **Testability**: **Propan**
 allows you to test your app without external dependencies: you do not have to
 set up a Message Broker, you can use a virtual one! ### Supported MQ brokers |
 | async | sync | |-------------------|:----------------------------------------
 ---------------:|:--------------------:| | **RabbitMQ** | :heavy_check_mark:
 **stable** :heavy_check_mark: | :mag: planning :mag: | | **Redis** | :
 heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
 **Nats** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
@@ -82,41 +84,50 @@
 (like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
 main/examples/dependencies). ```python import aio_pika from propan import
 PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
 guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
 dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
 def base_handler(body: dict, dep: bool = Depends(dependency), broker:
 RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
-``` --- ## CLI power **Propan** has its own CLI tool that provided the
-following features: * project generation * multiprocessing workers * project
-hot reloading * custom command line arguments passing ### Context passing For
-example: pass your current *.env* project setting to context ```bash propan run
-serve:app --env=.env.dev ``` ```python from propan import PropanApp,
-RabbitBroker from propan.annotations import ContextRepo from pydantic import
-BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
-setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
-context.set_global("settings", settings) ``` ### Project template Also,
-**Propan CLI** is able to generate a production-ready application template:
-```bash propan create async rabbit [projectname] ``` *Notice: project template
-require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
-Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
-d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
-Now you can enjoy a new development experience! --- ## HTTP Frameworks
-integrations ### Any Framework You can use **Propan** `MQBrokers` without
-`PropanApp`. Just *start* and *stop* them according to your application
-lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
-Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
-@broker.handle("test") async def base_handler(body): print(body)
-@app.after_server_start async def start_broker(app, loop): await broker.start()
-@app.after_server_stop async def stop_broker(app, loop): await broker.close()
-``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
-Just import a **PropanRouter** you need and declare the message handler using
-the `@event` decorator. This decorator is similar to the decorator `@handle`
-for the corresponding brokers. ```python from fastapi import Depends, FastAPI
-from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
-FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
+``` --- ## Project Documentation **Propan** automatically generates
+documentation for your project according to the **AsyncAPI** specification. You
+can work with both generated artifacts and place a Web view of your
+documentation on resources available to related teams. The availability of such
+documentation significantly simplifies the integration of services: you can
+immediately see what channels and message format the application works with.
+And most importantly, it doesn't cost you anything - **Propan** has already
+done everything for you! ![HTML-page](https://lancetnik.github.io/Propan/
+assets/img/docs-html-short.png) --- ## CLI power **Propan** has its own CLI
+tool that provided the following features: * project generation *
+multiprocessing workers * project hot reloading * custom command line arguments
+passing ### Context passing For example: pass your current *.env* project
+setting to context ```bash propan run serve:app --env=.env.dev ``` ```python
+from propan import PropanApp, RabbitBroker from propan.annotations import
+ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
+(BaseSettings): ... @app.on_startup async def setup(env: str, context:
+ContextRepo): settings = Settings(_env_file=env) context.set_global("settings",
+settings) ``` ### Project template Also, **Propan CLI** is able to generate a
+production-ready application template: ```bash propan create async rabbit
+[projectname] ``` *Notice: project template require* `pydantic[dotenv]`
+*installation.* Run the created project: ```bash # Run rabbimq first docker
+compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
+[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+development experience! --- ## HTTP Frameworks integrations ### Any Framework
+You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
+them according to your application lifespan. ```python from propan import
+NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
+NatsBroker("nats://localhost:4222") @broker.handle("test") async def
+base_handler(body): print(body) @app.after_server_start async def start_broker
+(app, loop): await broker.start() @app.after_server_stop async def stop_broker
+(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
+be used as part of **FastAPI**. Just import a **PropanRouter** you need and
+declare the message handler using the `@event` decorator. This decorator is
+similar to the decorator `@handle` for the corresponding brokers. ```python
+from fastapi import Depends, FastAPI from pydantic import BaseModel from
+propan.fastapi import RabbitRouter router = RabbitRouter("amqp://guest:
+guest@localhost:5672") app = FastAPI(lifespan=router.lifespan_context) class
 Incoming(BaseModel): m: dict def call(): return True @router.event("test")
 async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
 "Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
 framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
 tree/main/examples)
```

### Comparing `propan-0.1.2.9/pyproject.toml` & `propan-0.1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends>=1.1.5",
+    "fast-depends==1.1.6",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
@@ -66,55 +66,68 @@
 ]
 
 async-nats = [
     "nats-py>=2,!=2.3.0",
 ]
 
 async-redis = [
-    "redis>=4.2.0rc1"
+    "redis>=4.2.0rc1",
 ]
 
 async-kafka = [
-    "aiokafka>=0.8"
+    "aiokafka>=0.8",
+]
+
+doc = [
+    "PyYAML",
+    "pytest[email]",
+    "polyfactory; python_version > '3.7'",
+    "jsonref",
+    "fastapi",
+    "uvicorn",
 ]
 
 async-sqs = [
-    "aiobotocore"
+    "aiobotocore",
 ]
 
 test = [
+    "propan[doc]",
     "propan[async-rabbit]",
     "propan[async-nats]",
     "propan[async-redis]",
     "propan[async-kafka]",
     "propan[async-sqs]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
 
     "fastapi",
+    "python-dotenv",
 
     "asyncmock; python_version < '3.8'",
 ]
 
-doc = [
+dev-doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-macros-plugin",
+    "mkdocs-glightbox",
 
     "typer[all]",
 ]
 
 dev = [
     "propan[test]",
-    "propan[doc]",
+    "propan[dev-doc]",
 
     "types-redis",
+    "types-PyYAML",
 
     "mypy==1.1.1",
     "black==23.3.0",
     "isort>=5",
     "ruff==0.0.261",
     "typer[all]",
 ]
```

### Comparing `propan-0.1.2.9/PKG-INFO` & `propan-0.1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6f70  : 2.1.Name: prop
 00000020: 616e 0a56 6572 7369 6f6e 3a20 302e 312e  an.Version: 0.1.
-00000030: 322e 390a 5375 6d6d 6172 793a 2050 726f  2.9.Summary: Pro
+00000030: 332e 300a 5375 6d6d 6172 793a 2050 726f  3.0.Summary: Pro
 00000040: 7061 6e20 6672 616d 6577 6f72 6b3a 2074  pan framework: t
 00000050: 6865 2073 696d 706c 6573 7420 7761 7920  he simplest way 
 00000060: 746f 2077 6f72 6b20 7769 7468 2061 206d  to work with a m
 00000070: 6573 7361 6769 6e67 2071 7565 7565 730a  essaging queues.
 00000080: 5072 6f6a 6563 742d 5552 4c3a 2048 6f6d  Project-URL: Hom
 00000090: 6570 6167 652c 2068 7474 7073 3a2f 2f6c  epage, https://l
 000000a0: 616e 6365 746e 696b 2e67 6974 6875 622e  ancetnik.github.
@@ -105,15 +105,15 @@
 00000680: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
 00000690: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
 000006a0: 4d6f 6475 6c65 730a 436c 6173 7369 6669  Modules.Classifi
 000006b0: 6572 3a20 5479 7069 6e67 203a 3a20 5479  er: Typing :: Ty
 000006c0: 7065 640a 5265 7175 6972 6573 2d50 7974  ped.Requires-Pyt
 000006d0: 686f 6e3a 203e 3d33 2e37 0a52 6571 7569  hon: >=3.7.Requi
 000006e0: 7265 732d 4469 7374 3a20 6661 7374 2d64  res-Dist: fast-d
-000006f0: 6570 656e 6473 3e3d 312e 312e 350a 5265  epends>=1.1.5.Re
+000006f0: 6570 656e 6473 3d3d 312e 312e 360a 5265  epends==1.1.6.Re
 00000700: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
 00000710: 6572 0a52 6571 7569 7265 732d 4469 7374  er.Requires-Dist
 00000720: 3a20 7576 6c6f 6f70 213d 302e 3135 2e30  : uvloop!=0.15.0
 00000730: 2c21 3d30 2e31 352e 312c 3e3d 302e 3134  ,!=0.15.1,>=0.14
 00000740: 2e30 3b20 7379 735f 706c 6174 666f 726d  .0; sys_platform
 00000750: 2021 3d20 2777 696e 3332 2720 616e 6420   != 'win32' and 
 00000760: 2873 7973 5f70 6c61 7466 6f72 6d20 213d  (sys_platform !=
@@ -154,857 +154,947 @@
 00000990: 2027 6465 7627 0a52 6571 7569 7265 732d   'dev'.Requires-
 000009a0: 4469 7374 3a20 6973 6f72 743e 3d35 3b20  Dist: isort>=5; 
 000009b0: 6578 7472 6120 3d3d 2027 6465 7627 0a52  extra == 'dev'.R
 000009c0: 6571 7569 7265 732d 4469 7374 3a20 6d79  equires-Dist: my
 000009d0: 7079 3d3d 312e 312e 313b 2065 7874 7261  py==1.1.1; extra
 000009e0: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
 000009f0: 6573 2d44 6973 743a 2070 726f 7061 6e5b  es-Dist: propan[
-00000a00: 646f 635d 3b20 6578 7472 6120 3d3d 2027  doc]; extra == '
-00000a10: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
-00000a20: 7374 3a20 7072 6f70 616e 5b74 6573 745d  st: propan[test]
-00000a30: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
-00000a40: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a50: 7275 6666 3d3d 302e 302e 3236 313b 2065  ruff==0.0.261; e
-00000a60: 7874 7261 203d 3d20 2764 6576 270a 5265  xtra == 'dev'.Re
-00000a70: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
-00000a80: 6572 5b61 6c6c 5d3b 2065 7874 7261 203d  er[all]; extra =
-00000a90: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
-00000aa0: 2d44 6973 743a 2074 7970 6573 2d72 6564  -Dist: types-red
-00000ab0: 6973 3b20 6578 7472 6120 3d3d 2027 6465  is; extra == 'de
-00000ac0: 7627 0a50 726f 7669 6465 732d 4578 7472  v'.Provides-Extr
-00000ad0: 613a 2064 6f63 0a52 6571 7569 7265 732d  a: doc.Requires-
-00000ae0: 4469 7374 3a20 6d64 782d 696e 636c 7564  Dist: mdx-includ
-00000af0: 653c 322e 302e 302c 3e3d 312e 342e 313b  e<2.0.0,>=1.4.1;
-00000b00: 2065 7874 7261 203d 3d20 2764 6f63 270a   extra == 'doc'.
-00000b10: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-00000b20: 6b64 6f63 732d 6d61 6372 6f73 2d70 6c75  kdocs-macros-plu
-00000b30: 6769 6e3b 2065 7874 7261 203d 3d20 2764  gin; extra == 'd
-00000b40: 6f63 270a 5265 7175 6972 6573 2d44 6973  oc'.Requires-Dis
-00000b50: 743a 206d 6b64 6f63 732d 6d61 7465 7269  t: mkdocs-materi
-00000b60: 616c 3c39 2e30 2e30 2c3e 3d38 2e31 2e34  al<9.0.0,>=8.1.4
-00000b70: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
-00000b80: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b90: 6d6b 646f 6373 2d73 7461 7469 632d 6931  mkdocs-static-i1
-00000ba0: 386e 3b20 6578 7472 6120 3d3d 2027 646f  8n; extra == 'do
-00000bb0: 6327 0a52 6571 7569 7265 732d 4469 7374  c'.Requires-Dist
-00000bc0: 3a20 7479 7065 725b 616c 6c5d 3b20 6578  : typer[all]; ex
-00000bd0: 7472 6120 3d3d 2027 646f 6327 0a50 726f  tra == 'doc'.Pro
-00000be0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
-00000bf0: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
-00000c00: 2061 7379 6e63 6d6f 636b 3b20 7079 7468   asyncmock; pyth
-00000c10: 6f6e 5f76 6572 7369 6f6e 203c 2027 332e  on_version < '3.
-00000c20: 3827 2061 6e64 2065 7874 7261 203d 3d20  8' and extra == 
-00000c30: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-00000c40: 4469 7374 3a20 636f 7665 7261 6765 5b74  Dist: coverage[t
-00000c50: 6f6d 6c5d 3e3d 372e 323b 2065 7874 7261  oml]>=7.2; extra
-00000c60: 203d 3d20 2774 6573 7427 0a52 6571 7569   == 'test'.Requi
-00000c70: 7265 732d 4469 7374 3a20 6661 7374 6170  res-Dist: fastap
-00000c80: 693b 2065 7874 7261 203d 3d20 2774 6573  i; extra == 'tes
-00000c90: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
-00000ca0: 3a20 7072 6f70 616e 5b61 7379 6e63 2d6b  : propan[async-k
-00000cb0: 6166 6b61 5d3b 2065 7874 7261 203d 3d20  afka]; extra == 
-00000cc0: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-00000cd0: 4469 7374 3a20 7072 6f70 616e 5b61 7379  Dist: propan[asy
-00000ce0: 6e63 2d6e 6174 735d 3b20 6578 7472 6120  nc-nats]; extra 
-00000cf0: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-00000d00: 6573 2d44 6973 743a 2070 726f 7061 6e5b  es-Dist: propan[
-00000d10: 6173 796e 632d 7261 6262 6974 5d3b 2065  async-rabbit]; e
-00000d20: 7874 7261 203d 3d20 2774 6573 7427 0a52  xtra == 'test'.R
-00000d30: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
-00000d40: 6f70 616e 5b61 7379 6e63 2d72 6564 6973  opan[async-redis
-00000d50: 5d3b 2065 7874 7261 203d 3d20 2774 6573  ]; extra == 'tes
-00000d60: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
-00000d70: 3a20 7072 6f70 616e 5b61 7379 6e63 2d73  : propan[async-s
-00000d80: 7173 5d3b 2065 7874 7261 203d 3d20 2774  qs]; extra == 't
-00000d90: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-00000da0: 7374 3a20 7079 7465 7374 2d61 7379 6e63  st: pytest-async
-00000db0: 696f 3e3d 302e 3231 3b20 6578 7472 6120  io>=0.21; extra 
-00000dc0: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-00000dd0: 6573 2d44 6973 743a 2070 7974 6573 743e  es-Dist: pytest>
-00000de0: 3d37 3b20 6578 7472 6120 3d3d 2027 7465  =7; extra == 'te
-00000df0: 7374 270a 4465 7363 7269 7074 696f 6e2d  st'.Description-
-00000e00: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000e10: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 7020  xt/markdown..<p 
-00000e20: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000e30: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000e40: 7073 3a2f 2f6c 616e 6365 746e 696b 2e67  ps://lancetnik.g
-00000e50: 6974 6875 622e 696f 2f50 726f 7061 6e2f  ithub.io/Propan/
-00000e60: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000e70: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-00000e80: 7372 633d 2268 7474 7073 3a2f 2f6c 616e  src="https://lan
-00000e90: 6365 746e 696b 2e67 6974 6875 622e 696f  cetnik.github.io
-00000ea0: 2f50 726f 7061 6e2f 6173 7365 7473 2f69  /Propan/assets/i
-00000eb0: 6d67 2f6c 6f67 6f2d 6e6f 2d62 6163 6b67  mg/logo-no-backg
-00000ec0: 726f 756e 642e 706e 6722 2061 6c74 3d22  round.png" alt="
-00000ed0: 5072 6f70 616e 206c 6f67 6f22 2073 7479  Propan logo" sty
-00000ee0: 6c65 3d22 6865 6967 6874 3a20 3235 3070  le="height: 250p
-00000ef0: 783b 2077 6964 7468 3a20 3630 3070 783b  x; width: 600px;
-00000f00: 222f 3e0a 2020 2020 3c2f 613e 0a3c 2f70  "/>.    </a>.</p
-00000f10: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
-00000f20: 7465 7222 3e0a 2020 2020 3c61 2068 7265  ter">.    <a hre
-00000f30: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000f40: 622e 636f 6d2f 4c61 6e63 6574 6e69 6b2f  b.com/Lancetnik/
-00000f50: 5072 6f70 616e 2f61 6374 696f 6e73 2f77  Propan/actions/w
-00000f60: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
-00000f70: 6d6c 2220 7461 7267 6574 3d22 5f62 6c61  ml" target="_bla
-00000f80: 6e6b 223e 0a20 2020 2020 2020 203c 696d  nk">.        <im
-00000f90: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
-00000fa0: 6974 6875 622e 636f 6d2f 4c61 6e63 6574  ithub.com/Lancet
-00000fb0: 6e69 6b2f 5072 6f70 616e 2f61 6374 696f  nik/Propan/actio
-00000fc0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-00000fd0: 7473 2e79 6d6c 2f62 6164 6765 2e73 7667  ts.yml/badge.svg
-00000fe0: 2220 616c 743d 2254 6573 7473 2063 6f76  " alt="Tests cov
-00000ff0: 6572 6167 6522 2f3e 0a20 2020 203c 2f61  erage"/>.    </a
-00001000: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00001010: 7474 7073 3a2f 2f63 6f76 6572 6167 652d  ttps://coverage-
-00001020: 6261 6467 652e 7361 6d75 656c 636f 6c76  badge.samuelcolv
-00001030: 696e 2e77 6f72 6b65 7273 2e64 6576 2f72  in.workers.dev/r
-00001040: 6564 6972 6563 742f 6c61 6e63 6574 6e69  edirect/lancetni
-00001050: 6b2f 7072 6f70 616e 2220 7461 7267 6574  k/propan" target
+00000a00: 6465 762d 646f 635d 3b20 6578 7472 6120  dev-doc]; extra 
+00000a10: 3d3d 2027 6465 7627 0a52 6571 7569 7265  == 'dev'.Require
+00000a20: 732d 4469 7374 3a20 7072 6f70 616e 5b74  s-Dist: propan[t
+00000a30: 6573 745d 3b20 6578 7472 6120 3d3d 2027  est]; extra == '
+00000a40: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
+00000a50: 7374 3a20 7275 6666 3d3d 302e 302e 3236  st: ruff==0.0.26
+00000a60: 313b 2065 7874 7261 203d 3d20 2764 6576  1; extra == 'dev
+00000a70: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
+00000a80: 2074 7970 6572 5b61 6c6c 5d3b 2065 7874   typer[all]; ext
+00000a90: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
+00000aa0: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
+00000ab0: 2d70 7979 616d 6c3b 2065 7874 7261 203d  -pyyaml; extra =
+00000ac0: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
+00000ad0: 2d44 6973 743a 2074 7970 6573 2d72 6564  -Dist: types-red
+00000ae0: 6973 3b20 6578 7472 6120 3d3d 2027 6465  is; extra == 'de
+00000af0: 7627 0a50 726f 7669 6465 732d 4578 7472  v'.Provides-Extr
+00000b00: 613a 2064 6576 2d64 6f63 0a52 6571 7569  a: dev-doc.Requi
+00000b10: 7265 732d 4469 7374 3a20 6d64 782d 696e  res-Dist: mdx-in
+00000b20: 636c 7564 653c 322e 302e 302c 3e3d 312e  clude<2.0.0,>=1.
+00000b30: 342e 313b 2065 7874 7261 203d 3d20 2764  4.1; extra == 'd
+00000b40: 6576 2d64 6f63 270a 5265 7175 6972 6573  ev-doc'.Requires
+00000b50: 2d44 6973 743a 206d 6b64 6f63 732d 676c  -Dist: mkdocs-gl
+00000b60: 6967 6874 626f 783b 2065 7874 7261 203d  ightbox; extra =
+00000b70: 3d20 2764 6576 2d64 6f63 270a 5265 7175  = 'dev-doc'.Requ
+00000b80: 6972 6573 2d44 6973 743a 206d 6b64 6f63  ires-Dist: mkdoc
+00000b90: 732d 6d61 6372 6f73 2d70 6c75 6769 6e3b  s-macros-plugin;
+00000ba0: 2065 7874 7261 203d 3d20 2764 6576 2d64   extra == 'dev-d
+00000bb0: 6f63 270a 5265 7175 6972 6573 2d44 6973  oc'.Requires-Dis
+00000bc0: 743a 206d 6b64 6f63 732d 6d61 7465 7269  t: mkdocs-materi
+00000bd0: 616c 3c39 2e30 2e30 2c3e 3d38 2e31 2e34  al<9.0.0,>=8.1.4
+00000be0: 3b20 6578 7472 6120 3d3d 2027 6465 762d  ; extra == 'dev-
+00000bf0: 646f 6327 0a52 6571 7569 7265 732d 4469  doc'.Requires-Di
+00000c00: 7374 3a20 6d6b 646f 6373 2d73 7461 7469  st: mkdocs-stati
+00000c10: 632d 6931 386e 3b20 6578 7472 6120 3d3d  c-i18n; extra ==
+00000c20: 2027 6465 762d 646f 6327 0a52 6571 7569   'dev-doc'.Requi
+00000c30: 7265 732d 4469 7374 3a20 7479 7065 725b  res-Dist: typer[
+00000c40: 616c 6c5d 3b20 6578 7472 6120 3d3d 2027  all]; extra == '
+00000c50: 6465 762d 646f 6327 0a50 726f 7669 6465  dev-doc'.Provide
+00000c60: 732d 4578 7472 613a 2064 6f63 0a52 6571  s-Extra: doc.Req
+00000c70: 7569 7265 732d 4469 7374 3a20 6661 7374  uires-Dist: fast
+00000c80: 6170 693b 2065 7874 7261 203d 3d20 2764  api; extra == 'd
+00000c90: 6f63 270a 5265 7175 6972 6573 2d44 6973  oc'.Requires-Dis
+00000ca0: 743a 206a 736f 6e72 6566 3b20 6578 7472  t: jsonref; extr
+00000cb0: 6120 3d3d 2027 646f 6327 0a52 6571 7569  a == 'doc'.Requi
+00000cc0: 7265 732d 4469 7374 3a20 706f 6c79 6661  res-Dist: polyfa
+00000cd0: 6374 6f72 793b 2070 7974 686f 6e5f 7665  ctory; python_ve
+00000ce0: 7273 696f 6e20 3e20 2733 2e37 2720 616e  rsion > '3.7' an
+00000cf0: 6420 6578 7472 6120 3d3d 2027 646f 6327  d extra == 'doc'
+00000d00: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000d10: 7079 7465 7374 5b65 6d61 696c 5d3b 2065  pytest[email]; e
+00000d20: 7874 7261 203d 3d20 2764 6f63 270a 5265  xtra == 'doc'.Re
+00000d30: 7175 6972 6573 2d44 6973 743a 2070 7979  quires-Dist: pyy
+00000d40: 616d 6c3b 2065 7874 7261 203d 3d20 2764  aml; extra == 'd
+00000d50: 6f63 270a 5265 7175 6972 6573 2d44 6973  oc'.Requires-Dis
+00000d60: 743a 2075 7669 636f 726e 3b20 6578 7472  t: uvicorn; extr
+00000d70: 6120 3d3d 2027 646f 6327 0a50 726f 7669  a == 'doc'.Provi
+00000d80: 6465 732d 4578 7472 613a 2074 6573 740a  des-Extra: test.
+00000d90: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+00000da0: 7379 6e63 6d6f 636b 3b20 7079 7468 6f6e  syncmock; python
+00000db0: 5f76 6572 7369 6f6e 203c 2027 332e 3827  _version < '3.8'
+00000dc0: 2061 6e64 2065 7874 7261 203d 3d20 2774   and extra == 't
+00000dd0: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
+00000de0: 7374 3a20 636f 7665 7261 6765 5b74 6f6d  st: coverage[tom
+00000df0: 6c5d 3e3d 372e 323b 2065 7874 7261 203d  l]>=7.2; extra =
+00000e00: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
+00000e10: 732d 4469 7374 3a20 6661 7374 6170 693b  s-Dist: fastapi;
+00000e20: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
+00000e30: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000e40: 7072 6f70 616e 5b61 7379 6e63 2d6b 6166  propan[async-kaf
+00000e50: 6b61 5d3b 2065 7874 7261 203d 3d20 2774  ka]; extra == 't
+00000e60: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
+00000e70: 7374 3a20 7072 6f70 616e 5b61 7379 6e63  st: propan[async
+00000e80: 2d6e 6174 735d 3b20 6578 7472 6120 3d3d  -nats]; extra ==
+00000e90: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
+00000ea0: 2d44 6973 743a 2070 726f 7061 6e5b 6173  -Dist: propan[as
+00000eb0: 796e 632d 7261 6262 6974 5d3b 2065 7874  ync-rabbit]; ext
+00000ec0: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
+00000ed0: 7569 7265 732d 4469 7374 3a20 7072 6f70  uires-Dist: prop
+00000ee0: 616e 5b61 7379 6e63 2d72 6564 6973 5d3b  an[async-redis];
+00000ef0: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
+00000f00: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000f10: 7072 6f70 616e 5b61 7379 6e63 2d73 7173  propan[async-sqs
+00000f20: 5d3b 2065 7874 7261 203d 3d20 2774 6573  ]; extra == 'tes
+00000f30: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
+00000f40: 3a20 7072 6f70 616e 5b64 6f63 5d3b 2065  : propan[doc]; e
+00000f50: 7874 7261 203d 3d20 2774 6573 7427 0a52  xtra == 'test'.R
+00000f60: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000f70: 7465 7374 2d61 7379 6e63 696f 3e3d 302e  test-asyncio>=0.
+00000f80: 3231 3b20 6578 7472 6120 3d3d 2027 7465  21; extra == 'te
+00000f90: 7374 270a 5265 7175 6972 6573 2d44 6973  st'.Requires-Dis
+00000fa0: 743a 2070 7974 6573 743e 3d37 3b20 6578  t: pytest>=7; ex
+00000fb0: 7472 6120 3d3d 2027 7465 7374 270a 5265  tra == 'test'.Re
+00000fc0: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
+00000fd0: 686f 6e2d 646f 7465 6e76 3b20 6578 7472  hon-dotenv; extr
+00000fe0: 6120 3d3d 2027 7465 7374 270a 4465 7363  a == 'test'.Desc
+00000ff0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00001000: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00001010: 6f77 6e0a 0a3c 7020 616c 6967 6e3d 2263  own..<p align="c
+00001020: 656e 7465 7222 3e0a 2020 2020 3c61 2068  enter">.    <a h
+00001030: 7265 663d 2268 7474 7073 3a2f 2f6c 616e  ref="https://lan
+00001040: 6365 746e 696b 2e67 6974 6875 622e 696f  cetnik.github.io
+00001050: 2f50 726f 7061 6e2f 2220 7461 7267 6574  /Propan/" target
 00001060: 3d22 5f62 6c61 6e6b 223e 0a20 2020 2020  ="_blank">.     
 00001070: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00001080: 7073 3a2f 2f63 6f76 6572 6167 652d 6261  ps://coverage-ba
-00001090: 6467 652e 7361 6d75 656c 636f 6c76 696e  dge.samuelcolvin
-000010a0: 2e77 6f72 6b65 7273 2e64 6576 2f6c 616e  .workers.dev/lan
-000010b0: 6365 746e 696b 2f70 726f 7061 6e2e 7376  cetnik/propan.sv
-000010c0: 6722 2061 6c74 3d22 436f 7665 7261 6765  g" alt="Coverage
-000010d0: 223e 0a20 2020 203c 2f61 3e0a 2020 2020  ">.    </a>.    
-000010e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000010f0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001100: 742f 7072 6f70 616e 2220 7461 7267 6574  t/propan" target
-00001110: 3d22 5f62 6c61 6e6b 223e 0a20 2020 2020  ="_blank">.     
-00001120: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00001130: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001140: 2e69 6f2f 7079 7069 2f76 2f70 726f 7061  .io/pypi/v/propa
-00001150: 6e3f 6c61 6265 6c3d 7079 7069 2532 3070  n?label=pypi%20p
-00001160: 6163 6b61 6765 2220 616c 743d 2250 6163  ackage" alt="Pac
-00001170: 6b61 6765 2076 6572 7369 6f6e 223e 0a20  kage version">. 
-00001180: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
-00001190: 7265 663d 2268 7474 7073 3a2f 2f70 6570  ref="https://pep
-000011a0: 792e 7465 6368 2f70 726f 6a65 6374 2f70  y.tech/project/p
-000011b0: 726f 7061 6e22 2074 6172 6765 743d 225f  ropan" target="_
-000011c0: 626c 616e 6b22 3e0a 2020 2020 2020 2020  blank">.        
-000011d0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000011e0: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
-000011f0: 6368 2f70 6572 736f 6e61 6c69 7a65 642d  ch/personalized-
-00001200: 6261 6467 652f 7072 6f70 616e 3f70 6572  badge/propan?per
-00001210: 696f 643d 746f 7461 6c26 756e 6974 733d  iod=total&units=
-00001220: 696e 7465 726e 6174 696f 6e61 6c5f 7379  international_sy
-00001230: 7374 656d 266c 6566 745f 636f 6c6f 723d  stem&left_color=
-00001240: 6772 6579 2672 6967 6874 5f63 6f6c 6f72  grey&right_color
-00001250: 3d62 6c75 6526 6c65 6674 5f74 6578 743d  =blue&left_text=
-00001260: 446f 776e 6c6f 6164 7322 2061 6c74 3d22  Downloads" alt="
-00001270: 646f 776e 6c6f 6164 7322 2f3e 0a20 2020  downloads"/>.   
-00001280: 203c 2f61 3e0a 2020 2020 3c62 722f 3e0a   </a>.    <br/>.
-00001290: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-000012a0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000012b0: 6f6a 6563 742f 7072 6f70 616e 2220 7461  oject/propan" ta
-000012c0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-000012d0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-000012e0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000012f0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-00001300: 6572 7369 6f6e 732f 7072 6f70 616e 2e73  ersions/propan.s
-00001310: 7667 2220 616c 743d 2253 7570 706f 7274  vg" alt="Support
-00001320: 6564 2050 7974 686f 6e20 7665 7273 696f  ed Python versio
-00001330: 6e73 223e 0a20 2020 203c 2f61 3e0a 2020  ns">.    </a>.  
-00001340: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00001350: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c61  ://github.com/La
-00001360: 6e63 6574 6e69 6b2f 5072 6f70 616e 2f62  ncetnik/Propan/b
-00001370: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
-00001380: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00001390: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-000013a0: 616c 743d 2247 6974 4875 6222 2073 7263  alt="GitHub" src
-000013b0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000013c0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000013d0: 6c69 6365 6e73 652f 4c61 6e63 6574 6e69  license/Lancetni
-000013e0: 6b2f 5072 6f70 616e 3f63 6f6c 6f72 3d25  k/Propan?color=%
-000013f0: 3233 3030 3765 6336 223e 0a20 2020 203c  23007ec6">.    <
-00001400: 2f61 3e0a 3c2f 703e 0a0a 2320 5072 6f70  /a>.</p>..# Prop
-00001410: 616e 0a0a 2a2a 5072 6f70 616e 2a2a 202d  an..**Propan** -
-00001420: 206a 7573 7420 2a7e 7e61 6e20 616e 6f74   just *~~an anot
-00001430: 6865 7220 6f6e 6520 4854 5450 7e7e 2a20  her one HTTP~~* 
-00001440: 6120 2a2a 6465 636c 6172 6174 6976 6520  a **declarative 
-00001450: 5079 7468 6f6e 204d 5120 6672 616d 6577  Python MQ framew
-00001460: 6f72 6b2a 2a2e 2049 7427 7320 666f 6c6c  ork**. It's foll
-00001470: 6f77 696e 6720 6279 203c 6120 6872 6566  owing by <a href
-00001480: 3d22 6874 7470 733a 2f2f 6661 7374 6170  ="https://fastap
-00001490: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f72  i.tiangolo.com/r
-000014a0: 752f 2220 7461 7267 6574 3d22 5f62 6c61  u/" target="_bla
-000014b0: 6e6b 223e 2a66 6173 7461 7069 2a3c 2f61  nk">*fastapi*</a
-000014c0: 3e2c 2073 696d 706c 6966 7920 4d65 7373  >, simplify Mess
-000014d0: 6167 6520 4272 6f6b 6572 7320 6172 6f75  age Brokers arou
-000014e0: 6e64 2063 6f64 6520 7772 6974 696e 6720  nd code writing 
-000014f0: 616e 6420 7072 6f76 6964 6573 2061 2068  and provides a h
-00001500: 656c 7066 756c 2064 6576 656c 6f70 6d65  elpful developme
-00001510: 6e74 2074 6f6f 6c6b 6974 2c20 7768 6963  nt toolkit, whic
-00001520: 6820 6578 6973 7465 6420 6f6e 6c79 2069  h existed only i
-00001530: 6e20 4854 5450 2d66 7261 6d65 776f 726b  n HTTP-framework
-00001540: 7320 776f 726c 6420 756e 7469 6c20 6e6f  s world until no
-00001550: 772e 0a0a 4974 2773 2064 6573 6967 6e65  w...It's designe
-00001560: 6420 746f 2063 7265 6174 6520 7265 6163  d to create reac
-00001570: 7469 7665 206d 6963 726f 7365 7276 6963  tive microservic
-00001580: 6573 2061 726f 756e 6420 3c61 2068 7265  es around <a hre
-00001590: 663d 2268 7474 7073 3a2f 2f6d 6963 726f  f="https://micro
-000015a0: 7365 7276 6963 6573 2e69 6f2f 7061 7474  services.io/patt
-000015b0: 6572 6e73 2f63 6f6d 6d75 6e69 6361 7469  erns/communicati
-000015c0: 6f6e 2d73 7479 6c65 2f6d 6573 7361 6769  on-style/messagi
-000015d0: 6e67 2e68 746d 6c22 2074 6172 6765 743d  ng.html" target=
-000015e0: 225f 626c 616e 6b22 3e4d 6573 7361 6769  "_blank">Messagi
-000015f0: 6e67 2041 7263 6869 7465 6374 7572 653c  ng Architecture<
-00001600: 2f61 3e2e 0a0a 4974 2069 7320 6120 6d6f  /a>...It is a mo
-00001610: 6465 726e 2c20 6869 6768 2d6c 6576 656c  dern, high-level
-00001620: 2066 7261 6d65 776f 726b 206f 6e20 746f   framework on to
-00001630: 7020 6f66 2070 6f70 756c 6172 2073 7065  p of popular spe
-00001640: 6369 6669 6320 5079 7468 6f6e 2062 726f  cific Python bro
-00001650: 6b65 7273 206c 6962 7261 7269 6573 2c20  kers libraries, 
-00001660: 6261 7365 6420 6f6e 203c 6120 6872 6566  based on <a href
-00001670: 3d22 6874 7470 733a 2f2f 646f 6373 2e70  ="https://docs.p
-00001680: 7964 616e 7469 632e 6465 762f 2220 7461  ydantic.dev/" ta
-00001690: 7267 6574 3d22 5f62 6c61 6e6b 223e 2a70  rget="_blank">*p
-000016a0: 7964 616e 7469 632a 3c2f 613e 2061 6e64  ydantic*</a> and
-000016b0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000016c0: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-000016d0: 6c6f 2e63 6f6d 2f72 752f 2220 7461 7267  lo.com/ru/" targ
-000016e0: 6574 3d22 5f62 6c61 6e6b 223e 2a66 6173  et="_blank">*fas
-000016f0: 7461 7069 2a3c 2f61 3e2c 203c 6120 6872  tapi*</a>, <a hr
-00001700: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
-00001710: 2e70 7974 6573 742e 6f72 672f 656e 2f6c  .pytest.org/en/l
-00001720: 6174 6573 742f 2220 7461 7267 6574 3d22  atest/" target="
-00001730: 5f62 6c61 6e6b 223e 2a70 7974 6573 742a  _blank">*pytest*
-00001740: 3c2f 613e 2063 6f6e 6365 7074 732e 0a0a  </a> concepts...
-00001750: 2d2d 2d0a 0a2a 2a44 6f63 756d 656e 7461  ---..**Documenta
-00001760: 7469 6f6e 2a2a 3a20 3c61 2068 7265 663d  tion**: <a href=
-00001770: 2268 7474 7073 3a2f 2f6c 616e 6365 746e  "https://lancetn
-00001780: 696b 2e67 6974 6875 622e 696f 2f50 726f  ik.github.io/Pro
-00001790: 7061 6e2f 2220 7461 7267 6574 3d22 5f62  pan/" target="_b
-000017a0: 6c61 6e6b 223e 6874 7470 733a 2f2f 6c61  lank">https://la
-000017b0: 6e63 6574 6e69 6b2e 6769 7468 7562 2e69  ncetnik.github.i
-000017c0: 6f2f 5072 6f70 616e 2f3c 2f61 3e0a 0a2d  o/Propan/</a>..-
-000017d0: 2d2d 0a0a 2323 2320 5468 6520 6b65 7920  --..### The key 
-000017e0: 6665 6174 7572 6573 2061 7265 0a0a 2a20  features are..* 
-000017f0: 2a2a 5369 6d70 6c65 2a2a 3a20 4465 7369  **Simple**: Desi
-00001800: 676e 6564 2074 6f20 6265 2065 6173 7920  gned to be easy 
-00001810: 746f 2075 7365 2061 6e64 206c 6561 726e  to use and learn
-00001820: 2e0a 2a20 2a2a 496e 7475 6974 6976 652a  ..* **Intuitive*
-00001830: 2a3a 2047 7265 6174 2065 6469 746f 7220  *: Great editor 
-00001840: 7375 7070 6f72 742e 2041 7574 6f63 6f6d  support. Autocom
-00001850: 706c 6574 696f 6e20 6576 6572 7977 6865  pletion everywhe
-00001860: 7265 2e0a 2a20 5b2a 2a44 6570 656e 6465  re..* [**Depende
-00001870: 6e63 6965 7320 6d61 6e61 6765 6d65 6e74  ncies management
-00001880: 2a2a 5d28 2364 6570 656e 6465 6e63 6965  **](#dependencie
-00001890: 7329 3a20 4d69 6e69 6d69 7a61 7469 6f6e  s): Minimization
-000018a0: 206f 6620 636f 6465 2064 7570 6c69 6361   of code duplica
-000018b0: 7469 6f6e 2e20 4163 6365 7373 2074 6f20  tion. Access to 
-000018c0: 6465 7065 6e64 656e 6369 6573 2061 7420  dependencies at 
-000018d0: 616e 7920 6c65 7665 6c20 6f66 2074 6865  any level of the
-000018e0: 2063 616c 6c20 7374 6163 6b2e 0a2a 205b   call stack..* [
-000018f0: 2a2a 496e 7465 6772 6174 696f 6e73 2a2a  **Integrations**
-00001900: 5d28 2368 7474 702d 6672 616d 6577 6f72  ](#http-framewor
-00001910: 6b73 2d69 6e74 6567 7261 7469 6f6e 7329  ks-integrations)
-00001920: 3a20 2a2a 5072 6f70 616e 2a2a 2069 7320  : **Propan** is 
-00001930: 6675 6c6c 7920 636f 6d70 6174 6962 6c65  fully compatible
-00001940: 2077 6974 6820 3c61 2068 7265 663d 2268   with <a href="h
-00001950: 7474 7073 3a2f 2f6c 616e 6365 746e 696b  ttps://lancetnik
-00001960: 2e67 6974 6875 622e 696f 2f50 726f 7061  .github.io/Propa
-00001970: 6e2f 696e 7465 6772 6174 696f 6e73 2f31  n/integrations/1
-00001980: 5f69 6e74 6567 7261 7469 6f6e 732d 696e  _integrations-in
-00001990: 6465 782f 2220 7461 7267 6574 3d22 5f62  dex/" target="_b
-000019a0: 6c61 6e6b 223e 616e 7920 4854 5450 2066  lank">any HTTP f
-000019b0: 7261 6d65 776f 726b 3c2f 613e 2079 6f75  ramework</a> you
-000019c0: 2077 616e 740a 2a20 2a2a 4d51 2069 6e64   want.* **MQ ind
-000019d0: 6570 656e 6465 6e74 2a2a 3a20 5369 6e67  ependent**: Sing
-000019e0: 6c65 2069 6e74 6572 6661 6365 2074 6f20  le interface to 
-000019f0: 706f 7075 6c61 7220 4d51 3a0a 2020 2a20  popular MQ:.  * 
-00001a00: 2a2a 5265 6469 732a 2a20 2862 6173 6564  **Redis** (based
-00001a10: 206f 6e20 3c61 2068 7265 663d 2268 7474   on <a href="htt
-00001a20: 7073 3a2f 2f72 6564 6973 2e72 6561 6474  ps://redis.readt
-00001a30: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00001a40: 626c 652f 696e 6465 782e 6874 6d6c 2220  ble/index.html" 
-00001a50: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00001a60: 7265 6469 732d 7079 3c2f 613e 290a 2020  redis-py</a>).  
-00001a70: 2a20 2a2a 5261 6262 6974 4d51 2a2a 2028  * **RabbitMQ** (
-00001a80: 6261 7365 6420 6f6e 203c 6120 6872 6566  based on <a href
-00001a90: 3d22 6874 7470 733a 2f2f 6169 6f2d 7069  ="https://aio-pi
-00001aa0: 6b61 2e72 6561 6474 6865 646f 6373 2e69  ka.readthedocs.i
-00001ab0: 6f2f 656e 2f6c 6174 6573 742f 2220 7461  o/en/latest/" ta
-00001ac0: 7267 6574 3d22 5f62 6c61 6e6b 223e 6169  rget="_blank">ai
-00001ad0: 6f2d 7069 6b61 3c2f 613e 290a 2020 2a20  o-pika</a>).  * 
-00001ae0: 2a2a 4b61 666b 612a 2a20 2862 6173 6564  **Kafka** (based
-00001af0: 206f 6e20 3c61 2068 7265 663d 2268 7474   on <a href="htt
-00001b00: 7073 3a2f 2f61 696f 6b61 666b 612e 7265  ps://aiokafka.re
-00001b10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00001b20: 7374 6162 6c65 2f22 2074 6172 6765 743d  stable/" target=
-00001b30: 225f 626c 616e 6b22 3e61 696f 6b61 666b  "_blank">aiokafk
-00001b40: 613c 2f61 3e29 0a20 202a 202a 2a53 5153  a</a>).  * **SQS
-00001b50: 2a2a 2028 6261 7365 6420 6f6e 203c 6120  ** (based on <a 
-00001b60: 6872 6566 3d22 6874 7470 733a 2f2f 6169  href="https://ai
-00001b70: 6f62 6f74 6f63 6f72 652e 7265 6164 7468  obotocore.readth
-00001b80: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001b90: 7374 2f22 2074 6172 6765 743d 225f 626c  st/" target="_bl
-00001ba0: 616e 6b22 3e61 696f 626f 746f 636f 7265  ank">aiobotocore
-00001bb0: 3c2f 613e 290a 2020 2a20 2a2a 4e61 7473  </a>).  * **Nats
-00001bc0: 2a2a 2028 6261 7365 6420 6f6e 203c 6120  ** (based on <a 
-00001bd0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001be0: 7468 7562 2e63 6f6d 2f6e 6174 732d 696f  thub.com/nats-io
-00001bf0: 2f6e 6174 732e 7079 2220 7461 7267 6574  /nats.py" target
-00001c00: 3d22 5f62 6c61 6e6b 223e 6e61 7473 2d70  ="_blank">nats-p
-00001c10: 793c 2f61 3e29 0a2a 203c 6120 6872 6566  y</a>).* <a href
-00001c20: 3d22 6874 7470 733a 2f2f 6c61 6e63 6574  ="https://lancet
-00001c30: 6e69 6b2e 6769 7468 7562 2e69 6f2f 5072  nik.github.io/Pr
-00001c40: 6f70 616e 2f67 6574 7469 6e67 5f73 7461  opan/getting_sta
-00001c50: 7274 6564 2f34 5f62 726f 6b65 722f 355f  rted/4_broker/5_
-00001c60: 7270 632f 2220 7461 7267 6574 3d22 5f62  rpc/" target="_b
-00001c70: 6c61 6e6b 223e 2a2a 5250 432a 2a3c 2f61  lank">**RPC**</a
-00001c80: 3e3a 2054 6865 2066 7261 6d65 776f 726b  >: The framework
-00001c90: 2073 7570 706f 7274 7320 5250 4320 7265   supports RPC re
-00001ca0: 7175 6573 7473 206f 7665 7220 4d51 2c20  quests over MQ, 
-00001cb0: 7768 6963 6820 7769 6c6c 2061 6c6c 6f77  which will allow
-00001cc0: 2070 6572 666f 726d 696e 6720 6c6f 6e67   performing long
-00001cd0: 206f 7065 7261 7469 6f6e 7320 6f6e 2072   operations on r
-00001ce0: 656d 6f74 6520 7365 7276 6963 6573 2061  emote services a
-00001cf0: 7379 6e63 6872 6f6e 6f75 736c 792e 0a2a  synchronously..*
-00001d00: 205b 2a2a 4772 6561 7420 746f 2064 6576   [**Great to dev
-00001d10: 656c 6f70 2a2a 5d28 2363 6c69 2d70 6f77  elop**](#cli-pow
-00001d20: 6572 293a 2043 4c49 2074 6f6f 6c20 7072  er): CLI tool pr
-00001d30: 6f76 6964 6573 2067 7265 6174 2064 6576  ovides great dev
-00001d40: 656c 6f70 6d65 6e74 2065 7870 6572 6965  elopment experie
-00001d50: 6e63 653a 0a20 202a 2066 7261 6d65 776f  nce:.  * framewo
-00001d60: 726b 2d69 6e64 6570 656e 6465 6e74 2077  rk-independent w
-00001d70: 6179 2074 6f20 6d61 6e61 6765 2074 6865  ay to manage the
-00001d80: 2070 726f 6a65 6374 2065 6e76 6972 6f6e   project environ
-00001d90: 6d65 6e74 0a20 202a 2061 7070 6c69 6361  ment.  * applica
-00001da0: 7469 6f6e 2063 6f64 6520 2a68 6f74 2072  tion code *hot r
-00001db0: 656c 6f61 642a 0a20 202a 2072 6f62 7573  eload*.  * robus
-00001dc0: 7420 6170 706c 6963 6174 696f 6e20 7465  t application te
-00001dd0: 6d70 6c61 7465 730a 2a20 3c61 2068 7265  mplates.* <a hre
-00001de0: 663d 2268 7474 7073 3a2f 2f6c 616e 6365  f="https://lance
-00001df0: 746e 696b 2e67 6974 6875 622e 696f 2f50  tnik.github.io/P
-00001e00: 726f 7061 6e2f 6765 7474 696e 675f 7374  ropan/getting_st
-00001e10: 6172 7465 642f 375f 7465 7374 696e 6722  arted/7_testing"
-00001e20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001e30: 3e2a 2a54 6573 7461 6269 6c69 7479 2a2a  >**Testability**
-00001e40: 3c2f 613e 3a20 2a2a 5072 6f70 616e 2a2a  </a>: **Propan**
-00001e50: 2061 6c6c 6f77 7320 796f 7520 746f 2074   allows you to t
-00001e60: 6573 7420 796f 7572 2061 7070 2077 6974  est your app wit
-00001e70: 686f 7574 2065 7874 6572 6e61 6c20 6465  hout external de
-00001e80: 7065 6e64 656e 6369 6573 3a20 796f 7520  pendencies: you 
-00001e90: 646f 206e 6f74 2068 6176 6520 746f 2073  do not have to s
-00001ea0: 6574 2075 7020 6120 4d65 7373 6167 6520  et up a Message 
-00001eb0: 4272 6f6b 6572 2c20 796f 7520 6361 6e20  Broker, you can 
-00001ec0: 7573 6520 6120 7669 7274 7561 6c20 6f6e  use a virtual on
-00001ed0: 6521 0a0a 2323 2320 5375 7070 6f72 7465  e!..### Supporte
-00001ee0: 6420 4d51 2062 726f 6b65 7273 0a0a 7c20  d MQ brokers..| 
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 7c20 6173 796e 6320 2020 2020 2020    | async       
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 2020 2020 2020 2020 2020 2020 7c20 7379              | sy
-00001f40: 6e63 2020 2020 2020 2020 2020 2020 2020  nc              
-00001f50: 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d     |.|----------
-00001f60: 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  ---------|:-----
-00001f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001fa0: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
-00001fb0: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2a2a  ---------:|.| **
-00001fc0: 5261 6262 6974 4d51 2a2a 2020 2020 2020  RabbitMQ**      
-00001fd0: 7c20 3a68 6561 7679 5f63 6865 636b 5f6d  | :heavy_check_m
-00001fe0: 6172 6b3a 202a 2a73 7461 626c 652a 2a20  ark: **stable** 
-00001ff0: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
-00002000: 6b3a 2020 2020 2020 2020 7c20 3a6d 6167  k:        | :mag
-00002010: 3a20 706c 616e 6e69 6e67 203a 6d61 673a  : planning :mag:
-00002020: 207c 0a7c 202a 2a52 6564 6973 2a2a 2020   |.| **Redis**  
-00002030: 2020 2020 2020 207c 203a 6865 6176 795f         | :heavy_
-00002040: 6368 6563 6b5f 6d61 726b 3a20 2a2a 7374  check_mark: **st
-00002050: 6162 6c65 2a2a 203a 6865 6176 795f 6368  able** :heavy_ch
-00002060: 6563 6b5f 6d61 726b 3a20 2020 2020 2020  eck_mark:       
-00002070: 207c 203a 6d61 673a 2070 6c61 6e6e 696e   | :mag: plannin
-00002080: 6720 3a6d 6167 3a20 7c0a 7c20 2a2a 4e61  g :mag: |.| **Na
-00002090: 7473 2a2a 2020 2020 2020 2020 2020 7c20  ts**          | 
-000020a0: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
-000020b0: 6b3a 202a 2a73 7461 626c 652a 2a20 3a68  k: **stable** :h
-000020c0: 6561 7679 5f63 6865 636b 5f6d 6172 6b3a  eavy_check_mark:
-000020d0: 2020 2020 2020 2020 7c20 3a6d 6167 3a20          | :mag: 
-000020e0: 706c 616e 6e69 6e67 203a 6d61 673a 207c  planning :mag: |
-000020f0: 0a7c 202a 2a4b 6166 6b61 2a2a 2020 2020  .| **Kafka**    
-00002100: 2020 2020 207c 203a 7761 726e 696e 673a       | :warning:
-00002110: 202a 2a62 6574 612a 2a20 3a77 6172 6e69   **beta** :warni
-00002120: 6e67 3a20 2020 2020 2020 2020 2020 2020  ng:             
-00002130: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00002140: 203a 6d61 673a 2070 6c61 6e6e 696e 6720   :mag: planning 
-00002150: 3a6d 6167 3a20 7c0a 7c20 2a2a 5351 532a  :mag: |.| **SQS*
-00002160: 2a20 2020 2020 2020 2020 2020 7c20 3a77  *           | :w
-00002170: 6172 6e69 6e67 3a20 2a2a 6265 7461 2a2a  arning: **beta**
-00002180: 203a 7761 726e 696e 673a 2020 2020 2020   :warning:      
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2020 2020 2020 7c20 3a6d 6167 3a20 706c        | :mag: pl
-000021b0: 616e 6e69 6e67 203a 6d61 673a 207c 0a7c  anning :mag: |.|
-000021c0: 202a 2a4e 6174 734a 532a 2a20 2020 2020   **NatsJS**     
-000021d0: 2020 207c 203a 6861 6d6d 6572 5f61 6e64     | :hammer_and
-000021e0: 5f77 7265 6e63 683a 202a 2a69 6e20 7072  _wrench: **in pr
-000021f0: 6f67 7265 7373 2a2a 203a 6861 6d6d 6572  ogress** :hammer
-00002200: 5f61 6e64 5f77 7265 6e63 683a 207c 203a  _and_wrench: | :
-00002210: 6d61 673a 2070 6c61 6e6e 696e 6720 3a6d  mag: planning :m
-00002220: 6167 3a20 7c0a 7c20 2a2a 4d51 5454 2a2a  ag: |.| **MQTT**
-00002230: 2020 2020 2020 2020 2020 7c20 3a6d 6167            | :mag
-00002240: 3a20 706c 616e 6e69 6e67 203a 6d61 673a  : planning :mag:
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 7c20 3a6d 6167 3a20 706c 616e      | :mag: plan
-00002280: 6e69 6e67 203a 6d61 673a 207c 0a7c 202a  ning :mag: |.| *
-00002290: 2a52 6564 6973 2053 7472 6561 6d73 2a2a  *Redis Streams**
-000022a0: 207c 203a 6d61 673a 2070 6c61 6e6e 696e   | :mag: plannin
-000022b0: 6720 3a6d 6167 3a20 2020 2020 2020 2020  g :mag:         
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2020 2020 2020 2020 207c 203a 6d61             | :ma
-000022e0: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
-000022f0: 3a20 7c0a 7c20 2a2a 5075 6c73 6172 2a2a  : |.| **Pulsar**
-00002300: 2020 2020 2020 2020 7c20 3a6d 6167 3a20          | :mag: 
-00002310: 706c 616e 6e69 6e67 203a 6d61 673a 2020  planning :mag:  
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 7c20 3a6d 6167 3a20 706c 616e 6e69    | :mag: planni
-00002350: 6e67 203a 6d61 673a 207c 0a0a 2323 2320  ng :mag: |..### 
-00002360: 436f 6d6d 756e 6974 790a 0a49 6620 796f  Community..If yo
-00002370: 7520 6172 6520 696e 7465 7265 7374 6564  u are interested
-00002380: 2069 6e20 7468 6973 2070 726f 6a65 6374   in this project
-00002390: 2c20 706c 6561 7365 2067 6976 6520 6d65  , please give me
-000023a0: 2066 6565 6462 6163 6b20 6279 2073 7461   feedback by sta
-000023b0: 7220 6f72 2f61 6e64 2077 6174 6368 2072  r or/and watch r
-000023c0: 6570 6f73 6974 6f72 792e 0a0a 4966 2079  epository...If y
-000023d0: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
-000023e0: 7469 6f6e 7320 6f72 2069 6465 6173 2061  tions or ideas a
-000023f0: 626f 7574 2066 6561 7475 7265 7320 746f  bout features to
-00002400: 2069 6d70 6c65 6d65 6e74 2c20 7765 6c63   implement, welc
-00002410: 6f6d 6520 746f 205b 6469 7363 7573 7369  ome to [discussi
-00002420: 6f6e 735d 2868 7474 7073 3a2f 2f67 6974  ons](https://git
-00002430: 6875 622e 636f 6d2f 4c61 6e63 6574 6e69  hub.com/Lancetni
-00002440: 6b2f 5072 6f70 616e 2f64 6973 6375 7373  k/Propan/discuss
-00002450: 696f 6e73 292e 0a0a 2d2d 2d0a 0a23 2320  ions)...---..## 
-00002460: 4465 636c 6172 6174 6976 653f 0a0a 5769  Declarative?..Wi
-00002470: 7468 2064 6563 6c61 7261 7469 7665 2074  th declarative t
-00002480: 6f6f 6c73 2079 6f75 2063 616e 2064 6566  ools you can def
-00002490: 696e 6520 2a2a 7768 6174 2079 6f75 206e  ine **what you n
-000024a0: 6565 6420 746f 2067 6574 2a2a 2e20 5769  eed to get**. Wi
-000024b0: 7468 2074 7261 6469 7469 6f6e 616c 2069  th traditional i
-000024c0: 6d70 6572 6174 6976 6520 746f 6f6c 7320  mperative tools 
-000024d0: 796f 7520 6d75 7374 2077 7269 7465 202a  you must write *
-000024e0: 2a77 6861 7420 796f 7520 6e65 6564 2074  *what you need t
-000024f0: 6f20 646f 2a2a 2e0a 0a54 616b 6520 6120  o do**...Take a 
-00002500: 6c6f 6f6b 2061 7420 636c 6173 7369 6320  look at classic 
-00002510: 696d 7065 7261 7469 7665 2074 6f6f 6c73  imperative tools
-00002520: 2c20 7375 6368 2061 7320 3c61 2068 7265  , such as <a hre
-00002530: 663d 2268 7474 7073 3a2f 2f61 696f 2d70  f="https://aio-p
-00002540: 696b 612e 7265 6164 7468 6564 6f63 732e  ika.readthedocs.
-00002550: 696f 2f65 6e2f 6c61 7465 7374 2f22 2074  io/en/latest/" t
-00002560: 6172 6765 743d 225f 626c 616e 6b22 3e61  arget="_blank">a
-00002570: 696f 2d70 696b 613c 2f61 3e2c 203c 6120  io-pika</a>, <a 
-00002580: 6872 6566 3d22 6874 7470 733a 2f2f 7069  href="https://pi
-00002590: 6b61 2e72 6561 6474 6865 646f 6373 2e69  ka.readthedocs.i
-000025a0: 6f2f 656e 2f73 7461 626c 652f 2220 7461  o/en/stable/" ta
-000025b0: 7267 6574 3d22 5f62 6c61 6e6b 223e 7069  rget="_blank">pi
-000025c0: 6b61 3c2f 613e 2c20 3c61 2068 7265 663d  ka</a>, <a href=
-000025d0: 2268 7474 7073 3a2f 2f72 6564 6973 2e72  "https://redis.r
-000025e0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000025f0: 2f73 7461 626c 652f 696e 6465 782e 6874  /stable/index.ht
-00002600: 6d6c 2220 7461 7267 6574 3d22 5f62 6c61  ml" target="_bla
-00002610: 6e6b 223e 7265 6469 732d 7079 3c2f 613e  nk">redis-py</a>
-00002620: 2c20 3c61 2068 7265 663d 2268 7474 7073  , <a href="https
-00002630: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-00002640: 7473 2d69 6f2f 6e61 7473 2e70 7922 2074  ts-io/nats.py" t
-00002650: 6172 6765 743d 225f 626c 616e 6b22 3e6e  arget="_blank">n
-00002660: 6174 732d 7079 3c2f 613e 2c20 6574 632e  ats-py</a>, etc.
-00002670: 0a0a 5468 6973 2069 7320 7468 6520 2a2a  ..This is the **
-00002680: 5175 6963 6b73 7461 7274 2a2a 2077 6974  Quickstart** wit
-00002690: 6820 7468 6520 2a61 696f 2d70 696b 612a  h the *aio-pika*
-000026a0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
-000026b0: 6f72 7420 6173 796e 6369 6f0a 696d 706f  ort asyncio.impo
-000026c0: 7274 2061 696f 5f70 696b 610a 0a61 7379  rt aio_pika..asy
-000026d0: 6e63 2064 6566 206d 6169 6e28 293a 0a20  nc def main():. 
-000026e0: 2020 2063 6f6e 6e65 6374 696f 6e20 3d20     connection = 
-000026f0: 6177 6169 7420 6169 6f5f 7069 6b61 2e63  await aio_pika.c
-00002700: 6f6e 6e65 6374 5f72 6f62 7573 7428 0a20  onnect_robust(. 
-00002710: 2020 2020 2020 2022 616d 7170 3a2f 2f67         "amqp://g
-00002720: 7565 7374 3a67 7565 7374 4031 3237 2e30  uest:guest@127.0
-00002730: 2e30 2e31 2f22 0a20 2020 2029 0a0a 2020  .0.1/".    )..  
-00002740: 2020 7175 6575 655f 6e61 6d65 203d 2022    queue_name = "
-00002750: 7465 7374 5f71 7565 7565 220a 0a20 2020  test_queue"..   
-00002760: 2061 7379 6e63 2077 6974 6820 636f 6e6e   async with conn
-00002770: 6563 7469 6f6e 3a0a 2020 2020 2020 2020  ection:.        
-00002780: 6368 616e 6e65 6c20 3d20 6177 6169 7420  channel = await 
-00002790: 636f 6e6e 6563 7469 6f6e 2e63 6861 6e6e  connection.chann
-000027a0: 656c 2829 0a0a 2020 2020 2020 2020 7175  el()..        qu
-000027b0: 6575 6520 3d20 6177 6169 7420 6368 616e  eue = await chan
-000027c0: 6e65 6c2e 6465 636c 6172 655f 7175 6575  nel.declare_queu
-000027d0: 6528 7175 6575 655f 6e61 6d65 290a 0a20  e(queue_name).. 
-000027e0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-000027f0: 6820 7175 6575 652e 6974 6572 6174 6f72  h queue.iterator
-00002800: 2829 2061 7320 7175 6575 655f 6974 6572  () as queue_iter
-00002810: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-00002820: 796e 6320 666f 7220 6d65 7373 6167 6520  ync for message 
-00002830: 696e 2071 7565 7565 5f69 7465 723a 0a20  in queue_iter:. 
-00002840: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00002850: 7379 6e63 2077 6974 6820 6d65 7373 6167  sync with messag
-00002860: 652e 7072 6f63 6573 7328 293a 0a20 2020  e.process():.   
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2070 7269 6e74 286d 6573 7361 6765 2e62   print(message.b
-00002890: 6f64 7929 0a0a 6173 796e 6369 6f2e 7275  ody)..asyncio.ru
-000028a0: 6e28 6d61 696e 2829 290a 6060 600a 0a2a  n(main()).```..*
-000028b0: 2a61 696f 2d70 696b 612a 2a20 6973 2061  *aio-pika** is a
-000028c0: 2067 7265 6174 2074 6f6f 6c20 7769 7468   great tool with
-000028d0: 2061 2072 6561 6c6c 7920 6561 7379 206c   a really easy l
-000028e0: 6561 726e 696e 6720 6375 7276 652e 2042  earning curve. B
-000028f0: 7574 2069 7427 7320 7374 696c 6c20 696d  ut it's still im
-00002900: 7065 7261 7469 7665 2e20 596f 7520 6e65  perative. You ne
-00002910: 6564 2074 6f20 2a63 6f6e 6e65 6374 2a2c  ed to *connect*,
-00002920: 2064 6563 6c61 7265 202a 6368 616e 6e65   declare *channe
-00002930: 6c2a 2c20 2a71 7565 7565 732a 2c20 2a65  l*, *queues*, *e
-00002940: 7863 6861 6e67 6573 2a20 6279 2079 6f75  xchanges* by you
-00002950: 7273 656c 662e 2041 6c73 6f2c 2079 6f75  rself. Also, you
-00002960: 206e 6565 6420 746f 206d 616e 6167 6520   need to manage 
-00002970: 2a63 6f6e 6e65 6374 696f 6e2a 2c20 2a6d  *connection*, *m
-00002980: 6573 7361 6765 2a2c 202a 7175 6575 652a  essage*, *queue*
-00002990: 2063 6f6e 7465 7874 2074 6f20 6176 6f69   context to avoi
-000029a0: 6420 616e 7920 7472 6f75 626c 6573 2e0a  d any troubles..
-000029b0: 0a49 7420 6973 206e 6f74 2061 2062 6164  .It is not a bad
-000029c0: 2077 6179 2c20 6275 7420 6974 2063 616e   way, but it can
-000029d0: 2062 6520 6d75 6368 2065 6173 6965 722e   be much easier.
-000029e0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000029f0: 2070 726f 7061 6e20 696d 706f 7274 2050   propan import P
-00002a00: 726f 7061 6e41 7070 2c20 5261 6262 6974  ropanApp, Rabbit
-00002a10: 4272 6f6b 6572 0a0a 6272 6f6b 6572 203d  Broker..broker =
-00002a20: 2052 6162 6269 7442 726f 6b65 7228 2261   RabbitBroker("a
-00002a30: 6d71 703a 2f2f 6775 6573 743a 6775 6573  mqp://guest:gues
-00002a40: 7440 6c6f 6361 6c68 6f73 743a 3536 3732  t@localhost:5672
-00002a50: 2f22 290a 0a61 7070 203d 2050 726f 7061  /")..app = Propa
-00002a60: 6e41 7070 2862 726f 6b65 7229 0a0a 4062  nApp(broker)..@b
-00002a70: 726f 6b65 722e 6861 6e64 6c65 2822 7465  roker.handle("te
-00002a80: 7374 5f71 7565 7565 2229 0a61 7379 6e63  st_queue").async
-00002a90: 2064 6566 2062 6173 655f 6861 6e64 6c65   def base_handle
-00002aa0: 7228 626f 6479 293a 0a20 2020 2070 7269  r(body):.    pri
-00002ab0: 6e74 2862 6f64 7929 0a60 6060 0a0a 5468  nt(body).```..Th
-00002ac0: 6973 2069 7320 7468 6520 2a2a 5072 6f70  is is the **Prop
-00002ad0: 616e 2a2a 2064 6563 6c61 7261 7469 7665  an** declarative
-00002ae0: 2077 6179 2074 6f20 7772 6974 6520 7468   way to write th
-00002af0: 6520 7361 6d65 2063 6f64 652e 2054 6861  e same code. Tha
-00002b00: 7420 6973 2073 6f20 6d75 6368 2065 6173  t is so much eas
-00002b10: 6965 722c 2069 736e 2774 2069 743f 0a0a  ier, isn't it?..
-00002b20: 2d2d 2d0a 0a23 2320 5175 6963 6b73 7461  ---..## Quicksta
-00002b30: 7274 0a0a 496e 7374 616c 6c20 7573 696e  rt..Install usin
-00002b40: 6720 6070 6970 603a 0a0a 6060 6073 6865  g `pip`:..```she
-00002b50: 6c6c 0a70 6970 2069 6e73 7461 6c6c 2022  ll.pip install "
-00002b60: 7072 6f70 616e 5b61 7379 6e63 2d72 6162  propan[async-rab
-00002b70: 6269 745d 220a 2320 6f72 0a70 6970 2069  bit]".# or.pip i
-00002b80: 6e73 7461 6c6c 2022 7072 6f70 616e 5b61  nstall "propan[a
-00002b90: 7379 6e63 2d6e 6174 735d 220a 2320 6f72  sync-nats]".# or
-00002ba0: 0a70 6970 2069 6e73 7461 6c6c 2022 7072  .pip install "pr
-00002bb0: 6f70 616e 5b61 7379 6e63 2d72 6564 6973  opan[async-redis
-00002bc0: 5d22 0a23 206f 720a 7069 7020 696e 7374  ]".# or.pip inst
-00002bd0: 616c 6c20 2270 726f 7061 6e5b 6173 796e  all "propan[asyn
-00002be0: 632d 6b61 666b 615d 220a 2320 6f72 0a70  c-kafka]".# or.p
-00002bf0: 6970 2069 6e73 7461 6c6c 2022 7072 6f70  ip install "prop
-00002c00: 616e 5b61 7379 6e63 2d73 7173 5d22 0a60  an[async-sqs]".`
-00002c10: 6060 0a0a 2323 2320 4261 7369 6320 7573  ``..### Basic us
-00002c20: 6167 650a 0a43 7265 6174 6520 616e 2061  age..Create an a
-00002c30: 7070 6c69 6361 7469 6f6e 2077 6974 6820  pplication with 
-00002c40: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00002c50: 6465 2061 7420 6073 6572 7665 2e70 7960  de at `serve.py`
-00002c60: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-00002c70: 6d20 7072 6f70 616e 2069 6d70 6f72 7420  m propan import 
-00002c80: 5072 6f70 616e 4170 700a 6672 6f6d 2070  PropanApp.from p
-00002c90: 726f 7061 6e20 696d 706f 7274 2052 6162  ropan import Rab
-00002ca0: 6269 7442 726f 6b65 720a 2320 6672 6f6d  bitBroker.# from
-00002cb0: 2070 726f 7061 6e20 696d 706f 7274 2052   propan import R
-00002cc0: 6564 6973 4272 6f6b 6572 0a23 2066 726f  edisBroker.# fro
-00002cd0: 6d20 7072 6f70 616e 2069 6d70 6f72 7420  m propan import 
-00002ce0: 4e61 7473 4272 6f6b 6572 0a23 2066 726f  NatsBroker.# fro
-00002cf0: 6d20 7072 6f70 616e 2069 6d70 6f72 7420  m propan import 
-00002d00: 5351 5342 726f 6b65 720a 2320 6672 6f6d  SQSBroker.# from
-00002d10: 2070 726f 7061 6e20 696d 706f 7274 204b   propan import K
-00002d20: 6166 6b61 4272 6f6b 6572 0a0a 6272 6f6b  afkaBroker..brok
-00002d30: 6572 203d 2052 6162 6269 7442 726f 6b65  er = RabbitBroke
-00002d40: 7228 2261 6d71 703a 2f2f 6775 6573 743a  r("amqp://guest:
-00002d50: 6775 6573 7440 6c6f 6361 6c68 6f73 743a  guest@localhost:
-00002d60: 3536 3732 2f22 290a 2320 6272 6f6b 6572  5672/").# broker
-00002d70: 203d 204e 6174 7342 726f 6b65 7228 226e   = NatsBroker("n
-00002d80: 6174 733a 2f2f 6c6f 6361 6c68 6f73 743a  ats://localhost:
-00002d90: 3432 3232 2229 0a23 2062 726f 6b65 7220  4222").# broker 
-00002da0: 3d20 5265 6469 7342 726f 6b65 7228 2272  = RedisBroker("r
-00002db0: 6564 6973 3a2f 2f6c 6f63 616c 686f 7374  edis://localhost
-00002dc0: 3a36 3337 3922 290a 2320 6272 6f6b 6572  :6379").# broker
-00002dd0: 203d 2053 5153 4272 6f6b 6572 2822 6874   = SQSBroker("ht
-00002de0: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a39  tp://localhost:9
-00002df0: 3332 3422 2c20 2e2e 2e29 0a23 2062 726f  324", ...).# bro
-00002e00: 6b65 7220 3d20 4b61 666b 6142 726f 6b65  ker = KafkaBroke
-00002e10: 7228 226c 6f63 616c 686f 7374 3a39 3039  r("localhost:909
-00002e20: 3222 290a 0a61 7070 203d 2050 726f 7061  2")..app = Propa
-00002e30: 6e41 7070 2862 726f 6b65 7229 0a0a 4062  nApp(broker)..@b
-00002e40: 726f 6b65 722e 6861 6e64 6c65 2822 7465  roker.handle("te
-00002e50: 7374 2229 0a61 7379 6e63 2064 6566 2062  st").async def b
-00002e60: 6173 655f 6861 6e64 6c65 7228 626f 6479  ase_handler(body
-00002e70: 293a 0a20 2020 2027 2727 4861 6e64 6c65  ):.    '''Handle
-00002e80: 2061 6c6c 2064 6566 6175 6c74 2065 7863   all default exc
-00002e90: 6861 6e67 6520 6d65 7373 6167 6573 2077  hange messages w
-00002ea0: 6974 6820 6074 6573 7460 2072 6f75 7469  ith `test` routi
-00002eb0: 6e67 206b 6579 2727 270a 2020 2020 7072  ng key'''.    pr
-00002ec0: 696e 7428 626f 6479 290a 6060 600a 0a41  int(body).```..A
-00002ed0: 6e64 206a 7573 7420 7275 6e20 6974 3a0a  nd just run it:.
-00002ee0: 0a60 6060 7368 656c 6c0a 7072 6f70 616e  .```shell.propan
-00002ef0: 2072 756e 2073 6572 7665 3a61 7070 0a60   run serve:app.`
-00002f00: 6060 0a0a 2d2d 2d0a 0a23 2320 5479 7065  ``..---..## Type
-00002f10: 2063 6173 7469 6e67 0a0a 5072 6f70 616e   casting..Propan
-00002f20: 2075 7365 7320 6070 7964 616e 7469 6360   uses `pydantic`
-00002f30: 2074 6f20 6361 7374 2069 6e63 6f6d 696e   to cast incomin
-00002f40: 6720 6675 6e63 7469 6f6e 2061 7267 756d  g function argum
-00002f50: 656e 7473 2074 6f20 7479 7065 7320 6163  ents to types ac
-00002f60: 636f 7264 696e 6720 746f 2074 6865 6972  cording to their
-00002f70: 2061 6e6e 6f74 6174 696f 6e2e 0a0a 6060   annotation...``
-00002f80: 6070 7974 686f 6e0a 6672 6f6d 2070 7964  `python.from pyd
-00002f90: 616e 7469 6320 696d 706f 7274 2042 6173  antic import Bas
-00002fa0: 654d 6f64 656c 0a66 726f 6d20 7072 6f70  eModel.from prop
-00002fb0: 616e 2069 6d70 6f72 7420 5072 6f70 616e  an import Propan
-00002fc0: 4170 702c 2043 6f6e 7465 7874 2c20 5261  App, Context, Ra
-00002fd0: 6262 6974 4272 6f6b 6572 0a0a 6272 6f6b  bbitBroker..brok
-00002fe0: 6572 203d 2052 6162 6269 7442 726f 6b65  er = RabbitBroke
-00002ff0: 7228 2261 6d71 703a 2f2f 6775 6573 743a  r("amqp://guest:
-00003000: 6775 6573 7440 6c6f 6361 6c68 6f73 743a  guest@localhost:
-00003010: 3536 3732 2f22 290a 6170 7020 3d20 5072  5672/").app = Pr
-00003020: 6f70 616e 4170 7028 6272 6f6b 6572 290a  opanApp(broker).
-00003030: 0a63 6c61 7373 2053 696d 706c 654d 6573  .class SimpleMes
-00003040: 7361 6765 2842 6173 654d 6f64 656c 293a  sage(BaseModel):
-00003050: 0a20 2020 206b 6579 3a20 696e 740a 0a40  .    key: int..@
-00003060: 6272 6f6b 6572 2e68 616e 646c 6528 2274  broker.handle("t
-00003070: 6573 7432 2229 0a61 7379 6e63 2064 6566  est2").async def
-00003080: 2073 6563 6f6e 645f 6861 6e64 6c65 7228   second_handler(
-00003090: 626f 6479 3a20 5369 6d70 6c65 4d65 7373  body: SimpleMess
-000030a0: 6167 6529 3a0a 2020 2020 6173 7365 7274  age):.    assert
-000030b0: 2069 7369 6e73 7461 6e63 6528 626f 6479   isinstance(body
-000030c0: 2e6b 6579 2c20 696e 7429 0a0a 6060 600a  .key, int)..```.
-000030d0: 0a2d 2d2d 0a0a 2323 2044 6570 656e 6465  .---..## Depende
-000030e0: 6e63 6965 730a 0a2a 2a50 726f 7061 6e2a  ncies..**Propan*
-000030f0: 2a20 6120 6861 7320 6465 7065 6e64 656e  * a has dependen
-00003100: 6369 6573 206d 616e 6167 656d 656e 7420  cies management 
-00003110: 706f 6c69 6379 2063 6c6f 7365 2074 6f20  policy close to 
-00003120: 6070 7974 6573 7420 6669 7874 7572 6573  `pytest fixtures
-00003130: 602e 0a59 6f75 2063 616e 2073 7065 6369  `..You can speci
-00003140: 6679 2069 6e20 6675 6e63 7469 6f6e 7320  fy in functions 
-00003150: 6172 6775 6d65 6e74 7320 7768 6963 6820  arguments which 
-00003160: 6465 7065 6e64 656e 6369 6573 0a79 6f75  dependencies.you
-00003170: 2077 6f75 6c64 2074 6f20 7573 652e 2046   would to use. F
-00003180: 7261 6d65 776f 726b 2070 6173 7365 7320  ramework passes 
-00003190: 7468 656d 2066 726f 6d20 7468 6520 676c  them from the gl
-000031a0: 6f62 616c 2043 6f6e 7465 7874 206f 626a  obal Context obj
-000031b0: 6563 742e 0a0a 416c 7265 6164 7920 6578  ect...Already ex
-000031c0: 6973 7465 6420 636f 6e74 6578 7420 6669  isted context fi
-000031d0: 656c 6473 2061 7265 3a20 2a61 7070 2a2c  elds are: *app*,
-000031e0: 202a 6272 6f6b 6572 2a2c 202a 636f 6e74   *broker*, *cont
-000031f0: 6578 742a 2028 6974 7365 6c66 292c 202a  ext* (itself), *
-00003200: 6c6f 6767 6572 2a20 616e 6420 2a6d 6573  logger* and *mes
-00003210: 7361 6765 2a2e 0a49 6620 796f 7520 6361  sage*..If you ca
-00003220: 6c6c 206e 6f74 2065 7869 7374 696e 6720  ll not existing 
-00003230: 6669 656c 642c 2072 6169 7365 7320 2a70  field, raises *p
-00003240: 7964 616e 7469 632e 5661 6c69 6461 7469  ydantic.Validati
-00003250: 6f6e 4572 726f 722a 2076 616c 7565 2e0a  onError* value..
-00003260: 0a42 7574 2079 6f75 2063 616e 2073 7065  .But you can spe
-00003270: 6369 6679 2079 6f75 7220 6f77 6e20 6465  cify your own de
-00003280: 7065 6e64 656e 6369 6573 2c20 6361 6c6c  pendencies, call
-00003290: 2064 6570 656e 6465 6e63 6965 7320 6675   dependencies fu
-000032a0: 6e63 7469 6f6e 7320 286c 696b 6520 6046  nctions (like `F
-000032b0: 6173 7461 7069 2044 6570 656e 6473 6029  astapi Depends`)
-000032c0: 0a61 6e64 205b 6d6f 7265 5d28 6874 7470  .and [more](http
-000032d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
-000032e0: 616e 6365 746e 696b 2f50 726f 7061 6e2f  ancetnik/Propan/
-000032f0: 7472 6565 2f6d 6169 6e2f 6578 616d 706c  tree/main/exampl
-00003300: 6573 2f64 6570 656e 6465 6e63 6965 7329  es/dependencies)
-00003310: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
-00003320: 6f72 7420 6169 6f5f 7069 6b61 0a66 726f  ort aio_pika.fro
-00003330: 6d20 7072 6f70 616e 2069 6d70 6f72 7420  m propan import 
-00003340: 5072 6f70 616e 4170 702c 2052 6162 6269  PropanApp, Rabbi
-00003350: 7442 726f 6b65 722c 2043 6f6e 7465 7874  tBroker, Context
-00003360: 2c20 4465 7065 6e64 730a 0a72 6162 6269  , Depends..rabbi
-00003370: 745f 6272 6f6b 6572 203d 2052 6162 6269  t_broker = Rabbi
-00003380: 7442 726f 6b65 7228 2261 6d71 703a 2f2f  tBroker("amqp://
-00003390: 6775 6573 743a 6775 6573 7440 6c6f 6361  guest:guest@loca
-000033a0: 6c68 6f73 743a 3536 3732 2f22 290a 0a61  lhost:5672/")..a
-000033b0: 7070 203d 2050 726f 7061 6e41 7070 2872  pp = PropanApp(r
-000033c0: 6162 6269 745f 6272 6f6b 6572 290a 0a61  abbit_broker)..a
-000033d0: 7379 6e63 2064 6566 2064 6570 656e 6465  sync def depende
-000033e0: 6e63 7928 626f 6479 3a20 6469 6374 2920  ncy(body: dict) 
-000033f0: 2d3e 2062 6f6f 6c3a 0a20 2020 2072 6574  -> bool:.    ret
-00003400: 7572 6e20 5472 7565 0a0a 4072 6162 6269  urn True..@rabbi
-00003410: 745f 6272 6f6b 6572 2e68 616e 646c 6528  t_broker.handle(
-00003420: 2274 6573 7422 290a 6173 796e 6320 6465  "test").async de
-00003430: 6620 6261 7365 5f68 616e 646c 6572 2862  f base_handler(b
-00003440: 6f64 793a 2064 6963 742c 0a20 2020 2020  ody: dict,.     
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 6465 703a 2062 6f6f 6c20 3d20 4465    dep: bool = De
-00003470: 7065 6e64 7328 6465 7065 6e64 656e 6379  pends(dependency
-00003480: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00003490: 2020 2020 2020 2020 2020 6272 6f6b 6572            broker
-000034a0: 3a20 5261 6262 6974 4272 6f6b 6572 203d  : RabbitBroker =
-000034b0: 2043 6f6e 7465 7874 2829 293a 0a20 2020   Context()):.   
-000034c0: 2061 7373 6572 7420 6465 7020 6973 2054   assert dep is T
-000034d0: 7275 650a 2020 2020 6173 7365 7274 2062  rue.    assert b
-000034e0: 726f 6b65 7220 6973 2072 6162 6269 745f  roker is rabbit_
-000034f0: 6272 6f6b 6572 0a60 6060 0a0a 2d2d 2d0a  broker.```..---.
-00003500: 0a23 2320 434c 4920 706f 7765 720a 0a2a  .## CLI power..*
-00003510: 2a50 726f 7061 6e2a 2a20 6861 7320 6974  *Propan** has it
-00003520: 7320 6f77 6e20 434c 4920 746f 6f6c 2074  s own CLI tool t
-00003530: 6861 7420 7072 6f76 6964 6564 2074 6865  hat provided the
-00003540: 2066 6f6c 6c6f 7769 6e67 2066 6561 7475   following featu
-00003550: 7265 733a 0a0a 2a20 7072 6f6a 6563 7420  res:..* project 
-00003560: 6765 6e65 7261 7469 6f6e 0a2a 206d 756c  generation.* mul
-00003570: 7469 7072 6f63 6573 7369 6e67 2077 6f72  tiprocessing wor
-00003580: 6b65 7273 0a2a 2070 726f 6a65 6374 2068  kers.* project h
-00003590: 6f74 2072 656c 6f61 6469 6e67 0a2a 2063  ot reloading.* c
-000035a0: 7573 746f 6d20 636f 6d6d 616e 6420 6c69  ustom command li
-000035b0: 6e65 2061 7267 756d 656e 7473 2070 6173  ne arguments pas
-000035c0: 7369 6e67 0a0a 2323 2320 436f 6e74 6578  sing..### Contex
-000035d0: 7420 7061 7373 696e 670a 0a46 6f72 2065  t passing..For e
-000035e0: 7861 6d70 6c65 3a20 7061 7373 2079 6f75  xample: pass you
-000035f0: 7220 6375 7272 656e 7420 2a2e 656e 762a  r current *.env*
-00003600: 2070 726f 6a65 6374 2073 6574 7469 6e67   project setting
-00003610: 2074 6f20 636f 6e74 6578 740a 0a60 6060   to context..```
-00003620: 6261 7368 0a70 726f 7061 6e20 7275 6e20  bash.propan run 
-00003630: 7365 7276 653a 6170 7020 2d2d 656e 763d  serve:app --env=
-00003640: 2e65 6e76 2e64 6576 0a60 6060 0a0a 6060  .env.dev.```..``
-00003650: 6070 7974 686f 6e0a 6672 6f6d 2070 726f  `python.from pro
-00003660: 7061 6e20 696d 706f 7274 2050 726f 7061  pan import Propa
-00003670: 6e41 7070 2c20 5261 6262 6974 4272 6f6b  nApp, RabbitBrok
-00003680: 6572 0a66 726f 6d20 7072 6f70 616e 2e61  er.from propan.a
-00003690: 6e6e 6f74 6174 696f 6e73 2069 6d70 6f72  nnotations impor
-000036a0: 7420 436f 6e74 6578 7452 6570 6f0a 6672  t ContextRepo.fr
-000036b0: 6f6d 2070 7964 616e 7469 6320 696d 706f  om pydantic impo
-000036c0: 7274 2042 6173 6553 6574 7469 6e67 730a  rt BaseSettings.
-000036d0: 0a62 726f 6b65 7220 3d20 5261 6262 6974  .broker = Rabbit
-000036e0: 4272 6f6b 6572 2822 616d 7170 3a2f 2f67  Broker("amqp://g
-000036f0: 7565 7374 3a67 7565 7374 406c 6f63 616c  uest:guest@local
-00003700: 686f 7374 3a35 3637 322f 2229 0a0a 6170  host:5672/")..ap
-00003710: 7020 3d20 5072 6f70 616e 4170 7028 6272  p = PropanApp(br
-00003720: 6f6b 6572 290a 0a63 6c61 7373 2053 6574  oker)..class Set
-00003730: 7469 6e67 7328 4261 7365 5365 7474 696e  tings(BaseSettin
-00003740: 6773 293a 0a20 2020 202e 2e2e 0a0a 4061  gs):.    .....@a
-00003750: 7070 2e6f 6e5f 7374 6172 7475 700a 6173  pp.on_startup.as
-00003760: 796e 6320 6465 6620 7365 7475 7028 656e  ync def setup(en
-00003770: 763a 2073 7472 2c20 636f 6e74 6578 743a  v: str, context:
-00003780: 2043 6f6e 7465 7874 5265 706f 293a 0a20   ContextRepo):. 
-00003790: 2020 2073 6574 7469 6e67 7320 3d20 5365     settings = Se
-000037a0: 7474 696e 6773 285f 656e 765f 6669 6c65  ttings(_env_file
-000037b0: 3d65 6e76 290a 2020 2020 636f 6e74 6578  =env).    contex
-000037c0: 742e 7365 745f 676c 6f62 616c 2822 7365  t.set_global("se
-000037d0: 7474 696e 6773 222c 2073 6574 7469 6e67  ttings", setting
-000037e0: 7329 0a60 6060 0a0a 2323 2320 5072 6f6a  s).```..### Proj
-000037f0: 6563 7420 7465 6d70 6c61 7465 0a0a 416c  ect template..Al
-00003800: 736f 2c20 2a2a 5072 6f70 616e 2043 4c49  so, **Propan CLI
-00003810: 2a2a 2069 7320 6162 6c65 2074 6f20 6765  ** is able to ge
-00003820: 6e65 7261 7465 2061 2070 726f 6475 6374  nerate a product
-00003830: 696f 6e2d 7265 6164 7920 6170 706c 6963  ion-ready applic
-00003840: 6174 696f 6e20 7465 6d70 6c61 7465 3a0a  ation template:.
-00003850: 0a60 6060 6261 7368 0a70 726f 7061 6e20  .```bash.propan 
-00003860: 6372 6561 7465 2061 7379 6e63 2072 6162  create async rab
-00003870: 6269 7420 5b70 726f 6a65 6374 6e61 6d65  bit [projectname
-00003880: 5d0a 6060 600a 0a2a 4e6f 7469 6365 3a20  ].```..*Notice: 
-00003890: 7072 6f6a 6563 7420 7465 6d70 6c61 7465  project template
-000038a0: 2072 6571 7569 7265 2a20 6070 7964 616e   require* `pydan
-000038b0: 7469 635b 646f 7465 6e76 5d60 202a 696e  tic[dotenv]` *in
-000038c0: 7374 616c 6c61 7469 6f6e 2e2a 0a0a 5275  stallation.*..Ru
-000038d0: 6e20 7468 6520 6372 6561 7465 6420 7072  n the created pr
-000038e0: 6f6a 6563 743a 0a0a 6060 6062 6173 680a  oject:..```bash.
-000038f0: 2320 5275 6e20 7261 6262 696d 7120 6669  # Run rabbimq fi
-00003900: 7273 740a 646f 636b 6572 2063 6f6d 706f  rst.docker compo
-00003910: 7365 202d 2d66 696c 6520 5b70 726f 6a65  se --file [proje
-00003920: 6374 6e61 6d65 5d2f 646f 636b 6572 2d63  ctname]/docker-c
-00003930: 6f6d 706f 7365 2e79 616d 6c20 7570 202d  ompose.yaml up -
-00003940: 640a 0a23 2052 756e 2070 726f 6a65 6374  d..# Run project
-00003950: 0a70 726f 7061 6e20 7275 6e20 5b70 726f  .propan run [pro
-00003960: 6a65 6374 6e61 6d65 5d2e 6170 702e 7365  jectname].app.se
-00003970: 7276 653a 6170 7020 2d2d 656e 763d 2e65  rve:app --env=.e
-00003980: 6e76 202d 2d72 656c 6f61 640a 6060 600a  nv --reload.```.
-00003990: 0a4e 6f77 2079 6f75 2063 616e 2065 6e6a  .Now you can enj
-000039a0: 6f79 2061 206e 6577 2064 6576 656c 6f70  oy a new develop
-000039b0: 6d65 6e74 2065 7870 6572 6965 6e63 6521  ment experience!
-000039c0: 0a0a 2d2d 2d0a 0a23 2320 4854 5450 2046  ..---..## HTTP F
-000039d0: 7261 6d65 776f 726b 7320 696e 7465 6772  rameworks integr
-000039e0: 6174 696f 6e73 0a0a 2323 2320 416e 7920  ations..### Any 
-000039f0: 4672 616d 6577 6f72 6b0a 0a59 6f75 2063  Framework..You c
-00003a00: 616e 2075 7365 202a 2a50 726f 7061 6e2a  an use **Propan*
-00003a10: 2a20 604d 5142 726f 6b65 7273 6020 7769  * `MQBrokers` wi
-00003a20: 7468 6f75 7420 6050 726f 7061 6e41 7070  thout `PropanApp
-00003a30: 602e 0a4a 7573 7420 2a73 7461 7274 2a20  `..Just *start* 
-00003a40: 616e 6420 2a73 746f 702a 2074 6865 6d20  and *stop* them 
-00003a50: 6163 636f 7264 696e 6720 746f 2079 6f75  according to you
-00003a60: 7220 6170 706c 6963 6174 696f 6e20 6c69  r application li
-00003a70: 6665 7370 616e 2e0a 0a60 6060 7079 7468  fespan...```pyth
-00003a80: 6f6e 0a66 726f 6d20 7072 6f70 616e 2069  on.from propan i
-00003a90: 6d70 6f72 7420 4e61 7473 4272 6f6b 6572  mport NatsBroker
-00003aa0: 0a66 726f 6d20 7361 6e69 6320 696d 706f  .from sanic impo
-00003ab0: 7274 2053 616e 6963 0a0a 6170 7020 3d20  rt Sanic..app = 
-00003ac0: 5361 6e69 6328 224d 7948 656c 6c6f 576f  Sanic("MyHelloWo
-00003ad0: 726c 6441 7070 2229 0a62 726f 6b65 7220  rldApp").broker 
-00003ae0: 3d20 4e61 7473 4272 6f6b 6572 2822 6e61  = NatsBroker("na
-00003af0: 7473 3a2f 2f6c 6f63 616c 686f 7374 3a34  ts://localhost:4
-00003b00: 3232 3222 290a 0a40 6272 6f6b 6572 2e68  222")..@broker.h
-00003b10: 616e 646c 6528 2274 6573 7422 290a 6173  andle("test").as
-00003b20: 796e 6320 6465 6620 6261 7365 5f68 616e  ync def base_han
-00003b30: 646c 6572 2862 6f64 7929 3a0a 2020 2020  dler(body):.    
-00003b40: 7072 696e 7428 626f 6479 290a 0a40 6170  print(body)..@ap
-00003b50: 702e 6166 7465 725f 7365 7276 6572 5f73  p.after_server_s
-00003b60: 7461 7274 0a61 7379 6e63 2064 6566 2073  tart.async def s
-00003b70: 7461 7274 5f62 726f 6b65 7228 6170 702c  tart_broker(app,
-00003b80: 206c 6f6f 7029 3a0a 2020 2020 6177 6169   loop):.    awai
-00003b90: 7420 6272 6f6b 6572 2e73 7461 7274 2829  t broker.start()
-00003ba0: 0a0a 4061 7070 2e61 6674 6572 5f73 6572  ..@app.after_ser
-00003bb0: 7665 725f 7374 6f70 0a61 7379 6e63 2064  ver_stop.async d
-00003bc0: 6566 2073 746f 705f 6272 6f6b 6572 2861  ef stop_broker(a
-00003bd0: 7070 2c20 6c6f 6f70 293a 0a20 2020 2061  pp, loop):.    a
-00003be0: 7761 6974 2062 726f 6b65 722e 636c 6f73  wait broker.clos
-00003bf0: 6528 290a 6060 600a 0a23 2323 2046 6173  e().```..### Fas
-00003c00: 7441 5049 2050 6c75 6769 6e0a 0a41 6c73  tAPI Plugin..Als
-00003c10: 6f2c 202a 2a50 726f 7061 6e2a 2a20 6361  o, **Propan** ca
-00003c20: 6e20 6265 2075 7365 6420 6173 2070 6172  n be used as par
-00003c30: 7420 6f66 202a 2a46 6173 7441 5049 2a2a  t of **FastAPI**
-00003c40: 2e0a 0a4a 7573 7420 696d 706f 7274 2061  ...Just import a
-00003c50: 202a 2a50 726f 7061 6e52 6f75 7465 722a   **PropanRouter*
-00003c60: 2a20 796f 7520 6e65 6564 2061 6e64 2064  * you need and d
-00003c70: 6563 6c61 7265 2074 6865 206d 6573 7361  eclare the messa
-00003c80: 6765 2068 616e 646c 6572 0a75 7369 6e67  ge handler.using
-00003c90: 2074 6865 2060 4065 7665 6e74 6020 6465   the `@event` de
-00003ca0: 636f 7261 746f 722e 2054 6869 7320 6465  corator. This de
-00003cb0: 636f 7261 746f 7220 6973 2073 696d 696c  corator is simil
-00003cc0: 6172 2074 6f20 7468 6520 6465 636f 7261  ar to the decora
-00003cd0: 746f 7220 6040 6861 6e64 6c65 6020 666f  tor `@handle` fo
-00003ce0: 7220 7468 6520 636f 7272 6573 706f 6e64  r the correspond
-00003cf0: 696e 6720 6272 6f6b 6572 732e 0a0a 6060  ing brokers...``
-00003d00: 6070 7974 686f 6e0a 6672 6f6d 2066 6173  `python.from fas
-00003d10: 7461 7069 2069 6d70 6f72 7420 4465 7065  tapi import Depe
-00003d20: 6e64 732c 2046 6173 7441 5049 0a66 726f  nds, FastAPI.fro
-00003d30: 6d20 7079 6461 6e74 6963 2069 6d70 6f72  m pydantic impor
-00003d40: 7420 4261 7365 4d6f 6465 6c0a 6672 6f6d  t BaseModel.from
-00003d50: 2070 726f 7061 6e2e 6661 7374 6170 6920   propan.fastapi 
-00003d60: 696d 706f 7274 2052 6162 6269 7452 6f75  import RabbitRou
-00003d70: 7465 720a 0a61 7070 203d 2046 6173 7441  ter..app = FastA
-00003d80: 5049 2829 0a0a 726f 7574 6572 203d 2052  PI()..router = R
-00003d90: 6162 6269 7452 6f75 7465 7228 2261 6d71  abbitRouter("amq
-00003da0: 703a 2f2f 6775 6573 743a 6775 6573 7440  p://guest:guest@
-00003db0: 6c6f 6361 6c68 6f73 743a 3536 3732 2229  localhost:5672")
-00003dc0: 0a0a 636c 6173 7320 496e 636f 6d69 6e67  ..class Incoming
-00003dd0: 2842 6173 654d 6f64 656c 293a 0a20 2020  (BaseModel):.   
-00003de0: 206d 3a20 6469 6374 0a0a 6465 6620 6361   m: dict..def ca
-00003df0: 6c6c 2829 3a0a 2020 2020 7265 7475 726e  ll():.    return
-00003e00: 2054 7275 650a 0a40 726f 7574 6572 2e65   True..@router.e
-00003e10: 7665 6e74 2822 7465 7374 2229 0a61 7379  vent("test").asy
-00003e20: 6e63 2064 6566 2068 656c 6c6f 286d 3a20  nc def hello(m: 
-00003e30: 496e 636f 6d69 6e67 2c20 6420 3d20 4465  Incoming, d = De
-00003e40: 7065 6e64 7328 6361 6c6c 2929 202d 3e20  pends(call)) -> 
-00003e50: 6469 6374 3a0a 2020 2020 7265 7475 726e  dict:.    return
-00003e60: 207b 2022 7265 7370 6f6e 7365 223a 2022   { "response": "
-00003e70: 4865 6c6c 6f2c 2050 726f 7061 6e21 2220  Hello, Propan!" 
-00003e80: 7d0a 0a61 7070 2e69 6e63 6c75 6465 5f72  }..app.include_r
-00003e90: 6f75 7465 7228 726f 7574 6572 290a 6060  outer(router).``
-00003ea0: 600a 0a23 2320 4578 616d 706c 6573 0a0a  `..## Examples..
-00003eb0: 546f 2073 6565 206d 6f72 6520 6672 616d  To see more fram
-00003ec0: 6577 6f72 6b20 7573 6167 6573 2067 6f20  ework usages go 
-00003ed0: 746f 205b 2a2a 6578 616d 706c 6573 2f2a  to [**examples/*
-00003ee0: 2a5d 2868 7474 7073 3a2f 2f67 6974 6875  *](https://githu
-00003ef0: 622e 636f 6d2f 4c61 6e63 6574 6e69 6b2f  b.com/Lancetnik/
-00003f00: 5072 6f70 616e 2f74 7265 652f 6d61 696e  Propan/tree/main
-00003f10: 2f65 7861 6d70 6c65 7329 0a              /examples).
+00001080: 7073 3a2f 2f6c 616e 6365 746e 696b 2e67  ps://lancetnik.g
+00001090: 6974 6875 622e 696f 2f50 726f 7061 6e2f  ithub.io/Propan/
+000010a0: 6173 7365 7473 2f69 6d67 2f6c 6f67 6f2d  assets/img/logo-
+000010b0: 6e6f 2d62 6163 6b67 726f 756e 642e 706e  no-background.pn
+000010c0: 6722 2061 6c74 3d22 5072 6f70 616e 206c  g" alt="Propan l
+000010d0: 6f67 6f22 2073 7479 6c65 3d22 6865 6967  ogo" style="heig
+000010e0: 6874 3a20 3235 3070 783b 2077 6964 7468  ht: 250px; width
+000010f0: 3a20 3630 3070 783b 222f 3e0a 2020 2020  : 600px;"/>.    
+00001100: 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020 616c  </a>.</p>..<p al
+00001110: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00001120: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001130: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c61  ://github.com/La
+00001140: 6e63 6574 6e69 6b2f 5072 6f70 616e 2f61  ncetnik/Propan/a
+00001150: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00001160: 2f74 6573 7473 2e79 6d6c 2220 7461 7267  /tests.yml" targ
+00001170: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+00001180: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00001190: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000011a0: 6d2f 4c61 6e63 6574 6e69 6b2f 5072 6f70  m/Lancetnik/Prop
+000011b0: 616e 2f61 6374 696f 6e73 2f77 6f72 6b66  an/actions/workf
+000011c0: 6c6f 7773 2f74 6573 7473 2e79 6d6c 2f62  lows/tests.yml/b
+000011d0: 6164 6765 2e73 7667 2220 616c 743d 2254  adge.svg" alt="T
+000011e0: 6573 7473 2063 6f76 6572 6167 6522 2f3e  ests coverage"/>
+000011f0: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+00001200: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00001210: 6f76 6572 6167 652d 6261 6467 652e 7361  overage-badge.sa
+00001220: 6d75 656c 636f 6c76 696e 2e77 6f72 6b65  muelcolvin.worke
+00001230: 7273 2e64 6576 2f72 6564 6972 6563 742f  rs.dev/redirect/
+00001240: 6c61 6e63 6574 6e69 6b2f 7072 6f70 616e  lancetnik/propan
+00001250: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001260: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+00001270: 7372 633d 2268 7474 7073 3a2f 2f63 6f76  src="https://cov
+00001280: 6572 6167 652d 6261 6467 652e 7361 6d75  erage-badge.samu
+00001290: 656c 636f 6c76 696e 2e77 6f72 6b65 7273  elcolvin.workers
+000012a0: 2e64 6576 2f6c 616e 6365 746e 696b 2f70  .dev/lancetnik/p
+000012b0: 726f 7061 6e2e 7376 6722 2061 6c74 3d22  ropan.svg" alt="
+000012c0: 436f 7665 7261 6765 223e 0a20 2020 203c  Coverage">.    <
+000012d0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+000012e0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000012f0: 672f 7072 6f6a 6563 742f 7072 6f70 616e  g/project/propan
+00001300: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001310: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+00001320: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00001330: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00001340: 2f76 2f70 726f 7061 6e3f 6c61 6265 6c3d  /v/propan?label=
+00001350: 7079 7069 2532 3070 6163 6b61 6765 2220  pypi%20package" 
+00001360: 616c 743d 2250 6163 6b61 6765 2076 6572  alt="Package ver
+00001370: 7369 6f6e 223e 0a20 2020 203c 2f61 3e0a  sion">.    </a>.
+00001380: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00001390: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+000013a0: 726f 6a65 6374 2f70 726f 7061 6e22 2074  roject/propan" t
+000013b0: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+000013c0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+000013d0: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
+000013e0: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+000013f0: 6e61 6c69 7a65 642d 6261 6467 652f 7072  nalized-badge/pr
+00001400: 6f70 616e 3f70 6572 696f 643d 746f 7461  opan?period=tota
+00001410: 6c26 756e 6974 733d 696e 7465 726e 6174  l&units=internat
+00001420: 696f 6e61 6c5f 7379 7374 656d 266c 6566  ional_system&lef
+00001430: 745f 636f 6c6f 723d 6772 6579 2672 6967  t_color=grey&rig
+00001440: 6874 5f63 6f6c 6f72 3d62 6c75 6526 6c65  ht_color=blue&le
+00001450: 6674 5f74 6578 743d 446f 776e 6c6f 6164  ft_text=Download
+00001460: 7322 2061 6c74 3d22 646f 776e 6c6f 6164  s" alt="download
+00001470: 7322 2f3e 0a20 2020 203c 2f61 3e0a 2020  s"/>.    </a>.  
+00001480: 2020 3c62 722f 3e0a 2020 2020 3c61 2068    <br/>.    <a h
+00001490: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000014a0: 692e 6f72 672f 7072 6f6a 6563 742f 7072  i.org/project/pr
+000014b0: 6f70 616e 2220 7461 7267 6574 3d22 5f62  opan" target="_b
+000014c0: 6c61 6e6b 223e 0a20 2020 2020 2020 203c  lank">.        <
+000014d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000014e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000014f0: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00001500: 7072 6f70 616e 2e73 7667 2220 616c 743d  propan.svg" alt=
+00001510: 2253 7570 706f 7274 6564 2050 7974 686f  "Supported Pytho
+00001520: 6e20 7665 7273 696f 6e73 223e 0a20 2020  n versions">.   
+00001530: 203c 2f61 3e0a 2020 2020 3c61 2068 7265   </a>.    <a hre
+00001540: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001550: 622e 636f 6d2f 4c61 6e63 6574 6e69 6b2f  b.com/Lancetnik/
+00001560: 5072 6f70 616e 2f62 6c6f 622f 6d61 696e  Propan/blob/main
+00001570: 2f4c 4943 454e 5345 2220 7461 7267 6574  /LICENSE" target
+00001580: 3d22 5f62 6c61 6e6b 223e 0a20 2020 2020  ="_blank">.     
+00001590: 2020 203c 696d 6720 616c 743d 2247 6974     <img alt="Git
+000015a0: 4875 6222 2073 7263 3d22 6874 7470 733a  Hub" src="https:
+000015b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000015c0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+000015d0: 4c61 6e63 6574 6e69 6b2f 5072 6f70 616e  Lancetnik/Propan
+000015e0: 3f63 6f6c 6f72 3d25 3233 3030 3765 6336  ?color=%23007ec6
+000015f0: 223e 0a20 2020 203c 2f61 3e0a 3c2f 703e  ">.    </a>.</p>
+00001600: 0a0a 2320 5072 6f70 616e 0a0a 2a2a 5072  ..# Propan..**Pr
+00001610: 6f70 616e 2a2a 202d 206a 7573 7420 2a7e  opan** - just *~
+00001620: 7e61 6e20 616e 6f74 6865 7220 6f6e 6520  ~an another one 
+00001630: 4854 5450 7e7e 2a20 6120 2a2a 6465 636c  HTTP~~* a **decl
+00001640: 6172 6174 6976 6520 5079 7468 6f6e 204d  arative Python M
+00001650: 5120 6672 616d 6577 6f72 6b2a 2a2e 2049  Q framework**. I
+00001660: 7427 7320 666f 6c6c 6f77 696e 6720 6279  t's following by
+00001670: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001680: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
+00001690: 6c6f 2e63 6f6d 2f72 752f 2220 7461 7267  lo.com/ru/" targ
+000016a0: 6574 3d22 5f62 6c61 6e6b 223e 2a66 6173  et="_blank">*fas
+000016b0: 7461 7069 2a3c 2f61 3e2c 2073 696d 706c  tapi*</a>, simpl
+000016c0: 6966 7920 4d65 7373 6167 6520 4272 6f6b  ify Message Brok
+000016d0: 6572 7320 6172 6f75 6e64 2063 6f64 6520  ers around code 
+000016e0: 7772 6974 696e 6720 616e 6420 7072 6f76  writing and prov
+000016f0: 6964 6573 2061 2068 656c 7066 756c 2064  ides a helpful d
+00001700: 6576 656c 6f70 6d65 6e74 2074 6f6f 6c6b  evelopment toolk
+00001710: 6974 2c20 7768 6963 6820 6578 6973 7465  it, which existe
+00001720: 6420 6f6e 6c79 2069 6e20 4854 5450 2d66  d only in HTTP-f
+00001730: 7261 6d65 776f 726b 7320 776f 726c 6420  rameworks world 
+00001740: 756e 7469 6c20 6e6f 772e 0a0a 4974 2773  until now...It's
+00001750: 2064 6573 6967 6e65 6420 746f 2063 7265   designed to cre
+00001760: 6174 6520 7265 6163 7469 7665 206d 6963  ate reactive mic
+00001770: 726f 7365 7276 6963 6573 2061 726f 756e  roservices aroun
+00001780: 6420 3c61 2068 7265 663d 2268 7474 7073  d <a href="https
+00001790: 3a2f 2f6d 6963 726f 7365 7276 6963 6573  ://microservices
+000017a0: 2e69 6f2f 7061 7474 6572 6e73 2f63 6f6d  .io/patterns/com
+000017b0: 6d75 6e69 6361 7469 6f6e 2d73 7479 6c65  munication-style
+000017c0: 2f6d 6573 7361 6769 6e67 2e68 746d 6c22  /messaging.html"
+000017d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000017e0: 3e4d 6573 7361 6769 6e67 2041 7263 6869  >Messaging Archi
+000017f0: 7465 6374 7572 653c 2f61 3e2e 0a0a 4974  tecture</a>...It
+00001800: 2069 7320 6120 6d6f 6465 726e 2c20 6869   is a modern, hi
+00001810: 6768 2d6c 6576 656c 2066 7261 6d65 776f  gh-level framewo
+00001820: 726b 206f 6e20 746f 7020 6f66 2070 6f70  rk on top of pop
+00001830: 756c 6172 2073 7065 6369 6669 6320 5079  ular specific Py
+00001840: 7468 6f6e 2062 726f 6b65 7273 206c 6962  thon brokers lib
+00001850: 7261 7269 6573 2c20 6261 7365 6420 6f6e  raries, based on
+00001860: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001870: 2f2f 646f 6373 2e70 7964 616e 7469 632e  //docs.pydantic.
+00001880: 6465 762f 2220 7461 7267 6574 3d22 5f62  dev/" target="_b
+00001890: 6c61 6e6b 223e 2a70 7964 616e 7469 632a  lank">*pydantic*
+000018a0: 3c2f 613e 2061 6e64 203c 6120 6872 6566  </a> and <a href
+000018b0: 3d22 6874 7470 733a 2f2f 6661 7374 6170  ="https://fastap
+000018c0: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f72  i.tiangolo.com/r
+000018d0: 752f 2220 7461 7267 6574 3d22 5f62 6c61  u/" target="_bla
+000018e0: 6e6b 223e 2a66 6173 7461 7069 2a3c 2f61  nk">*fastapi*</a
+000018f0: 3e2c 203c 6120 6872 6566 3d22 6874 7470  >, <a href="http
+00001900: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
+00001910: 6f72 672f 656e 2f6c 6174 6573 742f 2220  org/en/latest/" 
+00001920: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00001930: 2a70 7974 6573 742a 3c2f 613e 2063 6f6e  *pytest*</a> con
+00001940: 6365 7074 732e 0a0a 2d2d 2d0a 0a2a 2a44  cepts...---..**D
+00001950: 6f63 756d 656e 7461 7469 6f6e 2a2a 3a20  ocumentation**: 
+00001960: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001970: 2f6c 616e 6365 746e 696b 2e67 6974 6875  /lancetnik.githu
+00001980: 622e 696f 2f50 726f 7061 6e2f 2220 7461  b.io/Propan/" ta
+00001990: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
+000019a0: 7470 733a 2f2f 6c61 6e63 6574 6e69 6b2e  tps://lancetnik.
+000019b0: 6769 7468 7562 2e69 6f2f 5072 6f70 616e  github.io/Propan
+000019c0: 2f3c 2f61 3e0a 0a2d 2d2d 0a0a 2323 2320  /</a>..---..### 
+000019d0: 5468 6520 6b65 7920 6665 6174 7572 6573  The key features
+000019e0: 2061 7265 0a0a 2a20 2a2a 5369 6d70 6c65   are..* **Simple
+000019f0: 2a2a 3a20 4465 7369 676e 6564 2074 6f20  **: Designed to 
+00001a00: 6265 2065 6173 7920 746f 2075 7365 2061  be easy to use a
+00001a10: 6e64 206c 6561 726e 2e0a 2a20 2a2a 496e  nd learn..* **In
+00001a20: 7475 6974 6976 652a 2a3a 2047 7265 6174  tuitive**: Great
+00001a30: 2065 6469 746f 7220 7375 7070 6f72 742e   editor support.
+00001a40: 2041 7574 6f63 6f6d 706c 6574 696f 6e20   Autocompletion 
+00001a50: 6576 6572 7977 6865 7265 2e0a 2a20 5b2a  everywhere..* [*
+00001a60: 2a44 6570 656e 6465 6e63 6965 7320 6d61  *Dependencies ma
+00001a70: 6e61 6765 6d65 6e74 2a2a 5d28 2364 6570  nagement**](#dep
+00001a80: 656e 6465 6e63 6965 7329 3a20 4d69 6e69  endencies): Mini
+00001a90: 6d69 7a61 7469 6f6e 206f 6620 636f 6465  mization of code
+00001aa0: 2064 7570 6c69 6361 7469 6f6e 2e20 4163   duplication. Ac
+00001ab0: 6365 7373 2074 6f20 6465 7065 6e64 656e  cess to dependen
+00001ac0: 6369 6573 2061 7420 616e 7920 6c65 7665  cies at any leve
+00001ad0: 6c20 6f66 2074 6865 2063 616c 6c20 7374  l of the call st
+00001ae0: 6163 6b2e 0a2a 205b 2a2a 496e 7465 6772  ack..* [**Integr
+00001af0: 6174 696f 6e73 2a2a 5d28 2368 7474 702d  ations**](#http-
+00001b00: 6672 616d 6577 6f72 6b73 2d69 6e74 6567  frameworks-integ
+00001b10: 7261 7469 6f6e 7329 3a20 2a2a 5072 6f70  rations): **Prop
+00001b20: 616e 2a2a 2069 7320 6675 6c6c 7920 636f  an** is fully co
+00001b30: 6d70 6174 6962 6c65 2077 6974 6820 3c61  mpatible with <a
+00001b40: 2068 7265 663d 2268 7474 7073 3a2f 2f6c   href="https://l
+00001b50: 616e 6365 746e 696b 2e67 6974 6875 622e  ancetnik.github.
+00001b60: 696f 2f50 726f 7061 6e2f 696e 7465 6772  io/Propan/integr
+00001b70: 6174 696f 6e73 2f31 5f69 6e74 6567 7261  ations/1_integra
+00001b80: 7469 6f6e 732d 696e 6465 782f 2220 7461  tions-index/" ta
+00001b90: 7267 6574 3d22 5f62 6c61 6e6b 223e 616e  rget="_blank">an
+00001ba0: 7920 4854 5450 2066 7261 6d65 776f 726b  y HTTP framework
+00001bb0: 3c2f 613e 2079 6f75 2077 616e 740a 2a20  </a> you want.* 
+00001bc0: 2a2a 4d51 2069 6e64 6570 656e 6465 6e74  **MQ independent
+00001bd0: 2a2a 3a20 5369 6e67 6c65 2069 6e74 6572  **: Single inter
+00001be0: 6661 6365 2074 6f20 706f 7075 6c61 7220  face to popular 
+00001bf0: 4d51 3a0a 2020 2a20 2a2a 5265 6469 732a  MQ:.  * **Redis*
+00001c00: 2a20 2862 6173 6564 206f 6e20 3c61 2068  * (based on <a h
+00001c10: 7265 663d 2268 7474 7073 3a2f 2f72 6564  ref="https://red
+00001c20: 6973 2e72 6561 6474 6865 646f 6373 2e69  is.readthedocs.i
+00001c30: 6f2f 656e 2f73 7461 626c 652f 696e 6465  o/en/stable/inde
+00001c40: 782e 6874 6d6c 2220 7461 7267 6574 3d22  x.html" target="
+00001c50: 5f62 6c61 6e6b 223e 7265 6469 732d 7079  _blank">redis-py
+00001c60: 3c2f 613e 290a 2020 2a20 2a2a 5261 6262  </a>).  * **Rabb
+00001c70: 6974 4d51 2a2a 2028 6261 7365 6420 6f6e  itMQ** (based on
+00001c80: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001c90: 2f2f 6169 6f2d 7069 6b61 2e72 6561 6474  //aio-pika.readt
+00001ca0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001cb0: 6573 742f 2220 7461 7267 6574 3d22 5f62  est/" target="_b
+00001cc0: 6c61 6e6b 223e 6169 6f2d 7069 6b61 3c2f  lank">aio-pika</
+00001cd0: 613e 290a 2020 2a20 2a2a 4b61 666b 612a  a>).  * **Kafka*
+00001ce0: 2a20 2862 6173 6564 206f 6e20 3c61 2068  * (based on <a h
+00001cf0: 7265 663d 2268 7474 7073 3a2f 2f61 696f  ref="https://aio
+00001d00: 6b61 666b 612e 7265 6164 7468 6564 6f63  kafka.readthedoc
+00001d10: 732e 696f 2f65 6e2f 7374 6162 6c65 2f22  s.io/en/stable/"
+00001d20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001d30: 3e61 696f 6b61 666b 613c 2f61 3e29 0a20  >aiokafka</a>). 
+00001d40: 202a 202a 2a53 5153 2a2a 2028 6261 7365   * **SQS** (base
+00001d50: 6420 6f6e 203c 6120 6872 6566 3d22 6874  d on <a href="ht
+00001d60: 7470 733a 2f2f 6169 6f62 6f74 6f63 6f72  tps://aiobotocor
+00001d70: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00001d80: 2f65 6e2f 6c61 7465 7374 2f22 2074 6172  /en/latest/" tar
+00001d90: 6765 743d 225f 626c 616e 6b22 3e61 696f  get="_blank">aio
+00001da0: 626f 746f 636f 7265 3c2f 613e 290a 2020  botocore</a>).  
+00001db0: 2a20 2a2a 4e61 7473 2a2a 2028 6261 7365  * **Nats** (base
+00001dc0: 6420 6f6e 203c 6120 6872 6566 3d22 6874  d on <a href="ht
+00001dd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001de0: 2f6e 6174 732d 696f 2f6e 6174 732e 7079  /nats-io/nats.py
+00001df0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001e00: 223e 6e61 7473 2d70 793c 2f61 3e29 0a2a  ">nats-py</a>).*
+00001e10: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001e20: 2f2f 6c61 6e63 6574 6e69 6b2e 6769 7468  //lancetnik.gith
+00001e30: 7562 2e69 6f2f 5072 6f70 616e 2f67 6574  ub.io/Propan/get
+00001e40: 7469 6e67 5f73 7461 7274 6564 2f34 5f62  ting_started/4_b
+00001e50: 726f 6b65 722f 355f 7270 632f 2220 7461  roker/5_rpc/" ta
+00001e60: 7267 6574 3d22 5f62 6c61 6e6b 223e 2a2a  rget="_blank">**
+00001e70: 5250 432a 2a3c 2f61 3e3a 2054 6865 2066  RPC**</a>: The f
+00001e80: 7261 6d65 776f 726b 2073 7570 706f 7274  ramework support
+00001e90: 7320 5250 4320 7265 7175 6573 7473 206f  s RPC requests o
+00001ea0: 7665 7220 4d51 2c20 7768 6963 6820 7769  ver MQ, which wi
+00001eb0: 6c6c 2061 6c6c 6f77 2070 6572 666f 726d  ll allow perform
+00001ec0: 696e 6720 6c6f 6e67 206f 7065 7261 7469  ing long operati
+00001ed0: 6f6e 7320 6f6e 2072 656d 6f74 6520 7365  ons on remote se
+00001ee0: 7276 6963 6573 2061 7379 6e63 6872 6f6e  rvices asynchron
+00001ef0: 6f75 736c 792e 0a2a 205b 2a2a 4772 6561  ously..* [**Grea
+00001f00: 7420 746f 2064 6576 656c 6f70 2a2a 5d28  t to develop**](
+00001f10: 2363 6c69 2d70 6f77 6572 293a 2043 4c49  #cli-power): CLI
+00001f20: 2074 6f6f 6c20 7072 6f76 6964 6573 2067   tool provides g
+00001f30: 7265 6174 2064 6576 656c 6f70 6d65 6e74  reat development
+00001f40: 2065 7870 6572 6965 6e63 653a 0a20 202a   experience:.  *
+00001f50: 2066 7261 6d65 776f 726b 2d69 6e64 6570   framework-indep
+00001f60: 656e 6465 6e74 2077 6179 2074 6f20 6d61  endent way to ma
+00001f70: 6e61 6765 2074 6865 2070 726f 6a65 6374  nage the project
+00001f80: 2065 6e76 6972 6f6e 6d65 6e74 0a20 202a   environment.  *
+00001f90: 2061 7070 6c69 6361 7469 6f6e 2063 6f64   application cod
+00001fa0: 6520 2a68 6f74 2072 656c 6f61 642a 0a20  e *hot reload*. 
+00001fb0: 202a 2072 6f62 7573 7420 6170 706c 6963   * robust applic
+00001fc0: 6174 696f 6e20 7465 6d70 6c61 7465 730a  ation templates.
+00001fd0: 2a20 5b2a 2a44 6f63 756d 656e 7461 7469  * [**Documentati
+00001fe0: 6f6e 2a2a 5d28 2370 726f 6a65 6374 2d64  on**](#project-d
+00001ff0: 6f63 756d 656e 7461 7469 6f6e 293a 202a  ocumentation): *
+00002000: 2a50 726f 7061 6e2a 2a20 6175 746f 6d61  *Propan** automa
+00002010: 7469 6361 6c6c 7920 6765 6e65 7261 7465  tically generate
+00002020: 7320 616e 6420 7072 6573 656e 7473 2061  s and presents a
+00002030: 6e20 696e 7465 7261 6374 6976 6520 3c61  n interactive <a
+00002040: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+00002050: 7777 2e61 7379 6e63 6170 692e 636f 6d2f  ww.asyncapi.com/
+00002060: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00002070: 223e 2a2a 4173 796e 6341 5049 2a2a 3c2f  ">**AsyncAPI**</
+00002080: 613e 2064 6f63 756d 656e 7461 7469 6f6e  a> documentation
+00002090: 2066 6f72 2079 6f75 7220 7072 6f6a 6563   for your projec
+000020a0: 740a 2a20 3c61 2068 7265 663d 2268 7474  t.* <a href="htt
+000020b0: 7073 3a2f 2f6c 616e 6365 746e 696b 2e67  ps://lancetnik.g
+000020c0: 6974 6875 622e 696f 2f50 726f 7061 6e2f  ithub.io/Propan/
+000020d0: 6765 7474 696e 675f 7374 6172 7465 642f  getting_started/
+000020e0: 375f 7465 7374 696e 6722 2074 6172 6765  7_testing" targe
+000020f0: 743d 225f 626c 616e 6b22 3e2a 2a54 6573  t="_blank">**Tes
+00002100: 7461 6269 6c69 7479 2a2a 3c2f 613e 3a20  tability**</a>: 
+00002110: 2a2a 5072 6f70 616e 2a2a 2061 6c6c 6f77  **Propan** allow
+00002120: 7320 796f 7520 746f 2074 6573 7420 796f  s you to test yo
+00002130: 7572 2061 7070 2077 6974 686f 7574 2065  ur app without e
+00002140: 7874 6572 6e61 6c20 6465 7065 6e64 656e  xternal dependen
+00002150: 6369 6573 3a20 796f 7520 646f 206e 6f74  cies: you do not
+00002160: 2068 6176 6520 746f 2073 6574 2075 7020   have to set up 
+00002170: 6120 4d65 7373 6167 6520 4272 6f6b 6572  a Message Broker
+00002180: 2c20 796f 7520 6361 6e20 7573 6520 6120  , you can use a 
+00002190: 7669 7274 7561 6c20 6f6e 6521 0a0a 2323  virtual one!..##
+000021a0: 2320 5375 7070 6f72 7465 6420 4d51 2062  # Supported MQ b
+000021b0: 726f 6b65 7273 0a0a 7c20 2020 2020 2020  rokers..|       
+000021c0: 2020 2020 2020 2020 2020 2020 7c20 6173              | as
+000021d0: 796e 6320 2020 2020 2020 2020 2020 2020  ync             
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2020 2020 7c20 7379 6e63 2020 2020        | sync    
+00002210: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00002220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002230: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
+00002240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  ------------:|:-
+00002270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002280: 2d2d 2d3a 7c0a 7c20 2a2a 5261 6262 6974  ---:|.| **Rabbit
+00002290: 4d51 2a2a 2020 2020 2020 7c20 3a68 6561  MQ**      | :hea
+000022a0: 7679 5f63 6865 636b 5f6d 6172 6b3a 202a  vy_check_mark: *
+000022b0: 2a73 7461 626c 652a 2a20 3a68 6561 7679  *stable** :heavy
+000022c0: 5f63 6865 636b 5f6d 6172 6b3a 2020 2020  _check_mark:    
+000022d0: 2020 2020 7c20 3a6d 6167 3a20 706c 616e      | :mag: plan
+000022e0: 6e69 6e67 203a 6d61 673a 207c 0a7c 202a  ning :mag: |.| *
+000022f0: 2a52 6564 6973 2a2a 2020 2020 2020 2020  *Redis**        
+00002300: 207c 203a 6865 6176 795f 6368 6563 6b5f   | :heavy_check_
+00002310: 6d61 726b 3a20 2a2a 7374 6162 6c65 2a2a  mark: **stable**
+00002320: 203a 6865 6176 795f 6368 6563 6b5f 6d61   :heavy_check_ma
+00002330: 726b 3a20 2020 2020 2020 207c 203a 6d61  rk:        | :ma
+00002340: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
+00002350: 3a20 7c0a 7c20 2a2a 4e61 7473 2a2a 2020  : |.| **Nats**  
+00002360: 2020 2020 2020 2020 7c20 3a68 6561 7679          | :heavy
+00002370: 5f63 6865 636b 5f6d 6172 6b3a 202a 2a73  _check_mark: **s
+00002380: 7461 626c 652a 2a20 3a68 6561 7679 5f63  table** :heavy_c
+00002390: 6865 636b 5f6d 6172 6b3a 2020 2020 2020  heck_mark:      
+000023a0: 2020 7c20 3a6d 6167 3a20 706c 616e 6e69    | :mag: planni
+000023b0: 6e67 203a 6d61 673a 207c 0a7c 202a 2a4b  ng :mag: |.| **K
+000023c0: 6166 6b61 2a2a 2020 2020 2020 2020 207c  afka**         |
+000023d0: 203a 7761 726e 696e 673a 202a 2a62 6574   :warning: **bet
+000023e0: 612a 2a20 3a77 6172 6e69 6e67 3a20 2020  a** :warning:   
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 2020 2020 207c 203a 6d61 673a           | :mag:
+00002410: 2070 6c61 6e6e 696e 6720 3a6d 6167 3a20   planning :mag: 
+00002420: 7c0a 7c20 2a2a 5351 532a 2a20 2020 2020  |.| **SQS**     
+00002430: 2020 2020 2020 7c20 3a77 6172 6e69 6e67        | :warning
+00002440: 3a20 2a2a 6265 7461 2a2a 203a 7761 726e  : **beta** :warn
+00002450: 696e 673a 2020 2020 2020 2020 2020 2020  ing:            
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 7c20 3a6d 6167 3a20 706c 616e 6e69 6e67  | :mag: planning
+00002480: 203a 6d61 673a 207c 0a7c 202a 2a4e 6174   :mag: |.| **Nat
+00002490: 734a 532a 2a20 2020 2020 2020 207c 203a  sJS**        | :
+000024a0: 6861 6d6d 6572 5f61 6e64 5f77 7265 6e63  hammer_and_wrenc
+000024b0: 683a 202a 2a69 6e20 7072 6f67 7265 7373  h: **in progress
+000024c0: 2a2a 203a 6861 6d6d 6572 5f61 6e64 5f77  ** :hammer_and_w
+000024d0: 7265 6e63 683a 207c 203a 6d61 673a 2070  rench: | :mag: p
+000024e0: 6c61 6e6e 696e 6720 3a6d 6167 3a20 7c0a  lanning :mag: |.
+000024f0: 7c20 2a2a 4d51 5454 2a2a 2020 2020 2020  | **MQTT**      
+00002500: 2020 2020 7c20 3a6d 6167 3a20 706c 616e      | :mag: plan
+00002510: 6e69 6e67 203a 6d61 673a 2020 2020 2020  ning :mag:      
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00002540: 3a6d 6167 3a20 706c 616e 6e69 6e67 203a  :mag: planning :
+00002550: 6d61 673a 207c 0a7c 202a 2a52 6564 6973  mag: |.| **Redis
+00002560: 2053 7472 6561 6d73 2a2a 207c 203a 6d61   Streams** | :ma
+00002570: 673a 2070 6c61 6e6e 696e 6720 3a6d 6167  g: planning :mag
+00002580: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 2020 207c 203a 6d61 673a 2070 6c61       | :mag: pla
+000025b0: 6e6e 696e 6720 3a6d 6167 3a20 7c0a 7c20  nning :mag: |.| 
+000025c0: 2a2a 5075 6c73 6172 2a2a 2020 2020 2020  **Pulsar**      
+000025d0: 2020 7c20 3a6d 6167 3a20 706c 616e 6e69    | :mag: planni
+000025e0: 6e67 203a 6d61 673a 2020 2020 2020 2020  ng :mag:        
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 2020 2020 2020 2020 2020 7c20 3a6d              | :m
+00002610: 6167 3a20 706c 616e 6e69 6e67 203a 6d61  ag: planning :ma
+00002620: 673a 207c 0a0a 2323 2320 436f 6d6d 756e  g: |..### Commun
+00002630: 6974 790a 0a49 6620 796f 7520 6172 6520  ity..If you are 
+00002640: 696e 7465 7265 7374 6564 2069 6e20 7468  interested in th
+00002650: 6973 2070 726f 6a65 6374 2c20 706c 6561  is project, plea
+00002660: 7365 2067 6976 6520 6d65 2066 6565 6462  se give me feedb
+00002670: 6163 6b20 6279 2073 7461 7220 6f72 2f61  ack by star or/a
+00002680: 6e64 2077 6174 6368 2072 6570 6f73 6974  nd watch reposit
+00002690: 6f72 792e 0a0a 4966 2079 6f75 2068 6176  ory...If you hav
+000026a0: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+000026b0: 6f72 2069 6465 6173 2061 626f 7574 2066  or ideas about f
+000026c0: 6561 7475 7265 7320 746f 2069 6d70 6c65  eatures to imple
+000026d0: 6d65 6e74 2c20 7765 6c63 6f6d 6520 746f  ment, welcome to
+000026e0: 205b 6469 7363 7573 7369 6f6e 735d 2868   [discussions](h
+000026f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002700: 6d2f 4c61 6e63 6574 6e69 6b2f 5072 6f70  m/Lancetnik/Prop
+00002710: 616e 2f64 6973 6375 7373 696f 6e73 292e  an/discussions).
+00002720: 0a0a 2d2d 2d0a 0a23 2320 4465 636c 6172  ..---..## Declar
+00002730: 6174 6976 653f 0a0a 5769 7468 2064 6563  ative?..With dec
+00002740: 6c61 7261 7469 7665 2074 6f6f 6c73 2079  larative tools y
+00002750: 6f75 2063 616e 2064 6566 696e 6520 2a2a  ou can define **
+00002760: 7768 6174 2079 6f75 206e 6565 6420 746f  what you need to
+00002770: 2067 6574 2a2a 2e20 5769 7468 2074 7261   get**. With tra
+00002780: 6469 7469 6f6e 616c 2069 6d70 6572 6174  ditional imperat
+00002790: 6976 6520 746f 6f6c 7320 796f 7520 6d75  ive tools you mu
+000027a0: 7374 2077 7269 7465 202a 2a77 6861 7420  st write **what 
+000027b0: 796f 7520 6e65 6564 2074 6f20 646f 2a2a  you need to do**
+000027c0: 2e0a 0a54 616b 6520 6120 6c6f 6f6b 2061  ...Take a look a
+000027d0: 7420 636c 6173 7369 6320 696d 7065 7261  t classic impera
+000027e0: 7469 7665 2074 6f6f 6c73 2c20 7375 6368  tive tools, such
+000027f0: 2061 7320 3c61 2068 7265 663d 2268 7474   as <a href="htt
+00002800: 7073 3a2f 2f61 696f 2d70 696b 612e 7265  ps://aio-pika.re
+00002810: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00002820: 6c61 7465 7374 2f22 2074 6172 6765 743d  latest/" target=
+00002830: 225f 626c 616e 6b22 3e61 696f 2d70 696b  "_blank">aio-pik
+00002840: 613c 2f61 3e2c 203c 6120 6872 6566 3d22  a</a>, <a href="
+00002850: 6874 7470 733a 2f2f 7069 6b61 2e72 6561  https://pika.rea
+00002860: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00002870: 7461 626c 652f 2220 7461 7267 6574 3d22  table/" target="
+00002880: 5f62 6c61 6e6b 223e 7069 6b61 3c2f 613e  _blank">pika</a>
+00002890: 2c20 3c61 2068 7265 663d 2268 7474 7073  , <a href="https
+000028a0: 3a2f 2f72 6564 6973 2e72 6561 6474 6865  ://redis.readthe
+000028b0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+000028c0: 652f 696e 6465 782e 6874 6d6c 2220 7461  e/index.html" ta
+000028d0: 7267 6574 3d22 5f62 6c61 6e6b 223e 7265  rget="_blank">re
+000028e0: 6469 732d 7079 3c2f 613e 2c20 3c61 2068  dis-py</a>, <a h
+000028f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00002900: 6875 622e 636f 6d2f 6e61 7473 2d69 6f2f  hub.com/nats-io/
+00002910: 6e61 7473 2e70 7922 2074 6172 6765 743d  nats.py" target=
+00002920: 225f 626c 616e 6b22 3e6e 6174 732d 7079  "_blank">nats-py
+00002930: 3c2f 613e 2c20 6574 632e 0a0a 5468 6973  </a>, etc...This
+00002940: 2069 7320 7468 6520 2a2a 5175 6963 6b73   is the **Quicks
+00002950: 7461 7274 2a2a 2077 6974 6820 7468 6520  tart** with the 
+00002960: 2a61 696f 2d70 696b 612a 3a0a 0a60 6060  *aio-pika*:..```
+00002970: 7079 7468 6f6e 0a69 6d70 6f72 7420 6173  python.import as
+00002980: 796e 6369 6f0a 696d 706f 7274 2061 696f  yncio.import aio
+00002990: 5f70 696b 610a 0a61 7379 6e63 2064 6566  _pika..async def
+000029a0: 206d 6169 6e28 293a 0a20 2020 2063 6f6e   main():.    con
+000029b0: 6e65 6374 696f 6e20 3d20 6177 6169 7420  nection = await 
+000029c0: 6169 6f5f 7069 6b61 2e63 6f6e 6e65 6374  aio_pika.connect
+000029d0: 5f72 6f62 7573 7428 0a20 2020 2020 2020  _robust(.       
+000029e0: 2022 616d 7170 3a2f 2f67 7565 7374 3a67   "amqp://guest:g
+000029f0: 7565 7374 4031 3237 2e30 2e30 2e31 2f22  uest@127.0.0.1/"
+00002a00: 0a20 2020 2029 0a0a 2020 2020 7175 6575  .    )..    queu
+00002a10: 655f 6e61 6d65 203d 2022 7465 7374 5f71  e_name = "test_q
+00002a20: 7565 7565 220a 0a20 2020 2061 7379 6e63  ueue"..    async
+00002a30: 2077 6974 6820 636f 6e6e 6563 7469 6f6e   with connection
+00002a40: 3a0a 2020 2020 2020 2020 6368 616e 6e65  :.        channe
+00002a50: 6c20 3d20 6177 6169 7420 636f 6e6e 6563  l = await connec
+00002a60: 7469 6f6e 2e63 6861 6e6e 656c 2829 0a0a  tion.channel()..
+00002a70: 2020 2020 2020 2020 7175 6575 6520 3d20          queue = 
+00002a80: 6177 6169 7420 6368 616e 6e65 6c2e 6465  await channel.de
+00002a90: 636c 6172 655f 7175 6575 6528 7175 6575  clare_queue(queu
+00002aa0: 655f 6e61 6d65 290a 0a20 2020 2020 2020  e_name)..       
+00002ab0: 2061 7379 6e63 2077 6974 6820 7175 6575   async with queu
+00002ac0: 652e 6974 6572 6174 6f72 2829 2061 7320  e.iterator() as 
+00002ad0: 7175 6575 655f 6974 6572 3a0a 2020 2020  queue_iter:.    
+00002ae0: 2020 2020 2020 2020 6173 796e 6320 666f          async fo
+00002af0: 7220 6d65 7373 6167 6520 696e 2071 7565  r message in que
+00002b00: 7565 5f69 7465 723a 0a20 2020 2020 2020  ue_iter:.       
+00002b10: 2020 2020 2020 2020 2061 7379 6e63 2077           async w
+00002b20: 6974 6820 6d65 7373 6167 652e 7072 6f63  ith message.proc
+00002b30: 6573 7328 293a 0a20 2020 2020 2020 2020  ess():.         
+00002b40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002b50: 286d 6573 7361 6765 2e62 6f64 7929 0a0a  (message.body)..
+00002b60: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
+00002b70: 2829 290a 6060 600a 0a2a 2a61 696f 2d70  ()).```..**aio-p
+00002b80: 696b 612a 2a20 6973 2061 2067 7265 6174  ika** is a great
+00002b90: 2074 6f6f 6c20 7769 7468 2061 2072 6561   tool with a rea
+00002ba0: 6c6c 7920 6561 7379 206c 6561 726e 696e  lly easy learnin
+00002bb0: 6720 6375 7276 652e 2042 7574 2069 7427  g curve. But it'
+00002bc0: 7320 7374 696c 6c20 696d 7065 7261 7469  s still imperati
+00002bd0: 7665 2e20 596f 7520 6e65 6564 2074 6f20  ve. You need to 
+00002be0: 2a63 6f6e 6e65 6374 2a2c 2064 6563 6c61  *connect*, decla
+00002bf0: 7265 202a 6368 616e 6e65 6c2a 2c20 2a71  re *channel*, *q
+00002c00: 7565 7565 732a 2c20 2a65 7863 6861 6e67  ueues*, *exchang
+00002c10: 6573 2a20 6279 2079 6f75 7273 656c 662e  es* by yourself.
+00002c20: 2041 6c73 6f2c 2079 6f75 206e 6565 6420   Also, you need 
+00002c30: 746f 206d 616e 6167 6520 2a63 6f6e 6e65  to manage *conne
+00002c40: 6374 696f 6e2a 2c20 2a6d 6573 7361 6765  ction*, *message
+00002c50: 2a2c 202a 7175 6575 652a 2063 6f6e 7465  *, *queue* conte
+00002c60: 7874 2074 6f20 6176 6f69 6420 616e 7920  xt to avoid any 
+00002c70: 7472 6f75 626c 6573 2e0a 0a49 7420 6973  troubles...It is
+00002c80: 206e 6f74 2061 2062 6164 2077 6179 2c20   not a bad way, 
+00002c90: 6275 7420 6974 2063 616e 2062 6520 6d75  but it can be mu
+00002ca0: 6368 2065 6173 6965 722e 0a0a 6060 6070  ch easier...```p
+00002cb0: 7974 686f 6e0a 6672 6f6d 2070 726f 7061  ython.from propa
+00002cc0: 6e20 696d 706f 7274 2050 726f 7061 6e41  n import PropanA
+00002cd0: 7070 2c20 5261 6262 6974 4272 6f6b 6572  pp, RabbitBroker
+00002ce0: 0a0a 6272 6f6b 6572 203d 2052 6162 6269  ..broker = Rabbi
+00002cf0: 7442 726f 6b65 7228 2261 6d71 703a 2f2f  tBroker("amqp://
+00002d00: 6775 6573 743a 6775 6573 7440 6c6f 6361  guest:guest@loca
+00002d10: 6c68 6f73 743a 3536 3732 2f22 290a 0a61  lhost:5672/")..a
+00002d20: 7070 203d 2050 726f 7061 6e41 7070 2862  pp = PropanApp(b
+00002d30: 726f 6b65 7229 0a0a 4062 726f 6b65 722e  roker)..@broker.
+00002d40: 6861 6e64 6c65 2822 7465 7374 5f71 7565  handle("test_que
+00002d50: 7565 2229 0a61 7379 6e63 2064 6566 2062  ue").async def b
+00002d60: 6173 655f 6861 6e64 6c65 7228 626f 6479  ase_handler(body
+00002d70: 293a 0a20 2020 2070 7269 6e74 2862 6f64  ):.    print(bod
+00002d80: 7929 0a60 6060 0a0a 5468 6973 2069 7320  y).```..This is 
+00002d90: 7468 6520 2a2a 5072 6f70 616e 2a2a 2064  the **Propan** d
+00002da0: 6563 6c61 7261 7469 7665 2077 6179 2074  eclarative way t
+00002db0: 6f20 7772 6974 6520 7468 6520 7361 6d65  o write the same
+00002dc0: 2063 6f64 652e 2054 6861 7420 6973 2073   code. That is s
+00002dd0: 6f20 6d75 6368 2065 6173 6965 722c 2069  o much easier, i
+00002de0: 736e 2774 2069 743f 0a0a 2d2d 2d0a 0a23  sn't it?..---..#
+00002df0: 2320 5175 6963 6b73 7461 7274 0a0a 496e  # Quickstart..In
+00002e00: 7374 616c 6c20 7573 696e 6720 6070 6970  stall using `pip
+00002e10: 603a 0a0a 6060 6073 6865 6c6c 0a70 6970  `:..```shell.pip
+00002e20: 2069 6e73 7461 6c6c 2022 7072 6f70 616e   install "propan
+00002e30: 5b61 7379 6e63 2d72 6162 6269 745d 220a  [async-rabbit]".
+00002e40: 2320 6f72 0a70 6970 2069 6e73 7461 6c6c  # or.pip install
+00002e50: 2022 7072 6f70 616e 5b61 7379 6e63 2d6e   "propan[async-n
+00002e60: 6174 735d 220a 2320 6f72 0a70 6970 2069  ats]".# or.pip i
+00002e70: 6e73 7461 6c6c 2022 7072 6f70 616e 5b61  nstall "propan[a
+00002e80: 7379 6e63 2d72 6564 6973 5d22 0a23 206f  sync-redis]".# o
+00002e90: 720a 7069 7020 696e 7374 616c 6c20 2270  r.pip install "p
+00002ea0: 726f 7061 6e5b 6173 796e 632d 6b61 666b  ropan[async-kafk
+00002eb0: 615d 220a 2320 6f72 0a70 6970 2069 6e73  a]".# or.pip ins
+00002ec0: 7461 6c6c 2022 7072 6f70 616e 5b61 7379  tall "propan[asy
+00002ed0: 6e63 2d73 7173 5d22 0a60 6060 0a0a 2323  nc-sqs]".```..##
+00002ee0: 2320 4261 7369 6320 7573 6167 650a 0a43  # Basic usage..C
+00002ef0: 7265 6174 6520 616e 2061 7070 6c69 6361  reate an applica
+00002f00: 7469 6f6e 2077 6974 6820 7468 6520 666f  tion with the fo
+00002f10: 6c6c 6f77 696e 6720 636f 6465 2061 7420  llowing code at 
+00002f20: 6073 6572 7665 2e70 7960 3a0a 0a60 6060  `serve.py`:..```
+00002f30: 7079 7468 6f6e 0a66 726f 6d20 7072 6f70  python.from prop
+00002f40: 616e 2069 6d70 6f72 7420 5072 6f70 616e  an import Propan
+00002f50: 4170 700a 6672 6f6d 2070 726f 7061 6e20  App.from propan 
+00002f60: 696d 706f 7274 2052 6162 6269 7442 726f  import RabbitBro
+00002f70: 6b65 720a 2320 6672 6f6d 2070 726f 7061  ker.# from propa
+00002f80: 6e20 696d 706f 7274 2052 6564 6973 4272  n import RedisBr
+00002f90: 6f6b 6572 0a23 2066 726f 6d20 7072 6f70  oker.# from prop
+00002fa0: 616e 2069 6d70 6f72 7420 4e61 7473 4272  an import NatsBr
+00002fb0: 6f6b 6572 0a23 2066 726f 6d20 7072 6f70  oker.# from prop
+00002fc0: 616e 2069 6d70 6f72 7420 5351 5342 726f  an import SQSBro
+00002fd0: 6b65 720a 2320 6672 6f6d 2070 726f 7061  ker.# from propa
+00002fe0: 6e20 696d 706f 7274 204b 6166 6b61 4272  n import KafkaBr
+00002ff0: 6f6b 6572 0a0a 6272 6f6b 6572 203d 2052  oker..broker = R
+00003000: 6162 6269 7442 726f 6b65 7228 2261 6d71  abbitBroker("amq
+00003010: 703a 2f2f 6775 6573 743a 6775 6573 7440  p://guest:guest@
+00003020: 6c6f 6361 6c68 6f73 743a 3536 3732 2f22  localhost:5672/"
+00003030: 290a 2320 6272 6f6b 6572 203d 204e 6174  ).# broker = Nat
+00003040: 7342 726f 6b65 7228 226e 6174 733a 2f2f  sBroker("nats://
+00003050: 6c6f 6361 6c68 6f73 743a 3432 3232 2229  localhost:4222")
+00003060: 0a23 2062 726f 6b65 7220 3d20 5265 6469  .# broker = Redi
+00003070: 7342 726f 6b65 7228 2272 6564 6973 3a2f  sBroker("redis:/
+00003080: 2f6c 6f63 616c 686f 7374 3a36 3337 3922  /localhost:6379"
+00003090: 290a 2320 6272 6f6b 6572 203d 2053 5153  ).# broker = SQS
+000030a0: 4272 6f6b 6572 2822 6874 7470 3a2f 2f6c  Broker("http://l
+000030b0: 6f63 616c 686f 7374 3a39 3332 3422 2c20  ocalhost:9324", 
+000030c0: 2e2e 2e29 0a23 2062 726f 6b65 7220 3d20  ...).# broker = 
+000030d0: 4b61 666b 6142 726f 6b65 7228 226c 6f63  KafkaBroker("loc
+000030e0: 616c 686f 7374 3a39 3039 3222 290a 0a61  alhost:9092")..a
+000030f0: 7070 203d 2050 726f 7061 6e41 7070 2862  pp = PropanApp(b
+00003100: 726f 6b65 7229 0a0a 4062 726f 6b65 722e  roker)..@broker.
+00003110: 6861 6e64 6c65 2822 7465 7374 2229 0a61  handle("test").a
+00003120: 7379 6e63 2064 6566 2062 6173 655f 6861  sync def base_ha
+00003130: 6e64 6c65 7228 626f 6479 293a 0a20 2020  ndler(body):.   
+00003140: 2027 2727 4861 6e64 6c65 2061 6c6c 2064   '''Handle all d
+00003150: 6566 6175 6c74 2065 7863 6861 6e67 6520  efault exchange 
+00003160: 6d65 7373 6167 6573 2077 6974 6820 6074  messages with `t
+00003170: 6573 7460 2072 6f75 7469 6e67 206b 6579  est` routing key
+00003180: 2727 270a 2020 2020 7072 696e 7428 626f  '''.    print(bo
+00003190: 6479 290a 6060 600a 0a41 6e64 206a 7573  dy).```..And jus
+000031a0: 7420 7275 6e20 6974 3a0a 0a60 6060 7368  t run it:..```sh
+000031b0: 656c 6c0a 7072 6f70 616e 2072 756e 2073  ell.propan run s
+000031c0: 6572 7665 3a61 7070 0a60 6060 0a0a 2d2d  erve:app.```..--
+000031d0: 2d0a 0a23 2320 5479 7065 2063 6173 7469  -..## Type casti
+000031e0: 6e67 0a0a 5072 6f70 616e 2075 7365 7320  ng..Propan uses 
+000031f0: 6070 7964 616e 7469 6360 2074 6f20 6361  `pydantic` to ca
+00003200: 7374 2069 6e63 6f6d 696e 6720 6675 6e63  st incoming func
+00003210: 7469 6f6e 2061 7267 756d 656e 7473 2074  tion arguments t
+00003220: 6f20 7479 7065 7320 6163 636f 7264 696e  o types accordin
+00003230: 6720 746f 2074 6865 6972 2061 6e6e 6f74  g to their annot
+00003240: 6174 696f 6e2e 0a0a 6060 6070 7974 686f  ation...```pytho
+00003250: 6e0a 6672 6f6d 2070 7964 616e 7469 6320  n.from pydantic 
+00003260: 696d 706f 7274 2042 6173 654d 6f64 656c  import BaseModel
+00003270: 0a66 726f 6d20 7072 6f70 616e 2069 6d70  .from propan imp
+00003280: 6f72 7420 5072 6f70 616e 4170 702c 2043  ort PropanApp, C
+00003290: 6f6e 7465 7874 2c20 5261 6262 6974 4272  ontext, RabbitBr
+000032a0: 6f6b 6572 0a0a 6272 6f6b 6572 203d 2052  oker..broker = R
+000032b0: 6162 6269 7442 726f 6b65 7228 2261 6d71  abbitBroker("amq
+000032c0: 703a 2f2f 6775 6573 743a 6775 6573 7440  p://guest:guest@
+000032d0: 6c6f 6361 6c68 6f73 743a 3536 3732 2f22  localhost:5672/"
+000032e0: 290a 6170 7020 3d20 5072 6f70 616e 4170  ).app = PropanAp
+000032f0: 7028 6272 6f6b 6572 290a 0a63 6c61 7373  p(broker)..class
+00003300: 2053 696d 706c 654d 6573 7361 6765 2842   SimpleMessage(B
+00003310: 6173 654d 6f64 656c 293a 0a20 2020 206b  aseModel):.    k
+00003320: 6579 3a20 696e 740a 0a40 6272 6f6b 6572  ey: int..@broker
+00003330: 2e68 616e 646c 6528 2274 6573 7432 2229  .handle("test2")
+00003340: 0a61 7379 6e63 2064 6566 2073 6563 6f6e  .async def secon
+00003350: 645f 6861 6e64 6c65 7228 626f 6479 3a20  d_handler(body: 
+00003360: 5369 6d70 6c65 4d65 7373 6167 6529 3a0a  SimpleMessage):.
+00003370: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00003380: 7461 6e63 6528 626f 6479 2e6b 6579 2c20  tance(body.key, 
+00003390: 696e 7429 0a0a 6060 600a 0a2d 2d2d 0a0a  int)..```..---..
+000033a0: 2323 2044 6570 656e 6465 6e63 6965 730a  ## Dependencies.
+000033b0: 0a2a 2a50 726f 7061 6e2a 2a20 6120 6861  .**Propan** a ha
+000033c0: 7320 6465 7065 6e64 656e 6369 6573 206d  s dependencies m
+000033d0: 616e 6167 656d 656e 7420 706f 6c69 6379  anagement policy
+000033e0: 2063 6c6f 7365 2074 6f20 6070 7974 6573   close to `pytes
+000033f0: 7420 6669 7874 7572 6573 602e 0a59 6f75  t fixtures`..You
+00003400: 2063 616e 2073 7065 6369 6679 2069 6e20   can specify in 
+00003410: 6675 6e63 7469 6f6e 7320 6172 6775 6d65  functions argume
+00003420: 6e74 7320 7768 6963 6820 6465 7065 6e64  nts which depend
+00003430: 656e 6369 6573 0a79 6f75 2077 6f75 6c64  encies.you would
+00003440: 2074 6f20 7573 652e 2046 7261 6d65 776f   to use. Framewo
+00003450: 726b 2070 6173 7365 7320 7468 656d 2066  rk passes them f
+00003460: 726f 6d20 7468 6520 676c 6f62 616c 2043  rom the global C
+00003470: 6f6e 7465 7874 206f 626a 6563 742e 0a0a  ontext object...
+00003480: 416c 7265 6164 7920 6578 6973 7465 6420  Already existed 
+00003490: 636f 6e74 6578 7420 6669 656c 6473 2061  context fields a
+000034a0: 7265 3a20 2a61 7070 2a2c 202a 6272 6f6b  re: *app*, *brok
+000034b0: 6572 2a2c 202a 636f 6e74 6578 742a 2028  er*, *context* (
+000034c0: 6974 7365 6c66 292c 202a 6c6f 6767 6572  itself), *logger
+000034d0: 2a20 616e 6420 2a6d 6573 7361 6765 2a2e  * and *message*.
+000034e0: 0a49 6620 796f 7520 6361 6c6c 206e 6f74  .If you call not
+000034f0: 2065 7869 7374 696e 6720 6669 656c 642c   existing field,
+00003500: 2072 6169 7365 7320 2a70 7964 616e 7469   raises *pydanti
+00003510: 632e 5661 6c69 6461 7469 6f6e 4572 726f  c.ValidationErro
+00003520: 722a 2076 616c 7565 2e0a 0a42 7574 2079  r* value...But y
+00003530: 6f75 2063 616e 2073 7065 6369 6679 2079  ou can specify y
+00003540: 6f75 7220 6f77 6e20 6465 7065 6e64 656e  our own dependen
+00003550: 6369 6573 2c20 6361 6c6c 2064 6570 656e  cies, call depen
+00003560: 6465 6e63 6965 7320 6675 6e63 7469 6f6e  dencies function
+00003570: 7320 286c 696b 6520 6046 6173 7461 7069  s (like `Fastapi
+00003580: 2044 6570 656e 6473 6029 0a61 6e64 205b   Depends`).and [
+00003590: 6d6f 7265 5d28 6874 7470 733a 2f2f 6769  more](https://gi
+000035a0: 7468 7562 2e63 6f6d 2f4c 616e 6365 746e  thub.com/Lancetn
+000035b0: 696b 2f50 726f 7061 6e2f 7472 6565 2f6d  ik/Propan/tree/m
+000035c0: 6169 6e2f 6578 616d 706c 6573 2f64 6570  ain/examples/dep
+000035d0: 656e 6465 6e63 6965 7329 2e0a 0a60 6060  endencies)...```
+000035e0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6169  python.import ai
+000035f0: 6f5f 7069 6b61 0a66 726f 6d20 7072 6f70  o_pika.from prop
+00003600: 616e 2069 6d70 6f72 7420 5072 6f70 616e  an import Propan
+00003610: 4170 702c 2052 6162 6269 7442 726f 6b65  App, RabbitBroke
+00003620: 722c 2043 6f6e 7465 7874 2c20 4465 7065  r, Context, Depe
+00003630: 6e64 730a 0a72 6162 6269 745f 6272 6f6b  nds..rabbit_brok
+00003640: 6572 203d 2052 6162 6269 7442 726f 6b65  er = RabbitBroke
+00003650: 7228 2261 6d71 703a 2f2f 6775 6573 743a  r("amqp://guest:
+00003660: 6775 6573 7440 6c6f 6361 6c68 6f73 743a  guest@localhost:
+00003670: 3536 3732 2f22 290a 0a61 7070 203d 2050  5672/")..app = P
+00003680: 726f 7061 6e41 7070 2872 6162 6269 745f  ropanApp(rabbit_
+00003690: 6272 6f6b 6572 290a 0a61 7379 6e63 2064  broker)..async d
+000036a0: 6566 2064 6570 656e 6465 6e63 7928 626f  ef dependency(bo
+000036b0: 6479 3a20 6469 6374 2920 2d3e 2062 6f6f  dy: dict) -> boo
+000036c0: 6c3a 0a20 2020 2072 6574 7572 6e20 5472  l:.    return Tr
+000036d0: 7565 0a0a 4072 6162 6269 745f 6272 6f6b  ue..@rabbit_brok
+000036e0: 6572 2e68 616e 646c 6528 2274 6573 7422  er.handle("test"
+000036f0: 290a 6173 796e 6320 6465 6620 6261 7365  ).async def base
+00003700: 5f68 616e 646c 6572 2862 6f64 793a 2064  _handler(body: d
+00003710: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+00003720: 2020 2020 2020 2020 2020 2020 6465 703a              dep:
+00003730: 2062 6f6f 6c20 3d20 4465 7065 6e64 7328   bool = Depends(
+00003740: 6465 7065 6e64 656e 6379 292c 0a20 2020  dependency),.   
+00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003760: 2020 2020 6272 6f6b 6572 3a20 5261 6262      broker: Rabb
+00003770: 6974 4272 6f6b 6572 203d 2043 6f6e 7465  itBroker = Conte
+00003780: 7874 2829 293a 0a20 2020 2061 7373 6572  xt()):.    asser
+00003790: 7420 6465 7020 6973 2054 7275 650a 2020  t dep is True.  
+000037a0: 2020 6173 7365 7274 2062 726f 6b65 7220    assert broker 
+000037b0: 6973 2072 6162 6269 745f 6272 6f6b 6572  is rabbit_broker
+000037c0: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 5072  .```..---..## Pr
+000037d0: 6f6a 6563 7420 446f 6375 6d65 6e74 6174  oject Documentat
+000037e0: 696f 6e0a 0a2a 2a50 726f 7061 6e2a 2a20  ion..**Propan** 
+000037f0: 6175 746f 6d61 7469 6361 6c6c 7920 6765  automatically ge
+00003800: 6e65 7261 7465 7320 646f 6375 6d65 6e74  nerates document
+00003810: 6174 696f 6e20 666f 7220 796f 7572 2070  ation for your p
+00003820: 726f 6a65 6374 2061 6363 6f72 6469 6e67  roject according
+00003830: 2074 6f20 7468 6520 3c61 2068 7265 663d   to the <a href=
+00003840: 2268 7474 7073 3a2f 2f77 7777 2e61 7379  "https://www.asy
+00003850: 6e63 6170 692e 636f 6d2f 2220 7461 7267  ncapi.com/" targ
+00003860: 6574 3d22 5f62 6c61 6e6b 223e 2a2a 4173  et="_blank">**As
+00003870: 796e 6341 5049 2a2a 3c2f 613e 2073 7065  yncAPI**</a> spe
+00003880: 6369 6669 6361 7469 6f6e 2e20 596f 7520  cification. You 
+00003890: 6361 6e20 776f 726b 2077 6974 6820 626f  can work with bo
+000038a0: 7468 2067 656e 6572 6174 6564 2061 7274  th generated art
+000038b0: 6966 6163 7473 2061 6e64 2070 6c61 6365  ifacts and place
+000038c0: 2061 2057 6562 2076 6965 7720 6f66 2079   a Web view of y
+000038d0: 6f75 7220 646f 6375 6d65 6e74 6174 696f  our documentatio
+000038e0: 6e20 6f6e 2072 6573 6f75 7263 6573 2061  n on resources a
+000038f0: 7661 696c 6162 6c65 2074 6f20 7265 6c61  vailable to rela
+00003900: 7465 6420 7465 616d 732e 0a0a 5468 6520  ted teams...The 
+00003910: 6176 6169 6c61 6269 6c69 7479 206f 6620  availability of 
+00003920: 7375 6368 2064 6f63 756d 656e 7461 7469  such documentati
+00003930: 6f6e 2073 6967 6e69 6669 6361 6e74 6c79  on significantly
+00003940: 2073 696d 706c 6966 6965 7320 7468 6520   simplifies the 
+00003950: 696e 7465 6772 6174 696f 6e20 6f66 2073  integration of s
+00003960: 6572 7669 6365 733a 2079 6f75 2063 616e  ervices: you can
+00003970: 2069 6d6d 6564 6961 7465 6c79 2073 6565   immediately see
+00003980: 2077 6861 7420 6368 616e 6e65 6c73 2061   what channels a
+00003990: 6e64 206d 6573 7361 6765 2066 6f72 6d61  nd message forma
+000039a0: 7420 7468 6520 6170 706c 6963 6174 696f  t the applicatio
+000039b0: 6e20 776f 726b 7320 7769 7468 2e20 416e  n works with. An
+000039c0: 6420 6d6f 7374 2069 6d70 6f72 7461 6e74  d most important
+000039d0: 6c79 2c20 6974 2064 6f65 736e 2774 2063  ly, it doesn't c
+000039e0: 6f73 7420 796f 7520 616e 7974 6869 6e67  ost you anything
+000039f0: 202d 202a 2a50 726f 7061 6e2a 2a20 6861   - **Propan** ha
+00003a00: 7320 616c 7265 6164 7920 646f 6e65 2065  s already done e
+00003a10: 7665 7279 7468 696e 6720 666f 7220 796f  verything for yo
+00003a20: 7521 0a0a 215b 4854 4d4c 2d70 6167 655d  u!..![HTML-page]
+00003a30: 2868 7474 7073 3a2f 2f6c 616e 6365 746e  (https://lancetn
+00003a40: 696b 2e67 6974 6875 622e 696f 2f50 726f  ik.github.io/Pro
+00003a50: 7061 6e2f 6173 7365 7473 2f69 6d67 2f64  pan/assets/img/d
+00003a60: 6f63 732d 6874 6d6c 2d73 686f 7274 2e70  ocs-html-short.p
+00003a70: 6e67 290a 0a2d 2d2d 0a0a 2323 2043 4c49  ng)..---..## CLI
+00003a80: 2070 6f77 6572 0a0a 2a2a 5072 6f70 616e   power..**Propan
+00003a90: 2a2a 2068 6173 2069 7473 206f 776e 2043  ** has its own C
+00003aa0: 4c49 2074 6f6f 6c20 7468 6174 2070 726f  LI tool that pro
+00003ab0: 7669 6465 6420 7468 6520 666f 6c6c 6f77  vided the follow
+00003ac0: 696e 6720 6665 6174 7572 6573 3a0a 0a2a  ing features:..*
+00003ad0: 2070 726f 6a65 6374 2067 656e 6572 6174   project generat
+00003ae0: 696f 6e0a 2a20 6d75 6c74 6970 726f 6365  ion.* multiproce
+00003af0: 7373 696e 6720 776f 726b 6572 730a 2a20  ssing workers.* 
+00003b00: 7072 6f6a 6563 7420 686f 7420 7265 6c6f  project hot relo
+00003b10: 6164 696e 670a 2a20 6375 7374 6f6d 2063  ading.* custom c
+00003b20: 6f6d 6d61 6e64 206c 696e 6520 6172 6775  ommand line argu
+00003b30: 6d65 6e74 7320 7061 7373 696e 670a 0a23  ments passing..#
+00003b40: 2323 2043 6f6e 7465 7874 2070 6173 7369  ## Context passi
+00003b50: 6e67 0a0a 466f 7220 6578 616d 706c 653a  ng..For example:
+00003b60: 2070 6173 7320 796f 7572 2063 7572 7265   pass your curre
+00003b70: 6e74 202a 2e65 6e76 2a20 7072 6f6a 6563  nt *.env* projec
+00003b80: 7420 7365 7474 696e 6720 746f 2063 6f6e  t setting to con
+00003b90: 7465 7874 0a0a 6060 6062 6173 680a 7072  text..```bash.pr
+00003ba0: 6f70 616e 2072 756e 2073 6572 7665 3a61  opan run serve:a
+00003bb0: 7070 202d 2d65 6e76 3d2e 656e 762e 6465  pp --env=.env.de
+00003bc0: 760a 6060 600a 0a60 6060 7079 7468 6f6e  v.```..```python
+00003bd0: 0a66 726f 6d20 7072 6f70 616e 2069 6d70  .from propan imp
+00003be0: 6f72 7420 5072 6f70 616e 4170 702c 2052  ort PropanApp, R
+00003bf0: 6162 6269 7442 726f 6b65 720a 6672 6f6d  abbitBroker.from
+00003c00: 2070 726f 7061 6e2e 616e 6e6f 7461 7469   propan.annotati
+00003c10: 6f6e 7320 696d 706f 7274 2043 6f6e 7465  ons import Conte
+00003c20: 7874 5265 706f 0a66 726f 6d20 7079 6461  xtRepo.from pyda
+00003c30: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
+00003c40: 5365 7474 696e 6773 0a0a 6272 6f6b 6572  Settings..broker
+00003c50: 203d 2052 6162 6269 7442 726f 6b65 7228   = RabbitBroker(
+00003c60: 2261 6d71 703a 2f2f 6775 6573 743a 6775  "amqp://guest:gu
+00003c70: 6573 7440 6c6f 6361 6c68 6f73 743a 3536  est@localhost:56
+00003c80: 3732 2f22 290a 0a61 7070 203d 2050 726f  72/")..app = Pro
+00003c90: 7061 6e41 7070 2862 726f 6b65 7229 0a0a  panApp(broker)..
+00003ca0: 636c 6173 7320 5365 7474 696e 6773 2842  class Settings(B
+00003cb0: 6173 6553 6574 7469 6e67 7329 3a0a 2020  aseSettings):.  
+00003cc0: 2020 2e2e 2e0a 0a40 6170 702e 6f6e 5f73    .....@app.on_s
+00003cd0: 7461 7274 7570 0a61 7379 6e63 2064 6566  tartup.async def
+00003ce0: 2073 6574 7570 2865 6e76 3a20 7374 722c   setup(env: str,
+00003cf0: 2063 6f6e 7465 7874 3a20 436f 6e74 6578   context: Contex
+00003d00: 7452 6570 6f29 3a0a 2020 2020 7365 7474  tRepo):.    sett
+00003d10: 696e 6773 203d 2053 6574 7469 6e67 7328  ings = Settings(
+00003d20: 5f65 6e76 5f66 696c 653d 656e 7629 0a20  _env_file=env). 
+00003d30: 2020 2063 6f6e 7465 7874 2e73 6574 5f67     context.set_g
+00003d40: 6c6f 6261 6c28 2273 6574 7469 6e67 7322  lobal("settings"
+00003d50: 2c20 7365 7474 696e 6773 290a 6060 600a  , settings).```.
+00003d60: 0a23 2323 2050 726f 6a65 6374 2074 656d  .### Project tem
+00003d70: 706c 6174 650a 0a41 6c73 6f2c 202a 2a50  plate..Also, **P
+00003d80: 726f 7061 6e20 434c 492a 2a20 6973 2061  ropan CLI** is a
+00003d90: 626c 6520 746f 2067 656e 6572 6174 6520  ble to generate 
+00003da0: 6120 7072 6f64 7563 7469 6f6e 2d72 6561  a production-rea
+00003db0: 6479 2061 7070 6c69 6361 7469 6f6e 2074  dy application t
+00003dc0: 656d 706c 6174 653a 0a0a 6060 6062 6173  emplate:..```bas
+00003dd0: 680a 7072 6f70 616e 2063 7265 6174 6520  h.propan create 
+00003de0: 6173 796e 6320 7261 6262 6974 205b 7072  async rabbit [pr
+00003df0: 6f6a 6563 746e 616d 655d 0a60 6060 0a0a  ojectname].```..
+00003e00: 2a4e 6f74 6963 653a 2070 726f 6a65 6374  *Notice: project
+00003e10: 2074 656d 706c 6174 6520 7265 7175 6972   template requir
+00003e20: 652a 2060 7079 6461 6e74 6963 5b64 6f74  e* `pydantic[dot
+00003e30: 656e 765d 6020 2a69 6e73 7461 6c6c 6174  env]` *installat
+00003e40: 696f 6e2e 2a0a 0a52 756e 2074 6865 2063  ion.*..Run the c
+00003e50: 7265 6174 6564 2070 726f 6a65 6374 3a0a  reated project:.
+00003e60: 0a60 6060 6261 7368 0a23 2052 756e 2072  .```bash.# Run r
+00003e70: 6162 6269 6d71 2066 6972 7374 0a64 6f63  abbimq first.doc
+00003e80: 6b65 7220 636f 6d70 6f73 6520 2d2d 6669  ker compose --fi
+00003e90: 6c65 205b 7072 6f6a 6563 746e 616d 655d  le [projectname]
+00003ea0: 2f64 6f63 6b65 722d 636f 6d70 6f73 652e  /docker-compose.
+00003eb0: 7961 6d6c 2075 7020 2d64 0a0a 2320 5275  yaml up -d..# Ru
+00003ec0: 6e20 7072 6f6a 6563 740a 7072 6f70 616e  n project.propan
+00003ed0: 2072 756e 205b 7072 6f6a 6563 746e 616d   run [projectnam
+00003ee0: 655d 2e61 7070 2e73 6572 7665 3a61 7070  e].app.serve:app
+00003ef0: 202d 2d65 6e76 3d2e 656e 7620 2d2d 7265   --env=.env --re
+00003f00: 6c6f 6164 0a60 6060 0a0a 4e6f 7720 796f  load.```..Now yo
+00003f10: 7520 6361 6e20 656e 6a6f 7920 6120 6e65  u can enjoy a ne
+00003f20: 7720 6465 7665 6c6f 706d 656e 7420 6578  w development ex
+00003f30: 7065 7269 656e 6365 210a 0a2d 2d2d 0a0a  perience!..---..
+00003f40: 2323 2048 5454 5020 4672 616d 6577 6f72  ## HTTP Framewor
+00003f50: 6b73 2069 6e74 6567 7261 7469 6f6e 730a  ks integrations.
+00003f60: 0a23 2323 2041 6e79 2046 7261 6d65 776f  .### Any Framewo
+00003f70: 726b 0a0a 596f 7520 6361 6e20 7573 6520  rk..You can use 
+00003f80: 2a2a 5072 6f70 616e 2a2a 2060 4d51 4272  **Propan** `MQBr
+00003f90: 6f6b 6572 7360 2077 6974 686f 7574 2060  okers` without `
+00003fa0: 5072 6f70 616e 4170 7060 2e0a 4a75 7374  PropanApp`..Just
+00003fb0: 202a 7374 6172 742a 2061 6e64 202a 7374   *start* and *st
+00003fc0: 6f70 2a20 7468 656d 2061 6363 6f72 6469  op* them accordi
+00003fd0: 6e67 2074 6f20 796f 7572 2061 7070 6c69  ng to your appli
+00003fe0: 6361 7469 6f6e 206c 6966 6573 7061 6e2e  cation lifespan.
+00003ff0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00004000: 2070 726f 7061 6e20 696d 706f 7274 204e   propan import N
+00004010: 6174 7342 726f 6b65 720a 6672 6f6d 2073  atsBroker.from s
+00004020: 616e 6963 2069 6d70 6f72 7420 5361 6e69  anic import Sani
+00004030: 630a 0a61 7070 203d 2053 616e 6963 2822  c..app = Sanic("
+00004040: 4d79 4865 6c6c 6f57 6f72 6c64 4170 7022  MyHelloWorldApp"
+00004050: 290a 6272 6f6b 6572 203d 204e 6174 7342  ).broker = NatsB
+00004060: 726f 6b65 7228 226e 6174 733a 2f2f 6c6f  roker("nats://lo
+00004070: 6361 6c68 6f73 743a 3432 3232 2229 0a0a  calhost:4222")..
+00004080: 4062 726f 6b65 722e 6861 6e64 6c65 2822  @broker.handle("
+00004090: 7465 7374 2229 0a61 7379 6e63 2064 6566  test").async def
+000040a0: 2062 6173 655f 6861 6e64 6c65 7228 626f   base_handler(bo
+000040b0: 6479 293a 0a20 2020 2070 7269 6e74 2862  dy):.    print(b
+000040c0: 6f64 7929 0a0a 4061 7070 2e61 6674 6572  ody)..@app.after
+000040d0: 5f73 6572 7665 725f 7374 6172 740a 6173  _server_start.as
+000040e0: 796e 6320 6465 6620 7374 6172 745f 6272  ync def start_br
+000040f0: 6f6b 6572 2861 7070 2c20 6c6f 6f70 293a  oker(app, loop):
+00004100: 0a20 2020 2061 7761 6974 2062 726f 6b65  .    await broke
+00004110: 722e 7374 6172 7428 290a 0a40 6170 702e  r.start()..@app.
+00004120: 6166 7465 725f 7365 7276 6572 5f73 746f  after_server_sto
+00004130: 700a 6173 796e 6320 6465 6620 7374 6f70  p.async def stop
+00004140: 5f62 726f 6b65 7228 6170 702c 206c 6f6f  _broker(app, loo
+00004150: 7029 3a0a 2020 2020 6177 6169 7420 6272  p):.    await br
+00004160: 6f6b 6572 2e63 6c6f 7365 2829 0a60 6060  oker.close().```
+00004170: 0a0a 2323 2320 4661 7374 4150 4920 506c  ..### FastAPI Pl
+00004180: 7567 696e 0a0a 416c 736f 2c20 2a2a 5072  ugin..Also, **Pr
+00004190: 6f70 616e 2a2a 2063 616e 2062 6520 7573  opan** can be us
+000041a0: 6564 2061 7320 7061 7274 206f 6620 2a2a  ed as part of **
+000041b0: 4661 7374 4150 492a 2a2e 0a0a 4a75 7374  FastAPI**...Just
+000041c0: 2069 6d70 6f72 7420 6120 2a2a 5072 6f70   import a **Prop
+000041d0: 616e 526f 7574 6572 2a2a 2079 6f75 206e  anRouter** you n
+000041e0: 6565 6420 616e 6420 6465 636c 6172 6520  eed and declare 
+000041f0: 7468 6520 6d65 7373 6167 6520 6861 6e64  the message hand
+00004200: 6c65 720a 7573 696e 6720 7468 6520 6040  ler.using the `@
+00004210: 6576 656e 7460 2064 6563 6f72 6174 6f72  event` decorator
+00004220: 2e20 5468 6973 2064 6563 6f72 6174 6f72  . This decorator
+00004230: 2069 7320 7369 6d69 6c61 7220 746f 2074   is similar to t
+00004240: 6865 2064 6563 6f72 6174 6f72 2060 4068  he decorator `@h
+00004250: 616e 646c 6560 2066 6f72 2074 6865 2063  andle` for the c
+00004260: 6f72 7265 7370 6f6e 6469 6e67 2062 726f  orresponding bro
+00004270: 6b65 7273 2e0a 0a60 6060 7079 7468 6f6e  kers...```python
+00004280: 0a66 726f 6d20 6661 7374 6170 6920 696d  .from fastapi im
+00004290: 706f 7274 2044 6570 656e 6473 2c20 4661  port Depends, Fa
+000042a0: 7374 4150 490a 6672 6f6d 2070 7964 616e  stAPI.from pydan
+000042b0: 7469 6320 696d 706f 7274 2042 6173 654d  tic import BaseM
+000042c0: 6f64 656c 0a66 726f 6d20 7072 6f70 616e  odel.from propan
+000042d0: 2e66 6173 7461 7069 2069 6d70 6f72 7420  .fastapi import 
+000042e0: 5261 6262 6974 526f 7574 6572 0a0a 726f  RabbitRouter..ro
+000042f0: 7574 6572 203d 2052 6162 6269 7452 6f75  uter = RabbitRou
+00004300: 7465 7228 2261 6d71 703a 2f2f 6775 6573  ter("amqp://gues
+00004310: 743a 6775 6573 7440 6c6f 6361 6c68 6f73  t:guest@localhos
+00004320: 743a 3536 3732 2229 0a0a 6170 7020 3d20  t:5672")..app = 
+00004330: 4661 7374 4150 4928 6c69 6665 7370 616e  FastAPI(lifespan
+00004340: 3d72 6f75 7465 722e 6c69 6665 7370 616e  =router.lifespan
+00004350: 5f63 6f6e 7465 7874 290a 0a63 6c61 7373  _context)..class
+00004360: 2049 6e63 6f6d 696e 6728 4261 7365 4d6f   Incoming(BaseMo
+00004370: 6465 6c29 3a0a 2020 2020 6d3a 2064 6963  del):.    m: dic
+00004380: 740a 0a64 6566 2063 616c 6c28 293a 0a20  t..def call():. 
+00004390: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+000043a0: 4072 6f75 7465 722e 6576 656e 7428 2274  @router.event("t
+000043b0: 6573 7422 290a 6173 796e 6320 6465 6620  est").async def 
+000043c0: 6865 6c6c 6f28 6d3a 2049 6e63 6f6d 696e  hello(m: Incomin
+000043d0: 672c 2064 203d 2044 6570 656e 6473 2863  g, d = Depends(c
+000043e0: 616c 6c29 2920 2d3e 2064 6963 743a 0a20  all)) -> dict:. 
+000043f0: 2020 2072 6574 7572 6e20 7b20 2272 6573     return { "res
+00004400: 706f 6e73 6522 3a20 2248 656c 6c6f 2c20  ponse": "Hello, 
+00004410: 5072 6f70 616e 2122 207d 0a0a 6170 702e  Propan!" }..app.
+00004420: 696e 636c 7564 655f 726f 7574 6572 2872  include_router(r
+00004430: 6f75 7465 7229 0a60 6060 0a0a 2323 2045  outer).```..## E
+00004440: 7861 6d70 6c65 730a 0a54 6f20 7365 6520  xamples..To see 
+00004450: 6d6f 7265 2066 7261 6d65 776f 726b 2075  more framework u
+00004460: 7361 6765 7320 676f 2074 6f20 5b2a 2a65  sages go to [**e
+00004470: 7861 6d70 6c65 732f 2a2a 5d28 6874 7470  xamples/**](http
+00004480: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00004490: 616e 6365 746e 696b 2f50 726f 7061 6e2f  ancetnik/Propan/
+000044a0: 7472 6565 2f6d 6169 6e2f 6578 616d 706c  tree/main/exampl
+000044b0: 6573 290a                                es).
```

