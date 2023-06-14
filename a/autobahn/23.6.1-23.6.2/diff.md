# Comparing `tmp/autobahn-23.6.1.tar.gz` & `tmp/autobahn-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobahn-23.6.1.tar", last modified: Sun Jun  4 22:11:32 2023, max compression
+gzip compressed data, was "autobahn-23.6.2.tar", last modified: Wed Jun 14 07:27:09 2023, max compression
```

## Comparing `autobahn-23.6.1.tar` & `autobahn-23.6.2.tar`

### file list

```diff
@@ -1,285 +1,290 @@
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.812810 autobahn-23.6.1/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1078 2023-01-15 21:52:21.000000 autobahn-23.6.1/LICENSE
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      305 2023-01-15 14:26:58.000000 autobahn-23.6.1/MANIFEST.in
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12908 2023-06-04 22:11:32.812810 autobahn-23.6.1/PKG-INFO
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11134 2023-01-15 21:52:21.000000 autobahn-23.6.1/README.rst
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.736808 autobahn-23.6.1/autobahn/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1908 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11022 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/__main__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1336 2023-06-04 22:10:37.000000 autobahn-23.6.1/autobahn/_version.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.740808 autobahn-23.6.1/autobahn/asset/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3246 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/asset/xbr_gray.svg
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3466 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/asset/xbr_white.svg
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.740808 autobahn-23.6.1/autobahn/asyncio/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1960 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15940 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/component.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    17995 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/rawsocket.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6026 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/util.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11355 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/wamp.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11950 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/websocket.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/asyncio/xbr/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3421 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/asyncio/xbr/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1770 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/exception.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/nvx/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1373 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/nvx/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    17102 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/nvx/_utf8validator.c
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2712 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/nvx/_utf8validator.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/nvx/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/nvx/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    14273 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/nvx/test/test_nvx_utf8validator.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/rawsocket/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/rawsocket/__init__.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/rawsocket/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/rawsocket/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4929 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/rawsocket/test/test_rawsocket_url.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5648 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/rawsocket/util.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.744808 autobahn-23.6.1/autobahn/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4061 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/test/test_rng.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2668 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/test/test_util.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2402 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/testutil.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.748808 autobahn-23.6.1/autobahn/twisted/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3015 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8989 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/choosereactor.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15120 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/component.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5825 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/cryptosign.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4642 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/forwarder.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    24091 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/rawsocket.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7208 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/resource.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.752808 autobahn-23.6.1/autobahn/twisted/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5051 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_application_runner.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4706 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_choosereactor.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16852 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_component.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2164 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_endpoint_plugins.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16570 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_protocol.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2739 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_rawsocket.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2400 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_tx_websocket_agent.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3412 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/test/test_wamp_runner.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.752808 autobahn-23.6.1/autobahn/twisted/testing/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10065 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/testing/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13627 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/util.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    34578 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/wamp.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    32842 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/websocket.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.752808 autobahn-23.6.1/autobahn/twisted/xbr/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3924 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/twisted/xbr/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    32789 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/util.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.760808 autobahn-23.6.1/autobahn/wamp/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2264 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    22913 2023-06-04 22:10:37.000000 autobahn-23.6.1/autobahn/wamp/auth.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    38364 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/component.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10518 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/cryptobox.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    39393 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/cryptosign.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10445 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/exception.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.760808 autobahn-23.6.1/autobahn/wamp/gen/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/__init__.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.760808 autobahn-23.6.1/autobahn/wamp/gen/schema/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12664 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/auth.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8760 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/pubsub.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8168 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/roles.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9456 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/rpc.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16112 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/session.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3600 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/types.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    28648 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/schema/wamp.bfbs
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.764809 autobahn-23.6.1/autobahn/wamp/gen/wamp/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1664 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/Map.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      878 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/Void.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/__init__.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.784809 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2134 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Abort.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      576 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AnyMessage.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2778 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraChallenge.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      959 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraRequest.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      959 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraWelcome.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1540 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignChallenge.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1985 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignRequest.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1015 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignWelcome.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      233 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthFactor.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      221 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthMethod.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      148 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthMode.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3682 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramChallenge.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1907 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramRequest.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1443 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramWelcome.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      999 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketChallenge.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      983 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketRequest.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      983 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketWelcome.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2385 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Authenticate.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8611 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/BrokerFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9460 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Call.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6267 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/CalleeFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4118 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/CallerFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3293 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Cancel.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      156 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/CancelMode.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2282 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Challenge.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      152 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/ChannelBinding.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3413 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/ClientRoles.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7799 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/DealerFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6004 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Error.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12820 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Event.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5475 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/EventReceived.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2598 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Goodbye.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6397 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Hello.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7663 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/HelloNew.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3797 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Interrupt.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10302 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Invocation.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      198 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/InvocationPolicy.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      152 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Kdf.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      157 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Match.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1801 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Message.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      580 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/MessageType.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      160 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Payload.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      673 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Principal.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    18774 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Publish.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2190 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Published.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4404 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/PublisherFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3901 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Register.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Registered.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8179 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Result.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2135 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/RouterRoles.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      246 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Serializer.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3016 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Subscribe.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Subscribed.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5532 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/SubscriberFeatures.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6776 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/SubscriberReceived.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unregister.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2690 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unregistered.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2232 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unsubscribe.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2690 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unsubscribed.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5956 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Welcome.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8124 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Yield.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    39242 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/interfaces.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)   213842 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/message.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4598 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/message_fbs.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    92340 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/protocol.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9645 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/request.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10917 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/role.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    36486 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/serializer.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.788809 autobahn-23.6.1/autobahn/wamp/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/wamp/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9849 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_auth.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7558 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_component.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6144 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_component_aio.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1541 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_cryptobox.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12970 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_cryptosign.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2130 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_exception.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3587 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_identifiers.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    48032 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_message.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    41896 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_protocol.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4289 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_protocol_peer.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2766 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_scram.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    23164 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_serializer.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3305 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_session_details.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5950 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_transport_details.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    24907 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_uri_pattern.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16218 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_user_handler_errors.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1730 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/test/test_wamp_websocket.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    85598 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/types.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13713 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/uri.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12907 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/wamp/websocket.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.792809 autobahn-23.6.1/autobahn/websocket/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1698 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4553 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/compress.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2133 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/compress_base.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    18315 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/compress_bzip2.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    29874 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/compress_deflate.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16926 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/compress_snappy.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    31338 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/interfaces.py
--rwxrwxr-x   0 oberstet  (1000) oberstet  (1000)   168445 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/protocol.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.792809 autobahn-23.6.1/autobahn/websocket/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/test/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13930 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/test/test_websocket_frame.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10010 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/test/test_websocket_protocol.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5402 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/test/test_websocket_url.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    14109 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/types.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6627 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/utf8validator.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6409 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/util.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3978 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/websocket/xormasker.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.800809 autobahn-23.6.1/autobahn/xbr/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16211 2023-02-08 01:22:33.000000 autobahn-23.6.1/autobahn/xbr/__init__.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6311 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_abi.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7325 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_blockchain.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    27913 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_buyer.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    52522 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_cli.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    20411 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_config.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3225 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_dialog.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5189 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_api_publish.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19320 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_authority_certificate.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5092 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_base.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4729 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_catalog_create.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1699 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_certificate.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5584 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_certificate_chain.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4945 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_channel_close.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5754 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_channel_open.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5895 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_consent.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16018 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_delegate_certificate.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5408 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_domain_create.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5904 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_market_create.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4827 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_market_join.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4548 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_market_leave.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2902 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_market_member_login.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5045 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_member_login.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4625 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_member_register.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4047 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_member_unregister.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5743 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_eip712_node_pair.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15693 2023-02-08 01:22:33.000000 autobahn-23.6.1/autobahn/xbr/_frealm.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    40135 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_gui.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4473 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_interfaces.py
--rwxrwxr-x   0 oberstet  (1000) oberstet  (1000)     6210 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/_mnemonic.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    76435 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_schema.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    21428 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_secmod.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    33548 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_seller.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9889 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_userkey.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5977 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_util.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3784 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/_wallet.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.732808 autobahn-23.6.1/autobahn/xbr/templates/
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.804809 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      330 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/enum.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      113 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/module.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16768 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/obj.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9896 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/service.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      265 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/test_enum.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       37 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/test_module.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8057 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/test_obj.py.jinja2
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       38 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/test_service.py.jinja2
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.804809 autobahn-23.6.1/autobahn/xbr/templates/sol-eip712/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19100 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/templates/sol-eip712/obj-eip712.sol.jinja2
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.808810 autobahn-23.6.1/autobahn/xbr/test/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/test/__init__.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.732808 autobahn-23.6.1/autobahn/xbr/test/catalog/
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.808810 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    21392 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/demo.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13416 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/testsvc1.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9048 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-auth.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16380 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-control.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19792 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-meta.bfbs
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6844 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp.bfbs
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.812810 autobahn-23.6.1/autobahn/xbr/test/profile/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       78 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/profile/config.ini
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      457 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/profile/default.priv
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      270 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/profile/default.pub
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2969 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_argon2.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2905 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_config.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    29577 2023-02-08 01:22:33.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_eip712.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7549 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_frealm.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5163 2023-02-08 01:22:33.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_mnemonic.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3530 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_demo.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13904 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_wamp.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8393 2023-01-15 14:26:58.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_wamp_control.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19066 2023-01-15 21:52:21.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_secmod.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1840 2023-02-08 01:22:33.000000 autobahn-23.6.1/autobahn/xbr/test/test_xbr_web3.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.740808 autobahn-23.6.1/autobahn.egg-info/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12908 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/PKG-INFO
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9209 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/SOURCES.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        1 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/dependency_links.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      127 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/entry_points.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        1 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/not-zip-safe
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2415 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/requires.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       17 2023-06-04 22:11:32.000000 autobahn-23.6.1/autobahn.egg-info/top_level.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      787 2023-01-15 21:52:21.000000 autobahn-23.6.1/requirements-dev.txt
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      229 2023-06-04 22:11:32.812810 autobahn-23.6.1/setup.cfg
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13201 2023-06-04 22:10:37.000000 autobahn-23.6.1/setup.py
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.736808 autobahn-23.6.1/twisted/
-drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-04 22:11:32.812810 autobahn-23.6.1/twisted/plugins/
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6336 2023-01-15 21:52:21.000000 autobahn-23.6.1/twisted/plugins/autobahn_endpoints.py
--rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1553 2023-01-15 21:52:21.000000 autobahn-23.6.1/twisted/plugins/autobahn_twistd.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.329488 autobahn-23.6.2/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1078 2023-01-15 21:52:21.000000 autobahn-23.6.2/LICENSE
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      305 2023-01-15 14:26:58.000000 autobahn-23.6.2/MANIFEST.in
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12906 2023-06-14 07:27:09.329488 autobahn-23.6.2/PKG-INFO
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11134 2023-01-15 21:52:21.000000 autobahn-23.6.2/README.rst
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.257487 autobahn-23.6.2/autobahn/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1908 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11022 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/__main__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1336 2023-06-14 07:26:19.000000 autobahn-23.6.2/autobahn/_version.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.261487 autobahn-23.6.2/autobahn/asset/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3246 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/asset/xbr_gray.svg
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3466 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/asset/xbr_white.svg
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.265487 autobahn-23.6.2/autobahn/asyncio/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1960 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15940 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/component.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    17995 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/rawsocket.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.265487 autobahn-23.6.2/autobahn/asyncio/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      951 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/asyncio/test/README_NO_INIT_PY
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7801 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/asyncio/test/test_aio_rawsocket.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1960 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/asyncio/test/test_aio_websocket.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6228 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/test/test_wamp_runner.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6026 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/util.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11355 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/wamp.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    11950 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/websocket.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.265487 autobahn-23.6.2/autobahn/asyncio/xbr/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3421 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/asyncio/xbr/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1770 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/exception.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.265487 autobahn-23.6.2/autobahn/nvx/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1373 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/nvx/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    17102 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/nvx/_utf8validator.c
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2712 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/nvx/_utf8validator.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.269487 autobahn-23.6.2/autobahn/nvx/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/nvx/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    14273 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/nvx/test/test_nvx_utf8validator.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.269487 autobahn-23.6.2/autobahn/rawsocket/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/rawsocket/__init__.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.269487 autobahn-23.6.2/autobahn/rawsocket/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/rawsocket/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4929 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/rawsocket/test/test_rawsocket_url.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5648 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/rawsocket/util.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.269487 autobahn-23.6.2/autobahn/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4061 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/test/test_rng.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2668 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/test/test_util.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2402 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/testutil.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.273487 autobahn-23.6.2/autobahn/twisted/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3015 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8989 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/choosereactor.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15120 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/component.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5825 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/cryptosign.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4642 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/forwarder.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    24091 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/rawsocket.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7208 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/resource.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.277487 autobahn-23.6.2/autobahn/twisted/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5051 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_application_runner.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4706 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_choosereactor.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16852 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_component.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2164 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_endpoint_plugins.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16570 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_protocol.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2739 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_rawsocket.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2400 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_tx_websocket_agent.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3412 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/test/test_wamp_runner.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.277487 autobahn-23.6.2/autobahn/twisted/testing/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10065 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/testing/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13627 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/util.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    34578 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/wamp.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    32842 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/websocket.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.277487 autobahn-23.6.2/autobahn/twisted/xbr/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3924 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/twisted/xbr/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    32789 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/util.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.281487 autobahn-23.6.2/autobahn/wamp/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2264 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    22913 2023-06-04 22:10:37.000000 autobahn-23.6.2/autobahn/wamp/auth.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    38364 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/component.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10518 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/cryptobox.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    39393 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/cryptosign.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10445 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/exception.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.281487 autobahn-23.6.2/autobahn/wamp/gen/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/__init__.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.281487 autobahn-23.6.2/autobahn/wamp/gen/schema/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12664 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/auth.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8760 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/pubsub.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8168 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/roles.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9456 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/rpc.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16112 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/session.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3600 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/types.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    28648 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/schema/wamp.bfbs
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.281487 autobahn-23.6.2/autobahn/wamp/gen/wamp/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1664 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/Map.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      878 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/Void.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/__init__.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.301488 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2134 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Abort.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      576 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AnyMessage.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2778 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraChallenge.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      959 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraRequest.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      959 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraWelcome.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1540 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignChallenge.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1985 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignRequest.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1015 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignWelcome.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      233 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthFactor.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      221 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthMethod.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      148 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthMode.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3682 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramChallenge.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1907 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramRequest.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1443 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramWelcome.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      999 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketChallenge.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      983 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketRequest.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      983 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketWelcome.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2385 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Authenticate.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8611 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/BrokerFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9460 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Call.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6267 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/CalleeFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4118 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/CallerFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3293 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Cancel.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      156 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/CancelMode.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2282 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Challenge.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      152 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/ChannelBinding.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3413 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/ClientRoles.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7799 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/DealerFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6004 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Error.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12820 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Event.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5475 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/EventReceived.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2598 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Goodbye.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6397 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Hello.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7663 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/HelloNew.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3797 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Interrupt.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10302 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Invocation.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      198 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/InvocationPolicy.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      152 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Kdf.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      157 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Match.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1801 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Message.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      580 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/MessageType.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      160 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Payload.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      673 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Principal.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    18774 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Publish.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2190 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Published.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4404 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/PublisherFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3901 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Register.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Registered.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8179 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Result.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2135 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/RouterRoles.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      246 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Serializer.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3016 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Subscribe.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Subscribed.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5532 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/SubscriberFeatures.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6776 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/SubscriberReceived.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2215 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unregister.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2690 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unregistered.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2232 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unsubscribe.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2690 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unsubscribed.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5956 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Welcome.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8124 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Yield.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    39242 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/interfaces.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)   213842 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/message.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4598 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/message_fbs.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    92340 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/protocol.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9645 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/request.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10917 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/role.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    36486 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/serializer.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.305487 autobahn-23.6.2/autobahn/wamp/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        0 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/wamp/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9849 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_auth.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7558 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_component.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6144 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_component_aio.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1541 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_cryptobox.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12970 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_cryptosign.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2130 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_exception.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3587 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_identifiers.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    48032 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_message.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    41896 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_protocol.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4289 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_protocol_peer.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2766 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_scram.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    23164 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_serializer.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3305 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_session_details.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5950 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_transport_details.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    24907 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_uri_pattern.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16218 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_user_handler_errors.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1730 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/test/test_wamp_websocket.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    85598 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/types.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13713 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/uri.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12907 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/wamp/websocket.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.309488 autobahn-23.6.2/autobahn/websocket/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1698 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4553 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/compress.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2133 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/compress_base.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    18315 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/compress_bzip2.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    29874 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/compress_deflate.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16926 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/compress_snappy.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    31338 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/interfaces.py
+-rwxrwxr-x   0 oberstet  (1000) oberstet  (1000)   168445 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/protocol.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.309488 autobahn-23.6.2/autobahn/websocket/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/test/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13930 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/test/test_websocket_frame.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    10010 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/test/test_websocket_protocol.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5402 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/test/test_websocket_url.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    14109 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/types.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6627 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/utf8validator.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6409 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/util.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3978 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/websocket/xormasker.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.317488 autobahn-23.6.2/autobahn/xbr/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16211 2023-02-08 01:22:33.000000 autobahn-23.6.2/autobahn/xbr/__init__.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6311 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_abi.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7325 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_blockchain.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    27913 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_buyer.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    52522 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_cli.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    20411 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_config.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3225 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_dialog.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5189 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_api_publish.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19320 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_authority_certificate.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5092 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_base.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4729 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_catalog_create.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1699 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_certificate.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5584 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_certificate_chain.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4945 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_channel_close.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5754 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_channel_open.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5895 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_consent.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16018 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_delegate_certificate.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5408 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_domain_create.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5904 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_market_create.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4827 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_market_join.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4548 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_market_leave.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2902 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_market_member_login.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5045 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_member_login.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4625 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_member_register.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4047 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_member_unregister.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5743 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_eip712_node_pair.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    15693 2023-02-08 01:22:33.000000 autobahn-23.6.2/autobahn/xbr/_frealm.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    40135 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_gui.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     4473 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_interfaces.py
+-rwxrwxr-x   0 oberstet  (1000) oberstet  (1000)     6210 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/_mnemonic.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    76435 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_schema.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    21428 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_secmod.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    33548 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_seller.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9889 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_userkey.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5977 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_util.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3784 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/_wallet.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.253487 autobahn-23.6.2/autobahn/xbr/templates/
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.321488 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      330 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/enum.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      113 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/module.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16768 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/obj.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9896 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/service.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      265 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/test_enum.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       37 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/test_module.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8057 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/test_obj.py.jinja2
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       38 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/test_service.py.jinja2
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.321488 autobahn-23.6.2/autobahn/xbr/templates/sol-eip712/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19100 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/templates/sol-eip712/obj-eip712.sol.jinja2
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.325488 autobahn-23.6.2/autobahn/xbr/test/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1280 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/test/__init__.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.253487 autobahn-23.6.2/autobahn/xbr/test/catalog/
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.329488 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    21392 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/demo.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13416 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/testsvc1.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9048 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-auth.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    16380 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-control.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19792 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-meta.bfbs
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6844 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp.bfbs
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.329488 autobahn-23.6.2/autobahn/xbr/test/profile/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       78 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/profile/config.ini
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      457 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/profile/default.priv
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      270 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/profile/default.pub
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2969 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_argon2.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     2905 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_config.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    29577 2023-02-08 01:22:33.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_eip712.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     7549 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_frealm.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     5163 2023-02-08 01:22:33.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_mnemonic.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     3530 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_demo.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13904 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_wamp.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     8393 2023-01-15 14:26:58.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_wamp_control.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    19066 2023-01-15 21:52:21.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_secmod.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1840 2023-02-08 01:22:33.000000 autobahn-23.6.2/autobahn/xbr/test/test_xbr_web3.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.261487 autobahn-23.6.2/autobahn.egg-info/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    12906 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/PKG-INFO
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     9379 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/SOURCES.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        1 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/dependency_links.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      126 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/entry_points.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)        1 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/not-zip-safe
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1918 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/requires.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)       17 2023-06-14 07:27:09.000000 autobahn-23.6.2/autobahn.egg-info/top_level.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      787 2023-01-15 21:52:21.000000 autobahn-23.6.2/requirements-dev.txt
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)      229 2023-06-14 07:27:09.329488 autobahn-23.6.2/setup.cfg
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)    13201 2023-06-14 07:26:19.000000 autobahn-23.6.2/setup.py
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.253487 autobahn-23.6.2/twisted/
+drwxrwxr-x   0 oberstet  (1000) oberstet  (1000)        0 2023-06-14 07:27:09.329488 autobahn-23.6.2/twisted/plugins/
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     6336 2023-01-15 21:52:21.000000 autobahn-23.6.2/twisted/plugins/autobahn_endpoints.py
+-rw-rw-r--   0 oberstet  (1000) oberstet  (1000)     1553 2023-01-15 21:52:21.000000 autobahn-23.6.2/twisted/plugins/autobahn_twistd.py
```

### Comparing `autobahn-23.6.1/LICENSE` & `autobahn-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/PKG-INFO` & `autobahn-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobahn
-Version: 23.6.1
+Version: 23.6.2
 Summary: WebSocket client & server library, WAMP real-time framework
 Home-page: https://github.com/crossbario/autobahn-python
 Author: typedef int GmbH
 License: MIT License
 Project-URL: Source, https://github.com/crossbario/autobahn-python
 Keywords: autobahn crossbar websocket realtime rfc6455 wamp rpc pubsub twisted asyncio xbr data-markets blockchain ethereum
 Platform: Any
@@ -318,9 +318,7 @@
    :target: https://autobahn.readthedocs.io/en/latest/
 
 .. |Docker Images| image:: https://img.shields.io/badge/download-docker-blue.svg?style=flat
    :target: https://hub.docker.com/r/crossbario/autobahn-python/
 
 .. |EXE Download| image:: https://img.shields.io/badge/download-exe-blue.svg?style=flat
    :target: https://download.crossbario.com/xbrnetwork/linux-amd64/xbrnetwork-latest
-
-
```

### Comparing `autobahn-23.6.1/README.rst` & `autobahn-23.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/__init__.py` & `autobahn-23.6.2/autobahn/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/__main__.py` & `autobahn-23.6.2/autobahn/__main__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/_version.py` & `autobahn-23.6.2/autobahn/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 ###############################################################################
 
-__version__ = '23.6.1'
+__version__ = '23.6.2'
 
 __build__ = '00000000-0000000'
```

### Comparing `autobahn-23.6.1/autobahn/asset/xbr_gray.svg` & `autobahn-23.6.2/autobahn/asset/xbr_gray.svg`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asset/xbr_white.svg` & `autobahn-23.6.2/autobahn/asset/xbr_white.svg`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/__init__.py` & `autobahn-23.6.2/autobahn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/component.py` & `autobahn-23.6.2/autobahn/asyncio/component.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/rawsocket.py` & `autobahn-23.6.2/autobahn/asyncio/rawsocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/util.py` & `autobahn-23.6.2/autobahn/asyncio/util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/wamp.py` & `autobahn-23.6.2/autobahn/asyncio/wamp.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/websocket.py` & `autobahn-23.6.2/autobahn/asyncio/websocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/asyncio/xbr/__init__.py` & `autobahn-23.6.2/autobahn/asyncio/xbr/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/exception.py` & `autobahn-23.6.2/autobahn/exception.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/nvx/__init__.py` & `autobahn-23.6.2/autobahn/nvx/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/nvx/_utf8validator.c` & `autobahn-23.6.2/autobahn/nvx/_utf8validator.c`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/nvx/_utf8validator.py` & `autobahn-23.6.2/autobahn/nvx/_utf8validator.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/nvx/test/__init__.py` & `autobahn-23.6.2/autobahn/nvx/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/nvx/test/test_nvx_utf8validator.py` & `autobahn-23.6.2/autobahn/nvx/test/test_nvx_utf8validator.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/rawsocket/__init__.py` & `autobahn-23.6.2/autobahn/rawsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/rawsocket/test/__init__.py` & `autobahn-23.6.2/autobahn/rawsocket/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/rawsocket/test/test_rawsocket_url.py` & `autobahn-23.6.2/autobahn/rawsocket/test/test_rawsocket_url.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/rawsocket/util.py` & `autobahn-23.6.2/autobahn/rawsocket/util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/test/__init__.py` & `autobahn-23.6.2/autobahn/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/test/test_rng.py` & `autobahn-23.6.2/autobahn/test/test_rng.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/test/test_util.py` & `autobahn-23.6.2/autobahn/test/test_util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/testutil.py` & `autobahn-23.6.2/autobahn/testutil.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/__init__.py` & `autobahn-23.6.2/autobahn/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/choosereactor.py` & `autobahn-23.6.2/autobahn/twisted/choosereactor.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/component.py` & `autobahn-23.6.2/autobahn/twisted/component.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/cryptosign.py` & `autobahn-23.6.2/autobahn/twisted/cryptosign.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/forwarder.py` & `autobahn-23.6.2/autobahn/twisted/forwarder.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/rawsocket.py` & `autobahn-23.6.2/autobahn/twisted/rawsocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/resource.py` & `autobahn-23.6.2/autobahn/twisted/resource.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/__init__.py` & `autobahn-23.6.2/autobahn/twisted/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_application_runner.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_application_runner.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_choosereactor.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_choosereactor.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_component.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_component.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_endpoint_plugins.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_endpoint_plugins.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_protocol.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_protocol.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_rawsocket.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_rawsocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_tx_websocket_agent.py` & `autobahn-23.6.2/autobahn/twisted/test/test_tx_websocket_agent.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/test/test_wamp_runner.py` & `autobahn-23.6.2/autobahn/twisted/test/test_wamp_runner.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/testing/__init__.py` & `autobahn-23.6.2/autobahn/twisted/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/util.py` & `autobahn-23.6.2/autobahn/twisted/util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/wamp.py` & `autobahn-23.6.2/autobahn/twisted/wamp.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/websocket.py` & `autobahn-23.6.2/autobahn/twisted/websocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/twisted/xbr/__init__.py` & `autobahn-23.6.2/autobahn/twisted/xbr/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/util.py` & `autobahn-23.6.2/autobahn/util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/__init__.py` & `autobahn-23.6.2/autobahn/wamp/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/auth.py` & `autobahn-23.6.2/autobahn/wamp/auth.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/component.py` & `autobahn-23.6.2/autobahn/wamp/component.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/cryptobox.py` & `autobahn-23.6.2/autobahn/wamp/cryptobox.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/cryptosign.py` & `autobahn-23.6.2/autobahn/wamp/cryptosign.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/exception.py` & `autobahn-23.6.2/autobahn/wamp/exception.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/auth.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/auth.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/pubsub.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/pubsub.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/roles.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/roles.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/rpc.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/rpc.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/session.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/session.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/types.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/types.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/schema/wamp.bfbs` & `autobahn-23.6.2/autobahn/wamp/gen/schema/wamp.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/Map.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/Map.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/Void.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/Void.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Abort.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Abort.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AnyMessage.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AnyMessage.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraChallenge.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraChallenge.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraRequest.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraRequest.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCraWelcome.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCraWelcome.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignChallenge.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignChallenge.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignRequest.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignRequest.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthCryptosignWelcome.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthCryptosignWelcome.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramChallenge.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramChallenge.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramRequest.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramRequest.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthScramWelcome.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthScramWelcome.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketChallenge.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketChallenge.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketRequest.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketRequest.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/AuthTicketWelcome.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/AuthTicketWelcome.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Authenticate.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Authenticate.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/BrokerFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/BrokerFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Call.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Call.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/CalleeFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/CalleeFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/CallerFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/CallerFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Cancel.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Cancel.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Challenge.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Challenge.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/ClientRoles.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/ClientRoles.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/DealerFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/DealerFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Error.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Error.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Event.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Event.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/EventReceived.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/EventReceived.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Goodbye.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Goodbye.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Hello.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Hello.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/HelloNew.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/HelloNew.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Interrupt.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Interrupt.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Invocation.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Invocation.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Message.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Message.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/MessageType.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/MessageType.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Principal.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Principal.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Publish.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Publish.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Published.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Published.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/PublisherFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/PublisherFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Register.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Register.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Registered.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Registered.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Result.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Result.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/RouterRoles.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/RouterRoles.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Subscribe.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Subscribe.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Subscribed.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Subscribed.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/SubscriberFeatures.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/SubscriberFeatures.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/SubscriberReceived.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/SubscriberReceived.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unregister.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unregister.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unregistered.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unregistered.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unsubscribe.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unsubscribe.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Unsubscribed.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Unsubscribed.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Welcome.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Welcome.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/gen/wamp/proto/Yield.py` & `autobahn-23.6.2/autobahn/wamp/gen/wamp/proto/Yield.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/interfaces.py` & `autobahn-23.6.2/autobahn/wamp/interfaces.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/message.py` & `autobahn-23.6.2/autobahn/wamp/message.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/message_fbs.py` & `autobahn-23.6.2/autobahn/wamp/message_fbs.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/protocol.py` & `autobahn-23.6.2/autobahn/wamp/protocol.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/request.py` & `autobahn-23.6.2/autobahn/wamp/request.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/role.py` & `autobahn-23.6.2/autobahn/wamp/role.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/serializer.py` & `autobahn-23.6.2/autobahn/wamp/serializer.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_auth.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_auth.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_component.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_component.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_component_aio.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_component_aio.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_cryptobox.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_cryptobox.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_cryptosign.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_cryptosign.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_exception.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_exception.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_identifiers.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_identifiers.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_message.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_message.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_protocol.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_protocol.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_protocol_peer.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_protocol_peer.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_scram.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_scram.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_serializer.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_serializer.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_session_details.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_session_details.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_transport_details.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_transport_details.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_uri_pattern.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_uri_pattern.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_user_handler_errors.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_user_handler_errors.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/test/test_wamp_websocket.py` & `autobahn-23.6.2/autobahn/wamp/test/test_wamp_websocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/types.py` & `autobahn-23.6.2/autobahn/wamp/types.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/uri.py` & `autobahn-23.6.2/autobahn/wamp/uri.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/wamp/websocket.py` & `autobahn-23.6.2/autobahn/wamp/websocket.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/__init__.py` & `autobahn-23.6.2/autobahn/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/compress.py` & `autobahn-23.6.2/autobahn/websocket/compress.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/compress_base.py` & `autobahn-23.6.2/autobahn/websocket/compress_base.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/compress_bzip2.py` & `autobahn-23.6.2/autobahn/websocket/compress_bzip2.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/compress_deflate.py` & `autobahn-23.6.2/autobahn/websocket/compress_deflate.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/compress_snappy.py` & `autobahn-23.6.2/autobahn/websocket/compress_snappy.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/interfaces.py` & `autobahn-23.6.2/autobahn/websocket/interfaces.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/protocol.py` & `autobahn-23.6.2/autobahn/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/test/__init__.py` & `autobahn-23.6.2/autobahn/websocket/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/test/test_websocket_frame.py` & `autobahn-23.6.2/autobahn/websocket/test/test_websocket_frame.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/test/test_websocket_protocol.py` & `autobahn-23.6.2/autobahn/websocket/test/test_websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/test/test_websocket_url.py` & `autobahn-23.6.2/autobahn/websocket/test/test_websocket_url.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/types.py` & `autobahn-23.6.2/autobahn/websocket/types.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/utf8validator.py` & `autobahn-23.6.2/autobahn/websocket/utf8validator.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/util.py` & `autobahn-23.6.2/autobahn/websocket/util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/websocket/xormasker.py` & `autobahn-23.6.2/autobahn/websocket/xormasker.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/__init__.py` & `autobahn-23.6.2/autobahn/xbr/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_abi.py` & `autobahn-23.6.2/autobahn/xbr/_abi.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_blockchain.py` & `autobahn-23.6.2/autobahn/xbr/_blockchain.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_buyer.py` & `autobahn-23.6.2/autobahn/xbr/_buyer.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_cli.py` & `autobahn-23.6.2/autobahn/xbr/_cli.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_config.py` & `autobahn-23.6.2/autobahn/xbr/_config.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_dialog.py` & `autobahn-23.6.2/autobahn/xbr/_dialog.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_api_publish.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_api_publish.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_authority_certificate.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_authority_certificate.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_base.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_base.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_catalog_create.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_catalog_create.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_certificate.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_certificate.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_certificate_chain.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_certificate_chain.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_channel_close.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_channel_close.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_channel_open.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_channel_open.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_consent.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_consent.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_delegate_certificate.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_delegate_certificate.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_domain_create.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_domain_create.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_market_create.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_market_create.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_market_join.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_market_join.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_market_leave.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_market_leave.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_market_member_login.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_market_member_login.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_member_login.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_member_login.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_member_register.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_member_register.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_member_unregister.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_member_unregister.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_eip712_node_pair.py` & `autobahn-23.6.2/autobahn/xbr/_eip712_node_pair.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_frealm.py` & `autobahn-23.6.2/autobahn/xbr/_frealm.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_gui.py` & `autobahn-23.6.2/autobahn/xbr/_gui.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_interfaces.py` & `autobahn-23.6.2/autobahn/xbr/_interfaces.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_mnemonic.py` & `autobahn-23.6.2/autobahn/xbr/_mnemonic.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_schema.py` & `autobahn-23.6.2/autobahn/xbr/_schema.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_secmod.py` & `autobahn-23.6.2/autobahn/xbr/_secmod.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_seller.py` & `autobahn-23.6.2/autobahn/xbr/_seller.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_userkey.py` & `autobahn-23.6.2/autobahn/xbr/_userkey.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_util.py` & `autobahn-23.6.2/autobahn/xbr/_util.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/_wallet.py` & `autobahn-23.6.2/autobahn/xbr/_wallet.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/obj.py.jinja2` & `autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/obj.py.jinja2`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/service.py.jinja2` & `autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/service.py.jinja2`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/templates/py-autobahn/test_obj.py.jinja2` & `autobahn-23.6.2/autobahn/xbr/templates/py-autobahn/test_obj.py.jinja2`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/templates/sol-eip712/obj-eip712.sol.jinja2` & `autobahn-23.6.2/autobahn/xbr/templates/sol-eip712/obj-eip712.sol.jinja2`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/__init__.py` & `autobahn-23.6.2/autobahn/xbr/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/demo.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/demo.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/testsvc1.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/testsvc1.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-auth.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-auth.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-control.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-control.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp-meta.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp-meta.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/catalog/schema/wamp.bfbs` & `autobahn-23.6.2/autobahn/xbr/test/catalog/schema/wamp.bfbs`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_argon2.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_argon2.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_config.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_config.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_eip712.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_eip712.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_frealm.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_frealm.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_mnemonic.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_mnemonic.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_demo.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_demo.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_wamp.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_wamp.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_schema_wamp_control.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_schema_wamp_control.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_secmod.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_secmod.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn/xbr/test/test_xbr_web3.py` & `autobahn-23.6.2/autobahn/xbr/test/test_xbr_web3.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/autobahn.egg-info/PKG-INFO` & `autobahn-23.6.2/autobahn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobahn
-Version: 23.6.1
+Version: 23.6.2
 Summary: WebSocket client & server library, WAMP real-time framework
 Home-page: https://github.com/crossbario/autobahn-python
 Author: typedef int GmbH
 License: MIT License
 Project-URL: Source, https://github.com/crossbario/autobahn-python
 Keywords: autobahn crossbar websocket realtime rfc6455 wamp rpc pubsub twisted asyncio xbr data-markets blockchain ethereum
 Platform: Any
@@ -318,9 +318,7 @@
    :target: https://autobahn.readthedocs.io/en/latest/
 
 .. |Docker Images| image:: https://img.shields.io/badge/download-docker-blue.svg?style=flat
    :target: https://hub.docker.com/r/crossbario/autobahn-python/
 
 .. |EXE Download| image:: https://img.shields.io/badge/download-exe-blue.svg?style=flat
    :target: https://download.crossbario.com/xbrnetwork/linux-amd64/xbrnetwork-latest
-
-
```

### Comparing `autobahn-23.6.1/autobahn.egg-info/SOURCES.txt` & `autobahn-23.6.2/autobahn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 autobahn/asset/xbr_white.svg
 autobahn/asyncio/__init__.py
 autobahn/asyncio/component.py
 autobahn/asyncio/rawsocket.py
 autobahn/asyncio/util.py
 autobahn/asyncio/wamp.py
 autobahn/asyncio/websocket.py
+autobahn/asyncio/test/README_NO_INIT_PY
+autobahn/asyncio/test/test_aio_rawsocket.py
+autobahn/asyncio/test/test_aio_websocket.py
+autobahn/asyncio/test/test_wamp_runner.py
 autobahn/asyncio/xbr/__init__.py
 autobahn/nvx/__init__.py
 autobahn/nvx/_utf8validator.c
 autobahn/nvx/_utf8validator.py
 autobahn/nvx/test/__init__.py
 autobahn/nvx/test/test_nvx_utf8validator.py
 autobahn/rawsocket/__init__.py
```

### Comparing `autobahn-23.6.1/autobahn.egg-info/requires.txt` & `autobahn-23.6.2/autobahn.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,66 +6,45 @@
 [accelerate]
 
 [all]
 zope.interface>=5.2.0
 twisted>=20.3.0
 attrs>=20.3.0
 python-snappy>=0.6.0
-u-msgpack-python>=2.1
+msgpack>=1.0.2
+ujson>=4.0.2
 cbor2>=5.2.0
 py-ubjson>=0.16.1
 flatbuffers>=22.12.6
 pyopenssl>=20.0.1
 service_identity>=18.1.0
 pynacl>=1.4.0
 pytrie>=0.4.0
 qrcode>=7.3.1
 cffi>=1.14.5
 argon2_cffi>=20.1.0
 passlib>=1.7.4
-cffi>=1.14.5
-bitarray@ git+https://github.com/ilanschnell/bitarray.git@master#egg=bitarray
+bitarray>=2.7.5
 xbr>=21.2.1
 click>=8.1.2
-cbor2>=5.2.0
 zlmdb>=21.2.1
-twisted>=20.3.0
 web3[ipfs]>=6.0.0
 rlp>=2.0.1
 py-eth-sig-utils>=0.4.0
 py-ecc>=5.1.0
 eth-abi>=4.0.0
 mnemonic>=0.19
 base58>=2.1.0
 ecdsa>=0.16.1
 py-multihash>=2.0.1
 jinja2>=2.11.3
 yapf==0.29.0
 spake2>=0.8
 hkdf>=0.0.3
 PyGObject>=3.40.0
-bitarray@ git+https://github.com/ilanschnell/bitarray.git@master#egg=bitarray
-xbr>=21.2.1
-click>=8.1.2
-cbor2>=5.2.0
-zlmdb>=21.2.1
-twisted>=20.3.0
-web3[ipfs]>=6.0.0
-rlp>=2.0.1
-py-eth-sig-utils>=0.4.0
-py-ecc>=5.1.0
-eth-abi>=4.0.0
-mnemonic>=0.19
-base58>=2.1.0
-ecdsa>=0.16.1
-py-multihash>=2.0.1
-jinja2>=2.11.3
-yapf==0.29.0
-spake2>=0.8
-hkdf>=0.0.3
 
 [asyncio]
 
 [compress]
 python-snappy>=0.6.0
 
 [dev]
@@ -115,29 +94,30 @@
 
 [scram]
 cffi>=1.14.5
 argon2_cffi>=20.1.0
 passlib>=1.7.4
 
 [serialization]
-u-msgpack-python>=2.1
+msgpack>=1.0.2
+ujson>=4.0.2
 cbor2>=5.2.0
 py-ubjson>=0.16.1
 flatbuffers>=22.12.6
 
 [twisted]
 zope.interface>=5.2.0
 twisted>=20.3.0
 attrs>=20.3.0
 
 [ui]
 PyGObject>=3.40.0
 
 [xbr]
-bitarray@ git+https://github.com/ilanschnell/bitarray.git@master#egg=bitarray
+bitarray>=2.7.5
 xbr>=21.2.1
 click>=8.1.2
 cbor2>=5.2.0
 zlmdb>=21.2.1
 twisted>=20.3.0
 web3[ipfs]>=6.0.0
 rlp>=2.0.1
```

### Comparing `autobahn-23.6.1/requirements-dev.txt` & `autobahn-23.6.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/setup.py` & `autobahn-23.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
     cffi_modules.append('autobahn/nvx/_utf8validator.py:ffi')
 
 # https://peps.python.org/pep-0440/#direct-references
 # https://stackoverflow.com/a/63688209/884770
 extras_require_xbr = [
     # bitarray is required by eth-account, but on pypy
     # see discussion/links on https://github.com/crossbario/autobahn-python/pull/1617
-    # 'bitarray>=2.7.5',          # PSF
-    'bitarray @ git+https://github.com/ilanschnell/bitarray.git@master#egg=bitarray',
+    'bitarray>=2.7.5',          # PSF
+    # 'bitarray @ git+https://github.com/ilanschnell/bitarray.git@master#egg=bitarray',
 
     # XBR contracts and ABI file bundle
     'xbr>=21.2.1',              # Apache 2.0
 
     # CLI handling and color terminal output
     'click>=8.1.2',             # BSD license
```

### Comparing `autobahn-23.6.1/twisted/plugins/autobahn_endpoints.py` & `autobahn-23.6.2/twisted/plugins/autobahn_endpoints.py`

 * *Files identical despite different names*

### Comparing `autobahn-23.6.1/twisted/plugins/autobahn_twistd.py` & `autobahn-23.6.2/twisted/plugins/autobahn_twistd.py`

 * *Files identical despite different names*

