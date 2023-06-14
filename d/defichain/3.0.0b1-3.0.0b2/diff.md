# Comparing `tmp/defichain-3.0.0b1.tar.gz` & `tmp/defichain-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defichain-3.0.0b1.tar", last modified: Thu May  4 20:14:01 2023, max compression
+gzip compressed data, was "defichain-3.0.0b2.tar", last modified: Wed Jun 14 18:19:06 2023, max compression
```

## Comparing `defichain-3.0.0b1.tar` & `defichain-3.0.0b2.tar`

### file list

```diff
@@ -1,204 +1,207 @@
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/
--rw-rw-r--   0 executor  (1000) executor  (1000)     1066 2023-03-23 01:00:00.000000 defichain-3.0.0b1/LICENSE
--rw-rw-r--   0 executor  (1000) executor  (1000)      121 2022-12-10 21:33:06.000000 defichain-3.0.0b1/MANIFEST.in
--rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-05-04 20:14:01.230239 defichain-3.0.0b1/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     2723 2022-12-10 21:33:06.000000 defichain-3.0.0b1/README.md
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/
--rw-rw-r--   0 executor  (1000) executor  (1000)      406 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/exceptions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/exceptions/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)      427 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/hdwallet/DerivationError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)       96 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/hdwallet/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.186239 defichain-3.0.0b1/defichain/exceptions/http/
--rw-rw-r--   0 executor  (1000) executor  (1000)      199 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/BadMethod.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      249 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/BadRequest.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/Forbidden.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1978 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/HTTPStatusCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      302 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/InternalServerError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      240 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/NotFound.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3982 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/RPCErrorCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      220 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/ServiceUnavailable.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      306 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/Unauthorized.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/UnprocessableEntity.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      215 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/WrongParmeters.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      615 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/exceptions/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      430 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      110 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/addresserror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/defitxerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      116 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/deserializeerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/inputerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      103 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/keyerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      114 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/notsupported.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      124 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/rawtransactionerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/tokenerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      112 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/txbuildererror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/verifyerror.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)       93 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2149 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/account.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3808 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/hdwallet/derivations.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1198 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/hdwallet/encryption.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10519 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/hdwallet/utils.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    55798 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/wallet.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/libs/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2222 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/base58.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4356 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/bech32.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14136 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/ecc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5376 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/ripemd160.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4660 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/logger.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/mnemonic/
--rw-rw-r--   0 executor  (1000) executor  (1000)       32 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10817 2023-03-14 21:50:04.000000 defichain-3.0.0b1/defichain/mnemonic/mnemonic.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/mnemonic/wordlist/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_simplified.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_traditional.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13116 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/english.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16776 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/french.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16033 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/italian.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    26423 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/japanese.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    37832 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/korean.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13996 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/spanish.txt
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/networks/
--rw-rw-r--   0 executor  (1000) executor  (1000)       84 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/networks/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4060 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/networks/networks.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.198239 defichain-3.0.0b1/defichain/node/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2888 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/RPCErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1081 2022-12-12 22:24:40.000000 defichain-3.0.0b1/defichain/node/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.206239 defichain-3.0.0b1/defichain/node/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)    21262 2023-03-18 22:57:44.000000 defichain-3.0.0b1/defichain/node/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    53564 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/blockchain.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5563 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/control.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      856 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/generating.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14857 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8435 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12054 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/mining.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    16833 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/network.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12270 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    13718 2023-03-18 22:58:05.000000 defichain-3.0.0b1/defichain/node/modules/poolpair.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5632 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/proposals.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    40311 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/rawtransactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      144 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/spv.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2530 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10291 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8691 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/util.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    15447 2023-04-24 23:36:41.000000 defichain-3.0.0b1/defichain/node/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    86413 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/wallet.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      848 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/zmq.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6802 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/node/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2182 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/node/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4216 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/util.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.206239 defichain-3.0.0b1/defichain/ocean/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2775 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/OceanErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      806 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2357 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/connection.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.210239 defichain-3.0.0b1/defichain/ocean/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)     6077 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2458 2022-12-28 14:30:10.000000 defichain-3.0.0b1/defichain/ocean/modules/blocks.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2163 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/modules/consortium.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      641 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5499 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6104 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1464 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2492 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7224 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/poolpairs.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5362 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/prices.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1691 2023-02-14 10:46:13.000000 defichain-3.0.0b1/defichain/ocean/modules/rawTx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      697 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2405 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1588 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2360 2022-12-28 14:30:13.000000 defichain-3.0.0b1/defichain/ocean/modules/transactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2973 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/ocean.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.210239 defichain-3.0.0b1/defichain/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.214239 defichain-3.0.0b1/defichain/transactions/address/
--rw-rw-r--   0 executor  (1000) executor  (1000)      288 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4009 2023-04-29 17:23:24.000000 defichain-3.0.0b1/defichain/transactions/address/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2667 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/address/base58address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5796 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/baseaddress.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2306 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/bech32address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3320 2023-05-01 20:04:00.000000 defichain-3.0.0b1/defichain/transactions/address/p2pkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2535 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/p2sh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3073 2023-04-29 17:19:29.000000 defichain-3.0.0b1/defichain/transactions/address/p2wpkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1073 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/script.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.214239 defichain-3.0.0b1/defichain/transactions/builder/
--rw-rw-r--   0 executor  (1000) executor  (1000)       33 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.218239 defichain-3.0.0b1/defichain/transactions/builder/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)      163 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1881 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2028 2023-04-24 23:35:56.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/loans.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1341 2023-04-29 16:28:12.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/masternode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4685 2023-04-01 19:19:45.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3176 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/utxo.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:52:35.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5465 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/rawtransactionbuilder.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6932 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/txbuilder.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.218239 defichain-3.0.0b1/defichain/transactions/constants/
--rw-rw-r--   0 executor  (1000) executor  (1000)      440 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      245 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:45:28.000000 defichain-3.0.0b1/defichain/transactions/constants/defitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      382 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/fees.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/constants/mainnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)     8734 2023-04-29 16:23:23.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     9370 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     5622 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     7346 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3265 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/opcodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/rawtransactions.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/constants/testnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)    18208 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1630 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      598 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1623 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      177 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3321 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/tokens.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/defitx/
--rw-rw-r--   0 executor  (1000) executor  (1000)      300 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2010 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/builddefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2863 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/defitx/defitx.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.226239 defichain-3.0.0b1/defichain/transactions/defitx/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6516 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      672 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/basedefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7538 2023-04-13 22:18:28.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/baseinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      264 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8707 2023-04-24 23:35:56.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/loans.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6124 2023-04-29 17:26:17.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/masternode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      209 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    16975 2023-04-13 22:05:54.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      204 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     9907 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4808 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/keys.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.226239 defichain-3.0.0b1/defichain/transactions/rawtransactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      338 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      954 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1438 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/sign.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    19708 2023-04-01 19:35:42.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/tx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4252 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txbase.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14476 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    11292 2023-04-01 16:54:42.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txoutput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8303 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/witness.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/defichain/transactions/remotedata/
--rw-rw-r--   0 executor  (1000) executor  (1000)       89 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/remotedata/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1747 2023-04-30 09:04:11.000000 defichain-3.0.0b1/defichain/transactions/remotedata/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1332 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/remotedata/ocean.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1469 2023-05-01 20:06:53.000000 defichain-3.0.0b1/defichain/transactions/remotedata/remotedata.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/defichain/transactions/utils/
--rw-rw-r--   0 executor  (1000) executor  (1000)      236 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/utils/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3239 2023-04-01 17:21:08.000000 defichain-3.0.0b1/defichain/transactions/utils/calculate.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2634 2023-04-12 23:08:52.000000 defichain-3.0.0b1/defichain/transactions/utils/converter.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3017 2023-03-31 19:16:18.000000 defichain-3.0.0b1/defichain/transactions/utils/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      987 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/utils/verify.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain.egg-info/
--rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     6958 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/SOURCES.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/dependency_links.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       57 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/requires.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       10 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/top_level.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)      174 2022-12-10 21:33:06.000000 defichain-3.0.0b1/pyproject.toml
--rw-rw-r--   0 executor  (1000) executor  (1000)       56 2022-12-10 21:33:06.000000 defichain-3.0.0b1/requirements.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       38 2023-05-04 20:14:01.230239 defichain-3.0.0b1/setup.cfg
--rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-05-04 20:13:13.000000 defichain-3.0.0b1/setup.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.093278 defichain-3.0.0b2/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1066 2023-03-23 01:00:00.000000 defichain-3.0.0b2/LICENSE
+-rw-rw-r--   0 executor  (1000) executor  (1000)      121 2022-12-10 21:33:06.000000 defichain-3.0.0b2/MANIFEST.in
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-06-14 18:19:06.093278 defichain-3.0.0b2/PKG-INFO
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2723 2022-12-10 21:33:06.000000 defichain-3.0.0b2/README.md
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      406 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/exceptions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain/exceptions/hdwallet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      427 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/hdwallet/DerivationError.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)       96 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/hdwallet/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/exceptions/http/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      199 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/BadMethod.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      249 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/BadRequest.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/Forbidden.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1978 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/HTTPStatusCode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      302 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/InternalServerError.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      240 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/NotFound.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3982 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/RPCErrorCode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      220 2023-05-13 11:11:51.000000 defichain-3.0.0b2/defichain/exceptions/http/ServiceUnavailable.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      306 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/Unauthorized.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/UnprocessableEntity.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      215 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/WrongParmeters.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      615 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/exceptions/http/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/exceptions/transactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      430 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      110 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/addresserror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/defitxerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      116 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/deserializeerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/inputerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      103 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/keyerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      114 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/notsupported.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      124 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/rawtransactionerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/tokenerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      112 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/txbuildererror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/exceptions/transactions/verifyerror.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/hdwallet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       93 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2149 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/account.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3808 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/hdwallet/derivations.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1200 2023-05-31 20:38:49.000000 defichain-3.0.0b2/defichain/hdwallet/encryption.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10519 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/hdwallet/utils.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    55798 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/hdwallet/wallet.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/libs/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2222 2023-05-24 21:37:48.000000 defichain-3.0.0b2/defichain/libs/base58.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4356 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/bech32.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14136 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/ecc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5376 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/libs/ripemd160.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4660 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/logger.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.077278 defichain-3.0.0b2/defichain/mnemonic/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       32 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10817 2023-03-14 21:50:04.000000 defichain-3.0.0b2/defichain/mnemonic/mnemonic.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/mnemonic/wordlist/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_simplified.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_traditional.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13116 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/english.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16776 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/french.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16033 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/italian.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    26423 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/japanese.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    37832 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/korean.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13996 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/mnemonic/wordlist/spanish.txt
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/networks/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       84 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/networks/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4060 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/networks/networks.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.081278 defichain-3.0.0b2/defichain/node/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2990 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/RPCErrorHandler.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1081 2022-12-12 22:24:40.000000 defichain-3.0.0b2/defichain/node/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/node/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)    21262 2023-06-12 22:07:50.000000 defichain-3.0.0b2/defichain/node/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    53564 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/blockchain.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5563 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/control.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1843 2023-06-12 22:08:23.000000 defichain-3.0.0b2/defichain/node/modules/evm.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      856 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/generating.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14857 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/loan.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8435 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/masternodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    12054 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/mining.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16833 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/network.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    12270 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13718 2023-03-18 22:58:05.000000 defichain-3.0.0b2/defichain/node/modules/poolpair.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5632 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/proposals.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    40311 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/rawtransactions.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      144 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/spv.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2530 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/stats.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10291 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/tokens.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8691 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/util.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    15447 2023-04-24 23:36:41.000000 defichain-3.0.0b2/defichain/node/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    86413 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/modules/wallet.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      848 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/node/modules/zmq.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6967 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/node.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2680 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/node/rpc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4216 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/node/util.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/ocean/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2775 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/OceanErrorHandler.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      806 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2357 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/connection.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/ocean/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6077 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2458 2022-12-28 14:30:10.000000 defichain-3.0.0b2/defichain/ocean/modules/blocks.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2163 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/modules/consortium.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      641 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/fee.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5499 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/modules/governance.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6104 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/loan.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1464 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/masternodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2492 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7224 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/poolpairs.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5362 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/prices.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1691 2023-02-14 10:46:13.000000 defichain-3.0.0b2/defichain/ocean/modules/rawTx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      697 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/rpc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2405 2022-12-23 22:10:17.000000 defichain-3.0.0b2/defichain/ocean/modules/stats.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1588 2022-12-10 21:33:06.000000 defichain-3.0.0b2/defichain/ocean/modules/tokens.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2360 2022-12-28 14:30:13.000000 defichain-3.0.0b2/defichain/ocean/modules/transactions.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2973 2023-04-24 22:47:23.000000 defichain-3.0.0b2/defichain/ocean/ocean.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/address/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      288 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/address/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4009 2023-04-29 17:23:24.000000 defichain-3.0.0b2/defichain/transactions/address/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2583 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/base58address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5750 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/baseaddress.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2317 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/bech32address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3828 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2pkh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2531 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2sh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3064 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/address/p2wpkh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1073 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/address/script.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.085278 defichain-3.0.0b2/defichain/transactions/builder/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       33 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/builder/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/builder/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      220 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2683 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3231 2023-05-31 20:59:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/data.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      963 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/governance.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2228 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/loans.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1541 2023-05-05 17:22:41.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/masternode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4685 2023-04-01 19:19:45.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/pool.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5305 2023-06-14 18:09:22.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/utxo.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:52:35.000000 defichain-3.0.0b2/defichain/transactions/builder/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6021 2023-06-14 18:09:22.000000 defichain-3.0.0b2/defichain/transactions/builder/rawtransactionbuilder.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7025 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/builder/txbuilder.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      440 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      245 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:45:28.000000 defichain-3.0.0b2/defichain/transactions/constants/defitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      382 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/fees.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/mainnet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8734 2023-04-29 16:23:23.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     9370 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5622 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/LOAN_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7346 2023-03-26 16:27:39.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/STANDARD_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/mainnet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3265 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/opcodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/rawtransactions.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/constants/testnet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)    18208 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/CUSTOM_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1630 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      598 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/LOAN_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1623 2023-03-26 16:27:43.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/STANDARD_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      177 2023-04-01 23:11:49.000000 defichain-3.0.0b2/defichain/transactions/constants/testnet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3321 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/constants/tokens.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/defitx/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      300 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2010 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/builddefitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3173 2023-05-13 09:00:19.000000 defichain-3.0.0b2/defichain/transactions/defitx/defitx.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/defitx/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     9987 2023-05-13 09:19:42.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      672 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/basedefitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7538 2023-04-13 22:18:28.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/baseinput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3779 2023-05-12 14:43:35.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/governance.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8707 2023-04-24 23:35:56.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/loans.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6082 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/masternode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      209 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16975 2023-04-13 22:05:54.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/pool.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      204 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/token.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     9907 2023-04-29 16:23:24.000000 defichain-3.0.0b2/defichain/transactions/defitx/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4808 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/keys.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/rawtransactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      339 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      954 2023-06-12 21:35:44.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/fee.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1438 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/sign.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    21228 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/tx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4252 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txbase.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14476 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txinput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10971 2023-05-31 20:38:47.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/txoutput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8572 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/rawtransactions/witness.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.089278 defichain-3.0.0b2/defichain/transactions/remotedata/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       89 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/remotedata/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1747 2023-04-30 09:04:11.000000 defichain-3.0.0b2/defichain/transactions/remotedata/node.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1332 2023-04-29 16:23:24.000000 defichain-3.0.0b2/defichain/transactions/remotedata/ocean.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1469 2023-05-01 20:06:53.000000 defichain-3.0.0b2/defichain/transactions/remotedata/remotedata.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.093278 defichain-3.0.0b2/defichain/transactions/utils/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      236 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/utils/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3970 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/utils/calculate.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2633 2023-06-12 21:37:02.000000 defichain-3.0.0b2/defichain/transactions/utils/converter.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3083 2023-05-31 20:38:42.000000 defichain-3.0.0b2/defichain/transactions/utils/token.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      987 2023-03-23 01:00:00.000000 defichain-3.0.0b2/defichain/transactions/utils/verify.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-06-14 18:19:06.073278 defichain-3.0.0b2/defichain.egg-info/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/PKG-INFO
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7088 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/SOURCES.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/dependency_links.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       57 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/requires.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       10 2023-06-14 18:19:06.000000 defichain-3.0.0b2/defichain.egg-info/top_level.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)      174 2022-12-10 21:33:06.000000 defichain-3.0.0b2/pyproject.toml
+-rw-rw-r--   0 executor  (1000) executor  (1000)       56 2023-05-31 20:38:42.000000 defichain-3.0.0b2/requirements.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       38 2023-06-14 18:19:06.093278 defichain-3.0.0b2/setup.cfg
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-06-12 22:06:26.000000 defichain-3.0.0b2/setup.py
```

### Comparing `defichain-3.0.0b1/LICENSE` & `defichain-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/PKG-INFO` & `defichain-3.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `defichain-3.0.0b1/README.md` & `defichain-3.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/exceptions/http/HTTPStatusCode.py` & `defichain-3.0.0b2/defichain/exceptions/http/HTTPStatusCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/exceptions/http/RPCErrorCode.py` & `defichain-3.0.0b2/defichain/exceptions/http/RPCErrorCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/exceptions/http/__init__.py` & `defichain-3.0.0b2/defichain/exceptions/http/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/hdwallet/account.py` & `defichain-3.0.0b2/defichain/hdwallet/account.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/hdwallet/derivations.py` & `defichain-3.0.0b2/defichain/hdwallet/derivations.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/hdwallet/encryption.py` & `defichain-3.0.0b2/defichain/hdwallet/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import base64
 import hashlib
-from Crypto import Random
-from Crypto.Cipher import AES
+#from Crypto import Random
+#from Crypto.Cipher import AES
 
 
 class AESCipher(object):
 
     def __init__(self, key):
         self.bs = AES.block_size
-        self.key = hashlib.sha256(key.encode()).digest()
+        self.key = hashlib.sha256(key.encode(,).digest()
 
     def encrypt(self, raw):
         raw = self._pad(raw)
         iv = Random.new().read(AES.block_size)
         cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return base64.b64encode(iv + cipher.encrypt(raw.encode())).hex()
+        return base64.b64encode(iv + cipher.encrypt(raw.encode(,)).hex()
 
     def decrypt(self, enc):
         enc = base64.b64decode(bytes.fromhex(enc))
         iv = enc[:AES.block_size]
         cipher = AES.new(self.key, AES.MODE_CBC, iv)
         return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
```

### Comparing `defichain-3.0.0b1/defichain/hdwallet/utils.py` & `defichain-3.0.0b2/defichain/hdwallet/utils.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/hdwallet/wallet.py` & `defichain-3.0.0b2/defichain/hdwallet/wallet.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/libs/base58.py` & `defichain-3.0.0b2/defichain/libs/base58.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/libs/bech32.py` & `defichain-3.0.0b2/defichain/libs/bech32.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/libs/ecc.py` & `defichain-3.0.0b2/defichain/libs/ecc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/libs/ripemd160.py` & `defichain-3.0.0b2/defichain/libs/ripemd160.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/logger.py` & `defichain-3.0.0b2/defichain/logger.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/mnemonic.py` & `defichain-3.0.0b2/defichain/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_simplified.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_traditional.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/english.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/french.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/italian.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/japanese.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/korean.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/mnemonic/wordlist/spanish.txt` & `defichain-3.0.0b2/defichain/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/networks/networks.py` & `defichain-3.0.0b2/defichain/networks/networks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/RPCErrorHandler.py` & `defichain-3.0.0b2/defichain/node/RPCErrorHandler.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,19 @@
         self.logger = logger
 
         if self.statusCode in STATUS_CODES_WITH_ERROR:
             if self.statusCode == 401:
                 if logger:
                     self.logger.error("NodeError", f"Unauthorized")
                 raise Unauthorized()
+            if self.statusCode == 503:
+                if logger:
+                    self.logger.error("NodeError", f"ServiceUnavailable: "
+                                                   f"The service you are trying to connect to is not available")
+                raise ServiceUnavailable("The service you are trying to connect to is not available")
             else:
                 self.response_text = response.json()
                 if 'error' in self.response_text and self.response_text['error'] is not None:
                     rpc_code = self.response_text["error"]["code"]
                     rpc_name = RPCErrorCode(rpc_code).name
                     msg = self.response_text["error"]["message"]
                     if self.statusCode == 400:
@@ -46,11 +51,7 @@
                         if logger:
                             self.logger.error("NodeError", f"BadMethod: {rpc_name}: {msg}")
                         raise BadMethod(f"{rpc_name}: {msg}")
                     if self.statusCode == 500:
                         if logger:
                             self.logger.error("NodeError", f"InternalServerError: {rpc_name}: {msg}")
                         raise InternalServerError(f"{rpc_name}: {msg}")
-                    if self.statusCode == 503:
-                        if logger:
-                            self.logger.error("NodeError", f"ServiceUnavailable: {rpc_name}: {msg}")
-                        raise ServiceUnavailable(f"{rpc_name}: {msg}")
```

### Comparing `defichain-3.0.0b1/defichain/node/__init__.py` & `defichain-3.0.0b2/defichain/node/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/accounts.py` & `defichain-3.0.0b2/defichain/node/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/blockchain.py` & `defichain-3.0.0b2/defichain/node/modules/blockchain.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/control.py` & `defichain-3.0.0b2/defichain/node/modules/control.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/generating.py` & `defichain-3.0.0b2/defichain/node/modules/generating.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/loan.py` & `defichain-3.0.0b2/defichain/node/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/masternodes.py` & `defichain-3.0.0b2/defichain/node/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/mining.py` & `defichain-3.0.0b2/defichain/node/modules/mining.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/network.py` & `defichain-3.0.0b2/defichain/node/modules/network.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/oracles.py` & `defichain-3.0.0b2/defichain/node/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/poolpair.py` & `defichain-3.0.0b2/defichain/node/modules/poolpair.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/proposals.py` & `defichain-3.0.0b2/defichain/node/modules/proposals.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/rawtransactions.py` & `defichain-3.0.0b2/defichain/node/modules/rawtransactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/stats.py` & `defichain-3.0.0b2/defichain/node/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/tokens.py` & `defichain-3.0.0b2/defichain/node/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/util.py` & `defichain-3.0.0b2/defichain/node/modules/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/vault.py` & `defichain-3.0.0b2/defichain/node/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/wallet.py` & `defichain-3.0.0b2/defichain/node/modules/wallet.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/modules/zmq.py` & `defichain-3.0.0b2/defichain/node/modules/zmq.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/node/node.py` & `defichain-3.0.0b2/defichain/node/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,16 @@
             wallet_name = wallet_path
 
         # Setup URL
         self.url = f"{protocol}://{user}:{password}@{url}:{port}/wallet/{wallet_name}"
 
         # Setup all different modules
         self._rpc = RPC(self.url, logger)
+        self._logger = logger
+
         self.accounts = Accounts(self)
         self.blockchain = Blockchain(self)
         self.control = Control(self)
         self.generating = Generating(self)
         self.icxorderbook = None
         self.loan = Loan(self)
         self.masternodes = Masternodes(self)
@@ -152,11 +154,13 @@
         Tests Connection to Defichain Node and raises ServiceUnavailable exception if no connection occurred
 
         :exception: ServiceUnavailable
         """
         try:
             self.network.ping()
         except ServiceUnavailable as e:
-            raise ServiceUnavailable(f"RPC_CLIENT_INVALID_IP_OR_SUBNET: Invalid IP/Subnet {e}")
+            if self._logger:
+                self._logger.error("ConnectionError", f"RPC_CLIENT_INVALID_IP_OR_SUBNET: Invalid IP/Subnet")
+            raise ServiceUnavailable(f"RPC_CLIENT_INVALID_IP_OR_SUBNET: Invalid IP/Subnet")
 
         except Exception as e:
             raise Exception(e)
```

### Comparing `defichain-3.0.0b1/defichain/node/rpc.py` & `defichain-3.0.0b2/defichain/node/rpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import requests
 import time
 from defichain.logger import Logger
 from defichain.node.RPCErrorHandler import RPCErrorHandler
 from defichain.exceptions.http.ServiceUnavailable import ServiceUnavailable
 
 
+RPC_TIMEOUT = 60
+
+
 class RPC(object):
     def __init__(self, url, logger: Logger):
         self._session = requests.Session()
         self._url = url
         self._headers = {'content-type': 'application/json'}
         self._logger = logger
 
@@ -22,26 +25,34 @@
         payload = json.dumps({"method": rpc_method, "params": list(filtered_params), "jsonrpc": "2.0"})
         tries = 3
         hadConnectionFailures = False
 
         # Logging of Node get request url
         if self._logger:
             if self._logger.log_level == "input" or self._logger.log_level == "all":
-                self._logger.input("NodeInput", f"Node request URL: {self._url} | Headers: {self._headers} | Payload: {payload}")
+                self._logger.input("NodeInput", f"Node request URL: {self._url} | Headers: {self._headers} | Payload: "
+                                                f"{payload}")
 
         while True:
             try:
-                response = self._session.post(self._url, headers=self._headers, data=payload)
+                response = self._session.post(self._url, headers=self._headers, data=payload, timeout=RPC_TIMEOUT)
             except requests.exceptions.ConnectionError as e:
                 tries -= 1
                 if tries == 0:
-                    raise ServiceUnavailable(e)
+                    raise ServiceUnavailable("The service you are trying to connect to is not available")
                 hadFailedConnections = True
-                print(f"Couldn't connect for remote procedure call, will sleep for five seconds and then try again ({tries} more tries)")
+                print(f"Couldn't connect for remote procedure call, will sleep for five seconds and then try again "
+                      f"({tries} more tries)")
+                if self._logger:
+                    self._logger.error("ConnectionError", f"Could not connect to the Node, trying again")
                 time.sleep(5)
+            except requests.exceptions.ReadTimeout as e:
+                if self._logger:
+                    self._logger.error("ConnectionError", f"The connection timed out: {e}")
+
             else:
                 if hadConnectionFailures:
                     print('Connected for remote procedure call after retry.')
                 break
 
         RPCErrorHandler(response, self._logger)  # Check for Exceptions
```

### Comparing `defichain-3.0.0b1/defichain/node/util.py` & `defichain-3.0.0b2/defichain/node/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/OceanErrorHandler.py` & `defichain-3.0.0b2/defichain/ocean/OceanErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/__init__.py` & `defichain-3.0.0b2/defichain/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/connection.py` & `defichain-3.0.0b2/defichain/ocean/connection.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/address.py` & `defichain-3.0.0b2/defichain/ocean/modules/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/blocks.py` & `defichain-3.0.0b2/defichain/ocean/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/consortium.py` & `defichain-3.0.0b2/defichain/ocean/modules/consortium.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/fee.py` & `defichain-3.0.0b2/defichain/ocean/modules/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/governance.py` & `defichain-3.0.0b2/defichain/ocean/modules/governance.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/loan.py` & `defichain-3.0.0b2/defichain/ocean/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/masternodes.py` & `defichain-3.0.0b2/defichain/ocean/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/oracles.py` & `defichain-3.0.0b2/defichain/ocean/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/poolpairs.py` & `defichain-3.0.0b2/defichain/ocean/modules/poolpairs.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/prices.py` & `defichain-3.0.0b2/defichain/ocean/modules/prices.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/rawTx.py` & `defichain-3.0.0b2/defichain/ocean/modules/rawTx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/rpc.py` & `defichain-3.0.0b2/defichain/ocean/modules/rpc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/stats.py` & `defichain-3.0.0b2/defichain/ocean/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/tokens.py` & `defichain-3.0.0b2/defichain/ocean/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/modules/transactions.py` & `defichain-3.0.0b2/defichain/ocean/modules/transactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/ocean/ocean.py` & `defichain-3.0.0b2/defichain/ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/address/address.py` & `defichain-3.0.0b2/defichain/transactions/address/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/address/base58address.py` & `defichain-3.0.0b2/defichain/transactions/address/base58address.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,26 +31,25 @@
         return True
 
     @staticmethod
     def decode(address: str) -> str:
         return base58.decode(address).hex()
 
     @staticmethod
-    def encode(network: Any, scriptPublicKey: str) -> str:
-        return base58.check_encode(Converter.hex_to_bytes(scriptPublicKey))
+    def encode(network: Any, data: str) -> str:
+        return base58.encode(bytes.fromhex(data))
 
     @staticmethod
     def scriptPublicKey_to_address(network: Any, scriptPublicKey: str) -> str:
         Base58Address._is_scriptPublicKey(scriptPublicKey)
         if scriptPublicKey[0:6] == "76a914":  # P2PKH
             script = Converter.int_to_hex(network.PUBLIC_KEY_ADDRESS, 1) + scriptPublicKey[6:46]
-            return Base58Address.encode(network, script)
         elif scriptPublicKey[0:4] == "a914":  # P2SH
             script = Converter.int_to_hex(network.SCRIPT_ADDRESS, 1) + scriptPublicKey[4:44]
-            return Base58Address.encode(network, script)
+        return base58.check_encode(Converter.hex_to_bytes(script))
 
     @staticmethod
     def verify(address: str) -> bool:
         return Base58Address._is_base58address(address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/baseaddress.py` & `defichain-3.0.0b2/defichain/transactions/address/baseaddress.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,28 +64,28 @@
         :type address: str
         :return: "hex" (str) - the decoded address
         """
         pass
 
     @staticmethod
     @abstractmethod
-    def encode(network: Any, scriptPublicKey: str) -> str:
+    def encode(network: Any, data: str) -> str:
         """
         Encodes a script public key into an address
 
         P2PKH address: use Base58Address or P2PKH object
 
         P2SH address: use Base58Address or P2SH object
 
         P2WPKH address: use Bech32Address or P2WpKH object
 
         :param network: (required) The network witch the script public key should be encoded for
         :type network: Network
-        :param scriptPublicKey: script public key
-        :type scriptPublicKey: str
+        :param data: data
+        :type data: str
         :return: "hex" (str) - address of the given script public key
         """
         pass
 
     @staticmethod
     def scriptPublicKey_to_address(network: Any, scriptPublicKey: str) -> str:
         """
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/bech32address.py` & `defichain-3.0.0b2/defichain/transactions/address/bech32address.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,24 +28,25 @@
         result = '%x' % sum([CHARSET.find(c) * CHARSET_BASE ** i for i, c in enumerate(data)])
 
         while len(result) < 40:
             result = "0" + result
         return result
 
     @staticmethod
-    def encode(network: Any, scriptPublicKey: str) -> str:
-        binary = binascii.unhexlify(scriptPublicKey)
+    def encode(network: Any, data: str) -> str:
+        data = "0014" + data
+        binary = binascii.unhexlify(data)
         version = binary[0] - 0x50 if binary[0] else 0
         program = binary[2:]
         return bech32.encode(network.SEGWIT_ADDRESS.HRP, version, program)
 
     @staticmethod
     def scriptPublicKey_to_address(network: Any, scriptPublicKey: str) -> str:
         if scriptPublicKey[0:4] == "0014":
-            return Bech32Address.encode(network, scriptPublicKey)
+            return Bech32Address.encode(network, scriptPublicKey[4:])
 
     @staticmethod
     def verify(address: str) -> bool:
         return Bech32Address._is_bech32address(address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/p2pkh.py` & `defichain-3.0.0b2/defichain/transactions/address/p2pkh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
 
 import hashlib
 import binascii
 
+from defichain.exceptions.transactions import AddressError
 from defichain.networks import Network
 from defichain.transactions.constants import AddressTypes, OPCodes
 from defichain.transactions.keys import PrivateKey, PublicKey
 from defichain.libs import base58
 from .base58address import Base58Address
 from .script import Script
 
@@ -50,19 +51,29 @@
         :type scriptPublicKey: str
         :return: P2PKH - returns the P2PKH address object
         """
         return P2PKH(network, Base58Address.scriptPublicKey_to_address(network, scriptPublicKey))
 
     @staticmethod
     def from_publicKeyHash(network: Any, publicKeyHash: str) -> "P2PKH":
-        checksumHash = "12" + publicKeyHash
+        if network.NETWORK == "mainnet":
+            checksumHash = "12" + publicKeyHash
+        elif network.NETWORK == "testnet":
+            checksumHash = "0f" + publicKeyHash
+        else:
+            raise AddressError("The specified network is not supported")
         for _ in range(2):
             checksumHash = hashlib.sha256(binascii.unhexlify(checksumHash)).hexdigest()
         checksum = checksumHash[:8]
-        hash = "12" + publicKeyHash + checksum
+        if network.NETWORK == "mainnet":
+            hash = "12" + publicKeyHash + checksum
+        elif network.NETWORK == "testnet":
+            hash = "0f" + publicKeyHash + checksum
+        else:
+            raise AddressError("The specified network is not supported")
         address = base58.encode(bytes.fromhex(hash))
         return P2PKH(network, address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network, address)
 
     def get_addressType(self) -> str:
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/p2sh.py` & `defichain-3.0.0b2/defichain/transactions/address/p2sh.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
         :param network: (required) The network in witch the public key should be used
         :type network: Network
         :param publicKey: (required) public key
         :type publicKey: str
         :return: P2SH - returns the P2SH address object
         """
-        return P2SH(network, PublicKey(network, publicKey).p2wpkh_address())
+        return P2SH(network, PublicKey(network, publicKey).p2sh_address())
 
     @staticmethod
     def from_privateKey(network: Any, privateKey: str) -> "P2SH":
         """
         Generates a P2SH address object from the given private key
 
         :param network: (required) The network in witch the private key should be used
         :type network: Network or DefichainRegtest
         :param privateKey: (required) private key
         :type privateKey: str
         :return: P2SH - returns the P2SH address object
         """
-        return P2SH(network, PrivateKey(network, privateKey).p2wpkh_address())
+        return P2SH(network, PrivateKey(network, privateKey).p2sh_address())
 
     @staticmethod
     def from_scriptPublicKey(network: Any, scriptPublicKey: str) -> "P2SH":
         """
         Generates a P2SH address object from the given script private key
 
         :param network: (required) The network in witch the script public key should be used
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/p2wpkh.py` & `defichain-3.0.0b2/defichain/transactions/address/p2wpkh.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         :type scriptPublicKey: str
         :return: P2WPKH - returns the P2WPKH address object
         """
         return P2WPKH(network, Bech32Address.scriptPublicKey_to_address(network, scriptPublicKey))
 
     @staticmethod
     def from_publicKeyHash(network: Any, publicKeyHash: str) -> "P2WPKH":
-        address = Bech32Address.encode(network, "0014" + publicKeyHash)
+        address = Bech32Address.encode(network, publicKeyHash)
         return P2WPKH(network, address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network, address)
 
     def get_addressType(self) -> str:
         return AddressTypes.P2WPKH
```

### Comparing `defichain-3.0.0b1/defichain/transactions/address/script.py` & `defichain-3.0.0b2/defichain/transactions/address/script.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/accounts.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from defichain.transactions.defitx import UtxosToAccount, AccountToAccount
-from defichain.transactions.utils import Converter
+from defichain.transactions.defitx import UtxosToAccount, AccountToUtxos, AccountToAccount
+from defichain.transactions.utils import Converter, Calculate
 from defichain.transactions.builder.rawtransactionbuilder import RawTransactionBuilder, Transaction
 
 
 class Accounts:
 
     def __init__(self, builder):
         self._builder: RawTransactionBuilder = builder
@@ -24,14 +24,33 @@
         """
         # Convert Float to Integer
         value = Converter.float_to_int(value)
 
         defiTx = UtxosToAccount(address, value, tokenId)
         return self._builder.build_defiTx(value, defiTx, inputs)
 
+    def accounttoutxos(self, addressFrom: str, addressAmountTo: {}, inputs=[]):
+        """
+        Creates s transaction to convert tokens into utxos
+
+        :param addressFrom: (required) the defi address of sender
+        :type addressFrom: str
+        :param addressAmountTo: (required) AddressAmount
+        :type addressAmountTo:
+        :param inputs: (optional) Inputs
+        :type inputs: TxInput
+        :return: Transaction
+        """
+        # Convert Float to Integer
+        addressAmountTo = Converter.addressAmount_float_to_int(addressAmountTo)
+        value = Calculate.addressAmountSum(addressAmountTo)
+
+        defiTx = AccountToUtxos(addressFrom, value, 2)
+        return self._builder.build_defiTx(0, defiTx, inputs, addressAmountTo=addressAmountTo)
+
     def accounttoaccount(self, addressFrom: str, addressAmountTo: {}, inputs=[]) -> "Transaction":
         """
         Sends token from one address to another address
 
         :param addressFrom: (required) address from which the tokens should be sent
         :type addressFrom: str
         :param addressAmountTo: (required) addressAmount
```

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/loans.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/loans.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
         :param vaultId: (required) id of vault used for loan
         :type vaultId: str
         :param addressTo: (required) address to transfer tokens
         :type addressTo: str
         :param amounts: (required) AddressAmount
         :type amounts: str | [str]
+        :param inputs: (optional) Inputs
+        :type inputs: TxInput
+        :return: Transaction
         """
 
         # Convert Float to Integer
         if not isinstance(amounts, list):
             amounts = [amounts]
 
         convertedAmount = []
@@ -37,14 +40,17 @@
 
         :param vaultId: (required) id of vault used for loan
         :type vaultId: str
         :param addressFrom: (required) address containing repayment tokens
         :type addressFrom: str
         :param amounts: (required) AddressAmount
         :type amounts: str | [str]
+        :param inputs: (optional) Inputs
+        :type inputs: TxInput
+        :return: Transaction
         """
 
         # Convert Float to Integer
         if not isinstance(amounts, list):
             amounts = [amounts]
 
         convertedAmount = []
```

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/masternode.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/masternode.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,29 @@
         """
         Creates a transaction to create a masternode with the given operator address and time lock
 
         :param operatorAddress: (required) legacy address of the operator
         :type operatorAddress: str
         :param timeLock: (optional) time period to lock the masternode: 0 (default), 5, 10 years
         :type timeLock: int
+        :param inputs: (optional) Inputs
+        :type inputs: TxInput
+        :return: Transaction
         """
 
         defiTx = CreateMasternode(operatorAddress, timeLock)
         return self._builder.build_defiTx(1000000000, defiTx, inputs)
 
     def resignmasternode(self, masternodeId: str, inputs=[]) -> Transaction:
         """
         Creates a transaction resigning your masternode.
 
         :param masternodeId: (required) masternodeId: txid of the creation of the masternode
         :type masternodeId: str
+        :param inputs: (optional) Inputs
+        :type inputs: TxInput
+        :return: Transaction
         """
 
         defiTx = ResignMasternode(masternodeId)
         return self._builder.build_defiTx(0, defiTx, inputs)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/pool.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/utxo.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 from defichain.exceptions.transactions import TxBuilderError
-from defichain.transactions.rawtransactions import TxAddressOutput, estimate_fee
-from defichain.transactions.utils import Converter
+from defichain.transactions.rawtransactions import TxAddressOutput, TxDataOutput, estimate_fee
+from defichain.transactions.utils import Converter, Calculate
 from defichain.transactions.builder.rawtransactionbuilder import RawTransactionBuilder, Transaction
 
 
-class UTXO:
+class Data:
 
     def __init__(self, builder):
         self._builder: RawTransactionBuilder = builder
 
-    def send(self, value: "float | int", addressTo: str, changeAddress: str = None, inputs=[]) -> Transaction:
+    def hex_data(self, data: str, addressAmountTo=None, changeAddress: str = None, inputs=None) -> Transaction:
         """
-        Sends the specified amount of UTXO to the specified address. Returns the remaining UTXO from the input to the
-        sender address if not changed.
+        Creates a transaction to submit data to the blockchain
 
-        :param value: (required) amount of UTXO to send
-        :type value: float | int
-        :param addressTo: (required) address to send the UTXO to
-        :type addressTo: str
-        :param changeAddress: (optional) address to which the remaining UTXO should be sent
+        :param data: (required) hexadecimal data
+        :type data: str
+        :param addressAmountTo: (required) AddressAmount
+        :type addressAmountTo: json string
+        :param changeAddress: (required) address to which the remaining UTXO should be sent
         :type changeAddress: str
         :param inputs: (optional) Inputs
-        :type inputs: TxInputs
+        :type inputs: TxInput
         :return: Transaction
         """
+
+        if inputs is None:
+            inputs = []
+        if addressAmountTo is None:
+            addressAmountTo = {}
         if changeAddress is None:
             changeAddress = self._builder.get_address()
 
         # Convert Float to Integer
-        value = Converter.float_to_int(value)
-
-        # If to_address is the same as account address
-        if addressTo == self._builder.get_address() or addressTo == changeAddress:
-            return self.sendall(addressTo)
+        addressAmountTo = Converter.addressAmount_float_to_int(addressAmountTo)
+        outputValue = Calculate.addressAmountSum(addressAmountTo)
 
-        # If to_address is different from account address
+        # Building the transaction
         tx = self._builder.build_transactionInputs(inputs)
-        input_value = tx.get_inputsValue()
-        changeOutputValue = input_value - value
-        sendingOutput = TxAddressOutput(value, addressTo)
+        inputValue = tx.get_inputsValue()
+
+        # Building Transaction Outputs
+        messageOutput = TxDataOutput(data)
+        tx.add_output(messageOutput)
+
+        for address in addressAmountTo:
+            value, token = addressAmountTo[address].split("@")
+            addressOutput = TxAddressOutput(value, address)
+            tx.add_output(addressOutput)
+
+        changeOutputValue = inputValue - outputValue
         changeOutput = TxAddressOutput(changeOutputValue, changeAddress)
-        tx.add_output(sendingOutput)
         tx.add_output(changeOutput)
 
         # Calculate fee
         fee = estimate_fee(tx, self._builder.get_feePerByte())
 
         # Subtract fee from output
-        value = tx.get_outputs()[1].get_value() - fee
+        value = changeOutput.get_value() - fee
         if value < 0:
             raise TxBuilderError("The used address has not enough UTXO to pay the transaction fee")
-        tx.get_outputs()[1].set_value(value)
+        changeOutput.set_value(value)
 
         self._builder.sign(tx)
         return tx
 
-    def sendall(self, addressTo: str, inputs=[]) -> Transaction:
+    def str_data(self, data: str, addressAmountTo=None, changeAddress: str = None, inputs=None) -> Transaction:
         """
-        Sends all UTXO to the specified address
+        Creates a transaction to submit data to the blockchain
 
-        :param addressTo: (required) address to send the UTXO to
-        :type addressTo: str
+        :param data: (required) string data
+        :type data: str
+        :param addressAmountTo: (required) AddressAmount
+        :type addressAmountTo: json string
+        :param changeAddress: (required) address to which the remaining UTXO should be sent
+        :type changeAddress: str
         :param inputs: (optional) Inputs
         :type inputs: TxInput
         :return: Transaction
         """
-        tx = self._builder.build_transactionInputs(inputs)
-        inputValue = tx.get_inputsValue()
-        output = TxAddressOutput(inputValue, addressTo)
-        tx.add_output(output)
+        if inputs is None:
+            inputs = []
+        if addressAmountTo is None:
+            addressAmountTo = {}
 
-        # Calculate fee
-        fee = estimate_fee(tx, self._builder.get_feePerByte())
-
-        # Subtract fee from output
-        value = tx.get_outputs()[0].get_value() - fee
-        if value < 0:
-            raise TxBuilderError("The used address has not enough UTXO to pay the transaction fee")
-        tx.get_outputs()[0].set_value(value)
-
-        self._builder.sign(tx)
-        return tx
+        return self.hex_data(Converter.str_to_hex(data), addressAmountTo, changeAddress, inputs)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/modules/vault.py` & `defichain-3.0.0b2/defichain/transactions/builder/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/rawtransactionbuilder.py` & `defichain-3.0.0b2/defichain/transactions/builder/rawtransactionbuilder.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,17 +40,19 @@
                     tx.add_input(TxP2SHInput(input["txid"], input["vout"], self.get_account().get_p2wpkh(),
                                              input["value"]))
                 # Build P2WPKH Input
                 elif address.get_addressType() == AddressTypes.P2WPKH:
                     tx.add_input(TxP2WPKHInput(input["txid"], input["vout"], self.get_address(), input["value"]))
             # Check Inputs for masternode collateral
             tx.set_inputs(self.checkMasternodeInputs(tx.get_inputs()))
+        if tx.get_inputs() == []:
+            raise TxBuilderError(f"Given address: {self._address} has no unspent inputs. Check your builder object!")
         return tx
 
-    def build_defiTx(self, value: int, defiTx: BaseDefiTx, inputs=[]) -> Transaction:
+    def build_defiTx(self, value: int, defiTx: BaseDefiTx, inputs=[], **additionalData) -> Transaction:
         tx = self.build_transactionInputs(inputs)
 
         # Check for errors in Inputs
         # Check masternode creation errors
         if defiTx.get_defiTxType() == DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE:
             if tx.get_inputsValue() - value < 2000000000000:
                 raise TxBuilderError("The address holds not enough DFI to create a masternode")
@@ -66,25 +68,34 @@
         # Masternode Output
         if defiTx.get_defiTxType() == DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE:
             masternodeOutput = TxAddressOutput(2000000000000, self.get_address())
             value = masternodeOutput.get_value() + value
             tx.add_output(masternodeOutput)
 
         # Change Output
-        change_output = TxAddressOutput(tx.get_inputsValue() - value, self.get_address())
-        tx.add_output(change_output)
+        changeOutput = TxAddressOutput(tx.get_inputsValue() - value, self.get_address())
+        tx.add_output(changeOutput)
+
+        # AccountToUtxos Output
+        if defiTx.get_defiTxType() == DefiTxType.OP_DEFI_TX_ACCOUNT_TO_UTXOS:
+            addressAmountTo = additionalData["addressAmountTo"]
+
+            # Build Outputs for Utxos
+            for address in addressAmountTo:
+                outputValue = int(addressAmountTo[address].split("@")[0])
+                tx.add_output(TxAddressOutput(outputValue, address, 0))
 
         # Calculate fee
         fee = estimate_fee(tx, self.get_feePerByte())
 
         # Subtract fee from output
-        value = tx.get_outputs()[-1].get_value() - fee
+        value = changeOutput.get_value() - fee
         if value < 0:
             raise TxBuilderError("The used address has not enough UTXO to pay the transaction fee")
-        tx.get_outputs()[-1].set_value(value)
+        changeOutput.set_value(value)
 
         # Sign and Return
         self.sign(tx)
         return tx
 
     def sign(self, tx: Transaction) -> None:
         tx.sign(self.get_account().get_network(), [self.get_account().get_privateKey()])
```

### Comparing `defichain-3.0.0b1/defichain/transactions/builder/txbuilder.py` & `defichain-3.0.0b2/defichain/transactions/builder/txbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,21 @@
         self._set_dataSource(dataSource)
         self._set_feePerByte(feePerByte)
 
         self._builder = RawTransactionBuilder(self.get_address(), self.get_account(), self.get_dataSource(),
                                               self.get_feePerByte())
 
         self.utxo = UTXO(self._builder)
+        self.data = Data(self._builder)
+
         self.accounts = Accounts(self._builder)
-        self.loan = Loans(self._builder)
+        self.governance = Governance(self._builder)
+        self.loans = Loans(self._builder)
         self.masternode = Masternode(self._builder)
         self.pool = Pool(self._builder)
-
         self.vault = Vault(self._builder)
 
         # Verify if address is represented by provided account
         self._verify()
 
     # Methods
     def send_tx(self, tx: "Transaction | str", maxFeeRate: float = None) -> str:
```

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/defitx.py` & `defichain-3.0.0b2/defichain/transactions/constants/defitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/mainnet/CUSTOM_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/mainnet/LOAN_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/mainnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/mainnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/opcodes.py` & `defichain-3.0.0b2/defichain/transactions/constants/opcodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/testnet/CUSTOM_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/testnet/LOAN_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/testnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/testnet/STANDARD_tokens.json` & `defichain-3.0.0b2/defichain/transactions/constants/testnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/constants/tokens.py` & `defichain-3.0.0b2/defichain/transactions/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/builddefitx.py` & `defichain-3.0.0b2/defichain/transactions/defitx/builddefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/defitx.py` & `defichain-3.0.0b2/defichain/transactions/defitx/defitx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
 
 from defichain.exceptions.transactions import NotYetSupportedError
 from defichain.transactions.constants import DefiTx_SIGNATURE
 from .modules.accounts import *
+from .modules.governance import *
 from .modules.loans import *
 from .modules.masternode import *
 from .modules.pool import *
 
 from .modules.vault import *
 
 
@@ -33,17 +34,23 @@
 
         defiTxType = hex[position: position + 2]
         position += 2
 
         # Account
         if DefiTxType.OP_DEFI_TX_UTXOS_TO_ACCOUNT == defiTxType:
             return UtxosToAccount.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_ACCOUNT_TO_UTXOS == defiTxType:
+            return AccountToUtxos.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_ACCOUNT_TO_ACCOUNT == defiTxType:
             return AccountToAccount.deserialize(network, hex[position:])
 
+        # Governance
+        elif DefiTxType.OP_DEFI_TX_VOTE == defiTxType:
+            return Vote.deserialize(network, hex[position:])
+
         # Loans
         elif DefiTxType.OP_DEFI_TX_TAKE_LOAN == defiTxType:
             return TakeLoan.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_PAYBACK_LOAN == defiTxType:
             return PaybackLoan.deserialize(network, hex[position:])
 
         # Masternode
```

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/basedefitx.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/basedefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/baseinput.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/baseinput.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/loans.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/loans.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/masternode.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/masternode.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         self.set_operatorAddress(operatorAddress)
         self.set_timeLock(timeLock)
 
     def __bytes__(self) -> bytes:
         # Convert to Bytes
         defiTxType = Converter.hex_to_bytes(self.get_defiTxType())
 
-        print(self.get_operatorAddress())
         if Address.from_address(self.get_operatorAddress()).get_addressType() == AddressTypes.P2PKH:
             operatorType = Converter.int_to_bytes(1, 1)
             operatorPubKeyHash = P2PKH(Address.from_address(self.get_operatorAddress()).get_network(),
                                        self.get_operatorAddress()).get_publicKeyHash()
         else:
             operatorType = Converter.int_to_bytes(4, 1)
             operatorPubKeyHash = P2WPKH(Address.from_address(self.get_operatorAddress()).get_network(),
```

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/pool.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/defitx/modules/vault.py` & `defichain-3.0.0b2/defichain/transactions/defitx/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/keys.py` & `defichain-3.0.0b2/defichain/transactions/keys.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/fee.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/sign.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/sign.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/tx.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/tx.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import Any
 
 from defichain.exceptions.transactions import RawTransactionError, NotYetSupportedError, DeserializeError
 from defichain.networks import Network
 from defichain.transactions.address import Address
 from defichain.transactions.keys import PrivateKey, KeyError, PublicKey
 from defichain.transactions.utils import Converter, Calculate
-from defichain.transactions.constants import SIGHASH
+from defichain.transactions.constants import SIGHASH, AddressTypes
 
 from .txbase import TxBase
 from .txinput import TxBaseInput, TxInput, TxP2PKHInput, TxP2SHInput, TxP2WPKHInput, TxCoinbaseInput
-from .txoutput import TxBaseOutput, TxOutput, TxAddressOutput, TxMsgOutput, TxDefiOutput, TxCoinbaseOutput
+from .txoutput import TxBaseOutput, TxOutput, TxAddressOutput, TxDataOutput, TxDefiOutput, TxCoinbaseOutput
 from .witness import WitnessHash, Witness
 from .sign import sign_input
 
 
 class BaseTransaction(TxBase, ABC):
 
     def __init__(self, inputs: [], outputs: [], lockTime: int = 0):
@@ -76,14 +76,32 @@
         for outputs in self.get_outputs():
             result += outputs.get_value()
         return result
 
     def get_fee(self) -> "int | None":
         return self.get_inputsValue() - self.get_outputsValue() if self.get_inputsValue() is not None else None
 
+    def get_unspent(self) -> [TxInput]:
+        outputs = self.get_outputs()
+        unspent = []
+        vout = 0
+        for output in outputs:
+            if isinstance(output, TxAddressOutput):
+                addressType = Address.from_address(output.get_address()).get_addressType()
+
+                if addressType == AddressTypes.P2PKH:
+                    unspent.append(TxP2PKHInput(self.get_txid(), vout))
+                elif addressType == AddressTypes.P2SH:
+                    unspent.append(TxP2SHInput(self.get_txid(), vout, output.get_address(), output.get_value()))
+                elif addressType == AddressTypes.P2WPKH:
+                    unspent.append(TxP2WPKHInput(self.get_txid(), vout, output.get_address(), output.get_value()))
+
+            vout += 1
+        return unspent
+
     # Get Information
     def get_version(self) -> int:
         return self._version
 
     def get_marker(self) -> int:
         return self._marker
 
@@ -228,15 +246,15 @@
         Limitations: Not all raw transactions can be deserialized for now. For example, it's not possible to deserialize
         multi signature transactions.
 
         :param network: (required) the corresponding network from the raw transaction
         :type network: Network
         :param hex: (required) the raw transaction as hexadecimal sting
         :type hex: str
-        :return: "Transaction"
+        :return: Transaction
         """
         try:
             tx = Transaction([], [])
             position = 0
 
             # Set Version
             version = Converter.hex_to_int(hex[position: position + 8])
@@ -419,16 +437,22 @@
 
         return result
 
     def sign(self, network: Any, private_keys: [str]) -> "Transaction":
         """
         Signs the raw transaction with the given private keys
 
-        :param: key: private key can be in wif or hex format
-        :return: None
+        :param network: (required) the corresponding network from the raw transaction
+        :type network: Network
+        :param private_keys: (required) a list of private keys. If there is only one private key in the list, it will
+        be used to sign all inputs of the transaction. If you have inputs witch use different private keys, provide a
+        separate private key for every input in the list. The private keys have to be provided in the same
+        order as the inputs
+        :type private_keys: [str]
+        :return: Transaction
         """
         if not isinstance(private_keys, list):
             raise RawTransactionError("The given private keys have to be parsed in a list: [key, key, ...]")
 
         # Check if wif and calc hexadecimal private key
         keys = []
         for key in private_keys:
@@ -436,32 +460,41 @@
                 key = PrivateKey(network, privateKey=key)
             elif PrivateKey.is_wif(network, key):
                 key = PrivateKey(network, wif=key)
             else:
                 raise KeyError("Given private key is not valid")
             keys.append({"private": key.get_privateKey(), "public": key.get_publicKey()})
 
-        # Assign private and public keys to the correct input
+        # Sign
+        index = 0
         for input in self.get_inputs():
             if isinstance(input, TxP2PKHInput):
                 raise NotYetSupportedError()
-            if not input._private_key:
-                for key in keys:
-                    priv = PrivateKey(network, key["private"])
-                    if input.get_address() in [priv.p2sh_address(), priv.p2wpkh_address(), priv.p2sh_address()]:
-                        input._private_key = key["private"]
-                        input._publicKey = key["public"]
+            elif isinstance(input, TxP2WPKHInput) or isinstance(input, TxP2SHInput):
+                if len(private_keys) == 1:
+                    privKey = keys[0]["private"]
+                    pubKey = keys[0]["public"]
+                else:
+                    if len(private_keys) <= index:
+                        raise RawTransactionError("The transaction could not from be signed. Not enough private keys "
+                                                  "were provided in the list")
+                    else:
+                        privKey = keys[index]["private"]
+                        pubKey = keys[index]["public"]
+
+                witness_hash = WitnessHash(self, input)
+                signature = sign_input(privKey, witness_hash.bytes_hash())
+                witness = Witness(signature, pubKey)
+                input.set_witness(witness)
 
-        # Sign the inputs with the given keys
-        for input in self.get_inputs():
-            witness_hash = WitnessHash(self, input)
-            signature = sign_input(input._private_key, witness_hash.bytes_hash())
-            witness = Witness(signature, input._publicKey)
-            input.set_witness(witness)
+            else:
+                raise NotYetSupportedError()
+            index += 1
         self._signed = True
+
         return self
 
     def _analyse(self):
         # Analyse Inputs
         signed = None
         for input in self.get_inputs():
             if isinstance(input, TxP2WPKHInput) or isinstance(input, TxP2SHInput):
```

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/txbase.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/txbase.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/txinput.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/txinput.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/txoutput.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/txoutput.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         self.set_tokenId(Converter.bytes_to_int(tokenId))
 
 
 class TxOutput(TxBaseOutput):
     @staticmethod
     def deserialize(network: Any, hex: str) -> "TxOutput":
         """
-        Deserializes a transaction output into an output object: TxAddressOutput | TxMsgOutput | TxDefiOutput |
+        Deserializes a transaction output into an output object: TxAddressOutput | TxDataOutput | TxDefiOutput |
         TxCoinbaseOutput.
 
         :param network: (required) the corresponding network from the raw transaction
         :type network: Network
         :param hex: (required) the raw transaction output as hexadecimal sting
         :type hex: str
         :return: "TxInput"
@@ -107,15 +107,15 @@
         output = TxBaseOutput.deserialize(network, hex)
         if output.get_script()[0: 2] == OPCodes.OP_RETURN:
             if DefiTx_SIGNATURE in output.get_script()[4: 16]:
                 return TxDefiOutput.deserialize(network, hex)
             elif output.get_script()[4: 12] == "aa21a9ed":
                 return TxCoinbaseOutput.deserialize(network, hex)
             else:
-                return TxMsgOutput.deserialize(network, hex)
+                return TxDataOutput.deserialize(network, hex)
         if len(output.get_script()) > 0:
             return TxAddressOutput.deserialize(network, hex)
         return output
 
     def __init__(self, value: int, script: str, tokenId: int):
         """
         Output to spend the specified inputs UTXO
@@ -183,74 +183,64 @@
         self._address = address.get_address()
         self.set_script(address.get_scriptPublicKey())
 
     def set_bytes_address(self, address: bytes) -> None:
         self.set_address(Converter.bytes_to_hex(address))
 
 
-class TxMsgOutput(TxOutput):
+class TxDataOutput(TxOutput):
 
     @staticmethod
-    def deserialize(network: Any, hex: str) -> "TxMsgOutput":
+    def deserialize(network: Any, hex: str) -> "TxDataOutput":
         output = TxBaseOutput.deserialize(network, hex)
         OP_Code = output.get_script()[0: 2]
         if OP_Code != OPCodes.OP_RETURN:
             raise DeserializeError("The given output to decode is not an message output (there is not OP_RETURN)")
         length_script = Converter.hex_to_int(output.get_script()[2: 4]) * 2
-        msg = Converter.hex_to_str(output.get_script()[4: 4 + length_script])
-        txMsgOutput = TxMsgOutput(msg=msg, tokenId=output.get_tokenId())
-        txMsgOutput.set_value(output.get_value())
-        return txMsgOutput
+        data = Converter.hex_to_str(output.get_script()[4: 4 + length_script])
+        txDataOutput = TxDataOutput(data=data, tokenId=output.get_tokenId())
+        txDataOutput.set_value(output.get_value())
+        return txDataOutput
 
-    def __init__(self, msg: str, tokenId: int = 0):
+    def __init__(self, data: str, tokenId: int = 0):
         """
-        An output witch includes a message.
+        An output witch includes a data.
 
-        Uses OP_RETURN Code.
-        TODO: Is limited to around 200 bytes
-
-        :param msg: (required) your text in plane text like "Hello Defichain Community!"
-        :type msg: str
+        :param data: (required) your data in hex encoding
+        :type data: str
         :param tokenId: (optional) which token you want to send (almost always 0 -> stands for DFI)
         :type tokenId: int
         """
-        self._msg = None
-        self.set_msg(msg)
-        super().__init__(0, self.get_customScript(), tokenId)
+        self._data = None
+        self.set_data(data)
+        super().__init__(0, self.get_script(), tokenId)
 
     # Get Information
-    def get_msg(self) -> str:
-        return self._msg
-
-    def get_customScript(self) -> str:
-        return Converter.bytes_to_hex(Script.custom_script(self.get_msg()))
+    def get_data(self) -> str:
+        return self._data
 
-    def get_bytes_customScript(self) -> bytes:
-        return Converter.hex_to_bytes(self.get_customScript())
-
-    def get_hex_msg(self) -> str:
-        return Converter.str_to_hex(self.get_msg())
+    def get_script(self) -> str:
+        op_return = OPCodes.OP_RETURN
+        data = Converter.str_to_hex(self.get_data())
+        lengthData = Calculate.write_compactSize(int(len(data) / 2))
+        return op_return + lengthData + data
 
     def to_json(self) -> {}:
         json = {}
-        json.update({"outputType": "msg"})
+        json.update({"outputType": "data"})
         json.update({"value": self.get_value()})
-        json.update({"rawMsg": self.get_hex_msg()})
-        json.update({"decodesMsg": self.get_msg()})
+        json.update({"rawData": self.get_data()})
         json.update({"script": self.get_script()})
         json.update({"tokenId": self.get_tokenId()})
         return json
 
     # Set Information
-    def set_msg(self, msg: str) -> None:
-        self._msg = msg
-        self.set_script(self.get_customScript())
-
-    def set_hex_msg(self, msg: str) -> None:
-        self.set_msg(Converter.hex_to_str(msg))
+    def set_data(self, data: str) -> None:
+        self._data = data
+        self.set_script(self.get_script())
 
 
 class TxDefiOutput(TxOutput):
     """
     An Output witch includes a defi transaction.
 
     For example a "Poolswap" or "AddPoolLiquidity"
```

### Comparing `defichain-3.0.0b1/defichain/transactions/rawtransactions/witness.py` & `defichain-3.0.0b2/defichain/transactions/rawtransactions/witness.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 from abc import ABC
 from typing import Any
 
 from defichain.exceptions.transactions import RawTransactionError
 from defichain.transactions.utils import Converter, Calculate
 from defichain.transactions.address.address import Address
 from defichain.transactions.rawtransactions.txbase import TxBase
-from defichain.transactions.rawtransactions.txinput import TxP2WPKHInput
+from defichain.transactions.rawtransactions.txinput import TxP2WPKHInput, TxP2SHInput
 from defichain.transactions.rawtransactions.txoutput import TxBaseOutput
 
 
 class WitnessHashBase(TxBase, ABC):
 
     # Get Information
     @staticmethod
-    def get_txid_from_input(input: TxP2WPKHInput) -> str:
+    def get_txid_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> str:
         return input.get_txid()
 
     @staticmethod
-    def get_index_from_input(input: TxP2WPKHInput) -> int:
+    def get_index_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> int:
         return input.get_vout()
 
     @staticmethod
-    def get_sequence_from_input(input: TxP2WPKHInput) -> str:
+    def get_sequence_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> str:
         return input.get_sequence()
 
     @staticmethod
-    def get_address_from_input(input: TxP2WPKHInput) -> str:
+    def get_address_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> str:
         return input.get_address()
 
     @staticmethod
-    def get_value_from_input(input: TxP2WPKHInput) -> int:
+    def get_value_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> int:
         return input.get_value()
 
     @staticmethod
-    def get_bytes_txid_from_input(input: TxP2WPKHInput) -> bytes:
+    def get_bytes_txid_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return input.get_bytes_txid()
 
     @staticmethod
-    def get_bytes_index_from_input(input: TxP2WPKHInput) -> bytes:
+    def get_bytes_index_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return input.get_bytes_vout()
 
     @staticmethod
-    def get_bytes_sequence_from_input(input: TxP2WPKHInput) -> bytes:
+    def get_bytes_sequence_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return input.get_bytes_sequence()
 
     @staticmethod
-    def get_bytes_address_from_input(input: TxP2WPKHInput) -> bytes:
+    def get_bytes_address_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return input.get_bytes_address()
 
     @staticmethod
-    def get_bytes_value_from_input(input: TxP2WPKHInput) -> bytes:
+    def get_bytes_value_from_input(input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return input.get_bytes_value()
 
-    def __init__(self, tx, input: TxP2WPKHInput):
+    def __init__(self, tx, input: "TxP2WPKHInput | TxP2SHInput"):
         self._tx, self._input = None, None
         self.set_tx(tx)
         self.set_input(input)
 
     def hash(self) -> str:
         return Converter.bytes_to_hex(self.bytes())
 
     def bytes_hash(self) -> bytes:
         return self.bytes()
 
     # Get Information
     def get_transaction(self) -> TxBase:
         return self._tx
 
-    def get_input(self) -> TxP2WPKHInput:
+    def get_input(self) -> "TxP2WPKHInput | TxP2SHInput":
         return self._input
 
     def get_version(self) -> int:
         return self._tx.get_version()
 
-    def get_inputs(self) -> [TxP2WPKHInput]:
+    def get_inputs(self) -> ["TxP2WPKHInput | TxP2SHInput"]:
         return self._tx.get_inputs()
 
     def get_outputs(self) -> [TxBaseOutput]:
         return self._tx.get_outputs()
 
     def get_redeemScript(self) -> str:
         return Address.from_address(self.get_address_from_input(self.get_input())).get_redeemScript()
@@ -116,19 +116,19 @@
         }
         return result
 
     # Set Information
     def set_tx(self, tx) -> None:
         self._tx = tx
 
-    def set_input(self, input: TxP2WPKHInput) -> None:
+    def set_input(self, input: "TxP2WPKHInput | TxP2SHInput") -> None:
         self._input = input
 
     # Calc Information
-    def outpoint(self, input: TxP2WPKHInput) -> bytes:
+    def outpoint(self, input: "TxP2WPKHInput | TxP2SHInput") -> bytes:
         return self.get_bytes_txid_from_input(input) + self.get_bytes_index_from_input(input)
 
     def hash_prevOuts(self) -> bytes:
         outpoint = b''
         for input in self.get_inputs():
             outpoint += self.outpoint(input)
         return Calculate.dHash256(outpoint)
@@ -192,15 +192,15 @@
 
 class WitnessHash(WitnessHashBase):
 
     @staticmethod
     def deserialize(network: Any, hex: str) -> "WitnessHash":
         raise RawTransactionError("The witness hash cannot be deserialized")
 
-    def __init__(self, tx, input: TxP2WPKHInput):
+    def __init__(self, tx, input: "TxP2WPKHInput | TxP2SHInput"):
         super().__init__(tx, input)
 
     def __bytes__(self) -> bytes:
         result = self.get_bytes_version()
         result += self.hash_prevOuts()
         result += self.hash_sequences()
         result += self.outpoint(self.get_input())
```

### Comparing `defichain-3.0.0b1/defichain/transactions/remotedata/node.py` & `defichain-3.0.0b2/defichain/transactions/remotedata/node.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/remotedata/ocean.py` & `defichain-3.0.0b2/defichain/transactions/remotedata/ocean.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/remotedata/remotedata.py` & `defichain-3.0.0b2/defichain/transactions/remotedata/remotedata.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain/transactions/utils/calculate.py` & `defichain-3.0.0b2/defichain/transactions/utils/calculate.py`

 * *Files 22% similar despite different names*

```diff
@@ -90,13 +90,32 @@
         elif hex[0:2] == "fe":
             return int.from_bytes(bytes.fromhex(hex[2:10]), byteorder="little")
         elif hex[0:2] == "ff":
             return int.from_bytes(bytes.fromhex(hex[2:18]), byteorder="little")
         else:
             return int.from_bytes(bytes.fromhex(hex), byteorder="little")
 
+    @staticmethod
+    def addressAmountSum(addressAmount: {}) -> "int | float":
+        resultValue = 0
+        for address in addressAmount:
+            if isinstance(addressAmount[address], list):
+                for amount in addressAmount[address]:
+                    value, token = amount.split('@')
+                    if "." in value:
+                        resultValue += float(value)
+                    else:
+                        resultValue += int(value)
+            else:
+                value, token = addressAmount[address].split('@')
+                if "." in value:
+                    resultValue += float(value)
+                else:
+                    resultValue += int(value)
+        return resultValue
+
 
 if __name__ == "__main__":
     c = Calculate.write_varInt(2 ** 32)
     print(c)
     print(Calculate.read_varInt(c))
     print(2**32)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/utils/converter.py` & `defichain-3.0.0b2/defichain/transactions/utils/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
                     value = Converter.float_to_int(float(value))
                     newAddressAmount.add(address, token, value)
             else:
                 value, token = addressAmount[address].split('@')
                 value = Converter.float_to_int(float(value))
                 newAddressAmount.add(address, token, value)
         return newAddressAmount.build()
-
```

### Comparing `defichain-3.0.0b1/defichain/transactions/utils/token.py` & `defichain-3.0.0b2/defichain/transactions/utils/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     def get_id_from_symbol(network: Any, symbol: str) -> int:
         for _type in Token.TOKEN_TYPES:
             tokens = Token._get_tokens(network, _type)
             for token in tokens:
                 if _type == TokenTypes.LIQUIDITY:
                     if token["symbol"] == str(symbol):
                         return int(token["id"])
-                    elif token["symbol"] == str(f"{symbol.split('-')[1]}-{symbol.split('-')[0]}"):
-                        return int(token["id"])
+                    elif len(symbol.split("-")) > 1:
+                        if token["symbol"] == str(f"{symbol.split('-')[1]}-{symbol.split('-')[0]}"):
+                            return int(token["id"])
                 if token["symbol"] == str(symbol):
                     return int(token["id"])
         raise TokenError(f"The given symbol: {symbol} does not exist. Check your input.")
 
     @staticmethod
     def get_name_from_id(network: Any, tokenId: int) -> str:
         for _type in Token.TOKEN_TYPES:
@@ -62,13 +63,13 @@
         try:
             Token.get_name_from_id(network, tokenId)
             return True
         except:
             raise TokenError("The given token id is not valid")
 
     @staticmethod
-    def checkAndConvert(network: Any, tokenId: "int | str"):
+    def checkAndConvert(network: Any, tokenId: "int | str") -> int:
         if isinstance(tokenId, str) and not Verify.is_only_number_str(tokenId):
             return int(Token.get_id_from_symbol(network, tokenId))
         else:
             Token.verify_tokenId(network, tokenId)
             return int(tokenId)
```

### Comparing `defichain-3.0.0b1/defichain/transactions/utils/verify.py` & `defichain-3.0.0b2/defichain/transactions/utils/verify.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b1/defichain.egg-info/PKG-INFO` & `defichain-3.0.0b2/defichain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `defichain-3.0.0b1/defichain.egg-info/SOURCES.txt` & `defichain-3.0.0b2/defichain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 defichain/node/__init__.py
 defichain/node/node.py
 defichain/node/rpc.py
 defichain/node/util.py
 defichain/node/modules/accounts.py
 defichain/node/modules/blockchain.py
 defichain/node/modules/control.py
+defichain/node/modules/evm.py
 defichain/node/modules/generating.py
 defichain/node/modules/loan.py
 defichain/node/modules/masternodes.py
 defichain/node/modules/mining.py
 defichain/node/modules/network.py
 defichain/node/modules/oracles.py
 defichain/node/modules/poolpair.py
@@ -115,14 +116,16 @@
 defichain/transactions/address/p2wpkh.py
 defichain/transactions/address/script.py
 defichain/transactions/builder/__init__.py
 defichain/transactions/builder/rawtransactionbuilder.py
 defichain/transactions/builder/txbuilder.py
 defichain/transactions/builder/modules/__init__.py
 defichain/transactions/builder/modules/accounts.py
+defichain/transactions/builder/modules/data.py
+defichain/transactions/builder/modules/governance.py
 defichain/transactions/builder/modules/loans.py
 defichain/transactions/builder/modules/masternode.py
 defichain/transactions/builder/modules/pool.py
 defichain/transactions/builder/modules/utxo.py
 defichain/transactions/builder/modules/vault.py
 defichain/transactions/constants/__init__.py
 defichain/transactions/constants/address.py
```

### Comparing `defichain-3.0.0b1/setup.py` & `defichain-3.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from os import path
 
-VERSION = '3.0.0b1'
+VERSION = '3.0.0b2'
 DESCRIPTION = 'Defichain Python Library'
 
 # Project URLs
 project_urls = {
     "Tracker": "https://github.com/eric-volz/DefichainPython",
     "Documentation": "https://docs.defichain-python.de"
 }
```

