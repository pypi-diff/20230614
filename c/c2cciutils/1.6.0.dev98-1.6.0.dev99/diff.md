# Comparing `tmp/c2cciutils-1.6.0.dev98.tar.gz` & `tmp/c2cciutils-1.6.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cciutils-1.6.0.dev98.tar", max compression
+gzip compressed data, was "c2cciutils-1.6.0.dev99.tar", max compression
```

## Comparing `c2cciutils-1.6.0.dev98.tar` & `c2cciutils-1.6.0.dev99.tar`

### file list

```diff
@@ -1,592 +1,592 @@
--rw-r--r--   0        0        0     1307 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/LICENSE
--rw-r--r--   0        0        0    14776 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/README.md
--rw-r--r--   0        0        0    18066 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/__init__.py
--rw-r--r--   0        0        0      178 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/applications-versions.yaml
--rw-r--r--   0        0        0      283 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/applications.yaml
--rw-r--r--   0        0        0     1232 2023-05-21 15:52:12.124421 c2cciutils-1.6.0.dev98/c2cciutils/applications_definition.py
--rw-r--r--   0        0        0     9028 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/audit.py
--rw-r--r--   0        0        0      358 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/branches.graphql
--rw-r--r--   0        0        0      308 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/commits.graphql
--rw-r--r--   0        0        0    22063 2023-05-21 15:52:09.932402 c2cciutils-1.6.0.dev98/c2cciutils/configuration.py
--rw-r--r--   0        0        0      131 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/default_branch.graphql
--rw-r--r--   0        0        0     3425 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/env.py
--rw-r--r--   0        0        0     5358 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/lib/docker.py
--rw-r--r--   0        0        0    13951 2023-05-21 15:46:56.953563 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/.package-lock.json
--rw-r--r--   0        0        0     2973 2023-05-21 15:46:54.345537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/api.js
--rw-r--r--   0        0        0    20649 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js
--rw-r--r--   0        0        0      196 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/constants.js
--rw-r--r--   0        0        0     2792 2023-05-21 15:46:54.357537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/envelope.js
--rw-r--r--   0        0        0     6114 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/exports.js
--rw-r--r--   0        0        0    14525 2023-05-21 15:46:54.369537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/hub.js
--rw-r--r--   0        0        0     4225 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/index.js
--rw-r--r--   0        0        0     4142 2023-05-21 15:46:54.385537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integration.js
--rw-r--r--   0        0        0     1305 2023-05-21 15:46:54.365537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js
--rw-r--r--   0        0        0     6540 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js
--rw-r--r--   0        0        0      333 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integrations/index.js
--rw-r--r--   0        0        0    13782 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/scope.js
--rw-r--r--   0        0        0     1161 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/sdk.js
--rw-r--r--   0        0        0     5052 2023-05-21 15:46:54.409537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/session.js
--rw-r--r--   0        0        0     3819 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js
--rw-r--r--   0        0        0     1220 2023-05-21 15:46:54.357537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js
--rw-r--r--   0        0        0     8922 2023-05-21 15:46:54.373537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js
--rw-r--r--   0        0        0    12257 2023-05-21 15:46:54.373537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js
--rw-r--r--   0        0        0     8973 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js
--rw-r--r--   0        0        0     2669 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js
--rw-r--r--   0        0        0     1877 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js
--rw-r--r--   0        0        0     7741 2023-05-21 15:46:54.421537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js
--rw-r--r--   0        0        0      623 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js
--rw-r--r--   0        0        0     3433 2023-05-21 15:46:54.345537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js
--rw-r--r--   0        0        0     2021 2023-05-21 15:46:54.385537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/multiplexed.js
--rw-r--r--   0        0        0     3513 2023-05-21 15:46:54.393537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js
--rw-r--r--   0        0        0      796 2023-05-21 15:46:54.365537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js
--rw-r--r--   0        0        0     8963 2023-05-21 15:46:54.401537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js
--rw-r--r--   0        0        0      166 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/version.js
--rw-r--r--   0        0        0     2845 2023-05-21 15:46:54.345537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/api.js
--rw-r--r--   0        0        0    20562 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/baseclient.js
--rw-r--r--   0        0        0      113 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/constants.js
--rw-r--r--   0        0        0     2723 2023-05-21 15:46:54.357537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/envelope.js
--rw-r--r--   0        0        0     5734 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/exports.js
--rw-r--r--   0        0        0    14180 2023-05-21 15:46:54.369537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/hub.js
--rw-r--r--   0        0        0     1971 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/index.js
--rw-r--r--   0        0        0     3983 2023-05-21 15:46:54.385537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integration.js
--rw-r--r--   0        0        0     1232 2023-05-21 15:46:54.365537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js
--rw-r--r--   0        0        0     6350 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js
--rw-r--r--   0        0        0      146 2023-05-21 15:46:54.381537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integrations/index.js
--rw-r--r--   0        0        0    13728 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/scope.js
--rw-r--r--   0        0        0     1079 2023-05-21 15:46:54.409537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/sdk.js
--rw-r--r--   0        0        0     4938 2023-05-21 15:46:54.409537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/session.js
--rw-r--r--   0        0        0     3751 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js
--rw-r--r--   0        0        0     1141 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js
--rw-r--r--   0        0        0     8723 2023-05-21 15:46:54.373537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js
--rw-r--r--   0        0        0    12026 2023-05-21 15:46:54.373537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js
--rw-r--r--   0        0        0     8841 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js
--rw-r--r--   0        0        0     2600 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js
--rw-r--r--   0        0        0     1803 2023-05-21 15:46:54.421537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js
--rw-r--r--   0        0        0     7640 2023-05-21 15:46:54.421537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js
--rw-r--r--   0        0        0      417 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/utils.js
--rw-r--r--   0        0        0     3404 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/base.js
--rw-r--r--   0        0        0     1978 2023-05-21 15:46:54.385537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/multiplexed.js
--rw-r--r--   0        0        0     3418 2023-05-21 15:46:54.401537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js
--rw-r--r--   0        0        0      720 2023-05-21 15:46:54.365537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js
--rw-r--r--   0        0        0     8845 2023-05-21 15:46:54.401537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js
--rw-r--r--   0        0        0       91 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/version.js
--rw-r--r--   0        0        0      627 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/package.json
--rw-r--r--   0        0        0     1705 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/domain.js
--rw-r--r--   0        0        0     1318 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/hooks.js
--rw-r--r--   0        0        0      652 2023-05-21 15:46:54.433538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/index.js
--rw-r--r--   0        0        0     5887 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/client.js
--rw-r--r--   0        0        0     3247 2023-05-21 15:46:54.421537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js
--rw-r--r--   0        0        0    11931 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/handlers.js
--rw-r--r--   0        0        0     2534 2023-05-21 15:46:54.433538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/index.js
--rw-r--r--   0        0        0     1462 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js
--rw-r--r--   0        0        0    11763 2023-05-21 15:46:54.409537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js
--rw-r--r--   0        0        0     5626 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js
--rw-r--r--   0        0        0    10377 2023-05-21 15:46:54.429538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js
--rw-r--r--   0        0        0     1151 2023-05-21 15:46:54.433538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js
--rw-r--r--   0        0        0     3071 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js
--rw-r--r--   0        0        0    12718 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js
--rw-r--r--   0        0        0     2184 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js
--rw-r--r--   0        0        0     6512 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js
--rw-r--r--   0        0        0     2505 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js
--rw-r--r--   0        0        0     6635 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js
--rw-r--r--   0        0        0     6064 2023-05-21 15:46:54.437538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js
--rw-r--r--   0        0        0     1296 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js
--rw-r--r--   0        0        0     8752 2023-05-21 15:46:54.429538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js
--rw-r--r--   0        0        0     1696 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/module.js
--rw-r--r--   0        0        0      246 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/nodeVersion.js
--rw-r--r--   0        0        0     1606 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js
--rw-r--r--   0        0        0     8798 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js
--rw-r--r--   0        0        0     9675 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/sdk.js
--rw-r--r--   0        0        0     1019 2023-05-21 15:46:54.437538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js
--rw-r--r--   0        0        0      396 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/tracing/integrations.js
--rw-r--r--   0        0        0     4786 2023-05-21 15:46:54.429538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js
--rw-r--r--   0        0        0     1644 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/utils.js
--rw-r--r--   0        0        0     1645 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/domain.js
--rw-r--r--   0        0        0     1262 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/hooks.js
--rw-r--r--   0        0        0      568 2023-05-21 15:46:54.437538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/index.js
--rw-r--r--   0        0        0     5836 2023-05-21 15:46:54.405537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/client.js
--rw-r--r--   0        0        0     3157 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js
--rw-r--r--   0        0        0    11809 2023-05-21 15:46:54.425538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/handlers.js
--rw-r--r--   0        0        0     1244 2023-05-21 15:46:54.437538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/index.js
--rw-r--r--   0        0        0     1400 2023-05-21 15:46:54.409537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js
--rw-r--r--   0        0        0    11588 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js
--rw-r--r--   0        0        0     5541 2023-05-21 15:46:54.413537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js
--rw-r--r--   0        0        0    10336 2023-05-21 15:46:54.429538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js
--rw-r--r--   0        0        0      564 2023-05-21 15:46:54.437538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js
--rw-r--r--   0        0        0     3001 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js
--rw-r--r--   0        0        0    12577 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js
--rw-r--r--   0        0        0     2122 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js
--rw-r--r--   0        0        0     6396 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js
--rw-r--r--   0        0        0     2409 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js
--rw-r--r--   0        0        0     6570 2023-05-21 15:46:54.449538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js
--rw-r--r--   0        0        0     6006 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js
--rw-r--r--   0        0        0     1200 2023-05-21 15:46:54.417538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js
--rw-r--r--   0        0        0     8507 2023-05-21 15:46:54.433538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js
--rw-r--r--   0        0        0     1618 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/module.js
--rw-r--r--   0        0        0      169 2023-05-21 15:46:54.445538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/nodeVersion.js
--rw-r--r--   0        0        0     1532 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js
--rw-r--r--   0        0        0     8640 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/requestdata.js
--rw-r--r--   0        0        0     9353 2023-05-21 15:46:54.453538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/sdk.js
--rw-r--r--   0        0        0      931 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js
--rw-r--r--   0        0        0      142 2023-05-21 15:46:54.441538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/tracing/integrations.js
--rw-r--r--   0        0        0     4667 2023-05-21 15:46:54.433538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/transports/http.js
--rw-r--r--   0        0        0     1565 2023-05-21 15:46:54.457538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/utils.js
--rw-r--r--   0        0        0      994 2023-05-21 15:46:54.457538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/package.json
--rw-r--r--   0        0        0       35 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/types/cjs/index.js
--rw-r--r--   0        0        0       35 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/types/esm/index.js
--rw-r--r--   0        0        0      506 2023-05-21 15:46:54.361537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/types/package.json
--rw-r--r--   0        0        0     5903 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js
--rw-r--r--   0        0        0     4527 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/browser.js
--rw-r--r--   0        0        0     1291 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js
--rw-r--r--   0        0        0     2210 2023-05-21 15:46:54.109534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js
--rw-r--r--   0        0        0     1749 2023-05-21 15:46:54.133535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js
--rw-r--r--   0        0        0      824 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js
--rw-r--r--   0        0        0      882 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js
--rw-r--r--   0        0        0      660 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js
--rw-r--r--   0        0        0     1002 2023-05-21 15:46:54.149535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js
--rw-r--r--   0        0        0      743 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js
--rw-r--r--   0        0        0      773 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js
--rw-r--r--   0        0        0     1100 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js
--rw-r--r--   0        0        0     2325 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js
--rw-r--r--   0        0        0     2078 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js
--rw-r--r--   0        0        0     1752 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js
--rw-r--r--   0        0        0     1941 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js
--rw-r--r--   0        0        0      727 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js
--rw-r--r--   0        0        0     3180 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js
--rw-r--r--   0        0        0     1613 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/env.js
--rw-r--r--   0        0        0     6925 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js
--rw-r--r--   0        0        0      819 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/error.js
--rw-r--r--   0        0        0     8501 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/index.js
--rw-r--r--   0        0        0    19360 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js
--rw-r--r--   0        0        0     4878 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/is.js
--rw-r--r--   0        0        0     2403 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/logger.js
--rw-r--r--   0        0        0     1096 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/memo.js
--rw-r--r--   0        0        0     7809 2023-05-21 15:46:54.221536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/misc.js
--rw-r--r--   0        0        0     2703 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js
--rw-r--r--   0        0        0     2267 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/node.js
--rw-r--r--   0        0        0     9677 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js
--rw-r--r--   0        0        0     9449 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/object.js
--rw-r--r--   0        0        0     5629 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/path.js
--rw-r--r--   0        0        0     3592 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js
--rw-r--r--   0        0        0     3349 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js
--rw-r--r--   0        0        0     9445 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js
--rw-r--r--   0        0        0     1725 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/severity.js
--rw-r--r--   0        0        0     4725 2023-05-21 15:46:54.249536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js
--rw-r--r--   0        0        0     3764 2023-05-21 15:46:54.249536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/string.js
--rw-r--r--   0        0        0     4591 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/supports.js
--rw-r--r--   0        0        0     4495 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js
--rw-r--r--   0        0        0     7845 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/time.js
--rw-r--r--   0        0        0     1094 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js
--rw-r--r--   0        0        0     2341 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/url.js
--rw-r--r--   0        0        0     3919 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js
--rw-r--r--   0        0        0     2198 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js
--rw-r--r--   0        0        0     1235 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js
--rw-r--r--   0        0        0     3202 2023-05-21 15:46:54.261536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js
--rw-r--r--   0        0        0     5598 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/baggage.js
--rw-r--r--   0        0        0     4394 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/browser.js
--rw-r--r--   0        0        0     1188 2023-05-21 15:46:54.097534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js
--rw-r--r--   0        0        0     2127 2023-05-21 15:46:54.125535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js
--rw-r--r--   0        0        0     1639 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js
--rw-r--r--   0        0        0      738 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js
--rw-r--r--   0        0        0      801 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js
--rw-r--r--   0        0        0      577 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js
--rw-r--r--   0        0        0      917 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js
--rw-r--r--   0        0        0      647 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js
--rw-r--r--   0        0        0      687 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js
--rw-r--r--   0        0        0     1013 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js
--rw-r--r--   0        0        0     2245 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js
--rw-r--r--   0        0        0     2000 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js
--rw-r--r--   0        0        0     1652 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js
--rw-r--r--   0        0        0      890 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js
--rw-r--r--   0        0        0      645 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js
--rw-r--r--   0        0        0     3038 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/dsn.js
--rw-r--r--   0        0        0     1511 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/env.js
--rw-r--r--   0        0        0     6527 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/envelope.js
--rw-r--r--   0        0        0      744 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/error.js
--rw-r--r--   0        0        0     3442 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/index.js
--rw-r--r--   0        0        0    19108 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/instrument.js
--rw-r--r--   0        0        0     4529 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/is.js
--rw-r--r--   0        0        0     2259 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/logger.js
--rw-r--r--   0        0        0     1021 2023-05-21 15:46:54.221536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/memo.js
--rw-r--r--   0        0        0     7523 2023-05-21 15:46:54.221536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/misc.js
--rw-r--r--   0        0        0     2635 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js
--rw-r--r--   0        0        0     2155 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/node.js
--rw-r--r--   0        0        0     9577 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/normalize.js
--rw-r--r--   0        0        0     9181 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/object.js
--rw-r--r--   0        0        0     5442 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/path.js
--rw-r--r--   0        0        0     3515 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js
--rw-r--r--   0        0        0     3159 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js
--rw-r--r--   0        0        0     9276 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js
--rw-r--r--   0        0        0     1579 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/severity.js
--rw-r--r--   0        0        0     4480 2023-05-21 15:46:54.249536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js
--rw-r--r--   0        0        0     3597 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/string.js
--rw-r--r--   0        0        0     4291 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/supports.js
--rw-r--r--   0        0        0     4364 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js
--rw-r--r--   0        0        0     7630 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/time.js
--rw-r--r--   0        0        0      979 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/tracing.js
--rw-r--r--   0        0        0     2169 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/url.js
--rw-r--r--   0        0        0     3833 2023-05-21 15:46:54.257536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js
--rw-r--r--   0        0        0     2114 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js
--rw-r--r--   0        0        0     1151 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js
--rw-r--r--   0        0        0     3073 2023-05-21 15:46:54.261536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js
--rw-r--r--   0        0        0      720 2023-05-21 15:46:54.261536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/package.json
--rw-r--r--   0        0        0     1549 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js
--rw-r--r--   0        0        0     9662 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js
--rw-r--r--   0        0        0    16045 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js
--rw-r--r--   0        0        0      839 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js
--rw-r--r--   0        0        0     9441 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js
--rw-r--r--   0        0        0     2597 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js
--rw-r--r--   0        0        0      199 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/types.js
--rw-r--r--   0        0        0     3902 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js
--rw-r--r--   0        0        0     2257 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js
--rw-r--r--   0        0        0     3094 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js
--rw-r--r--   0        0        0      843 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js
--rw-r--r--   0        0        0     1031 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js
--rw-r--r--   0        0        0      973 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js
--rw-r--r--   0        0        0     1851 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js
--rw-r--r--   0        0        0     1795 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js
--rw-r--r--   0        0        0     1563 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js
--rw-r--r--   0        0        0      943 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js
--rw-r--r--   0        0        0     1379 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js
--rw-r--r--   0        0        0     1735 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js
--rw-r--r--   0        0        0     2157 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js
--rw-r--r--   0        0        0     5368 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js
--rw-r--r--   0        0        0    12006 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js
--rw-r--r--   0        0        0     2405 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js
--rw-r--r--   0        0        0     1184 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js
--rw-r--r--   0        0        0     9526 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js
--rw-r--r--   0        0        0     2645 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js
--rw-r--r--   0        0        0     3457 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js
--rw-r--r--   0        0        0     1883 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js
--rw-r--r--   0        0        0      793 2023-05-21 15:46:54.221536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js
--rw-r--r--   0        0        0     1429 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js
--rw-r--r--   0        0        0     9706 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js
--rw-r--r--   0        0        0    15585 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js
--rw-r--r--   0        0        0      735 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js
--rw-r--r--   0        0        0     9229 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js
--rw-r--r--   0        0        0     2501 2023-05-21 15:46:54.237536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js
--rw-r--r--   0        0        0      127 2023-05-21 15:46:54.241536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/types.js
--rw-r--r--   0        0        0     3788 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js
--rw-r--r--   0        0        0     2121 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js
--rw-r--r--   0        0        0     2938 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js
--rw-r--r--   0        0        0      767 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js
--rw-r--r--   0        0        0      951 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js
--rw-r--r--   0        0        0      871 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js
--rw-r--r--   0        0        0     1739 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js
--rw-r--r--   0        0        0     1689 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js
--rw-r--r--   0        0        0     1425 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js
--rw-r--r--   0        0        0      872 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js
--rw-r--r--   0        0        0     1301 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js
--rw-r--r--   0        0        0     1668 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js
--rw-r--r--   0        0        0     1080 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js
--rw-r--r--   0        0        0     5248 2023-05-21 15:46:54.125535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js
--rw-r--r--   0        0        0    11942 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js
--rw-r--r--   0        0        0     2340 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js
--rw-r--r--   0        0        0     1039 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js
--rw-r--r--   0        0        0     9463 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js
--rw-r--r--   0        0        0     2576 2023-05-21 15:46:54.221536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js
--rw-r--r--   0        0        0     3385 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js
--rw-r--r--   0        0        0     1802 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js
--rw-r--r--   0        0        0      693 2023-05-21 15:46:54.229536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js
--rw-r--r--   0        0        0      723 2023-05-21 15:46:54.245536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/package.json
--rw-r--r--   0        0        0     7910 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/agent-base/dist/src/index.js
--rw-r--r--   0        0        0      495 2023-05-21 15:46:54.073534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/agent-base/dist/src/promisify.js
--rw-r--r--   0        0        0     1635 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/agent-base/package.json
--rw-r--r--   0        0        0       27 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/.eslintrc.json
--rw-r--r--   0        0        0       60 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/.npmpackagejsonlintrc.json
--rw-r--r--   0        0        0       50 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/.releaserc.json
--rw-r--r--   0        0        0      539 2023-05-21 15:46:54.037534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/build/lib/boolean.js
--rw-r--r--   0        0        0      463 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/build/lib/index.js
--rw-r--r--   0        0        0      646 2023-05-21 15:46:54.061534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js
--rw-r--r--   0        0        0      228 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/licenseCheck.json
--rw-r--r--   0        0        0      982 2023-05-21 15:46:54.093534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/package.json
--rw-r--r--   0        0        0      323 2023-05-21 15:46:54.097534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/tsconfig.json
--rw-r--r--   0        0        0     4047 2023-05-21 15:46:54.017533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/cookie/index.js
--rw-r--r--   0        0        0     1104 2023-05-21 15:46:54.037534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/cookie/package.json
--rw-r--r--   0        0        0     1419 2023-05-21 15:46:54.121534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/package.json
--rw-r--r--   0        0        0     6010 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/browser.js
--rw-r--r--   0        0        0     6289 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/common.js
--rw-r--r--   0        0        0      314 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/index.js
--rw-r--r--   0        0        0     4685 2023-05-21 15:46:54.097534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/node.js
--rw-r--r--   0        0        0     1429 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/define-properties/index.js
--rw-r--r--   0        0        0     2245 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/define-properties/package.json
--rw-r--r--   0        0        0       25 2023-05-21 15:46:54.017533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/detect-node/browser.js
--rw-r--r--   0        0        0      184 2023-05-21 15:46:54.037534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/detect-node/index.esm.js
--rw-r--r--   0        0        0      186 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/detect-node/index.js
--rw-r--r--   0        0        0      607 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/detect-node/package.json
--rw-r--r--   0        0        0     2582 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/es6/index.js
--rw-r--r--   0        0        0     2703 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/lib/index.js
--rw-r--r--   0        0        0     1404 2023-05-21 15:46:53.993533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/package.json
--rw-r--r--   0        0        0      461 2023-05-21 15:46:54.001533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/escape-string-regexp/index.js
--rw-r--r--   0        0        0      686 2023-05-21 15:46:54.013533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     4140 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/.jscs.json
--rw-r--r--   0        0        0     1463 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/implementation.js
--rw-r--r--   0        0        0      126 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/index.js
--rw-r--r--   0        0        0     1498 2023-05-21 15:46:53.993533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     8991 2023-05-21 15:46:54.097534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/test/index.js
--rw-r--r--   0        0        0    13145 2023-05-21 15:46:54.093534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/index.js
--rw-r--r--   0        0        0     2349 2023-05-21 15:46:54.105534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     8767 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js
--rw-r--r--   0        0        0       37 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/bootstrap.js
--rw-r--r--   0        0        0      414 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/Logger.js
--rw-r--r--   0        0        0     6510 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/Agent.js
--rw-r--r--   0        0        0      905 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js
--rw-r--r--   0        0        0     1542 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js
--rw-r--r--   0        0        0      814 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/index.js
--rw-r--r--   0        0        0      575 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/errors.js
--rw-r--r--   0        0        0     6002 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js
--rw-r--r--   0        0        0     1086 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js
--rw-r--r--   0        0        0      694 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/index.js
--rw-r--r--   0        0        0      476 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/index.js
--rw-r--r--   0        0        0      759 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js
--rw-r--r--   0        0        0      402 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/routines/index.js
--rw-r--r--   0        0        0      165 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/types.js
--rw-r--r--   0        0        0     1479 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js
--rw-r--r--   0        0        0      866 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/index.js
--rw-r--r--   0        0        0     1341 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js
--rw-r--r--   0        0        0     1065 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js
--rw-r--r--   0        0        0     2585 2023-05-21 15:46:54.217536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/package.json
--rw-r--r--   0        0        0      129 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/Logger.js
--rw-r--r--   0        0        0     6762 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/Agent.js
--rw-r--r--   0        0        0      733 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js
--rw-r--r--   0        0        0     1346 2023-05-21 15:46:54.197535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js
--rw-r--r--   0        0        0      174 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/index.js
--rw-r--r--   0        0        0      299 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/errors.js
--rw-r--r--   0        0        0     5715 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js
--rw-r--r--   0        0        0      882 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js
--rw-r--r--   0        0        0      160 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/factories/index.js
--rw-r--r--   0        0        0      100 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/index.js
--rw-r--r--   0        0        0      550 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js
--rw-r--r--   0        0        0       60 2023-05-21 15:46:54.201535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/routines/index.js
--rw-r--r--   0        0        0     1567 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/types.js
--rw-r--r--   0        0        0     1197 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js
--rw-r--r--   0        0        0      200 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/index.js
--rw-r--r--   0        0        0     1022 2023-05-21 15:46:54.205535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js
--rw-r--r--   0        0        0      874 2023-05-21 15:46:54.213535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js
--rw-r--r--   0        0        0       36 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/auto.js
--rw-r--r--   0        0        0      254 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/implementation.browser.js
--rw-r--r--   0        0        0       40 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/implementation.js
--rw-r--r--   0        0        0      408 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/index.js
--rw-r--r--   0        0        0     2418 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/package.json
--rw-r--r--   0        0        0      251 2023-05-21 15:46:54.117534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/polyfill.js
--rw-r--r--   0        0        0      722 2023-05-21 15:46:54.125535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/shim.js
--rw-r--r--   0        0        0      213 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/implementation.js
--rw-r--r--   0        0        0      196 2023-05-21 15:46:54.097534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/index.js
--rw-r--r--   0        0        0      767 2023-05-21 15:46:54.105534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/native.js
--rw-r--r--   0        0        0      900 2023-05-21 15:46:54.129535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/shimmed.js
--rw-r--r--   0        0        0     1399 2023-05-21 15:46:54.133535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/tests.js
--rw-r--r--   0        0        0     1011 2023-05-21 15:46:53.981533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has/package.json
--rw-r--r--   0        0        0      129 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has/src/index.js
--rw-r--r--   0        0        0      331 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has/test/index.js
--rw-r--r--   0        0        0      817 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/index.js
--rw-r--r--   0        0        0     1933 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     1405 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/test/index.js
--rw-r--r--   0        0        0      420 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/index.js
--rw-r--r--   0        0        0     2648 2023-05-21 15:46:54.121534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     1761 2023-05-21 15:46:54.093534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/shams.js
--rw-r--r--   0        0        0      654 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/index.js
--rw-r--r--   0        0        0      723 2023-05-21 15:46:54.057534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/shams/core-js.js
--rw-r--r--   0        0        0      686 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js
--rw-r--r--   0        0        0     2021 2023-05-21 15:46:54.105534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/tests.js
--rw-r--r--   0        0        0     7841 2023-05-21 15:46:54.001533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/agent.js
--rw-r--r--   0        0        0      579 2023-05-21 15:46:54.013533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/index.js
--rw-r--r--   0        0        0     2460 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js
--rw-r--r--   0        0        0     1405 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/package.json
--rw-r--r--   0        0        0      796 2023-05-21 15:46:53.929533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/package.json
--rw-r--r--   0        0        0      907 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/stringify.js
--rw-r--r--   0        0        0     7550 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js
--rw-r--r--   0        0        0     8186 2023-05-21 15:46:53.949533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru-cache/index.js
--rw-r--r--   0        0        0      705 2023-05-21 15:46:53.989533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0     4625 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/benchmark.js
--rw-r--r--   0        0        0     7934 2023-05-21 15:46:54.073534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/lru.js
--rw-r--r--   0        0        0      901 2023-05-21 15:46:53.929533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/package.json
--rw-r--r--   0        0        0     7366 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/test.js
--rw-r--r--   0        0        0      227 2023-05-21 15:46:54.129535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/tsconfig.json
--rw-r--r--   0        0        0     1785 2023-05-21 15:46:53.949533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/matcher/index.js
--rw-r--r--   0        0        0      871 2023-05-21 15:46:53.981533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/matcher/package.json
--rw-r--r--   0        0        0     3023 2023-05-21 15:46:53.949533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/ms/index.js
--rw-r--r--   0        0        0      705 2023-05-21 15:46:53.909532 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/ms/package.json
--rw-r--r--   0        0        0     3218 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/implementation.js
--rw-r--r--   0        0        0      823 2023-05-21 15:46:54.041534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/index.js
--rw-r--r--   0        0        0      422 2023-05-21 15:46:54.053534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/isArguments.js
--rw-r--r--   0        0        0     1903 2023-05-21 15:46:53.909532 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/package.json
--rw-r--r--   0        0        0       61 2023-05-21 15:46:54.085534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/test/index.js
--rw-r--r--   0        0        0      274 2023-05-21 15:46:54.121534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/constants.js
--rw-r--r--   0        0        0     6377 2023-05-21 15:46:54.129535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createLogger.js
--rw-r--r--   0        0        0     1103 2023-05-21 15:46:54.133535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js
--rw-r--r--   0        0        0      629 2023-05-21 15:46:54.133535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js
--rw-r--r--   0        0        0     2493 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js
--rw-r--r--   0        0        0      914 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/index.js
--rw-r--r--   0        0        0     1186 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/log.js
--rw-r--r--   0        0        0       47 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/types.js
--rw-r--r--   0        0        0     2350 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/package.json
--rwxr-xr-x   0        0        0     4823 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/bin/semver.js
--rw-r--r--   0        0        0     3563 2023-05-21 15:46:54.029534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/comparator.js
--rw-r--r--   0        0        0      129 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/index.js
--rw-r--r--   0        0        0    14283 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/range.js
--rw-r--r--   0        0        0     8673 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/semver.js
--rw-r--r--   0        0        0      191 2023-05-21 15:46:53.945533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/clean.js
--rw-r--r--   0        0        0      947 2023-05-21 15:46:53.977533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/cmp.js
--rw-r--r--   0        0        0     1505 2023-05-21 15:46:53.989533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/coerce.js
--rw-r--r--   0        0        0      267 2023-05-21 15:46:54.053534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/compare-build.js
--rw-r--r--   0        0        0      118 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/compare-loose.js
--rw-r--r--   0        0        0      156 2023-05-21 15:46:54.073534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/compare.js
--rw-r--r--   0        0        0     1303 2023-05-21 15:46:54.093534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/diff.js
--rw-r--r--   0        0        0      112 2023-05-21 15:46:54.105534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/eq.js
--rw-r--r--   0        0        0      110 2023-05-21 15:46:54.109534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/gt.js
--rw-r--r--   0        0        0      113 2023-05-21 15:46:54.121534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/gte.js
--rw-r--r--   0        0        0      464 2023-05-21 15:46:54.137535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/inc.js
--rw-r--r--   0        0        0      110 2023-05-21 15:46:54.149535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/lt.js
--rw-r--r--   0        0        0      113 2023-05-21 15:46:54.149535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/lte.js
--rw-r--r--   0        0        0      122 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/major.js
--rw-r--r--   0        0        0      122 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/minor.js
--rw-r--r--   0        0        0      114 2023-05-21 15:46:54.157535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/neq.js
--rw-r--r--   0        0        0      317 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/parse.js
--rw-r--r--   0        0        0      122 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/patch.js
--rw-r--r--   0        0        0      220 2023-05-21 15:46:54.169535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/prerelease.js
--rw-r--r--   0        0        0      118 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/rcompare.js
--rw-r--r--   0        0        0      149 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/rsort.js
--rw-r--r--   0        0        0      233 2023-05-21 15:46:54.181535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/satisfies.js
--rw-r--r--   0        0        0      147 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/sort.js
--rw-r--r--   0        0        0      162 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/valid.js
--rw-r--r--   0        0        0     2616 2023-05-21 15:46:54.141535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/index.js
--rw-r--r--   0        0        0      657 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/constants.js
--rw-r--r--   0        0        0      226 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/debug.js
--rw-r--r--   0        0        0      410 2023-05-21 15:46:54.133535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/identifiers.js
--rw-r--r--   0        0        0      324 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/parse-options.js
--rw-r--r--   0        0        0     6672 2023-05-21 15:46:54.177535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/re.js
--rw-r--r--   0        0        0     1748 2023-05-21 15:46:54.193535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/package.json
--rw-r--r--   0        0        0       69 2023-05-21 15:46:54.165535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/preload.js
--rw-r--r--   0        0        0      217 2023-05-21 15:46:54.129535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/gtr.js
--rw-r--r--   0        0        0      210 2023-05-21 15:46:54.145535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/intersects.js
--rw-r--r--   0        0        0      213 2023-05-21 15:46:54.149535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/ltr.js
--rw-r--r--   0        0        0      579 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/max-satisfying.js
--rw-r--r--   0        0        0      577 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/min-satisfying.js
--rw-r--r--   0        0        0     1500 2023-05-21 15:46:54.153535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/min-version.js
--rw-r--r--   0        0        0     2190 2023-05-21 15:46:54.161535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/outside.js
--rw-r--r--   0        0        0     1341 2023-05-21 15:46:54.185535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/simplify.js
--rw-r--r--   0        0        0     7510 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/subset.js
--rw-r--r--   0        0        0      268 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/to-comparators.js
--rw-r--r--   0        0        0      312 2023-05-21 15:46:54.189535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/valid.js
--rw-r--r--   0        0        0      210 2023-05-21 15:46:54.045534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/example/cmp.js
--rw-r--r--   0        0        0      181 2023-05-21 15:46:54.053534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/example/lex.js
--rw-r--r--   0        0        0      372 2023-05-21 15:46:54.001533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/index.js
--rw-r--r--   0        0        0      659 2023-05-21 15:46:53.929533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/package.json
--rw-r--r--   0        0        0      444 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/test/cmp.js
--rw-r--r--   0        0        0     2235 2023-05-21 15:46:53.949533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/serialize-error/index.js
--rw-r--r--   0        0        0      743 2023-05-21 15:46:53.981533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/serialize-error/package.json
--rwxr-xr-x   0        0        0       57 2023-05-21 15:46:54.121534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/bin/snyk
--rw-r--r--   0        0        0      150 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/config.default.json
--rw-r--r--   0        0        0     1838 2023-05-21 15:46:54.233536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/110.index.js
--rw-r--r--   0        0        0   103302 2023-05-21 15:46:54.249536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/213.index.js
--rw-r--r--   0        0        0   133844 2023-05-21 15:46:54.253536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/31.index.js
--rw-r--r--   0        0        0   173511 2023-05-21 15:46:54.261536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/38.index.js
--rw-r--r--   0        0        0   161488 2023-05-21 15:46:54.265536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/384.index.js
--rw-r--r--   0        0        0   128289 2023-05-21 15:46:54.273536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/395.index.js
--rw-r--r--   0        0        0     2969 2023-05-21 15:46:54.273536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/477.index.js
--rw-r--r--   0        0        0   557584 2023-05-21 15:46:54.297536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/503.index.js
--rw-r--r--   0        0        0    22931 2023-05-21 15:46:54.297536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/519.index.js
--rw-r--r--   0        0        0      612 2023-05-21 15:46:54.297536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/522.index.js
--rw-r--r--   0        0        0   569531 2023-05-21 15:46:54.313537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/535.index.js
--rw-r--r--   0        0        0     7242 2023-05-21 15:46:54.313537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/542.index.js
--rw-r--r--   0        0        0     1061 2023-05-21 15:46:54.313537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/575.index.js
--rw-r--r--   0        0        0    32497 2023-05-21 15:46:54.313537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/663.index.js
--rw-r--r--   0        0        0    18697 2023-05-21 15:46:54.313537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/726.index.js
--rw-r--r--   0        0        0   106008 2023-05-21 15:46:54.317536 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/741.index.js
--rw-r--r--   0        0        0   280086 2023-05-21 15:46:54.325537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/784.index.js
--rw-r--r--   0        0        0   265629 2023-05-21 15:46:54.333537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/790.index.js
--rw-r--r--   0        0        0     3295 2023-05-21 15:46:54.333537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/831.index.js
--rw-r--r--   0        0        0    11175 2023-05-21 15:46:54.333537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/85.index.js
--rw-r--r--   0        0        0     1445 2023-05-21 15:46:54.333537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/855.index.js
--rw-r--r--   0        0        0      523 2023-05-21 15:46:54.333537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/875.index.js
--rw-r--r--   0        0        0   267291 2023-05-21 15:46:54.345537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/895.index.js
--rw-r--r--   0        0        0   227159 2023-05-21 15:46:54.349537 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/905.index.js
--rw-r--r--   0        0        0  4489688 2023-05-21 15:46:54.493538 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/917.index.js
--rw-r--r--   0        0        0  8653273 2023-05-21 15:46:54.597539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/95.index.js
--rw-r--r--   0        0        0      592 2023-05-21 15:46:54.597539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/959.index.js
--rw-r--r--   0        0        0    93818 2023-05-21 15:46:54.597539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/970.index.js
--rw-r--r--   0        0        0    20674 2023-05-21 15:46:54.597539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/974.index.js
--rw-r--r--   0        0        0    14335 2023-05-21 15:46:54.601539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/989.index.js
--rw-r--r--   0        0        0  1682422 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/index.js
--rw-r--r--   0        0        0   613426 2023-05-21 15:46:54.905542 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm
--rw-r--r--   0        0        0   614892 2023-05-21 15:46:54.625540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json
--rw-r--r--   0        0        0      140 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/jest.config.js
--rw-r--r--   0        0        0     1094 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/package.json
--rw-r--r--   0        0        0     1203 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/distPackage.py
--rw-r--r--   0        0        0      844 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/package.py
--rw-r--r--   0        0        0      726 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py
--rw-r--r--   0        0        0      562 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py
--rw-r--r--   0        0        0     9460 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py
--rw-r--r--   0        0        0     5098 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py
--rw-r--r--   0        0        0     4385 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py
--rw-r--r--   0        0        0    15974 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/version.py
--rw-r--r--   0        0        0    13551 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py
--rw-r--r--   0        0        0     1788 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pipfile.py
--rw-r--r--   0        0        0   273365 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pyparsing.py
--rw-r--r--   0        0        0       92 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/__init__.py
--rw-r--r--   0        0        0      509 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/core.py
--rw-r--r--   0        0        0    11254 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py
--rw-r--r--   0        0        0     3815 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py
--rw-r--r--   0        0        0     1508 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/reqPackage.py
--rw-r--r--   0        0        0      353 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/__init__.py
--rw-r--r--   0        0        0     1352 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py
--rw-r--r--   0        0        0     3092 2023-05-21 15:46:54.797541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py
--rw-r--r--   0        0        0    10020 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py
--rw-r--r--   0        0        0      405 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/vcs.py
--rw-r--r--   0        0        0     1427 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/setup_file.py
--rw-r--r--   0        0        0     6291 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py
--rw-r--r--   0        0        0     2258 2023-05-21 15:46:54.801541 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/utils.py
--rw-r--r--   0        0        0      246 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/src/generated/binary-deployments.json
--rw-r--r--   0        0        0      186 2023-05-21 15:46:54.625540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/tsconfig.json
--rw-r--r--   0        0        0      843 2023-05-21 15:46:54.601539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js
--rw-r--r--   0        0        0    11438 2023-05-21 15:46:54.601539 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/common.js
--rw-r--r--   0        0        0      246 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/generated/binary-deployments.json
--rw-r--r--   0        0        0     2017 2023-05-21 15:46:54.613540 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/index.js
--rw-r--r--   0        0        0      498 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/dist/angular-sprintf.min.js
--rw-r--r--   0        0        0     3675 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js
--rw-r--r--   0        0        0      818 2023-05-21 15:46:53.901532 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/package.json
--rw-r--r--   0        0        0      663 2023-05-21 15:46:54.109534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js
--rw-r--r--   0        0        0     9250 2023-05-21 15:46:54.125535 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/src/sprintf.js
--rw-r--r--   0        0        0      943 2023-05-21 15:46:53.945533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/modules/index.js
--rw-r--r--   0        0        0       26 2023-05-21 15:46:54.077534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      915 2023-05-21 15:46:54.081534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/package.json
--rw-r--r--   0        0        0      824 2023-05-21 15:46:53.997533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
--rw-r--r--   0        0        0       71 2023-05-21 15:46:54.089534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0    10274 2023-05-21 15:46:54.041534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/tslib.es6.js
--rw-r--r--   0        0        0    13204 2023-05-21 15:46:54.069534 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/tslib.js
--rw-r--r--   0        0        0      782 2023-05-21 15:46:53.929533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/type-fest/package.json
--rw-r--r--   0        0        0      207 2023-05-21 15:46:53.909532 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/yallist/iterator.js
--rw-r--r--   0        0        0      652 2023-05-21 15:46:53.985533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/yallist/package.json
--rw-r--r--   0        0        0     8411 2023-05-21 15:46:53.945533 c2cciutils-1.6.0.dev98/c2cciutils/node_modules/yallist/yallist.js
--rw-r--r--   0        0        0    25304 2023-05-21 15:46:56.949563 c2cciutils-1.6.0.dev98/c2cciutils/package-lock.json
--rw-r--r--   0        0        0      134 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/package.json
--rw-r--r--   0        0        0    10112 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/pr_checks.py
--rw-r--r--   0        0        0    17707 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/publish.py
--rw-r--r--   0        0        0     1548 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/schema-applications.json
--rw-r--r--   0        0        0    22561 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/schema.json
--rw-r--r--   0        0        0       36 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/__init__.py
--rw-r--r--   0        0        0     1104 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/audit.py
--rw-r--r--   0        0        0     3039 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/clean.py
--rw-r--r--   0        0        0     1712 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/docker_logs.py
--rw-r--r--   0        0        0     1316 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/docker_versions_gen.py
--rw-r--r--   0        0        0     4385 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/download_applications.py
--rw-r--r--   0        0        0      375 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/env.py
--rw-r--r--   0        0        0       69 2023-05-21 15:46:43.349424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/__init__.py
--rw-r--r--   0        0        0     3274 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/db.py
--rw-r--r--   0        0        0      921 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/install.py
--rw-r--r--   0        0        0     2655 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/logs.py
--rw-r--r--   0        0        0     5661 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/wait.py
--rw-r--r--   0        0        0     1162 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/main.py
--rw-r--r--   0        0        0     2150 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/pin_pipenv.py
--rw-r--r--   0        0        0     2182 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/pr_checks.py
--rw-r--r--   0        0        0    18222 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/publish.py
--rw-r--r--   0        0        0     2804 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/scripts/trigger_image_update.py
--rw-r--r--   0        0        0     1517 2023-05-21 15:46:43.353424 c2cciutils-1.6.0.dev98/c2cciutils/security.py
--rw-r--r--   0        0        0     4334 2023-05-21 15:57:02.551056 c2cciutils-1.6.0.dev98/pyproject.toml
--rw-r--r--   0        0        0   358583 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev98/setup.py
--rw-r--r--   0        0        0    16769 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev98/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-06-02 07:02:00.535842 c2cciutils-1.6.0.dev99/LICENSE
+-rw-r--r--   0        0        0    14776 2023-06-02 07:02:00.535842 c2cciutils-1.6.0.dev99/README.md
+-rw-r--r--   0        0        0    18066 2023-06-02 07:02:00.535842 c2cciutils-1.6.0.dev99/c2cciutils/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-02 07:02:00.535842 c2cciutils-1.6.0.dev99/c2cciutils/applications-versions.yaml
+-rw-r--r--   0        0        0      283 2023-06-02 07:02:00.535842 c2cciutils-1.6.0.dev99/c2cciutils/applications.yaml
+-rw-r--r--   0        0        0     1232 2023-06-02 07:08:40.322701 c2cciutils-1.6.0.dev99/c2cciutils/applications_definition.py
+-rw-r--r--   0        0        0     9028 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/audit.py
+-rw-r--r--   0        0        0      358 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/branches.graphql
+-rw-r--r--   0        0        0      308 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/commits.graphql
+-rw-r--r--   0        0        0    22063 2023-06-02 07:08:37.670681 c2cciutils-1.6.0.dev99/c2cciutils/configuration.py
+-rw-r--r--   0        0        0      131 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/default_branch.graphql
+-rw-r--r--   0        0        0     3425 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/env.py
+-rw-r--r--   0        0        0     5358 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/lib/docker.py
+-rw-r--r--   0        0        0    13951 2023-06-02 07:02:17.351964 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/.package-lock.json
+-rw-r--r--   0        0        0     2973 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/api.js
+-rw-r--r--   0        0        0    20649 2023-06-02 07:02:14.243942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js
+-rw-r--r--   0        0        0      196 2023-06-02 07:02:14.259943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/constants.js
+-rw-r--r--   0        0        0     2792 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/envelope.js
+-rw-r--r--   0        0        0     6114 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/exports.js
+-rw-r--r--   0        0        0    14525 2023-06-02 07:02:14.327943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/hub.js
+-rw-r--r--   0        0        0     4225 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/index.js
+-rw-r--r--   0        0        0     4142 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integration.js
+-rw-r--r--   0        0        0     1305 2023-06-02 07:02:14.307943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js
+-rw-r--r--   0        0        0     6540 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js
+-rw-r--r--   0        0        0      333 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integrations/index.js
+-rw-r--r--   0        0        0    13782 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/scope.js
+-rw-r--r--   0        0        0     1161 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/sdk.js
+-rw-r--r--   0        0        0     5052 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/session.js
+-rw-r--r--   0        0        0     3819 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js
+-rw-r--r--   0        0        0     1220 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js
+-rw-r--r--   0        0        0     8922 2023-06-02 07:02:14.335943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js
+-rw-r--r--   0        0        0    12257 2023-06-02 07:02:14.343943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js
+-rw-r--r--   0        0        0     8973 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js
+-rw-r--r--   0        0        0     2669 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js
+-rw-r--r--   0        0        0     1877 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js
+-rw-r--r--   0        0        0     7741 2023-06-02 07:02:14.447944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js
+-rw-r--r--   0        0        0      623 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js
+-rw-r--r--   0        0        0     3433 2023-06-02 07:02:14.199942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js
+-rw-r--r--   0        0        0     2021 2023-06-02 07:02:14.375943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/multiplexed.js
+-rw-r--r--   0        0        0     3513 2023-06-02 07:02:14.387943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js
+-rw-r--r--   0        0        0      796 2023-06-02 07:02:14.319943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js
+-rw-r--r--   0        0        0     8963 2023-06-02 07:02:14.399943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js
+-rw-r--r--   0        0        0      166 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/version.js
+-rw-r--r--   0        0        0     2845 2023-06-02 07:02:14.179942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/api.js
+-rw-r--r--   0        0        0    20562 2023-06-02 07:02:14.259943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/baseclient.js
+-rw-r--r--   0        0        0      113 2023-06-02 07:02:14.263943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/constants.js
+-rw-r--r--   0        0        0     2723 2023-06-02 07:02:14.275943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/envelope.js
+-rw-r--r--   0        0        0     5734 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/exports.js
+-rw-r--r--   0        0        0    14180 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/hub.js
+-rw-r--r--   0        0        0     1971 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/index.js
+-rw-r--r--   0        0        0     3983 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integration.js
+-rw-r--r--   0        0        0     1232 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js
+-rw-r--r--   0        0        0     6350 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js
+-rw-r--r--   0        0        0      146 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integrations/index.js
+-rw-r--r--   0        0        0    13728 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/scope.js
+-rw-r--r--   0        0        0     1079 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/sdk.js
+-rw-r--r--   0        0        0     4938 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/session.js
+-rw-r--r--   0        0        0     3751 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js
+-rw-r--r--   0        0        0     1141 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js
+-rw-r--r--   0        0        0     8723 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js
+-rw-r--r--   0        0        0    12026 2023-06-02 07:02:14.351943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js
+-rw-r--r--   0        0        0     8841 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js
+-rw-r--r--   0        0        0     2600 2023-06-02 07:02:14.435944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js
+-rw-r--r--   0        0        0     1803 2023-06-02 07:02:14.447944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js
+-rw-r--r--   0        0        0     7640 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js
+-rw-r--r--   0        0        0      417 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/utils.js
+-rw-r--r--   0        0        0     3404 2023-06-02 07:02:14.211942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/base.js
+-rw-r--r--   0        0        0     1978 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/multiplexed.js
+-rw-r--r--   0        0        0     3418 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js
+-rw-r--r--   0        0        0      720 2023-06-02 07:02:14.323943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js
+-rw-r--r--   0        0        0     8845 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js
+-rw-r--r--   0        0        0       91 2023-06-02 07:02:14.459944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/version.js
+-rw-r--r--   0        0        0      627 2023-06-02 07:02:14.459944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/package.json
+-rw-r--r--   0        0        0     1705 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/domain.js
+-rw-r--r--   0        0        0     1318 2023-06-02 07:02:14.323943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/hooks.js
+-rw-r--r--   0        0        0      652 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/index.js
+-rw-r--r--   0        0        0     5887 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/client.js
+-rw-r--r--   0        0        0     3247 2023-06-02 07:02:14.307943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js
+-rw-r--r--   0        0        0    11931 2023-06-02 07:02:14.319943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/handlers.js
+-rw-r--r--   0        0        0     2534 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/index.js
+-rw-r--r--   0        0        0     1462 2023-06-02 07:02:14.219942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js
+-rw-r--r--   0        0        0    11763 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js
+-rw-r--r--   0        0        0     5626 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js
+-rw-r--r--   0        0        0    10377 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js
+-rw-r--r--   0        0        0     1151 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js
+-rw-r--r--   0        0        0     3071 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js
+-rw-r--r--   0        0        0    12718 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js
+-rw-r--r--   0        0        0     2184 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js
+-rw-r--r--   0        0        0     6512 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js
+-rw-r--r--   0        0        0     2505 2023-06-02 07:02:14.435944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js
+-rw-r--r--   0        0        0     6635 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js
+-rw-r--r--   0        0        0     6064 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js
+-rw-r--r--   0        0        0     1296 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js
+-rw-r--r--   0        0        0     8752 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js
+-rw-r--r--   0        0        0     1696 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/module.js
+-rw-r--r--   0        0        0      246 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/nodeVersion.js
+-rw-r--r--   0        0        0     1606 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js
+-rw-r--r--   0        0        0     8798 2023-06-02 07:02:14.447944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js
+-rw-r--r--   0        0        0     9675 2023-06-02 07:02:14.463944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/sdk.js
+-rw-r--r--   0        0        0     1019 2023-06-02 07:02:14.375943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js
+-rw-r--r--   0        0        0      396 2023-06-02 07:02:14.399943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/tracing/integrations.js
+-rw-r--r--   0        0        0     4786 2023-06-02 07:02:14.343943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js
+-rw-r--r--   0        0        0     1644 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/utils.js
+-rw-r--r--   0        0        0     1645 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/domain.js
+-rw-r--r--   0        0        0     1262 2023-06-02 07:02:14.327943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/hooks.js
+-rw-r--r--   0        0        0      568 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/index.js
+-rw-r--r--   0        0        0     5836 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/client.js
+-rw-r--r--   0        0        0     3157 2023-06-02 07:02:14.311943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js
+-rw-r--r--   0        0        0    11809 2023-06-02 07:02:14.319943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/handlers.js
+-rw-r--r--   0        0        0     1244 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/index.js
+-rw-r--r--   0        0        0     1400 2023-06-02 07:02:14.235942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js
+-rw-r--r--   0        0        0    11588 2023-06-02 07:02:14.259943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js
+-rw-r--r--   0        0        0     5541 2023-06-02 07:02:14.271943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js
+-rw-r--r--   0        0        0    10336 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js
+-rw-r--r--   0        0        0      564 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js
+-rw-r--r--   0        0        0     3001 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js
+-rw-r--r--   0        0        0    12577 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js
+-rw-r--r--   0        0        0     2122 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js
+-rw-r--r--   0        0        0     6396 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js
+-rw-r--r--   0        0        0     2409 2023-06-02 07:02:14.439944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js
+-rw-r--r--   0        0        0     6570 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js
+-rw-r--r--   0        0        0     6006 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js
+-rw-r--r--   0        0        0     1200 2023-06-02 07:02:14.303943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js
+-rw-r--r--   0        0        0     8507 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js
+-rw-r--r--   0        0        0     1618 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/module.js
+-rw-r--r--   0        0        0      169 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/nodeVersion.js
+-rw-r--r--   0        0        0     1532 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js
+-rw-r--r--   0        0        0     8640 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/requestdata.js
+-rw-r--r--   0        0        0     9353 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/sdk.js
+-rw-r--r--   0        0        0      931 2023-06-02 07:02:14.395943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js
+-rw-r--r--   0        0        0      142 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/tracing/integrations.js
+-rw-r--r--   0        0        0     4667 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/transports/http.js
+-rw-r--r--   0        0        0     1565 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/utils.js
+-rw-r--r--   0        0        0      994 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/package.json
+-rw-r--r--   0        0        0       35 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/types/cjs/index.js
+-rw-r--r--   0        0        0       35 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/types/esm/index.js
+-rw-r--r--   0        0        0      506 2023-06-02 07:02:14.215942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/types/package.json
+-rw-r--r--   0        0        0     5903 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js
+-rw-r--r--   0        0        0     4527 2023-06-02 07:02:14.343943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/browser.js
+-rw-r--r--   0        0        0     1291 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js
+-rw-r--r--   0        0        0     2210 2023-06-02 07:02:14.235942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js
+-rw-r--r--   0        0        0     1749 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js
+-rw-r--r--   0        0        0      824 2023-06-02 07:02:14.263943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js
+-rw-r--r--   0        0        0      882 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js
+-rw-r--r--   0        0        0      660 2023-06-02 07:02:14.271943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js
+-rw-r--r--   0        0        0     1002 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js
+-rw-r--r--   0        0        0      743 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js
+-rw-r--r--   0        0        0      773 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js
+-rw-r--r--   0        0        0     1100 2023-06-02 07:02:14.303943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js
+-rw-r--r--   0        0        0     2325 2023-06-02 07:02:14.311943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js
+-rw-r--r--   0        0        0     2078 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js
+-rw-r--r--   0        0        0     1752 2023-06-02 07:02:14.319943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js
+-rw-r--r--   0        0        0     1941 2023-06-02 07:02:14.399943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js
+-rw-r--r--   0        0        0      727 2023-06-02 07:02:14.351943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js
+-rw-r--r--   0        0        0     3180 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js
+-rw-r--r--   0        0        0     1613 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/env.js
+-rw-r--r--   0        0        0     6925 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js
+-rw-r--r--   0        0        0      819 2023-06-02 07:02:14.375943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/error.js
+-rw-r--r--   0        0        0     8501 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/index.js
+-rw-r--r--   0        0        0    19360 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js
+-rw-r--r--   0        0        0     4878 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/is.js
+-rw-r--r--   0        0        0     2403 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/logger.js
+-rw-r--r--   0        0        0     1096 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/memo.js
+-rw-r--r--   0        0        0     7809 2023-06-02 07:02:14.435944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/misc.js
+-rw-r--r--   0        0        0     2703 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js
+-rw-r--r--   0        0        0     2267 2023-06-02 07:02:14.447944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/node.js
+-rw-r--r--   0        0        0     9677 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js
+-rw-r--r--   0        0        0     9449 2023-06-02 07:02:14.463944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/object.js
+-rw-r--r--   0        0        0     5629 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/path.js
+-rw-r--r--   0        0        0     3592 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js
+-rw-r--r--   0        0        0     3349 2023-06-02 07:02:14.475944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js
+-rw-r--r--   0        0        0     9445 2023-06-02 07:02:14.479944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js
+-rw-r--r--   0        0        0     1725 2023-06-02 07:02:14.483944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/severity.js
+-rw-r--r--   0        0        0     4725 2023-06-02 07:02:14.487944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js
+-rw-r--r--   0        0        0     3764 2023-06-02 07:02:14.491944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/string.js
+-rw-r--r--   0        0        0     4591 2023-06-02 07:02:14.491944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/supports.js
+-rw-r--r--   0        0        0     4495 2023-06-02 07:02:14.495944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js
+-rw-r--r--   0        0        0     7845 2023-06-02 07:02:14.499944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/time.js
+-rw-r--r--   0        0        0     1094 2023-06-02 07:02:14.503944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js
+-rw-r--r--   0        0        0     2341 2023-06-02 07:02:14.503944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/url.js
+-rw-r--r--   0        0        0     3919 2023-06-02 07:02:14.507944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js
+-rw-r--r--   0        0        0     2198 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js
+-rw-r--r--   0        0        0     1235 2023-06-02 07:02:14.491944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js
+-rw-r--r--   0        0        0     3202 2023-06-02 07:02:14.511944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js
+-rw-r--r--   0        0        0     5598 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/baggage.js
+-rw-r--r--   0        0        0     4394 2023-06-02 07:02:14.343943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/browser.js
+-rw-r--r--   0        0        0     1188 2023-06-02 07:02:14.223942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js
+-rw-r--r--   0        0        0     2127 2023-06-02 07:02:14.247943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js
+-rw-r--r--   0        0        0     1639 2023-06-02 07:02:14.259943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js
+-rw-r--r--   0        0        0      738 2023-06-02 07:02:14.263943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js
+-rw-r--r--   0        0        0      801 2023-06-02 07:02:14.271943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js
+-rw-r--r--   0        0        0      577 2023-06-02 07:02:14.275943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js
+-rw-r--r--   0        0        0      917 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js
+-rw-r--r--   0        0        0      647 2023-06-02 07:02:14.295943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js
+-rw-r--r--   0        0        0      687 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js
+-rw-r--r--   0        0        0     1013 2023-06-02 07:02:14.303943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js
+-rw-r--r--   0        0        0     2245 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js
+-rw-r--r--   0        0        0     2000 2023-06-02 07:02:14.319943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js
+-rw-r--r--   0        0        0     1652 2023-06-02 07:02:14.323943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js
+-rw-r--r--   0        0        0      890 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js
+-rw-r--r--   0        0        0      645 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js
+-rw-r--r--   0        0        0     3038 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/dsn.js
+-rw-r--r--   0        0        0     1511 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/env.js
+-rw-r--r--   0        0        0     6527 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/envelope.js
+-rw-r--r--   0        0        0      744 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/error.js
+-rw-r--r--   0        0        0     3442 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/index.js
+-rw-r--r--   0        0        0    19108 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/instrument.js
+-rw-r--r--   0        0        0     4529 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/is.js
+-rw-r--r--   0        0        0     2259 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/logger.js
+-rw-r--r--   0        0        0     1021 2023-06-02 07:02:14.431944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/memo.js
+-rw-r--r--   0        0        0     7523 2023-06-02 07:02:14.439944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/misc.js
+-rw-r--r--   0        0        0     2635 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js
+-rw-r--r--   0        0        0     2155 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/node.js
+-rw-r--r--   0        0        0     9577 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/normalize.js
+-rw-r--r--   0        0        0     9181 2023-06-02 07:02:14.463944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/object.js
+-rw-r--r--   0        0        0     5442 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/path.js
+-rw-r--r--   0        0        0     3515 2023-06-02 07:02:14.475944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js
+-rw-r--r--   0        0        0     3159 2023-06-02 07:02:14.479944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js
+-rw-r--r--   0        0        0     9276 2023-06-02 07:02:14.479944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js
+-rw-r--r--   0        0        0     1579 2023-06-02 07:02:14.483944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/severity.js
+-rw-r--r--   0        0        0     4480 2023-06-02 07:02:14.487944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js
+-rw-r--r--   0        0        0     3597 2023-06-02 07:02:14.491944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/string.js
+-rw-r--r--   0        0        0     4291 2023-06-02 07:02:14.491944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/supports.js
+-rw-r--r--   0        0        0     4364 2023-06-02 07:02:14.495944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js
+-rw-r--r--   0        0        0     7630 2023-06-02 07:02:14.499944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/time.js
+-rw-r--r--   0        0        0      979 2023-06-02 07:02:14.503944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/tracing.js
+-rw-r--r--   0        0        0     2169 2023-06-02 07:02:14.507944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/url.js
+-rw-r--r--   0        0        0     3833 2023-06-02 07:02:14.507944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js
+-rw-r--r--   0        0        0     2114 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js
+-rw-r--r--   0        0        0     1151 2023-06-02 07:02:14.495944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js
+-rw-r--r--   0        0        0     3073 2023-06-02 07:02:14.511944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js
+-rw-r--r--   0        0        0      720 2023-06-02 07:02:14.511944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/package.json
+-rw-r--r--   0        0        0     1549 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js
+-rw-r--r--   0        0        0     9662 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js
+-rw-r--r--   0        0        0    16045 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js
+-rw-r--r--   0        0        0      839 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js
+-rw-r--r--   0        0        0     9441 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js
+-rw-r--r--   0        0        0     2597 2023-06-02 07:02:14.463944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js
+-rw-r--r--   0        0        0      199 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/types.js
+-rw-r--r--   0        0        0     3902 2023-06-02 07:02:14.347943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js
+-rw-r--r--   0        0        0     2257 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js
+-rw-r--r--   0        0        0     3094 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js
+-rw-r--r--   0        0        0      843 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js
+-rw-r--r--   0        0        0     1031 2023-06-02 07:02:14.335943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js
+-rw-r--r--   0        0        0      973 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js
+-rw-r--r--   0        0        0     1851 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js
+-rw-r--r--   0        0        0     1795 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js
+-rw-r--r--   0        0        0     1563 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js
+-rw-r--r--   0        0        0      943 2023-06-02 07:02:14.439944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js
+-rw-r--r--   0        0        0     1379 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js
+-rw-r--r--   0        0        0     1735 2023-06-02 07:02:14.323943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js
+-rw-r--r--   0        0        0     2157 2023-06-02 07:02:14.399943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js
+-rw-r--r--   0        0        0     5368 2023-06-02 07:02:14.199942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js
+-rw-r--r--   0        0        0    12006 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js
+-rw-r--r--   0        0        0     2405 2023-06-02 07:02:14.379943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js
+-rw-r--r--   0        0        0     1184 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js
+-rw-r--r--   0        0        0     9526 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js
+-rw-r--r--   0        0        0     2645 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js
+-rw-r--r--   0        0        0     3457 2023-06-02 07:02:14.447944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js
+-rw-r--r--   0        0        0     1883 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js
+-rw-r--r--   0        0        0      793 2023-06-02 07:02:14.427944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js
+-rw-r--r--   0        0        0     1429 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js
+-rw-r--r--   0        0        0     9706 2023-06-02 07:02:14.307943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js
+-rw-r--r--   0        0        0    15585 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js
+-rw-r--r--   0        0        0      735 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js
+-rw-r--r--   0        0        0     9229 2023-06-02 07:02:14.459944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js
+-rw-r--r--   0        0        0     2501 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js
+-rw-r--r--   0        0        0      127 2023-06-02 07:02:14.467944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/types.js
+-rw-r--r--   0        0        0     3788 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js
+-rw-r--r--   0        0        0     2121 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js
+-rw-r--r--   0        0        0     2938 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js
+-rw-r--r--   0        0        0      767 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js
+-rw-r--r--   0        0        0      951 2023-06-02 07:02:14.335943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js
+-rw-r--r--   0        0        0      871 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js
+-rw-r--r--   0        0        0     1739 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js
+-rw-r--r--   0        0        0     1689 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js
+-rw-r--r--   0        0        0     1425 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js
+-rw-r--r--   0        0        0      872 2023-06-02 07:02:14.439944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js
+-rw-r--r--   0        0        0     1301 2023-06-02 07:02:14.443944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js
+-rw-r--r--   0        0        0     1668 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js
+-rw-r--r--   0        0        0     1080 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js
+-rw-r--r--   0        0        0     5248 2023-06-02 07:02:14.235942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js
+-rw-r--r--   0        0        0    11942 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js
+-rw-r--r--   0        0        0     2340 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js
+-rw-r--r--   0        0        0     1039 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js
+-rw-r--r--   0        0        0     9463 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js
+-rw-r--r--   0        0        0     2576 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js
+-rw-r--r--   0        0        0     3385 2023-06-02 07:02:14.451944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js
+-rw-r--r--   0        0        0     1802 2023-06-02 07:02:14.455944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js
+-rw-r--r--   0        0        0      693 2023-06-02 07:02:14.435944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js
+-rw-r--r--   0        0        0      723 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/package.json
+-rw-r--r--   0        0        0     7910 2023-06-02 07:02:14.139942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/agent-base/dist/src/index.js
+-rw-r--r--   0        0        0      495 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/agent-base/dist/src/promisify.js
+-rw-r--r--   0        0        0     1635 2023-06-02 07:02:14.171942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/agent-base/package.json
+-rw-r--r--   0        0        0       27 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/.eslintrc.json
+-rw-r--r--   0        0        0       60 2023-06-02 07:02:14.167942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/.npmpackagejsonlintrc.json
+-rw-r--r--   0        0        0       50 2023-06-02 07:02:14.179942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/.releaserc.json
+-rw-r--r--   0        0        0      539 2023-06-02 07:02:14.123942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/build/lib/boolean.js
+-rw-r--r--   0        0        0      463 2023-06-02 07:02:14.139942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/build/lib/index.js
+-rw-r--r--   0        0        0      646 2023-06-02 07:02:14.151942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js
+-rw-r--r--   0        0        0      228 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/licenseCheck.json
+-rw-r--r--   0        0        0      982 2023-06-02 07:02:14.195942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/package.json
+-rw-r--r--   0        0        0      323 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/tsconfig.json
+-rw-r--r--   0        0        0     4047 2023-06-02 07:02:14.071941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/cookie/index.js
+-rw-r--r--   0        0        0     1104 2023-06-02 07:02:14.123942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/cookie/package.json
+-rw-r--r--   0        0        0     1419 2023-06-02 07:02:14.215942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/package.json
+-rw-r--r--   0        0        0     6010 2023-06-02 07:02:14.135942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/browser.js
+-rw-r--r--   0        0        0     6289 2023-06-02 07:02:14.179942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/common.js
+-rw-r--r--   0        0        0      314 2023-06-02 07:02:14.187942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/index.js
+-rw-r--r--   0        0        0     4685 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/node.js
+-rw-r--r--   0        0        0     1429 2023-06-02 07:02:14.151942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/define-properties/index.js
+-rw-r--r--   0        0        0     2245 2023-06-02 07:02:14.167942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0       25 2023-06-02 07:02:14.031941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/detect-node/browser.js
+-rw-r--r--   0        0        0      184 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/detect-node/index.esm.js
+-rw-r--r--   0        0        0      186 2023-06-02 07:02:14.067941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/detect-node/index.js
+-rw-r--r--   0        0        0      607 2023-06-02 07:02:14.119942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/detect-node/package.json
+-rw-r--r--   0        0        0     2582 2023-06-02 07:02:14.179942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/es6/index.js
+-rw-r--r--   0        0        0     2703 2023-06-02 07:02:14.195942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/lib/index.js
+-rw-r--r--   0        0        0     1404 2023-06-02 07:02:14.055941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/package.json
+-rw-r--r--   0        0        0      461 2023-06-02 07:02:14.031941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/escape-string-regexp/index.js
+-rw-r--r--   0        0        0      686 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     4140 2023-06-02 07:02:14.187942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/.jscs.json
+-rw-r--r--   0        0        0     1463 2023-06-02 07:02:14.135942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/implementation.js
+-rw-r--r--   0        0        0      126 2023-06-02 07:02:14.147942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/index.js
+-rw-r--r--   0        0        0     1498 2023-06-02 07:02:14.031941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     8991 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/test/index.js
+-rw-r--r--   0        0        0    13145 2023-06-02 07:02:14.195942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/index.js
+-rw-r--r--   0        0        0     2349 2023-06-02 07:02:14.211942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     8767 2023-06-02 07:02:14.147942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js
+-rw-r--r--   0        0        0       37 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/bootstrap.js
+-rw-r--r--   0        0        0      414 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/Logger.js
+-rw-r--r--   0        0        0     6510 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/Agent.js
+-rw-r--r--   0        0        0      905 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js
+-rw-r--r--   0        0        0     1542 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js
+-rw-r--r--   0        0        0      814 2023-06-02 07:02:14.387943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/index.js
+-rw-r--r--   0        0        0      575 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/errors.js
+-rw-r--r--   0        0        0     6002 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js
+-rw-r--r--   0        0        0     1086 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js
+-rw-r--r--   0        0        0      694 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/index.js
+-rw-r--r--   0        0        0      476 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/index.js
+-rw-r--r--   0        0        0      759 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js
+-rw-r--r--   0        0        0      402 2023-06-02 07:02:14.391943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/routines/index.js
+-rw-r--r--   0        0        0      165 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/types.js
+-rw-r--r--   0        0        0     1479 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js
+-rw-r--r--   0        0        0      866 2023-06-02 07:02:14.395943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/index.js
+-rw-r--r--   0        0        0     1341 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js
+-rw-r--r--   0        0        0     1065 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js
+-rw-r--r--   0        0        0     2585 2023-06-02 07:02:14.423944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/package.json
+-rw-r--r--   0        0        0      129 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/Logger.js
+-rw-r--r--   0        0        0     6762 2023-06-02 07:02:14.327943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/Agent.js
+-rw-r--r--   0        0        0      733 2023-06-02 07:02:14.375943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js
+-rw-r--r--   0        0        0     1346 2023-06-02 07:02:14.383943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js
+-rw-r--r--   0        0        0      174 2023-06-02 07:02:14.399943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/index.js
+-rw-r--r--   0        0        0      299 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/errors.js
+-rw-r--r--   0        0        0     5715 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js
+-rw-r--r--   0        0        0      882 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js
+-rw-r--r--   0        0        0      160 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/factories/index.js
+-rw-r--r--   0        0        0      100 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/index.js
+-rw-r--r--   0        0        0      550 2023-06-02 07:02:14.351943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js
+-rw-r--r--   0        0        0       60 2023-06-02 07:02:14.403943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/routines/index.js
+-rw-r--r--   0        0        0     1567 2023-06-02 07:02:14.419944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/types.js
+-rw-r--r--   0        0        0     1197 2023-06-02 07:02:14.335943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js
+-rw-r--r--   0        0        0      200 2023-06-02 07:02:14.407944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/index.js
+-rw-r--r--   0        0        0     1022 2023-06-02 07:02:14.411944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js
+-rw-r--r--   0        0        0      874 2023-06-02 07:02:14.415943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js
+-rw-r--r--   0        0        0       36 2023-06-02 07:02:14.147942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/auto.js
+-rw-r--r--   0        0        0      254 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/implementation.browser.js
+-rw-r--r--   0        0        0       40 2023-06-02 07:02:14.167942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/implementation.js
+-rw-r--r--   0        0        0      408 2023-06-02 07:02:14.195942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/index.js
+-rw-r--r--   0        0        0     2418 2023-06-02 07:02:14.247943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0      251 2023-06-02 07:02:14.215942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/polyfill.js
+-rw-r--r--   0        0        0      722 2023-06-02 07:02:14.223942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/shim.js
+-rw-r--r--   0        0        0      213 2023-06-02 07:02:14.187942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/implementation.js
+-rw-r--r--   0        0        0      196 2023-06-02 07:02:14.203942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/index.js
+-rw-r--r--   0        0        0      767 2023-06-02 07:02:14.211942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/native.js
+-rw-r--r--   0        0        0      900 2023-06-02 07:02:14.231942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/shimmed.js
+-rw-r--r--   0        0        0     1399 2023-06-02 07:02:14.239942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/tests.js
+-rw-r--r--   0        0        0     1011 2023-06-02 07:02:13.963940 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has/package.json
+-rw-r--r--   0        0        0      129 2023-06-02 07:02:14.135942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has/src/index.js
+-rw-r--r--   0        0        0      331 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has/test/index.js
+-rw-r--r--   0        0        0      817 2023-06-02 07:02:14.115942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/index.js
+-rw-r--r--   0        0        0     1933 2023-06-02 07:02:14.163942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     1405 2023-06-02 07:02:14.143942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/test/index.js
+-rw-r--r--   0        0        0      420 2023-06-02 07:02:14.163942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/index.js
+-rw-r--r--   0        0        0     2648 2023-06-02 07:02:14.215942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     1761 2023-06-02 07:02:14.203942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/shams.js
+-rw-r--r--   0        0        0      654 2023-06-02 07:02:14.195942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/index.js
+-rw-r--r--   0        0        0      723 2023-06-02 07:02:14.131942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/shams/core-js.js
+-rw-r--r--   0        0        0      686 2023-06-02 07:02:14.155942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js
+-rw-r--r--   0        0        0     2021 2023-06-02 07:02:14.211942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/tests.js
+-rw-r--r--   0        0        0     7841 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/agent.js
+-rw-r--r--   0        0        0      579 2023-06-02 07:02:14.067941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/index.js
+-rw-r--r--   0        0        0     2460 2023-06-02 07:02:14.115942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js
+-rw-r--r--   0        0        0     1405 2023-06-02 07:02:14.131942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/package.json
+-rw-r--r--   0        0        0      796 2023-06-02 07:02:13.963940 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/package.json
+-rw-r--r--   0        0        0      907 2023-06-02 07:02:14.131942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/stringify.js
+-rw-r--r--   0        0        0     7550 2023-06-02 07:02:14.203942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js
+-rw-r--r--   0        0        0     8186 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru-cache/index.js
+-rw-r--r--   0        0        0      705 2023-06-02 07:02:14.119942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0     4625 2023-06-02 07:02:14.131942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/benchmark.js
+-rw-r--r--   0        0        0     7934 2023-06-02 07:02:14.175942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/lru.js
+-rw-r--r--   0        0        0      901 2023-06-02 07:02:13.959941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/package.json
+-rw-r--r--   0        0        0     7366 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/test.js
+-rw-r--r--   0        0        0      227 2023-06-02 07:02:14.235942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/tsconfig.json
+-rw-r--r--   0        0        0     1785 2023-06-02 07:02:14.031941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/matcher/index.js
+-rw-r--r--   0        0        0      871 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/matcher/package.json
+-rw-r--r--   0        0        0     3023 2023-06-02 07:02:14.027941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/ms/index.js
+-rw-r--r--   0        0        0      705 2023-06-02 07:02:13.959941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/ms/package.json
+-rw-r--r--   0        0        0     3218 2023-06-02 07:02:14.143942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/implementation.js
+-rw-r--r--   0        0        0      823 2023-06-02 07:02:14.155942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/index.js
+-rw-r--r--   0        0        0      422 2023-06-02 07:02:14.163942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/isArguments.js
+-rw-r--r--   0        0        0     1903 2023-06-02 07:02:13.959941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0       61 2023-06-02 07:02:14.199942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/test/index.js
+-rw-r--r--   0        0        0      274 2023-06-02 07:02:14.227942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/constants.js
+-rw-r--r--   0        0        0     6377 2023-06-02 07:02:14.235942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createLogger.js
+-rw-r--r--   0        0        0     1103 2023-06-02 07:02:14.243942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js
+-rw-r--r--   0        0        0      629 2023-06-02 07:02:14.247943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js
+-rw-r--r--   0        0        0     2493 2023-06-02 07:02:14.251942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js
+-rw-r--r--   0        0        0      914 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/index.js
+-rw-r--r--   0        0        0     1186 2023-06-02 07:02:14.259943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/log.js
+-rw-r--r--   0        0        0       47 2023-06-02 07:02:14.263943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/types.js
+-rw-r--r--   0        0        0     2350 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/package.json
+-rwxr-xr-x   0        0        0     4823 2023-06-02 07:02:14.339943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/bin/semver.js
+-rw-r--r--   0        0        0     3563 2023-06-02 07:02:14.187942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/comparator.js
+-rw-r--r--   0        0        0      129 2023-06-02 07:02:14.271943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/index.js
+-rw-r--r--   0        0        0    14283 2023-06-02 07:02:14.323943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/range.js
+-rw-r--r--   0        0        0     8673 2023-06-02 07:02:14.347943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/semver.js
+-rw-r--r--   0        0        0      191 2023-06-02 07:02:14.067941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/clean.js
+-rw-r--r--   0        0        0      947 2023-06-02 07:02:14.135942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/cmp.js
+-rw-r--r--   0        0        0     1505 2023-06-02 07:02:14.159942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/coerce.js
+-rw-r--r--   0        0        0      267 2023-06-02 07:02:14.203942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/compare-build.js
+-rw-r--r--   0        0        0      118 2023-06-02 07:02:14.211942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/compare-loose.js
+-rw-r--r--   0        0        0      156 2023-06-02 07:02:14.215942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/compare.js
+-rw-r--r--   0        0        0     1303 2023-06-02 07:02:14.243942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/diff.js
+-rw-r--r--   0        0        0      112 2023-06-02 07:02:14.247943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/eq.js
+-rw-r--r--   0        0        0      110 2023-06-02 07:02:14.251942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/gt.js
+-rw-r--r--   0        0        0      113 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/gte.js
+-rw-r--r--   0        0        0      464 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/inc.js
+-rw-r--r--   0        0        0      110 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/lt.js
+-rw-r--r--   0        0        0      113 2023-06-02 07:02:14.279943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/lte.js
+-rw-r--r--   0        0        0      122 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/major.js
+-rw-r--r--   0        0        0      122 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/minor.js
+-rw-r--r--   0        0        0      114 2023-06-02 07:02:14.303943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/neq.js
+-rw-r--r--   0        0        0      317 2023-06-02 07:02:14.311943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/parse.js
+-rw-r--r--   0        0        0      122 2023-06-02 07:02:14.311943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/patch.js
+-rw-r--r--   0        0        0      220 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/prerelease.js
+-rw-r--r--   0        0        0      118 2023-06-02 07:02:14.327943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/rcompare.js
+-rw-r--r--   0        0        0      149 2023-06-02 07:02:14.331943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/rsort.js
+-rw-r--r--   0        0        0      233 2023-06-02 07:02:14.335943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/satisfies.js
+-rw-r--r--   0        0        0      147 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/sort.js
+-rw-r--r--   0        0        0      162 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/valid.js
+-rw-r--r--   0        0        0     2616 2023-06-02 07:02:14.275943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/index.js
+-rw-r--r--   0        0        0      657 2023-06-02 07:02:14.231942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/constants.js
+-rw-r--r--   0        0        0      226 2023-06-02 07:02:14.239942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/debug.js
+-rw-r--r--   0        0        0      410 2023-06-02 07:02:14.267943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/identifiers.js
+-rw-r--r--   0        0        0      324 2023-06-02 07:02:14.307943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/parse-options.js
+-rw-r--r--   0        0        0     6672 2023-06-02 07:02:14.327943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/re.js
+-rw-r--r--   0        0        0     1748 2023-06-02 07:02:14.371943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/package.json
+-rw-r--r--   0        0        0       69 2023-06-02 07:02:14.315943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/preload.js
+-rw-r--r--   0        0        0      217 2023-06-02 07:02:14.263943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/gtr.js
+-rw-r--r--   0        0        0      210 2023-06-02 07:02:14.275943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/intersects.js
+-rw-r--r--   0        0        0      213 2023-06-02 07:02:14.283943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/ltr.js
+-rw-r--r--   0        0        0      579 2023-06-02 07:02:14.287943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/max-satisfying.js
+-rw-r--r--   0        0        0      577 2023-06-02 07:02:14.295943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/min-satisfying.js
+-rw-r--r--   0        0        0     1500 2023-06-02 07:02:14.299943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/min-version.js
+-rw-r--r--   0        0        0     2190 2023-06-02 07:02:14.307943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/outside.js
+-rw-r--r--   0        0        0     1341 2023-06-02 07:02:14.355943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/simplify.js
+-rw-r--r--   0        0        0     7510 2023-06-02 07:02:14.359943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/subset.js
+-rw-r--r--   0        0        0      268 2023-06-02 07:02:14.363943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/to-comparators.js
+-rw-r--r--   0        0        0      312 2023-06-02 07:02:14.367943 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/valid.js
+-rw-r--r--   0        0        0      210 2023-06-02 07:02:14.143942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/example/cmp.js
+-rw-r--r--   0        0        0      181 2023-06-02 07:02:14.155942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/example/lex.js
+-rw-r--r--   0        0        0      372 2023-06-02 07:02:14.067941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/index.js
+-rw-r--r--   0        0        0      659 2023-06-02 07:02:13.963940 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/package.json
+-rw-r--r--   0        0        0      444 2023-06-02 07:02:14.183942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/test/cmp.js
+-rw-r--r--   0        0        0     2235 2023-06-02 07:02:14.031941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/serialize-error/index.js
+-rw-r--r--   0        0        0      743 2023-06-02 07:02:14.051941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/serialize-error/package.json
+-rwxr-xr-x   0        0        0       57 2023-06-02 07:02:14.255942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/bin/snyk
+-rw-r--r--   0        0        0      150 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/config.default.json
+-rw-r--r--   0        0        0     1838 2023-06-02 07:02:14.471944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/110.index.js
+-rw-r--r--   0        0        0   103302 2023-06-02 07:02:14.487944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/213.index.js
+-rw-r--r--   0        0        0   133844 2023-06-02 07:02:14.499944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/31.index.js
+-rw-r--r--   0        0        0   173511 2023-06-02 07:02:14.515944 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/38.index.js
+-rw-r--r--   0        0        0   161488 2023-06-02 07:02:14.539945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/384.index.js
+-rw-r--r--   0        0        0   128289 2023-06-02 07:02:14.551945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/395.index.js
+-rw-r--r--   0        0        0     2969 2023-06-02 07:02:14.551945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/477.index.js
+-rw-r--r--   0        0        0   557584 2023-06-02 07:02:14.611945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/503.index.js
+-rw-r--r--   0        0        0    22931 2023-06-02 07:02:14.615945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/519.index.js
+-rw-r--r--   0        0        0      612 2023-06-02 07:02:14.623945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/522.index.js
+-rw-r--r--   0        0        0   569531 2023-06-02 07:02:14.683946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/535.index.js
+-rw-r--r--   0        0        0     7242 2023-06-02 07:02:14.683946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/542.index.js
+-rw-r--r--   0        0        0     1061 2023-06-02 07:02:14.687945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/575.index.js
+-rw-r--r--   0        0        0    32497 2023-06-02 07:02:14.691945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/663.index.js
+-rw-r--r--   0        0        0    18697 2023-06-02 07:02:14.691945 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/726.index.js
+-rw-r--r--   0        0        0   106008 2023-06-02 07:02:14.707946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/741.index.js
+-rw-r--r--   0        0        0   280086 2023-06-02 07:02:14.731946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/784.index.js
+-rw-r--r--   0        0        0   265629 2023-06-02 07:02:14.751946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/790.index.js
+-rw-r--r--   0        0        0     3295 2023-06-02 07:02:14.751946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/831.index.js
+-rw-r--r--   0        0        0    11175 2023-06-02 07:02:14.763946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/85.index.js
+-rw-r--r--   0        0        0     1445 2023-06-02 07:02:14.763946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/855.index.js
+-rw-r--r--   0        0        0      523 2023-06-02 07:02:14.767946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/875.index.js
+-rw-r--r--   0        0        0   267291 2023-06-02 07:02:14.775946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/895.index.js
+-rw-r--r--   0        0        0   227159 2023-06-02 07:02:14.783946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/905.index.js
+-rw-r--r--   0        0        0  4489688 2023-06-02 07:02:14.839946 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/917.index.js
+-rw-r--r--   0        0        0  8653273 2023-06-02 07:02:14.935947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/95.index.js
+-rw-r--r--   0        0        0      592 2023-06-02 07:02:14.935947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/959.index.js
+-rw-r--r--   0        0        0    93818 2023-06-02 07:02:14.939947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/970.index.js
+-rw-r--r--   0        0        0    20674 2023-06-02 07:02:14.939947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/974.index.js
+-rw-r--r--   0        0        0    14335 2023-06-02 07:02:14.939947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/989.index.js
+-rw-r--r--   0        0        0  1682422 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/index.js
+-rw-r--r--   0        0        0   613426 2023-06-02 07:02:15.375950 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm
+-rw-r--r--   0        0        0   614892 2023-06-02 07:02:14.963947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json
+-rw-r--r--   0        0        0      140 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/jest.config.js
+-rw-r--r--   0        0        0     1094 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/package.json
+-rw-r--r--   0        0        0     1203 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/distPackage.py
+-rw-r--r--   0        0        0      844 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/package.py
+-rw-r--r--   0        0        0      726 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py
+-rw-r--r--   0        0        0     9460 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py
+-rw-r--r--   0        0        0     5098 2023-06-02 07:02:15.211949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2023-06-02 07:02:15.211949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2023-06-02 07:02:15.211949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/version.py
+-rw-r--r--   0        0        0    13551 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py
+-rw-r--r--   0        0        0     1788 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pipfile.py
+-rw-r--r--   0        0        0   273365 2023-06-02 07:02:15.203949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pyparsing.py
+-rw-r--r--   0        0        0       92 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/core.py
+-rw-r--r--   0        0        0    11254 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py
+-rw-r--r--   0        0        0     3815 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py
+-rw-r--r--   0        0        0     1508 2023-06-02 07:02:15.203949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/reqPackage.py
+-rw-r--r--   0        0        0      353 2023-06-02 07:02:15.195949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py
+-rw-r--r--   0        0        0     3092 2023-06-02 07:02:15.199949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py
+-rw-r--r--   0        0        0    10020 2023-06-02 07:02:15.211949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py
+-rw-r--r--   0        0        0      405 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/vcs.py
+-rw-r--r--   0        0        0     1427 2023-06-02 07:02:15.211949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/setup_file.py
+-rw-r--r--   0        0        0     6291 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py
+-rw-r--r--   0        0        0     2258 2023-06-02 07:02:15.215949 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/utils.py
+-rw-r--r--   0        0        0      246 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/src/generated/binary-deployments.json
+-rw-r--r--   0        0        0      186 2023-06-02 07:02:14.963947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/tsconfig.json
+-rw-r--r--   0        0        0      843 2023-06-02 07:02:14.939947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js
+-rw-r--r--   0        0        0    11438 2023-06-02 07:02:14.939947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/common.js
+-rw-r--r--   0        0        0      246 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/generated/binary-deployments.json
+-rw-r--r--   0        0        0     2017 2023-06-02 07:02:14.959947 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/index.js
+-rw-r--r--   0        0        0      498 2023-06-02 07:02:14.171942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/dist/angular-sprintf.min.js
+-rw-r--r--   0        0        0     3675 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js
+-rw-r--r--   0        0        0      818 2023-06-02 07:02:13.927940 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/package.json
+-rw-r--r--   0        0        0      663 2023-06-02 07:02:14.227942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js
+-rw-r--r--   0        0        0     9250 2023-06-02 07:02:14.243942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/src/sprintf.js
+-rw-r--r--   0        0        0      943 2023-06-02 07:02:14.027941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/modules/index.js
+-rw-r--r--   0        0        0       26 2023-06-02 07:02:14.191942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      915 2023-06-02 07:02:14.199942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/package.json
+-rw-r--r--   0        0        0      824 2023-06-02 07:02:14.111941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js
+-rw-r--r--   0        0        0       71 2023-06-02 07:02:14.207942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0    10274 2023-06-02 07:02:14.155942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/tslib.es6.js
+-rw-r--r--   0        0        0    13204 2023-06-02 07:02:14.171942 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/tslib.js
+-rw-r--r--   0        0        0      782 2023-06-02 07:02:13.959941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0      207 2023-06-02 07:02:13.959941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/yallist/iterator.js
+-rw-r--r--   0        0        0      652 2023-06-02 07:02:14.063941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/yallist/package.json
+-rw-r--r--   0        0        0     8411 2023-06-02 07:02:14.027941 c2cciutils-1.6.0.dev99/c2cciutils/node_modules/yallist/yallist.js
+-rw-r--r--   0        0        0    25304 2023-06-02 07:02:17.343963 c2cciutils-1.6.0.dev99/c2cciutils/package-lock.json
+-rw-r--r--   0        0        0      134 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/package.json
+-rw-r--r--   0        0        0    10112 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/pr_checks.py
+-rw-r--r--   0        0        0    17707 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/publish.py
+-rw-r--r--   0        0        0     1548 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/schema-applications.json
+-rw-r--r--   0        0        0    22561 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/schema.json
+-rw-r--r--   0        0        0       36 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/audit.py
+-rw-r--r--   0        0        0     3039 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/clean.py
+-rw-r--r--   0        0        0     1712 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/docker_logs.py
+-rw-r--r--   0        0        0     1316 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/docker_versions_gen.py
+-rw-r--r--   0        0        0     4385 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/download_applications.py
+-rw-r--r--   0        0        0      375 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/env.py
+-rw-r--r--   0        0        0       69 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/__init__.py
+-rw-r--r--   0        0        0     3274 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/db.py
+-rw-r--r--   0        0        0      921 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/install.py
+-rw-r--r--   0        0        0     2655 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/logs.py
+-rw-r--r--   0        0        0     5661 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/wait.py
+-rw-r--r--   0        0        0     1162 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/main.py
+-rw-r--r--   0        0        0     2150 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/pin_pipenv.py
+-rw-r--r--   0        0        0     2182 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/pr_checks.py
+-rw-r--r--   0        0        0    18222 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/publish.py
+-rw-r--r--   0        0        0     2804 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/scripts/trigger_image_update.py
+-rw-r--r--   0        0        0     1517 2023-06-02 07:02:00.539842 c2cciutils-1.6.0.dev99/c2cciutils/security.py
+-rw-r--r--   0        0        0     4334 2023-06-02 07:16:07.421802 c2cciutils-1.6.0.dev99/pyproject.toml
+-rw-r--r--   0        0        0   358583 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev99/setup.py
+-rw-r--r--   0        0        0    16769 1970-01-01 00:00:00.000000 c2cciutils-1.6.0.dev99/PKG-INFO
```

### Comparing `c2cciutils-1.6.0.dev98/LICENSE` & `c2cciutils-1.6.0.dev99/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/README.md` & `c2cciutils-1.6.0.dev99/README.md`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/__init__.py` & `c2cciutils-1.6.0.dev99/c2cciutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/applications_definition.py` & `c2cciutils-1.6.0.dev99/c2cciutils/applications_definition.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/audit.py` & `c2cciutils-1.6.0.dev99/c2cciutils/audit.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/configuration.py` & `c2cciutils-1.6.0.dev99/c2cciutils/configuration.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/env.py` & `c2cciutils-1.6.0.dev99/c2cciutils/env.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/lib/docker.py` & `c2cciutils-1.6.0.dev99/c2cciutils/lib/docker.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/.package-lock.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/api.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/api.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/baseclient.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/envelope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/exports.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/exports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/hub.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/hub.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integration.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integration.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integrations/functiontostring.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/integrations/inboundfilters.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/scope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/scope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/sdk.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/session.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/session.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/sessionflusher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/hubextensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/idletransaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/span.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/spanstatus.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/transaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/tracing/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/base.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/multiplexed.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/multiplexed.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/transports/offline.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/utils/hasTracingEnabled.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/cjs/utils/prepareEvent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/api.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/api.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/baseclient.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/baseclient.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/envelope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/exports.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/exports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/hub.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/hub.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integration.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integration.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integrations/functiontostring.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/integrations/inboundfilters.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/scope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/scope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/sdk.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/session.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/session.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/sessionflusher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/hubextensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/idletransaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/span.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/spanstatus.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/tracing/transaction.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/base.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/base.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/multiplexed.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/multiplexed.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/transports/offline.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/utils/hasTracingEnabled.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/esm/utils/prepareEvent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/core/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/core/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/domain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/domain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/hooks.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/hooks.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/async/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/async/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/client.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/client.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/eventbuilder.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/handlers.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/handlers.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/console.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/context.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/contextlines.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/linkederrors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/localvariables.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/modules.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/onuncaughtexception.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/onunhandledrejection.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/undici/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/errorhandling.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/integrations/utils/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/module.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/module.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/requestDataDeprecated.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/sdk.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/tracing/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/transports/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/cjs/utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/cjs/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/domain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/domain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/hooks.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/hooks.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/async/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/async/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/client.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/client.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/eventbuilder.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/handlers.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/handlers.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/console.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/context.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/contextlines.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/linkederrors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/localvariables.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/modules.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/onuncaughtexception.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/onunhandledrejection.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/undici/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/errorhandling.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/integrations/utils/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/module.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/module.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/requestDataDeprecated.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/sdk.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/sdk.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/tracing/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/transports/http.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/transports/http.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/esm/utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/esm/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/node/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/node/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/baggage.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/browser.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncNullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_asyncOptionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createNamedExportFrom.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_createStarExport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopNamespaceDefaultOnly.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_interopRequireWildcard.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_nullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/_optionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/buildPolyfills/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/clientreport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/dsn.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/env.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/env.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/error.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/error.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/instrument.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/is.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/is.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/logger.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/logger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/memo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/memo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/misc.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/misc.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/node-stack-trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/node.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/normalize.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/object.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/object.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/path.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/path.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/promisebuffer.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/ratelimit.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/severity.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/severity.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/stacktrace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/string.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/string.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/supports.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/supports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/syncpromise.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/time.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/time.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/tracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/url.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/url.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/userIntegrations.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/vendor/escapeStringForRegex.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/vendor/supportsHistory.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/cjs/worldwide.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/baggage.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/baggage.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/browser.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncNullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_asyncOptionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createNamedExportFrom.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_createStarExport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopNamespaceDefaultOnly.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireDefault.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_interopRequireWildcard.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_nullishCoalesce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChain.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/_optionalChainDelete.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/buildPolyfills/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/clientreport.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/dsn.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/dsn.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/env.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/env.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/envelope.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/envelope.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/error.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/error.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/instrument.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/instrument.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/is.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/is.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/logger.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/logger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/memo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/memo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/misc.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/misc.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/node-stack-trace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/node.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/normalize.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/normalize.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/object.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/object.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/path.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/path.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/promisebuffer.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/ratelimit.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/requestdata.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/severity.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/severity.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/stacktrace.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/string.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/string.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/supports.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/supports.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/syncpromise.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/time.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/time.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/tracing.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/tracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/url.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/url.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/userIntegrations.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/vendor/escapeStringForRegex.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/vendor/supportsHistory.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/esm/worldwide.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry/utils/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry/utils/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/backgroundtab.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/browsertracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/metrics/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/request.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/router.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getCLS.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getFID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/getLCP.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/bindReporter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/generateUniqueID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getActivationStart.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getNavigationEntry.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/getVisibilityWatcher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/initMetric.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/observe.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/browser/web-vitals/lib/onHidden.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/extensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/apollo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/express.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/graphql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/lazy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mongo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/mysql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/postgres.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/prisma.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/cjs/node/integrations/utils/node-utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/backgroundtab.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/browsertracing.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/metrics/utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/request.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/router.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getCLS.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getFID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/getLCP.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/bindReporter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/generateUniqueID.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getActivationStart.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getNavigationEntry.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/getVisibilityWatcher.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/initMetric.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/observe.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/browser/web-vitals/lib/onHidden.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/extensions.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/apollo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/express.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/graphql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/lazy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mongo.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/mysql.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/postgres.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/prisma.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/esm/node/integrations/utils/node-utils.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/@sentry-internal/tracing/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/@sentry-internal/tracing/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/agent-base/dist/src/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/agent-base/dist/src/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/agent-base/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/agent-base/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/build/lib/boolean.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/build/lib/boolean.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/build/lib/isBooleanable.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/boolean/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/boolean/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/cookie/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/cookie/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/cookie/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/cookie/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/browser.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/browser.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/common.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/common.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/debug/src/node.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/debug/src/node.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/define-properties/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/define-properties/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/define-properties/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/detect-node/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/detect-node/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/es6/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/es6/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/lib/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/lib/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/es6-error/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/es6-error/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/escape-string-regexp/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/.jscs.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/.jscs.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/implementation.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/implementation.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/function-bind/test/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/function-bind/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/get-intrinsic/test/GetIntrinsic.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/Agent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/Agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/HttpProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/HttpsProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/classes/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/classes/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/errors.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/errors.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/createGlobalProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/createProxyController.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/factories/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/factories/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/routines/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/bindHttpMethod.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/isUrlMatchingNoProxy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/dist/utilities/parseProxyUrl.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/Agent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/Agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/HttpProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/classes/HttpsProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/factories/createGlobalProxyAgent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/factories/createProxyController.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/routines/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/types.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/types.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/bindHttpMethod.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/isUrlMatchingNoProxy.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/global-agent/src/utilities/parseProxyUrl.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/shim.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/shim.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/native.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/native.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/shimmed.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/shimmed.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/globalthis/test/tests.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/globalthis/test/tests.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-property-descriptors/test/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-property-descriptors/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/shams.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/shams.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/shams/core-js.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/shams/core-js.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/shams/get-own-property-symbols.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/has-symbols/test/tests.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/has-symbols/test/tests.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/agent.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/agent.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/dist/parse-proxy-response.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/https-proxy-agent/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/https-proxy-agent/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/stringify.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/stringify.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/json-stringify-safe/test/stringify_test.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru-cache/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru-cache/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru-cache/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/benchmark.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/benchmark.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/lru.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/lru.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/lru_map/test.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/lru_map/test.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/matcher/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/matcher/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/matcher/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/matcher/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/ms/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/ms/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/ms/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/implementation.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/implementation.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/object-keys/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createLogger.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createLogger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createMockLogger.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createNodeWriter.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/createRoarrInititialGlobalState.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/factories/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/factories/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/dist/log.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/dist/log.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/roarr/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/roarr/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/bin/semver.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/bin/semver.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/comparator.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/comparator.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/range.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/range.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/classes/semver.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/classes/semver.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/cmp.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/cmp.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/coerce.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/coerce.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/functions/diff.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/functions/diff.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/constants.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/constants.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/internal/re.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/internal/re.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/max-satisfying.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/max-satisfying.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/min-satisfying.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/min-satisfying.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/min-version.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/min-version.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/outside.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/outside.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/simplify.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/simplify.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver/ranges/subset.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver/ranges/subset.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/semver-compare/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/semver-compare/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/serialize-error/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/serialize-error/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/serialize-error/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/serialize-error/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/110.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/110.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/213.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/213.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/31.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/31.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/38.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/38.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/384.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/384.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/395.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/395.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/477.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/477.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/503.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/503.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/519.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/519.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/522.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/522.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/535.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/535.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/542.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/542.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/575.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/575.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/663.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/663.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/726.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/726.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/741.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/741.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/784.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/784.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/790.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/790.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/831.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/831.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/85.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/85.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/855.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/855.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/875.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/875.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/895.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/895.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/905.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/905.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/917.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/917.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/95.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/95.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/959.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/959.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/970.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/970.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/974.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/974.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/989.index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/989.index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/sql-wasm.wasm`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/dist/cli/thirdPartyNotice.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/distPackage.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/distPackage.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/package.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/package.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/packaging/version.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/packaging/version.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pip_resolve.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pipfile.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pipfile.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pyparsing.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pyparsing.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/parser.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/pytoml/writer.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/reqPackage.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/reqPackage.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/fragment.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/parser.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/requirements/requirement.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/setup_file.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/setup_file.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/test_pip_resolve.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/pysrc/utils.py` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/pysrc/utils.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/bootstrap.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/common.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/common.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/snyk/wrapper_dist/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/snyk/wrapper_dist/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/dist/sprintf.min.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/src/angular-sprintf.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/sprintf-js/src/sprintf.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/sprintf-js/src/sprintf.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/modules/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/modules/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/test/validateModuleExportsMatchCommonJS/index.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/tslib.es6.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/tslib.es6.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/tslib/tslib.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/tslib/tslib.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/type-fest/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/yallist/package.json` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/yallist/package.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/node_modules/yallist/yallist.js` & `c2cciutils-1.6.0.dev99/c2cciutils/node_modules/yallist/yallist.js`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/package-lock.json` & `c2cciutils-1.6.0.dev99/c2cciutils/package-lock.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/pr_checks.py` & `c2cciutils-1.6.0.dev99/c2cciutils/pr_checks.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/publish.py` & `c2cciutils-1.6.0.dev99/c2cciutils/publish.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/schema-applications.json` & `c2cciutils-1.6.0.dev99/c2cciutils/schema-applications.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/schema.json` & `c2cciutils-1.6.0.dev99/c2cciutils/schema.json`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/audit.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/audit.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/clean.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/docker_logs.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/docker_logs.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/docker_versions_gen.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/docker_versions_gen.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/download_applications.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/download_applications.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/db.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/db.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/install.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/install.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/logs.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/logs.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/k8s/wait.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/k8s/wait.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/main.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/main.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/pin_pipenv.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/pin_pipenv.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/pr_checks.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/pr_checks.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/publish.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/publish.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/scripts/trigger_image_update.py` & `c2cciutils-1.6.0.dev99/c2cciutils/scripts/trigger_image_update.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/c2cciutils/security.py` & `c2cciutils-1.6.0.dev99/c2cciutils/security.py`

 * *Files identical despite different names*

### Comparing `c2cciutils-1.6.0.dev98/pyproject.toml` & `c2cciutils-1.6.0.dev99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cciutils"
-version = "1.6.0.dev98"
+version = "1.6.0.dev99"
 description = "Common utilities for Camptocamp CI"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["ci"]
 repository = "https://github.com/camptocamp/c2cciutils"
 license = "FreeBSD"
 packages = [{ include = "c2cciutils" }]
```

### Comparing `c2cciutils-1.6.0.dev98/setup.py` & `c2cciutils-1.6.0.dev99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5225,15 +5225,15 @@
                      'c2cciutils-pull-request-checks = '
                      'c2cciutils.scripts.pr_checks:main',
                      'c2cciutils-trigger-image-update = '
                      'c2cciutils.scripts.trigger_image_update:main']}
 
 setup_kwargs = {
     'name': 'c2cciutils',
-    'version': '1.6.0.dev98',
+    'version': '1.6.0.dev99',
     'description': 'Common utilities for Camptocamp CI',
     'long_description': '# C2C CI utils\n\nThe goals of C2C CI utils are:\n\n- Have some global checks that\'s didn\'t request any dependency related to the application:\n  this commands return 3 types of results:\n  - Print some useful information:\n    - The version of some packages\n    - The used configuration (with default and autodetect)\n    - The environment variables\n    - The GitHub event file\n  - Check that some configuration where correct:\n    - Git attributes\n    - That the timeout is present in the GitHub workflow files\n    - That the stabilization version (get from the Security.md) are used everywhere it\'s needed\n  - Snyk tests\n    - Test (never failed)\n    - Code test (never failed, disabled by default)\n    - Iac Test (never failed, disabled by default)\n    - Fix (For information only, disabled by default)\n\nEvery check can be disabled with the following config (the configuration is `ci/config.yaml`):\n\n```yaml\nchecks:\n  <check name>: false\n```\n\nIt make easier to place the following workflows:\n\n- `audit.yaml`: Audit the stabilization branches of the application against vulnerabilities in the python and node dependency\n- `auto-review.yaml`: Auto review the Renovate pull requests\n- `backport.yaml`: Trigger the backports (work with labels)\n- `clean.yaml`: Clean the Docker images related on a deleted feature branch\n- `codeql.yaml`: Run a GitHub CodeQL check\n- `main.yaml`: Main workflow especially with the c2cciutils-checks command\n- `rebuild.yaml`: Daily rebuild of the Docker images on the stabilization branches.\n\nAll the provided commands:\n\n- `c2cciutils`: some generic tools.\n- `c2cciutils-checks`: Run the checks on the code (those checks don\'t need any project dependencies).\n- `c2cciutils-audit`: Do the audit, the main difference with checks is that it can change between runs on the same code.\n- `c2cciutils-publish`: Publish the project.\n- `c2cciutils-clean`: Delete Docker images on Docker Hub after corresponding branch have been deleted.\n- `c2cciutils-google-calendar`: Tool to test the Google credentials for calendar API and refresh them if needed. See `c2cciutils-google-calendar -h` for more information.\n- `c2cciutils-k8s-install`: Install a k3d / k3s cluster, see below.\n- `c2cciutils-k8s-db`: Create a database in the k8s cluster, see below.\n- `c2cciutils-k8s-wait`: Wait that the application started correctly in the cluster, see below.\n- `c2cciutils-k8s-logs`: Display the logs of the application in the k8s cluster, see below.\n- `c2cciutils-pin-pipenv`: Display all the dependencies that\'s in the `Pipenv.lock` but not in the `Pipenv` to be able to pin them.\n- `c2cciutils-docker-logs`: Display the logs of the application in Docker (compose).\n- `c2cciutils-trigger-image-update`: Trigger the ArgoCD repository about image update on the CI (automatically done in the publishing).\n- `c2cciutils-download-applications`: Download the applications with version managed by Renovate, see below.\n- `c2cciutils-docker-versions-gen`: Generate the Docker package versions file (`ci/dpkg-versions.yaml`), see below.\n\n## New project\n\nThe content of `example-project` can be a good base for a new project.\n\n## Secrets\n\nIn the CI we need to have the following secrets::\n\n- `HAS_SECRETS` to be set to \'HAS_SECRETS\', to avoid error errors from external\n  pull requests, already set globally on Camptocamp organization.\n- `GOPASS_CI_GITHUB_TOKEN` and `CI_GPG_PRIVATE_KEY` required to initialize the gopass password store,\n  the secrets exists in the Camptocamp organization but not shared on all project, then you should add\n  your project to the shared list.\n\n## Use locally, in the projects that use c2cciutils\n\nInstall it: `python3 -m pip install --user --requirement ci/requirements.txt`\nRun the checkers: `c2cciutils-checks [--fix] [--stop] [--check CHECK]`\nDry run publish: `GITHUB_REF=... c2cciutils-publish --dry-run ...`\n\n## Configuration\n\nYou can get the current configuration with `c2cciutils --get-config`, the default configuration depends on your project.\nNote that it didn\'t contain the default defined the schema and visible in the [generated documentation](./config.md).\n\nYou can override the configuration with the file `ci/config.yaml`.\n\nAt the base of the configuration you have:\n\n- `version`: Contains some regular expressions to find the versions branches and tags, and to convert them into application versions.\n- `checks`: The checker\'s configuration, see `c2cciutils/checks.py` for more information.\n- `audit`: The audit configuration, see `c2cciutils/audit.py` for more information.\n- `publish`: The publishing configuration, see `c2cciutils/publish.py` for more information.\n\nMany actions can be disabled by setting the corresponding configuration part to `False`.\n\n## SECURITY.md\n\nThe `SECURITY.md` file should contain the security policy of the repository, especially the end of\nsupport dates.\n\nFor compatibility with `c2cciutils` it should contain an array with at least the columns\n`Version` and `Supported Until`. The `Version` column will contain the concerned version.\nThe `Supported Until` will contain the date of end of support `dd/mm/yyyy`.\nIt can also contain the following sentences:\n\n- `Unsupported`: no longer supported => no audit, no rebuild.\n- `Best effort`: the support is ended, it is still rebuilt and audited, but this can be stopped without any notice.\n- `To be defined`: not yet released or the date will be set related of another project release date (like for GeoMapFish).\n\nSee also [GitHub Documentation](https://docs.github.com/en/github/managing-security-vulnerabilities/adding-a-security-policy-to-your-repository)\n\n## IDE\n\nThe IDE should be configured as:\n\n- using `black` and `isort` without any arguments,\n- using the `editorconfig` configuration.\n\n### VScode\n\n- Recommend extensions to work well with c2cciutils:\n  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) And use EditorConfig\n  - [shell-format](https://marketplace.visualstudio.com/items?itemName=foxundermoon.shell-format) With the configuration\n    `"shellformat.flag": "-bn"`.\n  - [Better TOML](https://marketplace.visualstudio.com/items?itemName=bodil.prettier-toml)\n- Other recommend extensions:\n  - [hadolint](https://marketplace.visualstudio.com/items?itemName=exiasr.hadolint)\n  - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)\n\nSelect a formatter:\n\n- `CTRL+MAJ+P`\n- Format document With...\n- Configure Default Formatter...\n- Select the formatter\n\n## Publishing\n\n### To pypi\n\nThe config is like this:\n\n```yaml\nversions:\n  # List of kinds of versions you want to publish, that can be:\n  # rebuild (specified with --type),\n  # version_tag, version_branch, feature_branch, feature_tag (for pull request)\n```\n\nIt we have a `setup.py` file, we will be in legacy mode:\nWhen publishing, the version computed from arguments or `GITHUB_REF` is put in environment variable `VERSION`, thus you should use it in `setup.py`, example:\n\n```python\nVERSION = os.environ.get("VERSION", "1.0.0")\n```\n\nAlso we consider that we use `poetry` with [poetry-dynamic-versioning](https://pypi.org/project/poetry-dynamic-versioning/) to manage the version, and [poetry-plugin-tweak-dependencies-version](https://pypi.org/project/poetry-plugin-tweak-dependencies-version/) to manage the dependencies versions.\n\nExample of configuration:\n\n```toml\n[tool.poetry-dynamic-versioning]\nenable = true\nvcs = "git"\npattern = "^(?P<base>\\\\d+(\\\\.\\\\d+)*)"\nformat-jinja = """\n{%- if env.get("VERSION_TYPE") == "version_branch" -%}\n{{serialize_pep440(bump_version(base, 1 if env.get("IS_MASTER") == "TRUE" else 2), dev=distance)}}\n{%- elif distance == 0 -%}\n{{serialize_pep440(base)}}\n{%- else -%}\n{{serialize_pep440(bump_version(base), dev=distance)}}\n{%- endif -%}\n"""\n\n```\n\nNote that we can access to the environment variables `VERSION`,`VERSION_TYPE` and `IS_MASTER`.\n\nThen by default:\n\n- Tag with `1.2.3` => release `1.2.3`\n- Commit on feature branch just do a validation\n- Commit on `master` branch after the tag 1.3.0 => release `1.4.0.dev1`\n- Commit on `1.3` branch after the tag 1.3.0 => release `1.3.1.dev1`\n\nTo make it working in the `Dockerfile` you should have in the `poetry` stage:\n\n```Dockerfile\nENV POETRY_DYNAMIC_VERSIONING_BYPASS=dev\nRUN poetry export --extras=checks --extras=publish --extras=audit --output=requirements.txt \\\n    && poetry export --with=dev --output=requirements-dev.txt\n```\n\nAnd in the `run` stage\n\n```Dockerfile\nARG VERSION=dev\nRUN --mount=type=cache,target=/root/.cache \\\n    POETRY_DYNAMIC_VERSIONING_BYPASS=${VERSION} python3 -m pip install --disable-pip-version-check --no-deps --editable=.\n```\n\nAnd in the `Makefile`:\n\n```Makefile\nVERSION = $(strip $(shell poetry version --short))\n\n.PHONY: build\nbuild: ## Build the Docker images\n    docker build --build-arg=VERSION=$(VERSION) --tag=$(GITHUB_REPOSITORY) .\n```\n\n### To Docker registry\n\nThe config is like this:\n\n```yaml\nlatest: True\nimages:\n  - name: # The base name of the image we want to publish\nrepository:\n  <internal_name>:\n    \'server\': # The fqdn name of the server if not Docker hub\n    \'version\':# List of kinds of versions you want to publish, that can be: rebuild (specified using --type),\n      # version_tag, version_branch, feature_branch, feature_tag (for pull request)\n    \'tags\':# List of tags we want to publish interpreted with `template(version=version)`\n      # e.g. if you use `{version}-lite` when you publish the version `1.2.3` the source tag\n      # (that should be built by the application build) is `latest-lite`, and it will be published\n      # with the tag `1.2.3-lite`.\n    \'group\':# If your images are published by different jobs you can separate them in different groups\n      # and publish them with `c2cciutils-publish --group=<group>`\n```\n\nBy default, the last line of the `SECURITY.md` file will be published (`docker`) with the tag\n`latest`. Set `latest` to `False` to disable it.\n\nWith the `c2cciutils-clean` the images on Docker hub for `feature_branch` will be removed on branch removing.\n\n## Download applications\n\nIn case some executables or applications from GitHub releases or any other URLs are required on the CI host\nand are not handled by any dependency manager, we provide a set of tools to install them and manage upgrades\nthrough Renovate.\n\nCreate an application file (e.-g. `applications.yaml`) with:\n\n```yaml\n# yaml-language-server: $schema=https://raw.githubusercontent.com/camptocamp/c2cciutils/master/c2cciutils/schema-applications.json\n\n# Application from GitHub release\n<organization>/<project>:\n  get-file-name: <file name present in the release>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: # The command you want to run after the file is downloaded\n    - - chmod # To be executable (usually required)\n      - +x\n      - <to-file-name>\n    - - <to-file-name> # Print the version of the application\n      - --version\n# Application from GitHub release in a tar file (or tar.gz)\n<organization>/<project>:\n  get-file-name: <file name present in the release>\n  type: tar\n  tar-file-name: <The file name available in the tar file>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: [...] # The command you want to run after the file is downloaded\n# Application from an URL\n<application reference name>:\n  url-pattern: <The URL used to download the application>\n  to-file-name: <The file name you want to create in ~/.local/bin>\n  finish-command: [...] # The command you want to run after the file is downloaded\n```\n\nIn the attributes `url-pattern`, `get-file-name` you can use the following variables:\n\n- `{version}`: The version of the application present in the version file.\n- `{version_quote}`: The URL encoded version.\n- `{short_version}`: The version without the `v` prefix.\n\nThe `applications-versions.yaml` file is a map of applications and their versions.\n\nAdd in your Renovate configuration:\n\n```json5\n\n  regexManagers: [\n    {\n      fileMatch: [\'^applications-versions.yaml$\'],\n      matchStrings: [\n        \'(?<depName>[^\\\\s]+): (?<currentValue>[^\\\\s]+) # (?<datasource>[^\\\\s]+)\',\n      ],\n    },\n  ],\n```\n\nNow you need to call `c2cciutils-download-applications --applications-file=applications.yaml --versions-file=applications-version.yaml`\nto install required applications on CI host before using them (an already installed application is installed only if needed).\n\n## Use Renovate to trigger a new build instead of the legacy rebuild\n\nRun the command `c2cciutils-docker-versions-gen camptocamp/image[:tag]` to generate a file that is a kind of package lock of the Debian packages in the file `ci/dpkg-versions.yaml`.\n\nAdd in your renovate configuration:\n\n```javascript\n  regexManagers: [\n    {\n      fileMatch: [\'^ci/dpkg-versions.yaml$\'],\n      matchStrings: [" *(?<depName>[^\'\\\\s]+): \'?(?<currentValue>[^\'\\\\s/]*[0-9][^\'\\\\s/]*)\'?"],\n      datasourceTemplate: \'repology\',\n      versioningTemplate: \'loose\',\n    },\n  ],\n```\n\nWhen a new version of a Debian package will be available:\n\n- Renovate will automatically open a pull request to update the file `ci/dpkg-versions.yaml`.\n- And the continuous integration will build a new fresh Docker image with latest versions of all Debian packages.\n\n## Kubernetes\n\nC2cciutils provide some commands for Kubernetes.\n\nYou can define a workflow like that:\n\n```yaml\n- name: Install k3s/k3d (Kubernetes cluster)\n  run: c2cciutils-k8s-install\n\n- name: Create a database to do the tests\n  run: c2cciutils-k8s-db --script=<my_script>.sql\n\n- name: Install the application in the Kubernetes cluster\n  run: kubectl apply -f <my_application>.yaml\n\n- name: Wait that the application is ready\n  run: c2cciutils-k8s-wait\n- name: Print the application status and logs\n  run: c2cciutils-k8s-logs\n  if: always()\n\n- name: Uninstall the application\n  run: kubectl delete -f <my_application>.yaml || true\n\n- name: Cleanup the database\n  run: c2cciutils-k8s-db --cleanup\n```\n\n`c2cciutils-k8s-install` can be configured in the `ci/config.yaml` file, in section `k8s/k3d/install-commands`, default is:\n\n```yaml\n- - k3d\n    cluster\n    create\n    test-cluster\n    --no-lb\n    --no-rollback\n```\n\nSee also: [K3d cluster create documentation](https://k3d.io/v4.4.8/usage/commands/k3d_cluster_create/).\n\n`c2cciutils-k8s-db` can be configured in the `ci/config.yaml` file, in section `k8s/db/chart-options`, default is:\n\n```yaml\npersistence.enabled: \'false\'\ntls.enabled: \'true\'\ntls.autoGenerated: \'true\'\npostgresqlPassword: mySuperTestingPassword\nvolumePermissions.enabled: \'true\'\n```\n\nSee also: [Parameters documentations](https://github.com/bitnami/charts/tree/master/bitnami/postgresql#parameters).\n\n## Contributing\n\nInstall the pre-commit hooks:\n\n```bash\npip install pre-commit\npre-commit install --allow-missing-config\n```\n',
     'author': 'Camptocamp',
     'author_email': 'info@camptocamp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/camptocamp/c2cciutils',
```

### Comparing `c2cciutils-1.6.0.dev98/PKG-INFO` & `c2cciutils-1.6.0.dev99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cciutils
-Version: 1.6.0.dev98
+Version: 1.6.0.dev99
 Summary: Common utilities for Camptocamp CI
 Home-page: https://github.com/camptocamp/c2cciutils
 License: FreeBSD
 Keywords: ci
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4.0
```

